# Comparing `tmp/libcnmc-24.8.1.tar.gz` & `tmp/libcnmc-24.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcnmc-24.8.1.tar", last modified: Thu Apr  4 12:01:20 2024, max compression
+gzip compressed data, was "dist/libcnmc-24.8.2.tar", last modified: Fri Apr  5 10:20:50 2024, max compression
```

## Comparing `libcnmc-24.8.1.tar` & `libcnmc-24.8.2.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 12:01:02.000000 libcnmc-24.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 12:01:02.000000 libcnmc-24.8.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/res_4667/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/PRO.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/RES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/MACRO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/RES_CCAA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/CT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/FIA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4667/Otros.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/core/cnmc_inventari.py
--rw-r--r--   0 runner    (1001) docker     (127)    28273 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_4_2015.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18257 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/res_4771/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/SUB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/INV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4771/FIA.py
--rw-r--r--   0 runner    (1001) docker     (127)    38513 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/models/res_4667/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/pro_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/macro_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f1_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f6_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f3_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f4_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f8_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f2_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/resumen_ccaa_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f5_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/resumen_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4667/f7_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/models/res_4771/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f1_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f8_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f6_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f3_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f7_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f5_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f4_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4771/f2_4771.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/models/res_4666/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f5_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f6_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f8_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f4_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f1_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f2_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f7_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4666/f3_4666.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/cnmcmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/models/res_4131/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f1_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f2_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f4_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f3_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f5_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f8_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f6_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/models/res_4131/f7_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_4667.py
--rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_6181.py
--rw-r--r--   0 runner    (1001) docker     (127)    16843 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_4131.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_4666.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/audit_6181/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/FIA.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/audit_6181/SE.py
--rw-r--r--   0 runner    (1001) docker     (127)    45750 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    52793 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cli_8_2021.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/res_4603/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/update_cinis_trafo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/create_celles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/CINIMAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/SUB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/CINIPOS.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/update_cts_cinis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/INV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/update_trams_cinis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4603/FIA.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F13bis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F1bis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/create_celles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F9.py
--rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F11.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F13C.py
--rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F1.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F10AT.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F16.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F12.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F14.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F15.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F10BT.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F20.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2015/F12bis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/res_4666/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/AUD_LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/MOD.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/SUB.py
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/AUD_LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/AUD_POS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/AUD_CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/CON.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/FIA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4666/AUD_FIA.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FA5.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB7.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC1.py
--rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB6.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB1_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB2_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB2_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FA3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC4.py
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB8.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48519 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB9.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC6.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC5.py
--rw-r--r--   0 runner    (1001) docker     (127)    22907 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FD1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FD2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FA2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FF1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC7.py
--rw-r--r--   0 runner    (1001) docker     (127)    33027 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FA1.py
--rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_3.py
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FB4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FC3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_8_2021/FA4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/cir_3_2015/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_3_2015/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_3_2015/F3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/res_4131/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20902 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/POS.py
--rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/LAT.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/SUB.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/CTS.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/MAQ.py
--rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/LBT.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/DES.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/CON.py
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/res_4131/FIA.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:01:20.000000 libcnmc-24.8.1/libcnmc/cir_4_2014/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2014/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2014/F1bis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2014/F11.py
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-04 12:01:02.000000 libcnmc-24.8.1/libcnmc/cir_4_2014/F1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-04 12:01:02.000000 libcnmc-24.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:01:20.000000 libcnmc-24.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 12:01:02.000000 libcnmc-24.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 12:01:02.000000 libcnmc-24.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-04 12:01:20.000000 libcnmc-24.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 10:20:38.000000 libcnmc-24.8.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 10:20:38.000000 libcnmc-24.8.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/res_4667/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/PRO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/RES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/MACRO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/RES_CCAA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/CT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4667/Otros.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/core/cnmc_inventari.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28273 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_4_2015.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18257 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/res_4771/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/INV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4771/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38513 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/models/res_4667/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/pro_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/macro_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f1_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f6_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f3_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f4_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f8_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f2_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/resumen_ccaa_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f5_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/resumen_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4667/f7_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/models/res_4771/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f1_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f8_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f6_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f3_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f7_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f5_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f4_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4771/f2_4771.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/models/res_4666/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f5_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f6_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f8_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f4_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f1_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f2_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f7_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4666/f3_4666.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/cnmcmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/models/res_4131/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f1_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f2_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f4_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f3_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f5_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f8_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f6_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/models/res_4131/f7_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_4667.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_6181.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16843 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_4131.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_4666.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/audit_6181/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/audit_6181/SE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45750 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52793 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cli_8_2021.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/res_4603/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/update_cinis_trafo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/create_celles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/CINIMAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/CINIPOS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/update_cts_cinis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/INV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/update_trams_cinis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4603/FIA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F13bis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F1bis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/create_celles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F9.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F13C.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F10AT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F10BT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2015/F12bis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/res_4666/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/AUD_LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/MOD.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/AUD_LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/AUD_POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/AUD_CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/CON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/FIA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4666/AUD_FIA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FA5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48801 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22262 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB1_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB2_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB2_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FA3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48519 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22907 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FD1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FD2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FA2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FF1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FA1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20491 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FB4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FC3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_8_2021/FA4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/cir_3_2015/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_3_2015/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_3_2015/F3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/res_4131/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20902 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/POS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/LAT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/SUB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/CTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/MAQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/LBT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/DES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/CON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/res_4131/FIA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:20:50.000000 libcnmc-24.8.2/libcnmc/cir_4_2014/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2014/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2014/F1bis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2014/F11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-05 10:20:38.000000 libcnmc-24.8.2/libcnmc/cir_4_2014/F1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-05 10:20:38.000000 libcnmc-24.8.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:20:50.000000 libcnmc-24.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-05 10:20:38.000000 libcnmc-24.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 10:20:38.000000 libcnmc-24.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 10:20:50.000000 libcnmc-24.8.2/PKG-INFO
```

### Comparing `libcnmc-24.8.1/libcnmc.egg-info/SOURCES.txt` & `libcnmc-24.8.2/libcnmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/PRO.py` & `libcnmc-24.8.2/libcnmc/res_4667/PRO.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/RES.py` & `libcnmc-24.8.2/libcnmc/res_4667/RES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/MACRO.py` & `libcnmc-24.8.2/libcnmc/res_4667/MACRO.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/RES_CCAA.py` & `libcnmc-24.8.2/libcnmc/res_4667/RES_CCAA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/POS.py` & `libcnmc-24.8.2/libcnmc/res_4667/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/LAT.py` & `libcnmc-24.8.2/libcnmc/res_4667/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/CT.py` & `libcnmc-24.8.2/libcnmc/res_4667/CT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/MAQ.py` & `libcnmc-24.8.2/libcnmc/res_4667/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/LBT.py` & `libcnmc-24.8.2/libcnmc/res_4667/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/DES.py` & `libcnmc-24.8.2/libcnmc/res_4667/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/FIA.py` & `libcnmc-24.8.2/libcnmc/res_4667/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4667/Otros.py` & `libcnmc-24.8.2/libcnmc/res_4667/Otros.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/core/__init__.py` & `libcnmc-24.8.2/libcnmc/core/__init__.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/core/backend.py` & `libcnmc-24.8.2/libcnmc/core/backend.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/core/cnmc_inventari.py` & `libcnmc-24.8.2/libcnmc/core/cnmc_inventari.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_4_2015.py` & `libcnmc-24.8.2/libcnmc/cli_4_2015.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/utils.py` & `libcnmc-24.8.2/libcnmc/utils.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/POS.py` & `libcnmc-24.8.2/libcnmc/res_4771/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/LAT.py` & `libcnmc-24.8.2/libcnmc/res_4771/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/SUB.py` & `libcnmc-24.8.2/libcnmc/res_4771/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/CTS.py` & `libcnmc-24.8.2/libcnmc/res_4771/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/MAQ.py` & `libcnmc-24.8.2/libcnmc/res_4771/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/LBT.py` & `libcnmc-24.8.2/libcnmc/res_4771/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/INV.py` & `libcnmc-24.8.2/libcnmc/res_4771/INV.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/DES.py` & `libcnmc-24.8.2/libcnmc/res_4771/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4771/FIA.py` & `libcnmc-24.8.2/libcnmc/res_4771/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/checker.py` & `libcnmc-24.8.2/libcnmc/checker.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/pro_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/pro_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/macro_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/macro_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f1_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f1_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f6_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f6_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f3_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f3_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f4_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f4_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f8_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f8_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f2_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f2_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/resumen_ccaa_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/resumen_ccaa_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f5_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f5_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/resumen_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/resumen_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4667/f7_4667.py` & `libcnmc-24.8.2/libcnmc/models/res_4667/f7_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/__init__.py` & `libcnmc-24.8.2/libcnmc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f1_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f1_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f8_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f8_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f6_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f6_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f3_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f3_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f7_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f7_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f5_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f5_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f4_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f4_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4771/f2_4771.py` & `libcnmc-24.8.2/libcnmc/models/res_4771/f2_4771.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/fields.py` & `libcnmc-24.8.2/libcnmc/models/fields.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f5_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f5_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f6_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f6_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f8_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f8_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f4_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f4_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f1_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f1_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f2_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f2_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f7_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f7_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4666/f3_4666.py` & `libcnmc-24.8.2/libcnmc/models/res_4666/f3_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/cnmcmodel.py` & `libcnmc-24.8.2/libcnmc/models/cnmcmodel.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f1_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f1_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f2_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f2_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f4_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f4_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f3_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f3_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f5_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f5_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f8_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f8_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f6_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f6_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/models/res_4131/f7_4131.py` & `libcnmc-24.8.2/libcnmc/models/res_4131/f7_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_4667.py` & `libcnmc-24.8.2/libcnmc/cli_4667.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_6181.py` & `libcnmc-24.8.2/libcnmc/cli_6181.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_4131.py` & `libcnmc-24.8.2/libcnmc/cli_4131.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_4666.py` & `libcnmc-24.8.2/libcnmc/cli_4666.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/POS.py` & `libcnmc-24.8.2/libcnmc/audit_6181/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/LAT.py` & `libcnmc-24.8.2/libcnmc/audit_6181/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/CTS.py` & `libcnmc-24.8.2/libcnmc/audit_6181/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/MAQ.py` & `libcnmc-24.8.2/libcnmc/audit_6181/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/LBT.py` & `libcnmc-24.8.2/libcnmc/audit_6181/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/DES.py` & `libcnmc-24.8.2/libcnmc/audit_6181/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/FIA.py` & `libcnmc-24.8.2/libcnmc/audit_6181/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/audit_6181/SE.py` & `libcnmc-24.8.2/libcnmc/audit_6181/SE.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli.py` & `libcnmc-24.8.2/libcnmc/cli.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cli_8_2021.py` & `libcnmc-24.8.2/libcnmc/cli_8_2021.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/POS.py` & `libcnmc-24.8.2/libcnmc/res_4603/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/LAT.py` & `libcnmc-24.8.2/libcnmc/res_4603/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/create_celles.py` & `libcnmc-24.8.2/libcnmc/res_4603/create_celles.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/CINIMAQ.py` & `libcnmc-24.8.2/libcnmc/res_4603/CINIMAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/SUB.py` & `libcnmc-24.8.2/libcnmc/res_4603/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/CTS.py` & `libcnmc-24.8.2/libcnmc/res_4603/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/MAQ.py` & `libcnmc-24.8.2/libcnmc/res_4603/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/LBT.py` & `libcnmc-24.8.2/libcnmc/res_4603/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/CINIPOS.py` & `libcnmc-24.8.2/libcnmc/res_4603/CINIPOS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/INV.py` & `libcnmc-24.8.2/libcnmc/res_4603/INV.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/DES.py` & `libcnmc-24.8.2/libcnmc/res_4603/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4603/FIA.py` & `libcnmc-24.8.2/libcnmc/res_4603/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F13bis.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F13bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F1bis.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F1bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F13.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F13.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/create_celles.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/create_celles.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F9.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F9.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F11.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F11.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F13C.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F13C.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F1.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F10AT.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F10AT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F16.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F16.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F12.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F12.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F14.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F14.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F15.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F15.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F10BT.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F10BT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F20.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F20.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2015/F12bis.py` & `libcnmc-24.8.2/libcnmc/cir_4_2015/F12bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/AUD_LAT.py` & `libcnmc-24.8.2/libcnmc/res_4666/AUD_LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/POS.py` & `libcnmc-24.8.2/libcnmc/res_4666/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/MOD.py` & `libcnmc-24.8.2/libcnmc/res_4666/MOD.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/LAT.py` & `libcnmc-24.8.2/libcnmc/res_4666/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/SUB.py` & `libcnmc-24.8.2/libcnmc/res_4666/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/CTS.py` & `libcnmc-24.8.2/libcnmc/res_4666/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/MAQ.py` & `libcnmc-24.8.2/libcnmc/res_4666/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/LBT.py` & `libcnmc-24.8.2/libcnmc/res_4666/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/AUD_LBT.py` & `libcnmc-24.8.2/libcnmc/res_4666/AUD_LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/AUD_POS.py` & `libcnmc-24.8.2/libcnmc/res_4666/AUD_POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/DES.py` & `libcnmc-24.8.2/libcnmc/res_4666/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/AUD_CTS.py` & `libcnmc-24.8.2/libcnmc/res_4666/AUD_CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/CON.py` & `libcnmc-24.8.2/libcnmc/res_4666/CON.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/FIA.py` & `libcnmc-24.8.2/libcnmc/res_4666/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4666/AUD_FIA.py` & `libcnmc-24.8.2/libcnmc/res_4666/AUD_FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FA5.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FA5.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/__init__.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/__init__.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB7.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB7.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB6.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB6.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB1_1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB1_1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB2_1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB2_1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB2_2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB2_2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FA3.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FA3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC4.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC4.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB8.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB8.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB9.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB9.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC6.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC6.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB3.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC5.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC5.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB5.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB5.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FD1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FD1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FD2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FD2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FA2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FA2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FF1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FF1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC7.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC7.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FA1.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FA1.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,18 +722,19 @@
                         ('cups_id', '=', cups['id']),
                         '|', '|', '|',
                         '&', ('data', '=', False), ('data_vigencia', '=', False),
                         '&', ('data', '<=', current_date), ('data_vigencia', '=', False),
                         '&', ('data', '=', False), ('data_vigencia', '>=', current_date),
                         '&', ('data', '<=', current_date), ('data_vigencia', '>=', current_date),
                     ], 0, 0, False, {'active_test': False})
-                    o_pot_ads = max(
-                        b['pot_max_admisible']
-                        for b in self.connection.GiscedataButlleti.read(but_ids, ['pot_max_admisible'])
-                    )
+                    if but_ids:
+                        o_pot_ads = max(
+                            b['pot_max_admisible']
+                            for b in self.connection.GiscedataButlleti.read(but_ids, ['pot_max_admisible'])
+                        )
                 if o_pot_ads < o_potencia:
                     o_pot_ads = o_potencia
 
                 res_srid = ['', '']
                 if vertex:
                     res_srid = convert_srid(
                         get_srid(O), (vertex['x'], vertex['y'])
```

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB2.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB2.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB3_3.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB3_3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FB4.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FB4.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FC3.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FC3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_8_2021/FA4.py` & `libcnmc-24.8.2/libcnmc/cir_8_2021/FA4.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_3_2015/F3.py` & `libcnmc-24.8.2/libcnmc/cir_3_2015/F3.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/POS.py` & `libcnmc-24.8.2/libcnmc/res_4131/POS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/LAT.py` & `libcnmc-24.8.2/libcnmc/res_4131/LAT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/SUB.py` & `libcnmc-24.8.2/libcnmc/res_4131/SUB.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/CTS.py` & `libcnmc-24.8.2/libcnmc/res_4131/CTS.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/MAQ.py` & `libcnmc-24.8.2/libcnmc/res_4131/MAQ.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/LBT.py` & `libcnmc-24.8.2/libcnmc/res_4131/LBT.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/DES.py` & `libcnmc-24.8.2/libcnmc/res_4131/DES.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/CON.py` & `libcnmc-24.8.2/libcnmc/res_4131/CON.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/res_4131/FIA.py` & `libcnmc-24.8.2/libcnmc/res_4131/FIA.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2014/F1bis.py` & `libcnmc-24.8.2/libcnmc/cir_4_2014/F1bis.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2014/F11.py` & `libcnmc-24.8.2/libcnmc/cir_4_2014/F11.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/libcnmc/cir_4_2014/F1.py` & `libcnmc-24.8.2/libcnmc/cir_4_2014/F1.py`

 * *Files identical despite different names*

### Comparing `libcnmc-24.8.1/setup.py` & `libcnmc-24.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     INSTALL_REQUIRES += ['multiprocessing']
 
 setup(name='libcnmc',
       description='Generació fitxers CNMC',
       author='GISCE-TI, S.L.',
       author_email='devel@gisce.net',
       url='http://www.gisce.net',
-      version='24.8.1',
+      version='24.8.2',
       license='General Public Licence 2',
       long_description='''Long description''',
       provides=['libcnmc'],
       install_requires=INSTALL_REQUIRES,
       tests_require=TESTS_REQUIRE,
       packages=find_packages(exclude=['tests']),
       dependency_links=DEPENDENCY_LINKS,
```

