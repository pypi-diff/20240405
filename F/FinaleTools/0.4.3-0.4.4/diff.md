# Comparing `tmp/FinaleTools-0.4.3.tar.gz` & `tmp/FinaleTools-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinaleTools-0.4.3.tar", last modified: Mon Apr  1 20:44:27 2024, max compression
+gzip compressed data, was "FinaleTools-0.4.4.tar", last modified: Fri Apr  5 05:05:04 2024, max compression
```

## Comparing `FinaleTools-0.4.3.tar` & `FinaleTools-0.4.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.3/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.3/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-01 20:28:58.000000 FinaleTools-0.4.3/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.3/src/finaletools/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24643 2024-04-01 20:31:34.000000 FinaleTools-0.4.3/src/finaletools/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8349 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14184 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.3/src/finaletools/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.3/src/finaletools/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18313 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.4/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.4/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-05 04:59:24.000000 FinaleTools-0.4.4/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/FinaleTools.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.4/src/finaletools/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24678 2024-04-04 19:34:39.000000 FinaleTools-0.4.4/src/finaletools/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/agg_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.4/src/finaletools/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7546 2024-04-04 20:18:22.000000 FinaleTools-0.4.4/src/finaletools/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.4/src/finaletools/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14184 2024-04-04 19:21:37.000000 FinaleTools-0.4.4/src/finaletools/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.4/src/finaletools/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.4/src/finaletools/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.4/src/finaletools/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:03.000000 FinaleTools-0.4.4/src/finaletools/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-05 05:05:04.000000 FinaleTools-0.4.4/src/finaletools/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.4/src/finaletools/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18301 2024-04-04 20:13:31.000000 FinaleTools-0.4.4/src/finaletools/utils/utils.py
```

### Comparing `FinaleTools-0.4.3/LICENSE` & `FinaleTools-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/PKG-INFO` & `FinaleTools-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.3
+Version: 0.4.4
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.3/README.md` & `FinaleTools-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/pyproject.toml` & `FinaleTools-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleTools"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `FinaleTools-0.4.3/src/FinaleTools.egg-info/PKG-INFO` & `FinaleTools-0.4.4/src/FinaleTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.3
+Version: 0.4.4
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `FinaleTools-0.4.3/src/FinaleTools.egg-info/SOURCES.txt` & `FinaleTools-0.4.4/src/FinaleTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/cli/main_cli.py` & `FinaleTools-0.4.4/src/finaletools/cli/main_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     # Common arguments
 
     # Subcommand 1: frag-coverage
     parser_command1 = subparsers.add_parser(
         'coverage',
         description=(
         'Calculates fragmentation coverage over intervals in a BED file given '
-        'a BAM/SAM file'
+        'a SAM, BAM, CRAM, or Frag.gz file'
         )
     )
     # TODO: accept tabix
 
     parser_command1.add_argument(
         'input_file',
-        help='BAM or SAM file containing fragment data'
+        help='SAM, BAM, CRAM, or Frag.gz file containing fragment data'
     )
     parser_command1.add_argument(
         'interval_file',
         help='BED file containing intervals over which coverage is calculated'
     )
     parser_command1.add_argument(
         '-o',
```

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/adjust_wps.py` & `FinaleTools-0.4.4/src/finaletools/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/agg_wps.py` & `FinaleTools-0.4.4/src/finaletools/frag/agg_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/cleavage_profile.py` & `FinaleTools-0.4.4/src/finaletools/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/coverage.py` & `FinaleTools-0.4.4/src/finaletools/frag/coverage.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 from multiprocessing import Pool
 
 import pysam
 import gzip
 from tqdm import tqdm
 
 from finaletools.utils.utils import (
-    _not_read1_or_low_quality, _get_contigs, _get_intervals
+    _not_read1_or_low_quality, _get_contigs, _get_intervals, frag_generator
 )
 
 
 def single_coverage(
         input_file: Union[str, pysam.AlignmentFile],
         contig: str=None,
         start: int=0,
         stop: int=None,
         name: str='.',
+        intersect_policy: str="midpoint",
         quality_threshold: int=30,
         verbose: Union[bool, int]=False
     ) -> Tuple[str, int, int, str, float]:
     """
     Return estimated fragment coverage over specified `contig` and
     region of`input_file`. Uses an algorithm where the midpoints of
     fragments are calculated and coverage is tabulated from the
     midpoints that fall into the specified region. Not suitable for
     fragments of size approaching region size.
 
     Parameters
     ----------
     input_file : str or pysam.AlignmentFile
-        BAM, SAM, or CRAM file containing paired-end fragment reads or
+        BAM, SAM, CRAM, or Frag.gz file containing paired-end fragment reads or
         its path. `AlignmentFile` must be opened in read mode.
     contig : string
     start : int
     stop : int
     name : str
     quality_threshold : int, optional
     verbose : bool, optional
@@ -47,60 +48,47 @@
     coverage : int
         Fragment coverage over contig and region.
     """
     # TODO: determine if reference (like as found in pysam) is necessary
     # TODO: consider including region string (like in pysam)
     if verbose:
         start_time = time.time()
+        tqdm.write(
+            f"""
+input_file: 
+contig: {contig}
+start: {start}
+stop: {stop}
+name: {name}
+intersect_policy: {intersect_policy}
+quality_threshold: {quality_threshold}
+verbose: {verbose}
+"""
+        )
 
     # initializing variable for coverage tuple outside of with statement
     coverage = 0
 
     input_type = type(input_file)
 
-    try:
-        # Handling different input types
-        if input_type == pysam.AlignmentFile:
-            sam_file = input_file
-        elif input_type == str:
-            sam_file = pysam.AlignmentFile(input_file, 'r')
-        else:
-            raise TypeError('input_file should be str or pysam.AlignmentFile')
-
-        # Iterating on each read in file in
-        # specified contig/chromosome
-        for read1 in sam_file.fetch(
-            contig=contig,
-            start=0 if (tempstart:=start-500) < 0 else tempstart,
-            stop=stop+500 if stop is not None else None
-        ):
-            # Only select forward strand and filter out
-            # non-paired-end reads and low-quality reads
-            if _not_read1_or_low_quality(read1, quality_threshold):
-                pass
-            else:
-                # calculate mid-point of fragment
-                center = read1.reference_start + read1.template_length // 2
-                if start is None and stop is None:
-                    coverage += 1
-                elif start is None:
-                    if center < stop:
-                        coverage += 1
-                elif stop is None:
-                    if center >= start:
-                        coverage += 1
-                elif (center >= start) and (center < stop):
-                    coverage += 1
-                else:
-                    pass
-    finally:
-        if input_type == str:
-            sam_file.close()
-
-
+    frags = frag_generator(
+        input_file=input_file,
+        contig=contig,
+        quality_threshold=quality_threshold,
+        start=start,
+        stop=stop,
+        fraction_low=10,
+        fraction_high=10000000,
+        intersect_policy=intersect_policy)
+
+    # Iterating on each frag in file in
+    # specified contig/chromosome
+    for frag in frags:
+        coverage += 1
+        
     if verbose:
         end_time = time.time()
         tqdm.write(
             f'frag_coverage took {end_time - start_time} s to complete\n'
         )
 
     return contig, start, stop, name, coverage
@@ -121,24 +109,24 @@
         scale_factor: float=1e6,
         quality_threshold: int=30,
         workers: int=1,
         verbose: Union[bool, int]=False):
     """
     Return estimated fragment coverage over intervals specified in
     `intervals`. Fragments are read from `input_file` which may be
-    either a BAM or SAM file. Uses an algorithm where the midpoints of
+     a SAM, BAM, CRAM, or Frag.gz file. Uses an algorithm where the midpoints of
     fragments are calculated and coverage is tabulated from the
     midpoints that fall into the specified region. Not suitable for
     fragments of size approaching interval size.
 
     Parameters
     ----------
     input_file : str or pysam.AlignmentFile
-        BAM, SAM, or CRAM file containing paired-end fragment reads or
-        its path. `AlignmentFile` must be opened in read mode.
+        SAM, BAM, CRAM, or Frag.gz file containing paired-end fragment 
+        reads or its path. `AlignmentFile` must be opened in read mode.
     interval_file : str
         BED4 file containing intervals over which to generate coverage
         statistics.
     output_file : string, optional
         Path for bed file to print coverages to. If output_file = `_`,
         results will be printed to stdout.
     scale_factor : int, optional
@@ -161,102 +149,91 @@
             output_file: {output_file}
             quality_threshold: {quality_threshold}
             workers: {workers}
             verbose: {verbose}\n
             """
         )
 
-    contigs = _get_contigs(
-        input_file,
-        verbose=verbose-1 if verbose>1 else 0
-    )
-
-    # calculating coverage for each contig in the input_file
-    contig_intervals = []
-    for contig, length in contigs:
-        contig_intervals.append((
-            input_file,
-            contig,
-            0,
-            length,
-            ".",
-            quality_threshold,
-            verbose - 1 if verbose > 1 else 0
-        ))
     if verbose:
         sys.stderr.write('Creating process pool\n')
     try:
         pool = Pool(processes=workers, )
         if verbose:
             sys.stderr.write('Calculating total coverage for file,\n')
 
-        total_coverage_results = pool.imap(
-            _single_coverage_star,
-            tqdm(
-                contig_intervals,
-                desc='Genome contigs',
-                position=0
-            ) if verbose else contig_intervals
+        total_coverage_results = pool.apply_async(
+            single_coverage,
+            (input_file, None, 0, None, '.', "midpoint", quality_threshold, False)
         )
 
         if verbose:
             tqdm.write('reading intervals\n')
 
-        intervals = pool.apply(
-            _get_intervals,
-            (input_file, interval_file, quality_threshold, verbose)
-        )
+        intervals = _get_intervals(
+            input_file, interval_file,
+            intersect_policy="midpoint",
+            quality_threshold=quality_threshold,
+            verbose=verbose)
 
         if verbose:
             tqdm.write('calculating coverage\n')
 
         coverages = pool.imap(
             _single_coverage_star,
             tqdm(
                 intervals,
                 desc='Intervals',
                 position=2
             ) if verbose else intervals,
-            len(intervals) // 2 // workers + 1
+            min(len(intervals) // 2 // workers + 1, 40)
         )
 
         if verbose:
             tqdm.write('Retrieving total coverage for file\n')
-        total_coverage = sum(coverage[4] for coverage in total_coverage_results)
+        total_coverage = total_coverage_results.get()
         if verbose:
                 tqdm.write(f'Total coverage is {total_coverage}\n')
 
         # Output
         output_is_file = False
 
         if output_file != None:
             if verbose:
                 tqdm.write('Writing results to output\n')
             try:
                 # handle output types
-                if output_file.endswith('.bed'):
+                if (output_file.endswith('.bed')
+                    or output_file.endswith('.bedgraph')
+                ):
                     output_is_file = True
                     output = open(output_file, 'w')
                 elif output_file.endswith('.bed.gz'):
                     output = gzip.open(output_file, 'w')
                     output_is_file = True
                 elif output_file == '-':
                     output = sys.stdout
                 else:
                     raise ValueError(
                         'output_file should have .bed or .bed.gz as as suffix'
                     )
 
                 # print to files
-                for coverage in coverages:
-                    output.write(
-                        f'{coverage[0]}\t{coverage[1]}\t{coverage[2]}\t'
-                        f'{coverage[3]}\t'
-                        f'{coverage[4]/total_coverage*scale_factor}\n'
-                    )
+                if output_file.endswith(".bedgraph"):
+                    for contig, start, stop, name, coverage in coverages:
+                        output.write(
+                            f'{contig}\t{start}\t{stop}\t'
+                            f'{coverage/total_coverage[4]*scale_factor}\n'
+                        )
+                else:
+                    for contig, start, stop, name, coverage in coverages:
+                        output.write(
+                            f'{contig}\t{start}\t{stop}\t'
+                            f'{name}\t'
+                            f'{coverage/total_coverage*scale_factor}\n'
+                        )
 
             finally:
                 if output_is_file:
                     output.close()
     finally:
         pool.close()
```

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/delfi.py` & `FinaleTools-0.4.4/src/finaletools/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/delfi_gc_correct.py` & `FinaleTools-0.4.4/src/finaletools/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/delfi_merge_bins.py` & `FinaleTools-0.4.4/src/finaletools/frag/delfi_merge_bins.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/end_motifs.py` & `FinaleTools-0.4.4/src/finaletools/frag/end_motifs.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/frag_length.py` & `FinaleTools-0.4.4/src/finaletools/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/multi_wps.py` & `FinaleTools-0.4.4/src/finaletools/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/frag/wps.py` & `FinaleTools-0.4.4/src/finaletools/frag/wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/genome/gaps.py` & `FinaleTools-0.4.4/src/finaletools/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/utils/cli_hist.py` & `FinaleTools-0.4.4/src/finaletools/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/utils/filter_bam.py` & `FinaleTools-0.4.4/src/finaletools/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.3/src/finaletools/utils/utils.py` & `FinaleTools-0.4.4/src/finaletools/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,27 +426,26 @@
 
 def _get_intervals(
     input_file: Union[str, pysam.AlignmentFile],
     interval_file: str,
     intersect_policy: str,
     quality_threshold: int,
     verbose: Union[bool, int]
-) -> list:
+) -> list[Tuple[str,str,int,int,str,str,int,int]]:
     """Helper function to read intervals from bed file."""
     intervals = []  # list of inputs for single_coverage
 
     with open(interval_file) as bed:
         for line in bed:
             if ~line.startswith('#'):
                 if line != '':
-                    contents = line.split()
-                    contig = contents[0].strip()
-                    start = int(contents[1])
-                    stop = int(contents[2])
-                    name = contents[3] if len(contents) > 3 else '.'
+                    contig, start, stop, *name = line.split()
+                    start = int(start)
+                    stop = int(stop)
+                    name = name[0] if len(name) > 1 else '.'
                     interval = (
                         input_file,
                         contig,
                         start,
                         stop,
                         name,
                         intersect_policy,
```

