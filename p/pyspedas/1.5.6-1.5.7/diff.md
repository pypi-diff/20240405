# Comparing `tmp/pyspedas-1.5.6.tar.gz` & `tmp/pyspedas-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspedas-1.5.6.tar", last modified: Tue Feb 20 06:54:23 2024, max compression
+gzip compressed data, was "pyspedas-1.5.7.tar", last modified: Fri Apr  5 16:50:20 2024, max compression
```

## Comparing `pyspedas-1.5.6.tar` & `pyspedas-1.5.7.tar`

### file list

```diff
@@ -1,802 +1,814 @@
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.687806 pyspedas-1.5.6/
--rw-r--r--   0 jwl        (501) wheel        (0)     3332 2024-02-20 06:53:32.000000 pyspedas-1.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 jwl        (501) wheel        (0)     5749 2024-02-20 06:53:32.000000 pyspedas-1.5.6/CONTRIBUTING.md
--rw-r--r--   0 jwl        (501) wheel        (0)     1109 2024-02-20 06:53:32.000000 pyspedas-1.5.6/LICENSE.txt
--rw-r--r--   0 jwl        (501) wheel        (0)      335 2024-02-20 06:53:32.000000 pyspedas-1.5.6/MANIFEST.in
--rw-r--r--   0 jwl        (501) wheel        (0)    14462 2024-02-20 06:54:23.687660 pyspedas-1.5.6/PKG-INFO
--rw-r--r--   0 jwl        (501) wheel        (0)    13805 2024-02-20 06:53:32.000000 pyspedas-1.5.6/README.md
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.612874 pyspedas-1.5.6/pyspedas/
--rw-r--r--   0 jwl        (501) wheel        (0)     5799 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.613797 pyspedas-1.5.6/pyspedas/ace/
--rw-r--r--   0 jwl        (501) wheel        (0)    23202 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ace/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      399 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ace/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3103 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ace/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.614008 pyspedas-1.5.6/pyspedas/ace/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ace/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1962 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ace/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.614362 pyspedas-1.5.6/pyspedas/akebono/
--rw-r--r--   0 jwl        (501) wheel        (0)    14718 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/akebono/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      421 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/akebono/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2108 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/akebono/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.614565 pyspedas-1.5.6/pyspedas/akebono/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/akebono/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1141 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/akebono/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.616347 pyspedas-1.5.6/pyspedas/analysis/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6581 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/avg_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1904 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/deriv_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)      860 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/dpwrspc.py
--rw-r--r--   0 jwl        (501) wheel        (0)    24049 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/find_magnetic_nulls.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7839 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/lingradest.py
--rw-r--r--   0 jwl        (501) wheel        (0)    21664 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/neutral_sheet.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1634 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tdeflag.py
--rw-r--r--   0 jwl        (501) wheel        (0)      835 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tdpwrspc.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.616865 pyspedas-1.5.6/pyspedas/analysis/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5286 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tests/test_magnetic_nulls.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4705 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tests/test_twavpol.py
--rw-r--r--   0 jwl        (501) wheel        (0)    10987 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tests/tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2061 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/time_domain_filter.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3477 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tinterpol.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2055 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/tvectot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    31210 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/twavpol.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2870 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/wavelet.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2168 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/analysis/yclip.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.617239 pyspedas-1.5.6/pyspedas/barrel/
--rw-r--r--   0 jwl        (501) wheel        (0)    10483 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/barrel/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3469 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/barrel/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2592 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/barrel/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.617469 pyspedas-1.5.6/pyspedas/barrel/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/barrel/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      292 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/barrel/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.617973 pyspedas-1.5.6/pyspedas/cdagui/
--rw-r--r--   0 jwl        (501) wheel        (0)      121 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cdagui/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17376 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cdagui/cdagui.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6166 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cdagui/cdaweb.py
--rw-r--r--   0 jwl        (501) wheel        (0)      234 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cdagui/config.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.618561 pyspedas-1.5.6/pyspedas/cluster/
--rw-r--r--   0 jwl        (501) wheel        (0)    31937 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      419 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6106 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/load.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8563 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/load_csa.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.618822 pyspedas-1.5.6/pyspedas/cluster/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3129 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cluster/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.619254 pyspedas-1.5.6/pyspedas/cnofs/
--rw-r--r--   0 jwl        (501) wheel        (0)     7645 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cnofs/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cnofs/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1916 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cnofs/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.619470 pyspedas-1.5.6/pyspedas/cnofs/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cnofs/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1017 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cnofs/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.621467 pyspedas-1.5.6/pyspedas/cotrans/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1374 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/cart2spc.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3999 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)      227 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/cotrans_get_coord.py
--rw-r--r--   0 jwl        (501) wheel        (0)    30626 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/cotrans_lib.py
--rw-r--r--   0 jwl        (501) wheel        (0)      241 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/cotrans_set_coord.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2226 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/fac_matrix_make.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2327 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/gsm2lmn.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17808 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/igrf.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13130 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/j2000.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5141 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/matrix_array_lib.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1902 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/minvar.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2244 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/minvar_matrix_make.py
--rw-r--r--   0 jwl        (501) wheel        (0)    25354 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/quaternions.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1107 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/sm2mlt.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1199 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/spc2cart.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.622038 pyspedas-1.5.6/pyspedas/cotrans/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12066 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/tests/cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1235 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/tests/quaternions.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2141 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/tests/test_minvar.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3025 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/tvector_rotate.py
--rw-r--r--   0 jwl        (501) wheel        (0)      847 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/cotrans/xyz_to_polar.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.622502 pyspedas-1.5.6/pyspedas/csswe/
--rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/csswe/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/csswe/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3613 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/csswe/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.622779 pyspedas-1.5.6/pyspedas/csswe/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/csswe/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      617 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/csswe/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.623256 pyspedas-1.5.6/pyspedas/de2/
--rw-r--r--   0 jwl        (501) wheel        (0)    19125 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/de2/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      407 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/de2/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5044 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/de2/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.623525 pyspedas-1.5.6/pyspedas/de2/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/de2/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1945 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/de2/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.623966 pyspedas-1.5.6/pyspedas/dscovr/
--rw-r--r--   0 jwl        (501) wheel        (0)     9992 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/dscovr/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      408 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/dscovr/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4522 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/dscovr/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.624248 pyspedas-1.5.6/pyspedas/dscovr/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/dscovr/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1410 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/dscovr/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.624732 pyspedas-1.5.6/pyspedas/elfin/
--rw-r--r--   0 jwl        (501) wheel        (0)    17552 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      400 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/config.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.625026 pyspedas-1.5.6/pyspedas/elfin/eng/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/eng/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3488 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/eng/eng.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.626051 pyspedas-1.5.6/pyspedas/elfin/epd/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11396 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/calibration_l1.py
--rw-r--r--   0 jwl        (501) wheel        (0)    16661 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/calibration_l2.py
--rw-r--r--   0 jwl        (501) wheel        (0)      456 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/ela_epde_cal_data.txt
--rw-r--r--   0 jwl        (501) wheel        (0)     1355 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/elb_epde_cal_data.txt
--rw-r--r--   0 jwl        (501) wheel        (0)     7962 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/epd.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6642 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/epd/postprocessing.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.626326 pyspedas-1.5.6/pyspedas/elfin/fgm/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/fgm/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3341 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/fgm/fgm.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3231 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.626602 pyspedas-1.5.6/pyspedas/elfin/mrma/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/mrma/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3073 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/mrma/mrma.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.626854 pyspedas-1.5.6/pyspedas/elfin/mrmi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/mrmi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3053 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/mrmi/mrmi.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.627102 pyspedas-1.5.6/pyspedas/elfin/state/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/state/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3366 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/state/state.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.627803 pyspedas-1.5.6/pyspedas/elfin/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_calibration.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6130 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_l1.py
--rw-r--r--   0 jwl        (501) wheel        (0)    18200 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_l2.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3695 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/test_state.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1305 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/elfin/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.628123 pyspedas-1.5.6/pyspedas/equator_s/
--rw-r--r--   0 jwl        (501) wheel        (0)    14979 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/equator_s/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      427 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/equator_s/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4670 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/equator_s/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.628331 pyspedas-1.5.6/pyspedas/equator_s/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/equator_s/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1354 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/equator_s/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.628563 pyspedas-1.5.6/pyspedas/erg/
--rw-r--r--   0 jwl        (501) wheel        (0)     1504 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      515 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/config.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.628666 pyspedas-1.5.6/pyspedas/erg/ground/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.628850 pyspedas-1.5.6/pyspedas/erg/ground/camera/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/camera/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    10270 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/camera/camera_omti_asi.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.629612 pyspedas-1.5.6/pyspedas/erg/ground/geomag/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8590 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_isee_fluxgate.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8563 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_isee_induction.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9561 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_magdas_1sec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8934 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_mm210.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3293 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_stel_fluxgate.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3299 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_stel_induction.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.629724 pyspedas-1.5.6/pyspedas/erg/ground/radar/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/radar/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.630025 pyspedas-1.5.6/pyspedas/erg/ground/radar/superdarn/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/radar/superdarn/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      720 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/radar/superdarn/get_sphcntr.py
--rw-r--r--   0 jwl        (501) wheel        (0)    27656 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/radar/superdarn/sd_fit.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.630239 pyspedas-1.5.6/pyspedas/erg/ground/riometer/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/riometer/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9960 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/riometer/isee_brio.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.630450 pyspedas-1.5.6/pyspedas/erg/ground/vlf/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/vlf/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7733 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/ground/vlf/isee_vlf.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.630569 pyspedas-1.5.6/pyspedas/erg/satellite/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.630867 pyspedas-1.5.6/pyspedas/erg/satellite/erg/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.631065 pyspedas-1.5.6/pyspedas/erg/satellite/erg/att/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/att/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4772 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/att/att.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.631179 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.632062 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      530 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/cart_trans_matrix_make.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3901 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/dsi2j2000.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7228 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/erg_cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6153 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/erg_interpolate_att.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2945 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/sga2sgi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2651 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/sgi2dsi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2344 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/vector_rotate.py
--rw-r--r--   0 jwl        (501) wheel        (0)      525 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/config.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.632277 pyspedas-1.5.6/pyspedas/erg/satellite/erg/hep/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/hep/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    22375 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/hep/hep.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.632492 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepe/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepe/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15931 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepe/lepe.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.632707 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    14803 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepi/lepi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2729 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.632909 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepe/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepe/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7590 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepe/mepe.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.633217 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7390 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/mepi_nml.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6234 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/mepi_tof.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.633409 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mgf/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mgf/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12169 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/mgf/mgf.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.633737 pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15109 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/orb.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2225 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/remove_duplicated_tframe.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.636765 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4270 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_convert_flux_units.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15470 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_hep_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15726 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_hep_part_products.py
--rw-r--r--   0 jwl        (501) wheel        (0)    21859 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lep_part_products.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12715 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lepe_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)    10792 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lepi_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17987 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mep_part_products.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9719 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mepe_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)    10481 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mepi_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2647 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_clean_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1110 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_do_fac.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2728 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_limit_range.py
--rw-r--r--   0 jwl        (501) wheel        (0)      826 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_e_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_fac.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5366 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_phi_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4955 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_theta_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1655 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2019 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_moments_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1260 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_progress_update.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2727 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_units_string.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9563 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_xep_get_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9900 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_xep_part_products.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1443 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_lepi_flux_angle_in_sga.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1660 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepe_az_dir_in_sga.py
--rw-r--r--   0 jwl        (501) wheel        (0)      666 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepe_flux_angle_in_sga.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1343 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepi_flux_angle_in_sga.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.637304 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9689 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_efd.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11063 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_hfa.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6640 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_ofa.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12564 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_wfc.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.637512 pyspedas-1.5.6/pyspedas/erg/satellite/erg/xep/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/xep/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8565 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/satellite/erg/xep/xep.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.637711 pyspedas-1.5.6/pyspedas/erg/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3353 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/erg/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.638032 pyspedas-1.5.6/pyspedas/fast/
--rw-r--r--   0 jwl        (501) wheel        (0)    10890 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/fast/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/fast/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2260 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/fast/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.638227 pyspedas-1.5.6/pyspedas/fast/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/fast/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1342 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/fast/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.639305 pyspedas-1.5.6/pyspedas/geopack/
--rw-r--r--   0 jwl        (501) wheel        (0)      253 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6092 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/get_tsy_params.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3366 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/get_w_params.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2050 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/kp2iopt.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2096 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/t01.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1833 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/t89.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2364 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/t89_trace_equator.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2207 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/t89_trace_iono.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1965 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/t96.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.639644 pyspedas-1.5.6/pyspedas/geopack/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6871 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/tests/geopack_idl_validation_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4940 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/tests/tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2269 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geopack/ts04.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.639989 pyspedas-1.5.6/pyspedas/geotail/
--rw-r--r--   0 jwl        (501) wheel        (0)    13020 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geotail/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      419 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geotail/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5613 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geotail/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.640203 pyspedas-1.5.6/pyspedas/geotail/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geotail/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1329 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/geotail/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.640671 pyspedas-1.5.6/pyspedas/goes/
--rw-r--r--   0 jwl        (501) wheel        (0)      591 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      434 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)    19364 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/load.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3563 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/load_orbit.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.640864 pyspedas-1.5.6/pyspedas/goes/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7493 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/goes/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.641064 pyspedas-1.5.6/pyspedas/hapi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/hapi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5423 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/hapi/hapi.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.641269 pyspedas-1.5.6/pyspedas/hapi/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/hapi/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1313 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/hapi/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.641581 pyspedas-1.5.6/pyspedas/image/
--rw-r--r--   0 jwl        (501) wheel        (0)    15600 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/image/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      411 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/image/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4764 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/image/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.641780 pyspedas-1.5.6/pyspedas/image/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/image/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1641 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/image/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.641991 pyspedas-1.5.6/pyspedas/kyoto/
--rw-r--r--   0 jwl        (501) wheel        (0)       26 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/kyoto/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5874 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/kyoto/load_dst.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.642195 pyspedas-1.5.6/pyspedas/kyoto/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/kyoto/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1308 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/kyoto/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.642512 pyspedas-1.5.6/pyspedas/lanl/
--rw-r--r--   0 jwl        (501) wheel        (0)     6118 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/lanl/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      406 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/lanl/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4257 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/lanl/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.642706 pyspedas-1.5.6/pyspedas/lanl/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/lanl/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1070 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/lanl/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.643554 pyspedas-1.5.6/pyspedas/maven/
--rw-r--r--   0 jwl        (501) wheel        (0)    11613 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      334 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7009 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/download_files_utilities.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1940 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/file_regex.py
--rw-r--r--   0 jwl        (501) wheel        (0)    21768 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/maven_kp_to_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13748 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/maven_load.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1609 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/orbit_time.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.643905 pyspedas-1.5.6/pyspedas/maven/spdf/
--rw-r--r--   0 jwl        (501) wheel        (0)      346 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/spdf/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      406 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/spdf/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8460 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/spdf/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.644101 pyspedas-1.5.6/pyspedas/maven/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1906 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/tests/tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)    79453 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/maven/utilities.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.644421 pyspedas-1.5.6/pyspedas/mica/
--rw-r--r--   0 jwl        (501) wheel        (0)       80 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mica/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      393 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mica/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3986 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mica/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.644622 pyspedas-1.5.6/pyspedas/mica/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mica/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      831 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mica/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.646688 pyspedas-1.5.6/pyspedas/mms/
--rw-r--r--   0 jwl        (501) wheel        (0)     2849 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.646887 pyspedas-1.5.6/pyspedas/mms/aspoc/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/aspoc/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4618 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/aspoc/aspoc.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.647452 pyspedas-1.5.6/pyspedas/mms/cotrans/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/cotrans/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4894 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_lmn.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2598 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_qrotate.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2242 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_qtransformer.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7095 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/cotrans/mms_qcotrans.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.647752 pyspedas-1.5.6/pyspedas/mms/dsp/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/dsp/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4793 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/dsp/dsp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7458 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/dsp/mms_dsp_set_metadata.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.648058 pyspedas-1.5.6/pyspedas/mms/edi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4760 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edi/edi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3514 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edi/mms_edi_set_metadata.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.648419 pyspedas-1.5.6/pyspedas/mms/edp/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edp/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5279 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edp/edp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2556 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/edp/mms_edp_set_metadata.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.649560 pyspedas-1.5.6/pyspedas/mms/eis/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13061 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/eis.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3658 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_omni.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9776 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_pad.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3963 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_pad_spinavg.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1421 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_set_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7444 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_spec_combine_sc.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3837 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_spin_avg.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.652076 pyspedas-1.5.6/pyspedas/mms/feeps/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/feeps.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3428 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_active_eyes.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1951 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_correct_energies.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2134 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_energy_table.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5763 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_flat_field_corrections.py
--rw-r--r--   0 jwl        (501) wheel        (0)    15065 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_getgyrophase.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6974 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_gpd.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7106 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_omni.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7823 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pad.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4059 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pad_spinavg.py
--rw-r--r--   0 jwl        (501) wheel        (0)    14567 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pitch_angles.py
--rw-r--r--   0 jwl        (501) wheel        (0)    16172 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_remove_bad_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3658 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_remove_sun.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2935 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_spin_avg.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2905 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_split_integral_ch.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2200 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/mms_read_feeps_sector_masks_csv.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.656453 pyspedas-1.5.6/pyspedas/mms/feeps/sun/
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220113.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220506.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220815.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220113.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220506.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220815.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220113.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220506.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220815.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220113.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220506.csv
--rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220815.csv
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.657235 pyspedas-1.5.6/pyspedas/mms/fgm/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8114 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/fgm.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9700 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/mms_curl.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2402 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/mms_fgm_remove_flags.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4491 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/mms_fgm_set_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4632 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/mms_lingradest.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1907 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fgm/mms_split_fgm_data.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.658329 pyspedas-1.5.6/pyspedas/mms/fpi/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    16170 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/fpi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9260 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_ang_ang.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3111 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_make_compressionlossbars.py
--rw-r--r--   0 jwl        (501) wheel        (0)    14212 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_make_errorflagbars.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7916 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_set_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2189 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_split_tensor.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6780 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_get_fpi_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4383 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_load_fpi_calc_pad.py
--rw-r--r--   0 jwl        (501) wheel        (0)    19508 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fpi/mms_pad_fpi.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.658546 pyspedas-1.5.6/pyspedas/mms/fsm/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fsm/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4667 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/fsm/fsm.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.659385 pyspedas-1.5.6/pyspedas/mms/hpca/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9063 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/hpca.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8150 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_get_hpca_dist.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3254 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_get_hpca_info.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3612 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_calc_anodes.py
--rw-r--r--   0 jwl        (501) wheel        (0)      691 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_energies.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2846 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_set_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2698 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_spin_sum.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.660149 pyspedas-1.5.6/pyspedas/mms/mec/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)   769966 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec/earth_polar1.png
--rw-r--r--   0 jwl        (501) wheel        (0)     5235 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec/mec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4661 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec/mms_mec_set_metadata.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.661241 pyspedas-1.5.6/pyspedas/mms/mec_ascii/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2636 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_local_ancillary_files.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2857 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_local_state_files.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6217 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_state_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3999 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_tetrahedron_qf.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2638 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_att_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2360 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_eph_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1292 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_qf_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2099 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/state.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1378 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mec_ascii/tetrahedron_qf.py
--rw-r--r--   0 jwl        (501) wheel        (0)      782 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3006 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_events.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3632 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_file_filter.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1669 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_files_in_interval.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4495 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_get_local_files.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3670 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_load_brst_segments.py
--rw-r--r--   0 jwl        (501) wheel        (0)    10979 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_load_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6418 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_load_data_spdf.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_load_fast_segments.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3969 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_load_sroi_segments.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2432 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_login_lasp.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6158 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_orbit_plot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9072 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_overview_plot.py
--rw-r--r--   0 jwl        (501) wheel        (0)      507 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_python_startup.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1132 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_tai2unix.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3379 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/mms_update_brst_intervals.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.662983 pyspedas-1.5.6/pyspedas/mms/particles/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2829 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_convert_flux_units.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2710 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_part_des_photoelectrons.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8209 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_part_getspec.py
--rw-r--r--   0 jwl        (501) wheel        (0)    16781 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_part_products.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11889 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_part_slice2d.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1835 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_clean_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1519 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_clean_support.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2074 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_e_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4995 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_fac.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1971 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_phi_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1962 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_theta_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1074 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_split_hpca.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3235 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/particles/moka_mms_clean_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)      645 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/print_vars.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.663302 pyspedas-1.5.6/pyspedas/mms/scm/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/scm/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1603 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/scm/mms_scm_set_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6092 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/scm/scm.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1895 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/spd_mms_load_bss.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.665066 pyspedas-1.5.6/pyspedas/mms/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3610 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3668 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/curlometer.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3190 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/data_rate_segments.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6156 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/eis.py
--rw-r--r--   0 jwl        (501) wheel        (0)      433 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/events.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7663 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/feeps.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3564 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/file_filter.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8342 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/fpi_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)    20259 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/load_routine_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5994 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/mms_part_getspec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2595 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/neutral_sheet.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5885 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/orbit_plots.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4320 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/ql_l1b_sitl_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)      228 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/setup_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6898 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/slice2d.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2318 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/mms/tests/wavpol.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.665367 pyspedas-1.5.6/pyspedas/noaa/
--rw-r--r--   0 jwl        (501) wheel        (0)       38 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/noaa/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      429 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/noaa/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12504 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/noaa/noaa_load_kp.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.665671 pyspedas-1.5.6/pyspedas/omni/
--rw-r--r--   0 jwl        (501) wheel        (0)     3917 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/omni/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      416 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/omni/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4511 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/omni/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.665856 pyspedas-1.5.6/pyspedas/omni/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/omni/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3087 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/omni/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.666051 pyspedas-1.5.6/pyspedas/particles/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.666553 pyspedas-1.5.6/pyspedas/particles/moments/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/moments/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3465 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/moments/moments_3d.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1948 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/moments/moments_3d_omega_weights.py
--rw-r--r--   0 jwl        (501) wheel        (0)      475 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/moments/spd_pgs_moments.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1326 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/moments/spd_pgs_moments_tplot.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.667506 pyspedas-1.5.6/pyspedas/particles/spd_part_products/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1061 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_do_fac.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2160 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_limit_range.py
--rw-r--r--   0 jwl        (501) wheel        (0)      834 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_e_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4821 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_phi_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4244 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_theta_spec.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1571 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_tplot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1243 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_progress_update.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2745 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_regrid.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.670092 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2113 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/quaternions.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3394 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice1d_plot.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13802 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3388 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_2di.py
--rw-r--r--   0 jwl        (501) wheel        (0)      749 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_checkbins.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2419 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_collate.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1502 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_custom_rotation.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5883 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_geo.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3417 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_data.py
--rw-r--r--   0 jwl        (501) wheel        (0)      853 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_ebounds.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1473 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_sphere.py
--rw-r--r--   0 jwl        (501) wheel        (0)      753 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_support.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2702 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_getinfo.py
--rw-r--r--   0 jwl        (501) wheel        (0)      682 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_intrange.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1025 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_nearest.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1986 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_orientslice.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3715 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_plot.py
--rw-r--r--   0 jwl        (501) wheel        (0)      819 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_rlog.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3005 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_rotate.py
--rw-r--r--   0 jwl        (501) wheel        (0)      556 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_s2c.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1686 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_smooth.py
--rw-r--r--   0 jwl        (501) wheel        (0)      731 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_subtract.py
--rw-r--r--   0 jwl        (501) wheel        (0)      776 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/spd_cal_rot.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1236 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_slice2d/tplot_average.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1114 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/particles/spd_units_string.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.670393 pyspedas-1.5.6/pyspedas/poes/
--rw-r--r--   0 jwl        (501) wheel        (0)     2837 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/poes/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/poes/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3754 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/poes/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.670584 pyspedas-1.5.6/pyspedas/poes/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/poes/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1150 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/poes/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.670894 pyspedas-1.5.6/pyspedas/polar/
--rw-r--r--   0 jwl        (501) wheel        (0)    25546 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/polar/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/polar/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5809 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/polar/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.671073 pyspedas-1.5.6/pyspedas/polar/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/polar/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2120 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/polar/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.671603 pyspedas-1.5.6/pyspedas/psp/
--rw-r--r--   0 jwl        (501) wheel        (0)    22603 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      552 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)    12844 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/filter.py
--rw-r--r--   0 jwl        (501) wheel        (0)    14118 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/load.py
--rw-r--r--   0 jwl        (501) wheel        (0)      800 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/rfs.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.671787 pyspedas-1.5.6/pyspedas/psp/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7558 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/psp/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.672103 pyspedas-1.5.6/pyspedas/rbsp/
--rw-r--r--   0 jwl        (501) wheel        (0)    24859 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7692 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.672900 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4399 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_load_rbspice_read.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3193 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_omni.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8141 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5570 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad_spinavg.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4471 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_spin_avg.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.673115 pyspedas-1.5.6/pyspedas/rbsp/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5630 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/rbsp/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.673580 pyspedas-1.5.6/pyspedas/secs/
--rw-r--r--   0 jwl        (501) wheel        (0)     7306 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/secs/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1011 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/secs/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6549 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/secs/load.py
--rw-r--r--   0 jwl        (501) wheel        (0)    27415 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/secs/makeplots.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.673946 pyspedas-1.5.6/pyspedas/soho/
--rw-r--r--   0 jwl        (501) wheel        (0)    10173 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/soho/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/soho/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4604 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/soho/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.674154 pyspedas-1.5.6/pyspedas/soho/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/soho/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1160 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/soho/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.674466 pyspedas-1.5.6/pyspedas/solo/
--rw-r--r--   0 jwl        (501) wheel        (0)    12856 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/solo/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      431 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/solo/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6526 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/solo/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.674676 pyspedas-1.5.6/pyspedas/solo/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/solo/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2224 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/solo/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.674914 pyspedas-1.5.6/pyspedas/sosmag/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/sosmag/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    18449 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/sosmag/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.675187 pyspedas-1.5.6/pyspedas/sosmag/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/sosmag/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1520 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/sosmag/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.675608 pyspedas-1.5.6/pyspedas/st5/
--rw-r--r--   0 jwl        (501) wheel        (0)     3089 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/st5/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/st5/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1592 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/st5/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.675874 pyspedas-1.5.6/pyspedas/st5/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/st5/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      602 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/st5/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.676312 pyspedas-1.5.6/pyspedas/stereo/
--rw-r--r--   0 jwl        (501) wheel        (0)    26388 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/stereo/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      417 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/stereo/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3714 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/stereo/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.676579 pyspedas-1.5.6/pyspedas/stereo/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/stereo/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2940 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/stereo/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.676971 pyspedas-1.5.6/pyspedas/swarm/
--rw-r--r--   0 jwl        (501) wheel        (0)     1408 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/swarm/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)       58 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/swarm/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1484 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/swarm/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.677230 pyspedas-1.5.6/pyspedas/swarm/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/swarm/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      485 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/swarm/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.677636 pyspedas-1.5.6/pyspedas/themis/
--rw-r--r--   0 jwl        (501) wheel        (0)      976 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.677922 pyspedas-1.5.6/pyspedas/themis/analysis/
--rw-r--r--   0 jwl        (501) wheel        (0)       34 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/analysis/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11379 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/analysis/scpot2dens.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.678193 pyspedas-1.5.6/pyspedas/themis/common/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/common/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1956 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/common/check_args.py
--rw-r--r--   0 jwl        (501) wheel        (0)      452 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/config.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.678940 pyspedas-1.5.6/pyspedas/themis/cotrans/
--rw-r--r--   0 jwl        (501) wheel        (0)      115 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/cotrans/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6076 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/cotrans/dsl2gse.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7033 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/cotrans/gse2sse.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6493 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/cotrans/sse2sel.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4137 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/cotrans/ssl2dsl.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.679314 pyspedas-1.5.6/pyspedas/themis/ground/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/ground/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2892 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/ground/ask.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8880 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/ground/gmag.py
--rw-r--r--   0 jwl        (501) wheel        (0)    11391 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.679436 pyspedas-1.5.6/pyspedas/themis/spacecraft/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/__init__.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.680221 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2813 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/efi.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3234 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fbk.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2810 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fft.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6339 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fgm.py
--rw-r--r--   0 jwl        (501) wheel        (0)    17057 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fit.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2826 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/scm.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.680918 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3104 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/esa.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3408 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/esd.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2892 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/gmom.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2907 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/mom.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2787 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/sst.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.681461 pyspedas-1.5.6/pyspedas/themis/state/
--rw-r--r--   0 jwl        (501) wheel        (0)       73 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3362 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/apply_spinaxis_corrections.py
--rw-r--r--   0 jwl        (501) wheel        (0)     6442 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/autoload_support.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3149 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/slp.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.681915 pyspedas-1.5.6/pyspedas/themis/state/spinmodel/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/spinmodel/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)    33383 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1990 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel_postprocess.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4391 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel_segment.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5025 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/state/state.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.683245 pyspedas-1.5.6/pyspedas/themis/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     8403 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/autoload_support_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)      520 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/test_cal_fit_tplot_metadata.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5627 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     9008 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_cal_fit.py
--rw-r--r--   0 jwl        (501) wheel        (0)    13897 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_dsl_cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)    14360 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_lunar_cotrans.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4320 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_scpot2dens.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7292 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_spinmodel.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4448 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_state.py
--rw-r--r--   0 jwl        (501) wheel        (0)      885 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_themis_check_args.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4717 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/tests_tplot_time.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.683604 pyspedas-1.5.6/pyspedas/themis/tests/validation/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/validation/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3217 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/validation/cal_fit_validation.py
--rw-r--r--   0 jwl        (501) wheel        (0)      716 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/themis/tests/validation/dsl2gse.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.683973 pyspedas-1.5.6/pyspedas/twins/
--rw-r--r--   0 jwl        (501) wheel        (0)     7744 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/twins/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/twins/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4148 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/twins/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.684173 pyspedas-1.5.6/pyspedas/twins/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/twins/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      876 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/twins/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.684515 pyspedas-1.5.6/pyspedas/ulysses/
--rw-r--r--   0 jwl        (501) wheel        (0)    21167 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ulysses/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      411 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ulysses/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4669 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ulysses/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.684724 pyspedas-1.5.6/pyspedas/ulysses/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ulysses/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1781 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/ulysses/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.685876 pyspedas-1.5.6/pyspedas/utilities/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4624 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/dailynames.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1627 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/datasets.py
--rw-r--r--   0 jwl        (501) wheel        (0)    16124 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/download.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3059 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/download_ftp.py
--rw-r--r--   0 jwl        (501) wheel        (0)      849 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/interpol.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2018 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/leap_seconds.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5325 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/libs.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3234 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/mpause_2.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4482 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/mpause_t96.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.686089 pyspedas-1.5.6/pyspedas/utilities/spice/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/spice/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2113 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/spice/time_ephemeris.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1867 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tcopy.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.686638 pyspedas-1.5.6/pyspedas/utilities/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     4257 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tests/download_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2856 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tests/libs_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     5389 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tests/misc_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)     2652 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/utilities/tests/time_tests.py
--rw-r--r--   0 jwl        (501) wheel        (0)      302 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/version.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.686934 pyspedas-1.5.6/pyspedas/vires/
--rw-r--r--   0 jwl        (501) wheel        (0)      487 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/vires/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/vires/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     1950 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/vires/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.687258 pyspedas-1.5.6/pyspedas/wind/
--rw-r--r--   0 jwl        (501) wheel        (0)    12855 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/wind/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/wind/config.py
--rw-r--r--   0 jwl        (501) wheel        (0)     3924 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/wind/load.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.687457 pyspedas-1.5.6/pyspedas/wind/tests/
--rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/wind/tests/__init__.py
--rw-r--r--   0 jwl        (501) wheel        (0)     7573 2024-02-20 06:53:33.000000 pyspedas-1.5.6/pyspedas/wind/tests/tests.py
-drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-02-20 06:54:23.613448 pyspedas-1.5.6/pyspedas.egg-info/
--rw-r--r--   0 jwl        (501) wheel        (0)    14462 2024-02-20 06:54:23.000000 pyspedas-1.5.6/pyspedas.egg-info/PKG-INFO
--rw-r--r--   0 jwl        (501) wheel        (0)    24672 2024-02-20 06:54:23.000000 pyspedas-1.5.6/pyspedas.egg-info/SOURCES.txt
--rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-02-20 06:54:23.000000 pyspedas-1.5.6/pyspedas.egg-info/dependency_links.txt
--rw-r--r--   0 jwl        (501) wheel        (0)      161 2024-02-20 06:54:23.000000 pyspedas-1.5.6/pyspedas.egg-info/requires.txt
--rw-r--r--   0 jwl        (501) wheel        (0)        9 2024-02-20 06:54:23.000000 pyspedas-1.5.6/pyspedas.egg-info/top_level.txt
--rw-r--r--   0 jwl        (501) wheel        (0)       38 2024-02-20 06:54:23.687847 pyspedas-1.5.6/setup.cfg
--rwxr-xr-x   0 jwl        (501) wheel        (0)     1384 2024-02-20 06:53:33.000000 pyspedas-1.5.6/setup.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.343464 pyspedas-1.5.7/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3332 2024-04-05 16:50:01.000000 pyspedas-1.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jwl        (501) wheel        (0)     5749 2024-04-05 16:50:01.000000 pyspedas-1.5.7/CONTRIBUTING.md
+-rw-r--r--   0 jwl        (501) wheel        (0)     1109 2024-04-05 16:50:01.000000 pyspedas-1.5.7/LICENSE.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)      335 2024-04-05 16:50:01.000000 pyspedas-1.5.7/MANIFEST.in
+-rw-r--r--   0 jwl        (501) wheel        (0)    14462 2024-04-05 16:50:20.343259 pyspedas-1.5.7/PKG-INFO
+-rw-r--r--   0 jwl        (501) wheel        (0)    13805 2024-04-05 16:50:01.000000 pyspedas-1.5.7/README.md
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.269995 pyspedas-1.5.7/pyspedas/
+-rw-r--r--   0 jwl        (501) wheel        (0)     5860 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.270866 pyspedas-1.5.7/pyspedas/ace/
+-rw-r--r--   0 jwl        (501) wheel        (0)    23202 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ace/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      399 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ace/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3103 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ace/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.271060 pyspedas-1.5.7/pyspedas/ace/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ace/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1962 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ace/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.271351 pyspedas-1.5.7/pyspedas/akebono/
+-rw-r--r--   0 jwl        (501) wheel        (0)    14718 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/akebono/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      421 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/akebono/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2108 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/akebono/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.271544 pyspedas-1.5.7/pyspedas/akebono/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/akebono/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1141 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/akebono/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.273119 pyspedas-1.5.7/pyspedas/analysis/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6581 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/avg_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1960 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/deriv_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      860 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/dpwrspc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    24049 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/find_magnetic_nulls.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7839 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/lingradest.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    21664 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/neutral_sheet.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1634 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tdeflag.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      835 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tdpwrspc.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.273763 pyspedas-1.5.7/pyspedas/analysis/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5497 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tests/test_magnetic_nulls.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4705 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tests/test_twavpol.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    10987 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tests/tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2061 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/time_domain_filter.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3477 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tinterpol.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2055 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/tvectot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    31210 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/twavpol.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2870 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/wavelet.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2168 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/analysis/yclip.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.274142 pyspedas-1.5.7/pyspedas/barrel/
+-rw-r--r--   0 jwl        (501) wheel        (0)    10483 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/barrel/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3469 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/barrel/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2592 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/barrel/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.274364 pyspedas-1.5.7/pyspedas/barrel/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/barrel/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      292 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/barrel/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.274900 pyspedas-1.5.7/pyspedas/cdagui/
+-rw-r--r--   0 jwl        (501) wheel        (0)      121 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cdagui/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17376 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cdagui/cdagui.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6166 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cdagui/cdaweb.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      234 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cdagui/config.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.275410 pyspedas-1.5.7/pyspedas/cluster/
+-rw-r--r--   0 jwl        (501) wheel        (0)    31937 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      419 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6106 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/load.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8563 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/load_csa.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.275662 pyspedas-1.5.7/pyspedas/cluster/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3129 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cluster/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.276046 pyspedas-1.5.7/pyspedas/cnofs/
+-rw-r--r--   0 jwl        (501) wheel        (0)     7645 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cnofs/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cnofs/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1916 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cnofs/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.276284 pyspedas-1.5.7/pyspedas/cnofs/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cnofs/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1017 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cnofs/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.278335 pyspedas-1.5.7/pyspedas/cotrans/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1374 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/cart2spc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3999 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      227 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/cotrans_get_coord.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    30626 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/cotrans_lib.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      241 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/cotrans_set_coord.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2226 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/fac_matrix_make.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2327 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/gsm2lmn.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17808 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/igrf.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13130 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/j2000.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5141 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/matrix_array_lib.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1902 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/minvar.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2244 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/minvar_matrix_make.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    25354 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/quaternions.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1107 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/sm2mlt.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1199 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/spc2cart.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.278839 pyspedas-1.5.7/pyspedas/cotrans/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12066 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/tests/cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1235 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/tests/quaternions.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2141 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/tests/test_minvar.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3025 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/tvector_rotate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      847 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/cotrans/xyz_to_polar.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.279258 pyspedas-1.5.7/pyspedas/csswe/
+-rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/csswe/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/csswe/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3613 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/csswe/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.279526 pyspedas-1.5.7/pyspedas/csswe/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/csswe/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      617 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/csswe/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.279961 pyspedas-1.5.7/pyspedas/de2/
+-rw-r--r--   0 jwl        (501) wheel        (0)    19125 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/de2/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      407 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/de2/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5044 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/de2/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.280222 pyspedas-1.5.7/pyspedas/de2/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/de2/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1945 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/de2/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.280662 pyspedas-1.5.7/pyspedas/dscovr/
+-rw-r--r--   0 jwl        (501) wheel        (0)     9992 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/dscovr/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      408 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/dscovr/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4522 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/dscovr/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.280925 pyspedas-1.5.7/pyspedas/dscovr/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/dscovr/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1410 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/dscovr/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.281366 pyspedas-1.5.7/pyspedas/elfin/
+-rw-r--r--   0 jwl        (501) wheel        (0)    17552 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      400 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/config.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.281640 pyspedas-1.5.7/pyspedas/elfin/eng/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/eng/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3488 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/eng/eng.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.282610 pyspedas-1.5.7/pyspedas/elfin/epd/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11396 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/calibration_l1.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    16661 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/calibration_l2.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      456 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/ela_epde_cal_data.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)     1355 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/elb_epde_cal_data.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)     7962 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/epd.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6642 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/epd/postprocessing.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.282871 pyspedas-1.5.7/pyspedas/elfin/fgm/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/fgm/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3341 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/fgm/fgm.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3231 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.283110 pyspedas-1.5.7/pyspedas/elfin/mrma/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/mrma/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3073 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/mrma/mrma.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.283297 pyspedas-1.5.7/pyspedas/elfin/mrmi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/mrmi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3053 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/mrmi/mrmi.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.283484 pyspedas-1.5.7/pyspedas/elfin/state/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/state/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3366 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/state/state.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.284091 pyspedas-1.5.7/pyspedas/elfin/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_calibration.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6130 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_l1.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    18200 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_l2.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3695 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/test_state.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1305 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/elfin/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.284388 pyspedas-1.5.7/pyspedas/equator_s/
+-rw-r--r--   0 jwl        (501) wheel        (0)    14979 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/equator_s/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      427 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/equator_s/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4670 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/equator_s/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.284564 pyspedas-1.5.7/pyspedas/equator_s/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/equator_s/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1354 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/equator_s/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.284768 pyspedas-1.5.7/pyspedas/erg/
+-rw-r--r--   0 jwl        (501) wheel        (0)     1504 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      515 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/config.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.284870 pyspedas-1.5.7/pyspedas/erg/ground/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.285044 pyspedas-1.5.7/pyspedas/erg/ground/camera/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/camera/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9755 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/camera/camera_omti_asi.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.285794 pyspedas-1.5.7/pyspedas/erg/ground/geomag/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8180 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_isee_fluxgate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8097 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_isee_induction.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8887 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_magdas_1sec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9783 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_mm210.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3293 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_stel_fluxgate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3299 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_stel_induction.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.286098 pyspedas-1.5.7/pyspedas/erg/ground/radar/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/radar/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.286493 pyspedas-1.5.7/pyspedas/erg/ground/radar/superdarn/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/radar/superdarn/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      720 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/radar/superdarn/get_sphcntr.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    36883 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/radar/superdarn/sd_fit.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.286753 pyspedas-1.5.7/pyspedas/erg/ground/riometer/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/riometer/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11813 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/riometer/isee_brio.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.286975 pyspedas-1.5.7/pyspedas/erg/ground/vlf/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/vlf/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7832 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/ground/vlf/isee_vlf.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.287086 pyspedas-1.5.7/pyspedas/erg/satellite/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.287467 pyspedas-1.5.7/pyspedas/erg/satellite/erg/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.287681 pyspedas-1.5.7/pyspedas/erg/satellite/erg/att/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/att/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4939 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/att/att.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.287793 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.288603 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      530 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/cart_trans_matrix_make.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3901 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/dsi2j2000.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7228 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/erg_cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6153 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/erg_interpolate_att.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2945 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/sga2sgi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2651 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/sgi2dsi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2344 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/vector_rotate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      525 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1460 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/get_gatt_ror.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.288794 pyspedas-1.5.7/pyspedas/erg/satellite/erg/hep/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/hep/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    22023 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/hep/hep.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.289008 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepe/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepe/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15593 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepe/lepe.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.289212 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14466 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepi/lepi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2723 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.289402 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepe/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepe/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7253 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepe/mepe.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.289706 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7053 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/mepi_nml.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5895 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/mepi_tof.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.289898 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mgf/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mgf/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11832 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/mgf/mgf.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.290200 pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14771 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/orb.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2225 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/remove_duplicated_tframe.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.293106 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4270 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_convert_flux_units.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15470 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_hep_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15726 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_hep_part_products.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    21859 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lep_part_products.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12715 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lepe_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    10792 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lepi_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17987 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mep_part_products.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9719 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mepe_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    10481 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mepi_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2647 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_clean_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1110 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_do_fac.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2728 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_limit_range.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      826 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_e_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_fac.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5366 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_phi_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4955 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_theta_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1655 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2019 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_moments_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1260 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_progress_update.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2727 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_units_string.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9563 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_xep_get_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9900 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_xep_part_products.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1443 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_lepi_flux_angle_in_sga.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1660 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepe_az_dir_in_sga.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      666 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepe_flux_angle_in_sga.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1343 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepi_flux_angle_in_sga.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.293623 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9351 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_efd.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    10726 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_hfa.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6302 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_ofa.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12229 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_wfc.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.293832 pyspedas-1.5.7/pyspedas/erg/satellite/erg/xep/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/xep/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8225 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/satellite/erg/xep/xep.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.294122 pyspedas-1.5.7/pyspedas/erg/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3176 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/tests/ground_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6231 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/erg/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.294438 pyspedas-1.5.7/pyspedas/fast/
+-rw-r--r--   0 jwl        (501) wheel        (0)    10890 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/fast/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/fast/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2260 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/fast/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.294621 pyspedas-1.5.7/pyspedas/fast/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/fast/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1342 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/fast/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.295647 pyspedas-1.5.7/pyspedas/geopack/
+-rw-r--r--   0 jwl        (501) wheel        (0)      253 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6092 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/get_tsy_params.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3366 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/get_w_params.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2050 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/kp2iopt.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2096 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/t01.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1833 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/t89.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2364 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/t89_trace_equator.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2207 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/t89_trace_iono.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1965 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/t96.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.296043 pyspedas-1.5.7/pyspedas/geopack/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6871 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/tests/geopack_idl_validation_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4940 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/tests/tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2269 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geopack/ts04.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.296424 pyspedas-1.5.7/pyspedas/geotail/
+-rw-r--r--   0 jwl        (501) wheel        (0)    13020 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geotail/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      419 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geotail/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5613 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geotail/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.296620 pyspedas-1.5.7/pyspedas/geotail/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geotail/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1329 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/geotail/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.297034 pyspedas-1.5.7/pyspedas/goes/
+-rw-r--r--   0 jwl        (501) wheel        (0)      591 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      434 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    19364 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/load.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3563 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/load_orbit.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.297218 pyspedas-1.5.7/pyspedas/goes/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7493 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/goes/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.297399 pyspedas-1.5.7/pyspedas/hapi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/hapi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6217 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/hapi/hapi.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.297572 pyspedas-1.5.7/pyspedas/hapi/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/hapi/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1417 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/hapi/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.297885 pyspedas-1.5.7/pyspedas/image/
+-rw-r--r--   0 jwl        (501) wheel        (0)    15600 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/image/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      411 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/image/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4764 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/image/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.298081 pyspedas-1.5.7/pyspedas/image/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/image/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1641 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/image/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.298285 pyspedas-1.5.7/pyspedas/kyoto/
+-rw-r--r--   0 jwl        (501) wheel        (0)       26 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/kyoto/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5874 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/kyoto/load_dst.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.298466 pyspedas-1.5.7/pyspedas/kyoto/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/kyoto/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1308 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/kyoto/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.298766 pyspedas-1.5.7/pyspedas/lanl/
+-rw-r--r--   0 jwl        (501) wheel        (0)     6118 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/lanl/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      406 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/lanl/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4257 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/lanl/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.298956 pyspedas-1.5.7/pyspedas/lanl/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/lanl/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1070 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/lanl/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.299849 pyspedas-1.5.7/pyspedas/maven/
+-rw-r--r--   0 jwl        (501) wheel        (0)    19103 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      379 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12165 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/download_files_utilities.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1719 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/file_regex.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    24306 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/maven_kp_to_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    19014 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/maven_load.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2784 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/orbit_time.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.300185 pyspedas-1.5.7/pyspedas/maven/spdf/
+-rw-r--r--   0 jwl        (501) wheel        (0)      346 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/spdf/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      406 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/spdf/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8460 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/spdf/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.300380 pyspedas-1.5.7/pyspedas/maven/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2203 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/tests/tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    85975 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/maven/utilities.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.300727 pyspedas-1.5.7/pyspedas/mica/
+-rw-r--r--   0 jwl        (501) wheel        (0)       80 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mica/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      393 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mica/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3986 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mica/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.300922 pyspedas-1.5.7/pyspedas/mica/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mica/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      831 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mica/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.302821 pyspedas-1.5.7/pyspedas/mms/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3534 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.303024 pyspedas-1.5.7/pyspedas/mms/aspoc/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/aspoc/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4618 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/aspoc/aspoc.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.303550 pyspedas-1.5.7/pyspedas/mms/cotrans/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/cotrans/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4894 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_lmn.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2598 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_qrotate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2242 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_qtransformer.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7095 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/cotrans/mms_qcotrans.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.303861 pyspedas-1.5.7/pyspedas/mms/dsp/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/dsp/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4793 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/dsp/dsp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7458 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/dsp/mms_dsp_set_metadata.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.304237 pyspedas-1.5.7/pyspedas/mms/edi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4760 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edi/edi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3514 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edi/mms_edi_set_metadata.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.304639 pyspedas-1.5.7/pyspedas/mms/edp/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edp/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5279 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edp/edp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2556 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/edp/mms_edp_set_metadata.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.305720 pyspedas-1.5.7/pyspedas/mms/eis/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13061 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/eis.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3658 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_omni.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9776 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_pad.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3963 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_pad_spinavg.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1421 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_set_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7444 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_spec_combine_sc.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3837 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_spin_avg.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.308375 pyspedas-1.5.7/pyspedas/mms/feeps/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/feeps.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3428 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_active_eyes.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1951 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_correct_energies.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2134 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_energy_table.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5763 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_flat_field_corrections.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15065 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_getgyrophase.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6974 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_gpd.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7106 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_omni.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7823 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pad.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4059 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pad_spinavg.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14567 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pitch_angles.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    16172 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_remove_bad_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3658 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_remove_sun.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2935 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_spin_avg.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2905 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_split_integral_ch.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2246 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/mms_read_feeps_sector_masks_csv.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.312791 pyspedas-1.5.7/pyspedas/mms/feeps/sun/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220113.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220506.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220815.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3139 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20240202.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220113.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220506.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220815.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3075 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20240202.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220113.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220506.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220815.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3075 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20240202.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3072 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220113.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220506.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3071 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220815.csv
+-rw-r--r--   0 jwl        (501) wheel        (0)     3075 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20240202.csv
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.313554 pyspedas-1.5.7/pyspedas/mms/fgm/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8114 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/fgm.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9700 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/mms_curl.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2402 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/mms_fgm_remove_flags.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4491 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/mms_fgm_set_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4632 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/mms_lingradest.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1907 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fgm/mms_split_fgm_data.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.314643 pyspedas-1.5.7/pyspedas/mms/fpi/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    16170 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/fpi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9260 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_ang_ang.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3228 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_make_compressionlossbars.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14306 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_make_errorflagbars.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7916 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_set_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2189 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_split_tensor.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6760 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_get_fpi_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4383 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_load_fpi_calc_pad.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    19508 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fpi/mms_pad_fpi.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.314868 pyspedas-1.5.7/pyspedas/mms/fsm/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fsm/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4667 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/fsm/fsm.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.315714 pyspedas-1.5.7/pyspedas/mms/hpca/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9063 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/hpca.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8150 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_get_hpca_dist.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3254 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_get_hpca_info.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3612 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_calc_anodes.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      691 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_energies.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2846 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_set_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2698 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_spin_sum.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.316502 pyspedas-1.5.7/pyspedas/mms/mec/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)   769966 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec/earth_polar1.png
+-rw-r--r--   0 jwl        (501) wheel        (0)     5235 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec/mec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4661 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec/mms_mec_set_metadata.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.317511 pyspedas-1.5.7/pyspedas/mms/mec_ascii/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2636 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_local_ancillary_files.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2857 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_local_state_files.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6241 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_state_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3999 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_tetrahedron_qf.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2638 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_att_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2360 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_eph_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1292 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_qf_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2099 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/state.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1378 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mec_ascii/tetrahedron_qf.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      782 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3006 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_events.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3632 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_file_filter.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1669 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_files_in_interval.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4495 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_get_local_files.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3670 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_load_brst_segments.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11021 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_load_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6418 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_load_data_spdf.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2619 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_load_fast_segments.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3969 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_load_sroi_segments.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2432 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_login_lasp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6158 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_orbit_plot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      507 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_python_startup.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1132 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_tai2unix.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3379 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/mms_update_brst_intervals.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.318942 pyspedas-1.5.7/pyspedas/mms/particles/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2829 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_convert_flux_units.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2829 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_part_des_photoelectrons.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8227 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_part_getspec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    16781 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_part_products.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11888 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_part_slice2d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1835 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_clean_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1519 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_clean_support.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2074 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_e_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4995 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_fac.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1971 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_phi_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1962 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_theta_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1074 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_split_hpca.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3235 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/particles/moka_mms_clean_data.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.319129 pyspedas-1.5.7/pyspedas/mms/plots/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/plots/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8875 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/plots/mms_overview_plot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      645 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/print_vars.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.319407 pyspedas-1.5.7/pyspedas/mms/scm/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/scm/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1603 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/scm/mms_scm_set_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6092 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/scm/scm.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1895 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/spd_mms_load_bss.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.321229 pyspedas-1.5.7/pyspedas/mms/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3610 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3668 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/curlometer.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3190 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/data_rate_segments.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6156 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/eis.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      433 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/events.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7663 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/feeps.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3564 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/file_filter.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8342 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/fpi_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    20973 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/load_routine_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5994 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/mms_part_getspec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2595 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/neutral_sheet.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5885 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/orbit_plots.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      428 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/overview_plots.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4320 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/ql_l1b_sitl_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      228 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/setup_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6898 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/slice2d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2318 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/mms/tests/wavpol.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.321532 pyspedas-1.5.7/pyspedas/noaa/
+-rw-r--r--   0 jwl        (501) wheel        (0)       38 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/noaa/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      429 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/noaa/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12504 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/noaa/noaa_load_kp.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.321844 pyspedas-1.5.7/pyspedas/omni/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3917 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/omni/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      416 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/omni/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4511 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/omni/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.322046 pyspedas-1.5.7/pyspedas/omni/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/omni/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3494 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/omni/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.322239 pyspedas-1.5.7/pyspedas/particles/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.322758 pyspedas-1.5.7/pyspedas/particles/moments/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/moments/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3465 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/moments/moments_3d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1948 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/moments/moments_3d_omega_weights.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      475 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/moments/spd_pgs_moments.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1326 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/moments/spd_pgs_moments_tplot.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.323774 pyspedas-1.5.7/pyspedas/particles/spd_part_products/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1061 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_do_fac.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2160 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_limit_range.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      834 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_e_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4821 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_phi_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4244 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_theta_spec.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1571 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_tplot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1243 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_progress_update.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2745 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_regrid.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.326315 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2113 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/quaternions.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3394 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice1d_plot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13801 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3388 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_2di.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      749 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_checkbins.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2419 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_collate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1502 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_custom_rotation.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5883 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_geo.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3417 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_data.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      853 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_ebounds.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1473 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_sphere.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      753 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_support.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2701 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_getinfo.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      682 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_intrange.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1025 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_nearest.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1986 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_orientslice.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3715 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_plot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      819 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_rlog.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3005 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_rotate.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      556 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_s2c.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1686 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_smooth.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      731 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_subtract.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      776 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/spd_cal_rot.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1216 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_slice2d/tplot_average.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1114 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/particles/spd_units_string.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.326657 pyspedas-1.5.7/pyspedas/poes/
+-rw-r--r--   0 jwl        (501) wheel        (0)     2837 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/poes/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/poes/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3754 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/poes/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.326846 pyspedas-1.5.7/pyspedas/poes/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/poes/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1422 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/poes/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.327173 pyspedas-1.5.7/pyspedas/polar/
+-rw-r--r--   0 jwl        (501) wheel        (0)    25546 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/polar/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/polar/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5809 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/polar/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.327353 pyspedas-1.5.7/pyspedas/polar/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/polar/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2120 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/polar/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.327899 pyspedas-1.5.7/pyspedas/psp/
+-rw-r--r--   0 jwl        (501) wheel        (0)    22603 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      552 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12844 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/filter.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14249 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/load.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      794 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/rfs.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.328088 pyspedas-1.5.7/pyspedas/psp/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7558 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/psp/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.328437 pyspedas-1.5.7/pyspedas/rbsp/
+-rw-r--r--   0 jwl        (501) wheel        (0)    24859 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7692 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.329074 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4399 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_load_rbspice_read.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3193 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_omni.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8141 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5570 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad_spinavg.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4471 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_spin_avg.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.329261 pyspedas-1.5.7/pyspedas/rbsp/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5630 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/rbsp/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.329681 pyspedas-1.5.7/pyspedas/secs/
+-rw-r--r--   0 jwl        (501) wheel        (0)     7306 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/secs/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1011 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/secs/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6549 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/secs/load.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    27415 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/secs/makeplots.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.330020 pyspedas-1.5.7/pyspedas/soho/
+-rw-r--r--   0 jwl        (501) wheel        (0)    10173 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/soho/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/soho/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4604 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/soho/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.330253 pyspedas-1.5.7/pyspedas/soho/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/soho/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1160 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/soho/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.330681 pyspedas-1.5.7/pyspedas/solo/
+-rw-r--r--   0 jwl        (501) wheel        (0)    12856 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/solo/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      431 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/solo/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6526 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/solo/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.330947 pyspedas-1.5.7/pyspedas/solo/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/solo/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2224 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/solo/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.331204 pyspedas-1.5.7/pyspedas/sosmag/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/sosmag/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    18449 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/sosmag/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.331473 pyspedas-1.5.7/pyspedas/sosmag/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/sosmag/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1520 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/sosmag/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.331876 pyspedas-1.5.7/pyspedas/st5/
+-rw-r--r--   0 jwl        (501) wheel        (0)     3089 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/st5/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/st5/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1592 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/st5/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.332114 pyspedas-1.5.7/pyspedas/st5/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/st5/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      602 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/st5/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.332555 pyspedas-1.5.7/pyspedas/stereo/
+-rw-r--r--   0 jwl        (501) wheel        (0)    26388 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/stereo/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      417 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/stereo/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3714 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/stereo/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.332829 pyspedas-1.5.7/pyspedas/stereo/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/stereo/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2940 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/stereo/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.333320 pyspedas-1.5.7/pyspedas/swarm/
+-rw-r--r--   0 jwl        (501) wheel        (0)     1835 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/swarm/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)       58 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/swarm/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2761 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/swarm/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.333597 pyspedas-1.5.7/pyspedas/swarm/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/swarm/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      485 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/swarm/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.334000 pyspedas-1.5.7/pyspedas/themis/
+-rw-r--r--   0 jwl        (501) wheel        (0)      976 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.334246 pyspedas-1.5.7/pyspedas/themis/analysis/
+-rw-r--r--   0 jwl        (501) wheel        (0)       34 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/analysis/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11379 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/analysis/scpot2dens.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.334468 pyspedas-1.5.7/pyspedas/themis/common/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/common/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1956 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/common/check_args.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      452 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/config.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.334979 pyspedas-1.5.7/pyspedas/themis/cotrans/
+-rw-r--r--   0 jwl        (501) wheel        (0)      115 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/cotrans/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6076 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/cotrans/dsl2gse.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7033 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/cotrans/gse2sse.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6493 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/cotrans/sse2sel.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4137 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/cotrans/ssl2dsl.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.335251 pyspedas-1.5.7/pyspedas/themis/ground/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/ground/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2892 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/ground/ask.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    12212 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/ground/gmag.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    11391 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.335352 pyspedas-1.5.7/pyspedas/themis/spacecraft/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/__init__.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.336070 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2813 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/efi.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3234 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fbk.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2810 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fft.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6339 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fgm.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17057 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fit.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2826 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/scm.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.336656 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3104 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/esa.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3408 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/esd.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2892 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/gmom.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2907 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/mom.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2787 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/sst.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.337174 pyspedas-1.5.7/pyspedas/themis/state/
+-rw-r--r--   0 jwl        (501) wheel        (0)       73 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3362 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/apply_spinaxis_corrections.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     6442 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/autoload_support.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3149 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/slp.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.337604 pyspedas-1.5.7/pyspedas/themis/state/spinmodel/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/spinmodel/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    33383 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1990 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel_postprocess.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4391 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel_segment.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5025 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/state/state.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.338841 pyspedas-1.5.7/pyspedas/themis/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     8403 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/autoload_support_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      520 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/test_cal_fit_tplot_metadata.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5627 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     9008 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_cal_fit.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    13897 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_dsl_cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    14360 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_lunar_cotrans.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4320 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_scpot2dens.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7292 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_spinmodel.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4448 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_state.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      885 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_themis_check_args.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4717 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/tests_tplot_time.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.339121 pyspedas-1.5.7/pyspedas/themis/tests/validation/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/validation/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3217 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/validation/cal_fit_validation.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      716 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/themis/tests/validation/dsl2gse.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.339428 pyspedas-1.5.7/pyspedas/twins/
+-rw-r--r--   0 jwl        (501) wheel        (0)     7744 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/twins/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      409 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/twins/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4148 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/twins/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.339605 pyspedas-1.5.7/pyspedas/twins/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/twins/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      876 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/twins/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.339925 pyspedas-1.5.7/pyspedas/ulysses/
+-rw-r--r--   0 jwl        (501) wheel        (0)    21167 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ulysses/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      411 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ulysses/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4669 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ulysses/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.340107 pyspedas-1.5.7/pyspedas/ulysses/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ulysses/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1781 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/ulysses/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.341318 pyspedas-1.5.7/pyspedas/utilities/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4624 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/dailynames.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1848 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/datasets.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    17037 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/download.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3059 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/download_ftp.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      285 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/find_ip_address.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      849 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/interpol.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2018 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/leap_seconds.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     5325 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/libs.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3234 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/mpause_2.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4482 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/mpause_t96.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.341505 pyspedas-1.5.7/pyspedas/utilities/spice/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/spice/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2113 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/spice/time_ephemeris.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1867 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tcopy.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.342208 pyspedas-1.5.7/pyspedas/utilities/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4257 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/download_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2856 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/libs_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     4957 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/misc_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)    15002 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/plot_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      420 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/test_find_ip_address.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     2652 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/utilities/tests/time_tests.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      302 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/version.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.342495 pyspedas-1.5.7/pyspedas/vires/
+-rw-r--r--   0 jwl        (501) wheel        (0)      487 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/vires/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/vires/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     1950 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/vires/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.342813 pyspedas-1.5.7/pyspedas/wind/
+-rw-r--r--   0 jwl        (501) wheel        (0)    16632 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/wind/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)      404 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/wind/config.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     3924 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/wind/load.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.342999 pyspedas-1.5.7/pyspedas/wind/tests/
+-rw-r--r--   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/wind/tests/__init__.py
+-rw-r--r--   0 jwl        (501) wheel        (0)     7573 2024-04-05 16:50:01.000000 pyspedas-1.5.7/pyspedas/wind/tests/tests.py
+drwxr-xr-x   0 jwl        (501) wheel        (0)        0 2024-04-05 16:50:20.270527 pyspedas-1.5.7/pyspedas.egg-info/
+-rw-r--r--   0 jwl        (501) wheel        (0)    14462 2024-04-05 16:50:20.000000 pyspedas-1.5.7/pyspedas.egg-info/PKG-INFO
+-rw-r--r--   0 jwl        (501) wheel        (0)    25218 2024-04-05 16:50:20.000000 pyspedas-1.5.7/pyspedas.egg-info/SOURCES.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)        1 2024-04-05 16:50:20.000000 pyspedas-1.5.7/pyspedas.egg-info/dependency_links.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)      161 2024-04-05 16:50:20.000000 pyspedas-1.5.7/pyspedas.egg-info/requires.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)        9 2024-04-05 16:50:20.000000 pyspedas-1.5.7/pyspedas.egg-info/top_level.txt
+-rw-r--r--   0 jwl        (501) wheel        (0)       38 2024-04-05 16:50:20.343509 pyspedas-1.5.7/setup.cfg
+-rwxr-xr-x   0 jwl        (501) wheel        (0)     1384 2024-04-05 16:50:01.000000 pyspedas-1.5.7/setup.py
```

### Comparing `pyspedas-1.5.6/CODE_OF_CONDUCT.md` & `pyspedas-1.5.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/CONTRIBUTING.md` & `pyspedas-1.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/LICENSE.txt` & `pyspedas-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/PKG-INFO` & `pyspedas-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyspedas
-Version: 1.5.6
+Version: 1.5.7
 Summary: Python Space Physics Environment Data Analysis Software (pySPEDAS)
 Home-page: https://github.com/spedas/pyspedas
 Author: Jim Lewis
 Author-email: jwl@ssl.berkeley.edu
 License: MIT
 Project-URL: Information, http://spedas.org/wiki/
 Keywords: spedas data tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # PySPEDAS
 [![build](https://github.com/spedas/pyspedas/workflows/build/badge.svg)](https://github.com/spedas/pyspedas/actions)
 [![Coverage Status](https://coveralls.io/repos/github/spedas/pyspedas/badge.svg)](https://coveralls.io/github/spedas/pyspedas)
@@ -62,15 +62,15 @@
 - [Ulysses](https://pyspedas.readthedocs.io/en/latest/ulysses.html)
 - [Van Allen Probes (RBSP)](https://pyspedas.readthedocs.io/en/latest/rbsp.html)
 - [Wind](https://pyspedas.readthedocs.io/en/latest/wind.html)
 
 
 ## Requirements
 
-Python 3.8+ is required.
+Python 3.9+ is required.
 
 We recommend [Anaconda](https://www.continuum.io/downloads/) which comes with a suite of packages useful for scientific data analysis. Step-by-step instructions for installing Anaconda can be found at: [Windows](https://docs.anaconda.com/anaconda/install/windows/), [macOS](https://docs.anaconda.com/anaconda/install/mac-os/), [Linux](https://docs.anaconda.com/anaconda/install/linux/)
 
 
 ## Installation
 
 ### Virtual Environment
```

### Comparing `pyspedas-1.5.6/README.md` & `pyspedas-1.5.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 - [Ulysses](https://pyspedas.readthedocs.io/en/latest/ulysses.html)
 - [Van Allen Probes (RBSP)](https://pyspedas.readthedocs.io/en/latest/rbsp.html)
 - [Wind](https://pyspedas.readthedocs.io/en/latest/wind.html)
 
 
 ## Requirements
 
-Python 3.8+ is required.
+Python 3.9+ is required.
 
 We recommend [Anaconda](https://www.continuum.io/downloads/) which comes with a suite of packages useful for scientific data analysis. Step-by-step instructions for installing Anaconda can be found at: [Windows](https://docs.anaconda.com/anaconda/install/windows/), [macOS](https://docs.anaconda.com/anaconda/install/mac-os/), [Linux](https://docs.anaconda.com/anaconda/install/linux/)
 
 
 ## Installation
 
 ### Virtual Environment
```

### Comparing `pyspedas-1.5.6/pyspedas/__init__.py` & `pyspedas-1.5.7/pyspedas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .hapi.hapi import hapi
 from .utilities.spice.time_ephemeris import time_ephemeris
 from .utilities.dailynames import dailynames
 from .utilities.datasets import find_datasets
 # Note: "download" and "download_file" might be problematic names to import, due to risk of conflict with other packages
 from .utilities.download import download, download_file, check_downloaded_file
 from .utilities.download_ftp import download_ftp
+from .utilities.find_ip_address import find_ip_address
 from .utilities.interpol import interpol
 from .utilities.leap_seconds import load_leap_table
 from .utilities.libs import libs
 from .utilities.mpause_2 import mpause_2
 from .utilities.mpause_t96 import mpause_t96
 from .utilities.tcopy import tcopy
 from .version import version
@@ -64,15 +65,15 @@
     mms_load_dsp, mms_load_fsm, mms_load_state, \
     mms_qcotrans, mms_cotrans_lmn, mms_cotrans_qrotate, mms_cotrans_qtransformer
 from .mms.feeps.mms_feeps_pad import mms_feeps_pad
 from .mms.feeps.mms_feeps_gpd import mms_feeps_gpd
 from .mms.eis.mms_eis_pad import mms_eis_pad
 from .mms.hpca.mms_hpca_calc_anodes import mms_hpca_calc_anodes
 from .mms.hpca.mms_hpca_spin_sum import mms_hpca_spin_sum
-from .mms.mms_overview_plot import mms_overview_plot
+from .mms.plots.mms_overview_plot import mms_overview_plot
 from .mms.particles.mms_part_getspec import mms_part_getspec
 from .mms.particles.mms_part_slice2d import mms_part_slice2d
 from .maven import maven_load
 from .sosmag.load import sosmag_load
 from .noaa import noaa_load_kp
 
 # Make mission-specific namespaces available under pyspedas
```

### Comparing `pyspedas-1.5.6/pyspedas/ace/__init__.py` & `pyspedas-1.5.7/pyspedas/ace/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/ace/load.py` & `pyspedas-1.5.7/pyspedas/ace/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/ace/tests/tests.py` & `pyspedas-1.5.7/pyspedas/ace/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/akebono/__init__.py` & `pyspedas-1.5.7/pyspedas/akebono/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/akebono/load.py` & `pyspedas-1.5.7/pyspedas/akebono/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/akebono/tests/tests.py` & `pyspedas-1.5.7/pyspedas/akebono/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/avg_data.py` & `pyspedas-1.5.7/pyspedas/analysis/avg_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/deriv_data.py` & `pyspedas-1.5.7/pyspedas/analysis/deriv_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 
 import pyspedas
 import pytplot
 
 
-def deriv_data(names, newname=None, new_names=None, suffix=None, overwrite=None):
+def deriv_data(names, newname=None, new_names=None, suffix=None, overwrite=None, edge_order=1):
     """
     Compute the derivative.
 
     Parameters
     ----------
     names: str/list of str
         List of pytplot names.
@@ -65,10 +65,12 @@
         n_names = [n_names]
 
     if len(n_names) != len(old_names):
         n_names = [s + suffix for s in old_names]
 
     for i, old in enumerate(old_names):
         data = pytplot.get_data(old)
-        data_grad = np.gradient(data.y, data.times, axis = 0)
+        data_grad = np.gradient(data.y, data.times, axis = 0, edge_order=edge_order)
         pytplot.store_data(n_names[i], data={'x': data.times, 'y': data_grad})
         logging.info('deriv_data was applied to: ' + n_names[i])
+
+    return n_names
```

### Comparing `pyspedas-1.5.6/pyspedas/analysis/dpwrspc.py` & `pyspedas-1.5.7/pyspedas/analysis/dpwrspc.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/find_magnetic_nulls.py` & `pyspedas-1.5.7/pyspedas/analysis/find_magnetic_nulls.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/lingradest.py` & `pyspedas-1.5.7/pyspedas/analysis/lingradest.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/neutral_sheet.py` & `pyspedas-1.5.7/pyspedas/analysis/neutral_sheet.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tdeflag.py` & `pyspedas-1.5.7/pyspedas/analysis/tdeflag.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tdpwrspc.py` & `pyspedas-1.5.7/pyspedas/analysis/tdpwrspc.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tests/test_magnetic_nulls.py` & `pyspedas-1.5.7/pyspedas/analysis/tests/test_magnetic_nulls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 
 import unittest
 import pyspedas
 from pytplot import data_exists, tplot, get_data
 import numpy as np
 
+# Set this to False for Github CI testing, True to show the plots for interactive use
+global_display=False
+
 class MagNullTestCases(unittest.TestCase):
 
 
     def test_null_classification_x(self):
         # Test direct detection of 2-D type X nulls. (This will seldom or never occur in practice,
         # but see below for some degenerate cases that do appear in real data.
         l1 = complex(0.0,0.0)
@@ -107,28 +110,28 @@
 
 
     def test_find_magnetic_nulls_fote_mms(self):
         data = pyspedas.mms.fgm(probe=[1, 2, 3, 4], trange=['2015-09-19/07:40', '2015-09-19/07:45'], data_rate='srvy', time_clip=True, varformat='*_gse_*', get_fgm_ephemeris=True)
         fields = ['mms'+prb+'_fgm_b_gse_srvy_l2' for prb in ['1', '2', '3', '4']]
         positions = ['mms'+prb+'_fgm_r_gse_srvy_l2' for prb in ['1', '2', '3', '4']]
         null_vars = pyspedas.find_magnetic_nulls_fote(fields=fields, positions=positions, smooth_fields=True,smooth_npts=10,smooth_median=True)
-        #tplot(null_vars)
+        tplot(null_vars,save_png='magnetic_null_vars',display=global_display)
         # We reconstruct the field vectors at the s/c positions using the Jacobian and the field value at the tetrahedron
         # barycenter.  The max difference between the observations and the reconstructed values for each time step
         # should be extremely close to zero, so that's what we'll use for our test.
         d=get_data('max_reconstruction_error')
         np.testing.assert_allclose(d.y,0.0,atol=1.0e-10)
 
     def test_find_magnetic_nulls_fote_cluster(self):
         data = pyspedas.cluster.load_csa(probes=['C1','C2','C3','C4'],trange=['2003-08-17/16:40', '2003-08-17/16:45'],datatypes='CP_FGM_FULL', time_clip=True)
         #tplot_names()
         fields = ['B_vec_xyz_gse__C'+prb+'_CP_FGM_FULL' for prb in ['1', '2', '3', '4']]
         positions = ['sc_pos_xyz_gse__C'+prb+'_CP_FGM_FULL' for prb in ['1', '2', '3', '4']]
         null_vars = pyspedas.find_magnetic_nulls_fote(fields=fields, positions=positions, smooth_fields=True)
-        #tplot(null_vars)
+        tplot(null_vars,display=global_display,save_png='cluster_null_vars')
         d=get_data('max_reconstruction_error')
         np.testing.assert_allclose(d.y,0.0,atol=1.0e-10)
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tests/test_twavpol.py` & `pyspedas-1.5.7/pyspedas/analysis/tests/test_twavpol.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tests/tests.py` & `pyspedas-1.5.7/pyspedas/analysis/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/time_domain_filter.py` & `pyspedas-1.5.7/pyspedas/analysis/time_domain_filter.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tinterpol.py` & `pyspedas-1.5.7/pyspedas/analysis/tinterpol.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/tvectot.py` & `pyspedas-1.5.7/pyspedas/analysis/tvectot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/twavpol.py` & `pyspedas-1.5.7/pyspedas/analysis/twavpol.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/wavelet.py` & `pyspedas-1.5.7/pyspedas/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/analysis/yclip.py` & `pyspedas-1.5.7/pyspedas/analysis/yclip.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/barrel/__init__.py` & `pyspedas-1.5.7/pyspedas/barrel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/barrel/config.py` & `pyspedas-1.5.7/pyspedas/barrel/config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/barrel/load.py` & `pyspedas-1.5.7/pyspedas/barrel/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cdagui/cdagui.py` & `pyspedas-1.5.7/pyspedas/cdagui/cdagui.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cdagui/cdaweb.py` & `pyspedas-1.5.7/pyspedas/cdagui/cdaweb.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cluster/__init__.py` & `pyspedas-1.5.7/pyspedas/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cluster/load.py` & `pyspedas-1.5.7/pyspedas/cluster/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cluster/load_csa.py` & `pyspedas-1.5.7/pyspedas/cluster/load_csa.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cluster/tests/tests.py` & `pyspedas-1.5.7/pyspedas/cluster/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cnofs/__init__.py` & `pyspedas-1.5.7/pyspedas/cnofs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cnofs/load.py` & `pyspedas-1.5.7/pyspedas/cnofs/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cnofs/tests/tests.py` & `pyspedas-1.5.7/pyspedas/cnofs/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/cart2spc.py` & `pyspedas-1.5.7/pyspedas/cotrans/cart2spc.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/cotrans.py` & `pyspedas-1.5.7/pyspedas/cotrans/cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/cotrans_lib.py` & `pyspedas-1.5.7/pyspedas/cotrans/cotrans_lib.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/fac_matrix_make.py` & `pyspedas-1.5.7/pyspedas/cotrans/fac_matrix_make.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/gsm2lmn.py` & `pyspedas-1.5.7/pyspedas/cotrans/gsm2lmn.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/igrf.py` & `pyspedas-1.5.7/pyspedas/cotrans/igrf.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/j2000.py` & `pyspedas-1.5.7/pyspedas/cotrans/j2000.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/matrix_array_lib.py` & `pyspedas-1.5.7/pyspedas/cotrans/matrix_array_lib.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/minvar.py` & `pyspedas-1.5.7/pyspedas/cotrans/minvar.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/minvar_matrix_make.py` & `pyspedas-1.5.7/pyspedas/cotrans/minvar_matrix_make.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/quaternions.py` & `pyspedas-1.5.7/pyspedas/cotrans/quaternions.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/sm2mlt.py` & `pyspedas-1.5.7/pyspedas/cotrans/sm2mlt.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/spc2cart.py` & `pyspedas-1.5.7/pyspedas/cotrans/spc2cart.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/tests/cotrans.py` & `pyspedas-1.5.7/pyspedas/cotrans/tests/cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/tests/quaternions.py` & `pyspedas-1.5.7/pyspedas/cotrans/tests/quaternions.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/tests/test_minvar.py` & `pyspedas-1.5.7/pyspedas/cotrans/tests/test_minvar.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/tvector_rotate.py` & `pyspedas-1.5.7/pyspedas/cotrans/tvector_rotate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/cotrans/xyz_to_polar.py` & `pyspedas-1.5.7/pyspedas/cotrans/xyz_to_polar.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/csswe/__init__.py` & `pyspedas-1.5.7/pyspedas/csswe/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/csswe/load.py` & `pyspedas-1.5.7/pyspedas/csswe/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/csswe/tests/tests.py` & `pyspedas-1.5.7/pyspedas/csswe/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/de2/__init__.py` & `pyspedas-1.5.7/pyspedas/de2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/de2/load.py` & `pyspedas-1.5.7/pyspedas/de2/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/de2/tests/tests.py` & `pyspedas-1.5.7/pyspedas/de2/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/dscovr/__init__.py` & `pyspedas-1.5.7/pyspedas/dscovr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/dscovr/load.py` & `pyspedas-1.5.7/pyspedas/dscovr/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/dscovr/tests/tests.py` & `pyspedas-1.5.7/pyspedas/dscovr/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/__init__.py` & `pyspedas-1.5.7/pyspedas/elfin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/eng/eng.py` & `pyspedas-1.5.7/pyspedas/elfin/eng/eng.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/epd/calibration_l1.py` & `pyspedas-1.5.7/pyspedas/elfin/epd/calibration_l1.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/epd/calibration_l2.py` & `pyspedas-1.5.7/pyspedas/elfin/epd/calibration_l2.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/epd/elb_epde_cal_data.txt` & `pyspedas-1.5.7/pyspedas/elfin/epd/elb_epde_cal_data.txt`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/epd/epd.py` & `pyspedas-1.5.7/pyspedas/elfin/epd/epd.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/epd/postprocessing.py` & `pyspedas-1.5.7/pyspedas/elfin/epd/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/fgm/fgm.py` & `pyspedas-1.5.7/pyspedas/elfin/fgm/fgm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/load.py` & `pyspedas-1.5.7/pyspedas/elfin/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/mrma/mrma.py` & `pyspedas-1.5.7/pyspedas/elfin/mrma/mrma.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/mrmi/mrmi.py` & `pyspedas-1.5.7/pyspedas/elfin/mrmi/mrmi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/state/state.py` & `pyspedas-1.5.7/pyspedas/elfin/state/state.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_calibration.py` & `pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_calibration.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_l1.py` & `pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_l1.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/tests/test_epd_l2.py` & `pyspedas-1.5.7/pyspedas/elfin/tests/test_epd_l2.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/tests/test_state.py` & `pyspedas-1.5.7/pyspedas/elfin/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/elfin/tests/tests.py` & `pyspedas-1.5.7/pyspedas/elfin/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/equator_s/__init__.py` & `pyspedas-1.5.7/pyspedas/equator_s/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/equator_s/load.py` & `pyspedas-1.5.7/pyspedas/equator_s/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/equator_s/tests/tests.py` & `pyspedas-1.5.7/pyspedas/equator_s/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/__init__.py` & `pyspedas-1.5.7/pyspedas/erg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/config.py` & `pyspedas-1.5.7/pyspedas/erg/config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/camera/camera_omti_asi.py` & `pyspedas-1.5.7/pyspedas/erg/ground/camera/camera_omti_asi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cdflib
 import numpy as np
 
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
-
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 from typing import List, Union, Optional
 
 def camera_omti_asi(
     trange: List[str] = ['2020-08-01', '2020-08-02'],
     suffix: str = '',
     site: Union[str, List[str]] = 'all',
@@ -137,22 +137,15 @@
             
             if notplot:
                 loaded_data.update(loaded_data_temp)
             else:
                 loaded_data += loaded_data_temp
             if (len(loaded_data_temp) > 0) and ror:
                 try:
-                    if isinstance(loaded_data_temp, list):
-                        if downloadonly:
-                            cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                            gatt = cdf_file.globalattsget()
-                        else:
-                            gatt = get_data(loaded_data_temp[-1], metadata=True)['CDF']['GATT']
-                    elif isinstance(loaded_data_temp, dict):
-                        gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]]['CDF']['GATT']
+                    gatt = get_gatt_ror(downloadonly, loaded_data)
                     print('**************************************************************************')
                     print(gatt["Logical_source_description"])
                     print('')
                     print(f'Information about {gatt["Station_code"]}')
                     print(f'PI: {gatt["PI_name"]}')
                     print('')
                     print(f'Affiliations: {gatt["PI_affiliation"]}')
@@ -204,28 +197,27 @@
                         file_name = get_data(current_tplot_name,
                                             metadata=True)['CDF']['FILENAME']
                         if isinstance(file_name, list):
                             if len(file_name) > 0:
                                 file_name = file_name[0]
                         cdf_file = cdflib.CDF(file_name)
                         cdf_info = cdf_file.cdf_info()
-                        all_cdf_variables = cdf_info['rVariables'] + cdf_info['zVariables']
+                        all_cdf_variables = cdf_info.rVariables + cdf_info.zVariables
                         if 'image_raw' in all_cdf_variables:
                             var_string = 'image_raw'
                             var_properties = cdf_file.varinq(var_string)
-                            if 'Data_Type_Description' in var_properties:
-                                original_datatype_string = var_properties['Data_Type_Description']
-                                if original_datatype_string == 'CDF_INT4':
-                                    image_y_transpose = image_y_transpose.astype(np.int32)
-                                elif original_datatype_string == 'CDF_UINT1':
-                                    image_y_transpose = image_y_transpose.astype(np.uint8)
-                                elif original_datatype_string == 'CDF_UINT2':
-                                    image_y_transpose = image_y_transpose.astype(np.uint16)
-                                elif original_datatype_string == 'CDF_UINT4':
-                                    image_y_transpose = image_y_transpose.astype(np.uint32)
+                            original_datatype_string = var_properties.Data_Type_Description
+                            if original_datatype_string == 'CDF_INT4':
+                                image_y_transpose = image_y_transpose.astype(np.int32)
+                            elif original_datatype_string == 'CDF_UINT1':
+                                image_y_transpose = image_y_transpose.astype(np.uint8)
+                            elif original_datatype_string == 'CDF_UINT2':
+                                image_y_transpose = image_y_transpose.astype(np.uint16)
+                            elif original_datatype_string == 'CDF_UINT4':
+                                image_y_transpose = image_y_transpose.astype(np.uint32)
 
                         get_metadata_vars = get_data(current_tplot_name, metadata=True)
                         store_data(current_tplot_name,
                                    data={'x':get_data_vars[0],
                                          'y':image_y_transpose},
                                    attr_dict=get_metadata_vars)
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_isee_fluxgate.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_isee_fluxgate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import cdflib
 import numpy as np
 
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
-
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 from typing import List, Union, Optional, Dict, Any
 
 def gmag_isee_fluxgate(
     trange: List[str] = ['2020-08-01', '2020-08-02'],
     suffix: str = '',
     site: Union[str, List[str]] = 'all',
@@ -157,22 +156,15 @@
             
             if notplot:
                 loaded_data.update(loaded_data_temp)
             else:
                 loaded_data += loaded_data_temp
             if (len(loaded_data_temp) > 0) and ror:
                 try:
-                    if isinstance(loaded_data_temp, list):
-                        if downloadonly:
-                            cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                            gatt = cdf_file.globalattsget()
-                        else:
-                            gatt = get_data(loaded_data_temp[-1], metadata=True)['CDF']['GATT']
-                    elif isinstance(loaded_data_temp, dict):
-                        gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]]['CDF']['GATT']
+                    gatt = get_gatt_ror(downloadonly, loaded_data)
                     print('**************************************************************************')
                     print(gatt["Logical_source_description"])
                     print('')
                     print(f'Information about {gatt["Station_code"]}')
                     print('PI and Host PI(s):')
                     print(gatt["PI_name"])
                     print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_isee_induction.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_isee_induction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import cdflib
 import numpy as np
 
 from copy import deepcopy
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional, Union
 
+
 def gmag_isee_induction(
     trange: List[str] = ["2018-10-18/00:00:00", "2018-10-18/02:00:00"],
     suffix: str = "",
     site: Union[str, List[str]] = "all",
     get_support_data: bool = False,
     varformat: Optional[str] = None,
     varnames: List[str] = [],
@@ -165,26 +167,15 @@
 
         if notplot:
             loaded_data.update(loaded_data_temp)
         else:
             loaded_data += loaded_data_temp
         if (len(loaded_data_temp) > 0) and ror:
             try:
-                if isinstance(loaded_data_temp, list):
-                    if downloadonly:
-                        cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                        gatt = cdf_file.globalattsget()
-                    else:
-                        gatt = get_data(loaded_data_temp[-1], metadata=True)["CDF"][
-                            "GATT"
-                        ]
-                elif isinstance(loaded_data_temp, dict):
-                    gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]]["CDF"][
-                        "GATT"
-                    ]
+                gatt = get_gatt_ror(downloadonly, loaded_data)
                 print(
                     "**************************************************************************"
                 )
                 print(gatt["Logical_source_description"])
                 print("")
                 print(f'Information about {gatt["Station_code"]}')
                 print("PI and Host PI(s):")
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_magdas_1sec.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_magdas_1sec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import cdflib
 import numpy as np
 
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional, Union
 
+
 def gmag_magdas_1sec(
     trange: List[str] = ["2010-11-20/00:00:00", "2010-11-21/00:00:00"],
     suffix: str = "",
     site: Union[str, List[str]] = "all",
     datatype: Union[str, List[str]] = "1sec",
     get_support_data: bool = False,
     varformat: Optional[str] = None,
@@ -181,29 +182,15 @@
 
             if notplot:
                 loaded_data.update(loaded_data_temp)
             else:
                 loaded_data += loaded_data_temp
             if (len(loaded_data_temp) > 0) and ror:
                 try:
-                    if isinstance(loaded_data_temp, list):
-                        if downloadonly:
-                            cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                            gatt = cdf_file.globalattsget()
-                        else:
-                            gatt = get_data(loaded_data_temp[-1], metadata=True)["CDF"][
-                                "GATT"
-                            ]
-                    elif isinstance(loaded_data_temp, dict):
-                        gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]][
-                            "CDF"
-                        ]["GATT"]
-                    print(
-                        "**************************************************************************"
-                    )
+                    gatt = get_gatt_ror(downloadonly, loaded_data)
                     print(gatt["Logical_source_description"])
                     print("")
                     print(f'Information about {gatt["Station_code"]}')
                     print(f'PI and Host PI(s): {gatt["PI_name"]}')
                     print("")
                     print("Affiliations: ")
                     print(gatt["PI_affiliation"])
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_mm210.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_mm210.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-import cdflib
 import numpy as np
 
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional, Union
 
+
 def gmag_mm210(
-    trange: List[str] = ['2020-08-01', '2020-08-02'],
-    suffix: str = '',
-    site: Union[str, List[str]] = 'all',
-    datatype: Union[str, List[str]] = 'all',
+    trange: List[str] = ["2020-08-01", "2020-08-02"],
+    suffix: str = "",
+    site: Union[str, List[str]] = "all",
+    datatype: Union[str, List[str]] = "all",
     get_support_data: bool = False,
     varformat: Optional[str] = None,
     varnames: List[str] = [],
     downloadonly: bool = False,
     notplot: bool = False,
     no_update: bool = False,
     uname: Optional[str] = None,
     passwd: Optional[str] = None,
     time_clip: bool = False,
-    ror: bool = True
+    ror: bool = True,
 ) -> List[str]:
     """
     Load mm210 data from ERG Science Center
 
     Parameters
     ----------
     trange: list of str
@@ -94,130 +95,203 @@
     >>> import pyspedas
     >>> from pytplot import tplot
     >>> mm210_vars=pyspedas.erg.gmag_mm210(trange=["2005-01-01", "2005-01-02"],site='adl',datatype='1min')
     >>> tplot('mm210_mag_adl_1min_hdz')
 
     """
 
-    site_code_all = ['tik', 'zgn', 'yak', 'irt', 'ppi', 'bji',
-                    'lnp', 'mut', 'ptn', 'wtk', 'lmt', 'kat',
-                    'ktn', 'chd', 'zyk', 'mgd', 'ptk', 'msr',
-                    'rik', 'onw', 'kag', 'ymk', 'cbi', 'gua',
-                    'yap', 'kor', 'ktb', 'bik', 'wew', 'daw',
-                    'wep', 'bsv', 'dal', 'can', 'adl', 'kot',
-                    'cst', 'ewa', 'asa', 'mcq']
-    tres_all=['1sec', '1min', '1h']
+    site_code_all = [
+        "tik",
+        "zgn",
+        "yak",
+        "irt",
+        "ppi",
+        "bji",
+        "lnp",
+        "mut",
+        "ptn",
+        "wtk",
+        "lmt",
+        "kat",
+        "ktn",
+        "chd",
+        "zyk",
+        "mgd",
+        "ptk",
+        "msr",
+        "rik",
+        "onw",
+        "kag",
+        "ymk",
+        "cbi",
+        "gua",
+        "yap",
+        "kor",
+        "ktb",
+        "bik",
+        "wew",
+        "daw",
+        "wep",
+        "bsv",
+        "dal",
+        "can",
+        "adl",
+        "kot",
+        "cst",
+        "ewa",
+        "asa",
+        "mcq",
+    ]
+    tres_all = ["1sec", "1min", "1h"]
     if isinstance(datatype, str):
         datatype = datatype.lower()
-        datatype = datatype.split(' ')
+        datatype = datatype.split(" ")
     elif isinstance(datatype, list):
         for i in range(len(datatype)):
             datatype[i] = datatype[i].lower()
 
-    if 'all' in datatype:
-        datatype=tres_all
+    if "all" in datatype:
+        datatype = tres_all
     datatype = list(set(datatype).intersection(tres_all))
     if len(datatype) < 1:
         return
 
-    if '1s' in datatype:
-        index = np.where(np.array(datatype) == '1s')[0][0]
-        datatype[index] = '1sec'
-    elif  '1m' in datatype:
-        index = np.where(np.array(datatype) == '1m')[0][0]
-        datatype[index] = '1min'
-    elif  '1hr' in datatype:
-        index = np.where(np.array(datatype) == '1hr')[0][0]
-        datatype[index] = '1h'
+    if "1s" in datatype:
+        index = np.where(np.array(datatype) == "1s")[0][0]
+        datatype[index] = "1sec"
+    elif "1m" in datatype:
+        index = np.where(np.array(datatype) == "1m")[0][0]
+        datatype[index] = "1min"
+    elif "1hr" in datatype:
+        index = np.where(np.array(datatype) == "1hr")[0][0]
+        datatype[index] = "1h"
 
-    
     if isinstance(site, str):
         site_code = site.lower()
-        site_code = site_code.split(' ')
+        site_code = site_code.split(" ")
     elif isinstance(site, list):
         site_code = []
         for i in range(len(site)):
             site_code.append(site[i].lower())
-    if 'all' in site_code:
+    if "all" in site_code:
         site_code = site_code_all
-    
+
     site_code = list(set(site_code).intersection(site_code_all))
 
-    prefix = 'mm210_'
+    prefix = "mm210_"
     if notplot:
         loaded_data = {}
     else:
         loaded_data = []
     for site_input in site_code:
         for data_type_in in datatype:
             fres = data_type_in
 
-            if fres == '1h':
-                fres = '1min'
+            if fres == "1h":
+                fres = "1min"
+
+            file_res = 3600.0 * 24
+            pathformat = (
+                "ground/geomag/mm210/"
+                + fres
+                + "/"
+                + site_input
+                + "/%Y/mm210_"
+                + fres
+                + "_"
+                + site_input
+                + "_%Y%m%d_v??.cdf"
+            )
+
+            loaded_data_temp = load(
+                pathformat=pathformat,
+                file_res=file_res,
+                trange=trange,
+                datatype=datatype,
+                prefix=prefix,
+                suffix="_" + site_input + suffix,
+                get_support_data=get_support_data,
+                varformat=varformat,
+                downloadonly=downloadonly,
+                notplot=notplot,
+                time_clip=time_clip,
+                no_update=no_update,
+                uname=uname,
+                passwd=passwd,
+            )
 
-            file_res = 3600. * 24
-            pathformat = 'ground/geomag/mm210/'+fres+'/'+site_input\
-                            +'/%Y/mm210_'+fres+'_'+site_input+'_%Y%m%d_v??.cdf'
-            
-            loaded_data_temp = load(pathformat=pathformat, file_res=file_res, trange=trange, datatype=datatype, prefix=prefix, suffix='_'+site_input+suffix, get_support_data=get_support_data,
-                            varformat=varformat, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
-            
             if notplot:
                 loaded_data.update(loaded_data_temp)
             else:
                 loaded_data += loaded_data_temp
             if (len(loaded_data_temp) > 0) and ror:
                 try:
-                    if isinstance(loaded_data_temp, list):
-                        if downloadonly:
-                            cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                            gatt = cdf_file.globalattsget()
-                        else:
-                            gatt = get_data(loaded_data_temp[-1], metadata=True)['CDF']['GATT']
-                    elif isinstance(loaded_data_temp, dict):
-                        gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]]['CDF']['GATT']
-                    print('**************************************************************************')
+                    gatt = get_gatt_ror(downloadonly, loaded_data)
+                    print(
+                        "**************************************************************************"
+                    )
                     print(gatt["Logical_source_description"])
-                    print('')
+                    print("")
                     print(f'Information about {gatt["Station_code"]}')
-                    print('PI and Host PI(s):')
+                    print("PI and Host PI(s):")
                     print(gatt["PI_name"])
-                    print('')
-                    print('Affiliations: ')
+                    print("")
+                    print("Affiliations: ")
                     print(gatt["PI_affiliation"])
-                    print('')
-                    print('Rules of the Road for 210 MM Data Use:')
+                    print("")
+                    print("Rules of the Road for 210 MM Data Use:")
                     for gatt_text in gatt["TEXT"]:
                         print(gatt_text)
                     print(f'{gatt["LINK_TEXT"]} {gatt["HTTP_LINK"]}')
-                    print('**************************************************************************')
+                    print(
+                        "**************************************************************************"
+                    )
                 except:
-                    print('printing PI info and rules of the road was failed')
-                
+                    print("printing PI info and rules of the road was failed")
+
             if (not downloadonly) and (not notplot):
-                if fres == '1min':
-                    fres_list = ['1min', '1h']
+                if fres == "1min":
+                    fres_list = ["1min", "1h"]
                 else:
                     fres_list = [fres]
                 for fres_in in fres_list:
-                    current_tplot_name = prefix+'hdz_'+fres_in+'_' + site_input+suffix
+                    current_tplot_name = (
+                        prefix + "hdz_" + fres_in + "_" + site_input + suffix
+                    )
                     if current_tplot_name in loaded_data:
                         get_data_vars = get_data(current_tplot_name)
                         if get_data_vars is None:
                             store_data(current_tplot_name, delete=True)
                         else:
-                            #;--- Rename
-                            new_tplot_name = prefix+'mag_'+site_input+'_'+fres_in+'_hdz'+suffix
+                            # ;--- Rename
+                            new_tplot_name = (
+                                prefix
+                                + "mag_"
+                                + site_input
+                                + "_"
+                                + fres_in
+                                + "_hdz"
+                                + suffix
+                            )
                             store_data(current_tplot_name, newname=new_tplot_name)
                             loaded_data.remove(current_tplot_name)
                             loaded_data.append(new_tplot_name)
-                            #;--- Missing data -1.e+31 --> NaN
-                            clip(new_tplot_name, -1e+4, 1e+4)
+                            # ;--- Missing data -1.e+31 --> NaN
+                            clip(new_tplot_name, -1e4, 1e4)
                             get_data_vars = get_data(new_tplot_name)
-                            ylim(new_tplot_name, np.nanmin(get_data_vars[1]), np.nanmax(get_data_vars[1]))
-                            #;--- Labels
-                            options(new_tplot_name, 'legend_names', ['Ch1','Ch2','Ch3'])
-                            options(new_tplot_name, 'Color', ['b', 'g', 'r'])
-                            options(new_tplot_name, 'ytitle', '\n'.join(new_tplot_name.split('_')))
-
+                            ylim(
+                                new_tplot_name,
+                                np.nanmin(get_data_vars[1]),
+                                np.nanmax(get_data_vars[1]),
+                            )
+                            # ;--- Labels
+                            options(
+                                new_tplot_name, "legend_names", ["Ch1", "Ch2", "Ch3"]
+                            )
+                            options(new_tplot_name, "Color", ["b", "g", "r"])
+                            options(
+                                new_tplot_name,
+                                "ytitle",
+                                "\n".join(new_tplot_name.split("_")),
+                            )
 
     return loaded_data
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_stel_fluxgate.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_stel_fluxgate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/geomag/gmag_stel_induction.py` & `pyspedas-1.5.7/pyspedas/erg/ground/geomag/gmag_stel_induction.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/radar/superdarn/get_sphcntr.py` & `pyspedas-1.5.7/pyspedas/erg/ground/radar/superdarn/get_sphcntr.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/riometer/isee_brio.py` & `pyspedas-1.5.7/pyspedas/erg/ground/riometer/isee_brio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import cdflib
 import numpy as np
 
 from copy import deepcopy
 from pytplot import get_data, store_data, options, clip, ylim
 
 from ...satellite.erg.load import load
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional, Union
 
+
 def isee_brio(
-    trange: List[str] = ['2020-08-01', '2020-08-02'],
-    suffix: str = '',
-    site: Union[str, List[str]] = 'all',
+    trange: List[str] = ["2020-08-01", "2020-08-02"],
+    suffix: str = "",
+    site: Union[str, List[str]] = "all",
     get_support_data: bool = False,
     varformat: Optional[str] = None,
     varnames: List[str] = [],
     downloadonly: bool = False,
     notplot: bool = False,
     no_update: bool = False,
     uname: Optional[str] = None,
     passwd: Optional[str] = None,
     time_clip: bool = False,
-    ror: bool = True
+    ror: bool = True,
 ) -> List[str]:
     """
     Load isee_brio riometer data from ERG Science Center
 
     Parameters
     ----------
     trange: list of str
@@ -83,134 +85,201 @@
     ________
     >>> import pyspedas
     >>> brio_vars=pyspedas.erg.isee_brio(trange=['2020-08-01', '2020-08-02'],site='ath')
     >>> print(brio_vars)
 
     """
 
-    #;----- datatype -----;
-    datatype='64hz'
-    instr='brio'
-    freq='30'
-    
-    site_code_all = ['ath', 'kap', 'gak', 'hus', 'zgn', 'ist']
+    # ;----- datatype -----;
+    datatype = "64hz"
+    instr = "brio"
+    freq = "30"
+
+    site_code_all = ["ath", "kap", "gak", "hus", "zgn", "ist"]
     if isinstance(site, str):
         site_code = site.lower()
-        site_code = site_code.split(' ')
+        site_code = site_code.split(" ")
     elif isinstance(site, list):
         site_code = []
         for i in range(len(site)):
             site_code.append(site[i].lower())
-    if 'all' in site_code:
+    if "all" in site_code:
         site_code = site_code_all
-    
+
     site_code = list(set(site_code).intersection(site_code_all))
 
-    prefix = 'iseetmp_'
+    prefix = "iseetmp_"
     if notplot:
         loaded_data = {}
     else:
         loaded_data = []
     for site_input in site_code:
         fres = datatype
-        file_res = 3600. * 24
-        pathformat = 'ground/riometer/'+site_input\
-                        +'/%Y/isee_'+fres+'_'+instr+freq+'_'+site_input+'_%Y%m%d_v??.cdf'
-        
-        loaded_data_temp = load(pathformat=pathformat, file_res=file_res, trange=trange, datatype=datatype, prefix=prefix, suffix='_' + site_input +suffix, get_support_data=get_support_data,
-                        varformat=varformat, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
-        
+        file_res = 3600.0 * 24
+        pathformat = (
+            "ground/riometer/"
+            + site_input
+            + "/%Y/isee_"
+            + fres
+            + "_"
+            + instr
+            + freq
+            + "_"
+            + site_input
+            + "_%Y%m%d_v??.cdf"
+        )
+
+        loaded_data_temp = load(
+            pathformat=pathformat,
+            file_res=file_res,
+            trange=trange,
+            datatype=datatype,
+            prefix=prefix,
+            suffix="_" + site_input + suffix,
+            get_support_data=get_support_data,
+            varformat=varformat,
+            downloadonly=downloadonly,
+            notplot=notplot,
+            time_clip=time_clip,
+            no_update=no_update,
+            uname=uname,
+            passwd=passwd,
+        )
+
         if notplot:
             loaded_data.update(loaded_data_temp)
         else:
             loaded_data += loaded_data_temp
         if (len(loaded_data_temp) > 0) and ror:
             try:
-                if isinstance(loaded_data_temp, list):
-                    if downloadonly:
-                        cdf_file = cdflib.CDF(loaded_data_temp[-1])
-                        gatt = cdf_file.globalattsget()
-                    else:
-                        gatt = get_data(loaded_data_temp[-1], metadata=True)['CDF']['GATT']
-                elif isinstance(loaded_data_temp, dict):
-                    gatt = loaded_data_temp[list(loaded_data_temp.keys())[-1]]['CDF']['GATT']
-                print('**************************************************************************')
+                gatt = get_gatt_ror(downloadonly, loaded_data)
+                print(
+                    "**************************************************************************"
+                )
                 print(gatt["Logical_source_description"])
-                print('')
+                print("")
                 print(f'Information about {gatt["Station_code"]}')
                 print(f'PI {gatt["PI_name"]}')
-                print('')
+                print("")
                 print(f'Affiliations: {gatt["PI_affiliation"]}')
-                print('')
-                print('Rules of the Road for ISEE Riometer Data:')
-                print('')
+                print("")
+                print("Rules of the Road for ISEE Riometer Data:")
+                print("")
                 print(gatt["TEXT"])
-                print({gatt["LINK_TEXT"]})
-                print('**************************************************************************')
+                print(gatt["LINK_TEXT"])
+                print(
+                    "**************************************************************************"
+                )
             except:
-                print('printing PI info and rules of the road was failed')
-            
+                print("printing PI info and rules of the road was failed")
+
         if (not downloadonly) and (not notplot):
             if len(loaded_data_temp) > 0:
-                file_name = get_data(loaded_data_temp[-1], metadata=True)['CDF']['FILENAME']
+                file_name = get_data(loaded_data_temp[-1], metadata=True)["CDF"][
+                    "FILENAME"
+                ]
                 if isinstance(file_name, list):
                     file_name = file_name[0]
                 cdf_file = cdflib.CDF(file_name)
                 cdf_info = cdf_file.cdf_info()
-                all_cdf_variables = cdf_info['rVariables'] + cdf_info['zVariables']
+                all_cdf_variables = cdf_info.rVariables + cdf_info.zVariables
                 for t_plot_name in loaded_data_temp:
                     get_data_vars = get_data(t_plot_name)
                     if get_data_vars is None:
                         store_data(t_plot_name, delete=True)
                     else:
-                        t_plot_name_split =t_plot_name.split('_')
+                        t_plot_name_split = t_plot_name.split("_")
                         if len(t_plot_name_split) > 2:
-                            #;----- Find param -----;
+                            # ;----- Find param -----;
                             param = t_plot_name_split[1]
-                            if param in ['cna', 'qdc', 'raw']:
-                                #;----- Rename tplot variables -----;
-                                new_tplot_name = 'isee_brio'+freq+'_'+site_input+'_'+fres+'_'+param + suffix
+                            if param in ["cna", "qdc", "raw"]:
+                                # ;----- Rename tplot variables -----;
+                                new_tplot_name = (
+                                    "isee_brio"
+                                    + freq
+                                    + "_"
+                                    + site_input
+                                    + "_"
+                                    + fres
+                                    + "_"
+                                    + param
+                                    + suffix
+                                )
                                 store_data(t_plot_name, newname=new_tplot_name)
                                 loaded_data.remove(t_plot_name)
                                 loaded_data.append(new_tplot_name)
-                                #;----- Missing data -1.e+31 --> NaN -----;
-                                clip(new_tplot_name, -1e+5, 1e+5)
+                                # ;----- Missing data -1.e+31 --> NaN -----;
+                                clip(new_tplot_name, -1e5, 1e5)
                                 get_data_vars = get_data(new_tplot_name)
                                 if param in all_cdf_variables:
                                     var_atts = cdf_file.varattsget(param)
-                                    if "FILLVAL" in var_atts:  #removing "FILLVAL", like 999.9000 or 0.0.
-                                                            #removing process of cdf_to_tplot.py may be not working well.
+                                    if (
+                                        "FILLVAL" in var_atts
+                                    ):  # removing "FILLVAL", like 999.9000 or 0.0.
+                                        # removing process of cdf_to_tplot.py may be not working well.
                                         var_properties = cdf_file.varinq(param)
-                                        if ((var_properties['Data_Type_Description'] ==
-                                                'CDF_FLOAT') or
-                                                (var_properties['Data_Type_Description'] ==
-                                                'CDF_REAL4') or
-                                                (var_properties['Data_Type_Description'] ==
-                                                'CDF_DOUBLE') or
-                                                (var_properties['Data_Type_Description'] ==
-                                                'CDF_REAL8')):
+                                        if (
+                                            (
+                                                var_properties.Data_Type_Description
+                                                == "CDF_FLOAT"
+                                            )
+                                            or (
+                                                var_properties.Data_Type_Description
+                                                == "CDF_REAL4"
+                                            )
+                                            or (
+                                                var_properties.Data_Type_Description
+                                                == "CDF_DOUBLE"
+                                            )
+                                            or (
+                                                var_properties.Data_Type_Description
+                                                == "CDF_REAL8"
+                                            )
+                                        ):
                                             if isinstance(var_atts["FILLVAL"], str):
                                                 fill_value = float(var_atts["FILLVAL"])
                                             else:
-                                                fill_value = deepcopy(var_atts["FILLVAL"])
-                                            new_y = np.where(get_data_vars[1] == fill_value,
-                                                            np.nan, get_data_vars[1])
-                                            get_metadata_vars = get_data(new_tplot_name, metadata=True)
-                                            store_data(new_tplot_name, data={'x':get_data_vars[0],
-                                                                                'y':new_y},
-                                                        attr_dict=get_metadata_vars)
-                                            ylim(new_tplot_name, np.nanmin(new_y), np.nanmax(new_y))
+                                                fill_value = deepcopy(
+                                                    var_atts["FILLVAL"]
+                                                )
+                                            new_y = np.where(
+                                                get_data_vars[1] == fill_value,
+                                                np.nan,
+                                                get_data_vars[1],
+                                            )
+                                            get_metadata_vars = get_data(
+                                                new_tplot_name, metadata=True
+                                            )
+                                            store_data(
+                                                new_tplot_name,
+                                                data={
+                                                    "x": get_data_vars[0],
+                                                    "y": new_y,
+                                                },
+                                                attr_dict=get_metadata_vars,
+                                            )
+                                            ylim(
+                                                new_tplot_name,
+                                                np.nanmin(new_y),
+                                                np.nanmax(new_y),
+                                            )
                                     else:
-                                        ylim(new_tplot_name, np.nanmin(get_data_vars[1]), np.nanmax(get_data_vars[1]))
-                                #;----- Set options -----;
-                                options(new_tplot_name, 'ytitle', site_input.upper())
-                                if param == 'cna':
-                                    options(new_tplot_name, 'ysubtitle', '[dB]')
-                                    options(new_tplot_name, 'legend_names', ['CNA'])
-                                elif param == 'qdc':
-                                    options(new_tplot_name, 'ysubtitle', '[V]')
-                                    options(new_tplot_name, 'legend_names', ['QDC'])
-                                elif param == 'raw':
-                                    options(new_tplot_name, 'ysubtitle', '[V]')
-                                    options(new_tplot_name, 'legend_names', ['Raw data'])
+                                        ylim(
+                                            new_tplot_name,
+                                            np.nanmin(get_data_vars[1]),
+                                            np.nanmax(get_data_vars[1]),
+                                        )
+                                # ;----- Set options -----;
+                                options(new_tplot_name, "ytitle", site_input.upper())
+                                if param == "cna":
+                                    options(new_tplot_name, "ysubtitle", "[dB]")
+                                    options(new_tplot_name, "legend_names", ["CNA"])
+                                elif param == "qdc":
+                                    options(new_tplot_name, "ysubtitle", "[V]")
+                                    options(new_tplot_name, "legend_names", ["QDC"])
+                                elif param == "raw":
+                                    options(new_tplot_name, "ysubtitle", "[V]")
+                                    options(
+                                        new_tplot_name, "legend_names", ["Raw data"]
+                                    )
 
     return loaded_data
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/ground/vlf/isee_vlf.py` & `pyspedas-1.5.7/pyspedas/erg/ground/vlf/isee_vlf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import cdflib
 import numpy as np
 
 from pytplot import tnames
 from pytplot import get_data, store_data, options, clip, ylim, zlim
 
 from ...satellite.erg.load import load
+from ...satellite.erg.get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional, Union
 
+
 def isee_vlf(
-    trange: List[str] = ['2017-03-30/12:00:00', '2017-03-30/15:00:00'],
-    suffix: str = '',
-    site: Union[str, List[str]] = 'all',
+    trange: List[str] = ["2017-03-30/12:00:00", "2017-03-30/15:00:00"],
+    suffix: str = "",
+    site: Union[str, List[str]] = "all",
     get_support_data: bool = False,
     varformat: Optional[str] = None,
     varnames: List[str] = [],
     downloadonly: bool = False,
     notplot: bool = False,
     no_update: bool = False,
     uname: Optional[str] = None,
     passwd: Optional[str] = None,
     time_clip: bool = False,
     ror: bool = True,
-    cal_gain: bool = False
+    cal_gain: bool = False,
 ) -> List[str]:
     """
     Load ISEE VLF data from ERG Science Center
 
     Parameters
     ----------
     trange: list of str
@@ -87,114 +89,135 @@
     ________
     >>> import pyspedas
     >>> vlf_vars=pyspedas.erg.isee_vlf(trange=['2017-03-30/12:00:00', '2017-03-30/15:00:00'],site='ath')
     >>> print(vlf_vars)
 
     """
 
-    site_code_all = ['ath', 'gak', 'hus', 'ist', 'kap', 'mam', 'nai']
+    site_code_all = ["ath", "gak", "hus", "ist", "kap", "mam", "nai"]
 
     if isinstance(site, str):
         site_code = site.lower()
-        site_code = site_code.split(' ')
+        site_code = site_code.split(" ")
     elif isinstance(site, list):
         site_code = []
         for i in range(len(site)):
             site_code.append(site[i].lower())
-    if 'all' in site_code:
+    if "all" in site_code:
         site_code = site_code_all
-    
+
     site_code = list(set(site_code).intersection(site_code_all))
 
     if notplot:
         loaded_data = {}
     else:
         loaded_data = []
     for site_input in site_code:
-        prefix='isee_vlf_'+site_input+'_'
-        file_res = 3600.
-        pathformat = 'ground/vlf/'+site_input\
-                        +'/%Y/%m/isee_vlf_'+site_input+'_%Y%m%d%H_v??.cdf'
-
-        loaded_data_temp = load(pathformat=pathformat, file_res=file_res, trange=trange, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
-                        varformat=varformat, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
-        
+        prefix = "isee_vlf_" + site_input + "_"
+        file_res = 3600.0
+        pathformat = (
+            "ground/vlf/"
+            + site_input
+            + "/%Y/%m/isee_vlf_"
+            + site_input
+            + "_%Y%m%d%H_v??.cdf"
+        )
+
+        loaded_data_temp = load(
+            pathformat=pathformat,
+            file_res=file_res,
+            trange=trange,
+            prefix=prefix,
+            suffix=suffix,
+            get_support_data=get_support_data,
+            varformat=varformat,
+            downloadonly=downloadonly,
+            notplot=notplot,
+            time_clip=time_clip,
+            no_update=no_update,
+            uname=uname,
+            passwd=passwd,
+        )
+
         if notplot:
             loaded_data.update(loaded_data_temp)
         else:
             loaded_data += loaded_data_temp
         if (len(loaded_data_temp) > 0) and ror:
             try:
-                if isinstance(loaded_data_temp, list):
-                    if downloadonly:
-                        cdf_file = cdflib.CDF(loaded_data_temp[0])
-                        gatt = cdf_file.globalattsget()
-                    else:
-                        gatt = get_data(loaded_data_temp[0], metadata=True)['CDF']['GATT']
-                elif isinstance(loaded_data_temp, dict):
-                    gatt = loaded_data_temp[list(loaded_data_temp.keys())[0]]['CDF']['GATT']
-                print('**************************************************************************')
+                # Most of the load routines use the last variable loaded to get the ROR metadata, but in this
+                # case, it seems to want the first variable instead.  So we'll only pass that one.
+
+                gatt = get_gatt_ror(downloadonly, [loaded_data[0]])
+                print(
+                    "**************************************************************************"
+                )
                 print(gatt["Logical_source_description"])
-                print('')
+                print("")
                 print(f'Information about {gatt["Station_code"]}')
                 print(f'PI {gatt["PI_name"]}')
-                print('')
+                print("")
                 print(f'Affiliations: {gatt["PI_affiliation"]}')
-                print('')
-                print('Rules of the Road for ISEE VLF Data Use:')
-                print('')
+                print("")
+                print("Rules of the Road for ISEE VLF Data Use:")
+                print("")
                 for gatt_text in gatt["TEXT"]:
                     print(gatt_text)
-                print({gatt["LINK_TEXT"]})
-                print('**************************************************************************')
+                print(gatt["LINK_TEXT"])
+                print(
+                    "**************************************************************************"
+                )
             except:
-                print('printing PI info and rules of the road was failed')
-            
+                print("printing PI info and rules of the road was failed")
+
         if (not downloadonly) and (not notplot):
-            t_plot_name_list = list(set(tnames([prefix+'ch1'+suffix, 
-                                    prefix+'ch2'+suffix])).intersection(loaded_data))
-            options(t_plot_name_list, 'zlog', 1)
-            options(t_plot_name_list, 'ytitle', 'Frequency [Hz]')
-            options(t_plot_name_list, 'ysubtitle','')
+            t_plot_name_list = list(
+                set(
+                    tnames([prefix + "ch1" + suffix, prefix + "ch2" + suffix])
+                ).intersection(loaded_data)
+            )
+            options(t_plot_name_list, "zlog", 1)
+            options(t_plot_name_list, "ytitle", "Frequency [Hz]")
+            options(t_plot_name_list, "ysubtitle", "")
             if not cal_gain:
-                options(t_plot_name_list, 'ztitle', 'V^2/Hz')
+                options(t_plot_name_list, "ztitle", "V^2/Hz")
             else:
-                print('Calibrating the gain of VLF antenna system...')
-                file_name = get_data(t_plot_name_list[0], metadata=True)['CDF']['FILENAME']
+                print("Calibrating the gain of VLF antenna system...")
+                file_name = get_data(t_plot_name_list[0], metadata=True)["CDF"][
+                    "FILENAME"
+                ]
                 if isinstance(file_name, list):
                     file_name = file_name[0]
                 cdf_file = cdflib.CDF(file_name)
-                
-                ffreq=cdf_file.varget('freq_vlf')
-                gain_ch1=cdf_file.varget('amplitude_cal_vlf_ch1')
-                gain_ch2=cdf_file.varget('amplitude_cal_vlf_ch2')
 
-                gain_ch1_mod = np.interp(ffreq, gain_ch1[0], gain_ch1[1]) * 1.e-9
-                gain_ch2_mod = np.interp(ffreq, gain_ch2[0], gain_ch2[1]) * 1.e-9
+                ffreq = cdf_file.varget("freq_vlf")
+                gain_ch1 = cdf_file.varget("amplitude_cal_vlf_ch1")
+                gain_ch2 = cdf_file.varget("amplitude_cal_vlf_ch2")
+
+                gain_ch1_mod = np.interp(ffreq, gain_ch1[0], gain_ch1[1]) * 1.0e-9
+                gain_ch2_mod = np.interp(ffreq, gain_ch2[0], gain_ch2[1]) * 1.0e-9
 
-                t_plot_name = prefix+'ch1' + suffix
+                t_plot_name = prefix + "ch1" + suffix
                 tmp1 = get_data(t_plot_name)
                 if tmp1 is not None:
                     tmp1_metadata = get_data(t_plot_name, metadata=True)
-                    tmp1_y = tmp1[1] / gain_ch1_mod/gain_ch1_mod
-                    store_data(t_plot_name,
-                                data={'x':tmp1[0],
-                                      'y':tmp1_y,
-                                      'v':tmp1[2]},
-                                attr_dict=tmp1_metadata)
+                    tmp1_y = tmp1[1] / gain_ch1_mod / gain_ch1_mod
+                    store_data(
+                        t_plot_name,
+                        data={"x": tmp1[0], "y": tmp1_y, "v": tmp1[2]},
+                        attr_dict=tmp1_metadata,
+                    )
 
-                t_plot_name = prefix+'ch2' + suffix
+                t_plot_name = prefix + "ch2" + suffix
                 tmp2 = get_data(t_plot_name)
                 if tmp2 is not None:
                     tmp2_metadata = get_data(t_plot_name, metadata=True)
-                    tmp2_y = tmp1[1] / gain_ch2_mod/gain_ch2_mod
-                    store_data(t_plot_name,
-                                data={'x':tmp2[0],
-                                      'y':tmp2_y,
-                                      'v':tmp2[2]},
-                                attr_dict=tmp2_metadata)
-
-                options(t_plot_name_list, 'ztitle', 'nT^2/Hz')
-
+                    tmp2_y = tmp1[1] / gain_ch2_mod / gain_ch2_mod
+                    store_data(
+                        t_plot_name,
+                        data={"x": tmp2[0], "y": tmp2_y, "v": tmp2[2]},
+                        attr_dict=tmp2_metadata,
+                    )
 
+                options(t_plot_name_list, "ztitle", "nT^2/Hz")
 
     return loaded_data
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/att/att.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/att/att.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     trange: List[str] = ['2017-04-01', '2017-04-02'],
     level: str = 'l2',
     downloadonly: bool = False,
     notplot: bool = False,
     no_update: bool = False,
     uname: Optional[str] = None,
     passwd: Optional[str] = None
-) -> None:
+) -> List[str]:
     """
     This function loads attitude data from the Arase mission
 
     Parameters
     ----------
         trange : list of str
             time range of interest [starttime, endtime] with the format
@@ -45,15 +45,16 @@
             User name. Default: None
 
         passwd: str
             Password. Default: None
 
     Returns
     -------
-        None
+        list of str
+            List of tplot variables loaded
 
     Examples
     --------
     >>> import pyspedas
     >>> from pytplot import tplot
     >>> att_vars = pyspedas.erg.att(trange=['2017-04-01', '2017-04-02'])
     >>> tplot(['erg_att_sprate', 'erg_att_spphase', 'erg_att_izras', 'erg_att_izdec', 'erg_att_gxras', 'erg_att_gxdec', 'erg_att_gzras', 'erg_att_gzdec'])
@@ -120,8 +121,8 @@
         store_data('erg_att_gxdec', data={
             'x': time_float_array, 'y': GX_Delta_float_array})
         store_data('erg_att_gzras', data={
             'x': time_float_array, 'y': GZ_Alpha_float_array})
         store_data('erg_att_gzdec', data={
             'x': time_float_array, 'y': GZ_Delta_float_array})
 
-    return None
+    return ['erg_att_sprate','erg_att_spphase','erg_att_izras','erg_att_gxras','erg_att_gxdec','erg_att_gzras','erg_att_gzdec']
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/cart_trans_matrix_make.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/cart_trans_matrix_make.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/dsi2j2000.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/dsi2j2000.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/erg_cotrans.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/erg_cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/erg_interpolate_att.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/erg_interpolate_att.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/sga2sgi.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/sga2sgi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/sgi2dsi.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/sgi2dsi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/common/cotrans/vector_rotate.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/common/cotrans/vector_rotate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/config.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/hep/hep.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/hep/hep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import cdflib
 import numpy as np
 from pytplot import clip, options, store_data, ylim, zlim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def hep(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = 'omniflux',
@@ -126,32 +126,25 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd, version=version)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
-                
+            gatt = get_gatt_ror(downloadonly, loaded_data)
+
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ",gatt["PI_AFFILIATION"])
             print('')
             print('- The rules of the road (RoR) common to the ERG project:')
             print(
                 '       https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 '- RoR for HEP data: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Hep')
             if level == 'l3':
@@ -443,7 +436,9 @@
             options(tplot_variables, 'ysubtitle', 'PA [deg]')
             # set ztitle
             options(tplot_variables, 'ztitle', '[/keV/cm^{2}/sr/s]')
 
             return tplot_variables
 
     return loaded_data
+
+
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepe/lepe.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepe/lepe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
-import cdflib
 import numpy as np
 from pytplot import clip, get_data, options, store_data, ylim, zlim
 
 from pytplot import time_double
 
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def lepe(
     trange: List[str] = ['2017-04-04', '2017-04-05'],
     datatype: str = 'omniflux',
@@ -140,34 +140,27 @@
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG LEPe')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ",gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             if level == 'l2':
                 print(
                     'RoR of LEPe L2: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Lepe')
             if level == 'l3':
                 print(
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/lepi/lepi.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/lepi/lepi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
-import cdflib
 import numpy as np
 from pytplot import clip, get_data, options, store_data, ylim, zlim
 from pyspedas import tcopy
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def lepi(
     trange: List[str] = ['2017-07-01', '2017-07-02'],
     datatype: str = 'omniflux',
@@ -123,34 +123,27 @@
     loaded_data = load(pathformat=pathformat, trange=trange, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     flag_FPDO = False # In case it doesn't get set later
 
     if (len(loaded_data) > 0) and ror:
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG LEPi')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of LEPi L2: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Lepi')
             print(
                 'RoR of ERG/LEPi: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Lepi#Rules_of_the_Road')
             print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/load.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     tvars = cdf_to_tplot(out_files, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                          varformat=varformat, varnames=varnames, notplot=notplot)
 
     if notplot:
         if len(out_files) > 0:
             cdf_file = cdflib.CDF(out_files[-1])
             cdf_info = cdf_file.cdf_info()
-            all_cdf_variables = cdf_info['rVariables'] + cdf_info['zVariables']
+            all_cdf_variables = cdf_info.rVariables + cdf_info.zVariables
             gatt = cdf_file.globalattsget()
             for var in all_cdf_variables:
                 t_plot_name = prefix + var + suffix
                 if t_plot_name in tvars:
                     vatt = cdf_file.varattsget(var)
                     tvars[t_plot_name]['CDF'] = {'VATT':vatt,
                                                 'GATT':gatt,
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepe/mepe.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepe/mepe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-import cdflib
 from pytplot import options, ylim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def mepe(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = 'omniflux',
@@ -109,32 +109,25 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('- The rules of the road (RoR) common to the ERG project:')
             print(
                 '      https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 '- RoR for MEP-e data:  https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Mepe')
             print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/mepi_nml.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/mepi_nml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import cdflib
 from pytplot import options, ylim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def mepi_nml(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = 'omniflux',
@@ -105,33 +105,26 @@
         '/%Y/%m/erg_mepi_'+level+'_'+datatype+'_%Y%m%d_v??_??.cdf'
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('- The rules of the road (RoR) common to the ERG project:')
             print(
                 '      https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 '- RoR for MEP-i data: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Mepi')
             print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/mepi/mepi_tof.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/mepi/mepi_tof.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
-import cdflib
 from pytplot import options, ylim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def mepi_tof(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = 'flux',
@@ -108,32 +107,25 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ",gatt["PI_AFFILIATION"])
             print('')
             print('- The rules of the road (RoR) common to the ERG project:')
             print(
                 '      https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 '- RoR for MEP-i data: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Mepi')
             print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/mgf/mgf.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/mgf/mgf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import cdflib
 import numpy as np
 from pytplot import clip, get_data, options, ylim
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def mgf(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = '8sec',
@@ -131,33 +131,26 @@
 
     if (loaded_data is None) or (loaded_data == []):
         return loaded_data
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG MGF')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of MGF L2: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Mgf')
             print('Contact: erg_mgf_info at isee.nagoya-u.ac.jp')
             print(
                 '**************************************************************************')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/orb.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/orb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import cdflib
 import numpy as np
 from pytplot import tnames
 from pytplot import clip, get_data, options, ylim
 
 from ..load import load
 from .remove_duplicated_tframe import remove_duplicated_tframe
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def orb(
     trange: List[str] = ['2017-03-27', '2017-03-28'],
     datatype: str = 'def',
@@ -140,22 +140,15 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd, version=version)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/orb/remove_duplicated_tframe.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/orb/remove_duplicated_tframe.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_convert_flux_units.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_convert_flux_units.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_hep_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_hep_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_hep_part_products.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_hep_part_products.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lep_part_products.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lep_part_products.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lepe_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lepe_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_lepi_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_lepi_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mep_part_products.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mep_part_products.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mepe_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mepe_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_mepi_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_mepi_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_clean_data.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_clean_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_do_fac.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_do_fac.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_limit_range.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_limit_range.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_e_spec.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_e_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_fac.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_fac.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_phi_spec.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_phi_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_theta_spec.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_theta_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_make_tplot.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_make_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_moments_tplot.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_moments_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_pgs_progress_update.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_pgs_progress_update.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_units_string.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_units_string.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_xep_get_dist.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_xep_get_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/erg_xep_part_products.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/erg_xep_part_products.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_lepi_flux_angle_in_sga.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_lepi_flux_angle_in_sga.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepe_az_dir_in_sga.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepe_az_dir_in_sga.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepe_flux_angle_in_sga.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepe_flux_angle_in_sga.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/particle/get_mepi_flux_angle_in_sga.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/particle/get_mepi_flux_angle_in_sga.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_efd.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_efd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import cdflib
 import numpy as np
 from pytplot import tnames
 from pytplot import time_float
 from pytplot import get_data, options, store_data, ylim, zlim
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def pwe_efd(
     trange: List[str] = ['2017-04-01', '2017-04-02'],
     datatype: str = 'E_spin',
@@ -137,35 +137,28 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG PWE EFD')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ",gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of PWE/EFD: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Pwe/Efd')
             print('')
             print('Contact: erg_pwe_info at isee.nagoya-u.ac.jp')
             print(
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_hfa.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_hfa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import cdflib
 from pytplot import clip, options, ylim, zlim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def pwe_hfa(
     trange: List[str] = ['2017-04-01', '2017-04-02'],
     datatype: str = 'spec',
@@ -119,35 +119,28 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG PWE HFA')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of PWE/HFA: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Pwe/Hfa')
             print('')
             print('Contact: erg_pwe_info at isee.nagoya-u.ac.jp')
             print(
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_ofa.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_ofa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
-import cdflib
 from pytplot import options, ylim, zlim, get_data
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def pwe_ofa(
     trange: List[str] = ['2017-04-01', '2017-04-02'],
     datatype: str = 'spec',
@@ -108,35 +107,28 @@
 
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
             # --- print PI info and rules of the road
 
             print(' ')
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG PWE OFA')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ", gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of PWE/OFA: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Pwe/Ofa')
             print('')
             print('Contact: erg_pwe_info at isee.nagoya-u.ac.jp')
             print(
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/pwe/pwe_wfc.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/pwe/pwe_wfc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import cdflib
 import numpy as np
 from pytplot import tnames
 from pytplot import time_float
 from pytplot import clip, get_data, options, store_data, ylim, zlim
 
 from ..load import load
+from ..get_gatt_ror import get_gatt_ror
 
 
 from typing import List, Optional
 
 def pwe_wfc(
     trange: List[str] = ['2017-04-01/12:00:00', '2017-04-01/13:00:00'],
     datatype: str = 'waveform',
@@ -129,15 +129,15 @@
                 component_list = ['e', 'b']
             elif (component == 'e') or (component == 'b'):
                 component_list = [component]
             for com in component_list:
                 prefix = 'erg_pwe_wfc_' + level + '_' + com + '_' + mode + '_'
                 pathformat = 'satellite/erg/pwe/wfc/'+level+'/'+datatype+'/%Y/%m/erg_pwe_wfc_' + \
                     level+'_'+com+'_'+datatype+'_'+mode+'_'+coord+'_%Y%m%d%H_v??_??.cdf'
-                loaded_data.append(load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
+                loaded_data.extend(load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                                    varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd))
                 if com == 'e':
                     tplot_name_list += [prefix +
                                         'Ex_waveform', prefix + 'Ey_waveform']
                 elif com == 'b':
                     tplot_name_list += [prefix + 'Bx_waveform',
                                         prefix + 'By_waveform', prefix + 'Bz_waveform']
@@ -148,43 +148,36 @@
                 component_list = ['e', 'b']
             elif (component == 'e') or (component == 'b'):
                 component_list = [component]
             for com in component_list:
                 prefix = 'erg_pwe_wfc_' + level + '_' + com + '_' + mode + '_'
                 pathformat = 'satellite/erg/pwe/wfc/'+level+'/'+datatype+'/%Y/%m/erg_pwe_wfc_' + \
                     level+'_'+com+'_'+datatype+'_'+mode+'_%Y%m%d%H_v??_??.cdf'
-                loaded_data.append(load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
+                loaded_data.extend(load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                                    varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd))
                 prefix_list.append(prefix)
                 component_suffix_list.append(com.upper() + '_spectra')
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1][-1])
-                    gatt = cdf_file.globalattsget()
-                elif notplot:
-                    gatt = loaded_data[-1][list(loaded_data[-1].keys())[-1]]['CDF']['GATT']
-                else:
-                    gatt = get_data(loaded_data[-1][-1], metadata=True)['CDF']['GATT']
+            gatt = get_gatt_ror(downloadonly, loaded_data)
 
 
             # --- print PI info and rules of the road
             print(' ')
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG PWE WFC')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: "+str(gatt["PI_AFFILIATION"]))
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print(
                 'RoR of PWE/WFC: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Pwe/Wfc')
             print('')
             print('Contact: erg_pwe_info at isee.nagoya-u.ac.jp')
             print(
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/satellite/erg/xep/xep.py` & `pyspedas-1.5.7/pyspedas/erg/satellite/erg/xep/xep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import cdflib
 import numpy as np
 from pytplot import clip, options, store_data, ylim, zlim, get_data
 
 from ..load import load
-
+from ..get_gatt_ror import get_gatt_ror
 
 from typing import List, Optional
 
 def xep(
     trange: List[str] = ['2017-06-01', '2017-06-02'],
     datatype: str = 'omniflux',
     level: str = 'l2',
@@ -108,34 +107,26 @@
         '/%Y/%m/erg_xep_'+level+'_'+datatype+'_%Y%m%d_v??_??.cdf'
     loaded_data = load(pathformat=pathformat, trange=trange, level=level, datatype=datatype, file_res=file_res, prefix=prefix, suffix=suffix, get_support_data=get_support_data,
                        varformat=varformat, varnames=varnames, downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, uname=uname, passwd=passwd)
 
     if (len(loaded_data) > 0) and ror:
 
         try:
-            if isinstance(loaded_data, list):
-                if downloadonly:
-                    cdf_file = cdflib.CDF(loaded_data[-1])
-                    gatt = cdf_file.globalattsget()
-                else:
-                    gatt = get_data(loaded_data[-1], metadata=True)['CDF']['GATT']
-            elif isinstance(loaded_data, dict):
-                gatt = loaded_data[list(loaded_data.keys())[-1]]['CDF']['GATT']
-
+            gatt = get_gatt_ror(downloadonly, loaded_data)
             # --- print PI info and rules of the road
 
             print(' ')
             print(
                 '**************************************************************************')
             print(gatt["LOGICAL_SOURCE_DESCRIPTION"])
             print('')
             print('Information about ERG XEP')
             print('')
             print('PI: ', gatt['PI_NAME'])
-            print("Affiliation: "+gatt["PI_AFFILIATION"])
+            print("Affiliation: ",gatt["PI_AFFILIATION"])
             print('')
             print('RoR of ERG project common: https://ergsc.isee.nagoya-u.ac.jp/data_info/rules_of_the_road.shtml.en')
             print('RoR of XEP: https://ergsc.isee.nagoya-u.ac.jp/mw/index.php/ErgSat/Xep')
             print('')
             print('Contact: erg_xep_info at isee.nagoya-u.ac.jp')
             print(
                 '**************************************************************************')
```

### Comparing `pyspedas-1.5.6/pyspedas/erg/tests/tests.py` & `pyspedas-1.5.7/pyspedas/omni/tests/tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-
 import os
 import unittest
-from pytplot import data_exists
-
+from pytplot import data_exists, del_data
 import pyspedas
 
 class LoadTestCases(unittest.TestCase):
-    def test_load_hep_data(self):
-        hep_vars = pyspedas.erg.hep()
-        self.assertTrue(data_exists('erg_hep_l2_FEDO_L'))
-        self.assertTrue(data_exists('erg_hep_l2_FEDO_H'))
-
-    def test_load_xep_data(self):
-        xep_vars = pyspedas.erg.xep()
-        self.assertTrue(data_exists('erg_xep_l2_FEDO_SSD'))
-
-    def test_load_orb_data(self):
-        orb_vars = pyspedas.erg.orb()
-        self.assertTrue(data_exists('erg_orb_l2_pos_gse'))
-        self.assertTrue(data_exists('erg_orb_l2_pos_gsm'))
-        self.assertTrue(data_exists('erg_orb_l2_pos_sm'))
-        self.assertTrue(data_exists('erg_orb_l2_vel_gse'))
-        self.assertTrue(data_exists('erg_orb_l2_vel_gsm'))
-        self.assertTrue(data_exists('erg_orb_l2_vel_sm'))
-
-    def test_load_l3_orb_data(self):
-        orb_vars = pyspedas.erg.orb(level='l3')
-        self.assertTrue(data_exists('erg_orb_l3_pos_eq_op'))
-        self.assertTrue(data_exists('erg_orb_l3_pos_iono_north_op'))
-        self.assertTrue(data_exists('erg_orb_l3_pos_iono_south_op'))
-
-    def test_load_mgf_data(self):
-        mgf_vars = pyspedas.erg.mgf(time_clip=True)
-        self.assertTrue(data_exists('erg_mgf_l2_mag_8sec_sm'))
-
-    def test_load_lepe_data(self):
-        lepe_vars = pyspedas.erg.lepe()
-        self.assertTrue(data_exists('erg_lepe_l2_omniflux_FEDO'))
-
-    def test_load_lepi_data(self):
-        lepi_vars = pyspedas.erg.lepi()
-        self.assertTrue(data_exists('erg_lepi_l2_omniflux_FPDO'))
-        self.assertTrue(data_exists('erg_lepi_l2_omniflux_FHEDO'))
-        self.assertTrue(data_exists('erg_lepi_l2_omniflux_FODO'))
-
-    def test_load_mepe_data(self):
-        mepe_vars = pyspedas.erg.mepe()
-        self.assertTrue(data_exists('erg_mepe_l2_omniflux_FEDO'))
-
-    def test_load_mepi_data(self):
-        mepi_vars = pyspedas.erg.mepi_nml()
-        self.assertTrue(data_exists('erg_mepi_l2_omniflux_epoch_tof'))
-        mepi_vars = pyspedas.erg.mepi_tof()
-        self.assertTrue(data_exists('erg_mepi_l2_tofflux_FPDU'))
-        self.assertTrue(data_exists('erg_mepi_l2_tofflux_FODU'))
-
-    def test_load_pwe_ofa_data(self):
-        pwe_vars = pyspedas.erg.pwe_ofa()
-        self.assertTrue(data_exists('erg_pwe_ofa_l2_spec_E_spectra_132'))
-        self.assertTrue(data_exists('erg_pwe_ofa_l2_spec_B_spectra_132'))
-
-    def test_load_pwe_efd_data(self):
-        pwe_vars = pyspedas.erg.pwe_efd()
-        self.assertTrue(data_exists('erg_pwe_efd_l2_E_spin_Eu_dsi'))
-        self.assertTrue(data_exists('erg_pwe_efd_l2_E_spin_Ev_dsi'))
-        self.assertTrue(data_exists('erg_pwe_efd_l2_E_spin_Ev1_dsi'))
-        self.assertTrue(data_exists('erg_pwe_efd_l2_E_spin_Eu2_dsi'))
-
-    def test_load_pwe_hfa_data(self):
-        pwe_vars = pyspedas.erg.pwe_hfa()
-        self.assertTrue(data_exists('erg_pwe_hfa_l2_low_spectra_eu'))
-        self.assertTrue(data_exists('erg_pwe_hfa_l2_low_spectra_ev'))
-        self.assertTrue(data_exists('erg_pwe_hfa_l2_low_spectra_esum'))
-        self.assertTrue(data_exists('erg_pwe_hfa_l2_low_spectra_er'))
+    def test_utc_timestamp_regression(self):
+        varname = 'BX_GSE'
+        del_data('*')
+        data_omni = pyspedas.omni.data(trange=['2010-01-01/00:00:00', '2010-01-02/00:00:00'],notplot=True,varformat=varname,time_clip=True)
+        ts=data_omni[varname]['x'][0]
+        # Depending on the version of cdflib in use, ts might be a datetime.datetime, or np.datetime64.  The string representations
+        # are slightly different: "2010-01-01 00:00:00" vs "2010-01-01T00:00:00.000000".  So we replace "T" with " " and
+        # discard any fractional part before comparing.
+        ds=str(ts)
+        ds2=ds.replace("T"," ")
+        nofrac,frac=ds2.split(".")
+        self.assertTrue(nofrac == '2010-01-01 00:00:00')
+
+    def test_load_hro2_data(self):
+        del_data('*')
+        omni_vars = pyspedas.omni.data()
+        self.assertTrue(data_exists('BX_GSE'))
+        self.assertTrue(data_exists('BY_GSE'))
+        self.assertTrue(data_exists('BZ_GSE'))
+        self.assertTrue(data_exists('BY_GSM'))
+        self.assertTrue(data_exists('BZ_GSM'))
+        self.assertTrue(data_exists('proton_density'))
+
+    def test_load_hro_data(self):
+        del_data('*')
+        omni_vars = pyspedas.omni.data(level='hro')
+        self.assertTrue(data_exists('BX_GSE'))
+        self.assertTrue(data_exists('BY_GSE'))
+        self.assertTrue(data_exists('BZ_GSE'))
+        self.assertTrue(data_exists('BY_GSM'))
+        self.assertTrue(data_exists('BZ_GSM'))
+        self.assertTrue(data_exists('proton_density'))
+
+    def test_load_hro_5min_data(self):
+        del_data('*')
+        omni_vars = pyspedas.omni.data(level='hro', datatype='5min')
+        self.assertTrue(data_exists('BX_GSE'))
+        self.assertTrue(data_exists('BY_GSE'))
+        self.assertTrue(data_exists('BZ_GSE'))
+        self.assertTrue(data_exists('BY_GSM'))
+        self.assertTrue(data_exists('BZ_GSM'))
+        self.assertTrue(data_exists('proton_density'))
+
+    def test_load_hro_hour_data(self):
+        del_data('*')
+        omni_vars = pyspedas.omni.data(level='hro2', datatype='hour', trange=['2013-03-01', '2013-03-02'])
+        self.assertTrue(data_exists('BX_GSE'))
+        self.assertTrue(data_exists('BY_GSE'))
+        self.assertTrue(data_exists('BZ_GSE'))
+        self.assertTrue(data_exists('BY_GSM'))
+        self.assertTrue(data_exists('BZ_GSM'))
+
+    def test_load_hro_hour_data_long_interval(self):
+        from pyspedas.utilities.dailynames import dailynames
+        del_data('*')
+        trange=['2013-01-05','2013-11-06']
+        pathformat = 'hourly/%Y/omni2_h0_mrg1hr_%Y%m01_v??.cdf'
+        file_res=24*3600*183 # 1 file every 6 months
+        remote_names=dailynames(file_format=pathformat,trange=trange,res=file_res)
+        print(remote_names)
+        omni_vars = pyspedas.omni.data(datatype='hour', trange=trange)
+        self.assertTrue(data_exists('BX_GSE'))
+        self.assertTrue(data_exists('BY_GSE'))
+        self.assertTrue(data_exists('BZ_GSE'))
+        self.assertTrue(data_exists('BY_GSM'))
+        self.assertTrue(data_exists('BZ_GSM'))
+
+    def test_load_invalid_datatype(self):
+        omni_vars = pyspedas.omni.data(datatype='1')
 
     def test_downloadonly(self):
-        files = pyspedas.erg.mgf(downloadonly=True, trange=['2017-03-27', '2017-03-28'])
+        files = pyspedas.omni.data(downloadonly=True, trange=['2014-2-15', '2014-2-16'])
         self.assertTrue(os.path.exists(files[0]))
 
+
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/fast/__init__.py` & `pyspedas-1.5.7/pyspedas/fast/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/fast/load.py` & `pyspedas-1.5.7/pyspedas/fast/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/fast/tests/tests.py` & `pyspedas-1.5.7/pyspedas/fast/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/get_tsy_params.py` & `pyspedas-1.5.7/pyspedas/geopack/get_tsy_params.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/get_w_params.py` & `pyspedas-1.5.7/pyspedas/geopack/get_w_params.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/kp2iopt.py` & `pyspedas-1.5.7/pyspedas/geopack/kp2iopt.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/t01.py` & `pyspedas-1.5.7/pyspedas/geopack/t01.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/t89.py` & `pyspedas-1.5.7/pyspedas/geopack/t89.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/t89_trace_equator.py` & `pyspedas-1.5.7/pyspedas/geopack/t89_trace_equator.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/t89_trace_iono.py` & `pyspedas-1.5.7/pyspedas/geopack/t89_trace_iono.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/t96.py` & `pyspedas-1.5.7/pyspedas/geopack/t96.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/tests/geopack_idl_validation_tests.py` & `pyspedas-1.5.7/pyspedas/geopack/tests/geopack_idl_validation_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/tests/tests.py` & `pyspedas-1.5.7/pyspedas/geopack/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geopack/ts04.py` & `pyspedas-1.5.7/pyspedas/geopack/ts04.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geotail/__init__.py` & `pyspedas-1.5.7/pyspedas/geotail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geotail/load.py` & `pyspedas-1.5.7/pyspedas/geotail/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/geotail/tests/tests.py` & `pyspedas-1.5.7/pyspedas/geotail/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/goes/__init__.py` & `pyspedas-1.5.7/pyspedas/goes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/goes/load.py` & `pyspedas-1.5.7/pyspedas/goes/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/goes/load_orbit.py` & `pyspedas-1.5.7/pyspedas/goes/load_orbit.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/goes/tests/tests.py` & `pyspedas-1.5.7/pyspedas/goes/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/hapi/hapi.py` & `pyspedas-1.5.7/pyspedas/hapi/hapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import logging
 import warnings
 from pytplot import get_data, store_data, options, time_double
 import numpy as np
-
-try:
-    from hapiclient import hapi as load_hapi
-except ImportError:
-    logging.error('hapiclient not found; install with: "pip install hapiclient"')
+from hapiclient import hapi as load_hapi
 
 
 def hapi(trange=None, server=None, dataset=None, parameters='', suffix='',
-         prefix='', catalog=False):
+         prefix='', catalog=False, quiet=False):
     """
     Loads data from a HAPI server into pytplot variables
 
     Parameters
     -----------
         trange: list of str or list of float
             Time range to load the data for
@@ -24,50 +20,76 @@
 
         dataset: str
             HAPI dataset to load
 
         parameters: str or list of str
             Parameters in the dataset to load; default
             is to load them all
+            Default: '' (load all parameters)
 
         prefix: str
             Prefix to append to the tplot variables
+            Default: ''
 
         suffix: str
             Suffix to append to the tplot variables
+            Default: ''
 
         catalog: bool
             If True, returns the server's catalog of datasets
+            Default: False
+
+        quiet: bool
+            If True, suppress printing the catalog ids retrieved
+            Default: False
 
     Returns
     -------
-        List of tplot variables created.
+        list of str
+            List of catalog ids retrieved or tplot variables created.
+
+    Examples
+    --------
+    Print catalog from CDAWeb HAPI server
+    >>> import pyspedas
+    >>> cat_entries = pyspedas.hapi(server='https://cdaweb.gsfc.nasa.gov/hapi', catalog=True)
+
+    Load OMNI data from CDAWeg HAPI server
+    >>> import pyspedas
+    >>> from pytplot import tplot
+    >>> h_vars = pyspedas.hapi(trange=['2003-10-20', '2003-11-30'],server='https://cdaweb.gsfc.nasa.gov/hapi',dataset='OMNI_HRO2_1MIN')
+    >>> tplot(['BX_GSE','BY_GSE','BZ_GSE'])
     """
 
     if server is None:
         logging.error('No server specified; example servers include:')
         logging.error('- https://cdaweb.gsfc.nasa.gov/hapi')
         logging.error('- https://pds-ppi.igpp.ucla.edu/hapi')
         logging.error('- http://planet.physics.uiowa.edu/das/das2Server/hapi')
         logging.error('- https://iswa.gsfc.nasa.gov/IswaSystemWebApp/hapi')
         logging.error('- http://lasp.colorado.edu/lisird/hapi')
         return
 
     if catalog:
         catalog = load_hapi(server)
         items = []
+        id_list = []
         if 'catalog' in catalog.keys():
             items = catalog['catalog']
-        logging.info('Available datasets: ')
+        if not quiet:
+            print('Available datasets: ')
         for item in items:
             if 'title' in item.keys():
-                logging.info(item['id'] + ': ' + item['title'])
+                if not quiet:
+                    print(item['id'] + ': ' + item['title'])
             else:
-                logging.info(item['id'])
-        return
+                if not quiet:
+                    print(item['id'])
+            id_list.append(item['id'])
+        return id_list
 
     if dataset is None:
         logging.error('Error, no dataset specified; please see the catalog for a list of available data sets.')
         return
 
     if trange is None:
         logging.error('Error, no trange specified')
```

### Comparing `pyspedas-1.5.6/pyspedas/hapi/tests/tests.py` & `pyspedas-1.5.7/pyspedas/hapi/tests/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import unittest
-from pyspedas.hapi.hapi import hapi
-from pytplot import data_exists
+from pyspedas import hapi
+from pytplot import data_exists, del_data
 
 
 class HAPITests(unittest.TestCase):
     def test_print_servers(self):
         hapi(trange=['2003-10-20', '2003-11-30'])
 
-    def test_print_catalog(self):
-        hapi(server='https://cdaweb.gsfc.nasa.gov/hapi', catalog=True)
+    def test_return_catalog(self):
+        id_list = hapi(server='https://cdaweb.gsfc.nasa.gov/hapi', catalog=True, quiet=True)
+        self.assertTrue('MMS1_EDI_BRST_L2_EFIELD' in id_list)
 
     def test_dataset_not_specified(self):
         # dataset not specified
         h_vars = hapi(trange=['2003-10-20', '2003-11-30'],
                       server='https://cdaweb.gsfc.nasa.gov/hapi')
 
     def test_trange_not_specified(self):
@@ -22,14 +23,15 @@
 
     def test_cdaweb_mms_spec(self):
         h_vars = hapi(trange=['2019-10-16', '2019-10-17'],
                       server='https://cdaweb.gsfc.nasa.gov/hapi',
                       dataset='MMS4_EDP_SRVY_L2_HFESP')
 
     def test_cdaweb_omni(self):
+        del_data()
         h_vars = hapi(trange=['2003-10-20', '2003-11-30'],
                       server='https://cdaweb.gsfc.nasa.gov/hapi',
                       dataset='OMNI_HRO2_1MIN')
         self.assertTrue(data_exists('BX_GSE'))
         self.assertTrue(data_exists('BY_GSE'))
         self.assertTrue(data_exists('BZ_GSE'))
```

### Comparing `pyspedas-1.5.6/pyspedas/image/__init__.py` & `pyspedas-1.5.7/pyspedas/image/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/image/load.py` & `pyspedas-1.5.7/pyspedas/image/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/image/tests/tests.py` & `pyspedas-1.5.7/pyspedas/image/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/kyoto/load_dst.py` & `pyspedas-1.5.7/pyspedas/kyoto/load_dst.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/kyoto/tests/tests.py` & `pyspedas-1.5.7/pyspedas/kyoto/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/lanl/__init__.py` & `pyspedas-1.5.7/pyspedas/lanl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/lanl/load.py` & `pyspedas-1.5.7/pyspedas/lanl/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/lanl/tests/tests.py` & `pyspedas-1.5.7/pyspedas/lanl/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/maven/maven_kp_to_tplot.py` & `pyspedas-1.5.7/pyspedas/maven/maven_kp_to_tplot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,142 @@
-# Copyright 2017 Regents of the University of Colorado. All Rights Reserved.
-# Released under the MIT license.
-# This software was developed at the University of Colorado's Laboratory for Atmospheric and Space Physics.
-# Verify current version before use at: https://github.com/MAVENSDC/Pydivide
-
+import logging
 import calendar
 import numpy as np
-from .utilities import kp_regex
-from .utilities import param_dict
+from .utilities import maven_kp_l2_regex
+from .utilities import maven_param_list
 from .utilities import remove_inst_tag
-from .utilities import get_latest_files_from_date_range, read_iuvs_file, get_latest_iuvs_files_from_date_range
+from .utilities import (
+    get_latest_files_from_date_range,
+    read_iuvs_file,
+    get_latest_iuvs_files_from_date_range,
+)
 from .utilities import get_header_info
 from .utilities import orbit_time
 import pytplot
 from _collections import OrderedDict
 import builtins
 import os
 
 
-def maven_kp_to_tplot(filename=None, input_time=None, instruments=None, insitu_only=False, specified_files_only=False, ancillary_only=False):
-    '''
-    Read in a given filename in situ file into a dictionary object
-    Optional keywords maybe used to downselect instruments returned
-     and the time windows.
-
-    Input:
-        filename:
-            Name of the in situ KP file(s) to read in.
-        input_time:
-            Set a time bounds/filter on the data
-            (this will be necessary when this is called by a wrapper that
-             seeks to ingest all data within a range of dates that may
-             be allowed to span multiple days (files) ).
-        instruments:
-            Optional keyword listing the instruments to include
-            in the returned dictionary/structure.
-        insitu_only:
-            Optional keyword that allows you to specify that you only want
-            to download insitu files.
-        specified_files_only:
-            Optional keyword that allows you to specify you only want filenames
-            given in 'filename' to be read in, not other files close in date/time
-            as well.
-        ancillary_only:
-            Will only load in the spacecraft and APP info
-    Output:
-        A dictionary (data structure) containing up to all of the columns
-            included in a MAVEN in-situ Key parameter data file.
-    '''
+def maven_kp_to_tplot(
+    filename=None,
+    input_time=None,
+    instruments=None,
+    insitu_only=False,
+    specified_files_only=False,
+    ancillary_only=False,
+):
+    """
+    Convert MAVEN insitu (KP) data files to tplot variables.
+
+    Parameters
+    ----------
+    filename : str or list, optional
+        Name of the file(s) to read in. Defaults to None.
+    input_time : str or list or int, optional
+        Time frame in which to search for downloaded files.
+        Can be a single date string, a list of two date strings representing a time range, or an orbit number.
+        Defaults to None.
+    instruments : str or list, optional
+        List of instruments to include. Defaults to None.
+    insitu_only : bool, optional
+        Flag to include only insitu data files. Defaults to False.
+    specified_files_only : bool, optional
+        If True, specifies that only filenames given in 'filename' should be read in. Defaults to False.
+    ancillary_only : bool, optional
+        If True, only the spacecraft and APP info will be loaded. Defaults to False.
+
+    Returns
+    -------
+    dict
+        A dictionary containing up to all of the columns included in a MAVEN in-situ Key parameter data file.
+    """
+
     import pandas as pd
     import re
     from datetime import datetime, timedelta
     from dateutil.parser import parse
 
     filenames = []
     iuvs_filenames = []
+    param_dict = maven_param_list()
 
     if instruments is not None:
         if not isinstance(instruments, builtins.list):
             instruments = [instruments]
 
     if filename is None and input_time is None:
-        print('You must specify either a set of filenames to read in, or a time frame in which '
-              'you want to search for downloaded files.')
+        logging.warning(
+            "You must specify either a set of filenames to read in, or a time frame in which "
+            "you want to search for downloaded files."
+        )
 
     if ancillary_only:
-        instruments=['SPACECRAFT']
+        instruments = ["SPACECRAFT"]
 
     if filename is not None:
         if not isinstance(filename, builtins.list):
             filename = [filename]
 
         dates = []
         for file in filename:
-            date = re.findall(r'_(\d{8})', file)[0]
+            date = re.findall(r"_(\d{8})", file)[0]
             dates.append(date)
-            if 'iuvs' in file:
+            if "iuvs" in file:
                 iuvs_filenames.append(file)
             else:
                 filenames.append(file)
         dates.sort()
 
         # To keep the rest of the code consistent, if someone gave a files, or files, to load, but no input_time,
         # go ahead and create an 'input_time'
         if input_time is None:
             if len(dates) == 1:
-                input_time = str(dates[0][:4]) + '-' + str(dates[0][4:6]) + '-' + str(dates[0][6:])
+                input_time = (
+                    str(dates[0][:4])
+                    + "-"
+                    + str(dates[0][4:6])
+                    + "-"
+                    + str(dates[0][6:])
+                )
 
             else:
                 beg_date = min(dates)
                 end_date = max(dates)
-                input_time = [str(beg_date[:4]) + '-' + str(beg_date[4:6]) + '-' + str(beg_date[6:]),
-                              str(end_date[:4]) + '-' + str(end_date[4:6]) + '-' + str(end_date[6:])]
+                input_time = [
+                    str(beg_date[:4])
+                    + "-"
+                    + str(beg_date[4:6])
+                    + "-"
+                    + str(beg_date[6:]),
+                    str(end_date[:4])
+                    + "-"
+                    + str(end_date[4:6])
+                    + "-"
+                    + str(end_date[6:]),
+                ]
 
     # Check for orbit num rather than time string
     if isinstance(input_time, builtins.list):
         if isinstance(input_time[0], int):
             input_time = orbit_time(input_time[0], input_time[1])
     elif isinstance(input_time, int):
         input_time = orbit_time(input_time)
 
     # Turn string input into datetime objects
     if isinstance(input_time, list):
         if len(input_time[0]) <= 10:
-            input_time[0] = input_time[0] + ' 00:00:00'
+            input_time[0] = input_time[0] + " 00:00:00"
         if len(input_time[1]) <= 10:
-            input_time[1] = input_time[1] + ' 23:59:59'
+            input_time[1] = input_time[1] + " 23:59:59"
         date1 = parse(input_time[0])
         date2 = parse(input_time[1])
     else:
         if len(input_time) <= 10:
-            input_time += ' 00:00:00'
+            input_time += " 00:00:00"
         date1 = parse(input_time)
         date2 = date1 + timedelta(days=1)
 
     date1_unix = calendar.timegm(date1.timetuple())
     date2_unix = calendar.timegm(date2.timetuple())
 
     # Grab insitu and iuvs files for the specified/created date ranges
@@ -123,139 +146,194 @@
     # Add date range files to respective file lists if desired
     if not specified_files_only:
         filenames.extend(date_range_filenames)
         iuvs_filenames.extend(date_range_iuvs_filenames)
 
     if not date_range_filenames and not date_range_iuvs_filenames:
         if not filenames and not iuvs_filenames:
-            print("No files found for the input date range, and no specific filenames were given. Exiting.")
+            logging.warning(
+                "No files found for the input date range, and no specific filenames were given. Exiting."
+            )
             return
 
     # Going to look for files between time frames, but as we might have already specified
     # certain files to load in, we don't want to load them in 2x... so doing a check for that here
     filenames = list(set(filenames))
     iuvs_filenames = list(set(iuvs_filenames))
 
+    kp_regex, l2_regex = maven_kp_l2_regex()
     kp_insitu = []
     if filenames:
         # Get column names
         names, inst = [], []
         crus_name, crus_inst = [], []
         c_found = False
         r_found = False
         for f in filenames:
-            if kp_regex.match(os.path.basename(f)).group('description') == '_crustal' and not c_found:
+            if (
+                kp_regex.match(os.path.basename(f)).group("description") == "_crustal"
+                and not c_found
+            ):
                 name, inss = get_header_info(f)
                 # Strip off the first name for now (Time), and use that as the dataframe index.
                 # Seems to make sense for now, but will it always?
                 crus_name.extend(name[1:])
                 crus_inst.extend(inss[1:])
                 c_found = True
-            elif kp_regex.match(os.path.basename(f)).group('description') == '' and not r_found:
+            elif (
+                kp_regex.match(os.path.basename(f)).group("description") == ""
+                and not r_found
+            ):
                 name, ins = get_header_info(f)
                 # Strip off the first name for now (Time), and use that as the dataframe index.
                 # Seems to make sense for now, but will it always?
                 names.extend(name[1:])
                 inst.extend(ins[1:])
                 r_found = True
         all_names = names + crus_name
         all_inst = inst + crus_inst
 
         # Break up dictionary into instrument groups
-        lpw_group, euv_group, swe_group, swi_group, sta_group, sep_group, mag_group, ngi_group, app_group, sc_group, \
-        crus_group = [], [], [], [], [], [], [], [], [], [], []
+        (
+            lpw_group,
+            euv_group,
+            swe_group,
+            swi_group,
+            sta_group,
+            sep_group,
+            mag_group,
+            ngi_group,
+            app_group,
+            sc_group,
+            crus_group,
+        ) = ([], [], [], [], [], [], [], [], [], [], [])
 
         for i, j in zip(all_inst, all_names):
-            if re.match('^LPW$', i.strip()):
+            if re.match("^LPW$", i.strip()):
                 lpw_group.append(j)
-            elif re.match('^LPW-EUV$', i.strip()):
+            elif re.match("^LPW-EUV$", i.strip()):
                 euv_group.append(j)
-            elif re.match('^SWEA$', i.strip()):
+            elif re.match("^SWEA$", i.strip()):
                 swe_group.append(j)
-            elif re.match('^SWIA$', i.strip()):
+            elif re.match("^SWIA$", i.strip()):
                 swi_group.append(j)
-            elif re.match('^STATIC$', i.strip()):
+            elif re.match("^STATIC$", i.strip()):
                 sta_group.append(j)
-            elif re.match('^SEP$', i.strip()):
+            elif re.match("^SEP$", i.strip()):
                 sep_group.append(j)
-            elif re.match('^MAG$', i.strip()):
+            elif re.match("^MAG$", i.strip()):
                 mag_group.append(j)
-            elif re.match('^NGIMS$', i.strip()):
+            elif re.match("^NGIMS$", i.strip()):
                 ngi_group.append(j)
-            elif re.match('^MODELED_MAG$', i.strip()):
+            elif re.match("^MODELED_MAG$", i.strip()):
                 crus_group.append(j)
-            elif re.match('^SPICE$', i.strip()):
+            elif re.match("^SPICE$", i.strip()):
                 # NB Need to split into APP and SPACECRAFT
-                if re.match('(.+)APP(.+)', j):
+                if re.match("(.+)APP(.+)", j):
                     app_group.append(j)
                 else:  # Everything not APP is SC in SPICE
                     # But do not include Orbit Num, or IO Flag
                     # Could probably stand to clean this line up a bit
-                    if not re.match('(.+)(Orbit Number|Inbound Outbound Flag)', j):
+                    if not re.match("(.+)(Orbit Number|Inbound Outbound Flag)", j):
                         sc_group.append(j)
             else:
                 pass
 
         delete_groups = []
         if instruments is not None:
-            if 'LPW' not in instruments and 'lpw' not in instruments:
+            if "LPW" not in instruments and "lpw" not in instruments:
                 delete_groups += lpw_group
-            if 'MAG' not in instruments and 'mag' not in instruments:
+            if "MAG" not in instruments and "mag" not in instruments:
                 delete_groups += mag_group
-            if 'EUV' not in instruments and 'euv' not in instruments:
+            if "EUV" not in instruments and "euv" not in instruments:
                 delete_groups += euv_group
-            if 'SWI' not in instruments and 'swi' not in instruments:
+            if "SWI" not in instruments and "swi" not in instruments:
                 delete_groups += swi_group
-            if 'SWE' not in instruments and 'swe' not in instruments:
+            if "SWE" not in instruments and "swe" not in instruments:
                 delete_groups += swe_group
-            if 'NGI' not in instruments and 'ngi' not in instruments:
+            if "NGI" not in instruments and "ngi" not in instruments:
                 delete_groups += ngi_group
-            if 'SEP' not in instruments and 'sep' not in instruments:
+            if "SEP" not in instruments and "sep" not in instruments:
                 delete_groups += sep_group
-            if 'STA' not in instruments and 'sta' not in instruments:
+            if "STA" not in instruments and "sta" not in instruments:
                 delete_groups += sta_group
-            if 'MODELED_MAG' not in instruments and 'modeled_mag' not in instruments:
+            if "MODELED_MAG" not in instruments and "modeled_mag" not in instruments:
                 delete_groups += crus_group
 
         # Read in all relavent data into a pandas dataframe called "temp"
         temp_data = []
         filenames.sort()
         for filename in filenames:
             # Determine number of header lines
             nheader = 0
             with open(filename) as f:
                 for line in f:
-                    if line.startswith('#'):
+                    if line.startswith("#"):
                         nheader += 1
-                if kp_regex.match(os.path.basename(filename)).group('description') == '_crustal':
-                    temp_data.append(pd.read_fwf(filename, skiprows=nheader, index_col=0,
-                                                 widths=[19] + len(crus_name) * [16], names=crus_name))
+                if (
+                    kp_regex.match(os.path.basename(filename)).group("description")
+                    == "_crustal"
+                ):
+                    temp_data.append(
+                        pd.read_fwf(
+                            filename,
+                            skiprows=nheader,
+                            index_col=0,
+                            widths=[19] + len(crus_name) * [16],
+                            names=crus_name,
+                        )
+                    )
                 else:
-                    temp_data.append(pd.read_fwf(filename, skiprows=nheader, index_col=0,
-                                                 widths=[19] + len(names) * [16], names=names))
+                    temp_data.append(
+                        pd.read_fwf(
+                            filename,
+                            skiprows=nheader,
+                            index_col=0,
+                            widths=[19] + len(names) * [16],
+                            names=names,
+                        )
+                    )
                 for i in delete_groups:
                     del temp_data[-1][i]
 
         temp_unconverted = pd.concat(temp_data, axis=0, sort=True)
 
         # Need to convert columns
         # This is kind of a hack, but I can't figure out a better way for now
 
-        if 'SWEA.Electron Spectrum Shape' in temp_unconverted and 'NGIMS.Density NO' in temp_unconverted:
-            temp = temp_unconverted.astype(dtype={'SWEA.Electron Spectrum Shape': np.float64,
-                                                  'NGIMS.Density NO': np.float64})
-        elif 'SWEA.Electron Spectrum Shape' in temp_unconverted and 'NGIMS.Density NO' not in temp_unconverted:
-            temp = temp_unconverted.astype(dtype={'SWEA.Electron Spectrum Shape': np.float64})
-        elif 'SWEA.Electron Spectrum Shape' not in temp_unconverted and 'NGIMS.Density NO' in temp_unconverted:
-            temp = temp_unconverted.astype(dtype={'NGIMS.Density NO': np.float64})
+        if (
+            "SWEA.Electron Spectrum Shape" in temp_unconverted
+            and "NGIMS.Density NO" in temp_unconverted
+        ):
+            temp = temp_unconverted.astype(
+                dtype={
+                    "SWEA.Electron Spectrum Shape": np.float64,
+                    "NGIMS.Density NO": np.float64,
+                }
+            )
+        elif (
+            "SWEA.Electron Spectrum Shape" in temp_unconverted
+            and "NGIMS.Density NO" not in temp_unconverted
+        ):
+            temp = temp_unconverted.astype(
+                dtype={"SWEA.Electron Spectrum Shape": np.float64}
+            )
+        elif (
+            "SWEA.Electron Spectrum Shape" not in temp_unconverted
+            and "NGIMS.Density NO" in temp_unconverted
+        ):
+            temp = temp_unconverted.astype(dtype={"NGIMS.Density NO": np.float64})
         else:
             temp = temp_unconverted
 
         # Cut out the times not included in the date range
-        time_unix = [calendar.timegm(datetime.strptime(i, '%Y-%m-%dT%H:%M:%S').timetuple()) for i in temp.index]
+        time_unix = [
+            calendar.timegm(datetime.strptime(i, "%Y-%m-%dT%H:%M:%S").timetuple())
+            for i in temp.index
+        ]
         start_index = 0
         for t in time_unix:
             if t >= date1_unix:
                 break
             start_index += 1
         end_index = 0
         for t in time_unix:
@@ -266,60 +344,60 @@
         # Assign the first-level only tags
         time_unix = time_unix[start_index:end_index]
         temp = temp[start_index:end_index]
         time = temp.index
         time_unix = pd.Series(time_unix)  # convert into Series for consistency
         time_unix.index = temp.index
 
-        if 'SPICE.Orbit Number' in list(temp):
-            orbit = temp['SPICE.Orbit Number']
+        if "SPICE.Orbit Number" in list(temp):
+            orbit = temp["SPICE.Orbit Number"]
         else:
             orbit = None
-        if 'SPICE.Inbound Outbound Flag' in list(temp):
-            io_flag = temp['SPICE.Inbound Outbound Flag']
+        if "SPICE.Inbound Outbound Flag" in list(temp):
+            io_flag = temp["SPICE.Inbound Outbound Flag"]
         else:
             io_flag = None
 
         # Build the sub-level DataFrames for the larger dictionary/structure
         app = temp[app_group]
         spacecraft = temp[sc_group]
         if instruments is not None:
-            if 'LPW' in instruments or 'lpw' in instruments:
+            if "LPW" in instruments or "lpw" in instruments:
                 lpw = temp[lpw_group]
             else:
                 lpw = None
-            if 'MAG' in instruments or 'mag' in instruments:
+            if "MAG" in instruments or "mag" in instruments:
                 mag = temp[mag_group]
             else:
                 mag = None
-            if 'EUV' in instruments or 'euv' in instruments:
+            if "EUV" in instruments or "euv" in instruments:
                 euv = temp[euv_group]
             else:
                 euv = None
-            if 'SWE' in instruments or 'swe' in instruments:
+            if "SWE" in instruments or "swe" in instruments:
                 swea = temp[swe_group]
             else:
                 swea = None
-            if 'SWI' in instruments or 'swi' in instruments:
+            if "SWI" in instruments or "swi" in instruments:
                 swia = temp[swi_group]
             else:
                 swia = None
-            if 'NGI' in instruments or 'ngi' in instruments:
+            if "NGI" in instruments or "ngi" in instruments:
                 ngims = temp[ngi_group]
             else:
                 ngims = None
-            if 'SEP' in instruments or 'sep' in instruments:
+            if "SEP" in instruments or "sep" in instruments:
                 sep = temp[sep_group]
             else:
                 sep = None
-            if 'STA' in instruments or 'sta' in instruments:
+            if "STA" in instruments or "sta" in instruments:
                 static = temp[sta_group]
             else:
                 static = None
-            if 'MODELED_MAG' in instruments or 'modeled_mag' in instruments:
+            if "MODELED_MAG" in instruments or "modeled_mag" in instruments:
                 crus = temp[crus_group]
             else:
                 crus = None
         else:
             lpw = temp[lpw_group]
             euv = temp[euv_group]
             swea = temp[swe_group]
@@ -358,36 +436,85 @@
             app = app.rename(index=str, columns=param_dict)
         if spacecraft is not None:
             spacecraft = spacecraft.rename(index=str, columns=param_dict)
 
         if orbit is not None and io_flag is not None:
             # Do not forget to save units
             # Define the list of first level tag names
-            tag_names = ['TimeString', 'Time', 'Orbit', 'IOflag',
-                         'LPW', 'EUV', 'SWEA', 'SWIA', 'STATIC',
-                         'SEP', 'MAG', 'NGIMS', 'MODELED_MAG',
-                         'APP', 'SPACECRAFT']
+            tag_names = [
+                "TimeString",
+                "Time",
+                "Orbit",
+                "IOflag",
+                "LPW",
+                "EUV",
+                "SWEA",
+                "SWIA",
+                "STATIC",
+                "SEP",
+                "MAG",
+                "NGIMS",
+                "MODELED_MAG",
+                "APP",
+                "SPACECRAFT",
+            ]
 
             # Define list of first level data structures
-            data_tags = [time, time_unix, orbit, io_flag,
-                         lpw, euv, swea, swia, static,
-                         sep, mag, ngims, crus, app, spacecraft]
+            data_tags = [
+                time,
+                time_unix,
+                orbit,
+                io_flag,
+                lpw,
+                euv,
+                swea,
+                swia,
+                static,
+                sep,
+                mag,
+                ngims,
+                crus,
+                app,
+                spacecraft,
+            ]
         else:
             # Do not forget to save units
             # Define the list of first level tag names
-            tag_names = ['TimeString', 'Time', 'LPW', 'EUV',
-                         'SWEA', 'SWIA', 'STATIC', 'SEP',
-                         'MAG', 'NGIMS', 'MODELED_MAG',
-                         'APP', 'SPACECRAFT']
+            tag_names = [
+                "TimeString",
+                "Time",
+                "LPW",
+                "EUV",
+                "SWEA",
+                "SWIA",
+                "STATIC",
+                "SEP",
+                "MAG",
+                "NGIMS",
+                "MODELED_MAG",
+                "APP",
+                "SPACECRAFT",
+            ]
 
             # Define list of first level data structures
-            data_tags = [time, time_unix, lpw, euv,
-                         swea, swia, static, sep,
-                         mag, ngims, crus, app,
-                         spacecraft]
+            data_tags = [
+                time,
+                time_unix,
+                lpw,
+                euv,
+                swea,
+                swia,
+                static,
+                sep,
+                mag,
+                ngims,
+                crus,
+                app,
+                spacecraft,
+            ]
 
         kp_insitu = OrderedDict(zip(tag_names, data_tags))
 
     # Now for IUVS
     kp_iuvs = []
     if not insitu_only and iuvs_filenames:
         for file in iuvs_filenames:
@@ -395,87 +522,149 @@
     if not kp_iuvs:
         return tplot_varcreate(kp_insitu)
     else:
         return kp_insitu, kp_iuvs
 
 
 def tplot_varcreate(insitu):
-    """Creates tplot variables from the insitu variable
-    """
+    """Creates tplot variables from the insitu variable"""
     # initialize each instrument
     created_vars = []
     for obs in insitu["SPACECRAFT"]:
         obs_specific = "mvn_kp::spacecraft::" + obs.lower()
         try:
-            pytplot.store_data(obs_specific, data={'x': insitu['Time'], 'y': insitu["SPACECRAFT"][obs]})
+            pytplot.store_data(
+                obs_specific, data={"x": insitu["Time"], "y": insitu["SPACECRAFT"][obs]}
+            )
             created_vars.append(obs_specific)
         except:
             pass
 
     # Join together the matricies and remove the individual points
-    pytplot.join_vec(['mvn_kp::spacecraft::t11','mvn_kp::spacecraft::t12','mvn_kp::spacecraft::t13',
-                      'mvn_kp::spacecraft::t21','mvn_kp::spacecraft::t22','mvn_kp::spacecraft::t23',
-                      'mvn_kp::spacecraft::t31','mvn_kp::spacecraft::t32','mvn_kp::spacecraft::t33'],
-                     'mvn_kp::geo_to_mso_matrix')
-
-    pytplot.del_data(['mvn_kp::spacecraft::t11','mvn_kp::spacecraft::t12','mvn_kp::spacecraft::t13',
-                      'mvn_kp::spacecraft::t21','mvn_kp::spacecraft::t22','mvn_kp::spacecraft::t23',
-                      'mvn_kp::spacecraft::t31','mvn_kp::spacecraft::t32','mvn_kp::spacecraft::t33'])
-
-    pytplot.join_vec(['mvn_kp::spacecraft::spacecraft_t11', 'mvn_kp::spacecraft::spacecraft_t12',
-                      'mvn_kp::spacecraft::spacecraft_t13',
-                      'mvn_kp::spacecraft::spacecraft_t21', 'mvn_kp::spacecraft::spacecraft_t22',
-                      'mvn_kp::spacecraft::spacecraft_t23',
-                      'mvn_kp::spacecraft::spacecraft_t31', 'mvn_kp::spacecraft::spacecraft_t32',
-                      'mvn_kp::spacecraft::spacecraft_t33'],
-                     'mvn_kp::spacecraft_to_mso_matrix')
-
-    pytplot.del_data(['mvn_kp::spacecraft::spacecraft_t11', 'mvn_kp::spacecraft::spacecraft_t12',
-                      'mvn_kp::spacecraft::spacecraft_t13',
-                      'mvn_kp::spacecraft::spacecraft_t21', 'mvn_kp::spacecraft::spacecraft_t22',
-                      'mvn_kp::spacecraft::spacecraft_t23',
-                      'mvn_kp::spacecraft::spacecraft_t31', 'mvn_kp::spacecraft::spacecraft_t32',
-                      'mvn_kp::spacecraft::spacecraft_t33'])
-
-    created_vars.remove('mvn_kp::spacecraft::t11')
-    created_vars.remove('mvn_kp::spacecraft::t12')
-    created_vars.remove('mvn_kp::spacecraft::t13')
-    created_vars.remove('mvn_kp::spacecraft::t21')
-    created_vars.remove('mvn_kp::spacecraft::t22')
-    created_vars.remove('mvn_kp::spacecraft::t23')
-    created_vars.remove('mvn_kp::spacecraft::t31')
-    created_vars.remove('mvn_kp::spacecraft::t32')
-    created_vars.remove('mvn_kp::spacecraft::t33')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t11')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t12')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t13')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t21')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t22')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t23')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t31')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t32')
-    created_vars.remove('mvn_kp::spacecraft::spacecraft_t33')
+    pytplot.join_vec(
+        [
+            "mvn_kp::spacecraft::t11",
+            "mvn_kp::spacecraft::t12",
+            "mvn_kp::spacecraft::t13",
+            "mvn_kp::spacecraft::t21",
+            "mvn_kp::spacecraft::t22",
+            "mvn_kp::spacecraft::t23",
+            "mvn_kp::spacecraft::t31",
+            "mvn_kp::spacecraft::t32",
+            "mvn_kp::spacecraft::t33",
+        ],
+        "mvn_kp::geo_to_mso_matrix",
+    )
+
+    pytplot.del_data(
+        [
+            "mvn_kp::spacecraft::t11",
+            "mvn_kp::spacecraft::t12",
+            "mvn_kp::spacecraft::t13",
+            "mvn_kp::spacecraft::t21",
+            "mvn_kp::spacecraft::t22",
+            "mvn_kp::spacecraft::t23",
+            "mvn_kp::spacecraft::t31",
+            "mvn_kp::spacecraft::t32",
+            "mvn_kp::spacecraft::t33",
+        ]
+    )
+
+    pytplot.join_vec(
+        [
+            "mvn_kp::spacecraft::spacecraft_t11",
+            "mvn_kp::spacecraft::spacecraft_t12",
+            "mvn_kp::spacecraft::spacecraft_t13",
+            "mvn_kp::spacecraft::spacecraft_t21",
+            "mvn_kp::spacecraft::spacecraft_t22",
+            "mvn_kp::spacecraft::spacecraft_t23",
+            "mvn_kp::spacecraft::spacecraft_t31",
+            "mvn_kp::spacecraft::spacecraft_t32",
+            "mvn_kp::spacecraft::spacecraft_t33",
+        ],
+        "mvn_kp::spacecraft_to_mso_matrix",
+    )
+
+    pytplot.del_data(
+        [
+            "mvn_kp::spacecraft::spacecraft_t11",
+            "mvn_kp::spacecraft::spacecraft_t12",
+            "mvn_kp::spacecraft::spacecraft_t13",
+            "mvn_kp::spacecraft::spacecraft_t21",
+            "mvn_kp::spacecraft::spacecraft_t22",
+            "mvn_kp::spacecraft::spacecraft_t23",
+            "mvn_kp::spacecraft::spacecraft_t31",
+            "mvn_kp::spacecraft::spacecraft_t32",
+            "mvn_kp::spacecraft::spacecraft_t33",
+        ]
+    )
+
+    created_vars.remove("mvn_kp::spacecraft::t11")
+    created_vars.remove("mvn_kp::spacecraft::t12")
+    created_vars.remove("mvn_kp::spacecraft::t13")
+    created_vars.remove("mvn_kp::spacecraft::t21")
+    created_vars.remove("mvn_kp::spacecraft::t22")
+    created_vars.remove("mvn_kp::spacecraft::t23")
+    created_vars.remove("mvn_kp::spacecraft::t31")
+    created_vars.remove("mvn_kp::spacecraft::t32")
+    created_vars.remove("mvn_kp::spacecraft::t33")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t11")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t12")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t13")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t21")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t22")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t23")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t31")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t32")
+    created_vars.remove("mvn_kp::spacecraft::spacecraft_t33")
 
     inst_list = ["EUV", "LPW", "STATIC", "SWEA", "SWIA", "MAG", "SEP", "NGIMS"]
     for instrument in inst_list:
         # for each observation for each instrument
         if instrument in insitu:
             if insitu[instrument] is not None:
                 for obs in insitu[instrument]:
                     # create variable name
                     obs_specific = "mvn_kp::" + instrument.lower() + "::" + obs.lower()
                     try:
                         # store data in tplot variable
-                        pytplot.store_data(obs_specific, data={'x': insitu['Time'], 'y': insitu[instrument][obs]})
+                        pytplot.store_data(
+                            obs_specific,
+                            data={"x": insitu["Time"], "y": insitu[instrument][obs]},
+                        )
                         created_vars.append(obs_specific)
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::altitude", link_type='alt')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::mso_x", link_type='x')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::mso_y", link_type='y')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::mso_z", link_type='z')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::geo_x", link_type='geo_x')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::geo_y", link_type='geo_y')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::geo_z", link_type='geo_z')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::sub_sc_longitude", link_type='lon')
-                        pytplot.link(obs_specific, "mvn_kp::spacecraft::sub_sc_latitude", link_type='lat')
+                        pytplot.link(
+                            obs_specific,
+                            "mvn_kp::spacecraft::altitude",
+                            link_type="alt",
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::mso_x", link_type="x"
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::mso_y", link_type="y"
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::mso_z", link_type="z"
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::geo_x", link_type="geo_x"
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::geo_y", link_type="geo_y"
+                        )
+                        pytplot.link(
+                            obs_specific, "mvn_kp::spacecraft::geo_z", link_type="geo_z"
+                        )
+                        pytplot.link(
+                            obs_specific,
+                            "mvn_kp::spacecraft::sub_sc_longitude",
+                            link_type="lon",
+                        )
+                        pytplot.link(
+                            obs_specific,
+                            "mvn_kp::spacecraft::sub_sc_latitude",
+                            link_type="lat",
+                        )
                     except:
                         pass
-    return created_vars
+    return created_vars
```

### Comparing `pyspedas-1.5.6/pyspedas/maven/spdf/load.py` & `pyspedas-1.5.7/pyspedas/maven/spdf/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/maven/tests/tests.py` & `pyspedas-1.5.7/pyspedas/ulysses/tests/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,53 @@
-
 import os
 import unittest
 from pytplot import data_exists
-from pyspedas import maven
-from pyspedas.maven.download_files_utilities import get_orbit_files, merge_orbit_files
-
-
-class OrbitTestCases(unittest.TestCase):
-    def test_get_merge_orbit_files(self):
-        get_orbit_files()
-        merge_orbit_files()
-        self.assertTrue(os.path.join(os.path.join(os.path.dirname(__file__), '..'), 'maven_orb_rec.orb'))
+import pyspedas
 
 
 class LoadTestCases(unittest.TestCase):
-    def test_load_kp_data(self):
-        data = maven.kp()
-        self.assertTrue(data_exists('mvn_kp::spacecraft::geo_x'))
-
-    def test_load_mag_data(self):
-        data = maven.mag(datatype='ss1s')
-        self.assertTrue(data_exists('OB_B'))
-
-    def test_load_sta_data(self):
-        data = maven.sta()
-        self.assertTrue(data_exists('hkp_raw_2a-hkp'))
-        self.assertTrue(data_exists('hkp_2a-hkp'))
-
-    def test_load_swea_data(self):
-        data = maven.swea()
-        self.assertTrue(data_exists('diff_en_fluxes_svyspec'))
-
-    def test_load_swia_data(self):
-        data = maven.swia()
-        self.assertTrue(data_exists('spectra_diff_en_fluxes_onboardsvyspec'))
-
-    def test_load_sep_data(self):
-        data = maven.sep()
-        self.assertTrue(data_exists('f_ion_flux_tot_s2-cal-svy-full'))
-
-    #def test_load_lpw_data(self):
-    #    data = maven.lpw()
-    #    self.assertTrue(data_exists('mvn_lpw_lp_iv_l2_lpiv'))
-
-    def test_load_euv_data(self):
-        data = maven.euv()
-        self.assertTrue(data_exists('mvn_euv_calib_bands_bands'))
-
-    # def test_load_rse_data(self):
-    #     data = maven.rse()
-    #     self.assertTrue(data_exists(''))
-
-    # def test_load_iuv_data(self):
-    #     data = maven.iuv()
-    #     self.assertTrue(data_exists(''))
-
-    # def test_load_ngi_data(self):
-    #     data = maven.ngi()
-    #     self.assertTrue(data_exists(''))
+    def test_load_cospin_data(self):
+        data = pyspedas.ulysses.cospin()
+        self.assertTrue(data_exists('Protons'))
+        self.assertTrue(data_exists('Electrons'))
+        self.assertTrue(data_exists('HiE_protons'))
+        self.assertTrue(data_exists('Z_ge_3'))
+
+    def test_load_vhm_data(self):
+        data = pyspedas.ulysses.vhm()
+        self.assertTrue(data_exists('B_MAG'))
+        data = pyspedas.ulysses.vhm(notplot=True)
+        self.assertTrue('B_MAG' in data)
+
+    def test_load_swoops_data(self):
+        data = pyspedas.ulysses.swoops()
+        self.assertTrue(data_exists('Density'))
+        self.assertTrue(data_exists('Temperature'))
+        self.assertTrue(data_exists('Velocity'))
+        data = pyspedas.ulysses.swoops(datatype='proton-moments_swoops')
+        self.assertTrue(data_exists('Tpar'))
+        self.assertTrue(data_exists('Tper'))
+        self.assertTrue(data_exists('dens'))
+
+    def test_load_swics_data(self):
+        data = pyspedas.ulysses.swics()
+        self.assertTrue(data_exists('Velocity'))
+
+    def test_load_epac_data(self):
+        data = pyspedas.ulysses.epac()
+        self.assertTrue(data_exists('Omni_Protons'))
+
+    def test_load_hiscale_data(self):
+        data = pyspedas.ulysses.hiscale()
+        self.assertTrue(data_exists('Electrons'))
+        
+    def test_load_grb_data(self):
+        data = pyspedas.ulysses.grb()
+        self.assertTrue(data_exists('Count_Rate'))
+
+    def test_downloadonly(self):
+        files = pyspedas.ulysses.urap(downloadonly=True, trange=['2003-01-01', '2003-01-02'])
+        self.assertTrue(os.path.exists(files[0]))
+
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/maven/utilities.py` & `pyspedas-1.5.7/pyspedas/maven/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,126 @@
-# Copyright 2017 Regents of the University of Colorado. All Rights Reserved.
-# Released under the MIT license.
-# This software was developed at the University of Colorado's Laboratory for Atmospheric and Space Physics.
-# Verify current version before use at: https://github.com/MAVENSDC/Pydivide
-
 import logging
 import re
 import os
 from . import download_files_utilities as utils
-from .file_regex import kp_regex, l2_regex
+from .file_regex import maven_kp_l2_regex
 import numpy as np
 import collections
 
 
 def param_list(kp):
-    '''
+    """
     Return a listing of all parameters present in the given
     insitu data dictionary/structure.
 
-    Input:
+    Parameters:
         kp: insitu kp data structure/dictionary read from file(s)
     Output:
         ParamList: a list of all contained items and their indices.
-    '''
+    """
     import pandas as pd
+
     index = 1
     param_list_ = []
     for base_tag in kp.keys():
         if isinstance(kp[base_tag], pd.DataFrame):
             for obs_tag in kp[base_tag].columns:
                 param_list_.append("#%3d %s.%s" % (index, base_tag, obs_tag))
                 index += 1
         elif isinstance(kp[base_tag], pd.Series):
             param_list_.append("#%3d %s" % (index, base_tag))
             index += 1
         elif isinstance(kp[base_tag], pd.Index):
             param_list_.append("#%3d %s" % (index, base_tag))
             index += 1
         else:
-            logging.warning('*****WARNING*****')
-            logging.warning('Returning INCOMPLETE Parameter List')
-            logging.warning('Base tag neither DataFrame nor Series')
-            logging.warning('Plese check read_insitu_file definition')
+            logging.warning("*****WARNING*****")
+            logging.warning("Returning INCOMPLETE Parameter List")
+            logging.warning("Base tag neither DataFrame nor Series")
+            logging.warning("Plese check read_insitu_file definition")
 
     return param_list_
 
 
-# ---------------------------------------------------------------------
-
-
 def param_range(kp, iuvs=None):
-    '''
+    """
     Print the range of times and orbits for the provided insitu data.
     If iuvs data are also provided, return only orbit numbers for IUVS data.
 
     Caveats:
         At present, not configured to handle (real) IUVS data.
         Current configuration of procedure assumes IUVS has identical
             time information as in-situ.
 
-    Input:
+    Parameters:
         kp: insitu kp data structure/dictionary
         iuvs: IUVS kp data strucure/dictionary
     Output:
         None: prints information to screen
-    '''
+    """
 
     # First, the case where insitu data are provided
-    print("The loaded insitu KP data set contains data between")
-    print("   %s and %s" % (np.array(kp['TimeString'])[0], np.array(kp['TimeString'])[-1]))
-    print("Equivalently, this corresponds to orbits")
-    print("   %6d and %6d." % (np.array(kp['Orbit'])[0], np.array(kp['Orbit'])[-1]))
+    logging.warning("The loaded insitu KP data set contains data between")
+    logging.warning(
+        "   %s and %s" % (np.array(kp["TimeString"])[0], np.array(kp["TimeString"])[-1])
+    )
+    logging.warning("Equivalently, this corresponds to orbits")
+    logging.warning(
+        "   %6d and %6d." % (np.array(kp["Orbit"])[0], np.array(kp["Orbit"])[-1])
+    )
 
     #  Next, the case where IUVS data are provided
     iuvs_data = False
-    iuvs_tags = ['CORONA_LO_HIGH', 'CORONA_LO_LIMB', 'CORONA_LO_DISK',
-                 'CORONA_E_HIGH', 'CORONA_E_LIMB', 'CORONA_E_DISK',
-                 'APOAPSE', 'PERIAPSE', 'STELLAR_OCC']
+    iuvs_tags = [
+        "CORONA_LO_HIGH",
+        "CORONA_LO_LIMB",
+        "CORONA_LO_DISK",
+        "CORONA_E_HIGH",
+        "CORONA_E_LIMB",
+        "CORONA_E_DISK",
+        "APOAPSE",
+        "PERIAPSE",
+        "STELLAR_OCC",
+    ]
     if kp.keys() in iuvs_tags:
-        print("The loaded IUVS KP data set contains data between orbits")
-        print("   %6d and %6d." % (np.array(kp['Orbit'])[0], np.array(kp['Orbit'])[-1]))
+        logging.warning("The loaded IUVS KP data set contains data between orbits")
+        logging.warning(
+            "   %6d and %6d." % (np.array(kp["Orbit"])[0], np.array(kp["Orbit"])[-1])
+        )
 
     #  Finally, the case where both insitu and IUVS are provided
     if iuvs is not None:
-        print("The loaded IUVS KP data set contains data between orbits")
-        print("   %6d and %6d." % (np.array(iuvs['Orbit'])[0], np.array(iuvs['Orbit'])[-1]))
-        insitu_min, insitu_max = (np.nanmin([kp['Orbit']]), np.nanmax([kp['Orbit']]))
-        if np.nanmax([iuvs['Orbit']]) < insitu_min or np.nanmin([iuvs['Orbit']]) > insitu_max:
-            print("*** WARNING ***")
-            print("There is NO overlap between the supplied insitu and IUVS")
-            print("  data structures.  We cannot guarantee your safety ")
-            print("  should you attempt to display these IUVS data against")
-            print("  these insitu-supplied emphemeris data.")
+        logging.warning("The loaded IUVS KP data set contains data between orbits")
+        logging.warning(
+            "   %6d and %6d."
+            % (np.array(iuvs["Orbit"])[0], np.array(iuvs["Orbit"])[-1])
+        )
+        insitu_min, insitu_max = (np.nanmin([kp["Orbit"]]), np.nanmax([kp["Orbit"]]))
+        if (
+            np.nanmax([iuvs["Orbit"]]) < insitu_min
+            or np.nanmin([iuvs["Orbit"]]) > insitu_max
+        ):
+            logging.warning("*** WARNING ***")
+            logging.warning("There is NO overlap between the supplied insitu and IUVS")
+            logging.warning("  data structures.  We cannot guarantee your safety ")
+            logging.warning("  should you attempt to display these IUVS data against")
+            logging.warning("  these insitu-supplied emphemeris data.")
     return  # No information to return
 
 
-# --------------------------------------------------------------------------
-
-
 def range_select(kp, time=None, parameter=None, maximum=None, minimum=None):
-    '''
+    """
     Returns a subset of the input data based on the provided time
     and/or parameter criteria.  If neither Time nor Parameter filter
     information is provided, then no subselection of data will occur.
     Any parameter used as a filtering criterion must be paired with
     either a maximum and/or a minimum value.  Open ended bounds must
     be indicated with either a value of 'None' or an empty string ('').
 
-    Input:
+    Parameters:
         kp: insitu kp data structure/dictionary read from file(s)
         time: two-element time range must be either strings of format
             'yyyy-mm-ddThh:mm:ss' or integers (orbit numbers)
         parameter: Element of provided data structure/dictionary by
             which to filter data.  Parameter(s) must be either integer
             type (search by index) or string type (search by instrument
             name and observation type).  If multiple Parameters are used
@@ -124,35 +134,35 @@
             None or '' will leave the Parameter filter unbounded below.
             The number of elements of Minimum *MUST* equal the number of
             elements of Parameter.
     Output: a dictionary/structure containing the same elements as the provided
         one, but filtered according to the Time and Parameter options.
 
     ToDo: compartmentalize the filtering and/or argument checks.
-    '''
+    """
     from datetime import datetime
 
     #  Initialize the filter_list
     filter_list = []
 
     # First, check the arguments
     if time is None and parameter is None:
         insufficient_input_range_select()
-        print('Neither Time nor Parameter provided')
+        logging.warning("Neither Time nor Parameter provided")
         return kp
     elif time is None:
         # Then only subset based on parameters
         # Need to check whether one or several Parameters given
         inst = []
         obs = []
         if isinstance(parameter, int) or isinstance(parameter, str):
             # First, verify that at least one bound exists
             if minimum is None and maximum is None:
                 insufficient_input_range_select()
-                print('No bounds set for parameter: %s' % parameter)
+                logging.warning("No bounds set for parameter: %s" % parameter)
                 return kp
             elif minimum is None:
                 # Range only bounded above
                 minimum = -np.Infinity
             elif maximum is None:
                 # range only bounded below
                 maximum = np.Infinity
@@ -166,121 +176,122 @@
         elif type(parameter) is list:
             nparam = len(parameter)
             for param in parameter:
                 a, b = get_inst_obs_labels(kp, param)
                 inst.append(a)
                 obs.append(b)
         else:
-            print('*****ERROR*****')
-            print('Cannot identify given parameter: %s' % parameter)
-            print('Suggest using param_list(kp) to identify Parameter')
-            print('by index or by name')
-            print('Returning complete original data dictionary')
+            logging.warning("*****ERROR*****")
+            logging.warning("Cannot identify given parameter: %s" % parameter)
+            logging.warning("Suggest using param_list(kp) to identify Parameter")
+            logging.warning("by index or by name")
+            logging.warning("Returning complete original data dictionary")
             return kp
 
     # Should I move this below the Time conditional and move
     # Baselining of Filter List to above time
 
     else:
         # Time has been provided as a filtering agent
         # Determine whether Time is provided as strings or orbits
         if len(time) != 2:
             if parameter is not None:
-                print('*****WARNING*****')
-                print('Time must be provided as a two-element list')
-                print('of either strings (yyyy-mm-dd hh:mm:ss) ')
-                print('or orbits.  Since a Parameter *was* provided,')
-                print('I will filter on that, but ignore the time input.')
+                logging.warning("*****WARNING*****")
+                logging.warning("Time must be provided as a two-element list")
+                logging.warning("of either strings (yyyy-mm-dd hh:mm:ss) ")
+                logging.warning("or orbits.  Since a Parameter *was* provided,")
+                logging.warning("I will filter on that, but ignore the time input.")
             else:
                 # Cannot proceed with filtering
                 insufficient_input_range_select()
-                print('Time malformed must be either a string of format')
-                print('yyyy-mm-ddThh:mm:ss or integer orbit)')
-                print('and no Parameter criterion given')
+                logging.warning("Time malformed must be either a string of format")
+                logging.warning("yyyy-mm-ddThh:mm:ss or integer orbit)")
+                logging.warning("and no Parameter criterion given")
         else:
             # We have a two-element Time list: parse it
             if not isinstance(type(time[0]), type(time[1])):
                 if parameter is not None:
-                    print('*****WARNING*****')
-                    print('Both elements of time must be same type')
-                    print('Only strings of format yyyy-mm-dd hh:mm:ss')
-                    print('or integers (orbit numbers) are allowed.')
-                    print('Ignoring time inputs; will filter ONLY')
-                    print('on Parameter inputs.')
+                    logging.warning("*****WARNING*****")
+                    logging.warning("Both elements of time must be same type")
+                    logging.warning("Only strings of format yyyy-mm-dd hh:mm:ss")
+                    logging.warning("or integers (orbit numbers) are allowed.")
+                    logging.warning("Ignoring time inputs; will filter ONLY")
+                    logging.warning("on Parameter inputs.")
                 else:
-                    print('*****ERROR*****')
-                    print('Both elements of Time must be same type')
-                    print('Only Strings of format yyyy-mm-dd hh:mm:ss')
-                    print('or integers (orbit numbers) are allowed.')
-                    print('Returning original unchanged data dictionary')
+                    logging.warning("*****ERROR*****")
+                    logging.warning("Both elements of Time must be same type")
+                    logging.warning("Only Strings of format yyyy-mm-dd hh:mm:ss")
+                    logging.warning("or integers (orbit numbers) are allowed.")
+                    logging.warning("Returning original unchanged data dictionary")
                     return kp
             elif type(time[0]) is int:
                 # Filter based on orbit number
                 min_t = min(time)
                 max_t = max(time)
-                filter_list.append(kp['Orbit'] >= min_t)
-                filter_list.append(kp['Orbit'] <= max_t)
+                filter_list.append(kp["Orbit"] >= min_t)
+                filter_list.append(kp["Orbit"] <= max_t)
             elif isinstance(time[0], str):
                 # Filter acc to string dat, need to parse it
-                time_dt = [datetime.strptime(i, '%Y-%m-%d %H:%M:%S') for i in time]
+                time_dt = [datetime.strptime(i, "%Y-%m-%d %H:%M:%S") for i in time]
                 min_dt = min(time_dt)
                 max_dt = max(time_dt)
-                kp_dt = [datetime.strptime(i, '%Y-%m-%dT%H:%M:%S')
-                         for i in kp['TimeString']]
+                kp_dt = [
+                    datetime.strptime(i, "%Y-%m-%dT%H:%M:%S") for i in kp["TimeString"]
+                ]
                 delta_tmin = np.array([(i - min_dt).total_seconds() for i in kp_dt])
                 delta_tmax = np.array([(i - max_dt).total_seconds() for i in kp_dt])
                 filter_list.append(delta_tmin >= 0)
                 filter_list.append(delta_tmax <= 0)
             else:
                 # Time provided as other than string or Integer
                 if parameter is not None:
-                    print('*****WARNING*****')
-                    print('Both elements of time must be same type')
-                    print('Only strings of format yyyy-mm-dd hh:mm:ss')
-                    print('or integers (orbit numbers) are allowed.')
-                    print('Ignoring time inputs; will filter ONLY')
-                    print('on Parameter inputs.')
+                    logging.warning("*****WARNING*****")
+                    logging.warning("Both elements of time must be same type")
+                    logging.warning("Only strings of format yyyy-mm-dd hh:mm:ss")
+                    logging.warning("or integers (orbit numbers) are allowed.")
+                    logging.warning("Ignoring time inputs; will filter ONLY")
+                    logging.warning("on Parameter inputs.")
                 else:
-                    print('*****ERROR*****')
-                    print('Both elements of Time must be same type')
-                    print('Only Strings of format yyyy-mm-dd hh:mm:ss')
-                    print('or integers (orbit numbers) are allowed.')
-                    print('Returning original unchanged data dictionary')
+                    logging.warning("*****ERROR*****")
+                    logging.warning("Both elements of Time must be same type")
+                    logging.warning("Only Strings of format yyyy-mm-dd hh:mm:ss")
+                    logging.warning("or integers (orbit numbers) are allowed.")
+                    logging.warning("Returning original unchanged data dictionary")
                     return kp
             # Now, we apply the Parameter selection
             inst = []
             obs = []
             if isinstance(parameter, int) or isinstance(parameter, str):
                 # Then we have a single Parameter to filter on
                 # Verify that bounds info exists
                 if minimum is None and maximum is None:
                     insufficient_input_range_select()
-                    print('No bounds set for parameter %s' % parameter)
-                    print('Applying only Time filtering')
+                    logging.warning("No bounds set for parameter %s" % parameter)
+                    logging.warning("Applying only Time filtering")
                     parameter = None
                 elif minimum is None:
                     minimum = -np.Infinity  # Unbounded below
                 elif maximum is None:
                     maximum = np.Infinity  # Unbounded above
                 else:
                     pass  # Range fully bounded
                 a, b = get_inst_obs_labels(kp, parameter)
                 inst.append(a)
                 obs.append(b)
                 nparam = 1  # necessary?
             elif type(parameter) is list:
                 if len(parameter) != len(minimum) or len(parameter) != len(maximum):
-                    print('*****ERROR*****')
-                    print('---range_select---')
-                    print('Number of minima and maxima provided')
-                    print('MUST match number of Parameters provided')
-                    print('You provided %4d Parameters' % len(parameter))
-                    print('             %4d minima' % len(minimum))
-                    print('         and %4d maxima' % len(maximum))
-                    print('Filtering only on Time')
+                    logging.warning("*****ERROR*****")
+                    logging.warning("---range_select---")
+                    logging.warning("Number of minima and maxima provided")
+                    logging.warning("MUST match number of Parameters provided")
+                    logging.warning("You provided %4d Parameters" % len(parameter))
+                    logging.warning("             %4d minima" % len(minimum))
+                    logging.warning("         and %4d maxima" % len(maximum))
+                    logging.warning("Filtering only on Time")
                     parameter = None
                 else:
                     nparam = len(parameter)
                     for param in parameter:
                         a, b = get_inst_obs_labels(kp, param)
                         inst.append(a)
                         obs.append(b)
@@ -297,318 +308,395 @@
     new = {}
     for i in kp:
         temp = kp[i]
         new.update({i: temp[filter]})
     return new
 
 
-# --------------------------------------------------------------------------
-
-
 def insufficient_input_range_select():
-    '''
+    """
     This error message is called if user calls range_select with
     inputs that result in neither a valid Time range nor a valid
     Parameter range capable of being determined
 
     ToDo: Is there a way to hide this from the help feature?
-    '''
-    print('*****ERROR*****')
-    print('Either a time criterion with two values.')
-    print('  or a parameter name with maximum and/or')
-    print('  minimum values must be provided.')
-    print('Returning the complete original data dictionary')
-
+    """
+    logging.warning("*****ERROR*****")
+    logging.warning("Either a time criterion with two values.")
+    logging.warning("  or a parameter name with maximum and/or")
+    logging.warning("  minimum values must be provided.")
+    logging.warning("Returning the complete original data dictionary")
 
-# --------------------------------------------------------------------------
 
 def get_inst_obs_labels(kp, name):
-    '''
+    """
     Given parameter input in either string or integer format,
     identify the instrument name and observation type for use
     in accessing the relevant part of the data structure
     E.g.: 'LPW.EWAVE_LOW_FREQ' would be returned as
           ['LPW', 'EWAVE_LOW_FREQ']
 
-    Input:
+    Parameters:
         kp: insitu kp data structure/dictionary read from file(s)
         name: string identifying a parameter.
             (Indices must be converted to inst.obs strings before
              calling this routine)
     Output:
         inst (1st arg): instrument identifier
         obs (2nd arg): observation type identifier
-    '''
+    """
 
     # Need to ensure name is a string at this stage
-    name = ('%s' % name)
+    name = "%s" % name
 
     # Now, split at the dot (if it exists)
-    tags = name.split('.')
+    tags = name.split(".")
     # And consider the various possibilities...
     if len(tags) == 2:
         return tags
     elif len(tags) == 1:
         try:
             int(tags[0])
-            return (find_param_from_index(kp, tags[0])).split('.')
+            return (find_param_from_index(kp, tags[0])).split(".")
         except:
-            print('*****ERROR*****')
-            print('%s is an invalid parameter' % name)
-            print('If only one value is provided, it must be an integer')
+            logging.warning("*****ERROR*****")
+            logging.warning("%s is an invalid parameter" % name)
+            logging.warning("If only one value is provided, it must be an integer")
             return
     else:
-        print('*****ERROR*****')
-        print('%s is not a valid parameter' % name)
-        print('because it has %1d elements' % len(tags))
-        print('Only 1 integer or string of form "a.b" are allowed.')
-        print('Please use .param_list attribute to find valid parameters')
+        logging.warning("*****ERROR*****")
+        logging.warning("%s is not a valid parameter" % name)
+        logging.warning("because it has %1d elements" % len(tags))
+        logging.warning('Only 1 integer or string of form "a.b" are allowed.')
+        logging.warning("Please use .param_list attribute to find valid parameters")
         return
 
 
 def find_param_from_index(kp, index):
-    '''
+    """
     Given an integer index, find the name of the parameter
 
-    Input:
+    Parameters:
         kp: insitu kp data structure/dictionary read from file(s)
         index: the index of the desired parameter (integer type)
     Output:
         A string of form <instrument>.<observation>
         (e.g., LPW.EWAVE_LOW_FREQ)
-    '''
+    """
 
-    index = '#%3d' % int(index)
+    index = "#%3d" % int(index)
     plist = param_list(kp)
     found = False
     for i in plist:
         if re.search(index, i):
             return i[5:]  # clip the '#123 ' string
     if not found:
-        print('*****ERROR*****')
-        print('%s not a valid index.' % index)
-        print('Use param_list to list options')
+        logging.warning("*****ERROR*****")
+        logging.warning("%s not a valid index." % index)
+        logging.warning("Use param_list to list options")
         return
 
 
 def remove_inst_tag(df):
-    '''
+    """
     Remove the leading part of the column name that includes the instrument
     identifier for use in creating the parameter names for the toolkit.
 
-    Input:
+    Parameters:
         A DataFrame produced from the insitu KP data
     Output:
         A new set of column names
-    '''
+    """
 
     newcol = []
     for i in df.columns:
-        if len(i.split('.')) >= 2:
-            j = i.split('.')
-            newcol.append('.'.join(j[1:]))
+        if len(i.split(".")) >= 2:
+            j = i.split(".")
+            newcol.append(".".join(j[1:]))
 
     return newcol
 
 
 def get_latest_files_from_date_range(date1, date2):
+    """
+    Retrieves the latest files from a given date range.
+
+    Parameters:
+        date1 (datetime): The start date of the range.
+        date2 (datetime): The end date of the range.
+
+    Returns:
+        list: A list of file paths representing the latest files within the date range.
+    """
+
     from datetime import timedelta
 
     mvn_root_data_dir = utils.get_root_data_dir()
-    maven_data_dir = os.path.join(mvn_root_data_dir, 'maven', 'data', 'sci', 'kp', 'insitu')
+    maven_data_dir = os.path.join(
+        mvn_root_data_dir, "maven", "data", "sci", "kp", "insitu"
+    )
 
     # Each file starts at midnight, so lets cut off the hours and just pay attention to the days
     date1 = date1.replace(hour=0, minute=0, second=0)
     date2 = date2.replace(hour=0, minute=0, second=0) + timedelta(days=1)
 
     time_spanned = date2 - date1
     num_days = time_spanned.days
 
     filenames = []
+    kp_regex, l2_regex = maven_kp_l2_regex()
 
     for i in range(num_days):
         current_date = date1 + timedelta(days=i)
         year = str(current_date.year)
-        month = str('%02d' % current_date.month)
-        day = str('%02d' % current_date.day)
+        month = str("%02d" % current_date.month)
+        day = str("%02d" % current_date.day)
         full_path = os.path.join(maven_data_dir, year, month)
         if os.path.exists(full_path):
             # Grab only the most recent version/revision of regular and crustal insitu files for each
             # day
             insitu = {}
             c_insitu = {}
             for f in os.listdir(full_path):
-                # print(f)
-                if kp_regex.match(f).group('day') == day and not kp_regex.match(f).group('description'):
-                    v = kp_regex.match(f).group('version')
-                    r = kp_regex.match(f).group('revision')
+                # logging.warning(f)
+                if kp_regex.match(f).group("day") == day and not kp_regex.match(
+                    f
+                ).group("description"):
+                    v = kp_regex.match(f).group("version")
+                    r = kp_regex.match(f).group("revision")
                     insitu[f] = [v, r]
-                elif kp_regex.match(f).group('day') == day and kp_regex.match(f).group('description') == '_crustal':
-                    v = kp_regex.match(f).group('version')
-                    r = kp_regex.match(f).group('revision')
+                elif (
+                    kp_regex.match(f).group("day") == day
+                    and kp_regex.match(f).group("description") == "_crustal"
+                ):
+                    v = kp_regex.match(f).group("version")
+                    r = kp_regex.match(f).group("revision")
                     c_insitu[f] = [v, r]
 
             if insitu:
                 # Get max version
                 insitu_file = max(insitu.keys(), key=(lambda k: insitu[k][0]))
-                max_v = re.search('v\d{2}', insitu_file).group(0)
+                max_v = re.search("v\d{2}", insitu_file).group(0)
                 # Get max revision
-                max_r = max([re.search('r\d{2}', k).group(0) for k in insitu if max_v in k])
+                max_r = max(
+                    [re.search("r\d{2}", k).group(0) for k in insitu if max_v in k]
+                )
                 # Get most recent insitu file (based on max version, and then max revision values)
-                most_recent_insitu = [f for f in insitu.keys() if max_r in f and max_v in f]
+                most_recent_insitu = [
+                    f for f in insitu.keys() if max_r in f and max_v in f
+                ]
                 filenames.append(os.path.join(full_path, most_recent_insitu[0]))
 
             if c_insitu:
                 # Get max version
                 c_insitu_file = max(c_insitu.keys(), key=(lambda k: c_insitu[k][0]))
-                c_max_v = re.search('v\d{2}', c_insitu_file).group(0)
+                c_max_v = re.search("v\d{2}", c_insitu_file).group(0)
                 # Get max revision
-                c_max_r = max([re.search('r\d{2}', k).group(0) for k in c_insitu if c_max_v in k])
+                c_max_r = max(
+                    [re.search("r\d{2}", k).group(0) for k in c_insitu if c_max_v in k]
+                )
                 # Get most recent insitu file (based on max version, and then max revision values)
-                most_recent_c_insitu = [f for f in c_insitu.keys() if c_max_r in f and c_max_v in f]
+                most_recent_c_insitu = [
+                    f for f in c_insitu.keys() if c_max_r in f and c_max_v in f
+                ]
                 filenames.append(os.path.join(full_path, most_recent_c_insitu[0]))
 
     filenames = sorted(filenames)
     return filenames
 
 
 def get_latest_iuvs_files_from_date_range(date1, date2):
+    """
+    Get the latest IUVS files from a given date range.
+
+    Parameters:
+        date1 (datetime): The start date of the range.
+        date2 (datetime): The end date of the range.
+
+    Returns:
+        list: A sorted list of file paths for the latest IUVS files within the date range.
+    """
+
     from datetime import timedelta
 
+    kp_regex, l2_regex = maven_kp_l2_regex()
     mvn_root_data_dir = utils.get_root_data_dir()
-    maven_data_dir = os.path.join(mvn_root_data_dir, 'maven', 'data', 'sci', 'kp', 'iuvs')
+    maven_data_dir = os.path.join(
+        mvn_root_data_dir, "maven", "data", "sci", "kp", "iuvs"
+    )
 
     # Each file starts at midnight, so lets cut off the hours and just pay attention to the days
     date1 = date1.replace(hour=0, minute=0, second=0)
     date2 = date2.replace(day=date2.day, hour=0, minute=0, second=0) + timedelta(days=1)
 
     time_spanned = date2 - date1
     num_days = time_spanned.days
 
     files_to_return = []
     for i in range(num_days):
         current_date = date1 + timedelta(days=i)
         year = str(current_date.year)
-        month = str('%02d' % current_date.month)
-        day = str('%02d' % current_date.day)
+        month = str("%02d" % current_date.month)
+        day = str("%02d" % current_date.day)
         full_path = os.path.join(maven_data_dir, year, month)
         if os.path.exists(full_path):
             basenames = []
             # Obtain a list of all the basenames for the day
             for f in os.listdir(full_path):
-                if kp_regex.match(f).group('day') == day:
-                    description = kp_regex.match(f).group('description')
-                    year = kp_regex.match(f).group('year')
-                    month = kp_regex.match(f).group('month')
-                    day = kp_regex.match(f).group('day')
-                    time = kp_regex.match(f).group('time')
-                    seq = ('mvn', 'kp', 'iuvs' + description, year + month + day + time)
-                    basenames.append('_'.join(seq))
+                if kp_regex.match(f).group("day") == day:
+                    description = kp_regex.match(f).group("description")
+                    year = kp_regex.match(f).group("year")
+                    month = kp_regex.match(f).group("month")
+                    day = kp_regex.match(f).group("day")
+                    time = kp_regex.match(f).group("time")
+                    seq = ("mvn", "kp", "iuvs" + description, year + month + day + time)
+                    basenames.append("_".join(seq))
 
             basenames = list(set(basenames))
 
             for bn in basenames:
                 version = 0
                 revision = 0
                 for f in os.listdir(full_path):
-                    description = kp_regex.match(f).group('description')
-                    year = kp_regex.match(f).group('year')
-                    month = kp_regex.match(f).group('month')
-                    day = kp_regex.match(f).group('day')
-                    time = kp_regex.match(f).group('time')
-                    seq = ('mvn', 'kp', 'iuvs' + description, year + month + day + time)
-                    if bn == '_'.join(seq):
-                        v = kp_regex.match(f).group('version')
+                    description = kp_regex.match(f).group("description")
+                    year = kp_regex.match(f).group("year")
+                    month = kp_regex.match(f).group("month")
+                    day = kp_regex.match(f).group("day")
+                    time = kp_regex.match(f).group("time")
+                    seq = ("mvn", "kp", "iuvs" + description, year + month + day + time)
+                    if bn == "_".join(seq):
+                        v = kp_regex.match(f).group("version")
                         if int(v) > int(version):
                             version = v
 
                 for f in os.listdir(full_path):
-                    description = kp_regex.match(f).group('description')
-                    year = kp_regex.match(f).group('year')
-                    month = kp_regex.match(f).group('month')
-                    day = kp_regex.match(f).group('day')
-                    time = kp_regex.match(f).group('time')
-                    file_version = kp_regex.match(f).group('version')
-                    seq = ('mvn', 'kp', 'iuvs' + description, year + month + day + time)
-                    if bn == '_'.join(seq) and file_version == version:
-                        r = kp_regex.match(f).group('revision')
+                    description = kp_regex.match(f).group("description")
+                    year = kp_regex.match(f).group("year")
+                    month = kp_regex.match(f).group("month")
+                    day = kp_regex.match(f).group("day")
+                    time = kp_regex.match(f).group("time")
+                    file_version = kp_regex.match(f).group("version")
+                    seq = ("mvn", "kp", "iuvs" + description, year + month + day + time)
+                    if bn == "_".join(seq) and file_version == version:
+                        r = kp_regex.match(f).group("revision")
                         if int(r) > int(revision):
                             revision = r
                 if int(version) > 0:
-                    seq = (bn, 'v' + str(version), 'r' + str(revision) + '.tab')
-                    files_to_return.append(os.path.join(full_path, '_'.join(seq)))
+                    seq = (bn, "v" + str(version), "r" + str(revision) + ".tab")
+                    files_to_return.append(os.path.join(full_path, "_".join(seq)))
     files_to_return = sorted(files_to_return)
     return files_to_return
 
 
 def get_l2_files_from_date(date1, instrument):
+    """
+    Retrieves a list of Level 2 files for a given date and instrument.
+
+    Parameters:
+        date1 (datetime.datetime): The date for which to retrieve the files.
+        instrument (str): The instrument name.
+
+    Returns:
+        list: A sorted list of file paths for the Level 2 files.
+    """
+
+    kp_regex, l2_regex = maven_kp_l2_regex()
     mvn_root_data_dir = utils.get_root_data_dir()
-    maven_data_dir = os.path.join(mvn_root_data_dir, 'maven', 'data', 'sci', instrument, 'l2')
+    maven_data_dir = os.path.join(
+        mvn_root_data_dir, "maven", "data", "sci", instrument, "l2"
+    )
 
     # Each file starts at midnight, so lets cut off the hours and just pay attention to the days
     date1 = date1.replace(hour=0, minute=0, second=0)
 
     filenames = []
 
     year = str(date1.year)
-    month = str('%02d' % date1.month)
-    day = str('%02d' % date1.day)
+    month = str("%02d" % date1.month)
+    day = str("%02d" % date1.day)
     full_path = os.path.join(maven_data_dir, year, month)
     if os.path.exists(full_path):
         for f in os.listdir(full_path):
-            if l2_regex.match(f).group('day') == day:
+            if l2_regex.match(f).group("day") == day:
                 filenames.append(os.path.join(full_path, f))
 
     filenames = sorted(filenames)
     return filenames
 
 
 def get_header_info(filename):
+    """
+    Extracts header information from a file.
+
+    Parameters:
+        filename (str): The path to the file.
+
+    Returns:
+        tuple: A tuple containing two lists - `names` and `inst`.
+            - `names` (list): A list of column names extracted from the header.
+            - `inst` (list): A list of instrument names extracted from the header.
+    """
+
+    # Rest of the code...
+
+
+def get_header_info(filename):
+    """
+    Extracts header information from a file.
+
+    Parameters:
+    filename (str): The path to the file.
+
+    Returns:
+    tuple: A tuple containing the names list and inst list.
+    """
     # Determine number of header lines
     nheader = 0
     with open(filename) as f:
         for line in f:
-            if line.startswith('#'):
+            if line.startswith("#"):
                 nheader += 1
 
     # Parse the header (still needs special case work)
     read_param_list = False
     start_temp = False
     index_list = []
     with open(filename) as fin:
         icol = -2  # Counting header lines detailing column names
         iname = 1  # for counting seven lines with name info
         ncol = -1  # Dummy value to allow reading of early headerlines?
-        col_regex = '#\s(.{16}){%3d}' % ncol  # needed for column names
+        col_regex = "#\s(.{16}){%3d}" % ncol  # needed for column names
         crustal = False
-        if 'crustal' in filename:
+        if "crustal" in filename:
             crustal = True
         for iline in range(nheader):
             line = fin.readline()
             # Define the proper indices change depending on the file type and row
             i = [2, 2, 1] if crustal else [1, 1, 1]
-            if re.search('Number of parameter columns', line):
+            if re.search("Number of parameter columns", line):
                 ncol = int(re.split("\s{3}", line)[i[0]])
                 # needed for column names
-                col_regex = '#\s(.{16}){%2d}' % ncol if crustal else '#\s(.{16}){%3d}' % ncol
-            elif re.search('Line on which data begins', line):
+                col_regex = (
+                    "#\s(.{16}){%2d}" % ncol if crustal else "#\s(.{16}){%3d}" % ncol
+                )
+            elif re.search("Line on which data begins", line):
                 nhead_test = int(re.split("\s{3}", line)[i[1]]) - 1
-            elif re.search('Number of lines', line):
+            elif re.search("Number of lines", line):
                 ndata = int(re.split("\s{3}", line)[i[2]])
-            elif re.search('PARAMETER', line):
+            elif re.search("PARAMETER", line):
                 read_param_list = True
                 param_head = iline
             elif read_param_list:
                 icol += 1
                 if icol > ncol:
                     read_param_list = False
             elif re.match(col_regex, line):
                 # OK, verified match now get the values
-                temp = re.findall('(.{16})', line[3:])
-                if temp[0] == '               1':
+                temp = re.findall("(.{16})", line[3:])
+                if temp[0] == "               1":
                     start_temp = True
                 if start_temp:
                     # Crustal files do not have as much variable info as other insitu files, need
                     # to modify the lines below
                     if crustal:
                         if iname == 1:
                             index = temp
@@ -616,18 +704,20 @@
                             obs1 = temp
                         elif iname == 3:
                             obs2 = temp
                         elif iname == 4:
                             unit = temp
                             # crustal files don't come with this field
                             # throwing it in here for consistency with other insitu files
-                            inst = ['     MODELED_MAG'] * 13
+                            inst = ["     MODELED_MAG"] * 13
                         else:
-                            print('More lines in data descriptor than expected.')
-                            print('Line %d' % iline)
+                            logging.warning(
+                                "More lines in data descriptor than expected."
+                            )
+                            logging.warning("Line %d" % iline)
                     else:
                         if iname == 1:
                             index = temp
                         elif iname == 2:
                             obs1 = temp
                         elif iname == 3:
                             obs2 = temp
@@ -636,170 +726,248 @@
                         elif iname == 5:
                             inst = temp
                         elif iname == 6:
                             unit = temp
                         elif iname == 7:
                             format_code = temp
                         else:
-                            print('More lines in data descriptor than expected.')
-                            print('Line %d' % iline)
+                            logging.warning(
+                                "More lines in data descriptor than expected."
+                            )
+                            logging.warning("Line %d" % iline)
                     iname += 1
             else:
                 pass
 
         # Generate the names list.
         # NB, there are special case redundancies in there
         # (e.g., LPW: Electron Density Quality (min and max))
         # ****SWEA FLUX electron QUALITY *****
         first = True
         parallel = None
         names = []
         if crustal:
             for h, i, j in zip(inst, obs1, obs2):
-                combo_name = (' '.join([i.strip(), j.strip()])).strip()
+                combo_name = (" ".join([i.strip(), j.strip()])).strip()
                 # Add inst to names to avoid ambiguity
                 # Will need to remove these after splitting
-                names.append('.'.join([h.strip(), combo_name]))
-                names[0] = 'Time'
+                names.append(".".join([h.strip(), combo_name]))
+                names[0] = "Time"
         else:
             for h, i, j, k in zip(inst, obs1, obs2, obs3):
-                combo_name = (' '.join([i.strip(), j.strip(), k.strip()])).strip()
-                if re.match('^LPW$', h.strip()):
+                combo_name = (" ".join([i.strip(), j.strip(), k.strip()])).strip()
+                if re.match("^LPW$", h.strip()):
                     # Max and min error bars use same name in column
                     # SIS says first entry is min and second is max
-                    if re.match('(Electron|Spacecraft)(.+)Quality', combo_name):
+                    if re.match("(Electron|Spacecraft)(.+)Quality", combo_name):
                         if first:
-                            combo_name = combo_name + ' Min'
+                            combo_name = combo_name + " Min"
                             first = False
                         else:
-                            combo_name = combo_name + ' Max'
+                            combo_name = combo_name + " Max"
                             first = True
-                elif re.match('^SWEA$', h.strip()):
+                elif re.match("^SWEA$", h.strip()):
                     # electron flux qual flags do not indicate whether parallel or anti
                     # From context it is clear; but we need to specify in name
-                    if re.match('.+Parallel.+', combo_name):
+                    if re.match(".+Parallel.+", combo_name):
                         parallel = True
-                    elif re.match('.+Anti-par', combo_name):
+                    elif re.match(".+Anti-par", combo_name):
                         parallel = False
                     else:
                         pass
-                    if re.match('Flux, e-(.+)Quality', combo_name):
+                    if re.match("Flux, e-(.+)Quality", combo_name):
                         if parallel:
-                            p = re.compile('Flux, e- ')
-                            combo_name = p.sub('Flux, e- Parallel ', combo_name)
+                            p = re.compile("Flux, e- ")
+                            combo_name = p.sub("Flux, e- Parallel ", combo_name)
                         else:
-                            p = re.compile('Flux, e- ')
-                            combo_name = p.sub('Flux, e- Anti-par ', combo_name)
-                    if re.match('Electron eflux (.+)Quality', combo_name):
+                            p = re.compile("Flux, e- ")
+                            combo_name = p.sub("Flux, e- Anti-par ", combo_name)
+                    if re.match("Electron eflux (.+)Quality", combo_name):
                         if parallel:
-                            p = re.compile('Electron eflux ')
-                            combo_name = p.sub('Electron eflux  Parallel ', combo_name)
+                            p = re.compile("Electron eflux ")
+                            combo_name = p.sub("Electron eflux  Parallel ", combo_name)
                         else:
-                            p = re.compile('Electron eflux ')
-                            combo_name = p.sub('Electron eflux  Anti-par ', combo_name)
+                            p = re.compile("Electron eflux ")
+                            combo_name = p.sub("Electron eflux  Anti-par ", combo_name)
                 # Add inst to names to avoid ambiguity
                 # Will need to remove these after splitting
-                names.append('.'.join([h.strip(), combo_name]))
-                names[0] = 'Time'
+                names.append(".".join([h.strip(), combo_name]))
+                names[0] = "Time"
 
     return names, inst
 
 
 def initialize_list(the_list):
+    """
+    Recursively initializes a nested list by replacing each element with an empty list.
+
+    Parameters:
+        the_list (list): The list to be initialized.
+
+    Returns:
+        list: The initialized list.
+    """
     index = 0
     for i in the_list:
         if hasattr(i, "__len__"):
             the_list[index] = initialize_list(i)
         else:
             the_list[index] = []
         index += 1
     return the_list
 
 
 def place_values_in_list(the_list, location, to_append):
+    """
+    Appends a value to a list at the specified location.
+
+    Parameters:
+        the_list (list): The list to modify.
+        location (int or list): The index or indices specifying the location in the list.
+        to_append (any): The value to append to the list.
+
+    Returns:
+        None
+    """
     testing = the_list
     if hasattr(location, "__len__"):
         for i in range(len(location)):
             testing = testing[location[i]]
         testing.append(to_append)
     else:
         testing = testing[location]
         testing.append(to_append)
 
 
 def get_values_from_list(the_list, location):
+    """
+    Retrieves values from a nested list based on the provided location.
+
+    Parameters:
+        the_list (list): The nested list from which to retrieve values.
+        location (int or list): The index or list of indices specifying the location of the desired values.
+
+    Returns:
+        The value(s) at the specified location in the nested list.
+    """
     testing = the_list
     if hasattr(location, "__len__"):
         for i in range(len(location)):
             testing = testing[location[i]]
         return testing
     else:
         testing = testing[location]
         return testing
 
 
 def orbit_time(begin_orbit, end_orbit=None):
-    orb_file = os.path.join(os.path.dirname(__file__),
-                            'maven_orb_rec.orb')
+    """
+    Calculate the time range corresponding to the given orbit number(s).
+
+    Parameters:
+        begin_orbit (int): The starting orbit number.
+        end_orbit (int, optional): The ending orbit number. If not provided, the time range for the single orbit specified by `begin_orbit` will be returned.
+
+    Returns:
+        list: A list containing the begin and end times of the specified orbit range. If the orbit numbers are not found, the list will contain `None` values.
+
+    """
+    orb_file = os.path.join(os.path.dirname(__file__), "maven_orb_rec.orb")
 
     with open(orb_file, "r") as f:
         if end_orbit is None:
             end_orbit = begin_orbit
         orbit_num = []
         time = []
         f.readline()
         f.readline()
         for line in f:
             line = line[0:28]
-            line = line.split(' ')
-            line = [x for x in line if x != '']
+            line = line.split(" ")
+            line = [x for x in line if x != ""]
             orbit_num.append(int(line[0]))
-            time.append(line[1] + "-" + month_to_num(line[2]) + "-" + line[3] + "T" + line[4])
+            time.append(
+                line[1] + "-" + month_to_num(line[2]) + "-" + line[3] + "T" + line[4]
+            )
         try:
-            if orbit_num.index(begin_orbit) > len(time) or orbit_num.index(end_orbit) + 1 > len(time):
-                print("Orbit numbers not found.  Please choose a number between 1 and %s.", orbit_num[-1])
+            if orbit_num.index(begin_orbit) > len(time) or orbit_num.index(
+                end_orbit
+            ) + 1 > len(time):
+                logging.warning(
+                    "Orbit numbers not found.  Please choose a number between 1 and %s.",
+                    orbit_num[-1],
+                )
                 return [None, None]
             else:
                 begin_time = time[orbit_num.index(begin_orbit)]
                 end_time = time[orbit_num.index(end_orbit) + 1]
         except ValueError:
             return [None, None]
     return [begin_time, end_time]
 
 
 def month_to_num(month_string):
-    if month_string == 'JAN':
-        return '01'
-    if month_string == 'FEB':
-        return '02'
-    if month_string == 'MAR':
-        return '03'
-    if month_string == 'APR':
-        return '04'
-    if month_string == 'MAY':
-        return '05'
-    if month_string == 'JUN':
-        return '06'
-    if month_string == 'JUL':
-        return '07'
-    if month_string == 'AUG':
-        return '08'
-    if month_string == 'SEP':
-        return '09'
-    if month_string == 'OCT':
-        return '10'
-    if month_string == 'NOV':
-        return '11'
-    if month_string == 'DEC':
-        return '12'
+    """
+    Converts a three-letter month abbreviation to its corresponding two-digit number representation.
+
+    Args:
+        month_string (str): The three-letter month abbreviation (e.g., "JAN", "FEB", etc.).
 
+    Returns:
+        str: The two-digit number representation of the month (e.g., "01", "02", etc.).
+    """
+    if month_string == "JAN":
+        return "01"
+    if month_string == "FEB":
+        return "02"
+    if month_string == "MAR":
+        return "03"
+    if month_string == "APR":
+        return "04"
+    if month_string == "MAY":
+        return "05"
+    if month_string == "JUN":
+        return "06"
+    if month_string == "JUL":
+        return "07"
+    if month_string == "AUG":
+        return "08"
+    if month_string == "SEP":
+        return "09"
+    if month_string == "OCT":
+        return "10"
+    if month_string == "NOV":
+        return "11"
+    if month_string == "DEC":
+        return "12"
+
+
+def mvn_kp_sc_traj_xyz(
+    dims_x, dims_y, dims_z, values, x_array, y_array, z_array, nn="linear"
+):
+    """
+    Interpolates the values of a 3D array at given coordinates using trilinear interpolation.
+
+    Parameters:
+        dims_x (array-like): The x-coordinates of the grid points.
+        dims_y (array-like): The y-coordinates of the grid points.
+        dims_z (array-like): The z-coordinates of the grid points.
+        values (ndarray): The 3D array of values to be interpolated.
+        x_array (array-like): The x-coordinates of the points to interpolate.
+        y_array (array-like): The y-coordinates of the points to interpolate.
+        z_array (array-like): The z-coordinates of the points to interpolate.
+        nn (str, optional): The type of nearest neighbor interpolation to use.
+            Defaults to "linear".
+
+    Returns:
+        list: The interpolated values at the given coordinates.
+    """
 
-def mvn_kp_sc_traj_xyz(dims_x, dims_y, dims_z, values, x_array, y_array, z_array, nn='linear'):
     data = []
-    if nn == 'nearest':
+    if nn == "nearest":
         for x, y, z in np.array([a for a in zip(x_array, y_array, z_array)]):
             ix = np.abs(dims_x - x).argmin()
             iy = np.abs(dims_y - y).argmin()
             iz = np.abs(dims_z - z).argmin()
             data.append(values[ix, iy, iz])
     else:
         max_x = np.max(x_array)
@@ -845,862 +1013,989 @@
                 iz2 = iz1
                 iz1 = temp
 
             nx = (x - ix1) / (ix2 - ix1)
             ny = (y - iy1) / (iy2 - iy1)
             nz = (z - iz1) / (iz2 - iz1)
 
-            data.append(values[sorted_x_distance[0], sorted_y_distance[0], sorted_z_distance[0]]
-                        * (1 - nx) * (1 - ny) * (1 - nz) +
-                        values[sorted_x_distance[1], sorted_y_distance[0], sorted_z_distance[0]]
-                        * nx * (1 - ny) * (1 - nz) +
-                        values[sorted_x_distance[0], sorted_y_distance[1], sorted_z_distance[0]]
-                        * (1 - nx) * ny * (1 - nz) +
-                        values[sorted_x_distance[0], sorted_y_distance[0], sorted_z_distance[1]]
-                        * (1 - nx) * (1 - ny) * nz +
-                        values[sorted_x_distance[1], sorted_y_distance[0], sorted_z_distance[1]]
-                        * nx * (1 - ny) * nz +
-                        values[sorted_x_distance[0], sorted_y_distance[1], sorted_z_distance[1]]
-                        * (1 - nx) * ny * nz +
-                        values[sorted_x_distance[1], sorted_y_distance[1], sorted_z_distance[0]]
-                        * nx * ny * (1 - nz) +
-                        values[sorted_x_distance[1], sorted_y_distance[1], sorted_z_distance[1]]
-                        * nx * ny * nz)
+            data.append(
+                values[sorted_x_distance[0], sorted_y_distance[0], sorted_z_distance[0]]
+                * (1 - nx)
+                * (1 - ny)
+                * (1 - nz)
+                + values[
+                    sorted_x_distance[1], sorted_y_distance[0], sorted_z_distance[0]
+                ]
+                * nx
+                * (1 - ny)
+                * (1 - nz)
+                + values[
+                    sorted_x_distance[0], sorted_y_distance[1], sorted_z_distance[0]
+                ]
+                * (1 - nx)
+                * ny
+                * (1 - nz)
+                + values[
+                    sorted_x_distance[0], sorted_y_distance[0], sorted_z_distance[1]
+                ]
+                * (1 - nx)
+                * (1 - ny)
+                * nz
+                + values[
+                    sorted_x_distance[1], sorted_y_distance[0], sorted_z_distance[1]
+                ]
+                * nx
+                * (1 - ny)
+                * nz
+                + values[
+                    sorted_x_distance[0], sorted_y_distance[1], sorted_z_distance[1]
+                ]
+                * (1 - nx)
+                * ny
+                * nz
+                + values[
+                    sorted_x_distance[1], sorted_y_distance[1], sorted_z_distance[0]
+                ]
+                * nx
+                * ny
+                * (1 - nz)
+                + values[
+                    sorted_x_distance[1], sorted_y_distance[1], sorted_z_distance[1]
+                ]
+                * nx
+                * ny
+                * nz
+            )
     return data
 
 
 def read_iuvs_file(file):
+    """
+    Read an IUVS file and return a dictionary containing the data.
+
+    Parameters:
+        file (str): The path to the IUVS file to be read.
+
+    Returns:
+        dict: A dictionary containing the data read from the IUVS file.
+    """
     iuvs_dict = {}
     periapse_num = 0
     occ_num = 0
     with open(file) as f:
         line = f.readline()
-        while line != '':
-            if line.startswith('*'):
+        while line != "":
+            if line.startswith("*"):
                 # Read the header
                 line = f.readline()
-                obs_mode = line[19:len(line) - 1].strip()
+                obs_mode = line[19 : len(line) - 1].strip()
 
                 header = {}
                 f.readline()
                 line = f.readline()
-                header['time_start'] = line[19:len(line) - 1].strip()
+                header["time_start"] = line[19 : len(line) - 1].strip()
                 line = f.readline()
-                header['time_stop'] = line[19:len(line) - 1].strip()
+                header["time_stop"] = line[19 : len(line) - 1].strip()
                 line = f.readline()
                 if obs_mode == "OCCULTATION":
-                    header['target_name'] = line[19:len(line) - 1].strip()
+                    header["target_name"] = line[19 : len(line) - 1].strip()
                     line = f.readline()
-                header['sza'] = float(line[19:len(line) - 1].strip())
+                header["sza"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['local_time'] = float(line[19:len(line) - 1].strip())
+                header["local_time"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['lat'] = float(line[19:len(line) - 1].strip())
+                header["lat"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['lon'] = float(line[19:len(line) - 1].strip())
+                header["lon"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['lat_mso'] = float(line[19:len(line) - 1].strip())
+                header["lat_mso"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['lon_mso'] = float(line[19:len(line) - 1].strip())
+                header["lon_mso"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['orbit_number'] = int(line[19:len(line) - 1].strip())
+                header["orbit_number"] = int(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['mars_season'] = float(line[19:len(line) - 1].strip())
+                header["mars_season"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_geo_x'] = float(line[19:len(line) - 1].strip())
+                header["sc_geo_x"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_geo_y'] = float(line[19:len(line) - 1].strip())
+                header["sc_geo_y"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_geo_z'] = float(line[19:len(line) - 1].strip())
+                header["sc_geo_z"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_mso_x'] = float(line[19:len(line) - 1].strip())
+                header["sc_mso_x"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_mso_y'] = float(line[19:len(line) - 1].strip())
+                header["sc_mso_y"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_mso_z'] = float(line[19:len(line) - 1].strip())
+                header["sc_mso_z"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_geo_x'] = float(line[19:len(line) - 1].strip())
+                header["sun_geo_x"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_geo_y'] = float(line[19:len(line) - 1].strip())
+                header["sun_geo_y"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_geo_z'] = float(line[19:len(line) - 1].strip())
+                header["sun_geo_z"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_geo_lat'] = float(line[19:len(line) - 1].strip())
+                header["sun_geo_lat"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_geo_lon'] = float(line[19:len(line) - 1].strip())
+                header["sun_geo_lon"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_mso_lat'] = float(line[19:len(line) - 1].strip())
+                header["sun_mso_lat"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sun_mso_lon'] = float(line[19:len(line) - 1].strip())
+                header["sun_mso_lon"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['subsol_geo_lon'] = float(line[19:len(line) - 1].strip())
+                header["subsol_geo_lon"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['subsol_geo_lat'] = float(line[19:len(line) - 1].strip())
+                header["subsol_geo_lat"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_sza'] = float(line[19:len(line) - 1].strip())
+                header["sc_sza"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_local_time'] = float(line[19:len(line) - 1].strip())
+                header["sc_local_time"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['sc_alt'] = float(line[19:len(line) - 1].strip())
+                header["sc_alt"] = float(line[19 : len(line) - 1].strip())
                 line = f.readline()
-                header['mars_sun_dist'] = float(line[19:len(line) - 1].strip())
+                header["mars_sun_dist"] = float(line[19 : len(line) - 1].strip())
 
                 if obs_mode == "PERIAPSE":
                     periapse_num += 1
                     line = f.readline()
-                    n_alt_bins = int(line[19:len(line) - 1].strip())
-                    header['n_alt_bins'] = float(n_alt_bins)
+                    n_alt_bins = int(line[19 : len(line) - 1].strip())
+                    header["n_alt_bins"] = float(n_alt_bins)
                     line = f.readline()
-                    n_alt_den_bins = int(line[19:len(line) - 1].strip())
-                    header['n_alt_den_bins'] = float(n_alt_den_bins)
+                    n_alt_den_bins = int(line[19 : len(line) - 1].strip())
+                    header["n_alt_den_bins"] = float(n_alt_den_bins)
 
-                    iuvs_dict['periapse' + str(periapse_num)] = {}
-                    iuvs_dict['periapse' + str(periapse_num)].update(header)
+                    iuvs_dict["periapse" + str(periapse_num)] = {}
+                    iuvs_dict["periapse" + str(periapse_num)].update(header)
 
                     # Empty space
                     f.readline()
 
                     # Read the Temperature
                     line = f.readline()
-                    temp_labels = line[19:len(line) - 1].strip().split()
+                    temp_labels = line[19 : len(line) - 1].strip().split()
                     temperature = collections.OrderedDict((x, []) for x in temp_labels)
-                    temperature_unc = collections.OrderedDict((x, []) for x in temp_labels)
+                    temperature_unc = collections.OrderedDict(
+                        (x, []) for x in temp_labels
+                    )
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         temperature[list(temperature.keys())[index]].append(val)
                         index += 1
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         temperature_unc[list(temperature_unc.keys())[index]].append(val)
                         index += 1
-                    iuvs_dict['periapse' + str(periapse_num)]['temperature'] = temperature
-                    iuvs_dict['periapse' + str(periapse_num)]['temperature_unc'] = temperature_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "temperature"
+                    ] = temperature
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "temperature_unc"
+                    ] = temperature_unc
 
                     # Empty space
                     f.readline()
 
                     # Read the Scale Heights
                     line = f.readline()
-                    scale_height_labels = line[19:len(line) - 1].strip().split()
-                    scale_height = collections.OrderedDict((x, []) for x in scale_height_labels)
-                    scale_height_unc = collections.OrderedDict((x, []) for x in scale_height_labels)
+                    scale_height_labels = line[19 : len(line) - 1].strip().split()
+                    scale_height = collections.OrderedDict(
+                        (x, []) for x in scale_height_labels
+                    )
+                    scale_height_unc = collections.OrderedDict(
+                        (x, []) for x in scale_height_labels
+                    )
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         scale_height[list(scale_height.keys())[index]].append(val)
                         index += 1
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
-                        scale_height_unc[list(scale_height_unc.keys())[index]].append(val)
+                        scale_height_unc[list(scale_height_unc.keys())[index]].append(
+                            val
+                        )
                         index += 1
 
-                    iuvs_dict['periapse' + str(periapse_num)]['scale_height'] = scale_height
-                    iuvs_dict['periapse' + str(periapse_num)]['scale_height_unc'] = scale_height_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "scale_height"
+                    ] = scale_height
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "scale_height_unc"
+                    ] = scale_height_unc
 
                     # Empty space
                     f.readline()
                     f.readline()
 
                     # Read in the density
                     line = f.readline()
                     density_labels = line.strip().split()
                     density = collections.OrderedDict((x, []) for x in density_labels)
                     for i in range(0, n_alt_den_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             density[list(density.keys())[index]].append(val)
                             index += 1
-                    iuvs_dict['periapse' + str(periapse_num)]['density'] = density
+                    iuvs_dict["periapse" + str(periapse_num)]["density"] = density
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the density systematic uncertainty
-                    density_sys_unc = collections.OrderedDict((x, []) for x in density_labels)
+                    density_sys_unc = collections.OrderedDict(
+                        (x, []) for x in density_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         density_sys_unc[list(density.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['periapse' + str(periapse_num)]['density_sys_unc'] = density_sys_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "density_sys_unc"
+                    ] = density_sys_unc
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the density uncertainty
-                    density_unc = collections.OrderedDict((x, []) for x in density_labels)
+                    density_unc = collections.OrderedDict(
+                        (x, []) for x in density_labels
+                    )
                     for i in range(0, n_alt_den_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             density_unc[list(density.keys())[index]].append(val)
                             index += 1
-                    iuvs_dict['periapse' + str(periapse_num)]['density_sys_unc'] = density_sys_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "density_sys_unc"
+                    ] = density_sys_unc
 
                     f.readline()
                     f.readline()
 
                     line = f.readline()
                     radiance_labels = line.strip().split()
                     if "Cameron" in radiance_labels:
-                        radiance_labels.remove('Cameron')
+                        radiance_labels.remove("Cameron")
                     radiance = collections.OrderedDict((x, []) for x in radiance_labels)
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             radiance[list(radiance.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['periapse' + str(periapse_num)]['radiance'] = radiance
+                    iuvs_dict["periapse" + str(periapse_num)]["radiance"] = radiance
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the radiance systematic uncertainty
-                    radiance_sys_unc = collections.OrderedDict((x, []) for x in radiance_labels)
+                    radiance_sys_unc = collections.OrderedDict(
+                        (x, []) for x in radiance_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         radiance_sys_unc[list(radiance.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['periapse' + str(periapse_num)]['radiance_sys_unc'] = radiance_sys_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "radiance_sys_unc"
+                    ] = radiance_sys_unc
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the radiance uncertainty
-                    radiance_unc = collections.OrderedDict((x, []) for x in radiance_labels)
+                    radiance_unc = collections.OrderedDict(
+                        (x, []) for x in radiance_labels
+                    )
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             radiance_unc[list(radiance.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['periapse' + str(periapse_num)]['radiance_unc'] = radiance_unc
+                    iuvs_dict["periapse" + str(periapse_num)][
+                        "radiance_unc"
+                    ] = radiance_unc
 
                 elif obs_mode == "OCCULTATION":
                     occ_num += 1
                     line = f.readline()
-                    n_alt_den_bins = int(line[19:len(line) - 1].strip())
-                    header['n_alt_den_bins'] = float(n_alt_den_bins)
+                    n_alt_den_bins = int(line[19 : len(line) - 1].strip())
+                    header["n_alt_den_bins"] = float(n_alt_den_bins)
 
-                    iuvs_dict['occultation' + str(occ_num)] = {}
-                    iuvs_dict['occultation' + str(occ_num)].update(header)
+                    iuvs_dict["occultation" + str(occ_num)] = {}
+                    iuvs_dict["occultation" + str(occ_num)].update(header)
 
                     # Empty space
                     f.readline()
 
                     # Read the Scale Heights
                     line = f.readline()
-                    scale_height_labels = line[19:len(line) - 1].strip().split()
-                    scale_height = collections.OrderedDict((x, []) for x in scale_height_labels)
-                    scale_height_unc = collections.OrderedDict((x, []) for x in scale_height_labels)
+                    scale_height_labels = line[19 : len(line) - 1].strip().split()
+                    scale_height = collections.OrderedDict(
+                        (x, []) for x in scale_height_labels
+                    )
+                    scale_height_unc = collections.OrderedDict(
+                        (x, []) for x in scale_height_labels
+                    )
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         scale_height[list(scale_height.keys())[index]].append(val)
                         index += 1
                     line = f.readline()
-                    vals = line[20:len(line) - 1].strip().split()
+                    vals = line[20 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
-                        scale_height_unc[list(scale_height_unc.keys())[index]].append(val)
+                        scale_height_unc[list(scale_height_unc.keys())[index]].append(
+                            val
+                        )
                         index += 1
 
-                    iuvs_dict['occultation' + str(occ_num)]['scale_height'] = scale_height
-                    iuvs_dict['occultation' + str(occ_num)]['scale_height_unc'] = scale_height_unc
+                    iuvs_dict["occultation" + str(occ_num)][
+                        "scale_height"
+                    ] = scale_height
+                    iuvs_dict["occultation" + str(occ_num)][
+                        "scale_height_unc"
+                    ] = scale_height_unc
 
                     # Empty space
                     f.readline()
                     f.readline()
 
                     # Read in the retrieval
                     line = f.readline()
                     retrieval_labels = line.strip().split()
-                    retrieval = collections.OrderedDict((x, []) for x in retrieval_labels)
+                    retrieval = collections.OrderedDict(
+                        (x, []) for x in retrieval_labels
+                    )
                     for i in range(0, n_alt_den_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             retrieval[list(retrieval.keys())[index]].append(val)
                             index += 1
-                    iuvs_dict['occultation' + str(occ_num)]['retrieval'] = retrieval
+                    iuvs_dict["occultation" + str(occ_num)]["retrieval"] = retrieval
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the retrieval systematic uncertainty
-                    retrieval_sys_unc = collections.OrderedDict((x, []) for x in retrieval_labels)
+                    retrieval_sys_unc = collections.OrderedDict(
+                        (x, []) for x in retrieval_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         retrieval_sys_unc[list(retrieval.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['occultation' + str(occ_num)]['retrieval_sys_unc'] = retrieval_sys_unc
+                    iuvs_dict["occultation" + str(occ_num)][
+                        "retrieval_sys_unc"
+                    ] = retrieval_sys_unc
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the retrieval uncertainty
-                    retrieval_unc = collections.OrderedDict((x, []) for x in retrieval_labels)
+                    retrieval_unc = collections.OrderedDict(
+                        (x, []) for x in retrieval_labels
+                    )
                     for i in range(0, n_alt_den_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             retrieval_unc[list(retrieval.keys())[index]].append(val)
                             index += 1
-                    iuvs_dict['occultation' + str(occ_num)]['retrieval_sys_unc'] = retrieval_sys_unc
+                    iuvs_dict["occultation" + str(occ_num)][
+                        "retrieval_sys_unc"
+                    ] = retrieval_sys_unc
 
                 elif obs_mode == "CORONA_LORES_HIGH":
                     line = f.readline()
-                    n_alt_bins = int(line[19:len(line) - 1].strip())
-                    header['n_alt_bins'] = float(n_alt_bins)
+                    n_alt_bins = int(line[19 : len(line) - 1].strip())
+                    header["n_alt_bins"] = float(n_alt_bins)
 
-                    iuvs_dict['corona_lores_high'] = {}
-                    iuvs_dict['corona_lores_high'].update(header)
+                    iuvs_dict["corona_lores_high"] = {}
+                    iuvs_dict["corona_lores_high"].update(header)
 
                     f.readline()
 
                     # Read the Half int
                     line = f.readline()
-                    half_int_dist_labels = line[19:len(line) - 1].strip().split()
-                    half_int_dist = collections.OrderedDict((x, []) for x in half_int_dist_labels)
-                    half_int_dist_unc = collections.OrderedDict((x, []) for x in half_int_dist_labels)
+                    half_int_dist_labels = line[19 : len(line) - 1].strip().split()
+                    half_int_dist = collections.OrderedDict(
+                        (x, []) for x in half_int_dist_labels
+                    )
+                    half_int_dist_unc = collections.OrderedDict(
+                        (x, []) for x in half_int_dist_labels
+                    )
                     line = f.readline()
-                    vals = line[26:len(line) - 1].strip().split()
+                    vals = line[26 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         half_int_dist[list(half_int_dist.keys())[index]].append(val)
                         index += 1
                     line = f.readline()
-                    vals = line[26:len(line) - 1].strip().split()
+                    vals = line[26 : len(line) - 1].strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
-                        half_int_dist_unc[list(half_int_dist_unc.keys())[index]].append(val)
+                        half_int_dist_unc[list(half_int_dist_unc.keys())[index]].append(
+                            val
+                        )
                         index += 1
 
-                    iuvs_dict['corona_lores_high']['half_int_dist'] = half_int_dist
-                    iuvs_dict['corona_lores_high']['half_int_dist_unc'] = half_int_dist_unc
+                    iuvs_dict["corona_lores_high"]["half_int_dist"] = half_int_dist
+                    iuvs_dict["corona_lores_high"][
+                        "half_int_dist_unc"
+                    ] = half_int_dist_unc
 
                     # Blank space
                     f.readline()
                     f.readline()
 
                     # Read in the density
                     line = f.readline()
                     density_labels = line.strip().split()
                     density = collections.OrderedDict((x, []) for x in density_labels)
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             density[list(density.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['corona_lores_high']['density'] = density
+                    iuvs_dict["corona_lores_high"]["density"] = density
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the density systematic uncertainty
-                    density_sys_unc = collections.OrderedDict((x, []) for x in density_labels)
+                    density_sys_unc = collections.OrderedDict(
+                        (x, []) for x in density_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         density_sys_unc[list(density.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['corona_lores_high']['density_sys_unc'] = density_sys_unc
+                    iuvs_dict["corona_lores_high"]["density_sys_unc"] = density_sys_unc
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the density uncertainty
-                    density_unc = collections.OrderedDict((x, []) for x in density_labels)
+                    density_unc = collections.OrderedDict(
+                        (x, []) for x in density_labels
+                    )
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             density_unc[list(density.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['corona_lores_high']['density_unc'] = density_unc
+                    iuvs_dict["corona_lores_high"]["density_unc"] = density_unc
 
                     f.readline()
                     f.readline()
 
                     line = f.readline()
                     radiance_labels = line.strip().split()
                     if "Cameron" in radiance_labels:
-                        radiance_labels.remove('Cameron')
+                        radiance_labels.remove("Cameron")
                     radiance = collections.OrderedDict((x, []) for x in radiance_labels)
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             radiance[list(radiance.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['corona_lores_high']['radiance'] = radiance
+                    iuvs_dict["corona_lores_high"]["radiance"] = radiance
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the radiance systematic uncertainty
-                    radiance_sys_unc = collections.OrderedDict((x, []) for x in radiance_labels)
+                    radiance_sys_unc = collections.OrderedDict(
+                        (x, []) for x in radiance_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         radiance_sys_unc[list(radiance.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['corona_lores_high']['radiance_sys_unc'] = radiance_sys_unc
+                    iuvs_dict["corona_lores_high"][
+                        "radiance_sys_unc"
+                    ] = radiance_sys_unc
 
                     # Not needed lines
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the radiance uncertainty
-                    radiance_unc = collections.OrderedDict((x, []) for x in radiance_labels)
+                    radiance_unc = collections.OrderedDict(
+                        (x, []) for x in radiance_labels
+                    )
                     for i in range(0, n_alt_bins):
                         line = f.readline()
                         vals = line.strip().split()
                         index = 0
                         for val in vals:
-                            if val == '-9.9999990E+09':
-                                val = float('nan')
+                            if val == "-9.9999990E+09":
+                                val = float("nan")
                             else:
                                 val = float(val)
                             radiance_unc[list(radiance.keys())[index]].append(val)
                             index += 1
 
-                    iuvs_dict['corona_lores_high']['radiance_unc'] = radiance_unc
+                    iuvs_dict["corona_lores_high"]["radiance_unc"] = radiance_unc
 
-                elif obs_mode == 'APOAPSE':
+                elif obs_mode == "APOAPSE":
 
                     f.readline()
                     maps = {}
                     for j in range(0, 17):
                         var = f.readline().strip()
                         line = f.readline()
                         lons = line.strip().split()
                         lons = [float(x) for x in lons]
                         lats = []
                         data = []
                         for k in range(0, 45):
                             line = f.readline().strip().split()
                             lats.append(float(line[0]))
                             line_data = line[1:]
-                            line_data = [float(x) if x != '-9.9999990E+09' else float('nan') for x in line_data]
+                            line_data = [
+                                float(x) if x != "-9.9999990E+09" else float("nan")
+                                for x in line_data
+                            ]
                             data.append(line_data)
 
                         maps[var] = data
                         f.readline()
 
-                    maps['latitude'] = lats
-                    maps['longitude'] = lons
+                    maps["latitude"] = lats
+                    maps["longitude"] = lons
 
-                    iuvs_dict['apoapse'] = {}
-                    iuvs_dict['apoapse'].update(header)
-                    iuvs_dict['apoapse'].update(maps)
+                    iuvs_dict["apoapse"] = {}
+                    iuvs_dict["apoapse"].update(header)
+                    iuvs_dict["apoapse"].update(maps)
 
                     f.readline()
                     f.readline()
                     f.readline()
 
                     # Read in the radiance systematic uncertainty
                     line = f.readline()
                     radiance_labels = line.strip().split()
-                    radiance_sys_unc = collections.OrderedDict((x, []) for x in radiance_labels)
+                    radiance_sys_unc = collections.OrderedDict(
+                        (x, []) for x in radiance_labels
+                    )
                     line = f.readline()
                     vals = line.strip().split()
                     index = 0
                     for val in vals:
-                        if val == '-9.9999990E+09':
-                            val = float('nan')
+                        if val == "-9.9999990E+09":
+                            val = float("nan")
                         else:
                             val = float(val)
                         radiance_sys_unc[list(radiance.keys())[index + 1]].append(val)
                         index += 1
 
-                    iuvs_dict['apoapse']['radiance_sys_unc'] = radiance_sys_unc
+                    iuvs_dict["apoapse"]["radiance_sys_unc"] = radiance_sys_unc
 
             line = f.readline()
 
     return iuvs_dict
 
 
-param_dict = {'Electron Density': 'ELECTRON_DENSITY',
-              'Electron Density Quality Min': 'ELECTRON_DENSITY_QUAL_MIN',
-              'Electron Density Quality Max': 'ELECTRON_DENSITY_QUAL_MAX',
-              'Electron Temperature': 'ELECTRON_TEMPERATURE',
-              'Electron Temperature Quality Min': 'ELECTRON_TEMPERATURE_QUAL_MIN',
-              'Electron Temperature Quality Max': 'ELECTRON_TEMPERATURE_QUAL_MAX',
-              'Spacecraft Potential': 'SPACECRAFT_POTENTIAL',
-              'Spacecraft Potential Quality Min': 'SPACECRAFT_POTENTIAL_QUAL_MIN',
-              'Spacecraft Potential Quality Max': 'SPACECRAFT_POTENTIAL_QUAL_MAX',
-              'E-field Power 2-100 Hz': 'EWAVE_LOW_FREQ',
-              'E-field 2-100 Hz Quality': 'EWAVE_LOW_FREQ_QUAL_QUAL',
-              'E-field Power 100-800 Hz': 'EWAVE_MID_FREQ',
-              'E-field 100-800 Hz Quality': 'EWAVE_MID_FREQ_QUAL_QUAL',
-              'E-field Power 0.8-1.0 Mhz': 'EWAVE_HIGH_FREQ',
-              'E-field 0.8-1.0 Mhz Quality': 'EWAVE_HIGH_FREQ_QUAL_QUAL',
-              'EUV Irradiance 0.1-7.0 nm': 'IRRADIANCE_LOW',
-              'Irradiance 0.1-7.0 nm Quality': 'IRRADIANCE_LOW_QUAL',
-              'EUV Irradiance 17-22 nm': 'IRRADIANCE_MID',
-              'Irradiance 17-22 nm Quality': 'IRRADIANCE_MID_QUAL',
-              'EUV Irradiance Lyman-alpha': 'IRRADIANCE_LYMAN',
-              'Irradiance Lyman-alpha Quality': 'IRRADIANCE_LYMAN_QUAL',
-              'Solar Wind Electron Density': 'SOLAR_WIND_ELECTRON_DENSITY',
-              'Solar Wind E- Density Quality': 'SOLAR_WIND_ELECTRON_DENSITY_QUAL',
-              'Solar Wind Electron Temperature': 'SOLAR_WIND_ELECTRON_TEMPERATURE',
-              'Solar Wind E- Temperature Quality': 'SOLAR_WIND_ELECTRON_TEMPERATURE_QUAL',
-              'Flux, e- Parallel (5-100 ev)': 'ELECTRON_PARALLEL_FLUX_LOW',
-              'Flux, e- Parallel (5-100 ev) Quality': 'ELECTRON_PARALLEL_FLUX_LOW_QUAL',
-              'Flux, e- Parallel (100-500 ev)': 'ELECTRON_PARALLEL_FLUX_MID',
-              'Flux, e- Parallel (100-500 ev) Quality': 'ELECTRON_PARALLEL_FLUX_MID_QUAL',
-              'Flux, e- Parallel (500-1000 ev)': 'ELECTRON_PARALLEL_FLUX_HIGH',
-              'Flux, e- Parallel (500-1000 ev) Quality': 'ELECTRON_PARALLEL_FLUX_HIGH_QUAL',
-              'Flux, e- Anti-par (5-100 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_LOW',
-              'Flux, e- Anti-par (5-100 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_LOW_QUAL',
-              'Flux, e- Anti-par (100-500 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_MID',
-              'Flux, e- Anti-par (100-500 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_MID_QUAL',
-              'Flux, e- Anti-par (500-1000 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_HIGH',
-              'Flux, e- Anti-par (500-1000 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_HIGH_QUAL',
-              'Electron eflux Parallel (5-100 ev)': 'ELECTRON_PARALLEL_FLUX_LOW',
-              'Electron eflux Parallel (5-100 ev) Quality': 'ELECTRON_PARALLEL_FLUX_LOW_QUAL',
-              'Electron eflux Parallel (100-500 ev)': 'ELECTRON_PARALLEL_FLUX_MID',
-              'Electron eflux Parallel (100-500 ev) Quality': 'ELECTRON_PARALLEL_FLUX_MID_QUAL',
-              'Electron eflux Parallel (500-1000 ev)': 'ELECTRON_PARALLEL_FLUX_HIGH',
-              'Electron eflux Parallel (500-1000 ev) Quality': 'ELECTRON_PARALLEL_FLUX_HIGH_QUAL',
-              'Electron eflux Anti-par (5-100 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_LOW',
-              'Electron eflux Anti-par (5-100 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_LOW_QUAL',
-              'Electron eflux Anti-par (100-500 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_MID',
-              'Electron eflux Anti-par (100-500 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_MID_QUAL',
-              'Electron eflux Anti-par (500-1000 ev)': 'ELECTRON_ANTI_PARALLEL_FLUX_HIGH',
-              'Electron eflux Anti-par (500-1000 ev) Quality': 'ELECTRON_ANTI_PARALLEL_FLUX_HIGH_QUAL',
-              'Electron Spectrum Shape': 'ELECTRON_SPECTRUM_SHAPE_PARAMETER',
-              'Spectrum Shape Quality': 'ELECTRON_SPECTRUM_SHAPE_PARAMETER_QUAL',
-              'H+ Density': 'HPLUS_DENSITY',
-              'H+ Density Quality': 'HPLUS_DENSITY_QUAL',
-              'H+ Flow Velocity MSO X': 'HPLUS_FLOW_VELOCITY_MSO_X',
-              'H+ Flow MSO X Quality': 'HPLUS_FLOW_VELOCITY_MSO_X_QUAL',
-              'H+ Flow Velocity MSO Y': 'HPLUS_FLOW_VELOCITY_MSO_Y',
-              'H+ Flow MSO Y Quality': 'HPLUS_FLOW_VELOCITY_MSO_Y_QUAL',
-              'H+ Flow Velocity MSO Z': 'HPLUS_FLOW_VELOCITY_MSO_Z',
-              'H+ Flow MSO Z Quality': 'HPLUS_FLOW_VELOCITY_MSO_Z_QUAL',
-              'H+ Temperature': 'HPLUS_TEMPERATURE',
-              'H+ Temperature Quality': 'HPLUS_TEMPERATURE_QUAL',
-              'Solar Wind Dynamic Pressure': 'SOLAR_WIND_DYNAMIC_PRESSURE',
-              'Solar Wind Pressure Quality': 'SOLAR_WIND_DYNAMIC_PRESSURE_QUAL',
-              'STATIC Quality Flag': 'STATIC_QUALITY_FLAG',
-              'O+ Density': 'OPLUS_DENSITY',
-              'O+ Density Quality': 'OPLUS_DENSITY_QUAL',
-              'O2+ Density': 'O2PLUS_DENSITY',
-              'O2+ Density Quality': 'O2PLUS_DENSITY_QUAL',
-              'O+ Temperature': 'OPLUS_TEMPERATURE',
-              'O+ Temperature Quality': 'OPLUS_TEMPERATURE_QUAL',
-              'O2+ Temperature': 'O2PLUS_TEMPERATURE',
-              'O2+ Temperature Quality': 'O2PLUS_TEMPERATURE_QUAL',
-              'O2+ Flow Velocity MAVEN_APP X': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_X',
-              'O2+ Flow MAVEN_APP X Quality': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_X_QUAL',
-              'O2+ Flow Velocity MAVEN_APP Y': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_Y',
-              'O2+ Flow MAVEN_APP Y Quality': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_Y_QUAL',
-              'O2+ Flow Velocity MAVEN_APP Z': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_Z',
-              'O2+ Flow MAVEN_APP Z Quality': 'O2PLUS_FLOW_VELOCITY_MAVEN_APP_Z_QUAL',
-              'O2+ Flow Velocity MSO X': 'O2PLUS_FLOW_VELOCITY_MSO_X',
-              'O2+ Flow MSO X Quality': 'O2PLUS_FLOW_VELOCITY_MSO_X_QUAL',
-              'O2+ Flow Velocity MSO Y': 'O2PLUS_FLOW_VELOCITY_MSO_Y',
-              'O2+ Flow MSO Y Quality': 'O2PLUS_FLOW_VELOCITY_MSO_Y_QUAL',
-              'O2+ Flow Velocity MSO Z': 'O2PLUS_FLOW_VELOCITY_MSO_Z',
-              'O2+ Flow MSO Z Quality': 'O2PLUS_FLOW_VELOCITY_MSO_Z_QUAL',
-              'H+ Omni Flux': 'HPLUS_OMNI_DIRECTIONAL_FLUX',
-              'H+ Energy': 'HPLUS_CHARACTERISTIC_ENERGY',
-              'H+ Energy Quality': 'HPLUS_CHARACTERISTIC_ENERGY_QUAL',
-              'He++ Omni Flux': 'HEPLUS_OMNI_DIRECTIONAL_FLUX',
-              'He++ Energy': 'HEPLUS_CHARACTERISTIC_ENERGY',
-              'He++ Energy Quality': 'HEPLUS_CHARACTERISTIC_ENERGY_QUAL',
-              'O+ Omni Flux': 'OPLUS_OMNI_DIRECTIONAL_FLUX',
-              'O+ Energy': 'OPLUS_CHARACTERISTIC_ENERGY',
-              'O+ Energy Quality': 'OPLUS_CHARACTERISTIC_ENERGY_QUAL',
-              'O2+ Omni Flux': 'O2PLUS_OMNI_DIRECTIONAL_FLUX',
-              'O2+ Energy': 'O2PLUS_CHARACTERISTIC_ENERGY',
-              'O2+ Energy Quality': 'O2PLUS_CHARACTERISTIC_ENERGY_QUAL',
-              'H+ Direction MSO X': 'HPLUS_CHARACTERISTIC_DIRECTION_MSO_X',
-              'H+ Direction MSO Y': 'HPLUS_CHARACTERISTIC_DIRECTION_MSO_Y',
-              'H+ Direction MSO Z': 'HPLUS_CHARACTERISTIC_DIRECTION_MSO_Z',
-              'H+ Angular Width': 'HPLUS_CHARACTERISTIC_ANGULAR_WIDTH',
-              'H+ Width Quality': 'HPLUS_CHARACTERISTIC_ANGULAR_WIDTH_QUAL',
-              'Pickup Ion Direction MSO X': 'DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_X',
-              'Pickup Ion Direction MSO Y': 'DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_Y',
-              'Pickup Ion Direction MSO Z': 'DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_Z',
-              'Pickup Ion Angular Width': 'DOMINANT_PICKUP_ION_CHARACTERISTIC_ANGULAR_WIDTH',
-              'Pickup Ion Width Quality': 'DOMINANT_PICKUP_ION_CHARACTERISTIC_ANGULAR_WIDTH_QUAL',
-              'Ion Flux FOV 1 F': 'ION_ENERGY_FLUX__FOV_1_F',
-              'Ion Flux FOV 1F Quality': 'ION_ENERGY_FLUX__FOV_1_F_QUAL',
-              'Ion Flux FOV 1 R': 'ION_ENERGY_FLUX__FOV_1_R',
-              'Ion Flux FOV 1R Quality': 'ION_ENERGY_FLUX__FOV_1_R_QUAL',
-              'Ion Flux FOV 2 F': 'ION_ENERGY_FLUX__FOV_2_F',
-              'Ion Flux FOV 2F Quality': 'ION_ENERGY_FLUX__FOV_2_F_QUAL',
-              'Ion Flux FOV 2 R': 'ION_ENERGY_FLUX__FOV_2_R',
-              'Ion Flux FOV 2R Quality': 'ION_ENERGY_FLUX__FOV_2_R_QUAL',
-              'Electron Flux FOV 1 F': 'ELECTRON_ENERGY_FLUX___FOV_1_F',
-              'Electron Flux FOV 1F Quality': 'ELECTRON_ENERGY_FLUX___FOV_1_F_QUAL',
-              'Electron Flux FOV 1 R': 'ELECTRON_ENERGY_FLUX___FOV_1_R',
-              'Electron Flux FOV 1R Quality': 'ELECTRON_ENERGY_FLUX___FOV_1_R_QUAL',
-              'Electron Flux FOV 2 F': 'ELECTRON_ENERGY_FLUX___FOV_2_F',
-              'Electron Flux FOV 2F Quality': 'ELECTRON_ENERGY_FLUX___FOV_2_F_QUAL',
-              'Electron Flux FOV 2 R': 'ELECTRON_ENERGY_FLUX___FOV_2_R',
-              'Electron Flux FOV 2R Quality': 'ELECTRON_ENERGY_FLUX___FOV_2_R_QUAL',
-              'Look Direction 1-F MSO X': 'LOOK_DIRECTION_1_F_MSO_X',
-              'Look Direction 1-F MSO Y': 'LOOK_DIRECTION_1_F_MSO_Y',
-              'Look Direction 1-F MSO Z': 'LOOK_DIRECTION_1_F_MSO_Z',
-              'Look Direction 1-R MSO X': 'LOOK_DIRECTION_1_R_MSO_X',
-              'Look Direction 1-R MSO Y': 'LOOK_DIRECTION_1_R_MSO_Y',
-              'Look Direction 1-R MSO Z': 'LOOK_DIRECTION_1_R_MSO_Z',
-              'Look Direction 2-F MSO X': 'LOOK_DIRECTION_2_F_MSO_X',
-              'Look Direction 2-F MSO Y': 'LOOK_DIRECTION_2_F_MSO_Y',
-              'Look Direction 2-F MSO Z': 'LOOK_DIRECTION_2_F_MSO_Z',
-              'Look Direction 2-R MSO X': 'LOOK_DIRECTION_2_R_MSO_X',
-              'Look Direction 2-R MSO Y': 'LOOK_DIRECTION_2_R_MSO_Y',
-              'Look Direction 2-R MSO Z': 'LOOK_DIRECTION_2_R_MSO_Z',
-              'Magnetic Field MSO X': 'MSO_X',
-              'Magnetic MSO X Quality': 'MSO_X_QUAL',
-              'Magnetic Field MSO Y': 'MSO_Y',
-              'Magnetic MSO Y Quality': 'MSO_Y_QUAL',
-              'Magnetic Field MSO Z': 'MSO_Z',
-              'Magnetic MSO Z Quality': 'MSO_Z_QUAL',
-              'Magnetic Field GEO X': 'GEO_X',
-              'Magnetic GEO X Quality': 'GEO_X_QUAL',
-              'Magnetic Field GEO Y': 'GEO_Y',
-              'Magnetic GEO Y Quality': 'GEO_Y_QUAL',
-              'Magnetic Field GEO Z': 'GEO_Z',
-              'Magnetic GEO Z Quality': 'GEO_Z_QUAL',
-              'Magnetic Field RMS Dev': 'RMS_DEVIATION',
-              'Magnetic RMS Quality': 'RMS_DEVIATION_QUAL',
-              'Density He': 'HE_DENSITY',
-              'Density He Precision': 'HE_DENSITY_PRECISION',
-              'Density He Quality': 'HE_DENSITY_QUAL',
-              'Density O': 'O_DENSITY',
-              'Density O Precision': 'O_DENSITY_PRECISION',
-              'Density O Quality': 'O_DENSITY_QUAL',
-              'Density CO': 'CO_DENSITY',
-              'Density CO Precision': 'CO_DENSITY_PRECISION',
-              'Density CO Quality': 'CO_DENSITY_QUAL',
-              'Density N2': 'N2_DENSITY',
-              'Density N2 Precision': 'N2_DENSITY_PRECISION',
-              'Density N2 Quality': 'N2_DENSITY_QUAL',
-              'Density NO': 'NO_DENSITY',
-              'Density NO Precision': 'NO_DENSITY_PRECISION',
-              'Density NO Quality': 'NO_DENSITY_QUAL',
-              'Density Ar': 'AR_DENSITY',
-              'Density Ar Precision': 'AR_DENSITY_PRECISION',
-              'Density Ar Quality': 'AR_DENSITY_QUAL',
-              'Density CO2': 'CO2_DENSITY',
-              'Density CO2 Precision': 'CO2_DENSITY_PRECISION',
-              'Density CO2 Quality': 'CO2_DENSITY_QUAL',
-              'Density 32+': 'O2PLUS_DENSITY',
-              'Density 32+ Precision': 'O2PLUS_DENSITY_PRECISION',
-              'Density 32+ Quality': 'O2PLUS_DENSITY_QUAL',
-              'Density 44+': 'CO2PLUS_DENSITY',
-              'Density 44+ Precision': 'CO2PLUS_DENSITY_PRECISION',
-              'Density 44+ Quality': 'CO2PLUS_DENSITY_QUAL',
-              'Density 30+': 'NOPLUS_DENSITY',
-              'Density 30+ Precision': 'NOPLUS_DENSITY_PRECISION',
-              'Density 30+ Quality': 'NOPLUS_DENSITY_QUAL',
-              'Density 16+': 'OPLUS_DENSITY',
-              'Density 16+ Precision': 'OPLUS_DENSITY_PRECISION',
-              'Density 16+ Quality': 'OPLUS_DENSITY_QUAL',
-              'Density 28+': 'CO2PLUS_N2PLUS_DENSITY',
-              'Density 28+ Precision': 'CO2PLUS_N2PLUS_DENSITY_PRECISION',
-              'Density 28+ Quality': 'CO2PLUS_N2PLUS_DENSITY_QUAL',
-              'Density 12+': 'CPLUS_DENSITY',
-              'Density 12+ Precision': 'CPLUS_DENSITY_PRECISION',
-              'Density 12+ Quality': 'CPLUS_DENSITY_QUAL',
-              'Density 17+': 'OHPLUS_DENSITY',
-              'Density 17+ Precision': 'OHPLUS_DENSITY_PRECISION',
-              'Density 17+ Quality': 'OHPLUS_DENSITY_QUAL',
-              'Density 14+': 'NPLUS_DENSITY',
-              'Density 14+ Precision': 'NPLUS_DENSITY_PRECISION',
-              'Density 14+ Quality': 'NPLUS_DENSITY_QUAL',
-              'APP Attitude GEO X': 'ATTITUDE_GEO_X',
-              'APP Attitude GEO Y': 'ATTITUDE_GEO_Y',
-              'APP Attitude GEO Z': 'ATTITUDE_GEO_Z',
-              'APP Attitude MSO X': 'ATTITUDE_MSO_X',
-              'APP Attitude MSO Y': 'ATTITUDE_MSO_Y',
-              'APP Attitude MSO Z': 'ATTITUDE_MSO_Z',
-              'Spacecraft GEO X': 'GEO_X',
-              'Spacecraft GEO Y': 'GEO_Y',
-              'Spacecraft GEO Z': 'GEO_Z',
-              'Spacecraft MSO X': 'MSO_X',
-              'Spacecraft MSO Y': 'MSO_Y',
-              'Spacecraft MSO Z': 'MSO_Z',
-              'Spacecraft GEO Longitude': 'SUB_SC_LONGITUDE',
-              'Spacecraft GEO Latitude': 'SUB_SC_LATITUDE',
-              'Spacecraft Solar Zenith Angle': 'SZA',
-              'Spacecraft Local Time': 'LOCAL_TIME',
-              'Spacecraft Altitude Aeroid': 'ALTITUDE',
-              'Spacecraft Attitude GEO X': 'ATTITUDE_GEO_X',
-              'Spacecraft Attitude GEO Y': 'ATTITUDE_GEO_Y',
-              'Spacecraft Attitude GEO Z': 'ATTITUDE_GEO_Z',
-              'Spacecraft Attitude MSO X': 'ATTITUDE_MSO_X',
-              'Spacecraft Attitude MSO Y': 'ATTITUDE_MSO_Y',
-              'Spacecraft Attitude MSO Z': 'ATTITUDE_MSO_Z',
-              'Mars Season (Ls)': 'MARS_SEASON',
-              'Mars-Sun Distance': 'MARS_SUN_DISTANCE',
-              'Subsolar Point GEO Longitude': 'SUBSOLAR_POINT_GEO_LONGITUDE',
-              'Subsolar Point GEO Latitude': 'SUBSOLAR_POINT_GEO_LATITUDE',
-              'Sub-Mars Point on the Sun Longitude': 'SUBMARS_POINT_SOLAR_LONGITUDE',
-              'Sub-Mars Point on the Sun Latitude': 'SUBMARS_POINT_SOLAR_LATITUDE',
-              'Rot matrix MARS -> MSO Row 1, Col 1': 'T11',
-              'Rot matrix MARS -> MSO Row 1, Col 2': 'T12',
-              'Rot matrix MARS -> MSO Row 1, Col 3': 'T13',
-              'Rot matrix MARS -> MSO Row 2, Col 1': 'T21',
-              'Rot matrix MARS -> MSO Row 2, Col 2': 'T22',
-              'Rot matrix MARS -> MSO Row 2, Col 3': 'T23',
-              'Rot matrix MARS -> MSO Row 3, Col 1': 'T31',
-              'Rot matrix MARS -> MSO Row 3, Col 2': 'T32',
-              'Rot matrix MARS -> MSO Row 3, Col 3': 'T33',
-              'Rot matrix SPCCRFT -> MSO Row 1, Col 1': 'SPACECRAFT_T11',
-              'Rot matrix SPCCRFT -> MSO Row 1, Col 2': 'SPACECRAFT_T12',
-              'Rot matrix SPCCRFT -> MSO Row 1, Col 3': 'SPACECRAFT_T13',
-              'Rot matrix SPCCRFT -> MSO Row 2, Col 1': 'SPACECRAFT_T21',
-              'Rot matrix SPCCRFT -> MSO Row 2, Col 2': 'SPACECRAFT_T22',
-              'Rot matrix SPCCRFT -> MSO Row 2, Col 3': 'SPACECRAFT_T23',
-              'Rot matrix SPCCRFT -> MSO Row 3, Col 1': 'SPACECRAFT_T31',
-              'Rot matrix SPCCRFT -> MSO Row 3, Col 2': 'SPACECRAFT_T32',
-              'Rot matrix SPCCRFT -> MSO Row 3, Col 3': 'SPACECRAFT_T33'}
+def maven_param_list():
+    """
+    Returns a dictionary of MAVEN parameters and their corresponding keys.
+
+    Returns:
+        dict: A dictionary mapping parameter names to their keys.
+    """
+
+    param_dict = {
+        "Electron Density": "ELECTRON_DENSITY",
+        "Electron Density Quality Min": "ELECTRON_DENSITY_QUAL_MIN",
+        "Electron Density Quality Max": "ELECTRON_DENSITY_QUAL_MAX",
+        "Electron Temperature": "ELECTRON_TEMPERATURE",
+        "Electron Temperature Quality Min": "ELECTRON_TEMPERATURE_QUAL_MIN",
+        "Electron Temperature Quality Max": "ELECTRON_TEMPERATURE_QUAL_MAX",
+        "Spacecraft Potential": "SPACECRAFT_POTENTIAL",
+        "Spacecraft Potential Quality Min": "SPACECRAFT_POTENTIAL_QUAL_MIN",
+        "Spacecraft Potential Quality Max": "SPACECRAFT_POTENTIAL_QUAL_MAX",
+        "E-field Power 2-100 Hz": "EWAVE_LOW_FREQ",
+        "E-field 2-100 Hz Quality": "EWAVE_LOW_FREQ_QUAL_QUAL",
+        "E-field Power 100-800 Hz": "EWAVE_MID_FREQ",
+        "E-field 100-800 Hz Quality": "EWAVE_MID_FREQ_QUAL_QUAL",
+        "E-field Power 0.8-1.0 Mhz": "EWAVE_HIGH_FREQ",
+        "E-field 0.8-1.0 Mhz Quality": "EWAVE_HIGH_FREQ_QUAL_QUAL",
+        "EUV Irradiance 0.1-7.0 nm": "IRRADIANCE_LOW",
+        "Irradiance 0.1-7.0 nm Quality": "IRRADIANCE_LOW_QUAL",
+        "EUV Irradiance 17-22 nm": "IRRADIANCE_MID",
+        "Irradiance 17-22 nm Quality": "IRRADIANCE_MID_QUAL",
+        "EUV Irradiance Lyman-alpha": "IRRADIANCE_LYMAN",
+        "Irradiance Lyman-alpha Quality": "IRRADIANCE_LYMAN_QUAL",
+        "Solar Wind Electron Density": "SOLAR_WIND_ELECTRON_DENSITY",
+        "Solar Wind E- Density Quality": "SOLAR_WIND_ELECTRON_DENSITY_QUAL",
+        "Solar Wind Electron Temperature": "SOLAR_WIND_ELECTRON_TEMPERATURE",
+        "Solar Wind E- Temperature Quality": "SOLAR_WIND_ELECTRON_TEMPERATURE_QUAL",
+        "Flux, e- Parallel (5-100 ev)": "ELECTRON_PARALLEL_FLUX_LOW",
+        "Flux, e- Parallel (5-100 ev) Quality": "ELECTRON_PARALLEL_FLUX_LOW_QUAL",
+        "Flux, e- Parallel (100-500 ev)": "ELECTRON_PARALLEL_FLUX_MID",
+        "Flux, e- Parallel (100-500 ev) Quality": "ELECTRON_PARALLEL_FLUX_MID_QUAL",
+        "Flux, e- Parallel (500-1000 ev)": "ELECTRON_PARALLEL_FLUX_HIGH",
+        "Flux, e- Parallel (500-1000 ev) Quality": "ELECTRON_PARALLEL_FLUX_HIGH_QUAL",
+        "Flux, e- Anti-par (5-100 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_LOW",
+        "Flux, e- Anti-par (5-100 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_LOW_QUAL",
+        "Flux, e- Anti-par (100-500 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_MID",
+        "Flux, e- Anti-par (100-500 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_MID_QUAL",
+        "Flux, e- Anti-par (500-1000 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_HIGH",
+        "Flux, e- Anti-par (500-1000 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_HIGH_QUAL",
+        "Electron eflux Parallel (5-100 ev)": "ELECTRON_PARALLEL_FLUX_LOW",
+        "Electron eflux Parallel (5-100 ev) Quality": "ELECTRON_PARALLEL_FLUX_LOW_QUAL",
+        "Electron eflux Parallel (100-500 ev)": "ELECTRON_PARALLEL_FLUX_MID",
+        "Electron eflux Parallel (100-500 ev) Quality": "ELECTRON_PARALLEL_FLUX_MID_QUAL",
+        "Electron eflux Parallel (500-1000 ev)": "ELECTRON_PARALLEL_FLUX_HIGH",
+        "Electron eflux Parallel (500-1000 ev) Quality": "ELECTRON_PARALLEL_FLUX_HIGH_QUAL",
+        "Electron eflux Anti-par (5-100 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_LOW",
+        "Electron eflux Anti-par (5-100 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_LOW_QUAL",
+        "Electron eflux Anti-par (100-500 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_MID",
+        "Electron eflux Anti-par (100-500 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_MID_QUAL",
+        "Electron eflux Anti-par (500-1000 ev)": "ELECTRON_ANTI_PARALLEL_FLUX_HIGH",
+        "Electron eflux Anti-par (500-1000 ev) Quality": "ELECTRON_ANTI_PARALLEL_FLUX_HIGH_QUAL",
+        "Electron Spectrum Shape": "ELECTRON_SPECTRUM_SHAPE_PARAMETER",
+        "Spectrum Shape Quality": "ELECTRON_SPECTRUM_SHAPE_PARAMETER_QUAL",
+        "H+ Density": "HPLUS_DENSITY",
+        "H+ Density Quality": "HPLUS_DENSITY_QUAL",
+        "H+ Flow Velocity MSO X": "HPLUS_FLOW_VELOCITY_MSO_X",
+        "H+ Flow MSO X Quality": "HPLUS_FLOW_VELOCITY_MSO_X_QUAL",
+        "H+ Flow Velocity MSO Y": "HPLUS_FLOW_VELOCITY_MSO_Y",
+        "H+ Flow MSO Y Quality": "HPLUS_FLOW_VELOCITY_MSO_Y_QUAL",
+        "H+ Flow Velocity MSO Z": "HPLUS_FLOW_VELOCITY_MSO_Z",
+        "H+ Flow MSO Z Quality": "HPLUS_FLOW_VELOCITY_MSO_Z_QUAL",
+        "H+ Temperature": "HPLUS_TEMPERATURE",
+        "H+ Temperature Quality": "HPLUS_TEMPERATURE_QUAL",
+        "Solar Wind Dynamic Pressure": "SOLAR_WIND_DYNAMIC_PRESSURE",
+        "Solar Wind Pressure Quality": "SOLAR_WIND_DYNAMIC_PRESSURE_QUAL",
+        "STATIC Quality Flag": "STATIC_QUALITY_FLAG",
+        "O+ Density": "OPLUS_DENSITY",
+        "O+ Density Quality": "OPLUS_DENSITY_QUAL",
+        "O2+ Density": "O2PLUS_DENSITY",
+        "O2+ Density Quality": "O2PLUS_DENSITY_QUAL",
+        "O+ Temperature": "OPLUS_TEMPERATURE",
+        "O+ Temperature Quality": "OPLUS_TEMPERATURE_QUAL",
+        "O2+ Temperature": "O2PLUS_TEMPERATURE",
+        "O2+ Temperature Quality": "O2PLUS_TEMPERATURE_QUAL",
+        "O2+ Flow Velocity MAVEN_APP X": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_X",
+        "O2+ Flow MAVEN_APP X Quality": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_X_QUAL",
+        "O2+ Flow Velocity MAVEN_APP Y": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_Y",
+        "O2+ Flow MAVEN_APP Y Quality": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_Y_QUAL",
+        "O2+ Flow Velocity MAVEN_APP Z": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_Z",
+        "O2+ Flow MAVEN_APP Z Quality": "O2PLUS_FLOW_VELOCITY_MAVEN_APP_Z_QUAL",
+        "O2+ Flow Velocity MSO X": "O2PLUS_FLOW_VELOCITY_MSO_X",
+        "O2+ Flow MSO X Quality": "O2PLUS_FLOW_VELOCITY_MSO_X_QUAL",
+        "O2+ Flow Velocity MSO Y": "O2PLUS_FLOW_VELOCITY_MSO_Y",
+        "O2+ Flow MSO Y Quality": "O2PLUS_FLOW_VELOCITY_MSO_Y_QUAL",
+        "O2+ Flow Velocity MSO Z": "O2PLUS_FLOW_VELOCITY_MSO_Z",
+        "O2+ Flow MSO Z Quality": "O2PLUS_FLOW_VELOCITY_MSO_Z_QUAL",
+        "H+ Omni Flux": "HPLUS_OMNI_DIRECTIONAL_FLUX",
+        "H+ Energy": "HPLUS_CHARACTERISTIC_ENERGY",
+        "H+ Energy Quality": "HPLUS_CHARACTERISTIC_ENERGY_QUAL",
+        "He++ Omni Flux": "HEPLUS_OMNI_DIRECTIONAL_FLUX",
+        "He++ Energy": "HEPLUS_CHARACTERISTIC_ENERGY",
+        "He++ Energy Quality": "HEPLUS_CHARACTERISTIC_ENERGY_QUAL",
+        "O+ Omni Flux": "OPLUS_OMNI_DIRECTIONAL_FLUX",
+        "O+ Energy": "OPLUS_CHARACTERISTIC_ENERGY",
+        "O+ Energy Quality": "OPLUS_CHARACTERISTIC_ENERGY_QUAL",
+        "O2+ Omni Flux": "O2PLUS_OMNI_DIRECTIONAL_FLUX",
+        "O2+ Energy": "O2PLUS_CHARACTERISTIC_ENERGY",
+        "O2+ Energy Quality": "O2PLUS_CHARACTERISTIC_ENERGY_QUAL",
+        "H+ Direction MSO X": "HPLUS_CHARACTERISTIC_DIRECTION_MSO_X",
+        "H+ Direction MSO Y": "HPLUS_CHARACTERISTIC_DIRECTION_MSO_Y",
+        "H+ Direction MSO Z": "HPLUS_CHARACTERISTIC_DIRECTION_MSO_Z",
+        "H+ Angular Width": "HPLUS_CHARACTERISTIC_ANGULAR_WIDTH",
+        "H+ Width Quality": "HPLUS_CHARACTERISTIC_ANGULAR_WIDTH_QUAL",
+        "Pickup Ion Direction MSO X": "DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_X",
+        "Pickup Ion Direction MSO Y": "DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_Y",
+        "Pickup Ion Direction MSO Z": "DOMINANT_PICKUP_ION_CHARACTERISTIC_DIRECTION_MSO_Z",
+        "Pickup Ion Angular Width": "DOMINANT_PICKUP_ION_CHARACTERISTIC_ANGULAR_WIDTH",
+        "Pickup Ion Width Quality": "DOMINANT_PICKUP_ION_CHARACTERISTIC_ANGULAR_WIDTH_QUAL",
+        "Ion Flux FOV 1 F": "ION_ENERGY_FLUX__FOV_1_F",
+        "Ion Flux FOV 1F Quality": "ION_ENERGY_FLUX__FOV_1_F_QUAL",
+        "Ion Flux FOV 1 R": "ION_ENERGY_FLUX__FOV_1_R",
+        "Ion Flux FOV 1R Quality": "ION_ENERGY_FLUX__FOV_1_R_QUAL",
+        "Ion Flux FOV 2 F": "ION_ENERGY_FLUX__FOV_2_F",
+        "Ion Flux FOV 2F Quality": "ION_ENERGY_FLUX__FOV_2_F_QUAL",
+        "Ion Flux FOV 2 R": "ION_ENERGY_FLUX__FOV_2_R",
+        "Ion Flux FOV 2R Quality": "ION_ENERGY_FLUX__FOV_2_R_QUAL",
+        "Electron Flux FOV 1 F": "ELECTRON_ENERGY_FLUX___FOV_1_F",
+        "Electron Flux FOV 1F Quality": "ELECTRON_ENERGY_FLUX___FOV_1_F_QUAL",
+        "Electron Flux FOV 1 R": "ELECTRON_ENERGY_FLUX___FOV_1_R",
+        "Electron Flux FOV 1R Quality": "ELECTRON_ENERGY_FLUX___FOV_1_R_QUAL",
+        "Electron Flux FOV 2 F": "ELECTRON_ENERGY_FLUX___FOV_2_F",
+        "Electron Flux FOV 2F Quality": "ELECTRON_ENERGY_FLUX___FOV_2_F_QUAL",
+        "Electron Flux FOV 2 R": "ELECTRON_ENERGY_FLUX___FOV_2_R",
+        "Electron Flux FOV 2R Quality": "ELECTRON_ENERGY_FLUX___FOV_2_R_QUAL",
+        "Look Direction 1-F MSO X": "LOOK_DIRECTION_1_F_MSO_X",
+        "Look Direction 1-F MSO Y": "LOOK_DIRECTION_1_F_MSO_Y",
+        "Look Direction 1-F MSO Z": "LOOK_DIRECTION_1_F_MSO_Z",
+        "Look Direction 1-R MSO X": "LOOK_DIRECTION_1_R_MSO_X",
+        "Look Direction 1-R MSO Y": "LOOK_DIRECTION_1_R_MSO_Y",
+        "Look Direction 1-R MSO Z": "LOOK_DIRECTION_1_R_MSO_Z",
+        "Look Direction 2-F MSO X": "LOOK_DIRECTION_2_F_MSO_X",
+        "Look Direction 2-F MSO Y": "LOOK_DIRECTION_2_F_MSO_Y",
+        "Look Direction 2-F MSO Z": "LOOK_DIRECTION_2_F_MSO_Z",
+        "Look Direction 2-R MSO X": "LOOK_DIRECTION_2_R_MSO_X",
+        "Look Direction 2-R MSO Y": "LOOK_DIRECTION_2_R_MSO_Y",
+        "Look Direction 2-R MSO Z": "LOOK_DIRECTION_2_R_MSO_Z",
+        "Magnetic Field MSO X": "MSO_X",
+        "Magnetic MSO X Quality": "MSO_X_QUAL",
+        "Magnetic Field MSO Y": "MSO_Y",
+        "Magnetic MSO Y Quality": "MSO_Y_QUAL",
+        "Magnetic Field MSO Z": "MSO_Z",
+        "Magnetic MSO Z Quality": "MSO_Z_QUAL",
+        "Magnetic Field GEO X": "GEO_X",
+        "Magnetic GEO X Quality": "GEO_X_QUAL",
+        "Magnetic Field GEO Y": "GEO_Y",
+        "Magnetic GEO Y Quality": "GEO_Y_QUAL",
+        "Magnetic Field GEO Z": "GEO_Z",
+        "Magnetic GEO Z Quality": "GEO_Z_QUAL",
+        "Magnetic Field RMS Dev": "RMS_DEVIATION",
+        "Magnetic RMS Quality": "RMS_DEVIATION_QUAL",
+        "Density He": "HE_DENSITY",
+        "Density He Precision": "HE_DENSITY_PRECISION",
+        "Density He Quality": "HE_DENSITY_QUAL",
+        "Density O": "O_DENSITY",
+        "Density O Precision": "O_DENSITY_PRECISION",
+        "Density O Quality": "O_DENSITY_QUAL",
+        "Density CO": "CO_DENSITY",
+        "Density CO Precision": "CO_DENSITY_PRECISION",
+        "Density CO Quality": "CO_DENSITY_QUAL",
+        "Density N2": "N2_DENSITY",
+        "Density N2 Precision": "N2_DENSITY_PRECISION",
+        "Density N2 Quality": "N2_DENSITY_QUAL",
+        "Density NO": "NO_DENSITY",
+        "Density NO Precision": "NO_DENSITY_PRECISION",
+        "Density NO Quality": "NO_DENSITY_QUAL",
+        "Density Ar": "AR_DENSITY",
+        "Density Ar Precision": "AR_DENSITY_PRECISION",
+        "Density Ar Quality": "AR_DENSITY_QUAL",
+        "Density CO2": "CO2_DENSITY",
+        "Density CO2 Precision": "CO2_DENSITY_PRECISION",
+        "Density CO2 Quality": "CO2_DENSITY_QUAL",
+        "Density 32+": "O2PLUS_DENSITY",
+        "Density 32+ Precision": "O2PLUS_DENSITY_PRECISION",
+        "Density 32+ Quality": "O2PLUS_DENSITY_QUAL",
+        "Density 44+": "CO2PLUS_DENSITY",
+        "Density 44+ Precision": "CO2PLUS_DENSITY_PRECISION",
+        "Density 44+ Quality": "CO2PLUS_DENSITY_QUAL",
+        "Density 30+": "NOPLUS_DENSITY",
+        "Density 30+ Precision": "NOPLUS_DENSITY_PRECISION",
+        "Density 30+ Quality": "NOPLUS_DENSITY_QUAL",
+        "Density 16+": "OPLUS_DENSITY",
+        "Density 16+ Precision": "OPLUS_DENSITY_PRECISION",
+        "Density 16+ Quality": "OPLUS_DENSITY_QUAL",
+        "Density 28+": "CO2PLUS_N2PLUS_DENSITY",
+        "Density 28+ Precision": "CO2PLUS_N2PLUS_DENSITY_PRECISION",
+        "Density 28+ Quality": "CO2PLUS_N2PLUS_DENSITY_QUAL",
+        "Density 12+": "CPLUS_DENSITY",
+        "Density 12+ Precision": "CPLUS_DENSITY_PRECISION",
+        "Density 12+ Quality": "CPLUS_DENSITY_QUAL",
+        "Density 17+": "OHPLUS_DENSITY",
+        "Density 17+ Precision": "OHPLUS_DENSITY_PRECISION",
+        "Density 17+ Quality": "OHPLUS_DENSITY_QUAL",
+        "Density 14+": "NPLUS_DENSITY",
+        "Density 14+ Precision": "NPLUS_DENSITY_PRECISION",
+        "Density 14+ Quality": "NPLUS_DENSITY_QUAL",
+        "APP Attitude GEO X": "ATTITUDE_GEO_X",
+        "APP Attitude GEO Y": "ATTITUDE_GEO_Y",
+        "APP Attitude GEO Z": "ATTITUDE_GEO_Z",
+        "APP Attitude MSO X": "ATTITUDE_MSO_X",
+        "APP Attitude MSO Y": "ATTITUDE_MSO_Y",
+        "APP Attitude MSO Z": "ATTITUDE_MSO_Z",
+        "Spacecraft GEO X": "GEO_X",
+        "Spacecraft GEO Y": "GEO_Y",
+        "Spacecraft GEO Z": "GEO_Z",
+        "Spacecraft MSO X": "MSO_X",
+        "Spacecraft MSO Y": "MSO_Y",
+        "Spacecraft MSO Z": "MSO_Z",
+        "Spacecraft GEO Longitude": "SUB_SC_LONGITUDE",
+        "Spacecraft GEO Latitude": "SUB_SC_LATITUDE",
+        "Spacecraft Solar Zenith Angle": "SZA",
+        "Spacecraft Local Time": "LOCAL_TIME",
+        "Spacecraft Altitude Aeroid": "ALTITUDE",
+        "Spacecraft Attitude GEO X": "ATTITUDE_GEO_X",
+        "Spacecraft Attitude GEO Y": "ATTITUDE_GEO_Y",
+        "Spacecraft Attitude GEO Z": "ATTITUDE_GEO_Z",
+        "Spacecraft Attitude MSO X": "ATTITUDE_MSO_X",
+        "Spacecraft Attitude MSO Y": "ATTITUDE_MSO_Y",
+        "Spacecraft Attitude MSO Z": "ATTITUDE_MSO_Z",
+        "Mars Season (Ls)": "MARS_SEASON",
+        "Mars-Sun Distance": "MARS_SUN_DISTANCE",
+        "Subsolar Point GEO Longitude": "SUBSOLAR_POINT_GEO_LONGITUDE",
+        "Subsolar Point GEO Latitude": "SUBSOLAR_POINT_GEO_LATITUDE",
+        "Sub-Mars Point on the Sun Longitude": "SUBMARS_POINT_SOLAR_LONGITUDE",
+        "Sub-Mars Point on the Sun Latitude": "SUBMARS_POINT_SOLAR_LATITUDE",
+        "Rot matrix MARS -> MSO Row 1, Col 1": "T11",
+        "Rot matrix MARS -> MSO Row 1, Col 2": "T12",
+        "Rot matrix MARS -> MSO Row 1, Col 3": "T13",
+        "Rot matrix MARS -> MSO Row 2, Col 1": "T21",
+        "Rot matrix MARS -> MSO Row 2, Col 2": "T22",
+        "Rot matrix MARS -> MSO Row 2, Col 3": "T23",
+        "Rot matrix MARS -> MSO Row 3, Col 1": "T31",
+        "Rot matrix MARS -> MSO Row 3, Col 2": "T32",
+        "Rot matrix MARS -> MSO Row 3, Col 3": "T33",
+        "Rot matrix SPCCRFT -> MSO Row 1, Col 1": "SPACECRAFT_T11",
+        "Rot matrix SPCCRFT -> MSO Row 1, Col 2": "SPACECRAFT_T12",
+        "Rot matrix SPCCRFT -> MSO Row 1, Col 3": "SPACECRAFT_T13",
+        "Rot matrix SPCCRFT -> MSO Row 2, Col 1": "SPACECRAFT_T21",
+        "Rot matrix SPCCRFT -> MSO Row 2, Col 2": "SPACECRAFT_T22",
+        "Rot matrix SPCCRFT -> MSO Row 2, Col 3": "SPACECRAFT_T23",
+        "Rot matrix SPCCRFT -> MSO Row 3, Col 1": "SPACECRAFT_T31",
+        "Rot matrix SPCCRFT -> MSO Row 3, Col 2": "SPACECRAFT_T32",
+        "Rot matrix SPCCRFT -> MSO Row 3, Col 3": "SPACECRAFT_T33",
+    }
+    return param_dict
```

### Comparing `pyspedas-1.5.6/pyspedas/mica/load.py` & `pyspedas-1.5.7/pyspedas/mica/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mica/tests/tests.py` & `pyspedas-1.5.7/pyspedas/mica/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/__init__.py` & `pyspedas-1.5.7/pyspedas/mms/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 
         and/or
 
             >>> import pyspedas
             >>> fgm_data = pyspedas.mms.fgm(...)
 '''
 
+# Some of these wrappers shadow MMS module names in a way that seems too fragile -- adding an apparently unrelated
+# import in the "wrong" place can start triggering errors like "module fgm is not callable".  It might be better and
+# more robust to rename the instrument directories so they don't conflict with the wrapper names.  Also,
+# perhaps these wrapper names should be the "real" names, with the longer names mms_load_fgm, mms_load_state, etc.
+# as wrappers or aliases rather than the other way around.   At least in PyCharm, hovering over a call to fgm() to
+# see the argument list only shows the *args and **kwargs parameters, which is not terribly useful.
+# JWL 2024-03-29
+
 @wraps(spd_mms_load_bss)
 def bss(*args, **kwargs):
     return spd_mms_load_bss(*args, **kwargs)
 
 @wraps(mms_load_state)
 def state(*args, **kwargs):
     return mms_load_state(*args, **kwargs)
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/aspoc/aspoc.py` & `pyspedas-1.5.7/pyspedas/mms/aspoc/aspoc.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_lmn.py` & `pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_lmn.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_qrotate.py` & `pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_qrotate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/cotrans/mms_cotrans_qtransformer.py` & `pyspedas-1.5.7/pyspedas/mms/cotrans/mms_cotrans_qtransformer.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/cotrans/mms_qcotrans.py` & `pyspedas-1.5.7/pyspedas/mms/cotrans/mms_qcotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/dsp/dsp.py` & `pyspedas-1.5.7/pyspedas/mms/dsp/dsp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/dsp/mms_dsp_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/dsp/mms_dsp_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/edi/edi.py` & `pyspedas-1.5.7/pyspedas/mms/edi/edi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/edi/mms_edi_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/edi/mms_edi_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/edp/edp.py` & `pyspedas-1.5.7/pyspedas/mms/edp/edp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/edp/mms_edp_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/edp/mms_edp_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/eis.py` & `pyspedas-1.5.7/pyspedas/mms/eis/eis.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_omni.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_omni.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_pad.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_pad.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_pad_spinavg.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_spec_combine_sc.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_spec_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/eis/mms_eis_spin_avg.py` & `pyspedas-1.5.7/pyspedas/mms/eis/mms_eis_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/feeps.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/feeps.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_active_eyes.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_active_eyes.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_correct_energies.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_correct_energies.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_energy_table.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_energy_table.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_flat_field_corrections.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_flat_field_corrections.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_getgyrophase.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_getgyrophase.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_gpd.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_gpd.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_omni.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pad.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pad.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pad_spinavg.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_pitch_angles.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_pitch_angles.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_remove_bad_data.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_remove_bad_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_remove_sun.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_remove_sun.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_spin_avg.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_feeps_split_integral_ch.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_feeps_split_integral_ch.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/feeps/mms_read_feeps_sector_masks_csv.py` & `pyspedas-1.5.7/pyspedas/mms/feeps/mms_read_feeps_sector_masks_csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,16 @@
              1468022400.0000000, # 7/9/2016
              1477612800.0000000, # 10/28/2016
              1496188800.0000000, # 5/31/2017
              1506988800.0000000, # 10/3/2017
              1538697600.0000000, # 10/5/2018
              1642032000.0000000, # 1/13/2022
              1651795200.0000000, # 5/6/2022
-             1660521600.0000000] # 8/15/2022
+             1660521600.0000000, # 8/15/2022
+             1706832000.0000000] # 02/02/2024
 
     # find the file closest to the start time
     nearest_date = dates[(np.abs(np.array(dates)-time_double(trange[0]))).argmin()]
 
     for mms_sc in [1, 2, 3, 4]:
         csv_file = os.sep.join([os.path.dirname(os.path.abspath(__file__)), 'sun', 'MMS'+str(mms_sc)+'_FEEPS_ContaminatedSectors_'+time_string(nearest_date, fmt='%Y%m%d')+'.csv'])
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/fgm.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/fgm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/mms_curl.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/mms_curl.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/mms_fgm_remove_flags.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/mms_fgm_remove_flags.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/mms_fgm_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/mms_fgm_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/mms_lingradest.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/mms_lingradest.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fgm/mms_split_fgm_data.py` & `pyspedas-1.5.7/pyspedas/mms/fgm/mms_split_fgm_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/fpi.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/fpi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_ang_ang.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_make_compressionlossbars.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_make_compressionlossbars.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         logging.error('Problem reading the variable: ' + tname)
         return
 
     flagline = np.zeros(len(data.times))
 
     if not lossy:
         file_id = metadata['CDF']['GATT']['Logical_file_id']
+        if isinstance(file_id, list):  # Workaround for cdflib bug in globalattsget
+            file_id = file_id[0]
         version = file_id.split('_v')[1].split('.')
         if version[0] == '2':
             if version[1] == '1':
                 if data.times[0] < time_datetime('2016-04-01'):
                     lossy = 3
                 else:
                     lossy = 1
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_make_errorflagbars.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_make_errorflagbars.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,21 @@
 
     data = get_data(tname, dt=True)
     metadata = get_data(tname, metadata=True)
 
     if metadata is None:
         return
 
-    if metadata['CDF']['GATT']['Data_type'][-4:] == 'moms' or level == 'ql':
+
+    # Workaround for cdflib globalattsget() bug
+    md_dt = metadata['CDF']['GATT']['Data_type']
+    if isinstance(md_dt, list):
+        md_dt = md_dt[0]
+
+    if md_dt[-4:] == 'moms' or level == 'ql':
         labels_full=['Contact FPI team','Saturation','SCpot>20V','no SCpot','>10% Cold','>25% Hot','High Mach#','Low Density','Onboard Mag','L2pre Mag','Photoelectrons','Compression', 'Spintones', 'Radiation']
 
         flags = ['{0:014b}'.format(flag) for flag in data.y]
         flagline = np.zeros((len(data.times), 14))
         flagline_others = np.zeros(len(data.times))
         flagline_all = np.zeros(len(data.times))
         for j, flag in enumerate(flags):
@@ -216,15 +222,15 @@
             options(tname + '_flagbars_mini', 'symbols', True)
             options(tname + '_flagbars_mini', 'markers', 's')
 
         out_vars = [tname + '_flagbars_full',
                     tname + '_flagbars_main',
                     tname + '_flagbars_others',
                     tname + '_flagbars_mini']
-    elif metadata['CDF']['GATT']['Data_type'][-4:] == 'dist':
+    elif md_dt[-4:] == 'dist':
         flags = ['{0:014b}'.format(flag) for flag in data.y]
         flagline = np.zeros((len(data.times), 2))
         for i in [0, 1]:
             for j in range(len(flags)):
                 try:
                     flagset = int(flags[13-i:13-i+1][0])
                 except IndexError:
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_fpi_split_tensor.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_fpi_split_tensor.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_get_fpi_dist.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_get_fpi_dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import numpy as np
-from pyspedas import time_double
-from pytplot import get_data
+from pytplot import get_data, time_double
 
 logging.captureWarnings(True)
 logging.basicConfig(format='%(asctime)s: %(message)s', datefmt='%d-%b-%y %H:%M:%S', level=logging.INFO)
 
 
 def mms_get_fpi_dist(tname, index=None, probe=None, data_rate=None, species=None, level='l2', single_time=None):
     """
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_load_fpi_calc_pad.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_load_fpi_calc_pad.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fpi/mms_pad_fpi.py` & `pyspedas-1.5.7/pyspedas/mms/fpi/mms_pad_fpi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/fsm/fsm.py` & `pyspedas-1.5.7/pyspedas/mms/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/hpca.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/hpca.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_get_hpca_dist.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_get_hpca_dist.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_get_hpca_info.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_get_hpca_info.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_calc_anodes.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_calc_anodes.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_energies.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_energies.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/hpca/mms_hpca_spin_sum.py` & `pyspedas-1.5.7/pyspedas/mms/hpca/mms_hpca_spin_sum.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec/earth_polar1.png` & `pyspedas-1.5.7/pyspedas/mms/mec/earth_polar1.png`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec/mec.py` & `pyspedas-1.5.7/pyspedas/mms/mec/mec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec/mms_mec_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/mec/mms_mec_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_local_ancillary_files.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_local_ancillary_files.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_local_state_files.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_local_state_files.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_state_data.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_state_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     if 'spinras' in datatypes or 'spindec' in datatypes:
         filetypes.append('att')
 
     user = None
     if not no_download:
         sdc_session, user = mms_login_lasp(always_prompt=always_prompt)
 
+    return_vars = []
+
     for probe_id in probe:
         # probe will need to be a string from now on
         probe_id = str(probe_id)
 
         for filetype in filetypes:
             product = level + filetype
 
@@ -133,15 +135,15 @@
                 continue
 
             # if no files are found remotely, try locally
             if not out_files:
                 out_files = mms_get_local_state_files(probe=probe_id, level=level, filetype=filetype, trange=[start_time_str, end_time_str])
 
             if filetype == 'eph':
-                return_vars = mms_load_eph_tplot(sorted(out_files), level=level, probe=probe_id, datatypes=datatypes, suffix=suffix, trange=trange)
+                return_vars += mms_load_eph_tplot(sorted(out_files), level=level, probe=probe_id, datatypes=datatypes, suffix=suffix, trange=trange)
             elif filetype == 'att':
-                return_vars = mms_load_att_tplot(sorted(out_files), level=level, probe=probe_id, datatypes=datatypes, suffix=suffix, trange=trange)
+                return_vars += mms_load_att_tplot(sorted(out_files), level=level, probe=probe_id, datatypes=datatypes, suffix=suffix, trange=trange)
 
     if not no_download:
         sdc_session.close()
 
     return return_vars
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_get_tetrahedron_qf.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_get_tetrahedron_qf.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_att_tplot.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_att_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_eph_tplot.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_eph_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/mms_load_qf_tplot.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/mms_load_qf_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/state.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/state.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mec_ascii/tetrahedron_qf.py` & `pyspedas-1.5.7/pyspedas/mms/mec_ascii/tetrahedron_qf.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_config.py` & `pyspedas-1.5.7/pyspedas/mms/mms_config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_events.py` & `pyspedas-1.5.7/pyspedas/mms/mms_events.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_file_filter.py` & `pyspedas-1.5.7/pyspedas/mms/mms_file_filter.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_files_in_interval.py` & `pyspedas-1.5.7/pyspedas/mms/mms_files_in_interval.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_get_local_files.py` & `pyspedas-1.5.7/pyspedas/mms/mms_get_local_files.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_load_brst_segments.py` & `pyspedas-1.5.7/pyspedas/mms/mms_load_brst_segments.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_load_data.py` & `pyspedas-1.5.7/pyspedas/mms/mms_load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,17 @@
                                 # if the download was successful, copy to data directory
                                 copy(ftmp.name, out_file)
                                 out_files.append(out_file)
                                 file_found = True
                                 fsrc.close()
                                 ftmp.close()
                                 os.unlink(ftmp.name)  # delete the temporary file
-                        except requests.exceptions.ConnectionError:
+                        except requests.exceptions.ConnectionError as e:
                             # No/bad internet connection; try loading the files locally
+                            print(e)
                             logging.error('No internet connection!')
 
                     if not file_found:
                         added_local_files = False
                         if not download_only:
                             logging.info('Searching for local files...')
                             out_files.extend(mms_get_local_files(prb, instrument, drate, lvl, dtype, trange))
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_load_data_spdf.py` & `pyspedas-1.5.7/pyspedas/mms/mms_load_data_spdf.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_load_fast_segments.py` & `pyspedas-1.5.7/pyspedas/mms/mms_load_fast_segments.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_load_sroi_segments.py` & `pyspedas-1.5.7/pyspedas/mms/mms_load_sroi_segments.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_login_lasp.py` & `pyspedas-1.5.7/pyspedas/mms/mms_login_lasp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_orbit_plot.py` & `pyspedas-1.5.7/pyspedas/mms/mms_orbit_plot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_overview_plot.py` & `pyspedas-1.5.7/pyspedas/mms/plots/mms_overview_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
-from pyspedas import time_double, time_string
+import pyspedas
 from pyspedas.mms import fgm, fpi, feeps, hpca, edp, eis
 from pyspedas.themis import gmag
-from pytplot import options, tplot_options, store_data, tplot, tnames
+from pytplot import options, tplot_options, store_data, tplot, tnames, time_double, time_string
 
 
 def mms_overview_plot(
     trange=[],
     date="2022-03-23",
     duration="1",
     probe="1",
     skip_ae_idx=False,
-    save_png=False,
-    directory="",
-    filename="",
+    save_png='',
+    save_eps='',
+    save_svg='',
+    save_pdf='',
+    save_jpeg='',
     display=True,
-    xsize=1000,
-    ysize=1400,
+    xsize=10,
+    ysize=14,
 ):
     """
     Generate an overview plot for MMS data.
 
     Parameters:
     -----------
     trange (list of 2 strings, optional):
@@ -29,36 +31,40 @@
         Date in the format 'YYYY-MM-DD' or 'YYY-MM-DD/hh:mm:ss. Used to calculate the time range if trange is not specified.
     duration: str, optional
         Duration in days. Used to calculate the time range if trange is not specified.
     probe: str, optional
         MMS probe number (1-4).
     skip_ae_idx: bool, optional
         Whether to skip plotting the AE index panel.
-    save_png: bool, optional
-        Whether to save the plot as a PNG file.
-    directory: str, optional
-        Directory to save the plot. If not specified, the plot will not be saved.
-    filename: str, optional
-        Name of the PNG file to save (without the "png" extension). If not specified, a default name will be used.
+    save_png: str, optional
+        .Filename to save plot as PNG
+    save_eps: str, optional
+        .Filename to save plot as EPS
+    save_svg: str, optional
+        .Filename to save plot as SVG
+    save_pdf: str, optional
+        .Filename to save plot as PDF
+    save_jpeg: str, optional
+        .Filename to save plot as JPEG
     display: bool, optional
         If True, then this function will display the plotted tplot variables. Necessary to make this optional
         so we can avoid it in a headless server environment.
     xsize: int, optional
-        Size of the x-axis of the plot window in pixels. Default is 1000.
+        Size of the x-axis of the plot window in inches. Default is 10.
     ysize: int, optional
-        Size of the y-axis of the plot window in pixels. Default is 1400.
+        Size of the y-axis of the plot window in inches. Default is 14.
 
     Returns:
     --------
     None
 
     Examples:
     ---------
-    from pyspedas.mms.mms_overview_plot import mms_overview_plot
-    mms_overview_plot(date='2023-03-23', probe='1', save_png=True, display=False, directory='C:\\work\\mms\\summary plots\\')
+    from pyspedas import mms_overview_plot
+    mms_overview_plot(date='2023-03-23', probe='1', save_png="c:\\work\\mms\\summary_plots\mms_overview", display=False)
 
     Notes:
     ------
     It may need a long time to complete.
 
     Todo:
     -----
@@ -203,21 +209,14 @@
 
     # Save plot
     fname = None
     if isinstance(t1, str):
         t0 = time_string(time_double(t1), fmt="%Y_%m_%d")
     else:
         t0 = time_string(t1, fmt="%Y_%m_%d")
-    if save_png:
-        if directory is None or directory == "":
-            directory = "./"
-        if filename is None or filename == "":
-            fname = directory + "/mms" + probe + "_" + t0
-        else:
-            fname = directory + filename
 
     # Full plot
     vars = [
         panel02,
         panel03,
         panel04,
         panel05,
@@ -234,12 +233,12 @@
 
     # time_clip(vars, time_start=trange[0], time_end=trange[1])
     plot_title = "MMS-" + probe + " Overview (" + t0.replace("_", "-") + ")"
     tplot_options("title", plot_title)
     options(panel01, "name", plot_title)
     # tplot_options("wsize", [1400, 1000]) does not work
     tplot_options("show_all_axes", False)
-    xsize = int(xsize / 100)
-    ysize = int(ysize / 100)
+    xsize = int(xsize)
+    ysize = int(ysize)
 
-    tplot(vars, save_png=fname, display=display, xsize=xsize, ysize=ysize)
+    tplot(vars, save_png=save_png,save_eps=save_eps,save_svg=save_svg,save_pdf=save_pdf,save_jpeg=save_jpeg, display=display, xsize=xsize, ysize=ysize)
     logging.info("MMS overview plot completed.")
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_tai2unix.py` & `pyspedas-1.5.7/pyspedas/mms/mms_tai2unix.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/mms_update_brst_intervals.py` & `pyspedas-1.5.7/pyspedas/mms/mms_update_brst_intervals.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_convert_flux_units.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_convert_flux_units.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_part_des_photoelectrons.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_part_des_photoelectrons.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
     try:
         table_name = metadata['CDF']['GATT']['Energy_table_name']
     except KeyError:
         logging.error('Problem extracting the energy table name from the DF metadata')
         return
 
+    # Workaround for cdflib globalattsget() bug
+    if isinstance(table_name,list):
+        table_name = table_name[0]
     stepper_id = table_name.replace('.txt', '').split('energies_des_')[-1]
 
     # we'll need the data rate
     data_rate = dist_var.split('_')[-1]
 
     # download the model file from the SDC
     pe_model = download(
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_part_getspec.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_part_getspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from time import time
-from pyspedas import time_double, mms
+from pyspedas import mms
 from pyspedas.mms.particles.mms_part_products import mms_part_products
-
+from pytplot import time_double
 logging.captureWarnings(True)
 logging.basicConfig(format='%(asctime)s: %(message)s', datefmt='%d-%b-%y %H:%M:%S', level=logging.INFO)
 
 
 def mms_part_getspec(instrument='fpi',
                      probe='1',
                      species='e',
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_part_products.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_part_products.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_part_slice2d.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_part_slice2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import pyspedas
-from pyspedas import time_double
+from pytplot import time_double
 from pyspedas.mms.fpi.mms_get_fpi_dist import mms_get_fpi_dist
 from pyspedas.mms.hpca.mms_get_hpca_dist import mms_get_hpca_dist
 from pyspedas.particles.spd_slice2d.slice2d import slice2d
 from pyspedas.particles.spd_slice2d.slice2d_plot import plot
 
 
 def mms_part_slice2d(trange=None,
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_clean_data.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_clean_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_clean_support.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_clean_support.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_e_spec.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_e_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_fac.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_fac.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_phi_spec.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_phi_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_make_theta_spec.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_make_theta_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/mms_pgs_split_hpca.py` & `pyspedas-1.5.7/pyspedas/mms/particles/mms_pgs_split_hpca.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/particles/moka_mms_clean_data.py` & `pyspedas-1.5.7/pyspedas/mms/particles/moka_mms_clean_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/print_vars.py` & `pyspedas-1.5.7/pyspedas/mms/print_vars.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/scm/mms_scm_set_metadata.py` & `pyspedas-1.5.7/pyspedas/mms/scm/mms_scm_set_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/scm/scm.py` & `pyspedas-1.5.7/pyspedas/mms/scm/scm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/spd_mms_load_bss.py` & `pyspedas-1.5.7/pyspedas/mms/spd_mms_load_bss.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/cotrans.py` & `pyspedas-1.5.7/pyspedas/mms/tests/cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/curlometer.py` & `pyspedas-1.5.7/pyspedas/mms/tests/curlometer.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/data_rate_segments.py` & `pyspedas-1.5.7/pyspedas/mms/tests/data_rate_segments.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/eis.py` & `pyspedas-1.5.7/pyspedas/mms/tests/eis.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/feeps.py` & `pyspedas-1.5.7/pyspedas/mms/tests/feeps.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/file_filter.py` & `pyspedas-1.5.7/pyspedas/mms/tests/file_filter.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/fpi_tests.py` & `pyspedas-1.5.7/pyspedas/mms/tests/fpi_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/load_routine_tests.py` & `pyspedas-1.5.7/pyspedas/mms/tests/load_routine_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,27 @@
         data = mms_load_state(datatypes=['pos', 'vel'])
         self.assertTrue(data_exists('mms1_defeph_pos'))
         self.assertTrue(data_exists('mms1_defeph_vel'))
         tplot(['mms1_defeph_pos', 'mms1_defeph_vel'], display=False)
         self.assertTrue('mms1_defeph_pos' in data)
         self.assertTrue('mms1_defeph_vel' in data)
 
+    def test_load_eph_multiprobe_data(self):
+        data = mms_load_state(datatypes=['pos', 'vel'],probe=['1','2','3','4'])
+        self.assertTrue(data_exists('mms1_defeph_pos'))
+        self.assertTrue(data_exists('mms1_defeph_vel'))
+        tplot(['mms1_defeph_pos', 'mms1_defeph_vel'], display=False)
+        self.assertTrue('mms1_defeph_pos' in data)
+        self.assertTrue('mms1_defeph_vel' in data)
+        self.assertTrue('mms2_defeph_pos' in data)
+        self.assertTrue('mms2_defeph_vel' in data)
+        self.assertTrue('mms3_defeph_pos' in data)
+        self.assertTrue('mms3_defeph_vel' in data)
+        self.assertTrue('mms4_defeph_pos' in data)
+        self.assertTrue('mms4_defeph_vel' in data)
 
     def test_load_tqf(self):
         data = mms_load_tetrahedron_qf()
         self.assertTrue(data_exists('mms_tetrahedron_qf'))
         tplot('mms_tetrahedron_qf',display=False)
         self.assertTrue('mms_tetrahedron_qf' in data)
```

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/mms_part_getspec.py` & `pyspedas-1.5.7/pyspedas/mms/tests/mms_part_getspec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/neutral_sheet.py` & `pyspedas-1.5.7/pyspedas/mms/tests/neutral_sheet.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/orbit_plots.py` & `pyspedas-1.5.7/pyspedas/mms/tests/orbit_plots.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/ql_l1b_sitl_tests.py` & `pyspedas-1.5.7/pyspedas/mms/tests/ql_l1b_sitl_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/slice2d.py` & `pyspedas-1.5.7/pyspedas/mms/tests/slice2d.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/mms/tests/wavpol.py` & `pyspedas-1.5.7/pyspedas/mms/tests/wavpol.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/noaa/noaa_load_kp.py` & `pyspedas-1.5.7/pyspedas/noaa/noaa_load_kp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/omni/__init__.py` & `pyspedas-1.5.7/pyspedas/omni/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/omni/load.py` & `pyspedas-1.5.7/pyspedas/omni/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/omni/tests/tests.py` & `pyspedas-1.5.7/pyspedas/polar/tests/tests.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,66 @@
 import os
 import unittest
-from pytplot import data_exists, del_data
+from pytplot import data_exists
 import pyspedas
 
 
 class LoadTestCases(unittest.TestCase):
-    def test_utc_timestamp_regression(self):
-        varname = 'BX_GSE'
-        del_data('*')
-        data_omni = pyspedas.omni.data(trange=['2010-01-01/00:00:00', '2010-01-02/00:00:00'],notplot=True,varformat=varname,time_clip=True)
-        self.assertTrue(str(data_omni[varname]['x'][0]) == '2010-01-01 00:00:00')
-
-    def test_load_hro2_data(self):
-        del_data('*')
-        omni_vars = pyspedas.omni.data()
-        self.assertTrue(data_exists('BX_GSE'))
-        self.assertTrue(data_exists('BY_GSE'))
-        self.assertTrue(data_exists('BZ_GSE'))
-        self.assertTrue(data_exists('BY_GSM'))
-        self.assertTrue(data_exists('BZ_GSM'))
-        self.assertTrue(data_exists('proton_density'))
-
-    def test_load_hro_data(self):
-        del_data('*')
-        omni_vars = pyspedas.omni.data(level='hro')
-        self.assertTrue(data_exists('BX_GSE'))
-        self.assertTrue(data_exists('BY_GSE'))
-        self.assertTrue(data_exists('BZ_GSE'))
-        self.assertTrue(data_exists('BY_GSM'))
-        self.assertTrue(data_exists('BZ_GSM'))
-        self.assertTrue(data_exists('proton_density'))
-
-    def test_load_hro_5min_data(self):
-        del_data('*')
-        omni_vars = pyspedas.omni.data(level='hro', datatype='5min')
-        self.assertTrue(data_exists('BX_GSE'))
-        self.assertTrue(data_exists('BY_GSE'))
-        self.assertTrue(data_exists('BZ_GSE'))
-        self.assertTrue(data_exists('BY_GSM'))
-        self.assertTrue(data_exists('BZ_GSM'))
-        self.assertTrue(data_exists('proton_density'))
-
-    def test_load_hro_hour_data(self):
-        del_data('*')
-        omni_vars = pyspedas.omni.data(level='hro2', datatype='hour', trange=['2013-03-01', '2013-03-02'])
-        self.assertTrue(data_exists('BX_GSE'))
-        self.assertTrue(data_exists('BY_GSE'))
-        self.assertTrue(data_exists('BZ_GSE'))
-        self.assertTrue(data_exists('BY_GSM'))
-        self.assertTrue(data_exists('BZ_GSM'))
-
-    def test_load_hro_hour_data_long_interval(self):
-        from pyspedas.utilities.dailynames import dailynames
-        del_data('*')
-        trange=['2013-01-05','2013-11-06']
-        pathformat = 'hourly/%Y/omni2_h0_mrg1hr_%Y%m01_v??.cdf'
-        file_res=24*3600*183 # 1 file every 6 months
-        remote_names=dailynames(file_format=pathformat,trange=trange,res=file_res)
-        print(remote_names)
-        omni_vars = pyspedas.omni.data(datatype='hour', trange=trange)
-        self.assertTrue(data_exists('BX_GSE'))
-        self.assertTrue(data_exists('BY_GSE'))
-        self.assertTrue(data_exists('BZ_GSE'))
-        self.assertTrue(data_exists('BY_GSM'))
-        self.assertTrue(data_exists('BZ_GSM'))
-
-    def test_load_invalid_datatype(self):
-        omni_vars = pyspedas.omni.data(datatype='1')
-
     def test_downloadonly(self):
-        files = pyspedas.omni.data(downloadonly=True, trange=['2014-2-15', '2014-2-16'])
+        files = pyspedas.polar.efi(downloadonly=True)
         self.assertTrue(os.path.exists(files[0]))
 
+    def test_load_mfe_data(self):
+        mfe_vars = pyspedas.polar.mfe(trange=['2003-10-28', '2003-10-29'], get_support_data=True)
+        self.assertTrue(data_exists('B_GSE'))
+        self.assertTrue(data_exists('B_GSM'))
+
+    def test_load_efi_data(self):
+        efi_vars = pyspedas.polar.efi(time_clip=True)
+        self.assertTrue(data_exists('ESPIN'))
+
+    def test_load_pwi_data(self):
+        pwi_vars = pyspedas.polar.pwi()
+        self.assertTrue(data_exists('Fce'))
+
+    def test_load_hydra_data(self):
+        hydra_vars = pyspedas.polar.hydra()
+        self.assertTrue(data_exists('ELE_DENSITY'))
+
+    def test_load_tide_data(self):
+        tide_vars = pyspedas.polar.tide()
+        self.assertTrue(data_exists('total_den'))
+        self.assertTrue(data_exists('total_v'))
+        self.assertTrue(data_exists('total_t'))
+
+    def test_load_timas_data(self):
+        timas_vars = pyspedas.polar.timas()
+        self.assertTrue(data_exists('Density_H'))
+
+    def test_load_cammice_data(self):
+        cammice_vars = pyspedas.polar.cammice()
+        self.assertTrue(data_exists('Protons'))
+
+    def test_load_ceppad_data(self):
+        ceppad_vars = pyspedas.polar.ceppad()
+        self.assertTrue(data_exists('IPS_10_ERR'))
+
+    def test_load_uvi_data(self):
+        uvi_vars = pyspedas.polar.uvi()
+        self.assertTrue(data_exists('IMAGE_DATA'))
+
+    def test_load_pixie_data(self):
+        pixie_vars = pyspedas.polar.pixie()
+        self.assertTrue(data_exists('TXF_HIGH'))
+
+    def test_load_vis_data(self):
+        vis_vars = pyspedas.polar.vis(notplot=True)
+        self.assertTrue('Image_Counts' in vis_vars)
+
+    def test_load_orbit_data(self):
+        orbit_vars = pyspedas.polar.orbit()
+        self.assertTrue(data_exists('AVG_SPIN_RATE'))
+        self.assertTrue(data_exists('SPIN_PHASE'))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/particles/moments/moments_3d.py` & `pyspedas-1.5.7/pyspedas/particles/moments/moments_3d.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/moments/moments_3d_omega_weights.py` & `pyspedas-1.5.7/pyspedas/particles/moments/moments_3d_omega_weights.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/moments/spd_pgs_moments_tplot.py` & `pyspedas-1.5.7/pyspedas/particles/moments/spd_pgs_moments_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_do_fac.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_do_fac.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_limit_range.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_limit_range.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_e_spec.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_e_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_phi_spec.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_phi_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_theta_spec.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_theta_spec.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_make_tplot.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_make_tplot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_progress_update.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_progress_update.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_part_products/spd_pgs_regrid.py` & `pyspedas-1.5.7/pyspedas/particles/spd_part_products/spd_pgs_regrid.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/quaternions.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/quaternions.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice1d_plot.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice1d_plot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .slice2d_nearest import slice2d_nearest
 from .slice2d_rlog import slice2d_rlog
 from .slice2d_s2c import slice2d_s2c
 from .slice2d_2di import slice2d_2di
 from .slice2d_smooth import slice2d_smooth
 from .slice2d_subtract import slice2d_subtract
 
-from pyspedas import time_double, time_string
+from pytplot import time_double, time_string
 
 
 def slice2d(dists,
             time=None,
             samples=None,
             window=None,
             center_time=False,
```

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_2di.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_2di.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_checkbins.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_checkbins.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_collate.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_collate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_custom_rotation.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_custom_rotation.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_geo.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_geo.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_data.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_data.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_ebounds.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_ebounds.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_sphere.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_sphere.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_get_support.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_get_support.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_getinfo.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_getinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyspedas import time_string
+from pytplot import time_string
 from pyspedas.particles.spd_units_string import spd_units_string
 
 
 def slice2d_getinfo(the_slice, title=None, xtitle=None, ytitle=None, ztitle=None):
     """
     Forms various title annotations based on the slice's metadata
     """
```

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_intrange.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_intrange.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_nearest.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_nearest.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_orientslice.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_orientslice.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_plot.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_plot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_rlog.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_rlog.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_rotate.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_rotate.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_s2c.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_s2c.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_smooth.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_smooth.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/slice2d_subtract.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/slice2d_subtract.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/spd_cal_rot.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/spd_cal_rot.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_slice2d/tplot_average.py` & `pyspedas-1.5.7/pyspedas/particles/spd_slice2d/tplot_average.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import numpy as np
-from pytplot import get_data
-from pyspedas import time_string
+from pytplot import get_data, time_string
 
 
 def tplot_average(tvar, trange, quiet=False):
     """
     Returns the average value of a tplot variable over a specified time range.
 
     Input
```

### Comparing `pyspedas-1.5.6/pyspedas/particles/spd_units_string.py` & `pyspedas-1.5.7/pyspedas/particles/spd_units_string.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/poes/__init__.py` & `pyspedas-1.5.7/pyspedas/poes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/poes/load.py` & `pyspedas-1.5.7/pyspedas/poes/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/polar/__init__.py` & `pyspedas-1.5.7/pyspedas/polar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/polar/load.py` & `pyspedas-1.5.7/pyspedas/polar/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/polar/tests/tests.py` & `pyspedas-1.5.7/pyspedas/stereo/tests/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,65 +2,68 @@
 import unittest
 from pytplot import data_exists
 import pyspedas
 
 
 class LoadTestCases(unittest.TestCase):
     def test_downloadonly(self):
-        files = pyspedas.polar.efi(downloadonly=True)
+        files = pyspedas.stereo.mag(trange=['2013-1-6', '2013-1-7'], downloadonly=True)
         self.assertTrue(os.path.exists(files[0]))
 
-    def test_load_mfe_data(self):
-        mfe_vars = pyspedas.polar.mfe(trange=['2003-10-28', '2003-10-29'], get_support_data=True)
-        self.assertTrue(data_exists('B_GSE'))
-        self.assertTrue(data_exists('B_GSM'))
-
-    def test_load_efi_data(self):
-        efi_vars = pyspedas.polar.efi(time_clip=True)
-        self.assertTrue(data_exists('ESPIN'))
-
-    def test_load_pwi_data(self):
-        pwi_vars = pyspedas.polar.pwi()
-        self.assertTrue(data_exists('Fce'))
-
-    def test_load_hydra_data(self):
-        hydra_vars = pyspedas.polar.hydra()
-        self.assertTrue(data_exists('ELE_DENSITY'))
-
-    def test_load_tide_data(self):
-        tide_vars = pyspedas.polar.tide()
-        self.assertTrue(data_exists('total_den'))
-        self.assertTrue(data_exists('total_v'))
-        self.assertTrue(data_exists('total_t'))
-
-    def test_load_timas_data(self):
-        timas_vars = pyspedas.polar.timas()
-        self.assertTrue(data_exists('Density_H'))
-
-    def test_load_cammice_data(self):
-        cammice_vars = pyspedas.polar.cammice()
-        self.assertTrue(data_exists('Protons'))
-
-    def test_load_ceppad_data(self):
-        ceppad_vars = pyspedas.polar.ceppad()
-        self.assertTrue(data_exists('IPS_10_ERR'))
-
-    def test_load_uvi_data(self):
-        uvi_vars = pyspedas.polar.uvi()
-        self.assertTrue(data_exists('IMAGE_DATA'))
-
-    def test_load_pixie_data(self):
-        pixie_vars = pyspedas.polar.pixie()
-        self.assertTrue(data_exists('TXF_HIGH'))
-
-    def test_load_vis_data(self):
-        vis_vars = pyspedas.polar.vis(notplot=True)
-        self.assertTrue('Image_Counts' in vis_vars)
-
-    def test_load_orbit_data(self):
-        orbit_vars = pyspedas.polar.orbit()
-        self.assertTrue(data_exists('AVG_SPIN_RATE'))
-        self.assertTrue(data_exists('SPIN_PHASE'))
-
+    def test_load_mag_data(self):
+        mag_vars = pyspedas.stereo.mag(trange=['2013-11-5', '2013-11-6'], time_clip=True)
+        self.assertTrue(data_exists('BFIELD'))
+        mag_vars = pyspedas.stereo.mag(trange=['2013-11-5', '2013-11-6'], datatype='32hz')
+        mag_vars = pyspedas.stereo.mag(trange=['2013-11-5', '2013-11-6'], notplot=True)
+        self.assertTrue('BFIELD' in mag_vars)
+
+    def test_load_swea_data(self):
+        swea_vars = pyspedas.stereo.swea(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('SWEASpectra'))
+
+    def test_load_ste_data(self):
+        ste_vars = pyspedas.stereo.ste(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('STE_spectra'))
+
+    def test_load_sept_data(self):
+        sept_vars = pyspedas.stereo.sept(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('Spec_0_E'))
+
+    def test_load_sit_data(self):
+        sit_vars = pyspedas.stereo.sit(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('H_Intensity'))
+
+    def test_load_let_data(self):
+        let_vars = pyspedas.stereo.let(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('H_Hi_sec_flux'))
+
+    def test_load_het_data(self):
+        het_vars = pyspedas.stereo.het(trange=['2013-1-5', '2013-1-6'], time_clip=True)
+        self.assertTrue(data_exists('Electron_Flux'))
+        self.assertTrue(data_exists('Proton_Flux'))
+
+    def test_load_plastic_data(self):
+        p_vars = pyspedas.stereo.plastic(trange=['2013-11-5', '2013-11-6'], probe='b')
+        self.assertTrue(data_exists('proton_number_density'))
+        self.assertTrue(data_exists('proton_bulk_speed'))
+        self.assertTrue(data_exists('proton_temperature'))
+
+    def test_load_waves_data_a(self):
+        w_vars = pyspedas.stereo.waves(trange=['2013-11-5', '2013-11-6'], probe='a')
+        self.assertTrue(data_exists('PSD_FLUX'))
+        self.assertTrue(data_exists('PSD_SFU'))
+
+    def test_load_waves_data_b(self):
+        w_vars = pyspedas.stereo.waves(trange=['2013-11-5', '2013-11-6'], probe='b')
+        self.assertTrue(data_exists('PSD_FLUX'))
+        self.assertTrue(data_exists('PSD_SFU'))
+
+    def test_load_beacon_data_a(self):
+        w_vars = pyspedas.stereo.beacon(trange=['2013-11-5', '2013-11-6'], probe='a')
+        self.assertTrue(data_exists('MAGBField'))
+
+    def test_load_beacon_data_b(self):
+        w_vars = pyspedas.stereo.beacon(trange=['2013-11-5', '2013-11-6'], probe='b')
+        self.assertTrue(data_exists('MAGBField'))
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/psp/__init__.py` & `pyspedas-1.5.7/pyspedas/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/psp/config.py` & `pyspedas-1.5.7/pyspedas/psp/config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/psp/filter.py` & `pyspedas-1.5.7/pyspedas/psp/filter.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/psp/load.py` & `pyspedas-1.5.7/pyspedas/psp/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         elif datatype in ['mag_rtn_4_per_cycle', 'mag_rtn_4_sa_per_cyc']:
             pathformat = instrument + '/' + level + '/mag_rtn_4_per_cycle/%Y/psp_fld_' + level + '_mag_rtn_4_sa_per_cyc_%Y%m%d_v??.cdf'
         elif datatype in ['mag_sc_4_per_cycle', 'mag_sc_4_sa_per_cyc']:
             pathformat = instrument + '/' + level + '/mag_sc_4_per_cycle/%Y/psp_fld_' + level + '_mag_sc_4_sa_per_cyc_%Y%m%d_v??.cdf'
         elif datatype == 'sqtn_rfs_v1v2':
             pathformat = instrument + '/' + level + '/' + datatype + '/%Y/psp_fld_' + level + '_' + datatype + '_%Y%m%d_v?.?.cdf'        
         elif datatype == 'rfs_lfr_qtn':
-            pathformat = instrument + '/' + level + '/' + datatype + '/%Y/psp_fld_' + level + '_' + datatype + '_%Y%m*_v??.cdf'
+            pathformat = instrument + '/' + level + '/' + datatype + '/psp_fld_' + level + '_' + datatype + '_%Y%m*_v??.cdf'
         elif datatype in ['dfb_dc_spec', 'dfb_ac_spec', 'dfb_dc_xspec', 'dfb_ac_xspec']:
             out_vars = []
             for item in spec_types:
                 loaded_data = load(trange=trange, instrument=instrument, datatype=datatype + '_' + item, level=level, 
                     suffix=suffix, get_support_data=get_support_data, varformat=varformat, varnames=varnames, 
                     downloadonly=downloadonly, notplot=notplot, time_clip=time_clip, no_update=no_update, last_version=last_version)
                 if loaded_data != []:
@@ -203,14 +203,16 @@
             # Generic SPDF path.  
             pathformat = instrument + '/' + level + '/' + datatype + '/%Y/psp_fld_' + level + '_' + datatype + '_%Y%m%d%H_v??.cdf'
             file_resolution = 6*3600.
 
         # Files on Berkeley server are stored in monthly directories 
         if username != None:
             pathformat = pathformat.replace('/%Y/psp_fld', '/%Y/%m/psp_fld')
+            if datatype == 'rfs_lfr_qtn':
+                pathformat = pathformat.replace('l3/rfs_lfr_qtn/', 'l3/rfs_lfr_qtn/%Y/%m/')
             if level == 'l1':
                 pathformat = pathformat.replace('psp_fld', 'spp_fld')
 
 
     elif instrument == 'spc':
         if username is None:
             prefix = 'psp_spc_'
```

### Comparing `pyspedas-1.5.6/pyspedas/psp/rfs.py` & `pyspedas-1.5.7/pyspedas/psp/rfs.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     out = []
     if len(files) == 0:
         return []
     # the variables should be the same across all files
     file = files[0]
     cdf_file = cdflib.CDF(file)
     cdf_info = cdf_file.cdf_info()
-    variables = cdf_info['rVariables'] + cdf_info['zVariables']
+    variables = cdf_info.rVariables + cdf_info.zVariables
     for variable in variables:
         if variable[0:7] != 'psp_fld':
             continue
         try:
             elements = cdf_file.varget(variable)
         except ValueError:
             continue
```

### Comparing `pyspedas-1.5.6/pyspedas/psp/tests/tests.py` & `pyspedas-1.5.7/pyspedas/psp/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/__init__.py` & `pyspedas-1.5.7/pyspedas/rbsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/load.py` & `pyspedas-1.5.7/pyspedas/rbsp/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_load_rbspice_read.py` & `pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_load_rbspice_read.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_omni.py` & `pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_omni.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad.py` & `pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad_spinavg.py` & `pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_spin_avg.py` & `pyspedas-1.5.7/pyspedas/rbsp/rbspice_lib/rbsp_rbspice_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/rbsp/tests/tests.py` & `pyspedas-1.5.7/pyspedas/rbsp/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/secs/__init__.py` & `pyspedas-1.5.7/pyspedas/secs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/secs/config.py` & `pyspedas-1.5.7/pyspedas/secs/config.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/secs/load.py` & `pyspedas-1.5.7/pyspedas/secs/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/secs/makeplots.py` & `pyspedas-1.5.7/pyspedas/secs/makeplots.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/soho/__init__.py` & `pyspedas-1.5.7/pyspedas/soho/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/soho/load.py` & `pyspedas-1.5.7/pyspedas/soho/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/soho/tests/tests.py` & `pyspedas-1.5.7/pyspedas/soho/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/solo/__init__.py` & `pyspedas-1.5.7/pyspedas/solo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/solo/load.py` & `pyspedas-1.5.7/pyspedas/solo/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/solo/tests/tests.py` & `pyspedas-1.5.7/pyspedas/solo/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/sosmag/load.py` & `pyspedas-1.5.7/pyspedas/sosmag/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/sosmag/tests/tests.py` & `pyspedas-1.5.7/pyspedas/sosmag/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/st5/__init__.py` & `pyspedas-1.5.7/pyspedas/st5/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/st5/load.py` & `pyspedas-1.5.7/pyspedas/st5/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/st5/tests/tests.py` & `pyspedas-1.5.7/pyspedas/st5/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/stereo/__init__.py` & `pyspedas-1.5.7/pyspedas/stereo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/stereo/load.py` & `pyspedas-1.5.7/pyspedas/stereo/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/swarm/__init__.py` & `pyspedas-1.5.7/pyspedas/swarm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,43 +5,46 @@
         probe='a',
         datatype='hr',
         level='l1b', 
         suffix='', 
         varnames=[],
         time_clip=False):
     """
-    This function loads data from the Vector Field Magnetometer (VFM)
-    
+    Loads data from the Vector Field Magnetometer (VFM).
+
     Parameters
     ----------
-        trange : list of str
-            time range of interest [starttime, endtime] with the format 
-            'YYYY-MM-DD','YYYY-MM-DD'] or to specify more or less than a day 
-            ['YYYY-MM-DD/hh:mm:ss','YYYY-MM-DD/hh:mm:ss']
-
-        probe: str or list of str
-            Swarm spacecraft ID ('a', 'b' and/or 'c')
-
-        datatype: str
-            Data type; Valid options:
-                'hr', 'lr'
-
-        level: str
-            Data level; options: 'l1b'
-
-        suffix: str
-            The tplot variable names will be given this suffix.  By default, 
-            no suffix is added.
-
-        varnames: list of str
-            List of variable names to load (if not specified,
-            all data variables are loaded)
-
-        time_clip: bool
-            Time clip the variables to exactly the range specified in the trange keyword
+    trange : list of str, default=['2017-03-27/06:00', '2017-03-27/08:00']
+        Time range of interest [starttime, endtime] with the format
+        'YYYY-MM-DD' or 'YYYY-MM-DD/hh:mm:ss'.
+    probe : str or list of str, default='a'
+        Swarm spacecraft ID ('a', 'b', and/or 'c').
+    datatype : str, default='hr'
+        Data type; valid options: 'hr' (high resolution), 'lr' (low resolution).
+    level : str, default='l1b'
+        Data level; options: 'l1b'.
+    suffix : str, optional
+        The tplot variable names will be given this suffix. By default, no suffix is added.
+    varnames : list of str, optional
+        List of variable names to load. If not specified, all data variables are loaded.
+    time_clip : bool, default=False
+        Time clip the variables to exactly the range specified in the trange keyword.
 
     Returns
-    ----------
+    -------
+    out_vars : list of str
         List of tplot variables created.
 
+    Examples
+    --------
+    To load and plot Magnetometer (MAG) data from the Swarm mission for probe 'c' over a specific time range, you can use the following commands:
+
+    >>> import pyspedas
+    >>> from pytplot import tplot
+
+    # Load MAG data for probe 'c'
+    >>> mag_vars = pyspedas.swarm.mag(probe='c', trange=['2017-03-27/06:00', '2017-03-27/08:00'], datatype='hr')
+
+    # Plot the loaded MAG data
+    >>> tplot('swarmc_B_VFM')
     """
     return load(instrument='mag', trange=trange, probe=probe, level=level, datatype=datatype, suffix=suffix, varnames=varnames, time_clip=time_clip)
```

### Comparing `pyspedas-1.5.6/pyspedas/themis/__init__.py` & `pyspedas-1.5.7/pyspedas/themis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/analysis/scpot2dens.py` & `pyspedas-1.5.7/pyspedas/themis/analysis/scpot2dens.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/common/check_args.py` & `pyspedas-1.5.7/pyspedas/themis/common/check_args.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/cotrans/dsl2gse.py` & `pyspedas-1.5.7/pyspedas/themis/cotrans/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/cotrans/gse2sse.py` & `pyspedas-1.5.7/pyspedas/themis/cotrans/gse2sse.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/cotrans/sse2sel.py` & `pyspedas-1.5.7/pyspedas/themis/cotrans/sse2sel.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/cotrans/ssl2dsl.py` & `pyspedas-1.5.7/pyspedas/themis/cotrans/ssl2dsl.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/ground/ask.py` & `pyspedas-1.5.7/pyspedas/themis/ground/ask.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/load.py` & `pyspedas-1.5.7/pyspedas/themis/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/efi.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/efi.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fbk.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fbk.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fft.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fft.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fgm.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fgm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/fit.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/fit.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/fields/scm.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/fields/scm.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/esa.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/esa.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/esd.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/esd.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/gmom.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/gmom.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/mom.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/mom.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/spacecraft/particles/sst.py` & `pyspedas-1.5.7/pyspedas/themis/spacecraft/particles/sst.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/apply_spinaxis_corrections.py` & `pyspedas-1.5.7/pyspedas/themis/state/apply_spinaxis_corrections.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/autoload_support.py` & `pyspedas-1.5.7/pyspedas/themis/state/autoload_support.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/slp.py` & `pyspedas-1.5.7/pyspedas/themis/state/slp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel.py` & `pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel_postprocess.py` & `pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/spinmodel/spinmodel_segment.py` & `pyspedas-1.5.7/pyspedas/themis/state/spinmodel/spinmodel_segment.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/state/state.py` & `pyspedas-1.5.7/pyspedas/themis/state/state.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/autoload_support_tests.py` & `pyspedas-1.5.7/pyspedas/themis/tests/autoload_support_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/test_cal_fit_tplot_metadata.py` & `pyspedas-1.5.7/pyspedas/themis/tests/test_cal_fit_tplot_metadata.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_cal_fit.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_cal_fit.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_dsl_cotrans.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_dsl_cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_lunar_cotrans.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_lunar_cotrans.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_scpot2dens.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_scpot2dens.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_spinmodel.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_spinmodel.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_state.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_state.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_themis_check_args.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_themis_check_args.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/tests_tplot_time.py` & `pyspedas-1.5.7/pyspedas/themis/tests/tests_tplot_time.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/validation/cal_fit_validation.py` & `pyspedas-1.5.7/pyspedas/themis/tests/validation/cal_fit_validation.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/themis/tests/validation/dsl2gse.py` & `pyspedas-1.5.7/pyspedas/themis/tests/validation/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/twins/__init__.py` & `pyspedas-1.5.7/pyspedas/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/twins/load.py` & `pyspedas-1.5.7/pyspedas/twins/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/twins/tests/tests.py` & `pyspedas-1.5.7/pyspedas/twins/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/ulysses/__init__.py` & `pyspedas-1.5.7/pyspedas/ulysses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/ulysses/load.py` & `pyspedas-1.5.7/pyspedas/ulysses/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/dailynames.py` & `pyspedas-1.5.7/pyspedas/utilities/dailynames.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/datasets.py` & `pyspedas-1.5.7/pyspedas/utilities/datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 from cdasws import CdasWs
 
 
-def find_datasets(mission=None, instrument=None, label=False):
+def find_datasets(mission=None, instrument=None, label=False, quiet=False):
     """
     Find datasets from the Coordinated Data Analysis System (CDAS) based on mission and/or instrument criteria.
 
     This function queries the CDAS for datasets, optionally filtering by mission and instrument. It can
     also display labels for the datasets.
 
     Parameters
     ----------
     mission : str, optional
         The name of the mission to filter the datasets. If None, datasets are not filtered by mission.
     instrument : str, optional
         The name of the instrument to filter the datasets. If None, datasets are not filtered by instrument.
     label : bool, default=False
         If True, the function prints both the dataset ID and label. If False, only the dataset ID is printed.
+    quiet: bool, default=False
+        If True, suppresses printing of dataset IDs (and labels) found
 
     Returns
     -------
-    None
-        This function does not return any value. It prints the dataset IDs, and optionally labels, to the console.
+    list of str
+        List of datasets found
 
     Examples
     --------
+    >>> from pyspedas import find_datasets
     >>> find_datasets(mission='MMS', instrument='FGM')
     MMS1_FGM_BRST_L2
     MMS1_FGM_SRVY_L2
     ...
 
-    >>> find_datasets(mission='MMS', label=True)
-    MMS1_ASPOC_SRVY_L2: Level 2 Active Spacecraft Potential Control Survey Data - K. Torkar, R. Nakamura (IWF)
-    ...
+    # Suppress printed output
+    >>> from pyspedas import find_datasets
+    >>> mms_list = find_datasets(mission='MMS', quiet=True)
+    >>> print(mms_list[0:3])
+
     """
 
     cdas = CdasWs()
     datasets = cdas.get_datasets(observatoryGroup=mission)
+    output_list = []
     for index, dataset in enumerate(datasets):
         if instrument is not None:
             if instrument.upper() not in dataset['Id']:
                 continue
         if label:
-            print(dataset['Id'] + ': ' + dataset['Label'])
+            if not quiet:
+                print(dataset['Id'] + ': ' + dataset['Label'])
         else:
-            print(dataset['Id'])
+            if not quiet:
+                print(dataset['Id'])
+        output_list.append(dataset['Id'])
+    return output_list
```

### Comparing `pyspedas-1.5.6/pyspedas/utilities/download.py` & `pyspedas-1.5.7/pyspedas/utilities/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pathlib import Path
 from shutil import copyfileobj, copy
 from tempfile import NamedTemporaryFile
 from html.parser import HTMLParser
 from netCDF4 import Dataset
 from cdflib import CDF
-
+from time import sleep
 
 # the following is used to parse the links from an HTML index file
 class LinkParser(HTMLParser):
     def handle_starttag(self, tag, attrs):
         if tag == 'a':
             attrs = {k: v for (k, v) in attrs}
             if 'href' in attrs:
@@ -305,14 +305,18 @@
         except pkg_resources.DistributionNotFound:
             release_version = 'bleeding edge'
         headers['User-Agent'] = 'pySPEDAS ' + release_version
 
     out = []
     index_table = {}
 
+    # To avoid hammering the remote server with repeated failing requests, if we have a problem with an index
+    # URL we'll add it to bad_index_set and skip it if it comes up again.
+    bad_index_set = set()
+
     if not isinstance(remote_file, list):
         remote_file = [remote_file]
 
     urls = [remote_path+rfile for rfile in remote_file]
 
     for url in urls:
         resp_data = None
@@ -335,34 +339,46 @@
         short_path = local_file[:1+local_file.rfind("/")]
 
         if not no_download:
             # expand the wildcards in the url
             if ('?' in url or '*' in url or regex) and (not no_download and not no_wildcards):
                 if index_table.get(url_base) is not None:
                     links = index_table[url_base]
+                elif url_base in bad_index_set:
+                    logging.info('Skipping remote index: ' + url_base + ' (previous attempt failed)')
+                    continue
                 else:
                     logging.info('Downloading remote index: ' + url_base)
 
                     # we'll need to parse the HTML index file for the file list
                     with warnings.catch_warnings():
                         warnings.simplefilter("ignore", category=ResourceWarning)
                         try:
                             if not basic_auth:
                                 html_index = session.get(url_base, verify=verify, headers=headers)
                             else:
                                 html_index = session.get(url_base, verify=verify, headers=headers, auth=(username, password))
                         except requests.exceptions.ConnectionError:
+                            # Add this index to bad_index_set and cool down a bit
+                            bad_index_set.add(url_base)
+                            sleep(2)
                             continue
 
                     if html_index.status_code == 404:
                         logging.error('Remote index not found: ' + url_base)
+                        # Add this index to bad_index_set and cool down a bit
+                        bad_index_set.add(url_base)
+                        sleep(2)
                         continue
 
                     if html_index.status_code == 401 or html_index.status_code == 403:
                         logging.error('Unauthorized: ' + url_base)
+                        # Add this index to bad_index_set and cool down a bit
+                        bad_index_set.add(url_base)
+                        sleep(2)
                         continue
 
                     # grab the links
                     link_parser = LinkParser()
                     link_parser.feed(html_index.text)
 
                     try:
```

### Comparing `pyspedas-1.5.6/pyspedas/utilities/download_ftp.py` & `pyspedas-1.5.7/pyspedas/utilities/download_ftp.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/interpol.py` & `pyspedas-1.5.7/pyspedas/utilities/interpol.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/leap_seconds.py` & `pyspedas-1.5.7/pyspedas/utilities/leap_seconds.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/libs.py` & `pyspedas-1.5.7/pyspedas/utilities/libs.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/mpause_2.py` & `pyspedas-1.5.7/pyspedas/utilities/mpause_2.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/mpause_t96.py` & `pyspedas-1.5.7/pyspedas/utilities/mpause_t96.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/spice/time_ephemeris.py` & `pyspedas-1.5.7/pyspedas/utilities/spice/time_ephemeris.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/tcopy.py` & `pyspedas-1.5.7/pyspedas/utilities/tcopy.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/tests/download_tests.py` & `pyspedas-1.5.7/pyspedas/utilities/tests/download_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/tests/libs_tests.py` & `pyspedas-1.5.7/pyspedas/utilities/tests/libs_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/utilities/tests/misc_tests.py` & `pyspedas-1.5.7/pyspedas/utilities/tests/misc_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,20 +103,9 @@
         pytplot.time_clip('tst1',1.5,2.5,new_names=None, suffix='-tc4')
         self.assertTrue(data_exists('tst1-tc4'))
         # no such tplot name
         pytplot.time_clip('bogus',1.5,2.5)
         # empty input list
         pytplot.time_clip([],1.5,2.5)
 
-
-
-    @unittest.skip('Skipping line plot pseudovariables test')
-    def test_line_pseudovariables(self):
-        themis.fgm(probe='c')
-        store_data('comb_3_1',data=['thc_fge_dsl','thc_fge_btotal'])
-        store_data('comb_1_3',data=['thc_fge_btotal','thc_fge_dsl'])
-        tplot(['thc_fge_dsl','thc_fge_btotal','comb_3_1','comb_1_3'])
-        tplot('comb_1_3')
-        tplot('comb_3_1') # only plots 1 trace JWL 2024-02-19
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyspedas-1.5.6/pyspedas/utilities/tests/time_tests.py` & `pyspedas-1.5.7/pyspedas/utilities/tests/time_tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/vires/load.py` & `pyspedas-1.5.7/pyspedas/vires/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/wind/load.py` & `pyspedas-1.5.7/pyspedas/wind/load.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas/wind/tests/tests.py` & `pyspedas-1.5.7/pyspedas/wind/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyspedas-1.5.6/pyspedas.egg-info/PKG-INFO` & `pyspedas-1.5.7/pyspedas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyspedas
-Version: 1.5.6
+Version: 1.5.7
 Summary: Python Space Physics Environment Data Analysis Software (pySPEDAS)
 Home-page: https://github.com/spedas/pyspedas
 Author: Jim Lewis
 Author-email: jwl@ssl.berkeley.edu
 License: MIT
 Project-URL: Information, http://spedas.org/wiki/
 Keywords: spedas data tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # PySPEDAS
 [![build](https://github.com/spedas/pyspedas/workflows/build/badge.svg)](https://github.com/spedas/pyspedas/actions)
 [![Coverage Status](https://coveralls.io/repos/github/spedas/pyspedas/badge.svg)](https://coveralls.io/github/spedas/pyspedas)
@@ -62,15 +62,15 @@
 - [Ulysses](https://pyspedas.readthedocs.io/en/latest/ulysses.html)
 - [Van Allen Probes (RBSP)](https://pyspedas.readthedocs.io/en/latest/rbsp.html)
 - [Wind](https://pyspedas.readthedocs.io/en/latest/wind.html)
 
 
 ## Requirements
 
-Python 3.8+ is required.
+Python 3.9+ is required.
 
 We recommend [Anaconda](https://www.continuum.io/downloads/) which comes with a suite of packages useful for scientific data analysis. Step-by-step instructions for installing Anaconda can be found at: [Windows](https://docs.anaconda.com/anaconda/install/windows/), [macOS](https://docs.anaconda.com/anaconda/install/mac-os/), [Linux](https://docs.anaconda.com/anaconda/install/linux/)
 
 
 ## Installation
 
 ### Virtual Environment
```

### Comparing `pyspedas-1.5.6/pyspedas.egg-info/SOURCES.txt` & `pyspedas-1.5.7/pyspedas.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 pyspedas/erg/ground/riometer/__init__.py
 pyspedas/erg/ground/riometer/isee_brio.py
 pyspedas/erg/ground/vlf/__init__.py
 pyspedas/erg/ground/vlf/isee_vlf.py
 pyspedas/erg/satellite/__init__.py
 pyspedas/erg/satellite/erg/__init__.py
 pyspedas/erg/satellite/erg/config.py
+pyspedas/erg/satellite/erg/get_gatt_ror.py
 pyspedas/erg/satellite/erg/load.py
 pyspedas/erg/satellite/erg/att/__init__.py
 pyspedas/erg/satellite/erg/att/att.py
 pyspedas/erg/satellite/erg/common/__init__.py
 pyspedas/erg/satellite/erg/common/cotrans/__init__.py
 pyspedas/erg/satellite/erg/common/cotrans/cart_trans_matrix_make.py
 pyspedas/erg/satellite/erg/common/cotrans/dsi2j2000.py
@@ -210,14 +211,15 @@
 pyspedas/erg/satellite/erg/pwe/pwe_efd.py
 pyspedas/erg/satellite/erg/pwe/pwe_hfa.py
 pyspedas/erg/satellite/erg/pwe/pwe_ofa.py
 pyspedas/erg/satellite/erg/pwe/pwe_wfc.py
 pyspedas/erg/satellite/erg/xep/__init__.py
 pyspedas/erg/satellite/erg/xep/xep.py
 pyspedas/erg/tests/__init__.py
+pyspedas/erg/tests/ground_tests.py
 pyspedas/erg/tests/tests.py
 pyspedas/fast/__init__.py
 pyspedas/fast/config.py
 pyspedas/fast/load.py
 pyspedas/fast/tests/__init__.py
 pyspedas/fast/tests/tests.py
 pyspedas/geopack/__init__.py
@@ -289,15 +291,14 @@
 pyspedas/mms/mms_load_brst_segments.py
 pyspedas/mms/mms_load_data.py
 pyspedas/mms/mms_load_data_spdf.py
 pyspedas/mms/mms_load_fast_segments.py
 pyspedas/mms/mms_load_sroi_segments.py
 pyspedas/mms/mms_login_lasp.py
 pyspedas/mms/mms_orbit_plot.py
-pyspedas/mms/mms_overview_plot.py
 pyspedas/mms/mms_python_startup.py
 pyspedas/mms/mms_tai2unix.py
 pyspedas/mms/mms_update_brst_intervals.py
 pyspedas/mms/print_vars.py
 pyspedas/mms/spd_mms_load_bss.py
 pyspedas/mms/aspoc/__init__.py
 pyspedas/mms/aspoc/aspoc.py
@@ -345,41 +346,45 @@
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220113.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220506.csv
 pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20220815.csv
+pyspedas/mms/feeps/sun/MMS1_FEEPS_ContaminatedSectors_20240202.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220113.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220506.csv
 pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20220815.csv
+pyspedas/mms/feeps/sun/MMS2_FEEPS_ContaminatedSectors_20240202.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220113.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220506.csv
 pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20220815.csv
+pyspedas/mms/feeps/sun/MMS3_FEEPS_ContaminatedSectors_20240202.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220113.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220506.csv
 pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20220815.csv
+pyspedas/mms/feeps/sun/MMS4_FEEPS_ContaminatedSectors_20240202.csv
 pyspedas/mms/fgm/__init__.py
 pyspedas/mms/fgm/fgm.py
 pyspedas/mms/fgm/mms_curl.py
 pyspedas/mms/fgm/mms_fgm_remove_flags.py
 pyspedas/mms/fgm/mms_fgm_set_metadata.py
 pyspedas/mms/fgm/mms_lingradest.py
 pyspedas/mms/fgm/mms_split_fgm_data.py
@@ -427,14 +432,16 @@
 pyspedas/mms/particles/mms_pgs_clean_support.py
 pyspedas/mms/particles/mms_pgs_make_e_spec.py
 pyspedas/mms/particles/mms_pgs_make_fac.py
 pyspedas/mms/particles/mms_pgs_make_phi_spec.py
 pyspedas/mms/particles/mms_pgs_make_theta_spec.py
 pyspedas/mms/particles/mms_pgs_split_hpca.py
 pyspedas/mms/particles/moka_mms_clean_data.py
+pyspedas/mms/plots/__init__.py
+pyspedas/mms/plots/mms_overview_plot.py
 pyspedas/mms/scm/__init__.py
 pyspedas/mms/scm/mms_scm_set_metadata.py
 pyspedas/mms/scm/scm.py
 pyspedas/mms/tests/__init__.py
 pyspedas/mms/tests/cotrans.py
 pyspedas/mms/tests/curlometer.py
 pyspedas/mms/tests/data_rate_segments.py
@@ -443,14 +450,15 @@
 pyspedas/mms/tests/feeps.py
 pyspedas/mms/tests/file_filter.py
 pyspedas/mms/tests/fpi_tests.py
 pyspedas/mms/tests/load_routine_tests.py
 pyspedas/mms/tests/mms_part_getspec.py
 pyspedas/mms/tests/neutral_sheet.py
 pyspedas/mms/tests/orbit_plots.py
+pyspedas/mms/tests/overview_plots.py
 pyspedas/mms/tests/ql_l1b_sitl_tests.py
 pyspedas/mms/tests/setup_tests.py
 pyspedas/mms/tests/slice2d.py
 pyspedas/mms/tests/wavpol.py
 pyspedas/noaa/__init__.py
 pyspedas/noaa/config.py
 pyspedas/noaa/noaa_load_kp.py
@@ -625,26 +633,29 @@
 pyspedas/ulysses/tests/__init__.py
 pyspedas/ulysses/tests/tests.py
 pyspedas/utilities/__init__.py
 pyspedas/utilities/dailynames.py
 pyspedas/utilities/datasets.py
 pyspedas/utilities/download.py
 pyspedas/utilities/download_ftp.py
+pyspedas/utilities/find_ip_address.py
 pyspedas/utilities/interpol.py
 pyspedas/utilities/leap_seconds.py
 pyspedas/utilities/libs.py
 pyspedas/utilities/mpause_2.py
 pyspedas/utilities/mpause_t96.py
 pyspedas/utilities/tcopy.py
 pyspedas/utilities/spice/__init__.py
 pyspedas/utilities/spice/time_ephemeris.py
 pyspedas/utilities/tests/__init__.py
 pyspedas/utilities/tests/download_tests.py
 pyspedas/utilities/tests/libs_tests.py
 pyspedas/utilities/tests/misc_tests.py
+pyspedas/utilities/tests/plot_tests.py
+pyspedas/utilities/tests/test_find_ip_address.py
 pyspedas/utilities/tests/time_tests.py
 pyspedas/vires/__init__.py
 pyspedas/vires/config.py
 pyspedas/vires/load.py
 pyspedas/wind/__init__.py
 pyspedas/wind/config.py
 pyspedas/wind/load.py
```

### Comparing `pyspedas-1.5.6/setup.py` & `pyspedas-1.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 # To use a consistent encols distding
 from codecs import open
 
 setup(
     name="pyspedas",
-    version="1.5.6",
+    version="1.5.7",
     description="Python Space Physics Environment Data Analysis Software (pySPEDAS)",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/spedas/pyspedas",
     author="Jim Lewis",
     author_email="jwl@ssl.berkeley.edu",
     license="MIT",
@@ -35,13 +35,13 @@
         "scipy",
         "cdflib<1.0.0",
         "cdasws>=1.7.24",
         "netCDF4>=1.6.2",
         "pywavelets",
         "astropy",
         "hapiclient>=0.2.2",
-        "pytplot-mpl-temp>=2.2.6",
+        "pytplot-mpl-temp>=2.2.8",
         "viresclient",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     include_package_data=True,
 )
```

