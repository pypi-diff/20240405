# Comparing `tmp/Fragmenstein-1.0.1.tar.gz` & `tmp/Fragmenstein-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fragmenstein-1.0.1.tar", last modified: Thu Feb 22 13:28:39 2024, max compression
+gzip compressed data, was "Fragmenstein-1.0.2.tar", last modified: Wed Mar 13 13:41:26 2024, max compression
```

## Comparing `Fragmenstein-1.0.1.tar` & `Fragmenstein-1.0.2.tar`

### file list

```diff
@@ -1,720 +1,720 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:39.132345 Fragmenstein-1.0.1/
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:32.285587 Fragmenstein-1.0.1/Fragmenstein.egg-info/
--rw-r--r--   0 user       (502) staff       (20)    32364 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)    28971 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       55 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/entry_points.txt
--rw-r--r--   0 user       (502) staff       (20)      340 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       19 2024-02-22 13:28:31.000000 Fragmenstein-1.0.1/Fragmenstein.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)     1069 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/LICENSE
--rw-r--r--   0 user       (502) staff       (20)      317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/MANIFEST.in
--rw-r--r--   0 user       (502) staff       (20)    32364 2024-02-22 13:28:39.129632 Fragmenstein-1.0.1/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)    31456 2024-02-21 13:22:43.000000 Fragmenstein-1.0.1/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:32.463360 Fragmenstein-1.0.1/fragmenstein/
--rw-r--r--   0 user       (502) staff       (20)     2059 2024-02-21 13:07:25.000000 Fragmenstein-1.0.1/fragmenstein/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     1465 2024-02-15 19:52:24.000000 Fragmenstein-1.0.1/fragmenstein/_cli_defaults.py
--rw-r--r--   0 user       (502) staff       (20)     1189 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/branding.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:32.542857 Fragmenstein-1.0.1/fragmenstein/cli/
--rw-r--r--   0 user       (502) staff       (20)      826 2024-01-17 13:24:24.000000 Fragmenstein-1.0.1/fragmenstein/cli/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     3175 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/cli/base.py
--rw-r--r--   0 user       (502) staff       (20)     5136 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/cli/laboratory.py
--rw-r--r--   0 user       (502) staff       (20)     1474 2023-04-27 17:14:38.000000 Fragmenstein-1.0.1/fragmenstein/cli/monster.py
--rw-r--r--   0 user       (502) staff       (20)     4904 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/cli/old.py
--rw-r--r--   0 user       (502) staff       (20)      600 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/cli/parser.py
--rw-r--r--   0 user       (502) staff       (20)     8987 2024-02-09 11:09:55.000000 Fragmenstein-1.0.1/fragmenstein/cli/pipeline.py
--rw-r--r--   0 user       (502) staff       (20)     3287 2024-01-17 13:54:57.000000 Fragmenstein-1.0.1/fragmenstein/cli/utils.py
--rw-r--r--   0 user       (502) staff       (20)     1730 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/cli/victor.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:32.559650 Fragmenstein-1.0.1/fragmenstein/demo/
--rw-r--r--   0 user       (502) staff       (20)     2101 2023-09-18 15:43:25.000000 Fragmenstein-1.0.1/fragmenstein/demo/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4515 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/_base_dataset_holder.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:34.919776 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/
--rw-r--r--   0 user       (502) staff       (20)       85 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
--rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
--rw-r--r--   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
--rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
--rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
--rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
--rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
--rw-r--r--   0 user       (502) staff       (20)      557 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
--rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
--rw-r--r--   0 user       (502) staff       (20)     1605 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
--rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0115.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0116.mol
--rw-r--r--   0 user       (502) staff       (20)     1186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0123.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0124.mol
--rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0131.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0132.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0137.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0138.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0139.mol
--rw-r--r--   0 user       (502) staff       (20)     1531 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0142.mol
--rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0148.mol
--rw-r--r--   0 user       (502) staff       (20)     1518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0159.mol
--rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0161.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0163.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0178.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0179.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0180.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0182.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0188.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0190.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0193.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0204.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0206.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0212.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0213.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0223.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0224.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0226.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0227.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0228.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0231.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0255.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0263.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0271.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0277.mol
--rw-r--r--   0 user       (502) staff       (20)      841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0282.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0283.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0284.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0301.mol
--rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0302.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0303.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0305.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0306.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0309.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0319.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0321.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0326.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0328.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0333.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0337.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0338.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0341.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0343.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0344.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0345.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0346.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0347.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0348.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0354.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0357.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0358.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0360.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0361.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0365.mol
--rw-r--r--   0 user       (502) staff       (20)     2073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0371.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0373.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0375.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0378.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0379.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0380.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0381.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0385.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0387.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0392.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0394.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0396.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0397.mol
--rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0402.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0404.mol
--rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0411.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0412.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0415.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0417.mol
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0433.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0436.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0437.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0439.mol
--rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0441.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0444.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0451.mol
--rw-r--r--   0 user       (502) staff       (20)      745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0453.mol
--rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0455.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0472.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0482.mol
--rw-r--r--   0 user       (502) staff       (20)     1671 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0496.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0509.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0510.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0511.mol
--rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0522.mol
--rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0527.mol
--rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0546.mol
--rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0555.mol
--rw-r--r--   0 user       (502) staff       (20)     1269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0564.mol
--rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0565.mol
--rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0567.mol
--rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0568.mol
--rw-r--r--   0 user       (502) staff       (20)     2156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0570.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0572.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0576.mol
--rw-r--r--   0 user       (502) staff       (20)     1352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0582.mol
--rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0584.mol
--rw-r--r--   0 user       (502) staff       (20)     1326 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0587.mol
--rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0588.mol
--rw-r--r--   0 user       (502) staff       (20)     3121 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0590.mol
--rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x1493.mol
--rw-r--r--   0 user       (502) staff       (20)     1933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x1494.mol
--rw-r--r--   0 user       (502) staff       (20)   208424 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/template.pdb
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.406374 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/
--rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
--rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
--rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
--rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
--rw-r--r--   0 user       (502) staff       (20)      404 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
--rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
--rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
--rw-r--r--   0 user       (502) staff       (20)      972 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
--rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
--rw-r--r--   0 user       (502) staff       (20)     2920 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
--rw-r--r--   0 user       (502) staff       (20)      640 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
--rw-r--r--   0 user       (502) staff       (20)     2658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
--rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
--rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
--rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
--rw-r--r--   0 user       (502) staff       (20)      832 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
--rw-r--r--   0 user       (502) staff       (20)      505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
--rw-r--r--   0 user       (502) staff       (20)     2230 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
--rw-r--r--   0 user       (502) staff       (20)      754 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
--rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
--rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
--rw-r--r--   0 user       (502) staff       (20)     3820 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
--rw-r--r--   0 user       (502) staff       (20)     3667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
--rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7com.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
--rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
--rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
--rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
--rw-r--r--   0 user       (502) staff       (20)      391 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
--rw-r--r--   0 user       (502) staff       (20)     3112 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
--rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
--rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
--rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
--rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
--rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     1348 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
--rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
--rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
--rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
--rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
--rw-r--r--   0 user       (502) staff       (20)     1737 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
--rw-r--r--   0 user       (502) staff       (20)     1309 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
--rw-r--r--   0 user       (502) staff       (20)     1392 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
--rw-r--r--   0 user       (502) staff       (20)      479 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
--rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
--rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
--rw-r--r--   0 user       (502) staff       (20)     2160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
--rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
--rw-r--r--   0 user       (502) staff       (20)     1323 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
--rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
--rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
--rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
--rw-r--r--   0 user       (502) staff       (20)     1943 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
--rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
--rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
--rw-r--r--   0 user       (502) staff       (20)     1764 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
--rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
--rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
--rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
--rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
--rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
--rw-r--r--   0 user       (502) staff       (20)     1400 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
--rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
--rw-r--r--   0 user       (502) staff       (20)     2352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
--rw-r--r--   0 user       (502) staff       (20)     2697 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
--rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
--rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
--rw-r--r--   0 user       (502) staff       (20)     2593 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
--rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
--rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
--rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
--rw-r--r--   0 user       (502) staff       (20)     1675 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
--rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
--rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
--rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
--rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
--rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
--rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
--rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
--rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
--rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
--rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
--rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
--rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
--rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
--rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
--rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
--rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
--rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
--rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
--rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
--rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
--rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
--rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
--rw-r--r--   0 user       (502) staff       (20)     2186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
--rw-r--r--   0 user       (502) staff       (20)      907 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
--rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
--rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
--rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
--rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
--rw-r--r--   0 user       (502) staff       (20)     1073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
--rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
--rw-r--r--   0 user       (502) staff       (20)      824 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
--rw-r--r--   0 user       (502) staff       (20)      741 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
--rw-r--r--   0 user       (502) staff       (20)     2497 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
--rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
--rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
--rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
--rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
--rw-r--r--   0 user       (502) staff       (20)     3008 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
--rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
--rw-r--r--   0 user       (502) staff       (20)     2178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
--rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
--rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
--rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
--rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
--rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
--rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
--rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
--rw-r--r--   0 user       (502) staff       (20)     2829 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
--rw-r--r--   0 user       (502) staff       (20)     2663 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
--rw-r--r--   0 user       (502) staff       (20)     2580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
--rw-r--r--   0 user       (502) staff       (20)     2759 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
--rw-r--r--   0 user       (502) staff       (20)     2331 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
--rw-r--r--   0 user       (502) staff       (20)     2427 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
--rw-r--r--   0 user       (502) staff       (20)     2191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
--rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
--rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
--rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
--rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
--rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
--rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
--rw-r--r--   0 user       (502) staff       (20)     2414 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
--rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
--rw-r--r--   0 user       (502) staff       (20)       76 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/__init__.py
--rw-r--r--   0 user       (502) staff       (20)   379172 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/template.pdb
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.534472 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/
--rw-r--r--   0 user       (502) staff       (20)    17574 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/5SB7_mergers.sdf
--rw-r--r--   0 user       (502) staff       (20)     1254 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/F584.mol
--rw-r--r--   0 user       (502) staff       (20)      144 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/__init__.py
--rwxr-xr-x   0 user       (502) staff       (20)   467127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/apo_example1.pdb
--rw-r--r--   0 user       (502) staff       (20)     6701 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/dummy.pdb
--rwxr-xr-x   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/mac-x0138.mol
--rwxr-xr-x   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/mac-x0398.mol
--rw-r--r--   0 user       (502) staff       (20)     4580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/placed_example1.mol
--rw-r--r--   0 user       (502) staff       (20)      753 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/rototoluene.mol
--rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/toluene.mol
--rw-r--r--   0 user       (502) staff       (20)      758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/transtoluene.mol
--rw-r--r--   0 user       (502) staff       (20)      763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/transtoluene2.mol
--rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/x0032_0A.mol
--rw-r--r--   0 user       (502) staff       (20)     1421 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/demo/test_mols/x0103_0A.mol
--rw-r--r--   0 user       (502) staff       (20)     3115 2024-02-21 13:07:25.000000 Fragmenstein-1.0.1/fragmenstein/display.py
--rw-r--r--   0 user       (502) staff       (20)    56342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/divergent_colors.json
--rw-r--r--   0 user       (502) staff       (20)     1801 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/error.py
--rw-r--r--   0 user       (502) staff       (20)     6425 2023-12-18 18:30:24.000000 Fragmenstein-1.0.1/fragmenstein/extraction_funs.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.568053 Fragmenstein-1.0.1/fragmenstein/faux_victors/
--rw-r--r--   0 user       (502) staff       (20)     1178 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     4793 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/brics.py
--rw-r--r--   0 user       (502) staff       (20)    13343 2023-12-11 16:13:15.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/mcs_monster.py
--rw-r--r--   0 user       (502) staff       (20)      921 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/mcs_victor.py
--rw-r--r--   0 user       (502) staff       (20)     5845 2024-02-02 10:32:19.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/no_pyrosetta.py
--rw-r--r--   0 user       (502) staff       (20)     3648 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/others.py
--rw-r--r--   0 user       (502) staff       (20)     2712 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/faux_victors/quick.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.591759 Fragmenstein-1.0.1/fragmenstein/igor/
--rw-r--r--   0 user       (502) staff       (20)     2432 2023-04-26 12:35:21.000000 Fragmenstein-1.0.1/fragmenstein/igor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      817 2023-04-26 12:34:04.000000 Fragmenstein-1.0.1/fragmenstein/igor/_igor_base.py
--rw-r--r--   0 user       (502) staff       (20)     7774 2024-01-16 11:13:08.000000 Fragmenstein-1.0.1/fragmenstein/igor/_igor_init.py
--rw-r--r--   0 user       (502) staff       (20)    18404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/igor/_igor_min.py
--rw-r--r--   0 user       (502) staff       (20)    12183 2024-01-17 13:54:57.000000 Fragmenstein-1.0.1/fragmenstein/igor/_igor_utils.py
--rw-r--r--   0 user       (502) staff       (20)     1193 2023-10-27 10:05:23.000000 Fragmenstein-1.0.1/fragmenstein/igor/pyrosetta_import.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.624496 Fragmenstein-1.0.1/fragmenstein/laboratory/
--rw-r--r--   0 user       (502) staff       (20)     1565 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    11748 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/_base.py
--rw-r--r--   0 user       (502) staff       (20)     5057 2023-12-18 18:30:24.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/_combine.py
--rw-r--r--   0 user       (502) staff       (20)    13365 2024-02-15 19:30:09.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/_extras.py
--rw-r--r--   0 user       (502) staff       (20)     5025 2023-12-18 18:30:24.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/_place.py
--rw-r--r--   0 user       (502) staff       (20)    10861 2024-02-15 20:04:47.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/_score.py
--rw-r--r--   0 user       (502) staff       (20)     1419 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/laboratory/validator.py
--rw-r--r--   0 user       (502) staff       (20)     1715 2024-02-22 13:26:29.000000 Fragmenstein-1.0.1/fragmenstein/legacy.py
--rw-r--r--   0 user       (502) staff       (20)    21716 2023-07-13 16:14:35.000000 Fragmenstein-1.0.1/fragmenstein/m_rmsd.py
--rw-r--r--   0 user       (502) staff       (20)     4418 2024-02-21 12:47:15.000000 Fragmenstein-1.0.1/fragmenstein/mol3d_display.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.684498 Fragmenstein-1.0.1/fragmenstein/monster/
--rw-r--r--   0 user       (502) staff       (20)     6504 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     9148 2023-10-19 15:02:50.000000 Fragmenstein-1.0.1/fragmenstein/monster/_base.py
--rw-r--r--   0 user       (502) staff       (20)    53383 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/_collapse_ring.py
--rw-r--r--   0 user       (502) staff       (20)     4053 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_combine.py
--rw-r--r--   0 user       (502) staff       (20)    19282 2023-07-29 22:48:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/_communal.py
--rw-r--r--   0 user       (502) staff       (20)    16049 2024-02-07 10:37:46.000000 Fragmenstein-1.0.1/fragmenstein/monster/_ff.py
--rw-r--r--   0 user       (502) staff       (20)     6338 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_join_neighboring.py
--rw-r--r--   0 user       (502) staff       (20)    16359 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_merge.py
--rw-r--r--   0 user       (502) staff       (20)     1582 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_modification_logging.py
--rw-r--r--   0 user       (502) staff       (20)     8229 2023-11-14 13:15:23.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.748498 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/
--rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    13701 2023-07-12 11:22:55.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_expand.py
--rw-r--r--   0 user       (502) staff       (20)     1106 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_full.py
--rw-r--r--   0 user       (502) staff       (20)     8344 2023-07-05 11:51:56.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_make_chimera.py
--rw-r--r--   0 user       (502) staff       (20)    10200 2023-07-12 13:14:33.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_mappings.py
--rw-r--r--   0 user       (502) staff       (20)     9219 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_no_blending.py
--rw-r--r--   0 user       (502) staff       (20)     9905 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_partial.py
--rw-r--r--   0 user       (502) staff       (20)     6957 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_refine.py
--rw-r--r--   0 user       (502) staff       (20)    10464 2024-02-21 12:47:15.000000 Fragmenstein-1.0.1/fragmenstein/monster/_util_compare.py
--rw-r--r--   0 user       (502) staff       (20)    14404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/_utility.py
--rw-r--r--   0 user       (502) staff       (20)     1939 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/bond_provenance.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.776172 Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/
--rw-r--r--   0 user       (502) staff       (20)      342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    11854 2023-07-12 14:59:39.000000 Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/compare_atom.py
--rw-r--r--   0 user       (502) staff       (20)     1127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/types.py
--rw-r--r--   0 user       (502) staff       (20)     5354 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/utils.py
--rw-r--r--   0 user       (502) staff       (20)     5087 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/monster/positional_mapping.py
--rw-r--r--   0 user       (502) staff       (20)    21692 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/monster/unmerge_mapper.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.796231 Fragmenstein-1.0.1/fragmenstein/mpro/
--rw-r--r--   0 user       (502) staff       (20)     6088 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/mpro/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     1439 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/mpro/dataframe.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.813065 Fragmenstein-1.0.1/fragmenstein/multivictor/
--rw-r--r--   0 user       (502) staff       (20)       70 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/multivictor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     3254 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/multivictor/multivictor.py
--rw-r--r--   0 user       (502) staff       (20)     5508 2024-02-21 10:33:08.000000 Fragmenstein-1.0.1/fragmenstein/ngl_display.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.839009 Fragmenstein-1.0.1/fragmenstein/openmm/
--rw-r--r--   0 user       (502) staff       (20)       59 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/openmm/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    24977 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/openmm/fritz.py
--rw-r--r--   0 user       (502) staff       (20)     6995 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/openmm/openvictor.py
--rw-r--r--   0 user       (502) staff       (20)     2318 2023-11-23 13:18:06.000000 Fragmenstein-1.0.1/fragmenstein/settings.py
--rw-r--r--   0 user       (502) staff       (20)      676 2024-02-22 13:26:58.000000 Fragmenstein-1.0.1/fragmenstein/version.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:38.966520 Fragmenstein-1.0.1/fragmenstein/victor/
--rw-r--r--   0 user       (502) staff       (20)     6219 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      802 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_loggerwriter.py
--rw-r--r--   0 user       (502) staff       (20)     9364 2023-12-18 18:30:34.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_base.py
--rw-r--r--   0 user       (502) staff       (20)     7231 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_combine.py
--rw-r--r--   0 user       (502) staff       (20)    18020 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_common.py
--rw-r--r--   0 user       (502) staff       (20)     5547 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_igor.py
--rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_journal.py
--rw-r--r--   0 user       (502) staff       (20)      338 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_mode.py
--rw-r--r--   0 user       (502) staff       (20)      829 2023-12-18 18:30:40.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_overridables.py
--rw-r--r--   0 user       (502) staff       (20)     9133 2024-02-02 08:43:25.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_place.py
--rw-r--r--   0 user       (502) staff       (20)     8793 2024-02-07 09:50:10.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_plonk.py
--rw-r--r--   0 user       (502) staff       (20)     1863 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_safety.py
--rw-r--r--   0 user       (502) staff       (20)     6816 2024-02-13 16:18:01.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_show.py
--rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_store.py
--rw-r--r--   0 user       (502) staff       (20)    24750 2024-02-13 15:36:41.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_utils.py
--rw-r--r--   0 user       (502) staff       (20)     2202 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/fragmenstein/victor/_victor_validate.py
--rw-r--r--   0 user       (502) staff       (20)     5650 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/victor/minimalPDB.py
--rw-r--r--   0 user       (502) staff       (20)    10778 2023-08-22 10:47:34.000000 Fragmenstein-1.0.1/fragmenstein/victor/plip.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:39.010985 Fragmenstein-1.0.1/fragmenstein/walton/
--rw-r--r--   0 user       (502) staff       (20)     2277 2024-02-21 10:33:08.000000 Fragmenstein-1.0.1/fragmenstein/walton/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     8226 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/walton/_advmoves.py
--rw-r--r--   0 user       (502) staff       (20)     4004 2024-02-21 10:52:06.000000 Fragmenstein-1.0.1/fragmenstein/walton/_art.py
--rw-r--r--   0 user       (502) staff       (20)     4333 2024-02-21 13:07:25.000000 Fragmenstein-1.0.1/fragmenstein/walton/_base.py
--rw-r--r--   0 user       (502) staff       (20)     6289 2024-01-19 13:58:39.000000 Fragmenstein-1.0.1/fragmenstein/walton/_movements.py
--rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.1/fragmenstein/walton/_polygon.py
--rw-r--r--   0 user       (502) staff       (20)     1033 2024-02-22 13:18:08.000000 Fragmenstein-1.0.1/requirements.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2024-02-22 13:28:39.132546 Fragmenstein-1.0.1/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)     3377 2024-02-22 13:26:58.000000 Fragmenstein-1.0.1/setup.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-22 13:28:39.126226 Fragmenstein-1.0.1/tests/
--rw-r--r--   0 user       (502) staff       (20)     1689 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/MPro_combine.py
--rw-r--r--   0 user       (502) staff       (20)     4498 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/MPro_place.py
--rw-r--r--   0 user       (502) staff       (20)      404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/__init__.py
--rw-r--r--   0 user       (502) staff       (20)      725 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/baffled.py
--rw-r--r--   0 user       (502) staff       (20)     2623 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/cli.py
--rw-r--r--   0 user       (502) staff       (20)     2130 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/dummy_victor.py
--rw-r--r--   0 user       (502) staff       (20)     6666 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/internals.py
--rw-r--r--   0 user       (502) staff       (20)      642 2023-12-18 18:30:26.000000 Fragmenstein-1.0.1/tests/lab.py
--rw-r--r--   0 user       (502) staff       (20)     6321 2023-07-12 14:51:49.000000 Fragmenstein-1.0.1/tests/mapping.py
--rw-r--r--   0 user       (502) staff       (20)     4376 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/monster_combine.py
--rw-r--r--   0 user       (502) staff       (20)    11927 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/monster_place.py
--rw-r--r--   0 user       (502) staff       (20)     1323 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/multivictor.py
--rw-r--r--   0 user       (502) staff       (20)     4492 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/problems.py
--rw-r--r--   0 user       (502) staff       (20)     2814 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/victor_combine.py
--rw-r--r--   0 user       (502) staff       (20)     2911 2023-12-18 18:30:42.000000 Fragmenstein-1.0.1/tests/victor_discard.py
--rw-r--r--   0 user       (502) staff       (20)     4320 2023-07-07 14:11:40.000000 Fragmenstein-1.0.1/tests/walton.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.460112 Fragmenstein-1.0.2/
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:21.618124 Fragmenstein-1.0.2/Fragmenstein.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)    32364 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    28971 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       55 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/entry_points.txt
+-rw-r--r--   0 user       (502) staff       (20)      340 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       19 2024-03-13 13:41:21.000000 Fragmenstein-1.0.2/Fragmenstein.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)      317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/MANIFEST.in
+-rw-r--r--   0 user       (502) staff       (20)    32364 2024-03-13 13:41:26.457519 Fragmenstein-1.0.2/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    31456 2024-02-21 13:22:43.000000 Fragmenstein-1.0.2/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:21.665307 Fragmenstein-1.0.2/fragmenstein/
+-rw-r--r--   0 user       (502) staff       (20)     2059 2024-02-21 13:07:25.000000 Fragmenstein-1.0.2/fragmenstein/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1465 2024-02-15 19:52:24.000000 Fragmenstein-1.0.2/fragmenstein/_cli_defaults.py
+-rw-r--r--   0 user       (502) staff       (20)     1189 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/branding.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:21.698483 Fragmenstein-1.0.2/fragmenstein/cli/
+-rw-r--r--   0 user       (502) staff       (20)      826 2024-01-17 13:24:24.000000 Fragmenstein-1.0.2/fragmenstein/cli/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3175 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/cli/base.py
+-rw-r--r--   0 user       (502) staff       (20)     5136 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/cli/laboratory.py
+-rw-r--r--   0 user       (502) staff       (20)     1474 2023-04-27 17:14:38.000000 Fragmenstein-1.0.2/fragmenstein/cli/monster.py
+-rw-r--r--   0 user       (502) staff       (20)     4904 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/cli/old.py
+-rw-r--r--   0 user       (502) staff       (20)      600 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/cli/parser.py
+-rw-r--r--   0 user       (502) staff       (20)     8987 2024-02-09 11:09:55.000000 Fragmenstein-1.0.2/fragmenstein/cli/pipeline.py
+-rw-r--r--   0 user       (502) staff       (20)     3287 2024-01-17 13:54:57.000000 Fragmenstein-1.0.2/fragmenstein/cli/utils.py
+-rw-r--r--   0 user       (502) staff       (20)     1730 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/cli/victor.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:21.702027 Fragmenstein-1.0.2/fragmenstein/demo/
+-rw-r--r--   0 user       (502) staff       (20)     2101 2023-09-18 15:43:25.000000 Fragmenstein-1.0.2/fragmenstein/demo/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4515 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/_base_dataset_holder.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:23.224109 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/
+-rw-r--r--   0 user       (502) staff       (20)       85 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1592 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1247 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1317 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1164 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1343 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1234 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      736 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      998 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      902 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      570 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      557 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1068 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
+-rw-r--r--   0 user       (502) staff       (20)      915 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1605 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
+-rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0115.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0116.mol
+-rw-r--r--   0 user       (502) staff       (20)     1186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0123.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0124.mol
+-rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0131.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0132.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0137.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0138.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0139.mol
+-rw-r--r--   0 user       (502) staff       (20)     1531 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0142.mol
+-rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0148.mol
+-rw-r--r--   0 user       (502) staff       (20)     1518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0159.mol
+-rw-r--r--   0 user       (502) staff       (20)     1601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0161.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0163.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0178.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0179.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0180.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0182.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0188.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0190.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0193.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0204.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0206.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0212.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0213.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0223.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0224.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0226.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0227.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0228.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0231.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0255.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0263.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0271.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0277.mol
+-rw-r--r--   0 user       (502) staff       (20)      841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0282.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0283.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0284.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0301.mol
+-rw-r--r--   0 user       (502) staff       (20)     1243 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0302.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0303.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0306.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0309.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0319.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0321.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0326.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0328.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0333.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0337.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0338.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0341.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0343.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0344.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0345.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0346.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0347.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0354.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0357.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0358.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0360.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0361.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0365.mol
+-rw-r--r--   0 user       (502) staff       (20)     2073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0371.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0373.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0375.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0378.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0379.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0380.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0381.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0385.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0387.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0394.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0396.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0397.mol
+-rw-r--r--   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0402.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0404.mol
+-rw-r--r--   0 user       (502) staff       (20)     1160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0411.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0412.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0415.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0417.mol
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0433.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0436.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0437.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0439.mol
+-rw-r--r--   0 user       (502) staff       (20)     1505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0441.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0444.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0451.mol
+-rw-r--r--   0 user       (502) staff       (20)      745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0453.mol
+-rw-r--r--   0 user       (502) staff       (20)     1077 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0455.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0472.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0482.mol
+-rw-r--r--   0 user       (502) staff       (20)     1671 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0496.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0509.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0510.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0511.mol
+-rw-r--r--   0 user       (502) staff       (20)     1256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0522.mol
+-rw-r--r--   0 user       (502) staff       (20)     1422 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0527.mol
+-rw-r--r--   0 user       (502) staff       (20)     1339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0546.mol
+-rw-r--r--   0 user       (502) staff       (20)     1007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0555.mol
+-rw-r--r--   0 user       (502) staff       (20)     1269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0564.mol
+-rw-r--r--   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0565.mol
+-rw-r--r--   0 user       (502) staff       (20)      924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0567.mol
+-rw-r--r--   0 user       (502) staff       (20)      911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0568.mol
+-rw-r--r--   0 user       (502) staff       (20)     2156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0570.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0572.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0576.mol
+-rw-r--r--   0 user       (502) staff       (20)     1352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0582.mol
+-rw-r--r--   0 user       (502) staff       (20)     1614 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0584.mol
+-rw-r--r--   0 user       (502) staff       (20)     1326 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0587.mol
+-rw-r--r--   0 user       (502) staff       (20)     1435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0588.mol
+-rw-r--r--   0 user       (502) staff       (20)     3121 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0590.mol
+-rw-r--r--   0 user       (502) staff       (20)     1173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x1493.mol
+-rw-r--r--   0 user       (502) staff       (20)     1933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x1494.mol
+-rw-r--r--   0 user       (502) staff       (20)   208424 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/template.pdb
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:25.963261 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/
+-rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
+-rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
+-rw-r--r--   0 user       (502) staff       (20)     2933 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
+-rw-r--r--   0 user       (502) staff       (20)      723 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
+-rw-r--r--   0 user       (502) staff       (20)      404 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
+-rw-r--r--   0 user       (502) staff       (20)      985 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
+-rw-r--r--   0 user       (502) staff       (20)      819 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
+-rw-r--r--   0 user       (502) staff       (20)      972 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
+-rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
+-rw-r--r--   0 user       (502) staff       (20)     2920 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
+-rw-r--r--   0 user       (502) staff       (20)      640 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
+-rw-r--r--   0 user       (502) staff       (20)     2658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
+-rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
+-rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
+-rw-r--r--   0 user       (502) staff       (20)     3680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
+-rw-r--r--   0 user       (502) staff       (20)      832 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
+-rw-r--r--   0 user       (502) staff       (20)      505 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
+-rw-r--r--   0 user       (502) staff       (20)     2230 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
+-rw-r--r--   0 user       (502) staff       (20)      754 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
+-rw-r--r--   0 user       (502) staff       (20)      806 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
+-rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
+-rw-r--r--   0 user       (502) staff       (20)     3820 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
+-rw-r--r--   0 user       (502) staff       (20)     3667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
+-rw-r--r--   0 user       (502) staff       (20)     2492 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7com.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
+-rw-r--r--   0 user       (502) staff       (20)      142 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
+-rw-r--r--   0 user       (502) staff       (20)     2850 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
+-rw-r--r--   0 user       (502) staff       (20)     3527 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
+-rw-r--r--   0 user       (502) staff       (20)      391 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
+-rw-r--r--   0 user       (502) staff       (20)     3112 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
+-rw-r--r--   0 user       (502) staff       (20)     4178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
+-rw-r--r--   0 user       (502) staff       (20)     3169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
+-rw-r--r--   0 user       (502) staff       (20)     4191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
+-rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
+-rw-r--r--   0 user       (502) staff       (20)     1597 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     1348 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
+-rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
+-rwxr-xr-x   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
+-rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
+-rw-r--r--   0 user       (502) staff       (20)      990 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
+-rw-r--r--   0 user       (502) staff       (20)     1737 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
+-rw-r--r--   0 user       (502) staff       (20)     1309 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
+-rw-r--r--   0 user       (502) staff       (20)     1392 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
+-rw-r--r--   0 user       (502) staff       (20)      479 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
+-rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
+-rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
+-rw-r--r--   0 user       (502) staff       (20)     2160 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
+-rw-r--r--   0 user       (502) staff       (20)      658 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
+-rw-r--r--   0 user       (502) staff       (20)     1323 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
+-rw-r--r--   0 user       (502) staff       (20)     1502 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
+-rw-r--r--   0 user       (502) staff       (20)     2179 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
+-rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
+-rw-r--r--   0 user       (502) staff       (20)     1943 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
+-rw-r--r--   0 user       (502) staff       (20)     1668 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
+-rw-r--r--   0 user       (502) staff       (20)     1930 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
+-rw-r--r--   0 user       (502) staff       (20)     1764 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
+-rw-r--r--   0 user       (502) staff       (20)     2013 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
+-rw-r--r--   0 user       (502) staff       (20)     1585 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
+-rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
+-rw-r--r--   0 user       (502) staff       (20)     1751 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
+-rw-r--r--   0 user       (502) staff       (20)     1834 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
+-rw-r--r--   0 user       (502) staff       (20)     1400 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
+-rw-r--r--   0 user       (502) staff       (20)     1081 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
+-rw-r--r--   0 user       (502) staff       (20)     2352 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
+-rw-r--r--   0 user       (502) staff       (20)     2697 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
+-rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
+-rw-r--r--   0 user       (502) staff       (20)     1828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
+-rw-r--r--   0 user       (502) staff       (20)     2593 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
+-rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
+-rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
+-rw-r--r--   0 user       (502) staff       (20)     1854 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
+-rw-r--r--   0 user       (502) staff       (20)     1675 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
+-rw-r--r--   0 user       (502) staff       (20)     1937 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
+-rw-r--r--   0 user       (502) staff       (20)     1330 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
+-rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
+-rw-r--r--   0 user       (502) staff       (20)     1745 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
+-rw-r--r--   0 user       (502) staff       (20)     1413 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
+-rw-r--r--   0 user       (502) staff       (20)     1662 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
+-rw-r--r--   0 user       (502) staff       (20)     1924 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
+-rw-r--r--   0 user       (502) staff       (20)     1496 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
+-rw-r--r--   0 user       (502) staff       (20)     1579 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
+-rw-r--r--   0 user       (502) staff       (20)     1758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
+-rw-r--r--   0 user       (502) staff       (20)     2339 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
+-rw-r--r--   0 user       (502) staff       (20)     1911 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
+-rw-r--r--   0 user       (502) staff       (20)     2256 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
+-rw-r--r--   0 user       (502) staff       (20)     2173 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
+-rw-r--r--   0 user       (502) staff       (20)     2518 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
+-rw-r--r--   0 user       (502) staff       (20)     2435 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
+-rw-r--r--   0 user       (502) staff       (20)     2601 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
+-rw-r--r--   0 user       (502) staff       (20)     1841 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
+-rw-r--r--   0 user       (502) staff       (20)     2103 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
+-rw-r--r--   0 user       (502) staff       (20)     1335 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
+-rw-r--r--   0 user       (502) staff       (20)     2090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
+-rw-r--r--   0 user       (502) staff       (20)     2269 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
+-rw-r--r--   0 user       (502) staff       (20)     2186 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
+-rw-r--r--   0 user       (502) staff       (20)      907 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
+-rw-r--r--   0 user       (502) staff       (20)     1252 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
+-rw-r--r--   0 user       (502) staff       (20)     1239 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
+-rw-r--r--   0 user       (502) staff       (20)     1501 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
+-rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
+-rw-r--r--   0 user       (502) staff       (20)     1073 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
+-rw-r--r--   0 user       (502) staff       (20)     1156 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
+-rw-r--r--   0 user       (502) staff       (20)      824 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
+-rw-r--r--   0 user       (502) staff       (20)      741 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
+-rw-r--r--   0 user       (502) staff       (20)     2497 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
+-rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
+-rw-r--r--   0 user       (502) staff       (20)     1929 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
+-rw-r--r--   0 user       (502) staff       (20)     2925 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
+-rw-r--r--   0 user       (502) staff       (20)     1667 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
+-rw-r--r--   0 user       (502) staff       (20)     3008 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
+-rw-r--r--   0 user       (502) staff       (20)     1418 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
+-rw-r--r--   0 user       (502) staff       (20)     2178 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
+-rw-r--r--   0 user       (502) staff       (20)     1750 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
+-rw-r--r--   0 user       (502) staff       (20)     1846 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
+-rw-r--r--   0 user       (502) staff       (20)     1584 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
+-rw-r--r--   0 user       (502) staff       (20)     1994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
+-rw-r--r--   0 user       (502) staff       (20)     1680 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
+-rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
+-rw-r--r--   0 user       (502) staff       (20)     1833 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
+-rw-r--r--   0 user       (502) staff       (20)     2829 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
+-rw-r--r--   0 user       (502) staff       (20)     2663 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
+-rw-r--r--   0 user       (502) staff       (20)     2580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
+-rw-r--r--   0 user       (502) staff       (20)     2759 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
+-rw-r--r--   0 user       (502) staff       (20)     2331 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
+-rw-r--r--   0 user       (502) staff       (20)     2427 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
+-rw-r--r--   0 user       (502) staff       (20)     2191 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
+-rw-r--r--   0 user       (502) staff       (20)     2261 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
+-rw-r--r--   0 user       (502) staff       (20)     1322 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
+-rw-r--r--   0 user       (502) staff       (20)     1151 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
+-rw-r--r--   0 user       (502) staff       (20)     1488 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
+-rw-r--r--   0 user       (502) staff       (20)     2007 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
+-rw-r--r--   0 user       (502) staff       (20)     1169 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
+-rw-r--r--   0 user       (502) staff       (20)     2414 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
+-rw-r--r--   0 user       (502) staff       (20)     1763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
+-rw-r--r--   0 user       (502) staff       (20)       76 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)   379172 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/template.pdb
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.064468 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/
+-rw-r--r--   0 user       (502) staff       (20)    17574 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/5SB7_mergers.sdf
+-rw-r--r--   0 user       (502) staff       (20)     1254 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/F584.mol
+-rw-r--r--   0 user       (502) staff       (20)      144 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/__init__.py
+-rwxr-xr-x   0 user       (502) staff       (20)   467127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/apo_example1.pdb
+-rw-r--r--   0 user       (502) staff       (20)     6701 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/dummy.pdb
+-rwxr-xr-x   0 user       (502) staff       (20)     1090 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/mac-x0138.mol
+-rwxr-xr-x   0 user       (502) staff       (20)      994 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/mac-x0398.mol
+-rw-r--r--   0 user       (502) staff       (20)     4580 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/placed_example1.mol
+-rw-r--r--   0 user       (502) staff       (20)      753 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/rototoluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      653 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/toluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      758 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/transtoluene.mol
+-rw-r--r--   0 user       (502) staff       (20)      763 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/transtoluene2.mol
+-rw-r--r--   0 user       (502) staff       (20)     1509 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/x0032_0A.mol
+-rw-r--r--   0 user       (502) staff       (20)     1421 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/demo/test_mols/x0103_0A.mol
+-rw-r--r--   0 user       (502) staff       (20)     3115 2024-02-21 13:07:25.000000 Fragmenstein-1.0.2/fragmenstein/display.py
+-rw-r--r--   0 user       (502) staff       (20)    56342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/divergent_colors.json
+-rw-r--r--   0 user       (502) staff       (20)     1801 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/error.py
+-rw-r--r--   0 user       (502) staff       (20)     6425 2023-12-18 18:30:24.000000 Fragmenstein-1.0.2/fragmenstein/extraction_funs.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.087125 Fragmenstein-1.0.2/fragmenstein/faux_victors/
+-rw-r--r--   0 user       (502) staff       (20)     1178 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     4793 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/brics.py
+-rw-r--r--   0 user       (502) staff       (20)    13343 2023-12-11 16:13:15.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/mcs_monster.py
+-rw-r--r--   0 user       (502) staff       (20)     1018 2024-03-13 10:07:19.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/mcs_victor.py
+-rw-r--r--   0 user       (502) staff       (20)     5743 2024-03-13 10:05:02.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/no_pyrosetta.py
+-rw-r--r--   0 user       (502) staff       (20)     3648 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/others.py
+-rw-r--r--   0 user       (502) staff       (20)     2712 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/faux_victors/quick.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.105011 Fragmenstein-1.0.2/fragmenstein/igor/
+-rw-r--r--   0 user       (502) staff       (20)     2432 2023-04-26 12:35:21.000000 Fragmenstein-1.0.2/fragmenstein/igor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      817 2023-04-26 12:34:04.000000 Fragmenstein-1.0.2/fragmenstein/igor/_igor_base.py
+-rw-r--r--   0 user       (502) staff       (20)     7774 2024-01-16 11:13:08.000000 Fragmenstein-1.0.2/fragmenstein/igor/_igor_init.py
+-rw-r--r--   0 user       (502) staff       (20)    18404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/igor/_igor_min.py
+-rw-r--r--   0 user       (502) staff       (20)    12183 2024-01-17 13:54:57.000000 Fragmenstein-1.0.2/fragmenstein/igor/_igor_utils.py
+-rw-r--r--   0 user       (502) staff       (20)     1193 2023-10-27 10:05:23.000000 Fragmenstein-1.0.2/fragmenstein/igor/pyrosetta_import.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.123333 Fragmenstein-1.0.2/fragmenstein/laboratory/
+-rw-r--r--   0 user       (502) staff       (20)     1565 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    12391 2024-03-13 13:36:49.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/_base.py
+-rw-r--r--   0 user       (502) staff       (20)     5609 2024-03-13 13:33:10.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    13365 2024-02-15 19:30:09.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/_extras.py
+-rw-r--r--   0 user       (502) staff       (20)     5089 2024-03-13 13:36:49.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/_place.py
+-rw-r--r--   0 user       (502) staff       (20)    10885 2024-03-13 12:16:17.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/_score.py
+-rw-r--r--   0 user       (502) staff       (20)     1419 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/laboratory/validator.py
+-rw-r--r--   0 user       (502) staff       (20)     1715 2024-02-22 13:26:29.000000 Fragmenstein-1.0.2/fragmenstein/legacy.py
+-rw-r--r--   0 user       (502) staff       (20)    21716 2023-07-13 16:14:35.000000 Fragmenstein-1.0.2/fragmenstein/m_rmsd.py
+-rw-r--r--   0 user       (502) staff       (20)     4418 2024-02-21 12:47:15.000000 Fragmenstein-1.0.2/fragmenstein/mol3d_display.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.169216 Fragmenstein-1.0.2/fragmenstein/monster/
+-rw-r--r--   0 user       (502) staff       (20)     6504 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     9148 2023-10-19 15:02:50.000000 Fragmenstein-1.0.2/fragmenstein/monster/_base.py
+-rw-r--r--   0 user       (502) staff       (20)    53383 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/_collapse_ring.py
+-rw-r--r--   0 user       (502) staff       (20)     4053 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    19282 2023-07-29 22:48:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/_communal.py
+-rw-r--r--   0 user       (502) staff       (20)    16288 2024-03-13 10:07:19.000000 Fragmenstein-1.0.2/fragmenstein/monster/_ff.py
+-rw-r--r--   0 user       (502) staff       (20)     6338 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_join_neighboring.py
+-rw-r--r--   0 user       (502) staff       (20)    16359 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_merge.py
+-rw-r--r--   0 user       (502) staff       (20)     1582 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_modification_logging.py
+-rw-r--r--   0 user       (502) staff       (20)     8371 2024-03-13 12:01:11.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.187959 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/
+-rw-r--r--   0 user       (502) staff       (20)      828 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    13701 2023-07-12 11:22:55.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_expand.py
+-rw-r--r--   0 user       (502) staff       (20)     1106 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_full.py
+-rw-r--r--   0 user       (502) staff       (20)     8344 2023-07-05 11:51:56.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_make_chimera.py
+-rw-r--r--   0 user       (502) staff       (20)    10200 2023-07-12 13:14:33.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_mappings.py
+-rw-r--r--   0 user       (502) staff       (20)     9219 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_no_blending.py
+-rw-r--r--   0 user       (502) staff       (20)     9905 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_partial.py
+-rw-r--r--   0 user       (502) staff       (20)     6957 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_refine.py
+-rw-r--r--   0 user       (502) staff       (20)    10464 2024-02-21 12:47:15.000000 Fragmenstein-1.0.2/fragmenstein/monster/_util_compare.py
+-rw-r--r--   0 user       (502) staff       (20)    14404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/_utility.py
+-rw-r--r--   0 user       (502) staff       (20)     1939 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/bond_provenance.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.215024 Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/
+-rw-r--r--   0 user       (502) staff       (20)      342 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    11854 2023-07-12 14:59:39.000000 Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/compare_atom.py
+-rw-r--r--   0 user       (502) staff       (20)     1127 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/types.py
+-rw-r--r--   0 user       (502) staff       (20)     5354 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/utils.py
+-rw-r--r--   0 user       (502) staff       (20)     5087 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/monster/positional_mapping.py
+-rw-r--r--   0 user       (502) staff       (20)    21692 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/monster/unmerge_mapper.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.225616 Fragmenstein-1.0.2/fragmenstein/mpro/
+-rw-r--r--   0 user       (502) staff       (20)     6088 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/mpro/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     1439 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/mpro/dataframe.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.239749 Fragmenstein-1.0.2/fragmenstein/multivictor/
+-rw-r--r--   0 user       (502) staff       (20)       70 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/multivictor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3254 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/multivictor/multivictor.py
+-rw-r--r--   0 user       (502) staff       (20)     5508 2024-02-21 10:33:08.000000 Fragmenstein-1.0.2/fragmenstein/ngl_display.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.254368 Fragmenstein-1.0.2/fragmenstein/openmm/
+-rw-r--r--   0 user       (502) staff       (20)       59 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/openmm/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    24977 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/openmm/fritz.py
+-rw-r--r--   0 user       (502) staff       (20)     7011 2024-03-13 10:05:02.000000 Fragmenstein-1.0.2/fragmenstein/openmm/openvictor.py
+-rw-r--r--   0 user       (502) staff       (20)     2318 2023-11-23 13:18:06.000000 Fragmenstein-1.0.2/fragmenstein/settings.py
+-rw-r--r--   0 user       (502) staff       (20)      676 2024-03-13 13:40:53.000000 Fragmenstein-1.0.2/fragmenstein/version.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.336802 Fragmenstein-1.0.2/fragmenstein/victor/
+-rw-r--r--   0 user       (502) staff       (20)     6217 2024-03-13 11:43:40.000000 Fragmenstein-1.0.2/fragmenstein/victor/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      802 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_loggerwriter.py
+-rw-r--r--   0 user       (502) staff       (20)     9613 2024-03-13 11:55:09.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_base.py
+-rw-r--r--   0 user       (502) staff       (20)     7215 2024-03-13 11:43:40.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    18020 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_common.py
+-rw-r--r--   0 user       (502) staff       (20)     5547 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_igor.py
+-rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_journal.py
+-rw-r--r--   0 user       (502) staff       (20)      338 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_mode.py
+-rw-r--r--   0 user       (502) staff       (20)      829 2023-12-18 18:30:40.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_overridables.py
+-rw-r--r--   0 user       (502) staff       (20)     9321 2024-03-13 10:05:02.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_place.py
+-rw-r--r--   0 user       (502) staff       (20)     9457 2024-03-13 10:07:19.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_plonk.py
+-rw-r--r--   0 user       (502) staff       (20)     1863 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_safety.py
+-rw-r--r--   0 user       (502) staff       (20)     6816 2024-02-13 16:18:01.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_show.py
+-rw-r--r--   0 user       (502) staff       (20)     4674 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_store.py
+-rw-r--r--   0 user       (502) staff       (20)    24750 2024-02-13 15:36:41.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_utils.py
+-rw-r--r--   0 user       (502) staff       (20)     2202 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/fragmenstein/victor/_victor_validate.py
+-rw-r--r--   0 user       (502) staff       (20)     5650 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/victor/minimalPDB.py
+-rw-r--r--   0 user       (502) staff       (20)    10778 2023-08-22 10:47:34.000000 Fragmenstein-1.0.2/fragmenstein/victor/plip.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.355372 Fragmenstein-1.0.2/fragmenstein/walton/
+-rw-r--r--   0 user       (502) staff       (20)     2277 2024-02-21 10:33:08.000000 Fragmenstein-1.0.2/fragmenstein/walton/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     8226 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/walton/_advmoves.py
+-rw-r--r--   0 user       (502) staff       (20)     4004 2024-02-21 10:52:06.000000 Fragmenstein-1.0.2/fragmenstein/walton/_art.py
+-rw-r--r--   0 user       (502) staff       (20)     4333 2024-02-21 13:07:25.000000 Fragmenstein-1.0.2/fragmenstein/walton/_base.py
+-rw-r--r--   0 user       (502) staff       (20)     6289 2024-01-19 13:58:39.000000 Fragmenstein-1.0.2/fragmenstein/walton/_movements.py
+-rw-r--r--   0 user       (502) staff       (20)     1693 2023-04-25 12:43:41.000000 Fragmenstein-1.0.2/fragmenstein/walton/_polygon.py
+-rw-r--r--   0 user       (502) staff       (20)     1033 2024-02-22 13:18:08.000000 Fragmenstein-1.0.2/requirements.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-03-13 13:41:26.460440 Fragmenstein-1.0.2/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     3377 2024-03-13 13:40:53.000000 Fragmenstein-1.0.2/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-03-13 13:41:26.452798 Fragmenstein-1.0.2/tests/
+-rw-r--r--   0 user       (502) staff       (20)     1689 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/MPro_combine.py
+-rw-r--r--   0 user       (502) staff       (20)     4498 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/MPro_place.py
+-rw-r--r--   0 user       (502) staff       (20)      404 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)      725 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/baffled.py
+-rw-r--r--   0 user       (502) staff       (20)     2623 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/cli.py
+-rw-r--r--   0 user       (502) staff       (20)     2130 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/dummy_victor.py
+-rw-r--r--   0 user       (502) staff       (20)     6666 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/internals.py
+-rw-r--r--   0 user       (502) staff       (20)      642 2023-12-18 18:30:26.000000 Fragmenstein-1.0.2/tests/lab.py
+-rw-r--r--   0 user       (502) staff       (20)     6321 2023-07-12 14:51:49.000000 Fragmenstein-1.0.2/tests/mapping.py
+-rw-r--r--   0 user       (502) staff       (20)     4376 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/monster_combine.py
+-rw-r--r--   0 user       (502) staff       (20)    11927 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/monster_place.py
+-rw-r--r--   0 user       (502) staff       (20)     1323 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/multivictor.py
+-rw-r--r--   0 user       (502) staff       (20)     4492 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/problems.py
+-rw-r--r--   0 user       (502) staff       (20)     2814 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/victor_combine.py
+-rw-r--r--   0 user       (502) staff       (20)     2911 2023-12-18 18:30:42.000000 Fragmenstein-1.0.2/tests/victor_discard.py
+-rw-r--r--   0 user       (502) staff       (20)     4320 2023-07-07 14:11:40.000000 Fragmenstein-1.0.2/tests/walton.py
```

### Comparing `Fragmenstein-1.0.1/Fragmenstein.egg-info/PKG-INFO` & `Fragmenstein-1.0.2/Fragmenstein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 1.0.1
+Version: 1.0.2
 Summary: Merging, linking and placing compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `Fragmenstein-1.0.1/Fragmenstein.egg-info/SOURCES.txt` & `Fragmenstein-1.0.2/Fragmenstein.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/LICENSE` & `Fragmenstein-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/PKG-INFO` & `Fragmenstein-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 1.0.1
+Version: 1.0.2
 Summary: Merging, linking and placing compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `Fragmenstein-1.0.1/README.md` & `Fragmenstein-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/_cli_defaults.py` & `Fragmenstein-1.0.2/fragmenstein/_cli_defaults.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/branding.py` & `Fragmenstein-1.0.2/fragmenstein/branding.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/base.py` & `Fragmenstein-1.0.2/fragmenstein/cli/base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/laboratory.py` & `Fragmenstein-1.0.2/fragmenstein/cli/laboratory.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/monster.py` & `Fragmenstein-1.0.2/fragmenstein/cli/monster.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/old.py` & `Fragmenstein-1.0.2/fragmenstein/cli/old.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/parser.py` & `Fragmenstein-1.0.2/fragmenstein/cli/parser.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/pipeline.py` & `Fragmenstein-1.0.2/fragmenstein/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/utils.py` & `Fragmenstein-1.0.2/fragmenstein/cli/utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/cli/victor.py` & `Fragmenstein-1.0.2/fragmenstein/cli/victor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/_base_dataset_holder.py` & `Fragmenstein-1.0.2/fragmenstein/demo/_base_dataset_holder.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0115.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0116.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0116.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0123.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0123.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0124.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0131.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0131.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0132.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0137.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0137.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0138.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0139.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0139.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0142.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0142.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0148.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0148.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0159.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0161.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0163.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0178.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0179.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0179.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0180.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0180.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0182.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0182.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0188.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0188.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0190.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0190.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0193.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0204.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0206.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0206.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0212.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0213.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0213.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0223.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0224.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0224.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0226.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0227.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0227.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0228.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0228.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0231.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0255.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0255.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0263.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0263.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0271.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0277.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0277.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0282.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0282.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0283.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0283.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0284.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0284.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0301.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0301.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0302.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0302.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0303.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0305.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0306.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0309.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0309.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0319.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0319.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0321.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0321.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0326.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0326.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0328.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0328.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0333.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0337.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0337.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0338.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0341.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0341.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0343.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0343.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0344.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0344.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0345.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0345.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0346.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0347.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0347.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0348.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0354.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0357.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0357.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0358.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0360.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0360.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0361.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0361.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0365.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0365.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0371.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0373.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0373.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0375.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0378.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0378.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0379.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0379.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0380.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0381.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0381.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0385.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0387.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0392.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0394.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0394.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0396.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0397.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0398.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0402.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0404.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0404.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0411.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0411.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0412.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0415.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0415.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0417.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0433.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0433.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0436.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0436.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0437.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0437.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0439.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0439.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0441.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0441.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0444.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0444.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0451.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0451.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0453.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0453.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0455.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0455.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0472.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0472.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0482.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0482.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0496.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0496.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0509.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0509.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0510.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0510.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0511.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0511.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0522.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0522.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0527.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0527.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0546.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0546.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0555.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0564.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0565.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0567.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0567.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0568.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0568.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0570.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0570.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0572.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0576.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0576.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0582.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0582.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0584.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0587.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0588.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0588.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x0590.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x0590.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x1493.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/mac-x1494.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/mac-x1494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mac1_mols/template.pdb` & `Fragmenstein-1.0.2/fragmenstein/demo/mac1_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6lze.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6lze.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6w63.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6w63.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xch.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xch.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-6zru.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-6zru.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7aku.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7aku.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7brp.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7brp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7buy.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7buy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7com.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7com.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k40.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k40.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0072.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0072.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0104.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0104.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0107.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0107.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0161.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0165.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0165.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0177.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0177.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0194.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0194.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0195.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0195.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0305.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0336.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0350.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0350.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0354.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0376.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0376.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0387.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0390.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0390.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0395.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0397.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0398.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0425.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0426.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0434.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0434.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0464.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0464.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0478.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0499.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0540.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0669.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0669.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0678.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0689.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0689.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0691.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0691.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0692.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0692.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0705.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0708.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0708.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0731.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0731.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0734.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0734.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0736.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0736.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0748.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0748.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0749.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0749.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0752.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0752.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0755.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0755.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0759.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0759.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0769.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0769.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0770.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0770.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0771.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0771.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0774.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0774.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0786.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0786.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0820.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0830.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0830.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0831.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0874.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0874.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0887.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0887.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0946.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0946.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0967.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0967.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0978.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0978.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0981.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0981.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x0995.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x0995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10019.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10019.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1002.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1002.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10022.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10022.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10049.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10049.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10082.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10082.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1012.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1012.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10150.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10150.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10155.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10155.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10172.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10172.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10178.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10201.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10201.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10236.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10236.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10237.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10247.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10247.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10248.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10248.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10296.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10296.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10306.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10314.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10314.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10322.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10322.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10324.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10327.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10327.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10329.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10329.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10334.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10338.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10355.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10355.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10359.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10371.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10377.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10377.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10387.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10392.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10395.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10396.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10403.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10403.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10417.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10419.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10419.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10421.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10421.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10422.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10422.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10423.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10423.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10466.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10466.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10473.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10474.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10474.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10476.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10476.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10478.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10484.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10484.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10488.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10494.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10506.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10506.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10513.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10513.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10525.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10525.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10535.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10535.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10555.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10559.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10559.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10565.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10566.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10566.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10575.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10575.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10598.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10598.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10604.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10604.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10606.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10606.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10610.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10610.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10626.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10626.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10638.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10638.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10645.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10645.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10678.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10679.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10679.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10700.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10700.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10710.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10710.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10723.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10728.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10728.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10733.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10733.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10756.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10756.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1077.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10787.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10787.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10789.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10789.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10800.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10800.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10801.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10812.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10812.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10820.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10834.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10834.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10856.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10856.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1086.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1086.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10862.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10862.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10870.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10870.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10871.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10871.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10876.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10876.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10888.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10888.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10889.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10889.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10898.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10898.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10899.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10899.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10900.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10900.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10906.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10906.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1093.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1093.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10942.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10942.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10959.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10959.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10976.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10976.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10995.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x10996.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x10996.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11001.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11001.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1101.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1101.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11011.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11011.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11013.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11013.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11025.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11041.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11041.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11044.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11044.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11159.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11164.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11164.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11186.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11186.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1119.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11204.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11208.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11208.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11212.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11223.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11225.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11225.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11231.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11233.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11233.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11254.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11254.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11258.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11258.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11271.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11294.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11294.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11313.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11313.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11317.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11317.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11318.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11318.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1132.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11339.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11339.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11346.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11354.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11366.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11368.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11368.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11372.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11372.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11417.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11424.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11424.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11426.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11427.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11427.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11428.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11428.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11431.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11431.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11432.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11432.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11454.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11454.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11458.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11473.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11475.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11475.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11485.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11485.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11488.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11493.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11498.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11498.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11499.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11541.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11541.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11562.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11564.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11579.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11579.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11587.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11612.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11612.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1163.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11642.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11642.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11723.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11743.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11743.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11764.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11790.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11790.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11797.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11797.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11798.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11798.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11801.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11809.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11809.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11831.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1187.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1187.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x11894.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x11894.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12025.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12073.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12073.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x12080.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x12080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1226.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1235.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1235.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1237.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1249.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1249.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1308.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1308.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1311.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1311.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1334.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1336.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1348.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1351.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1358.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1374.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1374.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1375.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1380.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1382.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1382.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1384.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1384.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1385.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1386.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1386.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1392.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1402.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1412.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1418.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1418.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1425.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1458.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1478.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x1493.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2052.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2052.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2097.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2097.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2119.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2193.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2540.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2562.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2563.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2563.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2569.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2569.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2572.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2581.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2581.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2600.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2600.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2608.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2608.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2643.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2643.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2646.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2646.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2649.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2649.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2659.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2659.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2694.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2694.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2703.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2703.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2705.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2754.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2754.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2764.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2776.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2776.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2779.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2779.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2908.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2908.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2910.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2910.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2912.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2912.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2929.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2929.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2964.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2964.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x2971.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x2971.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3077.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3080.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3108.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3108.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3110.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3110.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3113.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3113.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3115.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3117.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3117.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3124.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3298.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3298.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3303.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3305.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3324.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3325.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3325.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3333.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3348.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3351.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3359.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/Mpro-x3366.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/Mpro-x3366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/mpro_mols/template.pdb` & `Fragmenstein-1.0.2/fragmenstein/demo/mpro_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/5SB7_mergers.sdf` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/5SB7_mergers.sdf`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/F584.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/F584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/apo_example1.pdb` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/apo_example1.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/dummy.pdb` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/dummy.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/mac-x0138.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/mac-x0398.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/placed_example1.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/placed_example1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/rototoluene.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/rototoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/toluene.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/toluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/transtoluene.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/transtoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/transtoluene2.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/transtoluene2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/x0032_0A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/x0032_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/demo/test_mols/x0103_0A.mol` & `Fragmenstein-1.0.2/fragmenstein/demo/test_mols/x0103_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/display.py` & `Fragmenstein-1.0.2/fragmenstein/display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/divergent_colors.json` & `Fragmenstein-1.0.2/fragmenstein/divergent_colors.json`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/error.py` & `Fragmenstein-1.0.2/fragmenstein/error.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/extraction_funs.py` & `Fragmenstein-1.0.2/fragmenstein/extraction_funs.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/brics.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/brics.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/mcs_monster.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/mcs_monster.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/mcs_victor.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/mcs_victor.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     This is used for benchmarking in the paper. Not for general use.
     """
 
     def _calculate_combination_chem(self):
         """
         The rdkit part. Monster is used to combine the hits.
         """
-        print("modded `_calculate_combination_chem` for `MCSMerger` called")
+        self.journal.info("modded `_calculate_combination_chem` for `MCSMerger` called")
         self._harmonize_warhead_combine()
         # TODO Does combine not need attachment??
         self.monster = MCSMerger(self.hits)
         self.monster.combine(embed_mode=0)
-        # self.monster_throw_on_discard is not applicable
+        # note: self.monster_throw_on_discard check is not applicable here hence absence
+        self.post_monster_step()  # empty overridable
         self.mol = self.monster.positioned_mol
         self.mol.SetProp('_Name', self.monster.merged_name)
         self.smiles = Chem.MolToSmiles(self.mol)
         # making folder.
         self.make_output_folder()
         self.unmatched = []
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/no_pyrosetta.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/no_pyrosetta.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,17 @@
 
     def _calculate_thermo_common(self):
         """
         This method is common to both combination and placement and is unique to Wictor
         as both ``_calculate_combination_thermo`` and ``_calculate_placement_thermo`` are overridden
         and do the same here.
         """
-        # this is a black overridable methods that will be the last thing called
-        # `_correct_ligand_info` requires this info
-        self.monster.positioned_mol = AllChem.AddHs(self.monster.positioned_mol)
-        self.mol = self.monster.positioned_mol
+        # in _calculate_*_chem this was set:
+        # self.mol = self.monster.positioned_mol
+        # I need to assign atom names and stuff still:
         self.params = Params.from_mol(self.mol, name=self.ligand_resn, generic=True)
         self.params.NAME = self.ligand_resn  # force it.
         self.params.polish_mol()
         self.params.comments.clear()
         self.params.comments.append('Generated via Fragmenstein')
         if self.settings['ff_use_neighborhood']:  # default True
             neighborhood = self.monster.get_neighborhood(self.apo_pdbblock,
@@ -84,15 +83,15 @@
         min_result = self.monster.mmff_minimize(self.mol,
                                                 neighborhood=neighborhood,
                                                 ff_max_displacement=float(self.settings['ff_max_displacement']), # def 0
                                                 ff_constraint=int(self.settings['ff_constraint']), # def 10
                                                 ff_max_iterations=int(self.settings['ff_max_iterations']), # def 200
                                                 allow_lax=True)
         self.minimized_mol: Chem.Mol = min_result.mol
-        self.minimized_pdbblock: str = self._plonk_monster_in_structure(prepped_mol=self.mol)
+        self.minimized_pdbblock: str = self._plonk_monster_in_structure(prepped_mol=self.minimized_mol)
         # The ddG is how strained the molecule is out of the protein... not the drop from binding.
         # recalculating:
         # min_result.ideal is with ff_minimise_ideal True
         ideal: Chem.Mol = self.monster.make_ideal_mol(ff_minimise=bool(self.settings['ff_minimise_ideal']))
         if neighborhood: # option ``ff_use_neighborhood`` is False. Why one would do this?
             AllChem.SanitizeMol(neighborhood)
         ideal_E: float = float('nan')
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/others.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/others.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/faux_victors/quick.py` & `Fragmenstein-1.0.2/fragmenstein/faux_victors/quick.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/igor/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/_igor_base.py` & `Fragmenstein-1.0.2/fragmenstein/igor/_igor_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/_igor_init.py` & `Fragmenstein-1.0.2/fragmenstein/igor/_igor_init.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/_igor_min.py` & `Fragmenstein-1.0.2/fragmenstein/igor/_igor_min.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/_igor_utils.py` & `Fragmenstein-1.0.2/fragmenstein/igor/_igor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/igor/pyrosetta_import.py` & `Fragmenstein-1.0.2/fragmenstein/igor/pyrosetta_import.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/_base.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 import operator
 import os
 from typing import (Any, Callable, Union, Iterator, Sequence, List, Dict)
 import pandas as pd
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from ..monster import Monster
-from ..victor import Victor
+from ..victor import Victor as RealVictor  # to avoid confusion
 
 # not needed for binarize... but just in case user is not using them...
 Chem.SetDefaultPickleProperties(Chem.PropertyPickleOptions.AllProps)
 
 def binarize(mol:Chem.Mol, ignore_errors:bool=True) -> bytes:
-    # this is convoluted as None is a common error outcome with RDKit
-    # so making it less cryptic
+    """
+    Wrapper for ``mol.ToBinary(propertyFlags=0b00010111)``, but with safeguards in case it's not a valid Chem.Mol.
+    This is convoluted as None is a common error outcome with RDKit
+    So making it less cryptic
+
+    Note that it will return an empty Chem.Mol binary if it fails, not raise an error
+    That kind of check is for the subprocesses
+    """
     if isinstance(mol, bytes):
         return mol   # messed up. it was bytes.
     elif not isinstance(mol, Chem.Mol): # likely None
         if ignore_errors:
             mol = Chem.Mol()    # noqa
         elif mol is None:
             raise TypeError('A Chem.Mol was expected by got None. '+
@@ -34,14 +40,17 @@
     except KeyboardInterrupt as err:
         raise err
     except exception as error:
         return Chem.Mol().ToBinary(propertyFlags=0b00010111)  # noqa
 
 
 def unbinarize(bin: bytes, ignore_errors:bool=True) -> Union[Chem.Mol, None]:
+    """
+    This is just a wrapper for ``Chem.Mol(bin)``, with safeguards in case it's not a bytes.
+    """
     exception = Exception if ignore_errors else ()
     if isinstance(bin, Chem.Mol):  # lol
         return bin
     elif not isinstance(bin, bytes) and ignore_errors:
         return None
     elif not isinstance(bin, bytes):
         raise TypeError('the molecule binary provide is not a bytes')
@@ -52,15 +61,15 @@
     except exception:
         return None
 
 class LabBench:
 
     # the ``outcome`` column in the pandas dataframe can have these values in order of niceness:
     category_labels = ['crashed', 'too distant', 'timeout', 'unstable', 'equally sized', 'deviant', 'acceptable']
-    Victor = Victor  # So it can be swapped for a subclass w/o the need to subclass Laboratory
+    Victor = RealVictor  # So it can be swapped for a subclass w/o the need to subclass Laboratory
 
     def __init__(self, pdbblock: str,
                  covalent_resi: Union[int, str, None] = None,
                  ligand_resi: Union[str, None]=None,
                  run_plip: bool=False,
                  **settings # for Victor
                  ):
@@ -68,16 +77,20 @@
         self.covalent_resi = covalent_resi
         self.init_options = '-ex1 -ex2 -no_optH false -mute all -ignore_unrecognized_res true -load_PDB_components false'
         self.raw_results = []
         self.ligand_resi = ligand_resi
         self.run_plip = run_plip
         self.blacklist = []  # list of names to skip
         self.settings = settings
-        if not len(Victor.journal.handlers):
-            Victor.enable_stdout(logging.CRITICAL)
+        self.journal = self.Victor.journal
+        if not len(self.journal.handlers):
+            self.Victor.enable_stdout(logging.CRITICAL)
+        # I honestly cannot understand the cause
+        # but the class attribute is not changed in the instance when it's passed to multiprocessing
+        self.Victor = self.__class__.Victor
 
     # keep it just in case: (not called within class as that would require `self.__class__.binarize`)
     binarize: Callable[[Chem.Mol, bool], bytes] = staticmethod(binarize)
     unbinarize: Callable[[bytes, bool], Union[Chem.Mol, None]] = staticmethod(unbinarize)
 
     def get_completed(self, futures: pebble.ProcessMapFuture) -> pd.DataFrame:
         """
@@ -89,31 +102,31 @@
         result_iter: Iterator[int] = futures.result()
         self.raw_results = []
         while True:
             try:
                 result = next(result_iter)
                 self.raw_results.append(result)
             except TimeoutError as error:
-                Victor.journal.error("Function took longer than %d seconds" % error.args[1])
+                self.journal.error("Function took longer than %d seconds" % error.args[1])
                 self.raw_results.append({'error': 'TimeoutError', 'name': ''})
             except StopIteration as error:
                 # it would be nice having a mock entry with the expected values...
                 # self.raw_results.append({})
                 break
             except KeyboardInterrupt as error:
                 print('Keyboard!')
                 self.raw_results.append({'error': 'KeyboardInterrupt', 'name': ''})
                 break
             except Exception as error:
-                Victor.journal.error(f'{error.__class__.__name__}: {error}')
+                self.journal.error(f'{error.__class__.__name__}: {error}')
                 self.raw_results.append({'error': error.__class__.__name__, 'name': ''})
         # list of dict to dataframe
         df = pd.DataFrame(self.raw_results)
         if not len(df) or '∆∆G' not in df.columns:
-            Victor.journal.critical('No results were found. Returning an empty dataframe.')
+            self.journal.critical('No results were found. Returning an empty dataframe.')
             return df
         df['LE'] = df.apply(
             lambda row: - row['∆∆G'] / (row.N_constrained_atoms + row.N_unconstrained_atoms),
             axis=1)
         nan_to_list = lambda value: value if isinstance(value, list) else []
         nan_to_mol = lambda m: m if isinstance(m, Chem.Mol) else Chem.Mol()
         df['disregarded'] = df.disregarded.apply(nan_to_list)  # str
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/_combine.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/_combine.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,28 +16,36 @@
         This is the combination subprocess. The placement subprocess is ``place_subprocess``.
         They are very similar...
         """
         if self.Victor.uses_pyrosetta:
             pyrosetta.distributed.maybe_init(extra_options=self.init_options)
         tentative_name = 'UNKNOWN'
         try:
+            # this works if monster.fix_hits is not neeeded
             hits: List[Chem.Mol] = [hit for hit in map(unbinarize, binary_hits) if hit]
             assert len(hits) > 0, 'No valid hits!'
-            tentative_name = '-'.join([mol.GetProp('_Name') for mol in hits])
-            if tentative_name in self.blacklist:
-                raise ValueError(f'{tentative_name} is blacklisted')
+            assert all([hit.GetNumAtoms() > 0 for hit in hits]), 'Some hits have no atoms!'
+            if all([mol.HasProp('_Name') for mol in hits]):
+                tentative_name = '-'.join([mol.GetProp('_Name') for mol in hits])
+                if tentative_name in self.blacklist:
+                    raise ValueError(f'{tentative_name} is blacklisted')
             # `self.Victor` is likely `Victor` but the user may have switched for a subclass, cf. `VictorMock`...
+            self.journal.debug(f'Using {self.Victor.__name__}')
             victor = self.Victor(hits=hits,
                                  pdb_block=self.pdbblock,
                                  ligand_resn='LIG',
                                  ligand_resi=self.ligand_resi,
                                  covalent_resi=self.covalent_resi,
                                  # a random residue is **still** required for the constaint ref atom.
                                  **self.settings
                                  )
+            # the names may have been fixed by ``monster.fix_hits``
+            tentative_name = '-'.join([mol.GetProp('_Name') for mol in hits])
+            if tentative_name in self.blacklist:
+                raise ValueError(f'{tentative_name} is blacklisted')
             victor.monster_throw_on_discard = True
             victor.monster.throw_on_discard = True
             victor.combine()
             result: dict = victor.summarize()
             result['unmin_binary'] = binarize(victor.monster.positioned_mol)
             result['min_binary'] = binarize(victor.minimized_mol)
             result['hit_binaries'] = [binarize(h) for h in victor.hits]
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/_extras.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/_extras.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/_place.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         if self.Victor.uses_pyrosetta:
             pyrosetta.distributed.maybe_init(extra_options=self.init_options)
         try:
             binary_hits = inputs['binary_hits']
             hits: List[Chem.Mol] = [hit for hit in map(unbinarize, binary_hits) if hit]
             assert len(hits) > 0, 'No valid hits!'
             # `self.Victor` is likely `Victor` but the user may have switched for a subclass, cf. `VictorMock`...
+            self.journal.debug(f'Using {self.Victor.__name__}')
             victor = self.Victor(hits=hits,
                             pdb_block=self.pdbblock,
                             ligand_resn='LIG',
                             ligand_resi=self.ligand_resi,
                             covalent_resi=self.covalent_resi,
                             **self.settings
                             )
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/_score.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/_score.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from rdkit.ML.Cluster import Butina
-from rdkit.Chem import rdMolDescriptors as rdmd
-from rdkit.Chem import Descriptors
-
-from typing import List, Dict, Any, Optional
-import operator, os, re, logging, random, time, argparse, string, itertools, json, contextlib, requests
+import contextlib
+import operator
+from typing import List
 from warnings import warn
-from ..monster import Monster
-import pandas as pd
-import pandera.typing as pdt
-from pandarallel import pandarallel
-from smallworld_api import SmallWorld
-
 
-from rdkit import Chem, rdBase, DataStructs
-from rdkit.Chem import AllChem, Draw, PandasTools, BRICS
-from rdkit.Chem.Draw import IPythonConsole
+import pandas as pd
+from rdkit import Chem, DataStructs
+from rdkit.Chem import AllChem, PandasTools
 from rdkit.Chem import rdFingerprintGenerator as rdfpg
+from rdkit.Chem import rdMolDescriptors as rdmd
 from rdkit.Chem.rdfiltercatalog import FilterCatalogParams, FilterCatalog, FilterCatalogEntry
+from rdkit.ML.Cluster import Butina
+
 from .._cli_defaults import cli_default_settings
+from ..monster import Monster
 
 # ----- Scoring -----------------------------------
 params = FilterCatalogParams()
 params.AddCatalog(FilterCatalogParams.FilterCatalogs.PAINS)
 catalog = FilterCatalog(params)
 
 def get_pains(mol) -> List[str]:
@@ -118,14 +113,23 @@
                 if col not in row.index:
                     warn(f'{col} column is missing from df')
                     continue
                 penalty += row[col] * w if str(row[col]) != 'nan' else self.nan_penalty
             return penalty
         return float('nan')
 
+    def make_weighted_df(self, df) -> pd.DataFrame:
+        """
+        Inspect whether the weights make sense
+        """
+        weighted = pd.DataFrame({k: df[k] * w for k, w in self.weights.items()})
+        weighted['total'] = df.apply(self, axis=1)
+        weighted.sort_values('total')
+        return weighted
+
 
 def butina_cluster(mol_list, cutoff=0.35):
     # https://github.com/PatWalters/workshop/blob/master/clustering/taylor_butina.ipynb
     fp_list = [rdmd.GetMorganFingerprintAsBitVect(AllChem.RemoveAllHs(m), 3, nBits=2048) for m in mol_list]
     dists = []
     nfps = len(fp_list)
     for i in range(1, nfps):
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/laboratory/validator.py` & `Fragmenstein-1.0.2/fragmenstein/laboratory/validator.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/legacy.py` & `Fragmenstein-1.0.2/fragmenstein/legacy.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/m_rmsd.py` & `Fragmenstein-1.0.2/fragmenstein/m_rmsd.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/mol3d_display.py` & `Fragmenstein-1.0.2/fragmenstein/mol3d_display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/monster/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_base.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_collapse_ring.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_collapse_ring.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_combine.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_communal.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_communal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_ff.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_ff.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
         for atom in conserved:
             i = atom.GetIdx()
             if atom.GetAtomicNum() == 1:
                 # let hydrogens move
                 continue
             elif fixed_mode:
                 ff.AddFixedPoint(i)
+            elif (atom.GetProp('_isRing') if atom.HasProp('_isRing') else False):
+                # be 5-fold more lax with rings
+                ff.MMFFAddPositionConstraint(i, maxDispl=ff_max_displacement, forceConstant=ff_constraint/2)
             else:
                 # https://github.com/rdkit/rdkit/blob/115317f43e3bdfd73673ca0e4c6b4035aa26a034/Code/ForceField/UFF/PositionConstraint.cpp#L35
                 ff.MMFFAddPositionConstraint(i, maxDispl=ff_max_displacement, forceConstant=ff_constraint)
             restrained.append(i)
         # constrain dummy atoms
         for atom in mol.GetAtomsMatchingQuery(rdqueries.HasPropQueryAtom('_IsDummy')):
             i = atom.GetIdx()
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_join_neighboring.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_join_neighboring.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_merge.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_merge.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_modification_logging.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_modification_logging.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     """
 
     def place(self,
               mol: Chem.Mol,
               attachment: Optional[Chem.Mol] = None,
               custom_map: Optional[Dict[str, Dict[int, int]]] = None,
               merging_mode: str = 'expansion',
-              enforce_warhead_mapping:bool=True):
+              enforce_warhead_mapping:bool=True,
+              primary_name=None):
         """
         Positioned a given mol based on the hits. (Main entrypoint)
         accepts the argument `merging_mode`, by default it is "expansion",
         but was "permissive_none",
         which call `.by_expansion` and `.no_blending(broad=True)` respectively.
         "off" (does nothing except fill the attribute ``initial_mol``),
         "full" (`.full_blending()`),
@@ -47,14 +48,15 @@
         and "none" (`.no_blending()`, but less thorough)
         are accepted.
 
         :param mol:
         :param attachment: This the SG of the cysteine if covalent
         :param custom_map: Dict of hit_name to Dict of hit_idx to followup_idx
         :param merging_mode:
+        :param primary_name: override the name of the primary hit if merging_mode is 'expansion'
         :return:
         """
         if not mol.HasProp('_Name'):
             mol.SetProp('_Name', 'followup')
         assert not any([mol.GetProp('_Name') == h.GetProp('_Name') for h in self.hits]), \
             'Placement has the same name as a hit!'
         self.initial_mol, self.attachment = self._parse_mol_for_place(mol, attachment)
@@ -77,15 +79,15 @@
         elif merging_mode == 'partial':
             self.partial_blending()
         elif merging_mode == 'none_permissive' or merging_mode == 'permissive_none':
             self.no_blending(broad=True)
         elif merging_mode == 'none':
             self.no_blending()
         elif merging_mode == 'expansion':
-            self.by_expansion()
+            self.by_expansion(primary_name)
         else:
             valid_modes = ('full', 'partial', 'none', 'none_permissive', 'off', 'expansion')
             raise ValueError(
                 f"Merging mode can only be {'| '.join(valid_modes)}, not '{merging_mode}'")
         return self
 
     def place_smiles(self,
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_expand.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_expand.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_full.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_full.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_make_chimera.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_make_chimera.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_mappings.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_mappings.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_no_blending.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_no_blending.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_partial.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_partial.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_place_modes/_refine.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_place_modes/_refine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_util_compare.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_util_compare.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/_utility.py` & `Fragmenstein-1.0.2/fragmenstein/monster/_utility.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/bond_provenance.py` & `Fragmenstein-1.0.2/fragmenstein/monster/bond_provenance.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/compare_atom.py` & `Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/compare_atom.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/types.py` & `Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/types.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/mcs_mapping/utils.py` & `Fragmenstein-1.0.2/fragmenstein/monster/mcs_mapping/utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/positional_mapping.py` & `Fragmenstein-1.0.2/fragmenstein/monster/positional_mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/monster/unmerge_mapper.py` & `Fragmenstein-1.0.2/fragmenstein/monster/unmerge_mapper.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/mpro/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/mpro/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/mpro/dataframe.py` & `Fragmenstein-1.0.2/fragmenstein/mpro/dataframe.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/multivictor/multivictor.py` & `Fragmenstein-1.0.2/fragmenstein/multivictor/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/ngl_display.py` & `Fragmenstein-1.0.2/fragmenstein/ngl_display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/openmm/fritz.py` & `Fragmenstein-1.0.2/fragmenstein/openmm/fritz.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/openmm/openvictor.py` & `Fragmenstein-1.0.2/fragmenstein/openmm/openvictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     def _calculate_placement_thermo(self):
         return self._calculate_thermo()
 
     def _calculate_thermo(self):
         if self.is_covalent:
             raise NotImplementedError('OpenVictor does not support covalent ligands')
         self.journal.debug(f'{self.long_name} - Starting system setup')
-        self.mol = AllChem.AddHs(self.monster.positioned_mol, addCoords=True)
+        # in _calculate_*_chem this was set:
+        # self.mol = self.monster.positioned_mol
         restraint_k = self.settings['mm_restraint_k'] # default 1000.
         tolerance = self.settings['mm_tolerance']  # 10 * mmu.kilocalorie_per_mole / (mmu.nano * mmu.meter)
         maxIterations = self.settings['mm_max_iterations'] # 0 is infinite
         self.fritz = Fritz(prepped_mol=self.preminimized_undummied_mol,
                            pdb_block=self.apo_pdbblock,
                            resn=self.ligand_resn,
                            restraining_atom_indices=self._get_restraining_atom_indices(),
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/settings.py` & `Fragmenstein-1.0.2/fragmenstein/settings.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/version.py` & `Fragmenstein-1.0.2/fragmenstein/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from typing import Dict
 def get_versions() -> Dict[str, str]:
     """
     Return a dict of versions of os, python, fragmenstein etc.
     """
     import pkg_resources, sys, platform
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/victor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
     :vartype long_name: str
     :ivar merging_mode:
     :vartype merging_mode: str
     :ivar minimized_mol:
     :vartype minimized_mol: Mol
     :ivar minimized_pdbblock:
     :vartype minimized_pdbblock: str
-    :ivar mmerging_mode:
-    :vartype mmerging_mode: str
+    :ivar merging_mode:
+    :vartype mmrging_mode: str
     :ivar modifications:
     :vartype modifications: dict
     :ivar mol:
     :vartype mol: Mol
     :ivar monster:
     :vartype monster: Monster
     :cvar monster_average_position:
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_loggerwriter.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_loggerwriter.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_base.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,40 +147,41 @@
         self.covalent_resi = covalent_resi
         self._correct_covalent_resi()  # noqa defined in plonk. todo: split into covalent and anchor residue.
         self.extra_constraint = extra_protein_constraint
         self.pose_fx = pose_fx
         self.random_seed = monster_random_seed
         self.settings = {**default_settings, **settings}
         self._process_settings()
+        # this is readied in case user wants to change it:
+        self.monster = self.Monster(hits,
+                                    average_position=self.monster_average_position,
+                                    random_seed=self.random_seed)
         # ## Fill by place and combine differently
-        self.long_name = 'ligand'
+        self.long_name: str = 'ligand'
         self.smiles = None
         # ## Filled by place
-        self.merging_mode = "none_permissive"
+        self.merging_mode = "not_set"
         self.custom_map = {}  # this will be fixed in monster by `.fix_custom_map`
         # ## Filled by combine
         self.joining_cutoff = None
         # ## Calculated
         self.is_covalent = None
-        self.params = None
-        self.mol = None
-        self.constraint = None
+        self.params = None  # this will be the rdkit_to_params.Params instance
+        self.mol = None   # this will be the unminimised mol
+        self.constraint = None  # Rosetta string-form constraint defs
         self.modifications = {}
         self.unminimized_pdbblock = None
-        self.monster = self.Monster(hits,
-                                    average_position=self.monster_average_position,
-                                    random_seed=self.random_seed)
         self.monster.throw_on_discard = self.monster_throw_on_discard
         self.igor = None
         self.unbound_pose = None
         self.minimized_pdbblock = None
         self.minimized_mol = None
         self.reference_mol = None  # filled only for validate
         # buffers etc.
-        self._warned = []
+        self._warned = warnings.catch_warnings()  # new one will be made. here for clarify
         self.energy_score = {'bound': {'total_score': float('nan')},
                              'unbound': {'total_score': float('nan')}}
         self.mrmsd = mRMSD.mock()
         self.ddG = float('nan')
         # for debug purposes
         self.tick = time.time()
         self.tock = float('inf')
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_combine.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_combine.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         # making folder.
         self.make_output_folder()
 
     def _calculate_combination_thermo(self):
         # paramterise
         self.journal.debug(f'{self.long_name} - Starting parameterisation')
         # ``Params.load_mol`` does a few things: ``from_mol``, the ``polish_mol`` ad then ``convert_mol``.
-        # here it is split up.
+        # here it is split up for clarity mostly
         self.params = Params.from_mol(self.mol, name=self.ligand_resn, generic=False)
         self.params.NAME = self.ligand_resn  # force it.
         self.params.polish_mol()
         self.params.comments.clear()
         self.params.comments.append('Generated via Fragmenstein')
         # get constraint
         self.constraint = self._get_constraint(self.extra_constraint)
@@ -130,15 +130,15 @@
         #self.params.add_Hs()  # already done by rectify
         self.params.add_conformer()
         self.params.convert_mol()
         # self.journal.warning(f'{self.long_name} - CHI HAS BEEN DISABLED')
         # self.params.CHI.data = []  # TODO check if chi fix is okay
         self._log_warnings()
         self.post_params_step()  # empty overridable
-        self.mmerging_mode = 'full' #TODO: check if this is intended
+        self.merging_mode = 'full'
         self.unminimized_pdbblock = self._plonk_monster_in_structure()
         params_file, holo_file, constraint_file = self._save_prerequisites()
         self.unbound_pose = self.params.test()
         self._checkpoint_alpha()
         self._checkpoint_bravo()
         self.pre_igor_step()  # empty overridable
         self.igor = Igor.from_pdbblock(pdbblock=self.unminimized_pdbblock,
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_common.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_common.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_igor.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_igor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_journal.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_journal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_overridables.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_overridables.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_place.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_place.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,16 +110,18 @@
         :return:
         '''
         # check they are okay
         self._assert_placement_inputs()
         # ***** PARAMS & CONSTRAINT *******
         self.journal.info(f'{self.long_name} - Starting work')
         self._log_warnings()
+        # self.mol will be replaced by the output of self.monster.positioned_mol
         if self.uses_pyrosetta:
             # self.params from _prepare_args_for_placement
+            # Don't worry: the coordinates will be ignored.
             self.mol = self.params.mol
         else:
             # `self.params.mol` adds hydrogens and atoms names
             self.mol = AllChem.AddHs(Chem.MolFromSmiles(self.smiles))
         self._log_warnings()
         # get constraint
         attachment = self._get_attachment_from_pdbblock() if self.is_covalent else None
@@ -129,14 +131,15 @@
         self.journal.debug(f'{self.long_name} - Starting fragmenstein')
         # monster_throw_on_discard controls if disconnected.
         self.monster.place(mol=self.mol,
                            attachment=attachment,
                            merging_mode=self.merging_mode,
                            custom_map=self.custom_map)
         self.post_monster_step()  # empty overridable
+        self.mol = self.monster.positioned_mol
         self.journal.debug(f'{self.long_name} - Tried {len(self.monster.mol_options)} combinations')
 
     def _calculate_placement_thermo(self):
         '''
         Second and last part of the placement pipeline.
           1) Plonks the monster in the structure
           2) Energy minimization ligand-protein
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_plonk.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_plonk.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,20 +33,22 @@
                 f'{cx} {self.ligand_resn} {l_chain} {l_resi: >3}     1555   1555  1.8\n'
         else:
             return ''
 
     def _correct_ligand_info(self, mol: Optional[Chem.Mol] = None) -> Chem.Mol:
         """
         Corrects in place the given mol based on self.ligand_resi.
-        If none provided it assumed self.monster.positioned_mol
+        If none provided it assumes ``self.mol`` (which in most cases is ``self.monster.positioned_mol``)
         Correcting the serial unfortunately does not do anything.
+
+        Called by ``._plonk_monster_in_structure_minimal`` (a route of ``._plonk_monster_in_structure``)
         """
         i = 0
         if mol is None:
-            mol = self.monster.positioned_mol
+            mol = self.mol
         l_resi, l_chain = re.match('(\d+)(\D?)', str(self.ligand_resi)).groups()  # TODO improve ligand_resi
         for atom in mol.GetAtoms():
             info = atom.GetPDBResidueInfo()
             if info is None:
                 i += 1
                 self.journal.warning(f'The atom #{atom.GetIdx()} has no PDB information in RDKit')
                 info = Chem.AtomPDBResidueInfo(atomName=f'X{i: <3}')
@@ -54,15 +56,22 @@
             info.SetChainId(l_chain)
             info.SetIsHeteroAtom(True)
             info.SetOccupancy(1.)
             info.SetResidueName(self.ligand_resn)
         return mol
 
     def _plonk_monster_in_structure(self, prepped_mol: Optional[Chem.Mol]=None, use_pymol=False):
-        prepped_mol = self._correct_ligand_info(prepped_mol)
+        """
+        Plonks the molecule in the structure. This is most likely self.mol
+        ``_correct_ligand_info`` will accept Chem.Mol or None (it will use self.mol).
+        As the preminimisation is all that happens in Wictor, the prepped_mol is passed.
+        """
+        # this is in place on ``prepped_mol`` or ``self.mol`` (None case).
+        # Passing its returned value to prepped_mol will result in minimisation being skipped (as its prepped already)
+        self._correct_ligand_info(prepped_mol)
         self.journal.debug(f'{self.long_name} - placing monster in structure')
         if use_pymol:
             return self._plonk_monster_in_structure_pymol()
         else:
             # _plonk_monster_in_structure_raw does no corrections.
             return self._plonk_monster_in_structure_minimal(prepped_mol)
 
@@ -72,15 +81,15 @@
         This cached property is the preminimised molecule.
         It extracts the neighbourhood (``monster.get_neighborhood``) and
         minimises the molecule (``monster.mmff_minimize``)
 
         This method is called by the plonking into structure methods.
         Not "positioning" as intended by ``monster`` is done.
         """
-        mol = Chem.Mol(self.monster.positioned_mol)
+        mol = Chem.Mol(self.mol)
         if self.monster_mmff_minisation:
             self.journal.debug(f'{self.long_name} - pre-minimising monster (MMFF)')
             if self.settings.get('ff_use_neighborhood', True):
                 neighborhood = self.monster.get_neighborhood(self.apo_pdbblock, cutoff=self.settings['ff_neighborhood'], addHs=True)
             else:
                 neighborhood = None
             # ff_max_displacement = float('nan') for fixed mode
@@ -103,15 +112,18 @@
         """
         Plonks the molecule in the structure without using pymol.
         Uses a custom miniparser. see minimalPDB.MinimalPDBParser
 
         :return:
         """
         # ----- load
-        mol = self.preminimized_undummied_mol if prepped_mol is None else AllChem.DeleteSubstructs(prepped_mol, Chem.MolFromSmiles('*'))
+        if prepped_mol is None:
+            mol = self.preminimized_undummied_mol
+        else:  # this was passed by the user, fixing dummies just in case
+            mol = AllChem.DeleteSubstructs(prepped_mol, Chem.MolFromSmiles('*'))
         pdbdata = MinimalPDBParser(self.apo_pdbblock, remove_other_hetatms=self.remove_other_hetatms,
                                    ligname=self.ligand_resn)
         moldata = MinimalPDBParser(Chem.MolToPDBBlock(mol))
         # ------- covalent fix
         if self.is_covalent:
             pdbdata.headers.append(self._get_LINK_record())
         # ------- assertions
```

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_safety.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_safety.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_show.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_show.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_store.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_store.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_utils.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/_victor_validate.py` & `Fragmenstein-1.0.2/fragmenstein/victor/_victor_validate.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/minimalPDB.py` & `Fragmenstein-1.0.2/fragmenstein/victor/minimalPDB.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/victor/plip.py` & `Fragmenstein-1.0.2/fragmenstein/victor/plip.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/__init__.py` & `Fragmenstein-1.0.2/fragmenstein/walton/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/_advmoves.py` & `Fragmenstein-1.0.2/fragmenstein/walton/_advmoves.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/_art.py` & `Fragmenstein-1.0.2/fragmenstein/walton/_art.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/_base.py` & `Fragmenstein-1.0.2/fragmenstein/walton/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/_movements.py` & `Fragmenstein-1.0.2/fragmenstein/walton/_movements.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/fragmenstein/walton/_polygon.py` & `Fragmenstein-1.0.2/fragmenstein/walton/_polygon.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/requirements.txt` & `Fragmenstein-1.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/setup.py` & `Fragmenstein-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '1.0.1'
+version = '1.0.2'
 
 
 from setuptools import setup, find_packages
 from warnings import warn
 from importlib import util
 import os
```

### Comparing `Fragmenstein-1.0.1/tests/MPro_combine.py` & `Fragmenstein-1.0.2/tests/MPro_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/MPro_place.py` & `Fragmenstein-1.0.2/tests/MPro_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/baffled.py` & `Fragmenstein-1.0.2/tests/baffled.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/cli.py` & `Fragmenstein-1.0.2/tests/cli.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/dummy_victor.py` & `Fragmenstein-1.0.2/tests/dummy_victor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/internals.py` & `Fragmenstein-1.0.2/tests/internals.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/lab.py` & `Fragmenstein-1.0.2/tests/lab.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/mapping.py` & `Fragmenstein-1.0.2/tests/mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/monster_combine.py` & `Fragmenstein-1.0.2/tests/monster_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/monster_place.py` & `Fragmenstein-1.0.2/tests/monster_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/multivictor.py` & `Fragmenstein-1.0.2/tests/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/problems.py` & `Fragmenstein-1.0.2/tests/problems.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/victor_combine.py` & `Fragmenstein-1.0.2/tests/victor_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/victor_discard.py` & `Fragmenstein-1.0.2/tests/victor_discard.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-1.0.1/tests/walton.py` & `Fragmenstein-1.0.2/tests/walton.py`

 * *Files identical despite different names*

