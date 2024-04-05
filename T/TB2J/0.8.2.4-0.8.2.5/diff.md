# Comparing `tmp/TB2J-0.8.2.4.tar.gz` & `tmp/TB2J-0.8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.8.2.4.tar", last modified: Mon Mar 18 09:11:37 2024, max compression
+gzip compressed data, was "TB2J-0.8.2.5.tar", last modified: Fri Apr  5 14:41:07 2024, max compression
```

## Comparing `TB2J-0.8.2.4.tar` & `TB2J-0.8.2.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.8.2.4/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/
--rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/Jdownfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/Jtensor.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3595 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/Oiju.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7332 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/Oiju_epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       24 2024-03-18 09:11:07.000000 TB2J-0.8.2.4/TB2J/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/abacus/
--rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/abacus_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-03-08 15:04:05.000000 TB2J-0.8.2.4/TB2J/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/gen_exchange_abacus.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/orbital_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.8.2.4/TB2J/abacus/stru_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/abacus/test_read_stru.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/TB2J/basis.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/citation.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/contour.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/density_matrix.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    30315 2024-03-14 08:51:41.000000 TB2J-0.8.2.4/TB2J/exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11350 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/exchangeCL2.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8521 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/exchange_pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/exchange_qspace.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/external/
--rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/external/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/external/p_tqdm.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/gpaw_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    13169 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/green.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/greentest.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/io_exchange/
--rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.8.2.4/TB2J/io_exchange/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-03-14 09:47:11.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_multibinit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_tomsasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_txt.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_uppasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/io_exchange/io_vampire.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15265 2024-03-08 15:04:05.000000 TB2J-0.8.2.4/TB2J/io_merge.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15817 2024-03-18 09:10:54.000000 TB2J-0.8.2.4/TB2J/manager.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/mathutils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    17721 2024-03-04 10:09:47.000000 TB2J-0.8.2.4/TB2J/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/orbmap.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/pauli.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/plot.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3031 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/rotate_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-03-18 09:10:54.000000 TB2J-0.8.2.4/TB2J/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/spinham/
--rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.8.2.4/TB2J/spinham/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/base_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/constants.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/hamiltonian.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/qsolver.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/spin_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/spin_xml.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/spinham/supercell.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/tensor_rotate.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/utest.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-03-18 09:04:29.000000 TB2J-0.8.2.4/TB2J/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/TB2J/versioninfo.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.8.2.4/TB2J/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.8.2.4/TB2J/wannier/w90_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.8.2.4/TB2J/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/TB2J.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-03-18 09:11:37.000000 TB2J-0.8.2.4/TB2J.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1747 2024-03-18 09:11:37.000000 TB2J-0.8.2.4/TB2J.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-03-18 09:11:37.000000 TB2J-0.8.2.4/TB2J.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-03-18 09:11:37.000000 TB2J-0.8.2.4/TB2J.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-03-18 09:11:37.000000 TB2J-0.8.2.4/TB2J.egg-info/top_level.txt
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_downfold.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_eigen.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_magnon.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_magnon_dos.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1636 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_merge.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      648 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/TB2J_rotate.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.8.2.4/scripts/abacus2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4720 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/siesta2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     6534 2024-02-28 11:18:04.000000 TB2J-0.8.2.4/scripts/wann2J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-03-18 09:11:37.396366 TB2J-0.8.2.4/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)     1952 2024-03-18 09:10:59.000000 TB2J-0.8.2.4/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3595 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7332 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       24 2024-04-05 14:40:14.000000 TB2J-0.8.2.5/TB2J/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/abacus/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/abacus_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/TB2J/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/gen_exchange_abacus.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/orbital_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.8.2.5/TB2J/abacus/stru_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/test_read_stru.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/basis.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/density_matrix.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    30380 2024-04-05 14:38:23.000000 TB2J-0.8.2.5/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11350 2024-04-05 14:37:55.000000 TB2J-0.8.2.5/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8521 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    13169 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.8.2.5/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-03-27 09:14:31.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15265 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15817 2024-03-18 09:10:54.000000 TB2J-0.8.2.5/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/mathutils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17721 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3031 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-03-18 09:10:54.000000 TB2J-0.8.2.5/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.8.2.5/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/base_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/spin_xml.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/tensor_rotate.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-03-18 09:04:29.000000 TB2J-0.8.2.5/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.8.2.5/TB2J/wannier/w90_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/wannier/w90_tb_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1747 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_magnon_dos.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1636 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      648 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_rotate.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/scripts/abacus2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4720 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     6534 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1952 2024-04-05 14:40:20.000000 TB2J-0.8.2.5/setup.py
```

### Comparing `TB2J-0.8.2.4/LICENSE` & `TB2J-0.8.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/PKG-INFO` & `TB2J-0.8.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.4
+Version: 0.8.2.5
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.4/README.md` & `TB2J-0.8.2.5/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/Jdownfolder.py` & `TB2J-0.8.2.5/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/Jtensor.py` & `TB2J-0.8.2.5/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/Oiju.py` & `TB2J-0.8.2.5/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/Oiju_epc.py` & `TB2J-0.8.2.5/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/abacus_api.py` & `TB2J-0.8.2.5/TB2J/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/abacus_wrapper.py` & `TB2J-0.8.2.5/TB2J/abacus/abacus_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/gen_exchange_abacus.py` & `TB2J-0.8.2.5/TB2J/abacus/gen_exchange_abacus.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/orbital_api.py` & `TB2J-0.8.2.5/TB2J/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/stru_api.py` & `TB2J-0.8.2.5/TB2J/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/test_read_HRSR.py` & `TB2J-0.8.2.5/TB2J/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/abacus/test_read_stru.py` & `TB2J-0.8.2.5/TB2J/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/basis.py` & `TB2J-0.8.2.5/TB2J/basis.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/citation.py` & `TB2J-0.8.2.5/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/contour.py` & `TB2J-0.8.2.5/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/density_matrix.py` & `TB2J-0.8.2.5/TB2J/density_matrix.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/epc.py` & `TB2J-0.8.2.5/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/exchange.py` & `TB2J-0.8.2.5/TB2J/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     def _prepare_Jorb_file(self):
         os.makedirs(self.output_path, exist_ok=True)
         self.orbpath = os.path.join(self.output_path, "OrbResolve")
         os.makedirs(self.orbpath, exist_ok=True)
 
     def _adjust_emin(self):
         self.emin = self.G.find_energy_ingap(rbound=self.efermi - 5.0) - self.efermi
+        print(f"A gap is found at {self.emin}, set emin to it.")
 
     def set_tbmodels(self, tbmodels):
         pass
 
     def _clean_tbmodels(self):
         del self.tbmodel
         del self.G.tbmodel
```

### Comparing `TB2J-0.8.2.4/TB2J/exchangeCL2.py` & `TB2J-0.8.2.5/TB2J/exchangeCL2.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/exchange_pert.py` & `TB2J-0.8.2.5/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/exchange_qspace.py` & `TB2J-0.8.2.5/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/external/p_tqdm.py` & `TB2J-0.8.2.5/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/gpaw_wrapper.py` & `TB2J-0.8.2.5/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/green.py` & `TB2J-0.8.2.5/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/greentest.py` & `TB2J-0.8.2.5/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_exchange.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_txt.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_exchange/io_vampire.py` & `TB2J-0.8.2.5/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/io_merge.py` & `TB2J-0.8.2.5/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/kpoints.py` & `TB2J-0.8.2.5/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/manager.py` & `TB2J-0.8.2.5/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/myTB.py` & `TB2J-0.8.2.5/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/orbmap.py` & `TB2J-0.8.2.5/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/pauli.py` & `TB2J-0.8.2.5/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/pert.py` & `TB2J-0.8.2.5/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/plot.py` & `TB2J-0.8.2.5/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/rotate_atoms.py` & `TB2J-0.8.2.5/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/sisl_wrapper.py` & `TB2J-0.8.2.5/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/base_parser.py` & `TB2J-0.8.2.5/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/constants.py` & `TB2J-0.8.2.5/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/hamiltonian.py` & `TB2J-0.8.2.5/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.8.2.5/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/plot.py` & `TB2J-0.8.2.5/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/qsolver.py` & `TB2J-0.8.2.5/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/spin_api.py` & `TB2J-0.8.2.5/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/spin_xml.py` & `TB2J-0.8.2.5/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/spinham/supercell.py` & `TB2J-0.8.2.5/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/tensor_rotate.py` & `TB2J-0.8.2.5/TB2J/tensor_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/utest.py` & `TB2J-0.8.2.5/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/utils.py` & `TB2J-0.8.2.5/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/wannier/w90_parser.py` & `TB2J-0.8.2.5/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J/wannier/w90_tb_parser.py` & `TB2J-0.8.2.5/TB2J/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/TB2J.egg-info/PKG-INFO` & `TB2J-0.8.2.5/TB2J.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.4
+Version: 0.8.2.5
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.4/TB2J.egg-info/SOURCES.txt` & `TB2J-0.8.2.5/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/TB2J_downfold.py` & `TB2J-0.8.2.5/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/TB2J_eigen.py` & `TB2J-0.8.2.5/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/TB2J_magnon.py` & `TB2J-0.8.2.5/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/TB2J_merge.py` & `TB2J-0.8.2.5/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/TB2J_rotate.py` & `TB2J-0.8.2.5/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/abacus2J.py` & `TB2J-0.8.2.5/scripts/abacus2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/siesta2J.py` & `TB2J-0.8.2.5/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/scripts/wann2J.py` & `TB2J-0.8.2.5/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.4/setup.py` & `TB2J-0.8.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.8.2.4"
+__version__ = "0.8.2.5"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name="TB2J",
     version=__version__,
     description="TB2J: First principle to Heisenberg exchange J using tight-binding Green function method",
```

