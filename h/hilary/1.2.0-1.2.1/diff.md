# Comparing `tmp/hilary-1.2.0.tar.gz` & `tmp/hilary-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilary-1.2.0.tar", last modified: Thu Mar  7 22:54:00 2024, max compression
+gzip compressed data, was "hilary-1.2.1.tar", last modified: Fri Apr  5 16:22:07 2024, max compression
```

## Comparing `hilary-1.2.0.tar` & `hilary-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-03-07 22:54:00.578251 hilary-1.2.0/
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      132 2024-02-02 17:03:29.000000 hilary-1.2.0/CHANGELOG.md
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    35149 2024-02-02 17:03:29.000000 hilary-1.2.0/LICENSE
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      673 2024-03-07 22:52:30.000000 hilary-1.2.0/MANIFEST.in
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      425 2024-03-07 22:54:00.578251 hilary-1.2.0/PKG-INFO
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     5476 2024-02-02 17:03:29.000000 hilary-1.2.0/README.md
-drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-03-07 22:54:00.578251 hilary-1.2.0/hilary/
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      186 2024-02-14 11:51:57.000000 hilary-1.2.0/hilary/__init__.py
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    16763 2024-03-07 00:50:56.000000 hilary-1.2.0/hilary/__main__.py
-drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-03-07 22:54:00.578251 hilary-1.2.0/hilary/__pycache__/
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      424 2024-02-29 22:55:34.000000 hilary-1.2.0/hilary/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      422 2024-02-14 11:58:19.000000 hilary-1.2.0/hilary/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     8750 2024-03-07 00:50:57.000000 hilary-1.2.0/hilary/__pycache__/__main__.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     8995 2024-03-05 03:43:01.000000 hilary-1.2.0/hilary/__pycache__/apriori.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     4079 2024-03-05 20:00:00.000000 hilary-1.2.0/hilary/__pycache__/expectmax.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    16089 2024-03-05 23:26:53.000000 hilary-1.2.0/hilary/__pycache__/inference.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     7203 2024-03-07 00:57:39.000000 hilary-1.2.0/hilary/__pycache__/utils.cpython-39.pyc
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    10204 2024-03-05 03:42:57.000000 hilary-1.2.0/hilary/apriori.py
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    22773 2024-02-02 17:03:32.000000 hilary-1.2.0/hilary/cdfs_326651.csv
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    22707 2024-02-02 17:03:32.000000 hilary-1.2.0/hilary/cdfs_326713.csv
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    55328 2024-02-02 17:03:32.000000 hilary-1.2.0/hilary/cdfs_paired.csv
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    49265 2024-02-08 17:25:48.000000 hilary-1.2.0/hilary/cdfs_paired_post_50K.csv
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     3795 2024-03-05 19:59:22.000000 hilary-1.2.0/hilary/expectmax.py
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    19914 2024-03-05 23:26:49.000000 hilary-1.2.0/hilary/inference.py
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     7992 2024-03-07 00:55:59.000000 hilary-1.2.0/hilary/utils.py
-drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-03-07 22:54:00.578251 hilary-1.2.0/hilary.egg-info/
--rw-r--r--   0 gathenes  (1003) gathenes  (1003)      425 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/PKG-INFO
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      746 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/SOURCES.txt
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)        1 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/dependency_links.txt
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)       56 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/entry_points.txt
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      191 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/requires.txt
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)        7 2024-03-07 22:54:00.000000 hilary-1.2.0/hilary.egg-info/top_level.txt
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)       38 2024-03-07 22:54:00.578251 hilary-1.2.0/setup.cfg
--rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     1016 2024-03-07 22:38:39.000000 hilary-1.2.0/setup.py
+drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-04-05 16:22:07.162284 hilary-1.2.1/
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)       22 2024-03-20 17:30:14.000000 hilary-1.2.1/CHANGELOG.md
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    35149 2024-02-02 17:03:29.000000 hilary-1.2.1/LICENSE
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      673 2024-03-07 22:52:30.000000 hilary-1.2.1/MANIFEST.in
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      473 2024-04-05 16:22:07.162284 hilary-1.2.1/PKG-INFO
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     6212 2024-03-20 17:30:14.000000 hilary-1.2.1/README.md
+drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-04-05 16:22:07.162284 hilary-1.2.1/hilary/
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      186 2024-02-14 11:51:57.000000 hilary-1.2.1/hilary/__init__.py
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    16767 2024-03-25 14:48:12.000000 hilary-1.2.1/hilary/__main__.py
+drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-04-05 16:22:07.162284 hilary-1.2.1/hilary/__pycache__/
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      424 2024-02-29 22:55:34.000000 hilary-1.2.1/hilary/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      422 2024-02-14 11:58:19.000000 hilary-1.2.1/hilary/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     8809 2024-03-25 14:50:20.000000 hilary-1.2.1/hilary/__pycache__/__main__.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     8999 2024-03-21 12:38:17.000000 hilary-1.2.1/hilary/__pycache__/apriori.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     4045 2024-03-20 20:34:07.000000 hilary-1.2.1/hilary/__pycache__/expectmax.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    16139 2024-03-21 12:39:11.000000 hilary-1.2.1/hilary/__pycache__/inference.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     7326 2024-03-25 14:53:19.000000 hilary-1.2.1/hilary/__pycache__/utils.cpython-39.pyc
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    10210 2024-03-21 12:38:13.000000 hilary-1.2.1/hilary/apriori.py
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    22773 2024-02-02 17:03:32.000000 hilary-1.2.1/hilary/cdfs_326651.csv
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    22707 2024-02-02 17:03:32.000000 hilary-1.2.1/hilary/cdfs_326713.csv
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    55328 2024-02-02 17:03:32.000000 hilary-1.2.1/hilary/cdfs_paired.csv
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    49265 2024-02-08 17:25:48.000000 hilary-1.2.1/hilary/cdfs_paired_post_50K.csv
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     3763 2024-03-20 17:30:14.000000 hilary-1.2.1/hilary/expectmax.py
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)    20014 2024-03-21 12:39:05.000000 hilary-1.2.1/hilary/inference.py
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     8335 2024-03-25 14:50:46.000000 hilary-1.2.1/hilary/utils.py
+drwxrwxr-x   0 gathenes  (1003) gathenes  (1003)        0 2024-04-05 16:22:07.162284 hilary-1.2.1/hilary.egg-info/
+-rw-r--r--   0 gathenes  (1003) gathenes  (1003)      473 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/PKG-INFO
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      746 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/SOURCES.txt
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)        1 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/dependency_links.txt
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)       56 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/entry_points.txt
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)      191 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/requires.txt
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)        7 2024-04-05 16:22:07.000000 hilary-1.2.1/hilary.egg-info/top_level.txt
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)       38 2024-04-05 16:22:07.162284 hilary-1.2.1/setup.cfg
+-rw-rw-r--   0 gathenes  (1003) gathenes  (1003)     1063 2024-04-05 16:21:14.000000 hilary-1.2.1/setup.py
```

### Comparing `hilary-1.2.0/LICENSE` & `hilary-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/MANIFEST.in` & `hilary-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/README.md` & `hilary-1.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,38 +13,61 @@
 | 1           | IGHV1-34*01 | IGHJ3*01 | TGTGCAACC | TTAGTACTT            | TTGCTTACT            | AGCACAGCC            | TTGCTTACT            |
 | 2           | IGHV1-18*01 | IGHJ4*01 | TGTGCAAGA | TTAATCCTA            | GCTATGGAC            | TTAATCCTA            | GCTATGGAC            |
 | 3           | IGHV1-74*01 | IGHJ4*01 | TGTGCAAGA | CATGCAACT            | GCTATGGAC            | CTACAATCA            | GCTATGGAC            |
 | 4           | IGHV5-17*01 | IGHJ4*01 | TGTGCAAGA | CCCTGTTCC            | CTATGCTATGG          | GAGGTGTTC            | CTATGCTAT            |
 
 ### 1.2 From the command line
 
-`infer --help`
+Hilary currently sypports three methods. A standard method performing single linkage clustering with fixed threshold on CDR3 pairwise Hamming distances. A method performing single linkage clustering with adaptive threshold on CDR3 Hamming distances (HILARy-CDR3). The full method performing single linkage clustering with adaptive threshold and using mutations in templated V and J regions (HILARy-full). Here are the different methods :
 
 ```
+infer-lineages --help
+Usage: infer-lineages [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  crude-method  Infer lineages with Standard method from data_path excel file.
+  cdr3-method   Infer lineages with HILARy-CDR3 from data_path excel file.
+  full-method   Infer lineages with HILARy-full from data_path excel file.
+```
+
+To get the options of the full method for example :
+
+```
+infer-lineages full-method --help
+Usage: infer-lineages full-method [OPTIONS] DATA_PATH
+
+  Infer lineages with HILARy-full from data_path excel file.
+
 Arguments:
   DATA_PATH  Path of the excel file to infer lineages.  [required]
 
 Options:
+  --kappa-file PATH        Path of the kappa chain file, hilary will
+                           automatically use its paired option.
   -v, --verbose            Set logging verbosity level.  [default: 0]
-  -t, --threads INTEGER    Choose number of cpus on which to run code.
-                           [default: all available]
-  -p, --precision FLOAT    Choose desired precision.  [default: 0.99]
+  -t, --threads INTEGER    Choose number of cpus on which to run code. -1 to
+                           use all available cpus.  [default: 1]
+  -p, --precision FLOAT    Choose desired precision.  [default: 1]
   -s, --sensitivity FLOAT  Choose desired sensitivity.  [default: 0.9]
-  --nmin INTEGER           Infer prevalence and mu on classes of size larger than nmin.
-                            Mean prevalence is assigned to lower than nmin classes.  [default: 1000]
-  -m, --model INTEGER      Model name to infer Null distribution.  [default: 326713]
   --silent                 Do not show progress bars if used.
-  --result-folder PATH     Where to save the result files. By default it will be saved in a
-                            'result/' folder in input data's parent directory.
-  --config PATH            Configuration file for column names. File should be a json with keys as
-                            your data's column names and values as hilary's required column names.
+  --result-folder PATH     Where to save the result files. By default it will
+                           be saved in a 'result/' folder.
+  --config PATH            Configuration file for column names. File should be
+                           a json with keys as your             data's column
+                           names and values as hilary's required column names.
+  --override               Override existing results.
+  --json / --text          Print logs as JSON or text.  [default: text]
+  --without-heuristic      DO not use heuristic for choosing the xy threshold.
   --help                   Show this message and exit.
 ```
 
-**example :** `infer /home/gabrielathenes/Documents/study/test.xlsx --nmin 10000 -vv --result-folder ../hilary_test`
+**example :** `infer-lineages full-method /home/gabrielathenes/Documents/study/exemple.xlsx`
 
 ### 1.3 From Python
 
 See `tutorial.ipynb`
 
 # 2. Functional description of HILARy
 
@@ -74,11 +97,8 @@
 ## 2.2 Incorporating phylogenetic signal
 
 For a wide range of parameters, the method is predicted to achieve both high precision and high sensitivity. However, it is expected to fail when the prevalence and the CDR3 length are both low. HILARy therefore uses the number of shared mutations to upgrade sensitivity for low.
 
 For each class, compute a high sensitivity (>90%) partition exactly like in step 2 but replacing precision with sensitivity. If the partition coincides with a high precision partition, then the partition is precise and sensitive and nothing needs to be done. Otherwise, we make the partition more precise by removing false positives. To do so we compute two variables $x'$ and $y$ coding respectfully for CDR3 divergence and number of mutations. We then classify pairs as related when $y-x'> t$ (resp. unrelated when <) with $t$ chosen to achieve high precision similarly than for the CDR3-based method.
 
 **Summary**
-Suppose we represent related sequences left (+ signs) and unrelated sequences right (o signs) on a plane. The rectangle-like shape is the estimation of positive sequences. In case the CDR3-based sensitive partition is not precise enough, the mutation based method upgrades the partition method by removing false positives.
-![Summary](./doc/mutations.png)
-
-# TODO
+![Summary](./doc/merging_partitions-1.png)
```

### Comparing `hilary-1.2.0/hilary/__main__.py` & `hilary-1.2.1/hilary/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     normalized_threshold: float = typer.Option(
         0.2,
         "--normalized_threshold",
         "-nt",
         help="Threshold to perform single linkage clustering on cdr3 normalized hamming distance.",
     ),
 ) -> None:
-    """Infer lineages with HILARy-CDR3 from data_path excel file."""
+    """Infer lineages with standard method from data_path excel file."""
     if result_folder is None:
         result_folder = data_path.parents[0] / Path("hilary_results/")
     result_folder.mkdir(parents=True, exist_ok=True)
     debug_folder = result_folder / Path("debug/")
     debug_folder.mkdir(parents=True, exist_ok=True)
     output_path = result_folder / Path(f"inferred_{data_path.name}")
     if output_path.exists() and not override:
```

### Comparing `hilary-1.2.0/hilary/__pycache__/__main__.cpython-39.pyc` & `hilary-1.2.1/hilary/__pycache__/__main__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  7 00:50:56 2024 UTC, .py size: 16763 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 700f e965 7b41 0000  a.......p..e{A..
+00000000: 610d 0d0a 0000 0000 ac8e 0166 7f41 0000  a..........f.A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0173 0603 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 5a09 6401 6406 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
@@ -169,379 +169,383 @@
 00000a80: 0064 1417 007c 0f64 0e3c 007c 0474 0164  .d...|.d.<.|.t.d
 00000a90: 267c 016a 039b 009d 0283 011b 007d 167c  &|.j.........}.|
 00000aa0: 0c6a 0964 277c 16a0 06a1 0064 258d 0201  .j.d'|.....d%...
 00000ab0: 0074 167c 0f7c 1664 1e8d 0201 007c 0264  .t.|.|.d.....|.d
 00000ac0: 1a6b 0590 0272 b664 287c 0d6a 0b76 0090  .k...r.d(|.j.v..
 00000ad0: 0272 b674 1d7c 0d64 2364 298d 025c 027d  .r.t.|.d#d)..\.}
 00000ae0: 177d 187c 0c6a 1564 2a7c 177c 1864 2b8d  .}.|.j.d*|.|.d+.
-00000af0: 0301 0064 0153 0029 2cfa 3a49 6e66 6572  ...d.S.),.:Infer
-00000b00: 206c 696e 6561 6765 7320 7769 7468 2048   lineages with H
-00000b10: 494c 4152 792d 4344 5233 2066 726f 6d20  ILARy-CDR3 from 
-00000b20: 6461 7461 5f70 6174 6820 6578 6365 6c20  data_path excel 
-00000b30: 6669 6c65 2e4e 7201 0000 00fa 0f68 696c  file.Nr......hil
-00000b40: 6172 795f 7265 7375 6c74 732f 54a9 02da  ary_results/T...
-00000b50: 0770 6172 656e 7473 da08 6578 6973 745f  .parents..exist_
-00000b60: 6f6b fa06 6465 6275 672f da09 696e 6665  ok..debug/..infe
-00000b70: 7272 6564 5ffa 3c20 616c 7265 6164 7920  rred_.< already 
-00000b80: 6578 6973 7473 2c20 7573 6520 6f76 6572  exists, use over
-00000b90: 7269 6465 2070 6172 616d 6574 6572 2074  ride parameter t
-00000ba0: 6f20 7265 706c 6163 6520 7468 6520 6669  o replace the fi
-00000bb0: 6c65 2e72 0f00 0000 a902 7216 0000 0072  le.r......r....r
-00000bc0: 1b00 0000 f512 0000 00f0 9f93 9620 5245  ............. RE
-00000bd0: 4144 494e 4720 4441 5441 20a9 0172 1400  ADING DATA ..r..
-00000be0: 0000 a902 da0a 696e 7075 745f 7061 7468  ......input_path
-00000bf0: 7219 0000 00da 0b73 6571 7565 6e63 655f  r......sequence_
-00000c00: 6964 fa28 4e6f 2027 7365 7175 656e 6365  id.(No 'sequence
-00000c10: 5f69 6427 2063 6f6c 756d 6e20 7072 6573  _id' column pres
-00000c20: 656e 7420 696e 2066 696c 652e da03 7374  ent in file...st
-00000c30: 72fa 042d 6967 6846 fa14 5553 494e 4720  r..-ighF..USING 
-00000c40: 5041 4952 4544 204f 5054 494f 4e2e fa04  PAIRED OPTION...
-00000c50: 2d69 676b e939 0000 00e9 9300 0000 e903  -igk.9..........
-00000c60: 0000 00e9 0f00 0000 e954 0000 00e9 0200  .........T......
-00000c70: 0000 5a06 696e 7075 745f 7a17 5361 7669  ..Z.input_z.Savi
-00000c80: 6e67 2069 6e70 7574 2064 6174 6166 7261  ng input datafra
-00000c90: 6d65 2ea9 01da 0470 6174 68a9 02da 0964  me.....path....d
-00000ca0: 6174 6166 7261 6d65 5a09 7361 7665 5f70  ataframeZ.save_p
-00000cb0: 6174 6829 03da 0670 6169 7265 64da 076c  ath)...paired..l
-00000cc0: 656e 6774 6873 7217 0000 00a9 02da 0264  engthsr........d
-00000cd0: 665a 0864 665f 6b61 7070 6129 0272 3f00  fZ.df_kappa).r?.
-00000ce0: 0000 5a05 6372 7564 6529 0272 1c00 0000  ..Z.crude).r....
-00000cf0: 721d 0000 005a 1363 7275 6465 5f6d 6574  r....Z.crude_met
-00000d00: 686f 645f 6661 6d69 6c79 f514 0000 00f0  hod_family......
-00000d10: 9f92 be20 5341 5649 4e47 2052 4553 554c  ... SAVING RESUL
-00000d20: 5453 20a9 01da 0b6f 7574 7075 745f 7061  TS ....output_pa
-00000d30: 7468 5a16 696e 6665 7272 6564 5f63 7275  thZ.inferred_cru
-00000d40: 6465 5f6d 6574 686f 645f f522 0000 00f0  de_method_."....
-00000d50: 9f92 be20 5341 5649 4e47 2052 4553 554c  ... SAVING RESUL
-00000d60: 5453 2046 4f52 204b 4150 5041 2046 494c  TS FOR KAPPA FIL
-00000d70: 45da 0863 6c6f 6e65 5f69 64a9 0272 3f00  E..clone_id..r?.
-00000d80: 0000 da09 7061 7274 6974 696f 6efa 4245  ....partition.BE
-00000d90: 7661 6c75 6174 696e 6720 4869 6c61 7279  valuating Hilary
-00000da0: 2773 2070 6572 666f 726d 616e 6365 206f  's performance o
-00000db0: 6e20 6772 6f75 6e64 2074 7275 7468 2063  n ground truth c
-00000dc0: 6f6c 756d 6e20 2763 6c6f 6e65 5f69 6427  olumn 'clone_id'
-00000dd0: 2e29 025a 0f70 7265 6369 7369 6f6e 5f63  .).Z.precision_c
-00000de0: 7275 6465 5a11 7365 6e73 6974 6976 6974  rudeZ.sensitivit
-00000df0: 795f 6372 7564 6529 1e72 2200 0000 7204  y_crude).r"...r.
-00000e00: 0000 00da 056d 6b64 6972 da04 6e61 6d65  .....mkdir..name
-00000e10: da06 6578 6973 7473 da0a 5661 6c75 6545  ..exists..ValueE
-00000e20: 7272 6f72 da08 6173 5f70 6f73 6978 7203  rror..as_posixr.
-00000e30: 0000 0072 0800 0000 da04 696e 666f 720a  ...r......infor.
-00000e40: 0000 00da 0763 6f6c 756d 6e73 da07 7761  .....columns..wa
-00000e50: 726e 696e 67da 0569 6e64 6578 da06 6173  rning..index..as
-00000e60: 7479 7065 722e 0000 00da 0573 7472 6970  typer......strip
-00000e70: da09 7365 745f 696e 6465 78da 026e 70da  ..set_index..np.
-00000e80: 0661 7261 6e67 6572 1000 0000 da05 6465  .aranger......de
-00000e90: 6275 6772 0b00 0000 7205 0000 00da 0a70  bugr....r......p
-00000ea0: 7265 7072 6f63 6573 7372 0700 0000 da07  reprocessr......
-00000eb0: 636c 6173 7365 7372 0600 0000 5a1d 636f  classesr....Z.co
-00000ec0: 6d70 7574 655f 6372 7564 655f 6d65 7468  mpute_crude_meth
-00000ed0: 6f64 5f63 6c75 7374 6572 7372 0900 0000  od_clustersr....
-00000ee0: 2919 7214 0000 0072 1500 0000 7216 0000  ).r....r....r...
-00000ef0: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000f00: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00000f10: 1d00 0000 da0c 6465 6275 675f 666f 6c64  ......debug_fold
-00000f20: 6572 7242 0000 00da 036c 6f67 723b 0000  errB.....logr;..
-00000f30: 0072 3c00 0000 da0f 6461 7461 6672 616d  .r<.....datafram
-00000f40: 655f 6b61 7070 6172 3d00 0000 722b 0000  e_kappar=...r+..
-00000f50: 00da 0761 7072 696f 7269 da13 6461 7461  ...apriori..data
-00000f60: 6672 616d 655f 7072 6f63 6573 7365 64da  frame_processed.
-00000f70: 0668 696c 6172 795a 0f64 6174 6166 7261  .hilaryZ.datafra
-00000f80: 6d65 5f63 7275 6465 da11 6f75 7470 7574  me_crude..output
-00000f90: 5f70 6174 685f 6b61 7070 61da 0970 7265  _path_kappa..pre
-00000fa0: 6369 7369 6f6e da0b 7365 6e73 6974 6976  cision..sensitiv
-00000fb0: 6974 79a9 0072 6200 0000 fa2f 2f68 6f6d  ity..rb....//hom
-00000fc0: 652f 6761 7468 656e 6573 2f67 6974 6c61  e/gathenes/gitla
-00000fd0: 622f 4849 4c41 5279 2f68 696c 6172 792f  b/HILARy/hilary/
-00000fe0: 5f5f 6d61 696e 5f5f 2e70 79da 0c63 7275  __main__.py..cru
-00000ff0: 6465 5f6d 6574 686f 6418 0000 0073 a800  de_method....s..
-00001000: 0000 003c 0801 1201 0e01 0c01 0e01 1401  ...<............
-00001010: 0c01 0201 0cff 0403 0801 0601 0c01 0401  ................
-00001020: 0201 06fe 0604 0c01 0a01 0a01 1001 1401  ................
-00001030: 0a01 0401 0601 0a01 0c01 0a01 02ff 0803  ................
-00001040: 0a01 1401 0602 0401 1402 0a01 1401 0401  ................
-00001050: 0201 06fe 0604 0c01 0201 0201 0201 02fd  ................
-00001060: 0605 0e01 0a01 0201 0201 0201 02fd 0605  ................
-00001070: 0401 0201 0201 02fd 0605 0c01 1002 1201  ................
-00001080: 1401 0c01 0601 0c01 1001 0401 0aff 0603  ................
-00001090: 0401 0201 06fe 0604 0c02 1601 0201 04ff  ................
-000010a0: 0a03 0401 0201 0201 02fd 7264 0000 0067  ..........rd...g
-000010b0: ae47 e17a 14ae ef3f 7a0b 2d2d 7072 6563  .G.z...?z.--prec
-000010c0: 6973 696f 6e7a 022d 707a 1943 686f 6f73  isionz.-pz.Choos
-000010d0: 6520 6465 7369 7265 6420 7072 6563 6973  e desired precis
-000010e0: 696f 6e2e 67cd cccc cccc ccec 3f7a 0d2d  ion.g.......?z.-
-000010f0: 2d73 656e 7369 7469 7669 7479 7a02 2d73  -sensitivityz.-s
-00001100: 7a1b 4368 6f6f 7365 2064 6573 6972 6564  z.Choose desired
-00001110: 2073 656e 7369 7469 7669 7479 2e7a 082d   sensitivity.z.-
-00001120: 2d73 696c 656e 747a 2244 6f20 6e6f 7420  -silentz"Do not 
-00001130: 7368 6f77 2070 726f 6772 6573 7320 6261  show progress ba
-00001140: 7273 2069 6620 7573 6564 2e29 0d72 1400  rs if used.).r..
-00001150: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001160: 0072 6000 0000 7261 0000 00da 0673 696c  .r`...ra.....sil
-00001170: 656e 7472 1800 0000 7219 0000 0072 1a00  entr....r....r..
-00001180: 0000 721b 0000 00da 0673 6176 696e 6772  ..r......savingr
-00001190: 1e00 0000 630c 0000 0000 0000 0000 0000  ....c...........
-000011a0: 001a 0000 0008 0000 0043 0000 0173 4403  .........C...sD.
-000011b0: 0000 7c07 6401 7500 721a 7c00 6a00 6402  ..|.d.u.r.|.j.d.
-000011c0: 1900 7401 6403 8301 1b00 7d07 7c07 6a02  ..t.d.....}.|.j.
-000011d0: 6404 6404 6405 8d02 0100 7c07 7401 6406  d.d.d.....|.t.d.
-000011e0: 8301 1b00 7d0c 7c0c 6a02 6404 6404 6405  ....}.|.j.d.d.d.
-000011f0: 8d02 0100 7c07 7401 6407 7c00 6a03 9b00  ....|.t.d.|.j...
-00001200: 9d02 8301 1b00 7d0d 7c0d a004 a100 7274  ......}.|.....rt
-00001210: 7c09 7374 7405 7c0d a006 a100 9b00 6408  |.stt.|.......d.
-00001220: 9d02 8301 8201 7c03 6409 6b02 7282 7407  ......|.d.k.r.t.
-00001230: 8300 7d03 7408 7c02 7c0a 640a 8d02 7d0e  ..}.t.|.|.d...}.
-00001240: 7c0e 6a09 640b 7c00 a006 a100 640c 8d02  |.j.d.|.....d...
-00001250: 0100 740a 7c00 7c08 640d 8d02 7d0f 640e  ..t.|.|.d...}.d.
-00001260: 7c0f 6a0b 7601 72d0 7c0e a00c 640f a101  |.j.v.r.|...d...
-00001270: 0100 7c0f 6a0d a00e 6410 a101 7c0f 640e  ..|.j...d...|.d.
-00001280: 3c00 7c0f 640e 1900 6a0f a010 6411 a101  <.|.d...j...d...
-00001290: 7c0f 640e 3c00 7c0f a011 640e a101 0100  |.d.<.|...d.....
-000012a0: 6412 7d10 7c01 9001 7246 7c0e a009 6413  d.}.|...rF|...d.
-000012b0: a101 0100 740a 7c01 7c08 640d 8d02 7d11  ....t.|.|.d...}.
-000012c0: 7c11 640e 1900 6a0f a010 6414 a101 7c11  |.d...j...d...|.
-000012d0: 640e 3c00 7c11 a011 640e a101 0100 7412  d.<.|...d.....t.
-000012e0: a013 6415 6416 6417 a103 a00e 7414 a101  ..d.d.d.....t...
-000012f0: 7d12 6404 7d10 6e18 6401 7d11 7412 a013  }.d.}.n.d.}.t...
-00001300: 6418 6419 6417 a103 a00e 7414 a101 7d12  d.d.d.....t...}.
-00001310: 7415 7c10 7c12 7c03 7c04 7c05 7c06 641a  t.|.|.|.|.|.|.d.
-00001320: 8d06 7d13 7c13 6a16 7c0f 7c11 641b 8d02  ..}.|.j.|.|.d...
-00001330: 7d14 7417 7c14 8301 7c13 5f18 7c0e a009  }.t.|...|._.|...
-00001340: 641c a101 0100 7c13 a019 7c14 a101 0100  d.....|...|.....
-00001350: 7c02 641d 6b05 9001 72da 7c0c 7401 641e  |.d.k...r.|.t.d.
-00001360: 7c00 6a03 9b00 9d02 8301 1b00 7d15 7c0e  |.j.........}.|.
-00001370: 6a1a 641f 7c15 a006 a100 6420 8d02 0100  j.d.|.....d ....
-00001380: 741b 7c13 6a1c 7c15 8302 0100 7c0e a009  t.|.j.|.....|...
-00001390: 6421 a101 0100 7c13 a01d a100 0100 7c0e  d!....|.......|.
-000013a0: a009 6422 a101 0100 7c13 a01e a100 0100  ..d"....|.......
-000013b0: 7c02 641d 6b05 9002 723a 7c0c 7401 6423  |.d.k...r:|.t.d#
-000013c0: 7c00 6a03 9b00 9d02 8301 1b00 7d16 7c0e  |.j.........}.|.
-000013d0: 6a1a 6424 7c16 a006 a100 6420 8d02 0100  j.d$|.....d ....
-000013e0: 741b 7c13 6a18 7c16 8302 0100 7c0e a009  t.|.j.|.....|...
-000013f0: 6425 a101 0100 741f 7c13 7c14 6426 8d02  d%....t.|.|.d&..
-00001400: 7d17 7c17 a020 7c14 a101 7d18 7c18 6427  }.|.. |...}.|.d'
-00001410: 1900 7c0f 6428 3c00 7c0f 640e 1900 6411  ..|.d(<.|.d...d.
-00001420: 1700 7c0f 640e 3c00 7c0b 9003 7202 7c0e  ..|.d.<.|...r.|.
-00001430: 6a09 6429 7c0d a006 a100 642a 8d02 0100  j.d)|.....d*....
-00001440: 7c07 7401 642b 7c00 6a03 9b00 9d02 8301  |.t.d+|.j.......
-00001450: 1b00 7d0d 741b 7c0f 7c0d 642c 8d02 0100  ..}.t.|.|.d,....
-00001460: 7c10 9003 7202 7c18 6427 1900 7c11 6428  |...r.|.d'..|.d(
-00001470: 3c00 7c0f 640e 1900 6414 1700 7c11 640e  <.|.d...d...|.d.
-00001480: 3c00 7c07 7401 642b 7c01 6a03 9b00 9d02  <.|.t.d+|.j.....
-00001490: 8301 1b00 7d19 7c0e 6a09 642d 7c19 a006  ....}.|.j.d-|...
-000014a0: a100 642a 8d02 0100 741b 7c11 7c19 642c  ..d*....t.|.|.d,
-000014b0: 8d02 0100 7c02 641d 6b05 9003 7238 642e  ....|.d.k...r8d.
-000014c0: 7c0f 6a0b 7600 9003 7238 7421 7c0f 6428  |.j.v...r8t!|.d(
-000014d0: 642f 8d02 5c02 7d04 7d05 7c0e 6a1a 6430  d/..\.}.}.|.j.d0
-000014e0: 7c04 7c05 6431 8d03 0100 7c18 7c0f 7c11  |.|.d1....|.|.|.
-000014f0: 7c17 6604 5300 2932 721f 0000 004e 7201  |.f.S.)2r....Nr.
-00001500: 0000 0072 2000 0000 5472 2100 0000 7224  ...r ...Tr!...r$
-00001510: 0000 0072 2500 0000 7226 0000 0072 0f00  ...r%...r&...r..
-00001520: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00001530: 0072 2a00 0000 722c 0000 0072 2d00 0000  .r*...r,...r-...
-00001540: 722e 0000 0072 2f00 0000 4672 3000 0000  r....r/...Fr0...
-00001550: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
-00001560: 3400 0000 7235 0000 0072 3600 0000 2906  4...r5...r6...).
-00001570: 723c 0000 0072 3d00 0000 7217 0000 0072  r<...r=...r....r
-00001580: 6000 0000 7261 0000 0072 6500 0000 723e  `...ra...re...r>
-00001590: 0000 0075 1d00 0000 e28f b320 434f 4d50  ...u....... COMP
-000015a0: 5554 494e 4720 4849 5354 4f47 5241 4d53  UTING HISTOGRAMS
-000015b0: 20e2 8fb3 2e72 3700 0000 5a0b 6869 7374   ....r7...Z.hist
-000015c0: 6f67 7261 6d73 5f7a 2153 6176 696e 6720  ograms_z!Saving 
-000015d0: 6869 7374 6f67 7261 6d73 2075 7365 6420  histograms used 
-000015e0: 6279 2048 696c 6172 792e 7238 0000 0075  by Hilary.r8...u
-000015f0: 1d00 0000 e28f b320 434f 4d50 5554 494e  ....... COMPUTIN
-00001600: 4720 5041 5241 4d45 5445 5253 20e2 8fb3  G PARAMETERS ...
-00001610: 2e75 1d00 0000 e28f b320 434f 4d50 5554  .u....... COMPUT
-00001620: 494e 4720 5448 5245 5348 4f4c 4453 20e2  ING THRESHOLDS .
-00001630: 8fb3 2eda 0b70 6172 616d 6574 6572 735f  .....parameters_
-00001640: fa29 5361 7669 6e67 2061 6c6c 2070 6172  .)Saving all par
-00001650: 616d 6574 6572 7320 696e 6665 7272 6564  ameters inferred
-00001660: 2062 7920 4869 6c61 7279 2e75 3100 0000   by Hilary.u1...
-00001670: e28f b320 434f 4d50 5554 494e 4720 5052  ... COMPUTING PR
-00001680: 4543 4953 4520 414e 4420 5345 4e53 4954  ECISE AND SENSIT
-00001690: 4956 4520 434c 5553 5445 5253 20e2 8fb3  IVE CLUSTERS ...
-000016a0: 2ea9 0172 3f00 0000 5a0f 7072 6563 6973  ...r?...Z.precis
-000016b0: 655f 636c 7573 7465 72da 1163 6472 335f  e_cluster..cdr3_
-000016c0: 6261 7365 645f 6661 6d69 6c79 7240 0000  based_familyr@..
-000016d0: 0072 4100 0000 5a14 696e 6665 7272 6564  .rA...Z.inferred
-000016e0: 5f63 6472 335f 6261 7365 645f 723a 0000  _cdr3_based_r:..
-000016f0: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
-00001700: 7247 0000 0029 02da 0e70 7265 6369 7369  rG...)...precisi
-00001710: 6f6e 5f63 6472 33da 1073 656e 7369 7469  on_cdr3..sensiti
-00001720: 7669 7479 5f63 6472 3329 2272 2200 0000  vity_cdr3)"r"...
-00001730: 7204 0000 0072 4800 0000 7249 0000 0072  r....rH...rI...r
-00001740: 4a00 0000 724b 0000 0072 4c00 0000 7203  J...rK...rL...r.
-00001750: 0000 0072 0800 0000 724d 0000 0072 0a00  ...r....rM...r..
-00001760: 0000 724e 0000 0072 4f00 0000 7250 0000  ..rN...rO...rP..
-00001770: 0072 5100 0000 722e 0000 0072 5200 0000  .rQ...r....rR...
-00001780: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00001790: 1000 0000 7205 0000 0072 5700 0000 7207  ....r....rW...r.
-000017a0: 0000 0072 5800 0000 5a0e 6765 745f 6869  ...rX...Z.get_hi
-000017b0: 7374 6f67 7261 6d73 7256 0000 0072 0b00  stogramsrV...r..
-000017c0: 0000 5a0a 6869 7374 6f67 7261 6d73 5a0e  ..Z.histogramsZ.
-000017d0: 6765 745f 7061 7261 6d65 7465 7273 5a0e  get_parametersZ.
-000017e0: 6765 745f 7468 7265 7368 6f6c 6473 7206  get_thresholdsr.
-000017f0: 0000 005a 1a63 6f6d 7075 7465 5f70 7265  ...Z.compute_pre
-00001800: 635f 7365 6e73 5f63 6c75 7374 6572 7372  c_sens_clustersr
-00001810: 0900 0000 291a 7214 0000 0072 1500 0000  ....).r....r....
-00001820: 7216 0000 0072 1700 0000 7260 0000 0072  r....r....r`...r
-00001830: 6100 0000 7265 0000 0072 1800 0000 7219  a...re...r....r.
-00001840: 0000 0072 1a00 0000 721b 0000 0072 6600  ...r....r....rf.
-00001850: 0000 7259 0000 0072 4200 0000 725a 0000  ..rY...rB...rZ..
-00001860: 0072 3b00 0000 723c 0000 0072 5b00 0000  .r;...r<...r[...
-00001870: 723d 0000 0072 5c00 0000 725d 0000 005a  r=...r\...r]...Z
-00001880: 0e68 6973 746f 6772 616d 5f70 6174 68da  .histogram_path.
-00001890: 0f70 6172 616d 6574 6572 735f 7061 7468  .parameters_path
-000018a0: 725e 0000 00da 0e64 6174 6166 7261 6d65  r^.....dataframe
-000018b0: 5f63 6472 3372 5f00 0000 7262 0000 0072  _cdr3r_...rb...r
-000018c0: 6200 0000 7263 0000 00da 0b63 6472 335f  b...rc.....cdr3_
-000018d0: 6d65 7468 6f64 ae00 0000 73be 0000 0000  method....s.....
-000018e0: 4208 0112 010e 010c 010e 0114 010c 0102  B...............
-000018f0: 010c ff04 0308 0106 010c 0104 0102 0106  ................
-00001900: fe06 040c 010a 010a 0110 0114 010a 0104  ................
-00001910: 0106 010a 010c 010a 0102 ff08 030a 0114  ................
-00001920: 0106 0204 0114 0202 0102 0102 0102 0102  ................
-00001930: 0102 0102 fa06 080e 010a 020a 010a 020a  ................
-00001940: 0114 0112 010c 020a 0108 020a 0108 010a  ................
-00001950: 0114 0104 0102 0106 fe06 040c 020a 0102  ................
-00001960: 0102 0102 fe06 040a 020c 0110 0206 0112  ................
-00001970: 0114 010c 0106 010c 0110 0104 010a ff06  ................
-00001980: 0304 0102 0106 fe06 040c 0216 0102 0104  ................
-00001990: ff0a 0304 0102 0102 0102 fd06 0572 6f00  .............ro.
-000019a0: 0000 7a13 2d2d 7769 7468 6f75 742d 6865  ..z.--without-he
-000019b0: 7572 6973 7469 637a 3344 4f20 6e6f 7420  uristicz3DO not 
-000019c0: 7573 6520 6865 7572 6973 7469 6320 666f  use heuristic fo
-000019d0: 7220 6368 6f6f 7369 6e67 2074 6865 2078  r choosing the x
-000019e0: 7920 7468 7265 7368 6f6c 642e 290d 7214  y threshold.).r.
-000019f0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00001a00: 0000 7260 0000 0072 6100 0000 7265 0000  ..r`...ra...re..
-00001a10: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001a20: 721b 0000 00da 1177 6974 686f 7574 5f68  r......without_h
-00001a30: 6575 7269 7374 6963 721e 0000 0063 0c00  euristicr....c..
-00001a40: 0000 0000 0000 0000 0000 1b00 0000 0e00  ................
-00001a50: 0000 4300 0001 73d4 0100 007c 0764 0175  ..C...s....|.d.u
-00001a60: 0072 1a7c 006a 0064 0219 0074 0164 0383  .r.|.j.d...t.d..
-00001a70: 011b 007d 077c 076a 0264 0464 0464 058d  ...}.|.j.d.d.d..
-00001a80: 0201 007c 0774 0164 0683 011b 007d 0c7c  ...|.t.d.....}.|
-00001a90: 0172 3e64 077d 0d6e 0464 027d 0d74 037c  .r>d.}.n.d.}.t.|
-00001aa0: 027c 0a64 088d 027d 0e74 047c 007c 017c  .|.d...}.t.|.|.|
-00001ab0: 027c 037c 047c 057c 067c 077c 087c 097c  .|.|.|.|.|.|.|.|
-00001ac0: 0a64 0964 0a8d 0c5c 047d 0f7d 107d 117d  .d.d...\.}.}.}.}
-00001ad0: 127c 0b72 867c 0d7c 126a 0564 0b3c 006e  .|.r.|.|.j.d.<.n
-00001ae0: 2a7c 0ea0 0664 0ca1 0101 007c 126a 077c  *|...d.....|.j.|
-00001af0: 0f64 0d8d 0101 007c 126a 0564 0b19 007c  .d.....|.j.d...|
-00001b00: 0d17 007c 126a 0564 0b3c 007c 0264 0e6b  ...|.j.d.<.|.d.k
-00001b10: 0572 ea7c 0c74 0164 0f7c 006a 089b 009d  .r.|.t.d.|.j....
-00001b20: 0283 011b 007d 137c 0e6a 0964 107c 13a0  .....}.|.j.d.|..
-00001b30: 0aa1 0064 118d 0201 0074 0b7c 126a 057c  ...d.....t.|.j.|
-00001b40: 1383 0201 007c 0ea0 0664 12a1 0101 007c  .....|...d.....|
-00001b50: 126a 0c7c 0f64 0d8d 017d 147c 1464 1319  .j.|.d...}.|.d..
-00001b60: 007c 1064 133c 007c 0774 0164 147c 006a  .|.d.<.|.t.d.|.j
-00001b70: 089b 009d 0283 011b 007d 157c 0e6a 0664  .........}.|.j.d
-00001b80: 157c 15a0 0aa1 0064 168d 0201 0074 0b7c  .|.....d.....t.|
-00001b90: 107c 1564 178d 0201 007c 1164 0175 0190  .|.d.....|.d.u..
-00001ba0: 0172 867c 1464 1319 007c 1164 133c 007c  .r.|.d...|.d.<.|
-00001bb0: 0774 0164 147c 016a 089b 009d 0283 011b  .t.d.|.j........
-00001bc0: 007d 167c 0e6a 0664 187c 16a0 0aa1 0064  .}.|.j.d.|.....d
-00001bd0: 168d 0201 0074 0b7c 117c 1664 178d 0201  .....t.|.|.d....
-00001be0: 007c 0264 0e6b 0590 0172 d064 197c 106a  .|.d.k...r.d.|.j
-00001bf0: 0d76 0090 0172 d074 0e7c 1064 1364 1a8d  .v...r.t.|.d.d..
-00001c00: 025c 027d 177d 1874 0e7c 1064 1b64 1a8d  .\.}.}.t.|.d.d..
-00001c10: 025c 027d 197d 1a7c 0e6a 0964 1c7c 177c  .\.}.}.|.j.d.|.|
-00001c20: 187c 197c 1a64 1d8d 0501 0064 0153 0029  .|.|.d.....d.S.)
-00001c30: 1e7a 3a49 6e66 6572 206c 696e 6561 6765  .z:Infer lineage
-00001c40: 7320 7769 7468 2048 494c 4152 792d 6675  s with HILARy-fu
-00001c50: 6c6c 2066 726f 6d20 6461 7461 5f70 6174  ll from data_pat
-00001c60: 6820 6578 6365 6c20 6669 6c65 2e4e 7201  h excel file.Nr.
-00001c70: 0000 0072 2000 0000 5472 2100 0000 7224  ...r ...Tr!...r$
-00001c80: 0000 00e9 0400 0000 7227 0000 0046 290c  ........r'...F).
-00001c90: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001ca0: 1700 0000 7260 0000 0072 6100 0000 7265  ....r`...ra...re
-00001cb0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00001cc0: 0000 721b 0000 0072 6600 0000 da0c 7879  ..r....rf.....xy
-00001cd0: 5f74 6872 6573 686f 6c64 7520 0000 00e2  _thresholdu ....
-00001ce0: 8fb3 2043 4f4d 5055 5449 4e47 2058 5920  .. COMPUTING XY 
-00001cf0: 5448 5245 5348 4f4c 4453 20e2 8fb3 2e72  THRESHOLDS ....r
-00001d00: 6900 0000 7237 0000 0072 6700 0000 7268  i...r7...rg...rh
-00001d10: 0000 0072 3800 0000 752e 0000 00e2 8fb3  ...r8...u.......
-00001d20: 2049 4e46 4552 5249 4e47 2046 414d 494c   INFERRING FAMIL
-00001d30: 4945 5320 5749 5448 2046 554c 4c20 5859  IES WITH FULL XY
-00001d40: 204d 4554 484f 44e2 8fb3 2e5a 0666 616d   METHOD....Z.fam
-00001d50: 696c 795a 1569 6e66 6572 7265 645f 6675  ilyZ.inferred_fu
-00001d60: 6c6c 5f6d 6574 686f 645f 7240 0000 0072  ll_method_r@...r
-00001d70: 4100 0000 723a 0000 0072 4300 0000 7244  A...r:...rC...rD
-00001d80: 0000 0072 4500 0000 726a 0000 0072 4700  ...rE...rj...rG.
-00001d90: 0000 2904 5a15 7072 6563 6973 696f 6e5f  ..).Z.precision_
-00001da0: 6675 6c6c 5f6d 6574 686f 645a 1773 656e  full_methodZ.sen
-00001db0: 7369 7469 7669 7479 5f66 756c 6c5f 6d65  sitivity_full_me
-00001dc0: 7468 6f64 726b 0000 0072 6c00 0000 290f  thodrk...rl...).
-00001dd0: 7222 0000 0072 0400 0000 7248 0000 0072  r"...r....rH...r
-00001de0: 0800 0000 726f 0000 0072 5800 0000 724d  ....ro...rX...rM
-00001df0: 0000 005a 1167 6574 5f78 795f 7468 7265  ...Z.get_xy_thre
-00001e00: 7368 6f6c 6473 7249 0000 0072 5600 0000  sholdsrI...rV...
-00001e10: 724c 0000 0072 0b00 0000 5a05 696e 6665  rL...r....Z.infe
-00001e20: 7272 4e00 0000 7209 0000 0029 1b72 1400  rrN...r....).r..
-00001e30: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001e40: 0072 6000 0000 7261 0000 0072 6500 0000  .r`...ra...re...
-00001e50: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00001e60: 1b00 0000 7270 0000 0072 5900 0000 7272  ....rp...rY...rr
-00001e70: 0000 0072 5a00 0000 726e 0000 0072 3b00  ...rZ...rn...r;.
-00001e80: 0000 725b 0000 0072 5e00 0000 726d 0000  ..r[...r^...rm..
-00001e90: 005a 1264 6174 6166 7261 6d65 5f69 6e66  .Z.dataframe_inf
-00001ea0: 6572 7265 6472 4200 0000 725f 0000 005a  erredrB...r_...Z
-00001eb0: 0e70 7265 6369 7369 6f6e 5f66 756c 6c5a  .precision_fullZ
-00001ec0: 1073 656e 7369 7469 7669 7479 5f66 756c  .sensitivity_ful
-00001ed0: 6c72 6b00 0000 726c 0000 0072 6200 0000  lrk...rl...rb...
-00001ee0: 7262 0000 0072 6300 0000 da0b 6675 6c6c  rb...rc.....full
-00001ef0: 5f6d 6574 686f 645b 0100 0073 8000 0000  _method[...s....
-00001f00: 0046 0801 1201 0e01 0c01 0401 0602 0401  .F..............
-00001f10: 0c02 0201 0201 0201 0201 0201 0201 0201  ................
-00001f20: 0201 0201 0201 0201 0201 02f4 0e0e 0401  ................
-00001f30: 0c02 0a01 0c01 1401 0801 1401 0401 0201  ................
-00001f40: 06fe 0604 0c02 0a01 0c02 0c02 1401 1202  ................
-00001f50: 0c02 0a01 0c01 0401 0aff 0603 0401 0201  ................
-00001f60: 06fe 0604 0c02 1601 0201 04ff 0a03 0201  ................
-00001f70: 04ff 0a03 0401 0201 0201 0201 0201 02fb  ................
-00001f80: 7273 0000 00da 085f 5f6d 6169 6e5f 5f29  rs.....__main__)
-00001f90: 1dda 075f 5f64 6f63 5f5f da0a 5f5f 6675  ...__doc__..__fu
-00001fa0: 7475 7265 5f5f 7202 0000 005a 0f6d 756c  ture__r....Z.mul
-00001fb0: 7469 7072 6f63 6573 7369 6e67 7203 0000  tiprocessingr...
-00001fc0: 00da 0770 6174 686c 6962 7204 0000 005a  ...pathlibr....Z
-00001fd0: 056e 756d 7079 7254 0000 005a 0574 7970  .numpyrT...Z.typ
-00001fe0: 6572 5a0e 6869 6c61 7279 2e61 7072 696f  erZ.hilary.aprio
-00001ff0: 7269 7205 0000 005a 1068 696c 6172 792e  rir....Z.hilary.
-00002000: 696e 6665 7265 6e63 6572 0600 0000 5a0c  inferencer....Z.
-00002010: 6869 6c61 7279 2e75 7469 6c73 7207 0000  hilary.utilsr...
-00002020: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00002030: 720b 0000 005a 0554 7970 6572 5a03 6170  r....Z.TyperZ.ap
-00002040: 705a 0763 6f6d 6d61 6e64 5a08 4172 6775  pZ.commandZ.Argu
-00002050: 6d65 6e74 5a06 4f70 7469 6f6e 7264 0000  mentZ.Optionrd..
-00002060: 0072 6f00 0000 7273 0000 00da 085f 5f6e  .ro...rs.....__n
-00002070: 616d 655f 5f72 6200 0000 7262 0000 0072  ame__rb...rb...r
-00002080: 6200 0000 7263 0000 00da 083c 6d6f 6475  b...rc.....<modu
-00002090: 6c65 3e01 0000 0073 9201 0000 0402 0c02  le>....s........
-000020a0: 0c01 0c02 0801 0802 0c01 0c01 1c08 0c03  ................
-000020b0: 0602 0401 0201 0201 02fd 0405 0401 0201  ................
-000020c0: 0201 02fd 0405 0401 0201 0201 0201 0201  ................
-000020d0: 02fb 0407 0401 0201 0201 0201 02fc 0406  ................
-000020e0: 0401 0201 0201 02fd 0405 0401 0201 0201  ................
-000020f0: 02fd 0406 0401 0201 0201 02fd 0405 0401  ................
-00002100: 0201 0201 02fd 0405 0401 0201 0201 0201  ................
-00002110: 02fc 0406 0401 0201 0201 0201 02fc 04cd  ................
-00002120: 267f 0016 0602 0401 0201 0201 02fd 0405  &...............
-00002130: 0401 0201 0201 02fd 0405 0401 0201 0201  ................
-00002140: 0201 0201 02fb 0407 0401 0201 0201 0201  ................
-00002150: 02fc 0406 0401 0201 0201 0201 02fc 0406  ................
-00002160: 0401 0201 0201 0201 02fc 0406 0401 0201  ................
-00002170: 0201 02fd 0405 0401 0201 0201 02fd 0405  ................
-00002180: 0401 0201 0201 02fd 0406 0401 0201 0201  ................
-00002190: 02fd 0405 0401 0201 0201 02fd 0405 02c2  ................
-000021a0: 2a7f 002d 0602 0401 0201 0201 02fd 0405  *..-............
-000021b0: 0401 0201 0201 02fd 0405 0401 0201 0201  ................
-000021c0: 0201 0201 02fb 0407 0401 0201 0201 0201  ................
-000021d0: 02fc 0406 0401 0201 0201 0201 02fc 0406  ................
-000021e0: 0401 0201 0201 0201 02fc 0406 0401 0201  ................
-000021f0: 0201 02fd 0405 0401 0201 0201 02fd 0405  ................
-00002200: 0401 0201 0201 02fd 0406 0401 0201 0201  ................
-00002210: 02fd 0405 0401 0201 0201 02fd 0405 0401  ................
-00002220: 0201 0201 02fd 04c2 2a7f 0011 0a01       ........*.....
+00000af0: 0301 0064 0153 0029 2c7a 3e49 6e66 6572  ...d.S.),z>Infer
+00000b00: 206c 696e 6561 6765 7320 7769 7468 2073   lineages with s
+00000b10: 7461 6e64 6172 6420 6d65 7468 6f64 2066  tandard method f
+00000b20: 726f 6d20 6461 7461 5f70 6174 6820 6578  rom data_path ex
+00000b30: 6365 6c20 6669 6c65 2e4e 7201 0000 00fa  cel file.Nr.....
+00000b40: 0f68 696c 6172 795f 7265 7375 6c74 732f  .hilary_results/
+00000b50: 54a9 02da 0770 6172 656e 7473 da08 6578  T....parents..ex
+00000b60: 6973 745f 6f6b fa06 6465 6275 672f da09  ist_ok..debug/..
+00000b70: 696e 6665 7272 6564 5ffa 3c20 616c 7265  inferred_.< alre
+00000b80: 6164 7920 6578 6973 7473 2c20 7573 6520  ady exists, use 
+00000b90: 6f76 6572 7269 6465 2070 6172 616d 6574  override paramet
+00000ba0: 6572 2074 6f20 7265 706c 6163 6520 7468  er to replace th
+00000bb0: 6520 6669 6c65 2e72 0f00 0000 a902 7216  e file.r......r.
+00000bc0: 0000 0072 1b00 0000 f512 0000 00f0 9f93  ...r............
+00000bd0: 9620 5245 4144 494e 4720 4441 5441 20a9  . READING DATA .
+00000be0: 0172 1400 0000 a902 da0a 696e 7075 745f  .r........input_
+00000bf0: 7061 7468 7219 0000 00da 0b73 6571 7565  pathr......seque
+00000c00: 6e63 655f 6964 fa28 4e6f 2027 7365 7175  nce_id.(No 'sequ
+00000c10: 656e 6365 5f69 6427 2063 6f6c 756d 6e20  ence_id' column 
+00000c20: 7072 6573 656e 7420 696e 2066 696c 652e  present in file.
+00000c30: da03 7374 72fa 042d 6967 6846 fa14 5553  ..str..-ighF..US
+00000c40: 494e 4720 5041 4952 4544 204f 5054 494f  ING PAIRED OPTIO
+00000c50: 4e2e fa04 2d69 676b e939 0000 00e9 9300  N...-igk.9......
+00000c60: 0000 e903 0000 00e9 0f00 0000 e954 0000  .............T..
+00000c70: 00e9 0200 0000 5a06 696e 7075 745f 7a17  ......Z.input_z.
+00000c80: 5361 7669 6e67 2069 6e70 7574 2064 6174  Saving input dat
+00000c90: 6166 7261 6d65 2ea9 01da 0470 6174 68a9  aframe.....path.
+00000ca0: 02da 0964 6174 6166 7261 6d65 5a09 7361  ...dataframeZ.sa
+00000cb0: 7665 5f70 6174 6829 03da 0670 6169 7265  ve_path)...paire
+00000cc0: 64da 076c 656e 6774 6873 7217 0000 00a9  d..lengthsr.....
+00000cd0: 02da 0264 665a 0864 665f 6b61 7070 6129  ...dfZ.df_kappa)
+00000ce0: 0272 3e00 0000 5a05 6372 7564 6529 0272  .r>...Z.crude).r
+00000cf0: 1c00 0000 721d 0000 005a 1363 7275 6465  ....r....Z.crude
+00000d00: 5f6d 6574 686f 645f 6661 6d69 6c79 f514  _method_family..
+00000d10: 0000 00f0 9f92 be20 5341 5649 4e47 2052  ....... SAVING R
+00000d20: 4553 554c 5453 20a9 01da 0b6f 7574 7075  ESULTS ....outpu
+00000d30: 745f 7061 7468 5a16 696e 6665 7272 6564  t_pathZ.inferred
+00000d40: 5f63 7275 6465 5f6d 6574 686f 645f f522  _crude_method_."
+00000d50: 0000 00f0 9f92 be20 5341 5649 4e47 2052  ....... SAVING R
+00000d60: 4553 554c 5453 2046 4f52 204b 4150 5041  ESULTS FOR KAPPA
+00000d70: 2046 494c 45da 0863 6c6f 6e65 5f69 64a9   FILE..clone_id.
+00000d80: 0272 3e00 0000 da09 7061 7274 6974 696f  .r>.....partitio
+00000d90: 6efa 4245 7661 6c75 6174 696e 6720 4869  n.BEvaluating Hi
+00000da0: 6c61 7279 2773 2070 6572 666f 726d 616e  lary's performan
+00000db0: 6365 206f 6e20 6772 6f75 6e64 2074 7275  ce on ground tru
+00000dc0: 7468 2063 6f6c 756d 6e20 2763 6c6f 6e65  th column 'clone
+00000dd0: 5f69 6427 2e29 025a 0f70 7265 6369 7369  _id'.).Z.precisi
+00000de0: 6f6e 5f63 7275 6465 5a11 7365 6e73 6974  on_crudeZ.sensit
+00000df0: 6976 6974 795f 6372 7564 6529 1e72 2100  ivity_crude).r!.
+00000e00: 0000 7204 0000 00da 056d 6b64 6972 da04  ..r......mkdir..
+00000e10: 6e61 6d65 da06 6578 6973 7473 da0a 5661  name..exists..Va
+00000e20: 6c75 6545 7272 6f72 da08 6173 5f70 6f73  lueError..as_pos
+00000e30: 6978 7203 0000 0072 0800 0000 da04 696e  ixr....r......in
+00000e40: 666f 720a 0000 00da 0763 6f6c 756d 6e73  for......columns
+00000e50: da07 7761 726e 696e 67da 0569 6e64 6578  ..warning..index
+00000e60: da06 6173 7479 7065 722d 0000 00da 0573  ..astyper-.....s
+00000e70: 7472 6970 da09 7365 745f 696e 6465 78da  trip..set_index.
+00000e80: 026e 70da 0661 7261 6e67 6572 1000 0000  .np..aranger....
+00000e90: da05 6465 6275 6772 0b00 0000 7205 0000  ..debugr....r...
+00000ea0: 00da 0a70 7265 7072 6f63 6573 7372 0700  ...preprocessr..
+00000eb0: 0000 da07 636c 6173 7365 7372 0600 0000  ....classesr....
+00000ec0: 5a1d 636f 6d70 7574 655f 6372 7564 655f  Z.compute_crude_
+00000ed0: 6d65 7468 6f64 5f63 6c75 7374 6572 7372  method_clustersr
+00000ee0: 0900 0000 2919 7214 0000 0072 1500 0000  ....).r....r....
+00000ef0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000f00: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000f10: 0000 0072 1d00 0000 da0c 6465 6275 675f  ...r......debug_
+00000f20: 666f 6c64 6572 7241 0000 00da 036c 6f67  folderrA.....log
+00000f30: 723a 0000 0072 3b00 0000 da0f 6461 7461  r:...r;.....data
+00000f40: 6672 616d 655f 6b61 7070 6172 3c00 0000  frame_kappar<...
+00000f50: 722a 0000 00da 0761 7072 696f 7269 da13  r*.....apriori..
+00000f60: 6461 7461 6672 616d 655f 7072 6f63 6573  dataframe_proces
+00000f70: 7365 64da 0668 696c 6172 795a 0f64 6174  sed..hilaryZ.dat
+00000f80: 6166 7261 6d65 5f63 7275 6465 da11 6f75  aframe_crude..ou
+00000f90: 7470 7574 5f70 6174 685f 6b61 7070 61da  tput_path_kappa.
+00000fa0: 0970 7265 6369 7369 6f6e da0b 7365 6e73  .precision..sens
+00000fb0: 6974 6976 6974 79a9 0072 6100 0000 fa2f  itivity..ra..../
+00000fc0: 2f68 6f6d 652f 6761 7468 656e 6573 2f67  /home/gathenes/g
+00000fd0: 6974 6c61 622f 4849 4c41 5279 2f68 696c  itlab/HILARy/hil
+00000fe0: 6172 792f 5f5f 6d61 696e 5f5f 2e70 79da  ary/__main__.py.
+00000ff0: 0c63 7275 6465 5f6d 6574 686f 6418 0000  .crude_method...
+00001000: 0073 a800 0000 003c 0801 1201 0e01 0c01  .s.....<........
+00001010: 0e01 1401 0c01 0201 0cff 0403 0801 0601  ................
+00001020: 0c01 0401 0201 06fe 0604 0c01 0a01 0a01  ................
+00001030: 1001 1401 0a01 0401 0601 0a01 0c01 0a01  ................
+00001040: 02ff 0803 0a01 1401 0602 0401 1402 0a01  ................
+00001050: 1401 0401 0201 06fe 0604 0c01 0201 0201  ................
+00001060: 0201 02fd 0605 0e01 0a01 0201 0201 0201  ................
+00001070: 02fd 0605 0401 0201 0201 02fd 0605 0c01  ................
+00001080: 1002 1201 1401 0c01 0601 0c01 1001 0401  ................
+00001090: 0aff 0603 0401 0201 06fe 0604 0c02 1601  ................
+000010a0: 0201 04ff 0a03 0401 0201 0201 02fd 7263  ..............rc
+000010b0: 0000 0067 ae47 e17a 14ae ef3f 7a0b 2d2d  ...g.G.z...?z.--
+000010c0: 7072 6563 6973 696f 6e7a 022d 707a 1943  precisionz.-pz.C
+000010d0: 686f 6f73 6520 6465 7369 7265 6420 7072  hoose desired pr
+000010e0: 6563 6973 696f 6e2e 67cd cccc cccc ccec  ecision.g.......
+000010f0: 3f7a 0d2d 2d73 656e 7369 7469 7669 7479  ?z.--sensitivity
+00001100: 7a02 2d73 7a1b 4368 6f6f 7365 2064 6573  z.-sz.Choose des
+00001110: 6972 6564 2073 656e 7369 7469 7669 7479  ired sensitivity
+00001120: 2e7a 082d 2d73 696c 656e 747a 2244 6f20  .z.--silentz"Do 
+00001130: 6e6f 7420 7368 6f77 2070 726f 6772 6573  not show progres
+00001140: 7320 6261 7273 2069 6620 7573 6564 2e29  s bars if used.)
+00001150: 0d72 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001160: 7217 0000 0072 5f00 0000 7260 0000 00da  r....r_...r`....
+00001170: 0673 696c 656e 7472 1800 0000 7219 0000  .silentr....r...
+00001180: 0072 1a00 0000 721b 0000 00da 0673 6176  .r....r......sav
+00001190: 696e 6772 1e00 0000 630c 0000 0000 0000  ingr....c.......
+000011a0: 0000 0000 001a 0000 0008 0000 0043 0000  .............C..
+000011b0: 0173 4403 0000 7c07 6401 7500 721a 7c00  .sD...|.d.u.r.|.
+000011c0: 6a00 6402 1900 7401 6403 8301 1b00 7d07  j.d...t.d.....}.
+000011d0: 7c07 6a02 6404 6404 6405 8d02 0100 7c07  |.j.d.d.d.....|.
+000011e0: 7401 6406 8301 1b00 7d0c 7c0c 6a02 6404  t.d.....}.|.j.d.
+000011f0: 6404 6405 8d02 0100 7c07 7401 6407 7c00  d.d.....|.t.d.|.
+00001200: 6a03 9b00 9d02 8301 1b00 7d0d 7c0d a004  j.........}.|...
+00001210: a100 7274 7c09 7374 7405 7c0d a006 a100  ..rt|.stt.|.....
+00001220: 9b00 6408 9d02 8301 8201 7c03 6409 6b02  ..d.......|.d.k.
+00001230: 7282 7407 8300 7d03 7408 7c02 7c0a 640a  r.t...}.t.|.|.d.
+00001240: 8d02 7d0e 7c0e 6a09 640b 7c00 a006 a100  ..}.|.j.d.|.....
+00001250: 640c 8d02 0100 740a 7c00 7c08 640d 8d02  d.....t.|.|.d...
+00001260: 7d0f 640e 7c0f 6a0b 7601 72d0 7c0e a00c  }.d.|.j.v.r.|...
+00001270: 640f a101 0100 7c0f 6a0d a00e 6410 a101  d.....|.j...d...
+00001280: 7c0f 640e 3c00 7c0f 640e 1900 6a0f a010  |.d.<.|.d...j...
+00001290: 6411 a101 7c0f 640e 3c00 7c0f a011 640e  d...|.d.<.|...d.
+000012a0: a101 0100 6412 7d10 7c01 9001 7246 7c0e  ....d.}.|...rF|.
+000012b0: a009 6413 a101 0100 740a 7c01 7c08 640d  ..d.....t.|.|.d.
+000012c0: 8d02 7d11 7c11 640e 1900 6a0f a010 6414  ..}.|.d...j...d.
+000012d0: a101 7c11 640e 3c00 7c11 a011 640e a101  ..|.d.<.|...d...
+000012e0: 0100 7412 a013 6415 6416 6417 a103 a00e  ..t...d.d.d.....
+000012f0: 7414 a101 7d12 6404 7d10 6e18 6401 7d11  t...}.d.}.n.d.}.
+00001300: 7412 a013 6418 6419 6417 a103 a00e 7414  t...d.d.d.....t.
+00001310: a101 7d12 7415 7c10 7c12 7c03 7c04 7c05  ..}.t.|.|.|.|.|.
+00001320: 7c06 641a 8d06 7d13 7c13 6a16 7c0f 7c11  |.d...}.|.j.|.|.
+00001330: 641b 8d02 7d14 7417 7c14 8301 7c13 5f18  d...}.t.|...|._.
+00001340: 7c0e a009 641c a101 0100 7c13 a019 7c14  |...d.....|...|.
+00001350: a101 0100 7c02 641d 6b05 9001 72da 7c0c  ....|.d.k...r.|.
+00001360: 7401 641e 7c00 6a03 9b00 9d02 8301 1b00  t.d.|.j.........
+00001370: 7d15 7c0e 6a1a 641f 7c15 a006 a100 6420  }.|.j.d.|.....d 
+00001380: 8d02 0100 741b 7c13 6a1c 7c15 8302 0100  ....t.|.j.|.....
+00001390: 7c0e a009 6421 a101 0100 7c13 a01d a100  |...d!....|.....
+000013a0: 0100 7c0e a009 6422 a101 0100 7c13 a01e  ..|...d"....|...
+000013b0: a100 0100 7c02 641d 6b05 9002 723a 7c0c  ....|.d.k...r:|.
+000013c0: 7401 6423 7c00 6a03 9b00 9d02 8301 1b00  t.d#|.j.........
+000013d0: 7d16 7c0e 6a1a 6424 7c16 a006 a100 6420  }.|.j.d$|.....d 
+000013e0: 8d02 0100 741b 7c13 6a18 7c16 8302 0100  ....t.|.j.|.....
+000013f0: 7c0e a009 6425 a101 0100 741f 7c13 7c14  |...d%....t.|.|.
+00001400: 6426 8d02 7d17 7c17 a020 7c14 a101 7d18  d&..}.|.. |...}.
+00001410: 7c18 6427 1900 7c0f 6428 3c00 7c0f 640e  |.d'..|.d(<.|.d.
+00001420: 1900 6411 1700 7c0f 640e 3c00 7c0b 9003  ..d...|.d.<.|...
+00001430: 7202 7c0e 6a09 6429 7c0d a006 a100 642a  r.|.j.d)|.....d*
+00001440: 8d02 0100 7c07 7401 642b 7c00 6a03 9b00  ....|.t.d+|.j...
+00001450: 9d02 8301 1b00 7d0d 741b 7c0f 7c0d 642c  ......}.t.|.|.d,
+00001460: 8d02 0100 7c10 9003 7202 7c18 6427 1900  ....|...r.|.d'..
+00001470: 7c11 6428 3c00 7c0f 640e 1900 6414 1700  |.d(<.|.d...d...
+00001480: 7c11 640e 3c00 7c07 7401 642b 7c01 6a03  |.d.<.|.t.d+|.j.
+00001490: 9b00 9d02 8301 1b00 7d19 7c0e 6a09 642d  ........}.|.j.d-
+000014a0: 7c19 a006 a100 642a 8d02 0100 741b 7c11  |.....d*....t.|.
+000014b0: 7c19 642c 8d02 0100 7c02 641d 6b05 9003  |.d,....|.d.k...
+000014c0: 7238 642e 7c0f 6a0b 7600 9003 7238 7421  r8d.|.j.v...r8t!
+000014d0: 7c0f 6428 642f 8d02 5c02 7d04 7d05 7c0e  |.d(d/..\.}.}.|.
+000014e0: 6a1a 6430 7c04 7c05 6431 8d03 0100 7c18  j.d0|.|.d1....|.
+000014f0: 7c0f 7c11 7c17 6604 5300 2932 7a3a 496e  |.|.|.f.S.)2z:In
+00001500: 6665 7220 6c69 6e65 6167 6573 2077 6974  fer lineages wit
+00001510: 6820 4849 4c41 5279 2d43 4452 3320 6672  h HILARy-CDR3 fr
+00001520: 6f6d 2064 6174 615f 7061 7468 2065 7863  om data_path exc
+00001530: 656c 2066 696c 652e 4e72 0100 0000 721f  el file.Nr....r.
+00001540: 0000 0054 7220 0000 0072 2300 0000 7224  ...Tr ...r#...r$
+00001550: 0000 0072 2500 0000 720f 0000 0072 2600  ...r%...r....r&.
+00001560: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
+00001570: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00001580: 722e 0000 0046 722f 0000 0072 3000 0000  r....Fr/...r0...
+00001590: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
+000015a0: 3400 0000 7235 0000 0029 0672 3b00 0000  4...r5...).r;...
+000015b0: 723c 0000 0072 1700 0000 725f 0000 0072  r<...r....r_...r
+000015c0: 6000 0000 7264 0000 0072 3d00 0000 751d  `...rd...r=...u.
+000015d0: 0000 00e2 8fb3 2043 4f4d 5055 5449 4e47  ...... COMPUTING
+000015e0: 2048 4953 544f 4752 414d 5320 e28f b32e   HISTOGRAMS ....
+000015f0: 7236 0000 005a 0b68 6973 746f 6772 616d  r6...Z.histogram
+00001600: 735f 7a21 5361 7669 6e67 2068 6973 746f  s_z!Saving histo
+00001610: 6772 616d 7320 7573 6564 2062 7920 4869  grams used by Hi
+00001620: 6c61 7279 2e72 3700 0000 751d 0000 00e2  lary.r7...u.....
+00001630: 8fb3 2043 4f4d 5055 5449 4e47 2050 4152  .. COMPUTING PAR
+00001640: 414d 4554 4552 5320 e28f b32e 751d 0000  AMETERS ....u...
+00001650: 00e2 8fb3 2043 4f4d 5055 5449 4e47 2054  .... COMPUTING T
+00001660: 4852 4553 484f 4c44 5320 e28f b32e da0b  HRESHOLDS ......
+00001670: 7061 7261 6d65 7465 7273 5ffa 2953 6176  parameters_.)Sav
+00001680: 696e 6720 616c 6c20 7061 7261 6d65 7465  ing all paramete
+00001690: 7273 2069 6e66 6572 7265 6420 6279 2048  rs inferred by H
+000016a0: 696c 6172 792e 7531 0000 00e2 8fb3 2043  ilary.u1...... C
+000016b0: 4f4d 5055 5449 4e47 2050 5245 4349 5345  OMPUTING PRECISE
+000016c0: 2041 4e44 2053 454e 5349 5449 5645 2043   AND SENSITIVE C
+000016d0: 4c55 5354 4552 5320 e28f b32e a901 723e  LUSTERS ......r>
+000016e0: 0000 005a 0f70 7265 6369 7365 5f63 6c75  ...Z.precise_clu
+000016f0: 7374 6572 da11 6364 7233 5f62 6173 6564  ster..cdr3_based
+00001700: 5f66 616d 696c 7972 3f00 0000 7240 0000  _familyr?...r@..
+00001710: 005a 1469 6e66 6572 7265 645f 6364 7233  .Z.inferred_cdr3
+00001720: 5f62 6173 6564 5f72 3900 0000 7242 0000  _based_r9...rB..
+00001730: 0072 4300 0000 7244 0000 0072 4600 0000  .rC...rD...rF...
+00001740: 2902 da0e 7072 6563 6973 696f 6e5f 6364  )...precision_cd
+00001750: 7233 da10 7365 6e73 6974 6976 6974 795f  r3..sensitivity_
+00001760: 6364 7233 2922 7221 0000 0072 0400 0000  cdr3)"r!...r....
+00001770: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
+00001780: 4a00 0000 724b 0000 0072 0300 0000 7208  J...rK...r....r.
+00001790: 0000 0072 4c00 0000 720a 0000 0072 4d00  ...rL...r....rM.
+000017a0: 0000 724e 0000 0072 4f00 0000 7250 0000  ..rN...rO...rP..
+000017b0: 0072 2d00 0000 7251 0000 0072 5200 0000  .r-...rQ...rR...
+000017c0: 7253 0000 0072 5400 0000 7210 0000 0072  rS...rT...r....r
+000017d0: 0500 0000 7256 0000 0072 0700 0000 7257  ....rV...r....rW
+000017e0: 0000 005a 0e67 6574 5f68 6973 746f 6772  ...Z.get_histogr
+000017f0: 616d 7372 5500 0000 720b 0000 005a 0a68  amsrU...r....Z.h
+00001800: 6973 746f 6772 616d 735a 0e67 6574 5f70  istogramsZ.get_p
+00001810: 6172 616d 6574 6572 735a 0e67 6574 5f74  arametersZ.get_t
+00001820: 6872 6573 686f 6c64 7372 0600 0000 5a1a  hresholdsr....Z.
+00001830: 636f 6d70 7574 655f 7072 6563 5f73 656e  compute_prec_sen
+00001840: 735f 636c 7573 7465 7273 7209 0000 0029  s_clustersr....)
+00001850: 1a72 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001860: 7217 0000 0072 5f00 0000 7260 0000 0072  r....r_...r`...r
+00001870: 6400 0000 7218 0000 0072 1900 0000 721a  d...r....r....r.
+00001880: 0000 0072 1b00 0000 7265 0000 0072 5800  ...r....re...rX.
+00001890: 0000 7241 0000 0072 5900 0000 723a 0000  ..rA...rY...r:..
+000018a0: 0072 3b00 0000 725a 0000 0072 3c00 0000  .r;...rZ...r<...
+000018b0: 725b 0000 0072 5c00 0000 5a0e 6869 7374  r[...r\...Z.hist
+000018c0: 6f67 7261 6d5f 7061 7468 da0f 7061 7261  ogram_path..para
+000018d0: 6d65 7465 7273 5f70 6174 6872 5d00 0000  meters_pathr]...
+000018e0: da0e 6461 7461 6672 616d 655f 6364 7233  ..dataframe_cdr3
+000018f0: 725e 0000 0072 6100 0000 7261 0000 0072  r^...ra...ra...r
+00001900: 6200 0000 da0b 6364 7233 5f6d 6574 686f  b.....cdr3_metho
+00001910: 64ae 0000 0073 be00 0000 0042 0801 1201  d....s.....B....
+00001920: 0e01 0c01 0e01 1401 0c01 0201 0cff 0403  ................
+00001930: 0801 0601 0c01 0401 0201 06fe 0604 0c01  ................
+00001940: 0a01 0a01 1001 1401 0a01 0401 0601 0a01  ................
+00001950: 0c01 0a01 02ff 0803 0a01 1401 0602 0401  ................
+00001960: 1402 0201 0201 0201 0201 0201 0201 02fa  ................
+00001970: 0608 0e01 0a02 0a01 0a02 0a01 1401 1201  ................
+00001980: 0c02 0a01 0802 0a01 0801 0a01 1401 0401  ................
+00001990: 0201 06fe 0604 0c02 0a01 0201 0201 02fe  ................
+000019a0: 0604 0a02 0c01 1002 0601 1201 1401 0c01  ................
+000019b0: 0601 0c01 1001 0401 0aff 0603 0401 0201  ................
+000019c0: 06fe 0604 0c02 1601 0201 04ff 0a03 0401  ................
+000019d0: 0201 0201 02fd 0605 726e 0000 007a 132d  ........rn...z.-
+000019e0: 2d77 6974 686f 7574 2d68 6575 7269 7374  -without-heurist
+000019f0: 6963 7a33 444f 206e 6f74 2075 7365 2068  icz3DO not use h
+00001a00: 6575 7269 7374 6963 2066 6f72 2063 686f  euristic for cho
+00001a10: 6f73 696e 6720 7468 6520 7879 2074 6872  osing the xy thr
+00001a20: 6573 686f 6c64 2e29 0d72 1400 0000 7215  eshold.).r....r.
+00001a30: 0000 0072 1600 0000 7217 0000 0072 5f00  ...r....r....r_.
+00001a40: 0000 7260 0000 0072 6400 0000 7218 0000  ..r`...rd...r...
+00001a50: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00001a60: da11 7769 7468 6f75 745f 6865 7572 6973  ..without_heuris
+00001a70: 7469 6372 1e00 0000 630c 0000 0000 0000  ticr....c.......
+00001a80: 0000 0000 001b 0000 000e 0000 0043 0000  .............C..
+00001a90: 0173 d401 0000 7c07 6401 7500 721a 7c00  .s....|.d.u.r.|.
+00001aa0: 6a00 6402 1900 7401 6403 8301 1b00 7d07  j.d...t.d.....}.
+00001ab0: 7c07 6a02 6404 6404 6405 8d02 0100 7c07  |.j.d.d.d.....|.
+00001ac0: 7401 6406 8301 1b00 7d0c 7c01 723e 6407  t.d.....}.|.r>d.
+00001ad0: 7d0d 6e04 6402 7d0d 7403 7c02 7c0a 6408  }.n.d.}.t.|.|.d.
+00001ae0: 8d02 7d0e 7404 7c00 7c01 7c02 7c03 7c04  ..}.t.|.|.|.|.|.
+00001af0: 7c05 7c06 7c07 7c08 7c09 7c0a 6409 640a  |.|.|.|.|.|.d.d.
+00001b00: 8d0c 5c04 7d0f 7d10 7d11 7d12 7c0b 7286  ..\.}.}.}.}.|.r.
+00001b10: 7c0d 7c12 6a05 640b 3c00 6e2a 7c0e a006  |.|.j.d.<.n*|...
+00001b20: 640c a101 0100 7c12 6a07 7c0f 640d 8d01  d.....|.j.|.d...
+00001b30: 0100 7c12 6a05 640b 1900 7c0d 1700 7c12  ..|.j.d...|...|.
+00001b40: 6a05 640b 3c00 7c02 640e 6b05 72ea 7c0c  j.d.<.|.d.k.r.|.
+00001b50: 7401 640f 7c00 6a08 9b00 9d02 8301 1b00  t.d.|.j.........
+00001b60: 7d13 7c0e 6a09 6410 7c13 a00a a100 6411  }.|.j.d.|.....d.
+00001b70: 8d02 0100 740b 7c12 6a05 7c13 8302 0100  ....t.|.j.|.....
+00001b80: 7c0e a006 6412 a101 0100 7c12 6a0c 7c0f  |...d.....|.j.|.
+00001b90: 640d 8d01 7d14 7c14 6413 1900 7c10 6413  d...}.|.d...|.d.
+00001ba0: 3c00 7c07 7401 6414 7c00 6a08 9b00 9d02  <.|.t.d.|.j.....
+00001bb0: 8301 1b00 7d15 7c0e 6a06 6415 7c15 a00a  ....}.|.j.d.|...
+00001bc0: a100 6416 8d02 0100 740b 7c10 7c15 6417  ..d.....t.|.|.d.
+00001bd0: 8d02 0100 7c11 6401 7501 9001 7286 7c14  ....|.d.u...r.|.
+00001be0: 6413 1900 7c11 6413 3c00 7c07 7401 6414  d...|.d.<.|.t.d.
+00001bf0: 7c01 6a08 9b00 9d02 8301 1b00 7d16 7c0e  |.j.........}.|.
+00001c00: 6a06 6418 7c16 a00a a100 6416 8d02 0100  j.d.|.....d.....
+00001c10: 740b 7c11 7c16 6417 8d02 0100 7c02 640e  t.|.|.d.....|.d.
+00001c20: 6b05 9001 72d0 6419 7c10 6a0d 7600 9001  k...r.d.|.j.v...
+00001c30: 72d0 740e 7c10 6413 641a 8d02 5c02 7d17  r.t.|.d.d...\.}.
+00001c40: 7d18 740e 7c10 641b 641a 8d02 5c02 7d19  }.t.|.d.d...\.}.
+00001c50: 7d1a 7c0e 6a09 641c 7c17 7c18 7c19 7c1a  }.|.j.d.|.|.|.|.
+00001c60: 641d 8d05 0100 6401 5300 291e 7a3a 496e  d.....d.S.).z:In
+00001c70: 6665 7220 6c69 6e65 6167 6573 2077 6974  fer lineages wit
+00001c80: 6820 4849 4c41 5279 2d66 756c 6c20 6672  h HILARy-full fr
+00001c90: 6f6d 2064 6174 615f 7061 7468 2065 7863  om data_path exc
+00001ca0: 656c 2066 696c 652e 4e72 0100 0000 721f  el file.Nr....r.
+00001cb0: 0000 0054 7220 0000 0072 2300 0000 e904  ...Tr ...r#.....
+00001cc0: 0000 0072 2600 0000 4629 0c72 1400 0000  ...r&...F).r....
+00001cd0: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00001ce0: 5f00 0000 7260 0000 0072 6400 0000 7218  _...r`...rd...r.
+00001cf0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00001d00: 0000 7265 0000 00da 0c78 795f 7468 7265  ..re.....xy_thre
+00001d10: 7368 6f6c 6475 2000 0000 e28f b320 434f  sholdu ...... CO
+00001d20: 4d50 5554 494e 4720 5859 2054 4852 4553  MPUTING XY THRES
+00001d30: 484f 4c44 5320 e28f b32e 7268 0000 0072  HOLDS ....rh...r
+00001d40: 3600 0000 7266 0000 0072 6700 0000 7237  6...rf...rg...r7
+00001d50: 0000 0075 2e00 0000 e28f b320 494e 4645  ...u....... INFE
+00001d60: 5252 494e 4720 4641 4d49 4c49 4553 2057  RRING FAMILIES W
+00001d70: 4954 4820 4655 4c4c 2058 5920 4d45 5448  ITH FULL XY METH
+00001d80: 4f44 e28f b32e 5a06 6661 6d69 6c79 5a15  OD....Z.familyZ.
+00001d90: 696e 6665 7272 6564 5f66 756c 6c5f 6d65  inferred_full_me
+00001da0: 7468 6f64 5f72 3f00 0000 7240 0000 0072  thod_r?...r@...r
+00001db0: 3900 0000 7242 0000 0072 4300 0000 7244  9...rB...rC...rD
+00001dc0: 0000 0072 6900 0000 7246 0000 0029 045a  ...ri...rF...).Z
+00001dd0: 1570 7265 6369 7369 6f6e 5f66 756c 6c5f  .precision_full_
+00001de0: 6d65 7468 6f64 5a17 7365 6e73 6974 6976  methodZ.sensitiv
+00001df0: 6974 795f 6675 6c6c 5f6d 6574 686f 6472  ity_full_methodr
+00001e00: 6a00 0000 726b 0000 0029 0f72 2100 0000  j...rk...).r!...
+00001e10: 7204 0000 0072 4700 0000 7208 0000 0072  r....rG...r....r
+00001e20: 6e00 0000 7257 0000 0072 4c00 0000 5a11  n...rW...rL...Z.
+00001e30: 6765 745f 7879 5f74 6872 6573 686f 6c64  get_xy_threshold
+00001e40: 7372 4800 0000 7255 0000 0072 4b00 0000  srH...rU...rK...
+00001e50: 720b 0000 005a 0569 6e66 6572 724d 0000  r....Z.inferrM..
+00001e60: 0072 0900 0000 291b 7214 0000 0072 1500  .r....).r....r..
+00001e70: 0000 7216 0000 0072 1700 0000 725f 0000  ..r....r....r_..
+00001e80: 0072 6000 0000 7264 0000 0072 1800 0000  .r`...rd...r....
+00001e90: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00001ea0: 6f00 0000 7258 0000 0072 7100 0000 7259  o...rX...rq...rY
+00001eb0: 0000 0072 6d00 0000 723a 0000 0072 5a00  ...rm...r:...rZ.
+00001ec0: 0000 725d 0000 0072 6c00 0000 5a12 6461  ..r]...rl...Z.da
+00001ed0: 7461 6672 616d 655f 696e 6665 7272 6564  taframe_inferred
+00001ee0: 7241 0000 0072 5e00 0000 5a0e 7072 6563  rA...r^...Z.prec
+00001ef0: 6973 696f 6e5f 6675 6c6c 5a10 7365 6e73  ision_fullZ.sens
+00001f00: 6974 6976 6974 795f 6675 6c6c 726a 0000  itivity_fullrj..
+00001f10: 0072 6b00 0000 7261 0000 0072 6100 0000  .rk...ra...ra...
+00001f20: 7262 0000 00da 0b66 756c 6c5f 6d65 7468  rb.....full_meth
+00001f30: 6f64 5b01 0000 7380 0000 0000 4608 0112  od[...s.....F...
+00001f40: 010e 010c 0104 0106 0204 010c 0202 0102  ................
+00001f50: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001f60: 0102 0102 0102 f40e 0e04 010c 020a 010c  ................
+00001f70: 0114 0108 0114 0104 0102 0106 fe06 040c  ................
+00001f80: 020a 010c 020c 0214 0112 020c 020a 010c  ................
+00001f90: 0104 010a ff06 0304 0102 0106 fe06 040c  ................
+00001fa0: 0216 0102 0104 ff0a 0302 0104 ff0a 0304  ................
+00001fb0: 0102 0102 0102 0102 0102 fb72 7200 0000  ...........rr...
+00001fc0: da08 5f5f 6d61 696e 5f5f 291d da07 5f5f  ..__main__)...__
+00001fd0: 646f 635f 5fda 0a5f 5f66 7574 7572 655f  doc__..__future_
+00001fe0: 5f72 0200 0000 5a0f 6d75 6c74 6970 726f  _r....Z.multipro
+00001ff0: 6365 7373 696e 6772 0300 0000 da07 7061  cessingr......pa
+00002000: 7468 6c69 6272 0400 0000 5a05 6e75 6d70  thlibr....Z.nump
+00002010: 7972 5300 0000 5a05 7479 7065 725a 0e68  yrS...Z.typerZ.h
+00002020: 696c 6172 792e 6170 7269 6f72 6972 0500  ilary.apriorir..
+00002030: 0000 5a10 6869 6c61 7279 2e69 6e66 6572  ..Z.hilary.infer
+00002040: 656e 6365 7206 0000 005a 0c68 696c 6172  encer....Z.hilar
+00002050: 792e 7574 696c 7372 0700 0000 7208 0000  y.utilsr....r...
+00002060: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00002070: 5a05 5479 7065 725a 0361 7070 5a07 636f  Z.TyperZ.appZ.co
+00002080: 6d6d 616e 645a 0841 7267 756d 656e 745a  mmandZ.ArgumentZ
+00002090: 064f 7074 696f 6e72 6300 0000 726e 0000  .Optionrc...rn..
+000020a0: 0072 7200 0000 da08 5f5f 6e61 6d65 5f5f  .rr.....__name__
+000020b0: 7261 0000 0072 6100 0000 7261 0000 0072  ra...ra...ra...r
+000020c0: 6200 0000 da08 3c6d 6f64 756c 653e 0100  b.....<module>..
+000020d0: 0000 7392 0100 0004 020c 020c 010c 0208  ..s.............
+000020e0: 0108 020c 010c 011c 080c 0306 0204 0102  ................
+000020f0: 0102 0102 fd04 0504 0102 0102 0102 fd04  ................
+00002100: 0504 0102 0102 0102 0102 0102 fb04 0704  ................
+00002110: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
+00002120: 0102 fd04 0504 0102 0102 0102 fd04 0604  ................
+00002130: 0102 0102 0102 fd04 0504 0102 0102 0102  ................
+00002140: fd04 0504 0102 0102 0102 0102 fc04 0604  ................
+00002150: 0102 0102 0102 0102 fc04 cd26 7f00 1606  ...........&....
+00002160: 0204 0102 0102 0102 fd04 0504 0102 0102  ................
+00002170: 0102 fd04 0504 0102 0102 0102 0102 0102  ................
+00002180: fb04 0704 0102 0102 0102 0102 fc04 0604  ................
+00002190: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
+000021a0: 0102 0102 fc04 0604 0102 0102 0102 fd04  ................
+000021b0: 0504 0102 0102 0102 fd04 0504 0102 0102  ................
+000021c0: 0102 fd04 0604 0102 0102 0102 fd04 0504  ................
+000021d0: 0102 0102 0102 fd04 0502 c22a 7f00 2d06  ...........*..-.
+000021e0: 0204 0102 0102 0102 fd04 0504 0102 0102  ................
+000021f0: 0102 fd04 0504 0102 0102 0102 0102 0102  ................
+00002200: fb04 0704 0102 0102 0102 0102 fc04 0604  ................
+00002210: 0102 0102 0102 0102 fc04 0604 0102 0102  ................
+00002220: 0102 0102 fc04 0604 0102 0102 0102 fd04  ................
+00002230: 0504 0102 0102 0102 fd04 0504 0102 0102  ................
+00002240: 0102 fd04 0604 0102 0102 0102 fd04 0504  ................
+00002250: 0102 0102 0102 fd04 0504 0102 0102 0102  ................
+00002260: fd04 c22a 7f00 110a 01                   ...*.....
```

### Comparing `hilary-1.2.0/hilary/__pycache__/apriori.cpython-39.pyc` & `hilary-1.2.1/hilary/__pycache__/apriori.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar  5 03:42:57 2024 UTC, .py size: 10204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c194 e665 dc27 0000  a..........e.'..
+00000000: 610d 0d0a 0000 0000 352a fc65 e227 0000  a.......5*.e.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 b400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6403 6c0a  d.l.m.Z...d.d.l.
 00000070: 5a0b 6401 6403 6c0c 5a0d 6401 6403 6c0e  Z.d.d.l.Z.d.d.l.
@@ -421,143 +421,143 @@
 00001a40: 616d 6574 6572 73ca 0000 0073 3a00 0000  ameters....s:...
 00001a50: 0002 0a01 0201 02ff 0403 0201 0c01 0401  ................
 00001a60: 0401 04fc 0605 02fb 0607 0c01 0802 0202  ................
 00001a70: 0201 02fe 02ff 0405 02fb 0c06 0e01 0e02  ................
 00001a80: 10ff 0803 1601 0a01 02ff 7a16 4170 7269  ..........z.Apri
 00001a90: 6f72 692e 6765 745f 7061 7261 6d65 7465  ori.get_paramete
 00001aa0: 7273 6302 0000 0000 0000 0000 0000 000c  rsc.............
-00001ab0: 0000 0006 0000 0003 0000 0173 4a01 0000  ...........sJ...
-00001ac0: 7c01 5c02 7d02 7d03 7c02 6401 1900 7d04  |.\.}.}.|.d...}.
-00001ad0: 7c04 8801 6a00 6402 1900 6b04 7334 7c04  |...j.d...k.s4|.
-00001ae0: 8801 6a00 6401 1900 6b00 7334 7c04 6403  ..j.d...k.s4|.d.
-00001af0: 1600 7266 7401 6a02 7403 7c03 8301 6404  ..rft.j.t.|...d.
-00001b00: 6602 7404 6405 8d02 7c04 1400 6406 1a00  f.t.d...|...d...
-00001b10: 7c03 6407 6408 6702 3c00 7c03 6407 6408  |.d.d.g.<.|.d.d.
-00001b20: 6702 1900 5300 7c03 6409 1900 7d05 7c03  g...S.|.d...}.|.
-00001b30: 640a 1900 7c04 1400 7d06 7401 a005 7c04  d...|...}.t...|.
-00001b40: 640b 1700 a101 8900 8801 6a06 6a07 8801  d.........j.j...
-00001b50: 6a06 640c 1900 7c04 6b02 1900 6a08 6401  j.d...|.k...j.d.
-00001b60: 640b 7c04 6404 1700 8502 6602 1900 7d07  d.|.d.....f...}.
-00001b70: 7401 a009 8700 6601 640d 640e 8408 7c06  t.....f.d.d...|.
-00001b80: 4400 8301 a101 740a 8800 8301 1b00 6a0b  D.....t.......j.
-00001b90: 640b 640f 8d01 7d08 7c07 7c08 1b00 7d09  d.d...}.|.|...}.
-00001ba0: 7c08 8801 6a0c 6b00 6a0d 640b 640f 8d01  |...j.k.j.d.d...
-00001bb0: 7d0a 7401 a009 8701 6601 6410 640e 8408  }.t.....f.d.d...
-00001bc0: 740e 7c09 7c05 8302 4400 8301 a101 6a0d  t.|.|...D.....j.
-00001bd0: 640b 640f 8d01 640b 1800 7d0b 7401 6a0f  d.d...d...}.t.j.
-00001be0: 7c0b 7c0a 6702 6401 640f 8d02 7d0b 7c0b  |.|.g.d.d...}.|.
-00001bf0: 7c03 6407 3c00 7c0a 7c03 6408 3c00 7c03  |.d.<.|.|.d.<.|.
-00001c00: 6407 6408 6702 1900 5300 2911 6102 0100  d.d.g...S.).a...
-00001c10: 0041 7373 6967 6e20 7072 6563 6973 6520  .Assign precise 
-00001c20: 616e 6420 7365 6e73 6974 6976 6520 7468  and sensitive th
-00001c30: 7265 7368 6f6c 6473 2074 6f20 6461 7461  resholds to data
-00001c40: 6672 616d 6520 6772 6f75 7065 6420 6279  frame grouped by
-00001c50: 206c 656e 6774 682e 0a0a 2020 2020 2020   length...      
-00001c60: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00001c70: 2020 2020 6172 6773 2074 7570 6c65 5b74      args tuple[t
-00001c80: 7570 6c65 5b69 6e74 5d2c 7064 2e44 6174  uple[int],pd.Dat
-00001c90: 6146 7261 6d65 5d3a 206c 656e 6774 682c  aFrame]: length,
-00001ca0: 2064 6174 6166 7261 6d65 2067 726f 7570   dataframe group
-00001cb0: 6564 2062 7920 6c65 6e67 7468 2e0a 2020  ed by length..  
-00001cc0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00001cd0: 2020 2020 2020 2020 2020 2070 642e 4461             pd.Da
-00001ce0: 7461 4672 616d 653a 2050 7265 6369 7365  taFrame: Precise
-00001cf0: 2061 6e64 2073 656e 7369 7469 7665 2074   and sensitive t
-00001d00: 6872 6573 686f 6c64 732e 0a20 2020 2020  hresholds..     
-00001d10: 2020 2072 0100 0000 7232 0000 0072 0f00     r....r2...r..
-00001d20: 0000 7231 0000 0029 01da 0564 7479 7065  ..r1...)...dtype
-00001d30: e905 0000 00da 1170 7265 6369 7365 5f74  .......precise_t
-00001d40: 6872 6573 686f 6c64 da13 7365 6e73 6974  hreshold..sensit
-00001d50: 6976 655f 7468 7265 7368 6f6c 6472 6900  ive_thresholdri.
-00001d60: 0000 726a 0000 0072 1000 0000 7259 0000  ..rj...r....rY..
-00001d70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001d80: 0000 0600 0000 1300 0001 7320 0000 0067  ..........s ...g
-00001d90: 007c 005d 187d 017c 0188 0013 0074 00a0  .|.].}.|.....t..
-00001da0: 017c 010b 00a1 0114 0091 0271 0453 0072  .|.........q.S.r
-00001db0: 2600 0000 2902 7238 0000 00da 0365 7870  &...).r8.....exp
-00001dc0: 2902 7249 0000 00da 026d 7529 0172 3300  ).rI.....mu).r3.
-00001dd0: 0000 7226 0000 0072 2700 0000 724e 0000  ..r&...r'...rN..
-00001de0: 0002 0100 00f3 0000 0000 7a3f 4170 7269  ..........z?Apri
-00001df0: 6f72 692e 6173 7369 676e 5f70 7265 6369  ori.assign_preci
-00001e00: 7365 5f73 656e 7369 7469 7665 5f74 6872  se_sensitive_thr
-00001e10: 6573 686f 6c64 732e 3c6c 6f63 616c 733e  esholds.<locals>
-00001e20: 2e3c 6c69 7374 636f 6d70 3e72 6700 0000  .<listcomp>rg...
-00001e30: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00001e40: 0006 0000 0013 0000 0173 3000 0000 6700  .........s0...g.
-00001e50: 7c00 5d28 5c02 7d01 7d02 7c01 7c02 6400  |.](\.}.}.|.|.d.
-00001e60: 7c02 1800 1b00 6401 8800 6a00 1800 1400  |.....d...j.....
-00001e70: 8800 6a00 1b00 6b00 9102 7104 5300 2902  ..j...k...q.S.).
-00001e80: 6772 c45a 7c0a 00f0 3f72 1000 0000 2901  gr.Z|...?r....).
-00001e90: 7216 0000 0029 0372 4900 0000 da01 705a  r....).rI.....pZ
-00001ea0: 0372 686f a901 7225 0000 0072 2600 0000  .rho..r%...r&...
-00001eb0: 7227 0000 0072 4e00 0000 0801 0000 7304  r'...rN.......s.
-00001ec0: 0000 0006 0206 ff29 1072 1400 0000 7238  .......).r....r8
-00001ed0: 0000 00da 046f 6e65 73da 036c 656e 7211  .....ones..lenr.
-00001ee0: 0000 00da 0661 7261 6e67 6572 2200 0000  .....aranger"...
-00001ef0: 7262 0000 0072 3600 0000 da05 6172 7261  rb...r6.....arra
-00001f00: 7972 0600 0000 da06 6375 6d73 756d 7217  yr......cumsumr.
-00001f10: 0000 00da 0373 756d da03 7a69 7072 4700  .....sum..ziprG.
-00001f20: 0000 290c 7225 0000 0072 3000 0000 5a07  ..).r%...r0...Z.
-00001f30: 7475 706c 655f 6c5a 036c 6466 7259 0000  tuple_lZ.ldfrY..
-00001f40: 005a 0472 686f 735a 036d 7573 5a04 6364  .Z.rhosZ.musZ.cd
-00001f50: 6630 5a04 6364 6631 5a02 7073 5a06 745f  f0Z.cdf1Z.psZ.t_
-00001f60: 7365 6e73 5a06 745f 7072 6563 7226 0000  sensZ.t_precr&..
-00001f70: 0029 0272 3300 0000 7225 0000 0072 2700  .).r3...r%...r'.
-00001f80: 0000 da23 6173 7369 676e 5f70 7265 6369  ...#assign_preci
-00001f90: 7365 5f73 656e 7369 7469 7665 5f74 6872  se_sensitive_thr
-00001fa0: 6573 686f 6c64 73ea 0000 0073 3c00 0000  esholds....s<...
-00001fb0: 000b 0801 0801 2402 1cff 0a03 0c02 0801  ......$.........
-00001fc0: 0c01 0e01 2802 1eff 0202 02fe 0603 0801  ....(...........
-00001fd0: 1202 0401 0a02 08fe 04ff 0405 02fb 0406  ................
-00001fe0: 02fa 02ff 0209 1201 0801 0801 7a2b 4170  ............z+Ap
-00001ff0: 7269 6f72 692e 6173 7369 676e 5f70 7265  riori.assign_pre
-00002000: 6369 7365 5f73 656e 7369 7469 7665 5f74  cise_sensitive_t
-00002010: 6872 6573 686f 6c64 7363 0100 0000 0000  hresholdsc......
-00002020: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00002030: 0001 732e 0000 0074 007c 006a 01a0 0264  ..s....t.|.j...d
-00002040: 0167 01a1 017c 006a 037c 006a 047c 006a  .g...|.j.|.j.|.j
-00002050: 0564 028d 047c 006a 0164 0364 0467 023c  .d...|.j.d.d.g.<
-00002060: 0064 0553 0029 067a 3541 7373 6967 6e20  .d.S.).z5Assign 
-00002070: 7468 7265 7368 6f6c 6473 2075 7369 6e67  thresholds using
-00002080: 206e 756c 6c20 6469 7374 7269 6275 7469   null distributi
-00002090: 6f6e 2066 726f 6d20 6d6f 6465 6c2e 7243  on from model.rC
-000020a0: 0000 0072 4f00 0000 7270 0000 0072 7100  ...rO...rp...rq.
-000020b0: 0000 4e29 0672 0900 0000 7224 0000 0072  ..N).r....r$...r
-000020c0: 5000 0000 727e 0000 0072 1800 0000 721a  P...r~...r....r.
-000020d0: 0000 0072 7600 0000 7226 0000 0072 2600  ...rv...r&...r&.
-000020e0: 0000 7227 0000 00da 0e67 6574 5f74 6872  ..r'.....get_thr
-000020f0: 6573 686f 6c64 7314 0100 0073 0c00 0000  esholds....s....
-00002100: 0002 0201 0c01 0401 0401 04fc 7a16 4170  ............z.Ap
-00002110: 7269 6f72 692e 6765 745f 7468 7265 7368  riori.get_thresh
-00002120: 6f6c 6473 2901 4e29 11da 085f 5f6e 616d  olds).N)...__nam
-00002130: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00002140: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00002150: 5f64 6f63 5f5f 7238 0000 0072 7900 0000  _doc__r8...ry...
-00002160: da06 6173 7479 7065 7211 0000 0072 2800  ..astyper....r(.
-00002170: 0000 720a 0000 0072 4000 0000 7256 0000  ..r....r@...rV..
-00002180: 0072 5700 0000 7265 0000 0072 6d00 0000  .rW...re...rm...
-00002190: 727e 0000 0072 7f00 0000 7226 0000 0072  r~...r....r&...r
-000021a0: 2600 0000 7226 0000 0072 2700 0000 720c  &...r&...r'...r.
-000021b0: 0000 0018 0000 0073 2600 0000 0801 0404  .......s&.......
-000021c0: 1201 0601 0201 0201 0201 0201 0201 02f7  ................
-000021d0: 1e2f 00ff 141c 0e11 1021 100e 1025 0e20  ./.......!...%. 
-000021e0: 102a 720c 0000 0029 1e72 8300 0000 da0a  .*r....).r......
-000021f0: 5f5f 6675 7475 7265 5f5f 7202 0000 0072  __future__r....r
-00002200: 1e00 0000 da09 6974 6572 746f 6f6c 7372  ......itertoolsr
-00002210: 0300 0000 da0f 6d75 6c74 6970 726f 6365  ......multiproce
-00002220: 7373 696e 6772 0400 0000 da07 7061 7468  ssingr......path
-00002230: 6c69 6272 0500 0000 da05 6e75 6d70 7972  libr......numpyr
-00002240: 3800 0000 5a06 7061 6e64 6173 721d 0000  8...Z.pandasr...
-00002250: 005a 0973 7472 7563 746c 6f67 5a0d 7363  .Z.structlogZ.sc
-00002260: 6970 792e 7370 6563 6961 6c72 0600 0000  ipy.specialr....
-00002270: 5a0c 7465 7874 6469 7374 616e 6365 7207  Z.textdistancer.
-00002280: 0000 005a 1068 696c 6172 792e 6578 7065  ...Z.hilary.expe
-00002290: 6374 6d61 7872 0800 0000 da0c 6869 6c61  ctmaxr......hila
-000022a0: 7279 2e75 7469 6c73 7209 0000 0072 0a00  ry.utilsr....r..
-000022b0: 0000 720b 0000 005a 0a73 6574 5f6f 7074  ..r....Z.set_opt
-000022c0: 696f 6eda 0a67 6574 5f6c 6f67 6765 7272  ion..get_loggerr
-000022d0: 8000 0000 7251 0000 0072 0c00 0000 7226  ....rQ...r....r&
-000022e0: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-000022f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002300: 731e 0000 0004 020c 0208 010c 010c 010c  s...............
-00002310: 0208 0108 0108 010c 010c 020c 0114 020c  ................
-00002320: 020a 03                                  ...
+00001ab0: 0000 0006 0000 0003 0000 0173 4e01 0000  ...........sN...
+00001ac0: 7c01 5c02 7d02 7d03 7400 7c02 6401 1900  |.\.}.}.t.|.d...
+00001ad0: 8301 7d04 7c04 8801 6a01 6402 1900 6b04  ..}.|...j.d...k.
+00001ae0: 7338 7c04 8801 6a01 6401 1900 6b00 7338  s8|...j.d...k.s8
+00001af0: 7c04 6403 1600 726a 7402 6a03 7404 7c03  |.d...rjt.j.t.|.
+00001b00: 8301 6404 6602 7400 6405 8d02 7c04 1400  ..d.f.t.d...|...
+00001b10: 6406 1a00 7c03 6407 6408 6702 3c00 7c03  d...|.d.d.g.<.|.
+00001b20: 6407 6408 6702 1900 5300 7c03 6409 1900  d.d.g...S.|.d...
+00001b30: 7d05 7c03 640a 1900 7c04 1400 7d06 7402  }.|.d...|...}.t.
+00001b40: a005 7c04 640b 1700 a101 8900 8801 6a06  ..|.d.........j.
+00001b50: 6a07 8801 6a06 640c 1900 7c04 6b02 1900  j...j.d...|.k...
+00001b60: 6a08 6401 640b 7c04 6404 1700 8502 6602  j.d.d.|.d.....f.
+00001b70: 1900 7d07 7402 a009 8700 6601 640d 640e  ..}.t.....f.d.d.
+00001b80: 8408 7c06 4400 8301 a101 740a 8800 8301  ..|.D.....t.....
+00001b90: 1b00 6a0b 640b 640f 8d01 7d08 7c07 7c08  ..j.d.d...}.|.|.
+00001ba0: 1b00 7d09 7c08 8801 6a0c 6b00 6a0d 640b  ..}.|...j.k.j.d.
+00001bb0: 640f 8d01 7d0a 7402 a009 8701 6601 6410  d...}.t.....f.d.
+00001bc0: 640e 8408 740e 7c09 7c05 8302 4400 8301  d...t.|.|...D...
+00001bd0: a101 6a0d 640b 640f 8d01 640b 1800 7d0b  ..j.d.d...d...}.
+00001be0: 7402 6a0f 7c0b 7c0a 6702 6401 640f 8d02  t.j.|.|.g.d.d...
+00001bf0: 7d0b 7c0b 7c03 6407 3c00 7c0a 7c03 6408  }.|.|.d.<.|.|.d.
+00001c00: 3c00 7c03 6407 6408 6702 1900 5300 2911  <.|.d.d.g...S.).
+00001c10: 6102 0100 0041 7373 6967 6e20 7072 6563  a....Assign prec
+00001c20: 6973 6520 616e 6420 7365 6e73 6974 6976  ise and sensitiv
+00001c30: 6520 7468 7265 7368 6f6c 6473 2074 6f20  e thresholds to 
+00001c40: 6461 7461 6672 616d 6520 6772 6f75 7065  dataframe groupe
+00001c50: 6420 6279 206c 656e 6774 682e 0a0a 2020  d by length...  
+00001c60: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00001c70: 2020 2020 2020 2020 6172 6773 2074 7570          args tup
+00001c80: 6c65 5b74 7570 6c65 5b69 6e74 5d2c 7064  le[tuple[int],pd
+00001c90: 2e44 6174 6146 7261 6d65 5d3a 206c 656e  .DataFrame]: len
+00001ca0: 6774 682c 2064 6174 6166 7261 6d65 2067  gth, dataframe g
+00001cb0: 726f 7570 6564 2062 7920 6c65 6e67 7468  rouped by length
+00001cc0: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001cd0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00001ce0: 642e 4461 7461 4672 616d 653a 2050 7265  d.DataFrame: Pre
+00001cf0: 6369 7365 2061 6e64 2073 656e 7369 7469  cise and sensiti
+00001d00: 7665 2074 6872 6573 686f 6c64 732e 0a20  ve thresholds.. 
+00001d10: 2020 2020 2020 2072 0100 0000 7232 0000         r....r2..
+00001d20: 0072 0f00 0000 7231 0000 0029 01da 0564  .r....r1...)...d
+00001d30: 7479 7065 e905 0000 00da 1170 7265 6369  type.......preci
+00001d40: 7365 5f74 6872 6573 686f 6c64 da13 7365  se_threshold..se
+00001d50: 6e73 6974 6976 655f 7468 7265 7368 6f6c  nsitive_threshol
+00001d60: 6472 6900 0000 726a 0000 0072 1000 0000  dri...rj...r....
+00001d70: 7259 0000 0063 0100 0000 0000 0000 0000  rY...c..........
+00001d80: 0000 0200 0000 0600 0000 1300 0001 7320  ..............s 
+00001d90: 0000 0067 007c 005d 187d 017c 0188 0013  ...g.|.].}.|....
+00001da0: 0074 00a0 017c 010b 00a1 0114 0091 0271  .t...|.........q
+00001db0: 0453 0072 2600 0000 2902 7238 0000 00da  .S.r&...).r8....
+00001dc0: 0365 7870 2902 7249 0000 00da 026d 7529  .exp).rI.....mu)
+00001dd0: 0172 3300 0000 7226 0000 0072 2700 0000  .r3...r&...r'...
+00001de0: 724e 0000 0003 0100 00f3 0000 0000 7a3f  rN............z?
+00001df0: 4170 7269 6f72 692e 6173 7369 676e 5f70  Apriori.assign_p
+00001e00: 7265 6369 7365 5f73 656e 7369 7469 7665  recise_sensitive
+00001e10: 5f74 6872 6573 686f 6c64 732e 3c6c 6f63  _thresholds.<loc
+00001e20: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00001e30: 6700 0000 6301 0000 0000 0000 0000 0000  g...c...........
+00001e40: 0003 0000 0006 0000 0013 0000 0173 3000  .............s0.
+00001e50: 0000 6700 7c00 5d28 5c02 7d01 7d02 7c01  ..g.|.](\.}.}.|.
+00001e60: 7c02 6400 7c02 1800 1b00 6401 8800 6a00  |.d.|.....d...j.
+00001e70: 1800 1400 8800 6a00 1b00 6b00 9102 7104  ......j...k...q.
+00001e80: 5300 2902 6772 c45a 7c0a 00f0 3f72 1000  S.).gr.Z|...?r..
+00001e90: 0000 2901 7216 0000 0029 0372 4900 0000  ..).r....).rI...
+00001ea0: da01 705a 0372 686f a901 7225 0000 0072  ..pZ.rho..r%...r
+00001eb0: 2600 0000 7227 0000 0072 4e00 0000 0901  &...r'...rN.....
+00001ec0: 0000 7304 0000 0006 0206 ff29 1072 1100  ..s........).r..
+00001ed0: 0000 7214 0000 0072 3800 0000 da04 6f6e  ..r....r8.....on
+00001ee0: 6573 da03 6c65 6eda 0661 7261 6e67 6572  es..len..aranger
+00001ef0: 2200 0000 7262 0000 0072 3600 0000 da05  "...rb...r6.....
+00001f00: 6172 7261 7972 0600 0000 da06 6375 6d73  arrayr......cums
+00001f10: 756d 7217 0000 00da 0373 756d da03 7a69  umr......sum..zi
+00001f20: 7072 4700 0000 290c 7225 0000 0072 3000  prG...).r%...r0.
+00001f30: 0000 5a07 7475 706c 655f 6c5a 036c 6466  ..Z.tuple_lZ.ldf
+00001f40: 7259 0000 005a 0472 686f 735a 036d 7573  rY...Z.rhosZ.mus
+00001f50: 5a04 6364 6630 5a04 6364 6631 5a02 7073  Z.cdf0Z.cdf1Z.ps
+00001f60: 5a06 745f 7365 6e73 5a06 745f 7072 6563  Z.t_sensZ.t_prec
+00001f70: 7226 0000 0029 0272 3300 0000 7225 0000  r&...).r3...r%..
+00001f80: 0072 2700 0000 da23 6173 7369 676e 5f70  .r'....#assign_p
+00001f90: 7265 6369 7365 5f73 656e 7369 7469 7665  recise_sensitive
+00001fa0: 5f74 6872 6573 686f 6c64 73ea 0000 0073  _thresholds....s
+00001fb0: 3c00 0000 000b 0801 0c02 2402 1cff 0a03  <.........$.....
+00001fc0: 0c02 0801 0c01 0e01 2802 1eff 0202 02fe  ........(.......
+00001fd0: 0603 0801 1202 0401 0a02 08fe 04ff 0405  ................
+00001fe0: 02fb 0406 02fa 02ff 0209 1201 0801 0801  ................
+00001ff0: 7a2b 4170 7269 6f72 692e 6173 7369 676e  z+Apriori.assign
+00002000: 5f70 7265 6369 7365 5f73 656e 7369 7469  _precise_sensiti
+00002010: 7665 5f74 6872 6573 686f 6c64 7363 0100  ve_thresholdsc..
+00002020: 0000 0000 0000 0000 0000 0100 0000 0600  ................
+00002030: 0000 4300 0001 732e 0000 0074 007c 006a  ..C...s....t.|.j
+00002040: 01a0 0264 0167 01a1 017c 006a 037c 006a  ...d.g...|.j.|.j
+00002050: 047c 006a 0564 028d 047c 006a 0164 0364  .|.j.d...|.j.d.d
+00002060: 0467 023c 0064 0553 0029 067a 3541 7373  .g.<.d.S.).z5Ass
+00002070: 6967 6e20 7468 7265 7368 6f6c 6473 2075  ign thresholds u
+00002080: 7369 6e67 206e 756c 6c20 6469 7374 7269  sing null distri
+00002090: 6275 7469 6f6e 2066 726f 6d20 6d6f 6465  bution from mode
+000020a0: 6c2e 7243 0000 0072 4f00 0000 7270 0000  l.rC...rO...rp..
+000020b0: 0072 7100 0000 4e29 0672 0900 0000 7224  .rq...N).r....r$
+000020c0: 0000 0072 5000 0000 727e 0000 0072 1800  ...rP...r~...r..
+000020d0: 0000 721a 0000 0072 7600 0000 7226 0000  ..r....rv...r&..
+000020e0: 0072 2600 0000 7227 0000 00da 0e67 6574  .r&...r'.....get
+000020f0: 5f74 6872 6573 686f 6c64 7315 0100 0073  _thresholds....s
+00002100: 0c00 0000 0002 0201 0c01 0401 0401 04fc  ................
+00002110: 7a16 4170 7269 6f72 692e 6765 745f 7468  z.Apriori.get_th
+00002120: 7265 7368 6f6c 6473 2901 4e29 11da 085f  resholds).N)..._
+00002130: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00002140: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00002150: 5fda 075f 5f64 6f63 5f5f 7238 0000 0072  _..__doc__r8...r
+00002160: 7900 0000 da06 6173 7479 7065 7211 0000  y.....astyper...
+00002170: 0072 2800 0000 720a 0000 0072 4000 0000  .r(...r....r@...
+00002180: 7256 0000 0072 5700 0000 7265 0000 0072  rV...rW...re...r
+00002190: 6d00 0000 727e 0000 0072 7f00 0000 7226  m...r~...r....r&
+000021a0: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+000021b0: 0000 720c 0000 0018 0000 0073 2600 0000  ..r........s&...
+000021c0: 0801 0404 1201 0601 0201 0201 0201 0201  ................
+000021d0: 0201 02f7 1e2f 00ff 141c 0e11 1021 100e  ...../.......!..
+000021e0: 1025 0e20 102b 720c 0000 0029 1e72 8300  .%. .+r....).r..
+000021f0: 0000 da0a 5f5f 6675 7475 7265 5f5f 7202  ....__future__r.
+00002200: 0000 0072 1e00 0000 da09 6974 6572 746f  ...r......iterto
+00002210: 6f6c 7372 0300 0000 da0f 6d75 6c74 6970  olsr......multip
+00002220: 726f 6365 7373 696e 6772 0400 0000 da07  rocessingr......
+00002230: 7061 7468 6c69 6272 0500 0000 da05 6e75  pathlibr......nu
+00002240: 6d70 7972 3800 0000 5a06 7061 6e64 6173  mpyr8...Z.pandas
+00002250: 721d 0000 005a 0973 7472 7563 746c 6f67  r....Z.structlog
+00002260: 5a0d 7363 6970 792e 7370 6563 6961 6c72  Z.scipy.specialr
+00002270: 0600 0000 5a0c 7465 7874 6469 7374 616e  ....Z.textdistan
+00002280: 6365 7207 0000 005a 1068 696c 6172 792e  cer....Z.hilary.
+00002290: 6578 7065 6374 6d61 7872 0800 0000 da0c  expectmaxr......
+000022a0: 6869 6c61 7279 2e75 7469 6c73 7209 0000  hilary.utilsr...
+000022b0: 0072 0a00 0000 720b 0000 005a 0a73 6574  .r....r....Z.set
+000022c0: 5f6f 7074 696f 6eda 0a67 6574 5f6c 6f67  _option..get_log
+000022d0: 6765 7272 8000 0000 7251 0000 0072 0c00  gerr....rQ...r..
+000022e0: 0000 7226 0000 0072 2600 0000 7226 0000  ..r&...r&...r&..
+000022f0: 0072 2700 0000 da08 3c6d 6f64 756c 653e  .r'.....<module>
+00002300: 0100 0000 731e 0000 0004 020c 0208 010c  ....s...........
+00002310: 010c 010c 0208 0108 0108 010c 010c 020c  ................
+00002320: 0114 020c 020a 03                        .......
```

### Comparing `hilary-1.2.0/hilary/__pycache__/expectmax.cpython-39.pyc` & `hilary-1.2.1/hilary/__pycache__/expectmax.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar  5 19:59:22 2024 UTC, .py size: 3795 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9a79 e765 d30e 0000  a........y.e....
+00000000: 610d 0d0a 0000 0000 261d fb65 b30e 0000  a.......&..e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0173 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c07 6d08 5a08 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a09 6403 5300 2907 7a1e  ..d...Z.d.S.).z.
 00000070: 436f 6465 2074 6f20 6669 7420 7072 6576  Code to fit prev
@@ -208,48 +208,46 @@
 00000cf0: 7212 0000 0072 2400 0000 7203 0000 0029  r....r$...r....)
 00000d00: 0572 1700 0000 da01 7872 2100 0000 7226  .r......xr!...r&
 00000d10: 0000 0072 2700 0000 7218 0000 0072 1800  ...r'...r....r..
 00000d20: 0000 7219 0000 00da 0b64 6973 6372 6574  ..r......discret
 00000d30: 654d 6978 5d00 0000 730c 0000 0000 0208  eMix]...s.......
 00000d40: 010a 012e 010a 0230 ff7a 0e45 4d2e 6469  .......0.z.EM.di
 00000d50: 7363 7265 7465 4d69 7863 0200 0000 0000  screteMixc......
-00000d60: 0000 0000 0000 0900 0000 0500 0000 4300  ..............C.
-00000d70: 0001 7372 0000 007c 006a 0074 017c 006a  ..sr...|.j.t.|.j
+00000d60: 0000 0000 0000 0900 0000 0400 0000 4300  ..............C.
+00000d70: 0001 735e 0000 007c 006a 0074 017c 006a  ..s^...|.j.t.|.j
 00000d80: 0083 011b 007d 027c 00a0 027c 006a 037c  .....}.|...|.j.|
 00000d90: 01a1 027d 037c 006a 0364 017c 006a 0414  ...}.|.j.d.|.j..
-00000da0: 006b 007d 0474 05a0 067c 027c 0419 0064  .k.}.t...|.|...d
-00000db0: 0217 00a1 0174 05a0 067c 037c 0419 0064  .....t...|.|...d
-00000dc0: 0217 00a1 0102 007d 057d 067c 057c 0618  .......}.}.|.|..
-00000dd0: 0064 0313 00a0 01a1 007d 0774 05a0 077c  .d.......}.t...|
-00000de0: 07a1 017d 087c 0853 0029 047a 4545 7374  ...}.|.S.).zEEst
-00000df0: 696d 6174 6520 676f 6f64 6e65 7373 206f  imate goodness o
-00000e00: 6620 6669 740a 2020 2020 2020 2020 4279  f fit.        By
-00000e10: 2064 6566 6175 6c74 2072 6574 7572 6e73   default returns
-00000e20: 2072 6573 6361 6c65 6420 726f 6f74 204d   rescaled root M
-00000e30: 5345 679a 9999 9999 99c9 3fe9 0500 0000  SEg.......?.....
-00000e40: e902 0000 0029 0872 0c00 0000 722c 0000  .....).r....r,..
-00000e50: 0072 3500 0000 7214 0000 0072 0b00 0000  .r5...r....r....
-00000e60: 7212 0000 00da 036c 6f67 da04 7371 7274  r......log..sqrt
-00000e70: 2909 7217 0000 0072 2100 0000 da02 7931  ).r....r!.....y1
-00000e80: da02 7932 da04 6d61 736b 5a05 6c6f 6779  ..y2..maskZ.logy
-00000e90: 315a 056c 6f67 7932 5a03 6d73 655a 0572  1Z.logy2Z.mseZ.r
-00000ea0: 726d 7365 7218 0000 0072 1800 0000 7219  rmser....r....r.
-00000eb0: 0000 00da 0565 7272 6f72 6700 0000 730e  .....errorg...s.
-00000ec0: 0000 0000 0310 010e 0110 0126 0210 010a  ...........&....
-00000ed0: 017a 0845 4d2e 6572 726f 724e 2902 7205  .z.EM.errorN).r.
-00000ee0: 0000 0072 0600 0000 290b da08 5f5f 6e61  ...r....)...__na
-00000ef0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000f00: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000f10: 5f5f 646f 635f 5f72 1a00 0000 7215 0000  __doc__r....r...
-00000f20: 0072 2a00 0000 722f 0000 0072 3300 0000  .r*...r/...r3...
-00000f30: 7235 0000 0072 3d00 0000 7218 0000 0072  r5...r=...r....r
-00000f40: 1800 0000 7218 0000 0072 1900 0000 7204  ....r....r....r.
-00000f50: 0000 000c 0000 0073 1400 0000 0801 0407  .......s........
-00000f60: 0001 00fa 1819 0e09 1010 100f 0e0d 080a  ................
-00000f70: 7204 0000 0029 0a72 4100 0000 da0a 5f5f  r....).rA.....__
-00000f80: 6675 7475 7265 5f5f 7202 0000 00da 056e  future__r......n
-00000f90: 756d 7079 7212 0000 00da 0670 616e 6461  umpyr......panda
-00000fa0: 73da 0270 64da 0d73 6369 7079 2e73 7065  s..pd..scipy.spe
-00000fb0: 6369 616c 7203 0000 0072 0400 0000 7218  cialr....r....r.
-00000fc0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000fd0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000fe0: 730a 0000 0004 020c 0208 0108 010c 05    s..............
+00000da0: 006b 007d 047c 027c 0419 007c 037c 0419  .k.}.|.|...|.|..
+00000db0: 0002 007d 057d 067c 057c 0618 0064 0213  ...}.}.|.|...d..
+00000dc0: 00a0 01a1 007d 0774 05a0 067c 07a1 017d  .....}.t...|...}
+00000dd0: 087c 0853 0029 037a 4545 7374 696d 6174  .|.S.).zEEstimat
+00000de0: 6520 676f 6f64 6e65 7373 206f 6620 6669  e goodness of fi
+00000df0: 740a 2020 2020 2020 2020 4279 2064 6566  t.        By def
+00000e00: 6175 6c74 2072 6574 7572 6e73 2072 6573  ault returns res
+00000e10: 6361 6c65 6420 726f 6f74 204d 5345 679a  caled root MSEg.
+00000e20: 9999 9999 99c9 3fe9 0200 0000 2907 720c  ......?.....).r.
+00000e30: 0000 0072 2c00 0000 7235 0000 0072 1400  ...r,...r5...r..
+00000e40: 0000 720b 0000 0072 1200 0000 da04 7371  ..r....r......sq
+00000e50: 7274 2909 7217 0000 0072 2100 0000 da02  rt).r....r!.....
+00000e60: 7931 da02 7932 da04 6d61 736b 5a03 7931  y1..y2..maskZ.y1
+00000e70: 6d5a 0379 326d 5a03 6d73 655a 0572 726d  mZ.y2mZ.mseZ.rrm
+00000e80: 7365 7218 0000 0072 1800 0000 7219 0000  ser....r....r...
+00000e90: 00da 0565 7272 6f72 6700 0000 730e 0000  ...errorg...s...
+00000ea0: 0000 0310 010e 0110 0112 0210 010a 017a  ...............z
+00000eb0: 0845 4d2e 6572 726f 724e 2902 7205 0000  .EM.errorN).r...
+00000ec0: 0072 0600 0000 290b da08 5f5f 6e61 6d65  .r....)...__name
+00000ed0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000ee0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000ef0: 646f 635f 5f72 1a00 0000 7215 0000 0072  doc__r....r....r
+00000f00: 2a00 0000 722f 0000 0072 3300 0000 7235  *...r/...r3...r5
+00000f10: 0000 0072 3b00 0000 7218 0000 0072 1800  ...r;...r....r..
+00000f20: 0000 7218 0000 0072 1900 0000 7204 0000  ..r....r....r...
+00000f30: 000c 0000 0073 1400 0000 0801 0407 0001  .....s..........
+00000f40: 00fa 1819 0e09 1010 100f 0e0d 080a 7204  ..............r.
+00000f50: 0000 0029 0a72 3f00 0000 da0a 5f5f 6675  ...).r?.....__fu
+00000f60: 7475 7265 5f5f 7202 0000 00da 056e 756d  ture__r......num
+00000f70: 7079 7212 0000 00da 0670 616e 6461 73da  pyr......pandas.
+00000f80: 0270 64da 0d73 6369 7079 2e73 7065 6369  .pd..scipy.speci
+00000f90: 616c 7203 0000 0072 0400 0000 7218 0000  alr....r....r...
+00000fa0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000fb0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000fc0: 0000 0004 020c 0208 0108 010c 05         .............
```

### Comparing `hilary-1.2.0/hilary/__pycache__/inference.cpython-39.pyc` & `hilary-1.2.1/hilary/__pycache__/inference.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar  5 23:26:49 2024 UTC, .py size: 19914 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,1006 +1,1009 @@
-00000000: 610d 0d0a 0000 0000 39aa e765 ca4d 0000  a.......9..e.M..
+00000000: 610d 0d0a 0000 0000 692a fc65 2e4e 0000  a.......i*.e.N..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0173 c600 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0173 d200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 5a0a 6401 6405 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6406 6c0c 6d0d 5a0e 0100 6401 6407 6c0f  d.l.m.Z...d.d.l.
 00000080: 6d10 5a10 6d11 5a11 0100 6401 6408 6c12  m.Z.m.Z...d.d.l.
 00000090: 6d13 5a13 0100 6401 6409 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
-000000a0: 0100 6401 640a 6c16 6d17 5a17 0100 6401  ..d.d.l.m.Z...d.
-000000b0: 640b 6c18 6d19 5a19 6d1a 5a1a 0100 650b  d.l.m.Z.m.Z...e.
-000000c0: a01b a100 5a1c 4700 640c 640d 8400 640d  ....Z.G.d.d...d.
-000000d0: 8302 5a1d 4700 640e 640f 8400 640f 8302  ..Z.G.d.d...d...
-000000e0: 5a1e 4700 6410 6411 8400 6411 8302 5a1f  Z.G.d.d...d...Z.
-000000f0: 6405 5300 2912 7a16 496e 6665 7220 636c  d.S.).z.Infer cl
-00000100: 6f6e 616c 2066 616d 696c 6965 732e e900  onal families...
-00000110: 0000 0029 01da 0b61 6e6e 6f74 6174 696f  ...)...annotatio
-00000120: 6e73 2901 da0c 636f 6d62 696e 6174 696f  ns)...combinatio
-00000130: 6e73 2901 da04 506f 6f6c 4e29 01da 0854  ns)...PoolN)...T
-00000140: 7269 654e 7563 6c29 02da 0866 636c 7573  rieNucl)...fclus
-00000150: 7465 72da 076c 696e 6b61 6765 2901 da0a  ter..linkage)...
-00000160: 7371 7561 7265 666f 726d 2901 da07 6861  squareform)...ha
-00000170: 6d6d 696e 6729 01da 0741 7072 696f 7269  mming)...Apriori
-00000180: 2902 da0d 6170 706c 7950 6172 616c 6c65  )...applyParalle
-00000190: 6cda 0970 5265 7175 6972 6564 6300 0000  l..pRequiredc...
-000001a0: 0000 0000 0000 0000 0000 0000 0006 0000  ................
-000001b0: 0040 0000 0173 5200 0000 6500 5a01 6400  .@...sR...e.Z.d.
-000001c0: 5a02 6401 5a03 6416 6403 6404 6405 6406  Z.d.Z.d.d.d.d.d.
-000001d0: 9c03 6407 6408 8405 5a04 6409 640a 640b  ..d.d...Z.d.d.d.
-000001e0: 9c02 640c 640d 8404 5a05 6700 640e a201  ..d.d...Z.g.d...
-000001f0: 640f 6602 6403 6410 6411 640a 6412 9c04  d.f.d.d.d.d.d...
-00000200: 6413 6414 8405 5a06 6415 5300 2917 da0e  d.d...Z.d.S.)...
-00000210: 4344 5233 436c 7573 7465 7269 6e67 7a4a  CDR3ClusteringzJ
-00000220: 496e 6665 7220 6661 6d69 6c69 6573 2075  Infer families u
-00000230: 7369 6e67 2043 4452 3320 6c65 6e67 7468  sing CDR3 length
-00000240: 2061 6e64 2074 6872 6573 686f 6c64 7320   and thresholds 
-00000250: 636f 6d70 7574 6564 2062 7920 4170 7269  computed by Apri
-00000260: 6f72 6920 636c 6173 732e e901 0000 00fa  ori class.......
-00000270: 0c70 642e 4461 7461 4672 616d 65da 0369  .pd.DataFrame..i
-00000280: 6e74 da04 4e6f 6e65 2903 da0a 7468 7265  nt..None)...thre
-00000290: 7368 6f6c 6473 da07 7468 7265 6164 73da  sholds..threads.
-000002a0: 0672 6574 7572 6e63 0300 0000 0000 0000  .returnc........
-000002b0: 0000 0000 0300 0000 0200 0000 4300 0001  ............C...
-000002c0: 7310 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
-000002d0: 0164 0153 0029 027a e449 6e69 7469 616c  .d.S.).z.Initial
-000002e0: 697a 6520 7468 7265 7368 6f6c 6473 2e0a  ize thresholds..
-000002f0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00000300: 2020 2020 2020 2020 2020 2074 6872 6573             thres
-00000310: 686f 6c64 7320 7064 2e44 6174 6146 7261  holds pd.DataFra
-00000320: 6d65 3a20 4461 7461 6672 616d 6520 636f  me: Dataframe co
-00000330: 6e74 6169 6e69 6e67 2074 6872 6573 686f  ntaining thresho
-00000340: 6c64 7320 666f 7220 6561 6368 2028 562c  lds for each (V,
-00000350: 4a2c 6c29 2063 6c61 7373 2e0a 2020 2020  J,l) class..    
-00000360: 2020 2020 2020 2020 7468 7265 6164 7320          threads 
-00000370: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-00000380: 204e 756d 6265 7220 6f66 2063 7075 7320   Number of cpus 
-00000390: 6f6e 2077 6869 6368 2074 6f20 7275 6e20  on which to run 
-000003a0: 636f 6465 2c20 6465 6661 756c 7473 2074  code, defaults t
-000003b0: 6f20 312e 0a20 2020 2020 2020 204e 2902  o 1..        N).
-000003c0: 7212 0000 0072 1300 0000 2903 da04 7365  r....r....)...se
-000003d0: 6c66 7212 0000 0072 1300 0000 a900 7216  lfr....r......r.
-000003e0: 0000 00fa 302f 686f 6d65 2f67 6174 6865  ....0/home/gathe
-000003f0: 6e65 732f 6769 746c 6162 2f48 494c 4152  nes/gitlab/HILAR
-00000400: 792f 6869 6c61 7279 2f69 6e66 6572 656e  y/hilary/inferen
-00000410: 6365 2e70 79da 085f 5f69 6e69 745f 5f1b  ce.py..__init__.
-00000420: 0000 0073 0400 0000 0007 0601 7a17 4344  ...s........z.CD
-00000430: 5233 436c 7573 7465 7269 6e67 2e5f 5f69  R3Clustering.__i
-00000440: 6e69 745f 5f7a 2974 7570 6c65 5b74 7570  nit__z)tuple[tup
-00000450: 6c65 5b73 7472 2c20 7374 722c 2069 6e74  le[str, str, int
-00000460: 5d2c 2070 642e 4461 7461 4672 616d 655d  ], pd.DataFrame]
-00000470: fa09 7064 2e53 6572 6965 73a9 02da 0461  ..pd.Series....a
-00000480: 7267 7372 1400 0000 6302 0000 0000 0000  rgsr....c.......
-00000490: 0000 0000 000a 0000 0004 0000 0043 0000  .............C..
-000004a0: 0173 8c00 0000 7c01 5c02 5c03 7d02 7d03  .s....|.\.\.}.}.
-000004b0: 7d04 7d05 7400 8300 7d06 7c05 6401 1900  }.}.t...}.|.d...
-000004c0: 4400 5d0e 7d07 7c06 a001 7c07 a101 0100  D.].}.|...|.....
-000004d0: 711c 7c00 6a02 6a03 7c00 6a02 6a04 7c02  q.|.j.j.|.j.j.|.
-000004e0: 6b02 7c00 6a02 6a05 7c03 6b02 4000 7c00  k.|.j.j.|.k.@.|.
-000004f0: 6a02 6a06 7c04 6b02 4000 1900 6a07 6402  j.j.|.k.@...j.d.
-00000500: 1900 6403 1900 7d08 7c08 6402 6b05 7282  ..d...}.|.d.k.r.
-00000510: 7c06 a008 7c08 a101 7d09 7c05 6401 1900  |...|...}.|.d...
-00000520: a009 7c09 a101 5300 7c05 6a0a a00b a100  ..|...S.|.j.....
-00000530: 5300 2904 6131 0100 0052 6574 7572 6e20  S.).a1...Return 
-00000540: 636c 7573 7465 7220 6c61 6265 6c73 2064  cluster labels d
-00000550: 6570 656e 6469 6e67 206f 6620 7468 7265  epending of thre
-00000560: 7368 6f6c 6473 2069 6e20 7365 6c66 2e74  sholds in self.t
-00000570: 6872 6573 686f 6c64 732e 0a0a 2020 2020  hresholds...    
-00000580: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000590: 2020 2020 2020 6172 6773 2028 5475 706c        args (Tupl
-000005a0: 655b 5475 706c 655b 7374 722c 2073 7472  e[Tuple[str, str
-000005b0: 2c20 696e 745d 2c20 7064 2e44 6174 6146  , int], pd.DataF
-000005c0: 7261 6d65 5d29 3a20 2856 6765 6e65 2c4a  rame]): (Vgene,J
-000005d0: 6765 6e65 2c6c 292c 2044 6174 6166 7261  gene,l), Datafra
-000005e0: 6d65 0a20 2020 2020 2020 2020 2020 206f  me.            o
-000005f0: 6620 7365 7175 656e 6365 7320 6772 6f75  f sequences grou
-00000600: 7065 6420 6279 2056 2c4a 2c6c 2063 6c61  ped by V,J,l cla
-00000610: 7373 2e0a 0a20 2020 2020 2020 2052 6574  ss...        Ret
-00000620: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00000630: 2020 7064 2e53 6572 6965 733a 2043 6c75    pd.Series: Clu
-00000640: 7374 6572 206c 6162 656c 7320 666f 7220  ster labels for 
-00000650: 7468 6973 2056 2c4a 2c6c 2063 6c61 7373  this V,J,l class
-00000660: 2e0a 2020 2020 2020 2020 da04 6364 7233  ..        ..cdr3
-00000670: 7201 0000 00e9 ffff ffff 290c da04 5472  r.........)...Tr
-00000680: 6965 da06 696e 7365 7274 7212 0000 00da  ie..insertr.....
-00000690: 036c 6f63 da06 765f 6765 6e65 da06 6a5f  .loc..v_gene..j_
-000006a0: 6765 6e65 da0b 6364 7233 5f6c 656e 6774  gene..cdr3_lengt
-000006b0: 68da 0676 616c 7565 73da 0863 6c75 7374  h..values..clust
-000006c0: 6572 73da 036d 6170 da05 696e 6465 78da  ers..map..index.
-000006d0: 0874 6f5f 6672 616d 6529 0a72 1500 0000  .to_frame).r....
-000006e0: 721b 0000 00da 0176 da01 6ada 016c da02  r......v..j..l..
-000006f0: 6466 5a04 7472 6965 721c 0000 00da 0174  dfZ.trier......t
-00000700: da03 6463 7472 1600 0000 7216 0000 0072  ..dctr....r....r
-00000710: 1700 0000 da07 636c 7573 7465 7225 0000  ......cluster%..
-00000720: 0073 2600 0000 000a 0e01 0601 0c01 0c01  .s&.............
-00000730: 0601 0a01 0aff 0202 0afe 02ff 0404 02fc  ................
-00000740: 0204 02fc 0405 0801 0a01 0e01 7a16 4344  ............z.CD
-00000750: 5233 436c 7573 7465 7269 6e67 2e63 6c75  R3Clustering.clu
-00000760: 7374 6572 a903 7221 0000 0072 2200 0000  ster..r!...r"...
-00000770: 7223 0000 0046 7a09 6c69 7374 5b73 7472  r#...Fz.list[str
-00000780: 5dda 0462 6f6f 6c29 0472 2c00 0000 da05  ]..bool).r,.....
-00000790: 6772 6f75 70da 0673 696c 656e 7472 1400  group..silentr..
-000007a0: 0000 6304 0000 0000 0000 0000 0000 0005  ..c.............
-000007b0: 0000 0006 0000 0043 0000 0173 4800 0000  .......C...sH...
-000007c0: 7c02 6401 6701 1700 7d04 7400 7c01 7c04  |.d.g...}.t.|.|.
-000007d0: 1900 a001 7c02 a101 7c00 6a02 7c03 7c00  ....|...|.j.|.|.
-000007e0: 6a03 6402 8d04 7c01 6403 3c00 7c02 6403  j.d...|.d.<.|.d.
-000007f0: 6701 1700 7d02 7c01 a001 7c02 a101 a004  g...}.|...|.....
-00000800: a100 6404 1700 5300 2905 6107 0200 0052  ..d...S.).a....R
-00000810: 6574 7572 6e20 636c 7573 7465 7220 6c61  eturn cluster la
-00000820: 6265 6c73 2064 6570 656e 6469 6e67 206f  bels depending o
-00000830: 6620 7468 7265 7368 6f6c 6473 2069 6e20  f thresholds in 
-00000840: 7365 6c66 2e74 6872 6573 686f 6c64 732e  self.thresholds.
-00000850: 0a0a 2020 2020 2020 2020 5275 6e73 2073  ..        Runs s
-00000860: 656c 662e 636c 7573 7465 7220 7061 7261  elf.cluster para
-00000870: 6c6c 656c 7920 6f6e 2064 6174 6166 7261  llely on datafra
-00000880: 6d65 2067 726f 7570 6564 2062 7920 2767  me grouped by 'g
-00000890: 726f 7570 2720 6172 6775 6d65 6e74 2e0a  roup' argument..
-000008a0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000008b0: 2020 2020 2020 2020 2020 2064 6620 2870             df (p
-000008c0: 642e 4461 7461 4672 616d 6529 3a20 4461  d.DataFrame): Da
-000008d0: 7461 6672 616d 6520 6f66 2073 6571 7565  taframe of seque
-000008e0: 6e63 6573 2e0a 2020 2020 2020 2020 2020  nces..          
-000008f0: 2020 6772 6f75 7020 286c 6973 745b 7374    group (list[st
-00000900: 725d 2c20 6f70 7469 6f6e 616c 293a 2047  r], optional): G
-00000910: 726f 7570 7320 6f6e 2077 6869 6368 2074  roups on which t
-00000920: 6f20 646f 2070 6172 616c 6c65 6c20 696e  o do parallel in
-00000930: 6665 7272 696e 6720 6f66 2063 6c75 7374  ferring of clust
-00000940: 6572 732e 0a20 2020 2020 2020 2020 2020  ers..           
-00000950: 2044 6566 6175 6c74 7320 746f 205b 2276   Defaults to ["v
-00000960: 5f67 656e 6522 2c20 226a 5f67 656e 6522  _gene", "j_gene"
-00000970: 2c20 2263 6472 335f 6c65 6e67 7468 225d  , "cdr3_length"]
-00000980: 2e0a 2020 2020 2020 2020 2020 2020 7369  ..            si
-00000990: 6c65 6e74 2028 626f 6f6c 2c6f 7074 696f  lent (bool,optio
-000009a0: 6e61 6c29 203a 2044 6f20 6e6f 7420 7368  nal) : Do not sh
-000009b0: 6f77 2070 726f 6772 6573 7320 6261 7220  ow progress bar 
-000009c0: 6966 2054 7275 652e 0a0a 2020 2020 2020  if True...      
-000009d0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000009e0: 2020 2020 2020 2070 642e 5365 7269 6573         pd.Series
-000009f0: 3a20 5365 7269 6573 2077 6974 6820 636c  : Series with cl
-00000a00: 7573 7465 7220 6c61 6265 6c73 2e0a 2020  uster labels..  
-00000a10: 2020 2020 2020 721c 0000 00a9 0272 3300        r......r3.
-00000a20: 0000 da08 6370 7543 6f75 6e74 722f 0000  ....cpuCountr/..
-00000a30: 0072 0e00 0000 2905 720b 0000 00da 0767  .r....).r......g
-00000a40: 726f 7570 6279 722f 0000 0072 1300 0000  roupbyr/...r....
-00000a50: da06 6e67 726f 7570 2905 7215 0000 0072  ..ngroup).r....r
-00000a60: 2c00 0000 7232 0000 0072 3300 0000 da03  ,...r2...r3.....
-00000a70: 7573 6572 1600 0000 7216 0000 0072 1700  user....r....r..
-00000a80: 0000 da05 696e 6665 723d 0000 0073 1200  ....infer=...s..
-00000a90: 0000 0013 0a01 0201 0c01 0401 0201 04fc  ................
-00000aa0: 0a06 0a01 7a14 4344 5233 436c 7573 7465  ....z.CDR3Cluste
-00000ab0: 7269 6e67 2e69 6e66 6572 4e29 0172 0e00  ring.inferN).r..
-00000ac0: 0000 2907 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00000ad0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000ae0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000af0: 5f72 1800 0000 722f 0000 0072 3900 0000  _r....r/...r9...
-00000b00: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000b10: 1700 0000 720d 0000 0018 0000 0073 0c00  ....r........s..
-00000b20: 0000 0801 0402 140a 101b 0601 02fc 720d  ..............r.
-00000b30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000b40: 0000 0000 0700 0000 4000 0001 7358 0000  ........@...sX..
-00000b50: 0065 005a 0164 005a 0264 015a 0364 1764  .e.Z.d.Z.d.Z.d.d
-00000b60: 0364 0364 0464 0364 0564 069c 0564 0764  .d.d.d.d.d...d.d
-00000b70: 0884 055a 0464 0964 0964 0a64 0b9c 0364  ...Z.d.d.d.d...d
-00000b80: 0c64 0d84 045a 0564 0364 0e64 0f9c 0264  .d...Z.d.d.d...d
-00000b90: 1064 1184 045a 0664 1264 139c 0164 1464  .d...Z.d.d...d.d
-00000ba0: 1584 045a 0764 1653 0029 18da 0e44 6973  ...Z.d.S.)...Dis
-00000bb0: 7461 6e63 654d 6174 7269 787a 4e4f 626a  tanceMatrixzNObj
-00000bc0: 6563 7420 656e 6162 6c69 6e67 2070 6172  ect enabling par
-00000bd0: 616c 6c65 6c20 636f 6d70 7574 696e 6720  allel computing 
-00000be0: 6f66 2074 6865 2064 6973 7461 6e63 6520  of the distance 
-00000bf0: 6d61 7274 7269 7820 6f66 2061 206c 6172  martrix of a lar
-00000c00: 6765 2063 6c75 7374 6572 2e72 0e00 0000  ge cluster.r....
-00000c10: 7210 0000 0072 0f00 0000 7211 0000 0029  r....r....r....)
-00000c20: 0572 2b00 0000 da10 616c 6967 6e6d 656e  .r+.....alignmen
-00000c30: 745f 6c65 6e67 7468 722c 0000 0072 1300  t_lengthr,...r..
-00000c40: 0000 7214 0000 0063 0500 0000 0000 0000  ..r....c........
-00000c50: 0000 0000 0500 0000 0300 0000 4300 0001  ............C...
-00000c60: 737a 0000 007c 047c 005f 007c 017c 005f  sz...|.|._.|.|._
-00000c70: 017c 027c 005f 027c 017c 006a 021b 007c  .|.|._.|.|.j...|
-00000c80: 005f 037c 017c 006a 0217 007c 006a 021b  ._.|.|.j...|.j..
-00000c90: 007c 005f 047c 036a 057c 005f 067c 006a  .|._.|.j.|._.|.j
-00000ca0: 066a 0764 0119 007c 005f 087c 006a 087c  .j.d...|._.|.j.|
-00000cb0: 006a 0864 0218 0014 0064 031a 007c 005f  .j.d.....d...|._
-00000cc0: 0974 0a7c 006a 0864 0313 0064 031a 0064  .t.|.j.d...d...d
-00000cd0: 041a 0064 0583 027c 005f 0b64 0653 0029  ...d...|._.d.S.)
-00000ce0: 0761 4001 0000 496e 6974 6961 6c69 7a65  .a@...Initialize
-00000cf0: 2061 7474 7269 6275 7465 732e 0a0a 2020   attributes...  
-00000d00: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00000d10: 2020 2020 2020 2020 6c20 2869 6e74 293a          l (int):
-00000d20: 2043 4452 3320 6c65 6e67 7468 0a20 2020   CDR3 length.   
-00000d30: 2020 2020 2020 2020 2061 6c69 676e 5f6c           align_l
-00000d40: 656e 6774 6820 2869 6e74 293a 204c 656e  ength (int): Len
-00000d50: 6774 6820 6f66 2074 6865 2056 6765 6e65  gth of the Vgene
-00000d60: 202b 204a 6765 6e65 2e0a 2020 2020 2020   + Jgene..      
-00000d70: 2020 2020 2020 6466 2028 7064 2e44 6174        df (pd.Dat
-00000d80: 6146 7261 6d65 293a 2044 6174 6166 7261  aFrame): Datafra
-00000d90: 6d65 206f 6620 7365 7175 656e 6365 7320  me of sequences 
-00000da0: 6772 6f75 7065 6420 6279 2028 762c 6a2c  grouped by (v,j,
-00000db0: 6c2c 7365 6e73 6974 6976 6520 636c 7573  l,sensitive clus
-00000dc0: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
-00000dd0: 2074 6872 6561 6473 2028 696e 742c 206f   threads (int, o
-00000de0: 7074 696f 6e61 6c29 3a20 4e75 6d62 6572  ptional): Number
-00000df0: 206f 6620 6370 7573 206f 6e20 7768 6963   of cpus on whic
-00000e00: 6820 746f 2072 756e 2063 6f64 652e 2044  h to run code. D
-00000e10: 6566 6175 6c74 7320 746f 2031 2e0a 2020  efaults to 1..  
-00000e20: 2020 2020 2020 7201 0000 0072 0e00 0000        r....r....
-00000e30: e902 0000 00e9 f401 0000 e903 0000 004e  ...............N
-00000e40: 290c 7213 0000 0072 2b00 0000 da01 4cda  ).r....r+.....L.
-00000e50: 036c 5f4c da05 6c5f 4c5f 4c72 2400 0000  .l_L..l_L_Lr$...
-00000e60: da04 6461 7461 da05 7368 6170 65da 016e  ..data..shape..n
-00000e70: da05 6b5f 6d61 78da 036d 6178 da06 6b5f  ..k_max..max..k_
-00000e80: 7374 6570 2905 7215 0000 0072 2b00 0000  step).r....r+...
-00000e90: 723f 0000 0072 2c00 0000 7213 0000 0072  r?...r,...r....r
-00000ea0: 1600 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000eb0: 0000 005e 0000 0073 1200 0000 000f 0601  ...^...s........
-00000ec0: 0601 0601 0c01 1201 0801 0e02 1601 7a17  ..............z.
-00000ed0: 4469 7374 616e 6365 4d61 7472 6978 2e5f  DistanceMatrix._
-00000ee0: 5f69 6e69 745f 5f7a 1974 7570 6c65 5b73  _init__z.tuple[s
-00000ef0: 7472 2c20 7374 722c 2069 6e74 2c20 696e  tr, str, int, in
-00000f00: 745d da05 666c 6f61 7429 03da 0461 7267  t]..float)...arg
-00000f10: 31da 0461 7267 3272 1400 0000 6303 0000  1..arg2r....c...
-00000f20: 0000 0000 0000 0000 0014 0000 0004 0000  ................
-00000f30: 0043 0000 0173 b000 0000 7c01 5c04 7d03  .C...s....|.\.}.
-00000f40: 7d04 7d05 7d06 7c02 5c04 7d07 7d08 7d09  }.}.}.|.\.}.}.}.
-00000f50: 7d0a 7c06 7c0a 6b02 7228 7c00 6a00 0b00  }.|.|.k.r(|.j...
-00000f60: 5300 7c05 7c09 1400 7336 7c00 6a00 5300  S.|.|...s6|.j.S.
-00000f70: 7401 7c03 7c07 8302 7d0b 7401 7c04 7c08  t.|.|...}.t.|.|.
-00000f80: 8302 7d0c 7c05 7c09 1700 7c0c 1800 6401  ..}.|.|...|...d.
-00000f90: 1b00 7d0d 7c00 6a02 7c0c 6402 1700 1400  ..}.|.j.|.d.....
-00000fa0: 7d0e 7403 a004 7c0e 7c00 6a05 1400 a101  }.t...|.|.j.....
-00000fb0: 7d0f 7c05 7c09 1400 7c00 6a00 1b00 7d10  }.|.|...|.j...}.
-00000fc0: 7403 a004 7c10 a101 7d11 7c0b 7c0e 1800  t...|...}.|.|...
-00000fd0: 7c0f 1b00 7d12 7c0d 7c10 1800 7c11 1b00  |...}.|.|...|...
-00000fe0: 7d13 7c12 7c13 1800 5300 2903 618e 0100  }.|.|...S.).a...
-00000ff0: 0043 6f6d 7075 7465 2064 6966 6665 7265  .Compute differe
-00001000: 6e63 6520 6274 7765 656e 206e 6f72 6d61  nce btween norma
-00001010: 6c69 7a65 6420 6364 7233 2064 6976 6572  lized cdr3 diver
-00001020: 6765 6e63 6520 2620 7368 6172 6564 206d  gence & shared m
-00001030: 7574 6174 696f 6e73 206f 6620 7477 6f20  utations of two 
-00001040: 7365 7175 656e 6365 732e 0a0a 2020 2020  sequences...    
-00001050: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00001060: 2020 2020 2020 6172 6731 2028 5475 706c        arg1 (Tupl
-00001070: 655b 7374 722c 7374 722c 696e 742c 696e  e[str,str,int,in
-00001080: 745d 293a 2028 4344 5233 206c 656e 6774  t]): (CDR3 lengt
-00001090: 682c 2056 2b4a 2073 6571 7565 6e63 6520  h, V+J sequence 
-000010a0: 616c 6967 6e6d 656e 742c 206e 756d 6265  alignment, numbe
-000010b0: 7220 6f66 206d 7574 6174 696f 6e73 0a20  r of mutations. 
-000010c0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-000010d0: 6765 726d 6c69 6e65 2c20 696e 6465 7829  germline, index)
-000010e0: 2066 6f72 2073 6571 7565 6e63 6520 310a   for sequence 1.
-000010f0: 2020 2020 2020 2020 2020 2020 6172 6732              arg2
-00001100: 2028 5475 706c 655b 7374 722c 7374 722c   (Tuple[str,str,
-00001110: 696e 742c 696e 745d 293a 2053 616d 6520  int,int]): Same 
-00001120: 666f 7220 7365 7175 656e 6365 2032 0a0a  for sequence 2..
-00001130: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00001140: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
-00001150: 6174 3a20 4469 6666 6572 656e 6365 2062  at: Difference b
-00001160: 6574 7765 656e 2074 776f 2071 7561 6e74  etween two quant
-00001170: 6974 6965 732e 0a20 2020 2020 2020 2072  ities..        r
-00001180: 4000 0000 720e 0000 0029 0672 4300 0000  @...r....).rC...
-00001190: 7209 0000 0072 4400 0000 da02 6e70 da04  r....rD.....np..
-000011a0: 7371 7274 7245 0000 0029 1472 1500 0000  sqrtrE...).r....
-000011b0: 724d 0000 0072 4e00 0000 da05 6364 7233  rM...rN.....cdr3
-000011c0: 31da 0273 31da 026e 31da 0269 31da 0563  1..s1..n1..i1..c
-000011d0: 6472 3332 da02 7332 da02 6e32 da02 6932  dr32..s2..n2..i2
-000011e0: 7248 0000 00da 026e 4cda 026e 30da 0565  rH.....nL..n0..e
-000011f0: 7870 5f6e da05 7374 645f 6eda 0665 7870  xp_n..std_n..exp
-00001200: 5f6e 30da 0673 7464 5f6e 30da 0178 da01  _n0..std_n0..x..
-00001210: 7972 1600 0000 7216 0000 0072 1700 0000  yr....r....r....
-00001220: da06 6d65 7472 6963 7800 0000 7320 0000  ..metricx...s ..
-00001230: 0000 0f0c 010c 0108 0108 0108 0106 010a  ................
-00001240: 010a 0110 020e 0110 020e 010a 020c 010c  ................
-00001250: 017a 1544 6973 7461 6e63 654d 6174 7269  .z.DistanceMatri
-00001260: 782e 6d65 7472 6963 7a1c 7475 706c 655b  x.metricz.tuple[
-00001270: 696e 742c 2069 6e74 2c20 6c69 7374 5b66  int, int, list[f
-00001280: 6c6f 6174 5d5d 2902 da05 7374 6172 7472  loat]])...startr
-00001290: 1400 0000 6302 0000 0000 0000 0000 0000  ....c...........
-000012a0: 000b 0000 000a 0000 0043 0000 0173 ee00  .........C...s..
-000012b0: 0000 6700 7d02 7c01 7d03 7400 7c01 7c00  ..g.}.|.}.t.|.|.
-000012c0: 6a01 1700 7c00 6a02 8302 7d04 7403 7c03  j...|.j...}.t.|.
-000012d0: 7c04 8302 4400 5dbe 7d05 7404 7c00 6a05  |...D.].}.t.|.j.
-000012e0: 6401 1800 7404 7406 a007 6402 7c05 1400  d...t.t...d.|...
-000012f0: 6403 7c00 6a05 1400 7c00 6a05 6404 1800  d.|.j...|.j.d...
-00001300: 1400 1700 6405 1800 a101 6406 1b00 6407  ....d.....d...d.
-00001310: 1800 8301 1800 8301 7d06 7404 7c05 7c06  ........}.t.|.|.
-00001320: 1700 6404 1700 7c00 6a05 7c00 6a05 6404  ..d...|.j.|.j.d.
-00001330: 1800 1400 6401 1b00 1800 7c00 6a05 7c06  ....d.....|.j.|.
-00001340: 1800 7c00 6a05 7c06 1800 6404 1800 1400  ..|.j.|...d.....
-00001350: 6401 1b00 1700 8301 7d07 7c00 6a08 7c06  d.......}.|.j.|.
-00001360: 6408 6408 8502 6602 1900 7d08 7c00 6a08  d.d...f...}.|.j.
-00001370: 7c07 6408 6408 8502 6602 1900 7d09 7c00  |.d.d...f...}.|.
-00001380: a009 7c08 7c09 a102 7d0a 7c02 a00a 7c0a  ..|.|...}.|...|.
-00001390: a101 0100 7124 7c03 7c04 7c02 6603 5300  ....q$|.|.|.f.S.
-000013a0: 2909 610a 0100 0043 6f6d 7075 7465 2031  ).a....Compute 1
-000013b0: 4420 6469 7374 616e 6365 206d 6174 7269  D distance matri
-000013c0: 7820 6265 7477 6565 6e20 7374 6172 7420  x between start 
-000013d0: 616e 6420 7374 6172 742b 7365 6c66 2e6b  and start+self.k
-000013e0: 5f73 7465 702e 0a0a 2020 2020 2020 2020  _step...        
-000013f0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00001400: 2020 7374 6172 7420 2869 6e74 293a 2049    start (int): I
-00001410: 6e64 6578 2066 726f 6d20 7768 6963 6820  ndex from which 
-00001420: 746f 2063 6f6d 7075 7465 2064 6973 7461  to compute dista
-00001430: 6e63 6573 2e0a 0a20 2020 2020 2020 2052  nces...        R
-00001440: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00001450: 2020 2020 5475 706c 655b 696e 742c 2069      Tuple[int, i
-00001460: 6e74 2c20 6c69 7374 5b66 6c6f 6174 5d5d  nt, list[float]]
-00001470: 3a20 5374 6172 7420 696e 6465 782c 2045  : Start index, E
-00001480: 6e64 2069 6e64 6578 2c20 6469 7374 616e  nd index, distan
-00001490: 6365 2066 6f72 2069 6e64 6963 6573 2069  ce for indices i
-000014a0: 6e62 6574 7765 656e 0a20 2020 2020 2020  nbetween.       
-000014b0: 2072 4000 0000 69f8 ffff ffe9 0400 0000   r@...i.........
-000014c0: 720e 0000 00e9 0700 0000 6700 0000 0000  r.........g.....
-000014d0: 0000 4067 0000 0000 0000 e03f 4e29 0bda  ..@g.......?N)..
-000014e0: 036d 696e 724b 0000 0072 4900 0000 da05  .minrK...rI.....
-000014f0: 7261 6e67 6572 1000 0000 7248 0000 0072  ranger....rH...r
-00001500: 4f00 0000 7250 0000 0072 4600 0000 7261  O...rP...rF...ra
-00001510: 0000 00da 0661 7070 656e 6429 0b72 1500  .....append).r..
-00001520: 0000 7262 0000 00da 0464 6973 74da 026b  ..rb.....dist..k
-00001530: 31da 026b 32da 016b da01 6972 2a00 0000  1..k2..k..ir*...
-00001540: da01 61da 0162 da01 6472 1600 0000 7216  ..a..b..dr....r.
-00001550: 0000 0072 1700 0000 da04 7072 6f63 9b00  ...r......proc..
-00001560: 0000 7336 0000 0000 0904 0104 0112 010e  ..s6............
-00001570: 0202 0104 0102 ff02 0230 fe02 ff04 0502  .........0......
-00001580: 0102 0102 ff02 0202 fe02 0312 fd02 041a  ................
-00001590: fc02 ff04 0812 0112 010c 010c 017a 1344  .............z.D
-000015a0: 6973 7461 6e63 654d 6174 7269 782e 7072  istanceMatrix.pr
-000015b0: 6f63 fa0a 6e70 2e6e 6461 7272 6179 a901  oc..np.ndarray..
-000015c0: 7214 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000015d0: 0000 0600 0000 0800 0000 4300 0001 7372  ..........C...sr
-000015e0: 0000 0074 00a0 017c 006a 02a1 017d 0174  ...t...|.j...}.t
-000015f0: 037c 006a 0483 018f 427d 027c 02a0 057c  .|.j....B}.|...|
-00001600: 006a 0674 0764 017c 006a 027c 006a 0883  .j.t.d.|.j.|.j..
-00001610: 03a1 0244 005d 165c 037d 037d 047d 057c  ...D.].\.}.}.}.|
-00001620: 057c 017c 037c 0485 023c 0071 3257 0064  .|.|.|...<.q2W.d
-00001630: 0204 0004 0083 0301 006e 1031 0073 5e30  .........n.1.s^0
-00001640: 0001 0001 0001 0059 0001 007c 017c 006a  .......Y...|.|.j
-00001650: 0917 0053 0029 037a 7a52 756e 2073 656c  ...S.).zzRun sel
-00001660: 662e 7072 6f63 2070 6172 616c 6c65 6c79  f.proc parallely
-00001670: 2074 6f20 636f 6d70 7574 6520 3144 2064   to compute 1D d
-00001680: 6973 7461 6e63 6520 6d61 7472 6978 2e0a  istance matrix..
-00001690: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000016a0: 3a0a 2020 2020 2020 2020 2020 2020 6e70  :.            np
-000016b0: 2e61 7272 6179 3a20 3144 2064 6973 7461  .array: 1D dista
-000016c0: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
-000016d0: 2020 2072 0100 0000 4e29 0a72 4f00 0000     r....N).rO...
-000016e0: da05 7a65 726f 7372 4900 0000 7204 0000  ..zerosrI...r...
-000016f0: 0072 1300 0000 5a0e 696d 6170 5f75 6e6f  .r....Z.imap_uno
-00001700: 7264 6572 6564 7270 0000 0072 6600 0000  rderedrp...rf...
-00001710: 724b 0000 0072 4300 0000 2906 7215 0000  rK...rC...).r...
-00001720: 0072 6800 0000 da04 706f 6f6c 7269 0000  .rh.....poolri..
-00001730: 0072 6a00 0000 da03 7265 7372 1600 0000  .rj.....resr....
-00001740: 7216 0000 0072 1700 0000 da07 636f 6d70  r....r......comp
-00001750: 7574 65bc 0000 0073 1000 0000 0006 0c01  ute....s........
-00001760: 0c01 0401 0401 0efe 0e04 2c01 7a16 4469  ..........,.z.Di
-00001770: 7374 616e 6365 4d61 7472 6978 2e63 6f6d  stanceMatrix.com
-00001780: 7075 7465 4e29 0172 0e00 0000 2908 723a  puteN).r....).r:
-00001790: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
-000017a0: 0000 7218 0000 0072 6100 0000 7270 0000  ..r....ra...rp..
-000017b0: 0072 7600 0000 7216 0000 0072 1600 0000  .rv...r....r....
-000017c0: 7216 0000 0072 1700 0000 723e 0000 005b  r....r....r>...[
-000017d0: 0000 0073 0c00 0000 0801 0407 00fb 181a  ...s............
-000017e0: 1223 1021 723e 0000 0063 0000 0000 0000  .#.!r>...c......
-000017f0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-00001800: 0001 73ac 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00001810: 015a 0364 2c64 0364 0464 059c 0264 0664  .Z.d,d.d.d...d.d
-00001820: 0784 055a 0464 0864 0984 005a 0564 0a64  ...Z.d.d...Z.d.d
-00001830: 0b84 005a 0664 0c64 0c64 0d64 0e64 0f9c  ...Z.d.d.d.d.d..
-00001840: 0464 1064 1184 045a 0764 1264 1364 149c  .d.d...Z.d.d.d..
-00001850: 0264 1564 1684 045a 0864 1764 1764 189c  .d.d...Z.d.d.d..
-00001860: 0264 1964 1a84 045a 0964 2d64 1764 0d64  .d.d...Z.d-d.d.d
-00001870: 1d64 1764 1e9c 0464 1f64 2084 055a 0a64  .d.d...d.d ..Z.d
-00001880: 1764 1364 189c 0264 2164 2284 045a 0b64  .d.d...d!d"..Z.d
-00001890: 2e64 1d64 2464 259c 0264 2664 2784 055a  .d.d$d%..d&d'..Z
-000018a0: 0c64 1764 289c 0164 2964 2a84 045a 0d64  .d.d(..d)d*..Z.d
-000018b0: 2b53 0029 2fda 0648 494c 4152 797a 3349  +S.)/..HILARyz3I
-000018c0: 6e66 6572 2066 616d 696c 6965 7320 7573  nfer families us
-000018d0: 696e 6720 4344 5233 2061 6e64 206d 7574  ing CDR3 and mut
-000018e0: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
-000018f0: 6e2e 4672 0a00 0000 7231 0000 0029 02da  n.Fr....r1...)..
-00001900: 0761 7072 696f 7269 da05 6372 7564 6563  .apriori..crudec
-00001910: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-00001920: 0300 0000 4300 0001 7374 0000 0067 0064  ....C...st...g.d
-00001930: 01a2 017c 005f 007c 016a 017c 005f 0167  ...|._.|.j.|._.g
-00001940: 0064 02a2 017c 005f 0274 037c 0264 0319  .d...|._.t.|.d..
-00001950: 006a 0464 0419 0083 017c 005f 057c 0373  .j.d.....|._.|.s
-00001960: 507c 006a 01a0 0664 05a1 01a0 077c 006a  P|.j...d.....|.j
-00001970: 00a1 01a0 08a1 006a 097c 005f 0a7c 016a  .......j.|._.|.j
-00001980: 0b7c 005f 0b7c 016a 0c7c 005f 0c7c 016a  .|._.|.j.|._.|.j
-00001990: 0d7c 005f 0d7c 016a 0e7c 005f 0e64 0653  .|._.|.j.|._.d.S
-000019a0: 0029 077a e149 6e69 7469 616c 697a 6520  .).z.Initialize 
-000019b0: 4869 6c61 7279 2061 7474 7269 6275 7465  Hilary attribute
-000019c0: 7320 7573 696e 6720 4170 7269 6f72 6920  s using Apriori 
-000019d0: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
-000019e0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-000019f0: 2020 2061 7072 696f 7269 2028 4170 7269     apriori (Apri
-00001a00: 6f72 6929 3a20 4170 7269 6f72 6920 6f62  ori): Apriori ob
-00001a10: 6a65 6374 2063 6f6e 7461 696e 696e 6720  ject containing 
-00001a20: 6869 7374 6f67 7261 6d73 2061 6e64 2074  histograms and t
-00001a30: 6872 6573 686f 6c64 732e 0a20 2020 2020  hresholds..     
-00001a40: 2020 2020 2020 2078 795f 7468 7265 7368         xy_thresh
-00001a50: 6f6c 6420 2869 6e74 293a 5468 7265 7368  old (int):Thresh
-00001a60: 6f6c 6420 746f 2075 7365 2066 6f72 2074  old to use for t
-00001a70: 6865 2078 7920 6d65 7468 6f64 2e0a 2020  he xy method..  
-00001a80: 2020 2020 2020 7230 0000 0029 0472 1c00        r0...).r..
-00001a90: 0000 da16 616c 745f 7365 7175 656e 6365  ....alt_sequence
-00001aa0: 5f61 6c69 676e 6d65 6e74 da0e 6d75 7461  _alignment..muta
-00001ab0: 7469 6f6e 5f63 6f75 6e74 7227 0000 0072  tion_countr'...r
-00001ac0: 7a00 0000 7201 0000 007a 4f76 5f67 656e  z...r....zOv_gen
-00001ad0: 6520 213d 2027 4e6f 6e65 2720 616e 6420  e != 'None' and 
-00001ae0: 7072 6563 6973 655f 7468 7265 7368 6f6c  precise_threshol
-00001af0: 6420 3c20 7365 6e73 6974 6976 655f 7468  d < sensitive_th
-00001b00: 7265 7368 6f6c 6420 616e 6420 7061 6972  reshold and pair
-00001b10: 5f63 6f75 6e74 203e 2030 4e29 0f72 3200  _count > 0N).r2.
-00001b20: 0000 da07 636c 6173 7365 7372 3800 0000  ....classesr8...
-00001b30: da03 6c65 6e72 2400 0000 723f 0000 00da  ..lenr$...r?....
-00001b40: 0571 7565 7279 7236 0000 00da 0566 6972  .queryr6.....fir
-00001b50: 7374 7227 0000 00da 0972 656d 6169 6e69  str'.....remaini
-00001b60: 6e67 7233 0000 00da 0463 6466 73da 076c  ngr3.....cdfs..l
-00001b70: 656e 6774 6873 7213 0000 0029 0472 1500  engthsr....).r..
-00001b80: 0000 7278 0000 0072 2c00 0000 7279 0000  ..rx...r,...ry..
-00001b90: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001ba0: 7218 0000 00cf 0000 0073 1e00 0000 0007  r........s......
-00001bb0: 0a01 0801 0a06 1401 0402 0601 02ff 0403  ................
-00001bc0: 04fd 08ff 0409 0801 0801 0801 7a0f 4849  ............z.HI
-00001bd0: 4c41 5279 2e5f 5f69 6e69 745f 5f63 0200  LARy.__init__c..
-00001be0: 0000 0000 0000 0000 0000 1b00 0000 0700  ................
-00001bf0: 0000 4300 0001 73d4 0100 0074 0064 0183  ..C...s....t.d..
-00001c00: 017d 027c 015c 077d 037d 037d 047d 057d  .}.|.\.}.}.}.}.}
-00001c10: 067d 077d 087c 047c 006a 0176 0173 3074  .}.}.|.|.j.v.s0t
-00001c20: 027c 0683 0164 026b 0072 3864 037c 0866  .|...d.k.r8d.|.f
-00001c30: 0253 0074 03a0 0474 03a0 057c 06a1 0164  .S.t...t...|...d
-00001c40: 0417 00a1 017d 0974 036a 067c 067c 0964  .....}.t.j.|.|.d
-00001c50: 058d 025c 027d 0a7d 0b7c 0a64 0464 0085  ...\.}.}.|.d.d..
-00001c60: 0219 0074 077c 0a64 0464 0085 0219 0083  ...t.|.d.d......
-00001c70: 011b 007d 0c74 027c 0b83 0164 066b 0072  ...}.t.|...d.k.r
-00001c80: 8e64 037c 0866 0253 0074 036a 086a 097c  .d.|.f.S.t.j.j.|
-00001c90: 0b64 0464 0785 0219 007c 0264 087c 0c64  .d.d.....|.d.|.d
-00001ca0: 098d 047d 0d74 036a 086a 097c 0b64 0464  ...}.t.j.j.|.d.d
+000000a0: 0100 6401 640a 6c16 6d16 5a16 0100 6401  ..d.d.l.m.Z...d.
+000000b0: 640b 6c17 6d18 5a18 0100 6401 640c 6c19  d.l.m.Z...d.d.l.
+000000c0: 6d1a 5a1a 6d1b 5a1b 0100 650b a01c a100  m.Z.m.Z...e.....
+000000d0: 5a1d 4700 640d 640e 8400 640e 8302 5a1e  Z.G.d.d...d...Z.
+000000e0: 4700 640f 6410 8400 6410 8302 5a1f 4700  G.d.d...d...Z.G.
+000000f0: 6411 6412 8400 6412 8302 5a20 6405 5300  d.d...d...Z d.S.
+00000100: 2913 7a16 496e 6665 7220 636c 6f6e 616c  ).z.Infer clonal
+00000110: 2066 616d 696c 6965 732e e900 0000 0029   families......)
+00000120: 01da 0b61 6e6e 6f74 6174 696f 6e73 2901  ...annotations).
+00000130: da0c 636f 6d62 696e 6174 696f 6e73 2901  ..combinations).
+00000140: da04 506f 6f6c 4e29 01da 0854 7269 654e  ..PoolN)...TrieN
+00000150: 7563 6c29 02da 0866 636c 7573 7465 72da  ucl)...fcluster.
+00000160: 076c 696e 6b61 6765 2901 da0a 7371 7561  .linkage)...squa
+00000170: 7265 666f 726d 2901 da07 6861 6d6d 696e  reform)...hammin
+00000180: 6729 01da 0474 7164 6d29 01da 0741 7072  g)...tqdm)...Apr
+00000190: 696f 7269 2902 da0d 6170 706c 7950 6172  iori)...applyPar
+000001a0: 616c 6c65 6cda 0970 5265 7175 6972 6564  allel..pRequired
+000001b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001c0: 0006 0000 0040 0000 0173 5200 0000 6500  .....@...sR...e.
+000001d0: 5a01 6400 5a02 6401 5a03 6416 6403 6404  Z.d.Z.d.Z.d.d.d.
+000001e0: 6405 6406 9c03 6407 6408 8405 5a04 6409  d.d...d.d...Z.d.
+000001f0: 640a 640b 9c02 640c 640d 8404 5a05 6700  d.d...d.d...Z.g.
+00000200: 640e a201 640f 6602 6403 6410 6411 640a  d...d.f.d.d.d.d.
+00000210: 6412 9c04 6413 6414 8405 5a06 6415 5300  d...d.d...Z.d.S.
+00000220: 2917 da0e 4344 5233 436c 7573 7465 7269  )...CDR3Clusteri
+00000230: 6e67 7a4a 496e 6665 7220 6661 6d69 6c69  ngzJInfer famili
+00000240: 6573 2075 7369 6e67 2043 4452 3320 6c65  es using CDR3 le
+00000250: 6e67 7468 2061 6e64 2074 6872 6573 686f  ngth and thresho
+00000260: 6c64 7320 636f 6d70 7574 6564 2062 7920  lds computed by 
+00000270: 4170 7269 6f72 6920 636c 6173 732e e901  Apriori class...
+00000280: 0000 00fa 0c70 642e 4461 7461 4672 616d  .....pd.DataFram
+00000290: 65da 0369 6e74 da04 4e6f 6e65 2903 da0a  e..int..None)...
+000002a0: 7468 7265 7368 6f6c 6473 da07 7468 7265  thresholds..thre
+000002b0: 6164 73da 0672 6574 7572 6e63 0300 0000  ads..returnc....
+000002c0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+000002d0: 4300 0001 7310 0000 007c 017c 005f 007c  C...s....|.|._.|
+000002e0: 027c 005f 0164 0153 0029 027a e449 6e69  .|._.d.S.).z.Ini
+000002f0: 7469 616c 697a 6520 7468 7265 7368 6f6c  tialize threshol
+00000300: 6473 2e0a 0a20 2020 2020 2020 2041 7267  ds...        Arg
+00000310: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00000320: 6872 6573 686f 6c64 7320 7064 2e44 6174  hresholds pd.Dat
+00000330: 6146 7261 6d65 3a20 4461 7461 6672 616d  aFrame: Datafram
+00000340: 6520 636f 6e74 6169 6e69 6e67 2074 6872  e containing thr
+00000350: 6573 686f 6c64 7320 666f 7220 6561 6368  esholds for each
+00000360: 2028 562c 4a2c 6c29 2063 6c61 7373 2e0a   (V,J,l) class..
+00000370: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+00000380: 6164 7320 2869 6e74 2c20 6f70 7469 6f6e  ads (int, option
+00000390: 616c 293a 204e 756d 6265 7220 6f66 2063  al): Number of c
+000003a0: 7075 7320 6f6e 2077 6869 6368 2074 6f20  pus on which to 
+000003b0: 7275 6e20 636f 6465 2c20 6465 6661 756c  run code, defaul
+000003c0: 7473 2074 6f20 312e 0a20 2020 2020 2020  ts to 1..       
+000003d0: 204e 2902 7213 0000 0072 1400 0000 2903   N).r....r....).
+000003e0: da04 7365 6c66 7213 0000 0072 1400 0000  ..selfr....r....
+000003f0: a900 7217 0000 00fa 302f 686f 6d65 2f67  ..r.....0/home/g
+00000400: 6174 6865 6e65 732f 6769 746c 6162 2f48  athenes/gitlab/H
+00000410: 494c 4152 792f 6869 6c61 7279 2f69 6e66  ILARy/hilary/inf
+00000420: 6572 656e 6365 2e70 79da 085f 5f69 6e69  erence.py..__ini
+00000430: 745f 5f1c 0000 0073 0400 0000 0007 0601  t__....s........
+00000440: 7a17 4344 5233 436c 7573 7465 7269 6e67  z.CDR3Clustering
+00000450: 2e5f 5f69 6e69 745f 5f7a 2974 7570 6c65  .__init__z)tuple
+00000460: 5b74 7570 6c65 5b73 7472 2c20 7374 722c  [tuple[str, str,
+00000470: 2069 6e74 5d2c 2070 642e 4461 7461 4672   int], pd.DataFr
+00000480: 616d 655d fa09 7064 2e53 6572 6965 73a9  ame]..pd.Series.
+00000490: 02da 0461 7267 7372 1500 0000 6302 0000  ...argsr....c...
+000004a0: 0000 0000 0000 0000 000a 0000 0004 0000  ................
+000004b0: 0043 0000 0173 8c00 0000 7c01 5c02 5c03  .C...s....|.\.\.
+000004c0: 7d02 7d03 7d04 7d05 7400 8300 7d06 7c05  }.}.}.}.t...}.|.
+000004d0: 6401 1900 4400 5d0e 7d07 7c06 a001 7c07  d...D.].}.|...|.
+000004e0: a101 0100 711c 7c00 6a02 6a03 7c00 6a02  ....q.|.j.j.|.j.
+000004f0: 6a04 7c02 6b02 7c00 6a02 6a05 7c03 6b02  j.|.k.|.j.j.|.k.
+00000500: 4000 7c00 6a02 6a06 7c04 6b02 4000 1900  @.|.j.j.|.k.@...
+00000510: 6a07 6402 1900 6403 1900 7d08 7c08 6402  j.d...d...}.|.d.
+00000520: 6b05 7282 7c06 a008 7c08 a101 7d09 7c05  k.r.|...|...}.|.
+00000530: 6401 1900 a009 7c09 a101 5300 7c05 6a0a  d.....|...S.|.j.
+00000540: a00b a100 5300 2904 6131 0100 0052 6574  ....S.).a1...Ret
+00000550: 7572 6e20 636c 7573 7465 7220 6c61 6265  urn cluster labe
+00000560: 6c73 2064 6570 656e 6469 6e67 206f 6620  ls depending of 
+00000570: 7468 7265 7368 6f6c 6473 2069 6e20 7365  thresholds in se
+00000580: 6c66 2e74 6872 6573 686f 6c64 732e 0a0a  lf.thresholds...
+00000590: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000005a0: 2020 2020 2020 2020 2020 6172 6773 2028            args (
+000005b0: 5475 706c 655b 5475 706c 655b 7374 722c  Tuple[Tuple[str,
+000005c0: 2073 7472 2c20 696e 745d 2c20 7064 2e44   str, int], pd.D
+000005d0: 6174 6146 7261 6d65 5d29 3a20 2856 6765  ataFrame]): (Vge
+000005e0: 6e65 2c4a 6765 6e65 2c6c 292c 2044 6174  ne,Jgene,l), Dat
+000005f0: 6166 7261 6d65 0a20 2020 2020 2020 2020  aframe.         
+00000600: 2020 206f 6620 7365 7175 656e 6365 7320     of sequences 
+00000610: 6772 6f75 7065 6420 6279 2056 2c4a 2c6c  grouped by V,J,l
+00000620: 2063 6c61 7373 2e0a 0a20 2020 2020 2020   class...       
+00000630: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00000640: 2020 2020 2020 7064 2e53 6572 6965 733a        pd.Series:
+00000650: 2043 6c75 7374 6572 206c 6162 656c 7320   Cluster labels 
+00000660: 666f 7220 7468 6973 2056 2c4a 2c6c 2063  for this V,J,l c
+00000670: 6c61 7373 2e0a 2020 2020 2020 2020 da04  lass..        ..
+00000680: 6364 7233 7201 0000 00e9 ffff ffff 290c  cdr3r.........).
+00000690: da04 5472 6965 da06 696e 7365 7274 7213  ..Trie..insertr.
+000006a0: 0000 00da 036c 6f63 da06 765f 6765 6e65  .....loc..v_gene
+000006b0: da06 6a5f 6765 6e65 da0b 6364 7233 5f6c  ..j_gene..cdr3_l
+000006c0: 656e 6774 68da 0676 616c 7565 73da 0863  ength..values..c
+000006d0: 6c75 7374 6572 73da 036d 6170 da05 696e  lusters..map..in
+000006e0: 6465 78da 0874 6f5f 6672 616d 6529 0a72  dex..to_frame).r
+000006f0: 1600 0000 721c 0000 00da 0176 da01 6ada  ....r......v..j.
+00000700: 016c da02 6466 5a04 7472 6965 721d 0000  .l..dfZ.trier...
+00000710: 00da 0174 da03 6463 7472 1700 0000 7217  ...t..dctr....r.
+00000720: 0000 0072 1800 0000 da07 636c 7573 7465  ...r......cluste
+00000730: 7226 0000 0073 2600 0000 000a 0e01 0601  r&...s&.........
+00000740: 0c01 0c01 0601 0a01 0aff 0202 0afe 02ff  ................
+00000750: 0404 02fc 0204 02fc 0405 0801 0a01 0e01  ................
+00000760: 7a16 4344 5233 436c 7573 7465 7269 6e67  z.CDR3Clustering
+00000770: 2e63 6c75 7374 6572 a903 7222 0000 0072  .cluster..r"...r
+00000780: 2300 0000 7224 0000 0046 7a09 6c69 7374  #...r$...Fz.list
+00000790: 5b73 7472 5dda 0462 6f6f 6c29 0472 2d00  [str]..bool).r-.
+000007a0: 0000 da05 6772 6f75 70da 0673 696c 656e  ....group..silen
+000007b0: 7472 1500 0000 6304 0000 0000 0000 0000  tr....c.........
+000007c0: 0000 0005 0000 0006 0000 0043 0000 0173  ...........C...s
+000007d0: 4800 0000 7c02 6401 6701 1700 7d04 7400  H...|.d.g...}.t.
+000007e0: 7c01 7c04 1900 a001 7c02 a101 7c00 6a02  |.|.....|...|.j.
+000007f0: 7c03 7c00 6a03 6402 8d04 7c01 6403 3c00  |.|.j.d...|.d.<.
+00000800: 7c02 6403 6701 1700 7d02 7c01 a001 7c02  |.d.g...}.|...|.
+00000810: a101 a004 a100 6404 1700 5300 2905 6107  ......d...S.).a.
+00000820: 0200 0052 6574 7572 6e20 636c 7573 7465  ...Return cluste
+00000830: 7220 6c61 6265 6c73 2064 6570 656e 6469  r labels dependi
+00000840: 6e67 206f 6620 7468 7265 7368 6f6c 6473  ng of thresholds
+00000850: 2069 6e20 7365 6c66 2e74 6872 6573 686f   in self.thresho
+00000860: 6c64 732e 0a0a 2020 2020 2020 2020 5275  lds...        Ru
+00000870: 6e73 2073 656c 662e 636c 7573 7465 7220  ns self.cluster 
+00000880: 7061 7261 6c6c 656c 7920 6f6e 2064 6174  parallely on dat
+00000890: 6166 7261 6d65 2067 726f 7570 6564 2062  aframe grouped b
+000008a0: 7920 2767 726f 7570 2720 6172 6775 6d65  y 'group' argume
+000008b0: 6e74 2e0a 0a20 2020 2020 2020 2041 7267  nt...        Arg
+000008c0: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+000008d0: 6620 2870 642e 4461 7461 4672 616d 6529  f (pd.DataFrame)
+000008e0: 3a20 4461 7461 6672 616d 6520 6f66 2073  : Dataframe of s
+000008f0: 6571 7565 6e63 6573 2e0a 2020 2020 2020  equences..      
+00000900: 2020 2020 2020 6772 6f75 7020 286c 6973        group (lis
+00000910: 745b 7374 725d 2c20 6f70 7469 6f6e 616c  t[str], optional
+00000920: 293a 2047 726f 7570 7320 6f6e 2077 6869  ): Groups on whi
+00000930: 6368 2074 6f20 646f 2070 6172 616c 6c65  ch to do paralle
+00000940: 6c20 696e 6665 7272 696e 6720 6f66 2063  l inferring of c
+00000950: 6c75 7374 6572 732e 0a20 2020 2020 2020  lusters..       
+00000960: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00000970: 205b 2276 5f67 656e 6522 2c20 226a 5f67   ["v_gene", "j_g
+00000980: 656e 6522 2c20 2263 6472 335f 6c65 6e67  ene", "cdr3_leng
+00000990: 7468 225d 2e0a 2020 2020 2020 2020 2020  th"]..          
+000009a0: 2020 7369 6c65 6e74 2028 626f 6f6c 2c6f    silent (bool,o
+000009b0: 7074 696f 6e61 6c29 203a 2044 6f20 6e6f  ptional) : Do no
+000009c0: 7420 7368 6f77 2070 726f 6772 6573 7320  t show progress 
+000009d0: 6261 7220 6966 2054 7275 652e 0a0a 2020  bar if True...  
+000009e0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+000009f0: 2020 2020 2020 2020 2020 2070 642e 5365             pd.Se
+00000a00: 7269 6573 3a20 5365 7269 6573 2077 6974  ries: Series wit
+00000a10: 6820 636c 7573 7465 7220 6c61 6265 6c73  h cluster labels
+00000a20: 2e0a 2020 2020 2020 2020 721d 0000 00a9  ..        r.....
+00000a30: 0272 3400 0000 da08 6370 7543 6f75 6e74  .r4.....cpuCount
+00000a40: 7230 0000 0072 0f00 0000 2905 720c 0000  r0...r....).r...
+00000a50: 00da 0767 726f 7570 6279 7230 0000 0072  ...groupbyr0...r
+00000a60: 1400 0000 da06 6e67 726f 7570 2905 7216  ......ngroup).r.
+00000a70: 0000 0072 2d00 0000 7233 0000 0072 3400  ...r-...r3...r4.
+00000a80: 0000 da03 7573 6572 1700 0000 7217 0000  ....user....r...
+00000a90: 0072 1800 0000 da05 696e 6665 723e 0000  .r......infer>..
+00000aa0: 0073 1200 0000 0013 0a01 0201 0c01 0401  .s..............
+00000ab0: 0201 04fc 0a06 0a01 7a14 4344 5233 436c  ........z.CDR3Cl
+00000ac0: 7573 7465 7269 6e67 2e69 6e66 6572 4e29  ustering.inferN)
+00000ad0: 0172 0f00 0000 2907 da08 5f5f 6e61 6d65  .r....)...__name
+00000ae0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000af0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000b00: 646f 635f 5f72 1900 0000 7230 0000 0072  doc__r....r0...r
+00000b10: 3a00 0000 7217 0000 0072 1700 0000 7217  :...r....r....r.
+00000b20: 0000 0072 1800 0000 720e 0000 0019 0000  ...r....r.......
+00000b30: 0073 0c00 0000 0801 0402 140a 101b 0601  .s..............
+00000b40: 02fc 720e 0000 0063 0000 0000 0000 0000  ..r....c........
+00000b50: 0000 0000 0000 0000 0700 0000 4000 0001  ............@...
+00000b60: 7358 0000 0065 005a 0164 005a 0264 015a  sX...e.Z.d.Z.d.Z
+00000b70: 0364 1764 0364 0364 0464 0364 0564 069c  .d.d.d.d.d.d.d..
+00000b80: 0564 0764 0884 055a 0464 0964 0964 0a64  .d.d...Z.d.d.d.d
+00000b90: 0b9c 0364 0c64 0d84 045a 0564 0364 0e64  ...d.d...Z.d.d.d
+00000ba0: 0f9c 0264 1064 1184 045a 0664 1264 139c  ...d.d...Z.d.d..
+00000bb0: 0164 1464 1584 045a 0764 1653 0029 18da  .d.d...Z.d.S.)..
+00000bc0: 0e44 6973 7461 6e63 654d 6174 7269 787a  .DistanceMatrixz
+00000bd0: 4e4f 626a 6563 7420 656e 6162 6c69 6e67  NObject enabling
+00000be0: 2070 6172 616c 6c65 6c20 636f 6d70 7574   parallel comput
+00000bf0: 696e 6720 6f66 2074 6865 2064 6973 7461  ing of the dista
+00000c00: 6e63 6520 6d61 7274 7269 7820 6f66 2061  nce martrix of a
+00000c10: 206c 6172 6765 2063 6c75 7374 6572 2e72   large cluster.r
+00000c20: 0f00 0000 7211 0000 0072 1000 0000 7212  ....r....r....r.
+00000c30: 0000 0029 0572 2c00 0000 da10 616c 6967  ...).r,.....alig
+00000c40: 6e6d 656e 745f 6c65 6e67 7468 722d 0000  nment_lengthr-..
+00000c50: 0072 1400 0000 7215 0000 0063 0500 0000  .r....r....c....
+00000c60: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000c70: 4300 0001 737a 0000 007c 047c 005f 007c  C...sz...|.|._.|
+00000c80: 017c 005f 017c 027c 005f 027c 017c 006a  .|._.|.|._.|.|.j
+00000c90: 021b 007c 005f 037c 017c 006a 0217 007c  ...|._.|.|.j...|
+00000ca0: 006a 021b 007c 005f 047c 036a 057c 005f  .j...|._.|.j.|._
+00000cb0: 067c 006a 066a 0764 0119 007c 005f 087c  .|.j.j.d...|._.|
+00000cc0: 006a 087c 006a 0864 0218 0014 0064 031a  .j.|.j.d.....d..
+00000cd0: 007c 005f 0974 0a7c 006a 0864 0313 0064  .|._.t.|.j.d...d
+00000ce0: 031a 0064 041a 0064 0583 027c 005f 0b64  ...d...d...|._.d
+00000cf0: 0653 0029 0761 4001 0000 496e 6974 6961  .S.).a@...Initia
+00000d00: 6c69 7a65 2061 7474 7269 6275 7465 732e  lize attributes.
+00000d10: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00000d20: 2020 2020 2020 2020 2020 2020 6c20 2869              l (i
+00000d30: 6e74 293a 2043 4452 3320 6c65 6e67 7468  nt): CDR3 length
+00000d40: 0a20 2020 2020 2020 2020 2020 2061 6c69  .            ali
+00000d50: 676e 5f6c 656e 6774 6820 2869 6e74 293a  gn_length (int):
+00000d60: 204c 656e 6774 6820 6f66 2074 6865 2056   Length of the V
+00000d70: 6765 6e65 202b 204a 6765 6e65 2e0a 2020  gene + Jgene..  
+00000d80: 2020 2020 2020 2020 2020 6466 2028 7064            df (pd
+00000d90: 2e44 6174 6146 7261 6d65 293a 2044 6174  .DataFrame): Dat
+00000da0: 6166 7261 6d65 206f 6620 7365 7175 656e  aframe of sequen
+00000db0: 6365 7320 6772 6f75 7065 6420 6279 2028  ces grouped by (
+00000dc0: 762c 6a2c 6c2c 7365 6e73 6974 6976 6520  v,j,l,sensitive 
+00000dd0: 636c 7573 7465 7229 0a20 2020 2020 2020  cluster).       
+00000de0: 2020 2020 2074 6872 6561 6473 2028 696e       threads (in
+00000df0: 742c 206f 7074 696f 6e61 6c29 3a20 4e75  t, optional): Nu
+00000e00: 6d62 6572 206f 6620 6370 7573 206f 6e20  mber of cpus on 
+00000e10: 7768 6963 6820 746f 2072 756e 2063 6f64  which to run cod
+00000e20: 652e 2044 6566 6175 6c74 7320 746f 2031  e. Defaults to 1
+00000e30: 2e0a 2020 2020 2020 2020 7201 0000 0072  ..        r....r
+00000e40: 0f00 0000 e902 0000 00e9 f401 0000 e903  ................
+00000e50: 0000 004e 290c 7214 0000 0072 2c00 0000  ...N).r....r,...
+00000e60: da01 4cda 036c 5f4c da05 6c5f 4c5f 4c72  ..L..l_L..l_L_Lr
+00000e70: 2500 0000 da04 6461 7461 da05 7368 6170  %.....data..shap
+00000e80: 65da 016e da05 6b5f 6d61 78da 036d 6178  e..n..k_max..max
+00000e90: da06 6b5f 7374 6570 2905 7216 0000 0072  ..k_step).r....r
+00000ea0: 2c00 0000 7240 0000 0072 2d00 0000 7214  ,...r@...r-...r.
+00000eb0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000ec0: 0000 7219 0000 005f 0000 0073 1200 0000  ..r...._...s....
+00000ed0: 000f 0601 0601 0601 0c01 1201 0801 0e02  ................
+00000ee0: 1601 7a17 4469 7374 616e 6365 4d61 7472  ..z.DistanceMatr
+00000ef0: 6978 2e5f 5f69 6e69 745f 5f7a 1974 7570  ix.__init__z.tup
+00000f00: 6c65 5b73 7472 2c20 7374 722c 2069 6e74  le[str, str, int
+00000f10: 2c20 696e 745d da05 666c 6f61 7429 03da  , int]..float)..
+00000f20: 0461 7267 31da 0461 7267 3272 1500 0000  .arg1..arg2r....
+00000f30: 6303 0000 0000 0000 0000 0000 0014 0000  c...............
+00000f40: 0004 0000 0043 0000 0173 b000 0000 7c01  .....C...s....|.
+00000f50: 5c04 7d03 7d04 7d05 7d06 7c02 5c04 7d07  \.}.}.}.}.|.\.}.
+00000f60: 7d08 7d09 7d0a 7c06 7c0a 6b02 7228 7c00  }.}.}.|.|.k.r(|.
+00000f70: 6a00 0b00 5300 7c05 7c09 1400 7336 7c00  j...S.|.|...s6|.
+00000f80: 6a00 5300 7401 7c03 7c07 8302 7d0b 7401  j.S.t.|.|...}.t.
+00000f90: 7c04 7c08 8302 7d0c 7c05 7c09 1700 7c0c  |.|...}.|.|...|.
+00000fa0: 1800 6401 1b00 7d0d 7c00 6a02 7c0c 6402  ..d...}.|.j.|.d.
+00000fb0: 1700 1400 7d0e 7403 a004 7c0e 7c00 6a05  ....}.t...|.|.j.
+00000fc0: 1400 a101 7d0f 7c05 7c09 1400 7c00 6a00  ....}.|.|...|.j.
+00000fd0: 1b00 7d10 7403 a004 7c10 a101 7d11 7c0b  ..}.t...|...}.|.
+00000fe0: 7c0e 1800 7c0f 1b00 7d12 7c0d 7c10 1800  |...|...}.|.|...
+00000ff0: 7c11 1b00 7d13 7c12 7c13 1800 5300 2903  |...}.|.|...S.).
+00001000: 618e 0100 0043 6f6d 7075 7465 2064 6966  a....Compute dif
+00001010: 6665 7265 6e63 6520 6274 7765 656e 206e  ference btween n
+00001020: 6f72 6d61 6c69 7a65 6420 6364 7233 2064  ormalized cdr3 d
+00001030: 6976 6572 6765 6e63 6520 2620 7368 6172  ivergence & shar
+00001040: 6564 206d 7574 6174 696f 6e73 206f 6620  ed mutations of 
+00001050: 7477 6f20 7365 7175 656e 6365 732e 0a0a  two sequences...
+00001060: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00001070: 2020 2020 2020 2020 2020 6172 6731 2028            arg1 (
+00001080: 5475 706c 655b 7374 722c 7374 722c 696e  Tuple[str,str,in
+00001090: 742c 696e 745d 293a 2028 4344 5233 206c  t,int]): (CDR3 l
+000010a0: 656e 6774 682c 2056 2b4a 2073 6571 7565  ength, V+J seque
+000010b0: 6e63 6520 616c 6967 6e6d 656e 742c 206e  nce alignment, n
+000010c0: 756d 6265 7220 6f66 206d 7574 6174 696f  umber of mutatio
+000010d0: 6e73 0a20 2020 2020 2020 2020 2020 2066  ns.            f
+000010e0: 726f 6d20 6765 726d 6c69 6e65 2c20 696e  rom germline, in
+000010f0: 6465 7829 2066 6f72 2073 6571 7565 6e63  dex) for sequenc
+00001100: 6520 310a 2020 2020 2020 2020 2020 2020  e 1.            
+00001110: 6172 6732 2028 5475 706c 655b 7374 722c  arg2 (Tuple[str,
+00001120: 7374 722c 696e 742c 696e 745d 293a 2053  str,int,int]): S
+00001130: 616d 6520 666f 7220 7365 7175 656e 6365  ame for sequence
+00001140: 2032 0a0a 2020 2020 2020 2020 5265 7475   2..        Retu
+00001150: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00001160: 2066 6c6f 6174 3a20 4469 6666 6572 656e   float: Differen
+00001170: 6365 2062 6574 7765 656e 2074 776f 2071  ce between two q
+00001180: 7561 6e74 6974 6965 732e 0a20 2020 2020  uantities..     
+00001190: 2020 2072 4100 0000 720f 0000 0029 0672     rA...r....).r
+000011a0: 4400 0000 7209 0000 0072 4500 0000 da02  D...r....rE.....
+000011b0: 6e70 da04 7371 7274 7246 0000 0029 1472  np..sqrtrF...).r
+000011c0: 1600 0000 724e 0000 0072 4f00 0000 da05  ....rN...rO.....
+000011d0: 6364 7233 31da 0273 31da 026e 31da 0269  cdr31..s1..n1..i
+000011e0: 31da 0563 6472 3332 da02 7332 da02 6e32  1..cdr32..s2..n2
+000011f0: da02 6932 7249 0000 00da 026e 4cda 026e  ..i2rI.....nL..n
+00001200: 30da 0565 7870 5f6e da05 7374 645f 6eda  0..exp_n..std_n.
+00001210: 0665 7870 5f6e 30da 0673 7464 5f6e 30da  .exp_n0..std_n0.
+00001220: 0178 da01 7972 1700 0000 7217 0000 0072  .x..yr....r....r
+00001230: 1800 0000 da06 6d65 7472 6963 7900 0000  ......metricy...
+00001240: 7320 0000 0000 0f0c 010c 0108 0108 0108  s ..............
+00001250: 0106 010a 010a 0110 020e 0110 020e 010a  ................
+00001260: 020c 010c 017a 1544 6973 7461 6e63 654d  .....z.DistanceM
+00001270: 6174 7269 782e 6d65 7472 6963 7a1c 7475  atrix.metricz.tu
+00001280: 706c 655b 696e 742c 2069 6e74 2c20 6c69  ple[int, int, li
+00001290: 7374 5b66 6c6f 6174 5d5d 2902 da05 7374  st[float]])...st
+000012a0: 6172 7472 1500 0000 6302 0000 0000 0000  artr....c.......
+000012b0: 0000 0000 000b 0000 000a 0000 0043 0000  .............C..
+000012c0: 0173 ee00 0000 6700 7d02 7c01 7d03 7400  .s....g.}.|.}.t.
+000012d0: 7c01 7c00 6a01 1700 7c00 6a02 8302 7d04  |.|.j...|.j...}.
+000012e0: 7403 7c03 7c04 8302 4400 5dbe 7d05 7404  t.|.|...D.].}.t.
+000012f0: 7c00 6a05 6401 1800 7404 7406 a007 6402  |.j.d...t.t...d.
+00001300: 7c05 1400 6403 7c00 6a05 1400 7c00 6a05  |...d.|.j...|.j.
+00001310: 6404 1800 1400 1700 6405 1800 a101 6406  d.......d.....d.
+00001320: 1b00 6407 1800 8301 1800 8301 7d06 7404  ..d.........}.t.
+00001330: 7c05 7c06 1700 6404 1700 7c00 6a05 7c00  |.|...d...|.j.|.
+00001340: 6a05 6404 1800 1400 6401 1b00 1800 7c00  j.d.....d.....|.
+00001350: 6a05 7c06 1800 7c00 6a05 7c06 1800 6404  j.|...|.j.|...d.
+00001360: 1800 1400 6401 1b00 1700 8301 7d07 7c00  ....d.......}.|.
+00001370: 6a08 7c06 6408 6408 8502 6602 1900 7d08  j.|.d.d...f...}.
+00001380: 7c00 6a08 7c07 6408 6408 8502 6602 1900  |.j.|.d.d...f...
+00001390: 7d09 7c00 a009 7c08 7c09 a102 7d0a 7c02  }.|...|.|...}.|.
+000013a0: a00a 7c0a a101 0100 7124 7c03 7c04 7c02  ..|.....q$|.|.|.
+000013b0: 6603 5300 2909 610a 0100 0043 6f6d 7075  f.S.).a....Compu
+000013c0: 7465 2031 4420 6469 7374 616e 6365 206d  te 1D distance m
+000013d0: 6174 7269 7820 6265 7477 6565 6e20 7374  atrix between st
+000013e0: 6172 7420 616e 6420 7374 6172 742b 7365  art and start+se
+000013f0: 6c66 2e6b 5f73 7465 702e 0a0a 2020 2020  lf.k_step...    
+00001400: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00001410: 2020 2020 2020 7374 6172 7420 2869 6e74        start (int
+00001420: 293a 2049 6e64 6578 2066 726f 6d20 7768  ): Index from wh
+00001430: 6963 6820 746f 2063 6f6d 7075 7465 2064  ich to compute d
+00001440: 6973 7461 6e63 6573 2e0a 0a20 2020 2020  istances...     
+00001450: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00001460: 2020 2020 2020 2020 5475 706c 655b 696e          Tuple[in
+00001470: 742c 2069 6e74 2c20 6c69 7374 5b66 6c6f  t, int, list[flo
+00001480: 6174 5d5d 3a20 5374 6172 7420 696e 6465  at]]: Start inde
+00001490: 782c 2045 6e64 2069 6e64 6578 2c20 6469  x, End index, di
+000014a0: 7374 616e 6365 2066 6f72 2069 6e64 6963  stance for indic
+000014b0: 6573 2069 6e62 6574 7765 656e 0a20 2020  es inbetween.   
+000014c0: 2020 2020 2072 4100 0000 69f8 ffff ffe9       rA...i.....
+000014d0: 0400 0000 720f 0000 00e9 0700 0000 6700  ....r.........g.
+000014e0: 0000 0000 0000 4067 0000 0000 0000 e03f  ......@g.......?
+000014f0: 4e29 0bda 036d 696e 724c 0000 0072 4a00  N)...minrL...rJ.
+00001500: 0000 da05 7261 6e67 6572 1100 0000 7249  ....ranger....rI
+00001510: 0000 0072 5000 0000 7251 0000 0072 4700  ...rP...rQ...rG.
+00001520: 0000 7262 0000 00da 0661 7070 656e 6429  ..rb.....append)
+00001530: 0b72 1600 0000 7263 0000 00da 0464 6973  .r....rc.....dis
+00001540: 74da 026b 31da 026b 32da 016b da01 6972  t..k1..k2..k..ir
+00001550: 2b00 0000 da01 61da 0162 da01 6472 1700  +.....a..b..dr..
+00001560: 0000 7217 0000 0072 1800 0000 da04 7072  ..r....r......pr
+00001570: 6f63 9c00 0000 7336 0000 0000 0904 0104  oc....s6........
+00001580: 0112 010e 0202 0104 0102 ff02 0230 fe02  .............0..
+00001590: ff04 0502 0102 0102 ff02 0202 fe02 0312  ................
+000015a0: fd02 041a fc02 ff04 0812 0112 010c 010c  ................
+000015b0: 017a 1344 6973 7461 6e63 654d 6174 7269  .z.DistanceMatri
+000015c0: 782e 7072 6f63 fa0a 6e70 2e6e 6461 7272  x.proc..np.ndarr
+000015d0: 6179 a901 7215 0000 0063 0100 0000 0000  ay..r....c......
+000015e0: 0000 0000 0000 0600 0000 0800 0000 4300  ..............C.
+000015f0: 0001 7372 0000 0074 00a0 017c 006a 02a1  ..sr...t...|.j..
+00001600: 017d 0174 037c 006a 0483 018f 427d 027c  .}.t.|.j....B}.|
+00001610: 02a0 057c 006a 0674 0764 017c 006a 027c  ...|.j.t.d.|.j.|
+00001620: 006a 0883 03a1 0244 005d 165c 037d 037d  .j.....D.].\.}.}
+00001630: 047d 057c 057c 017c 037c 0485 023c 0071  .}.|.|.|.|...<.q
+00001640: 3257 0064 0204 0004 0083 0301 006e 1031  2W.d.........n.1
+00001650: 0073 5e30 0001 0001 0001 0059 0001 007c  .s^0.......Y...|
+00001660: 017c 006a 0917 0053 0029 037a 7a52 756e  .|.j...S.).zzRun
+00001670: 2073 656c 662e 7072 6f63 2070 6172 616c   self.proc paral
+00001680: 6c65 6c79 2074 6f20 636f 6d70 7574 6520  lely to compute 
+00001690: 3144 2064 6973 7461 6e63 6520 6d61 7472  1D distance matr
+000016a0: 6978 2e0a 0a20 2020 2020 2020 2052 6574  ix...        Ret
+000016b0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000016c0: 2020 6e70 2e61 7272 6179 3a20 3144 2064    np.array: 1D d
+000016d0: 6973 7461 6e63 6520 6d61 7472 6978 0a20  istance matrix. 
+000016e0: 2020 2020 2020 2072 0100 0000 4e29 0a72         r....N).r
+000016f0: 5000 0000 da05 7a65 726f 7372 4a00 0000  P.....zerosrJ...
+00001700: 7204 0000 0072 1400 0000 5a0e 696d 6170  r....r....Z.imap
+00001710: 5f75 6e6f 7264 6572 6564 7271 0000 0072  _unorderedrq...r
+00001720: 6700 0000 724c 0000 0072 4400 0000 2906  g...rL...rD...).
+00001730: 7216 0000 0072 6900 0000 da04 706f 6f6c  r....ri.....pool
+00001740: 726a 0000 0072 6b00 0000 da03 7265 7372  rj...rk.....resr
+00001750: 1700 0000 7217 0000 0072 1800 0000 da07  ....r....r......
+00001760: 636f 6d70 7574 65bd 0000 0073 1000 0000  compute....s....
+00001770: 0006 0c01 0c01 0401 0401 0efe 0e04 2c01  ..............,.
+00001780: 7a16 4469 7374 616e 6365 4d61 7472 6978  z.DistanceMatrix
+00001790: 2e63 6f6d 7075 7465 4e29 0172 0f00 0000  .computeN).r....
+000017a0: 2908 723b 0000 0072 3c00 0000 723d 0000  ).r;...r<...r=..
+000017b0: 0072 3e00 0000 7219 0000 0072 6200 0000  .r>...r....rb...
+000017c0: 7271 0000 0072 7700 0000 7217 0000 0072  rq...rw...r....r
+000017d0: 1700 0000 7217 0000 0072 1800 0000 723f  ....r....r....r?
+000017e0: 0000 005c 0000 0073 0c00 0000 0801 0407  ...\...s........
+000017f0: 00fb 181a 1223 1021 723f 0000 0063 0000  .....#.!r?...c..
+00001800: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00001810: 0000 4000 0001 73ac 0000 0065 005a 0164  ..@...s....e.Z.d
+00001820: 005a 0264 015a 0364 2c64 0364 0464 059c  .Z.d.Z.d,d.d.d..
+00001830: 0264 0664 0784 055a 0464 0864 0984 005a  .d.d...Z.d.d...Z
+00001840: 0564 0a64 0b84 005a 0664 0c64 0c64 0d64  .d.d...Z.d.d.d.d
+00001850: 0e64 0f9c 0464 1064 1184 045a 0764 1264  .d...d.d...Z.d.d
+00001860: 1364 149c 0264 1564 1684 045a 0864 1764  .d...d.d...Z.d.d
+00001870: 1764 189c 0264 1964 1a84 045a 0964 2d64  .d...d.d...Z.d-d
+00001880: 1764 0d64 1d64 1764 1e9c 0464 1f64 2084  .d.d.d.d...d.d .
+00001890: 055a 0a64 1764 1364 189c 0264 2164 2284  .Z.d.d.d...d!d".
+000018a0: 045a 0b64 2e64 1d64 2464 259c 0264 2664  .Z.d.d.d$d%..d&d
+000018b0: 2784 055a 0c64 1764 289c 0164 2964 2a84  '..Z.d.d(..d)d*.
+000018c0: 045a 0d64 2b53 0029 2fda 0648 494c 4152  .Z.d+S.)/..HILAR
+000018d0: 797a 3349 6e66 6572 2066 616d 696c 6965  yz3Infer familie
+000018e0: 7320 7573 696e 6720 4344 5233 2061 6e64  s using CDR3 and
+000018f0: 206d 7574 6174 696f 6e20 696e 666f 726d   mutation inform
+00001900: 6174 696f 6e2e 4672 0b00 0000 7232 0000  ation.Fr....r2..
+00001910: 0029 02da 0761 7072 696f 7269 da05 6372  .)...apriori..cr
+00001920: 7564 6563 0400 0000 0000 0000 0000 0000  udec............
+00001930: 0400 0000 0300 0000 4300 0001 7374 0000  ........C...st..
+00001940: 0067 0064 01a2 017c 005f 007c 016a 017c  .g.d...|._.|.j.|
+00001950: 005f 0167 0064 02a2 017c 005f 0274 037c  ._.g.d...|._.t.|
+00001960: 0264 0319 006a 0464 0419 0083 017c 005f  .d...j.d.....|._
+00001970: 057c 0373 507c 006a 01a0 0664 05a1 01a0  .|.sP|.j...d....
+00001980: 077c 006a 00a1 01a0 08a1 006a 097c 005f  .|.j.......j.|._
+00001990: 0a7c 016a 0b7c 005f 0b7c 016a 0c7c 005f  .|.j.|._.|.j.|._
+000019a0: 0c7c 016a 0d7c 005f 0d7c 016a 0e7c 005f  .|.j.|._.|.j.|._
+000019b0: 0e64 0653 0029 077a e149 6e69 7469 616c  .d.S.).z.Initial
+000019c0: 697a 6520 4869 6c61 7279 2061 7474 7269  ize Hilary attri
+000019d0: 6275 7465 7320 7573 696e 6720 4170 7269  butes using Apri
+000019e0: 6f72 6920 6f62 6a65 6374 2e0a 0a20 2020  ori object...   
+000019f0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00001a00: 2020 2020 2020 2061 7072 696f 7269 2028         apriori (
+00001a10: 4170 7269 6f72 6929 3a20 4170 7269 6f72  Apriori): Aprior
+00001a20: 6920 6f62 6a65 6374 2063 6f6e 7461 696e  i object contain
+00001a30: 696e 6720 6869 7374 6f67 7261 6d73 2061  ing histograms a
+00001a40: 6e64 2074 6872 6573 686f 6c64 732e 0a20  nd thresholds.. 
+00001a50: 2020 2020 2020 2020 2020 2078 795f 7468             xy_th
+00001a60: 7265 7368 6f6c 6420 2869 6e74 293a 5468  reshold (int):Th
+00001a70: 7265 7368 6f6c 6420 746f 2075 7365 2066  reshold to use f
+00001a80: 6f72 2074 6865 2078 7920 6d65 7468 6f64  or the xy method
+00001a90: 2e0a 2020 2020 2020 2020 7231 0000 0029  ..        r1...)
+00001aa0: 0472 1d00 0000 da16 616c 745f 7365 7175  .r......alt_sequ
+00001ab0: 656e 6365 5f61 6c69 676e 6d65 6e74 da0e  ence_alignment..
+00001ac0: 6d75 7461 7469 6f6e 5f63 6f75 6e74 7228  mutation_countr(
+00001ad0: 0000 0072 7b00 0000 7201 0000 007a 4f76  ...r{...r....zOv
+00001ae0: 5f67 656e 6520 213d 2027 4e6f 6e65 2720  _gene != 'None' 
+00001af0: 616e 6420 7072 6563 6973 655f 7468 7265  and precise_thre
+00001b00: 7368 6f6c 6420 3c20 7365 6e73 6974 6976  shold < sensitiv
+00001b10: 655f 7468 7265 7368 6f6c 6420 616e 6420  e_threshold and 
+00001b20: 7061 6972 5f63 6f75 6e74 203e 2030 4e29  pair_count > 0N)
+00001b30: 0f72 3300 0000 da07 636c 6173 7365 7372  .r3.....classesr
+00001b40: 3900 0000 da03 6c65 6e72 2500 0000 7240  9.....lenr%...r@
+00001b50: 0000 00da 0571 7565 7279 7237 0000 00da  .....queryr7....
+00001b60: 0566 6972 7374 7228 0000 00da 0972 656d  .firstr(.....rem
+00001b70: 6169 6e69 6e67 7234 0000 00da 0463 6466  ainingr4.....cdf
+00001b80: 73da 076c 656e 6774 6873 7214 0000 0029  s..lengthsr....)
+00001b90: 0472 1600 0000 7279 0000 0072 2d00 0000  .r....ry...r-...
+00001ba0: 727a 0000 0072 1700 0000 7217 0000 0072  rz...r....r....r
+00001bb0: 1800 0000 7219 0000 00d0 0000 0073 1e00  ....r........s..
+00001bc0: 0000 0007 0a01 0801 0a06 1401 0402 0601  ................
+00001bd0: 02ff 0403 04fd 08ff 0408 0801 0801 0801  ................
+00001be0: 7a0f 4849 4c41 5279 2e5f 5f69 6e69 745f  z.HILARy.__init_
+00001bf0: 5f63 0200 0000 0000 0000 0000 0000 1b00  _c..............
+00001c00: 0000 0700 0000 4300 0001 73dc 0100 0074  ......C...s....t
+00001c10: 0064 0183 017d 027c 015c 077d 037d 037d  .d...}.|.\.}.}.}
+00001c20: 047d 057d 067d 077d 0874 007c 0483 017d  .}.}.}.}.t.|...}
+00001c30: 047c 047c 006a 0176 0173 3874 027c 0683  .|.|.j.v.s8t.|..
+00001c40: 0164 026b 0072 4064 037c 0866 0253 0074  .d.k.r@d.|.f.S.t
+00001c50: 03a0 0474 03a0 057c 06a1 0164 0417 00a1  ...t...|...d....
+00001c60: 017d 0974 036a 067c 067c 0964 058d 025c  .}.t.j.|.|.d...\
+00001c70: 027d 0a7d 0b7c 0a64 0464 0085 0219 0074  .}.}.|.d.d.....t
+00001c80: 077c 0a64 0464 0085 0219 0083 011b 007d  .|.d.d.........}
+00001c90: 0c74 027c 0b83 0164 066b 0072 9664 037c  .t.|...d.k.r.d.|
+00001ca0: 0866 0253 0074 036a 086a 097c 0b64 0464  .f.S.t.j.j.|.d.d
 00001cb0: 0785 0219 007c 0264 087c 0c64 098d 047d  .....|.d.|.d...}
-00001cc0: 0e7c 0d7c 0e14 007c 071b 007d 0f74 036a  .|.|...|...}.t.j
-00001cd0: 086a 0a7c 0f7c 0264 0a8d 027d 1074 03a0  .j.|.|.d...}.t..
-00001ce0: 0b7c 0fa1 017d 117c 107c 0f18 007c 111b  .|...}.|.|...|..
-00001cf0: 007d 127c 006a 0c6a 0d7c 006a 0c64 0b19  .}.|.j.j.|.j.d..
-00001d00: 007c 046b 0219 006a 0e64 0364 047c 0464  .|.k...j.d.d.|.d
-00001d10: 0417 0085 0266 0219 007d 1374 036a 0f7c  .....f...}.t.j.|
-00001d20: 1364 0367 0164 0467 0164 0c8d 037d 1474  .d.g.d.g.d...}.t
-00001d30: 036a 086a 0974 03a0 047c 0464 0417 00a1  .j.j.t...|.d....
-00001d40: 017c 0264 087c 147c 14a0 07a1 001b 0064  .|.d.|.|.......d
-00001d50: 098d 047d 1574 03a0 107c 0d7c 0e17 0064  ...}.t...|.|...d
-00001d60: 0d7c 1014 0018 0064 03a1 027d 167c 047c  .|.....d...}.|.|
-00001d70: 071b 007c 1664 0417 0014 007d 1774 03a0  ...|.d.....}.t..
-00001d80: 0b7c 177c 047c 0717 0014 007c 071b 00a1  .|.|.|.....|....
-00001d90: 017d 187c 157c 1718 007c 181b 007d 197c  .}.|.|...|...}.|
-00001da0: 197c 1218 007d 1a74 03a0 117c 1aa1 0174  .|...}.t...|...t
-00001db0: 1274 007c 0274 137c 0583 0114 0083 017c  .t.|.t.|.......|
-00001dc0: 0264 0418 0083 0219 007c 0866 0253 0029  .d.......|.f.S.)
-00001dd0: 0e4e 6700 0000 0080 842e 41e9 6400 0000  .Ng.......A.d...
-00001de0: 7201 0000 0072 0e00 0000 2901 da04 6269  r....r....)...bi
-00001df0: 6e73 7242 0000 0072 1d00 0000 5429 03da  nsrB...r....T)..
-00001e00: 0473 697a 65da 0772 6570 6c61 6365 da01  .size..replace..
-00001e10: 7029 02da 036c 616d 7285 0000 0072 2b00  p)...lamr....r+.
-00001e20: 0000 2902 da07 7072 6570 656e 6472 6700  ..)...prependrg.
-00001e30: 0000 7240 0000 0029 1472 1000 0000 7282  ..r@...).r....r.
-00001e40: 0000 0072 7d00 0000 724f 0000 00da 0661  ...r}...rO.....a
-00001e50: 7261 6e67 6572 4a00 0000 da09 6869 7374  rangerJ.....hist
-00001e60: 6f67 7261 6dda 0373 756d da06 7261 6e64  ogram..sum..rand
-00001e70: 6f6d da06 6368 6f69 6365 da07 706f 6973  om..choice..pois
-00001e80: 736f 6e72 5000 0000 7281 0000 0072 2000  sonrP...r....r .
-00001e90: 0000 7224 0000 00da 0464 6966 66da 076d  ..r$.....diff..m
-00001ea0: 6178 696d 756d da04 736f 7274 7265 0000  aximum..sortre..
-00001eb0: 0072 0c00 0000 291b 7215 0000 0072 1b00  .r....).r....r..
-00001ec0: 0000 7285 0000 00da 015f 722b 0000 00da  ..r......_r+....
-00001ed0: 0a70 7265 7661 6c65 6e63 65da 096d 7574  .prevalence..mut
-00001ee0: 6174 696f 6e73 723f 0000 00da 0863 6c61  ationsr?.....cla
-00001ef0: 7373 5f69 6472 8400 0000 5a03 706e 695a  ss_idr....Z.pniZ
-00001f00: 036e 6973 7287 0000 005a 036e 3173 5a03  .nisr....Z.n1sZ.
-00001f10: 6e32 7372 5d00 0000 5a03 6e30 7372 5e00  n2sr]...Z.n0sr^.
-00001f20: 0000 da02 7973 da03 6364 66da 0270 6eda  ....ys..cdf..pn.
-00001f30: 026e 735a 036e 4c73 725b 0000 0072 5c00  .nsZ.nLsr[...r\.
-00001f40: 0000 da02 7873 da02 7a73 7216 0000 0072  ....xs..zsr....r
-00001f50: 1600 0000 7217 0000 00da 0e73 696d 756c  ....r......simul
-00001f60: 6174 655f 7873 5f79 73ee 0000 0073 3800  ate_xs_ys....s8.
-00001f70: 0000 0004 0801 1201 1601 0801 1401 1201  ................
-00001f80: 1c01 0c01 0801 1c01 1c01 0c01 1001 0a01  ................
-00001f90: 0c02 2801 1401 0601 1aff 0603 1801 1001  ..(.............
-00001fa0: 1601 0c01 0802 2201 02fe 7a15 4849 4c41  ......"...z.HILA
-00001fb0: 5279 2e73 696d 756c 6174 655f 7873 5f79  Ry.simulate_xs_y
-00001fc0: 7363 0200 0000 0000 0000 0000 0000 0c00  sc..............
-00001fd0: 0000 0a00 0000 4300 0001 73b6 0000 0074  ......C...s....t
-00001fe0: 007c 0164 0119 006a 0164 0219 0083 017d  .|.d...j.d.....}
-00001ff0: 0267 007d 037c 006a 0267 0064 03a2 0119  .g.}.|.j.g.d....
-00002000: 006a 0144 005d 4c5c 057d 047d 057d 067d  .j.D.]L\.}.}.}.}
-00002010: 077d 087c 0464 046b 0272 4c7c 01a0 0364  .}.|.d.k.rL|...d
-00002020: 05a1 0164 0619 007d 096e 0e7c 01a0 0364  ...d...}.n.|...d
-00002030: 07a1 0164 0619 007d 097c 03a0 047c 047c  ...d...}.|...|.|
-00002040: 057c 067c 077c 097c 027c 0866 07a1 0101  .|.|.|.|.|.f....
-00002050: 0071 2674 057c 037c 006a 067c 006a 077c  .q&t.|.|.j.|.j.|
-00002060: 006a 0864 0864 098d 057d 0a74 096a 0a7c  .j.d.d...}.t.j.|
-00002070: 0a64 0a64 0b67 0264 0c8d 02a0 0b64 0ba1  .d.d.g.d.....d..
-00002080: 017d 0b7c 0b64 0a19 007c 006a 0264 0a3c  .}.|.d...|.j.d.<
-00002090: 0064 0053 0029 0d4e 727a 0000 0072 0100  .d.S.).Nrz...r..
-000020a0: 0000 2905 7221 0000 0072 2200 0000 7223  ..).r!...r"...r#
-000020b0: 0000 00da 1465 6666 6563 7469 7665 5f70  .....effective_p
-000020c0: 7265 7661 6c65 6e63 6572 9600 0000 7211  revalencer....r.
-000020d0: 0000 007a 1963 6472 335f 6c65 6e67 7468  ...z.cdr3_length
-000020e0: 3d3d 4063 6472 335f 6c65 6e67 7468 727b  ==@cdr3_lengthr{
-000020f0: 0000 007a 4176 5f67 656e 653d 3d40 765f  ...zAv_gene==@v_
-00002100: 6765 6e65 2061 6e64 206a 5f67 656e 653d  gene and j_gene=
-00002110: 3d40 6a5f 6765 6e65 2061 6e64 2063 6472  =@j_gene and cdr
-00002120: 335f 6c65 6e67 7468 3d3d 4063 6472 335f  3_length==@cdr3_
-00002130: 6c65 6e67 7468 5429 0372 3500 0000 7233  lengthT).r5...r3
-00002140: 0000 00da 0569 7369 6e74 da0c 7879 5f74  .....isint..xy_t
-00002150: 6872 6573 686f 6c64 7296 0000 00a9 01da  hresholdr.......
-00002160: 0763 6f6c 756d 6e73 290c 727d 0000 0072  .columns).r}...r
-00002170: 2400 0000 727c 0000 0072 7e00 0000 7267  $...r|...r~...rg
-00002180: 0000 0072 0b00 0000 729d 0000 0072 1300  ...r....r....r..
-00002190: 0000 7233 0000 00da 0270 64da 0944 6174  ..r3.....pd..Dat
-000021a0: 6146 7261 6d65 da09 7365 745f 696e 6465  aFrame..set_inde
-000021b0: 7829 0c72 1500 0000 722c 0000 0072 3f00  x).r....r,...r?.
-000021c0: 0000 5a11 6d75 7461 7469 6f6e 735f 6772  ..Z.mutations_gr
-000021d0: 6f75 7065 6472 2100 0000 7222 0000 0072  oupedr!...r"...r
-000021e0: 2300 0000 7294 0000 0072 9600 0000 7295  #...r....r....r.
-000021f0: 0000 00da 0672 6573 756c 745a 0f74 6872  .....resultZ.thr
-00002200: 6573 686f 6c64 735f 6461 7461 7216 0000  esholds_datar...
-00002210: 0072 1600 0000 7217 0000 00da 1167 6574  .r....r......get
-00002220: 5f78 795f 7468 7265 7368 6f6c 6473 1101  _xy_thresholds..
-00002230: 0000 7352 0000 0000 0112 0104 0704 0106  ..sR............
-00002240: ff04 fa06 0102 0102 0102 0102 0102 0a08  ................
-00002250: 0110 0204 0102 ff02 0202 fe04 0304 0202  ................
-00002260: 0102 0102 0102 0102 0102 0102 f902 ff06  ................
-00002270: 0c02 0102 0104 0104 0104 0102 fb06 0804  ................
-00002280: 0108 ff06 0202 fe04 037a 1848 494c 4152  .........z.HILAR
-00002290: 792e 6765 745f 7879 5f74 6872 6573 686f  y.get_xy_thresho
-000022a0: 6c64 7372 7100 0000 724c 0000 007a 0e64  ldsrq...rL...z.d
-000022b0: 6963 745b 696e 742c 2069 6e74 5d29 04da  ict[int, int])..
-000022c0: 0769 6e64 6963 6573 7268 0000 00da 0974  .indicesrh.....t
-000022d0: 6872 6573 686f 6c64 7214 0000 0063 0400  hresholdr....c..
-000022e0: 0000 0000 0000 0000 0000 0500 0000 0500  ................
-000022f0: 0000 4300 0001 7324 0000 0074 0074 017c  ..C...s$...t.t.|
-00002300: 0264 0164 028d 0264 037c 0364 048d 037d  .d.d...d.|.d...}
-00002310: 0474 0274 037c 017c 0483 0283 0153 0029  .t.t.|.|.....S.)
-00002320: 0561 b201 0000 4d61 7020 7072 6563 6973  .a....Map precis
-00002330: 6520 636c 7573 7465 7273 2074 6f20 6e65  e clusters to ne
-00002340: 7720 7072 6563 6973 6520 414e 4420 7365  w precise AND se
-00002350: 6e73 6974 6976 6520 636c 7573 7465 7273  nsitive clusters
-00002360: 2062 7920 6d65 7267 696e 6720 636c 7573   by merging clus
-00002370: 7465 7273 2074 6f67 6574 6865 722e 0a0a  ters together...
-00002380: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00002390: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-000023a0: 7320 286e 702e 6172 7261 7929 3a20 496e  s (np.array): In
-000023b0: 6469 6365 7320 6f66 2070 7265 6369 7365  dices of precise
-000023c0: 2063 6c75 7374 6572 732e 0a20 2020 2020   clusters..     
-000023d0: 2020 2020 2020 2064 6973 7420 286e 702e         dist (np.
-000023e0: 6e64 6172 7261 7929 3a20 4469 7374 616e  ndarray): Distan
-000023f0: 6365 7320 6265 7477 6565 6e20 7072 6563  ces between prec
-00002400: 6973 6520 636c 7573 7465 7273 2e0a 2020  ise clusters..  
-00002410: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
-00002420: 6f6c 6420 2866 6c6f 6174 293a 2054 6872  old (float): Thr
-00002430: 6573 686f 6c64 2074 6f20 6d65 7267 6520  eshold to merge 
-00002440: 7477 6f20 7072 6563 6973 6520 636c 7573  two precise clus
-00002450: 7465 7273 2069 6620 7468 6520 6469 7374  ters if the dist
-00002460: 616e 6365 2069 7320 736d 616c 6c65 722e  ance is smaller.
-00002470: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00002480: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-00002490: 6963 743a 2044 6963 7469 6f6e 6172 7920  ict: Dictionary 
-000024a0: 6d61 7070 696e 6720 7072 6563 6973 6520  mapping precise 
-000024b0: 636c 7573 7465 7273 2074 6f20 7468 6569  clusters to thei
-000024c0: 7220 6e65 7720 636c 7573 7465 7273 2e0a  r new clusters..
-000024d0: 2020 2020 2020 2020 da06 7369 6e67 6c65          ..single
-000024e0: 2901 da06 6d65 7468 6f64 da08 6469 7374  )...method..dist
-000024f0: 616e 6365 2902 5a09 6372 6974 6572 696f  ance).Z.criterio
-00002500: 6e72 2d00 0000 2904 7206 0000 0072 0700  nr-...).r....r..
-00002510: 0000 da04 6469 6374 da03 7a69 7029 0572  ....dict..zip).r
-00002520: 1500 0000 72a8 0000 0072 6800 0000 72a9  ....r....rh...r.
-00002530: 0000 0072 2500 0000 7216 0000 0072 1600  ...r%...r....r..
-00002540: 0000 7217 0000 00da 0d73 696e 676c 654c  ..r......singleL
-00002550: 696e 6b61 6765 4201 0000 730c 0000 0000  inkageB...s.....
-00002560: 1002 010a 0102 0102 fd06 057a 1448 494c  ...........z.HIL
-00002570: 4152 792e 7369 6e67 6c65 4c69 6e6b 6167  ARy.singleLinkag
-00002580: 657a 2e74 7570 6c65 5b74 7570 6c65 5b73  ez.tuple[tuple[s
-00002590: 7472 2c20 7374 722c 2069 6e74 2c20 696e  tr, str, int, in
-000025a0: 745d 2c20 7064 2e44 6174 6146 7261 6d65  t], pd.DataFrame
-000025b0: 5d72 1900 0000 721a 0000 0063 0200 0000  ]r....r....c....
-000025c0: 0000 0000 0000 0000 2100 0000 0600 0000  ........!.......
-000025d0: 4300 0001 73e0 0100 007c 0164 0119 007d  C...s....|.d...}
-000025e0: 027c 0164 0219 005c 047d 037d 047d 057d  .|.d...\.}.}.}.}
-000025f0: 067c 006a 00a0 0164 03a1 0164 0419 006a  .|.j...d...d...j
-00002600: 0264 0219 007d 0774 03a0 047c 0264 0519  .d...}.t...|.d..
-00002610: 00a1 017d 0874 057c 0883 0164 016b 0172  ...}.t.|...d.k.r
-00002620: 507c 0264 0519 0053 0074 0674 077c 0874  P|.d...S.t.t.|.t
-00002630: 0874 057c 0883 0183 0183 0283 017d 097c  .t.|.........}.|
-00002640: 0264 0519 00a0 097c 09a1 017c 0264 063c  .d.....|...|.d.<
-00002650: 0074 057c 0883 017d 0a74 036a 0a7c 0a7c  .t.|...}.t.j.|.|
-00002660: 0a66 0274 0b64 078d 0264 087c 006a 0c14  .f.t.d...d.|.j..
-00002670: 0014 007d 0b74 087c 0a83 0144 005d 107d  ...}.t.|...D.].}
-00002680: 0c64 027c 0b7c 0c7c 0c66 023c 0071 a474  .d.|.|.|.f.<.q.t
-00002690: 0d7c 027c 006a 0e19 006a 0264 0883 0244  .|.|.j...j.d...D
-000026a0: 005d ee5c 025c 047d 0d7d 0e7d 0f7d 105c  .].\.\.}.}.}.}.\
-000026b0: 047d 117d 127d 137d 147c 107c 146b 0372  .}.}.}.}.|.|.k.r
-000026c0: c87c 0f7c 1314 007d 157c 1564 026b 0472  .|.|...}.|.d.k.r
-000026d0: c874 0f7c 0d7c 1183 027d 1674 0f7c 0e7c  .t.|.|...}.t.|.|
-000026e0: 1283 027d 177c 0f7c 1317 007c 1718 0064  ...}.|.|...|...d
-000026f0: 081b 007d 187c 057c 006a 0c1b 007c 1764  ...}.|.|.j...|.d
-00002700: 0117 0014 007d 1974 03a0 107c 197c 057c  .....}.t...|.|.|
-00002710: 006a 0c17 0014 007c 006a 0c1b 00a1 017d  .j.....|.j.....}
-00002720: 1a7c 157c 006a 0c1b 007d 1b74 03a0 107c  .|.|.j...}.t...|
-00002730: 1ba1 017d 1c7c 167c 1918 007c 1a1b 007d  ...}.|.|...|...}
-00002740: 1d7c 187c 1b18 007c 1c1b 007d 1e7c 1d7c  .|.|...|...}.|.|
-00002750: 1e18 007c 006a 0c17 007d 1f74 117c 1f7c  ...|.j...}.t.|.|
-00002760: 0b7c 107c 1466 0219 0083 027c 0b7c 107c  .|.|.f.....|.|.|
-00002770: 1466 023c 0074 117c 1f7c 0b7c 147c 1066  .f.<.t.|.|.|.|.f
-00002780: 0219 0083 027c 0b7c 147c 1066 023c 0071  .....|.|.|.f.<.q
-00002790: c87c 006a 127c 0874 137c 0b83 017c 006a  .|.j.|.t.|...|.j
-000027a0: 0c7c 0717 0064 098d 037d 207c 0264 0519  .|...d...} |.d..
-000027b0: 00a0 097c 20a1 0153 0029 0a61 1e01 0000  ...| ..S.).a....
-000027c0: 4772 6f75 7020 7072 6563 6973 6520 636c  Group precise cl
-000027d0: 7573 7465 7273 2074 6f67 6574 6865 722e  usters together.
-000027e0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000027f0: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00002800: 2028 5475 706c 655b 5475 706c 655b 7374   (Tuple[Tuple[st
-00002810: 722c 7374 722c 696e 742c 696e 745d 2c70  r,str,int,int],p
-00002820: 642e 4461 7461 4672 616d 655d 293a 2028  d.DataFrame]): (
-00002830: 5667 656e 652c 4a67 656e 652c 6364 7233  Vgene,Jgene,cdr3
-00002840: 6c65 6e67 7468 292c 6461 7461 6672 616d  length),datafram
-00002850: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
-00002860: 7072 6573 656e 7469 6e67 2073 656e 7369  presenting sensi
-00002870: 7469 7665 2063 6c75 7374 6572 2e0a 0a20  tive cluster... 
-00002880: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00002890: 2020 2020 2020 2020 2020 2020 7064 2e53              pd.S
-000028a0: 6572 6965 733a 204e 6577 2063 6c75 7374  eries: New clust
-000028b0: 6572 7320 6d61 6465 206f 6620 6772 6f75  ers made of grou
-000028c0: 7065 6420 7072 6563 6973 6520 636c 7573  ped precise clus
-000028d0: 7465 7273 2e0a 2020 2020 2020 2020 720e  ters..        r.
-000028e0: 0000 0072 0100 0000 fa37 765f 6765 6e65  ...r.....7v_gene
-000028f0: 3d3d 4076 5f67 656e 6520 616e 6420 6a5f  ==@v_gene and j_
-00002900: 6765 6e65 3d3d 406a 5f67 656e 6520 616e  gene==@j_gene an
-00002910: 6420 6364 7233 5f6c 656e 6774 683d 3d40  d cdr3_length==@
-00002920: 6c72 a000 0000 da0f 7072 6563 6973 655f  lr......precise_
-00002930: 636c 7573 7465 7272 2700 0000 2901 da05  clusterr'...)...
-00002940: 6474 7970 6572 4000 0000 2901 72a9 0000  dtyper@...).r...
-00002950: 0029 1472 7c00 0000 727e 0000 0072 2400  .).r|...r~...r$.
-00002960: 0000 724f 0000 00da 0675 6e69 7175 6572  ..rO.....uniquer
-00002970: 7d00 0000 72ad 0000 0072 ae00 0000 7266  }...r....r....rf
-00002980: 0000 0072 2600 0000 da04 6f6e 6573 724c  ...r&.....onesrL
-00002990: 0000 0072 3f00 0000 7203 0000 0072 3800  ...r?...r....r8.
-000029a0: 0000 7209 0000 0072 5000 0000 7265 0000  ..r....rP...re..
-000029b0: 0072 af00 0000 7208 0000 0029 2172 1500  .r....r....)!r..
-000029c0: 0000 721b 0000 0072 2c00 0000 7221 0000  ..r....r,...r!..
-000029d0: 0072 2200 0000 722b 0000 0072 9300 0000  .r"...r+...r....
-000029e0: 72a0 0000 0072 a800 0000 5a10 7472 616e  r....r....Z.tran
-000029f0: 736c 6174 6549 6e64 6963 6573 da03 6469  slateIndices..di
-00002a00: 6d5a 0e64 6973 7461 6e63 654d 6174 7269  mZ.distanceMatri
-00002a10: 7872 6c00 0000 7251 0000 0072 5200 0000  xrl...rQ...rR...
-00002a20: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00002a30: 5600 0000 7257 0000 0072 5800 0000 5a04  V...rW...rX...Z.
-00002a40: 6e31 6e32 7248 0000 0072 5900 0000 725a  n1n2rH...rY...rZ
-00002a50: 0000 0072 5b00 0000 725c 0000 0072 5d00  ...r[...r\...r].
-00002a60: 0000 725e 0000 0072 5f00 0000 7260 0000  ..r^...r_...r`..
-00002a70: 0072 ac00 0000 da02 736c 7216 0000 0072  .r......slr....r
-00002a80: 1600 0000 7217 0000 00da 0b63 6c61 7373  ....r......class
-00002a90: 3270 6169 7273 5901 0000 7358 0000 0000  2pairsY...sX....
-00002aa0: 0d08 0110 0106 0102 ff02 0202 fe04 0202  ................
-00002ab0: fe04 040e 010c 0108 0216 0112 0108 011c  ................
-00002ac0: 010c 010e 0102 010c ff1c 0308 0108 0108  ................
-00002ad0: 010a 010a 0110 0212 0104 0112 ff04 030a  ................
-00002ae0: 010a 010c 010c 010e 011a 011c 0104 0102  ................
-00002af0: 0106 0108 fd06 057a 1248 494c 4152 792e  .......z.HILARy.
-00002b00: 636c 6173 7332 7061 6972 7372 0f00 0000  class2pairsr....
-00002b10: 2902 722c 0000 0072 1400 0000 6302 0000  ).r,...r....c...
-00002b20: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00002b30: 0043 0000 0173 6400 0000 7400 7c00 6a01  .C...sd...t.|.j.
-00002b40: 7c00 6a02 6401 6701 1700 1900 7c00 6a03  |.j.d.g.....|.j.
-00002b50: 6402 8d02 7d02 7400 7c00 6a01 7c00 6a02  d...}.t.|.j.|.j.
-00002b60: 6403 6701 1700 1900 7c00 6a03 6402 8d02  d.g.....|.j.d...
-00002b70: 7d03 7c02 6a04 7c01 7c00 6a05 6404 8d02  }.|.j.|.|.j.d...
-00002b80: 7c01 6405 3c00 7c03 6a04 7c01 7c00 6a05  |.d.<.|.j.|.|.j.
-00002b90: 6404 8d02 7c01 6406 3c00 7c01 5300 2907  d...|.d.<.|.S.).
-00002ba0: fac2 496e 6665 7220 7072 6563 6973 6520  ..Infer precise 
-00002bb0: 616e 6420 7365 6e73 6974 6976 6520 636c  and sensitive cl
-00002bc0: 7573 7465 7273 2e0a 0a20 2020 2020 2020  usters...       
-00002bd0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00002be0: 2020 2064 6628 7064 2e44 6174 6146 7261     df(pd.DataFra
-00002bf0: 6d65 293a 4461 7461 6672 616d 6520 6f66  me):Dataframe of
-00002c00: 2073 6571 7565 6e63 6573 2e0a 0a20 2020   sequences...   
-00002c10: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00002c20: 2020 2020 2020 2020 2020 7064 2e44 6174            pd.Dat
-00002c30: 6146 7261 6d65 2077 6974 6820 7365 6e73  aFrame with sens
-00002c40: 6974 6976 6520 616e 6420 7072 6563 6973  itive and precis
-00002c50: 6520 636c 7573 7465 7273 2e0a 2020 2020  e clusters..    
-00002c60: 2020 2020 da11 7072 6563 6973 655f 7468      ..precise_th
-00002c70: 7265 7368 6f6c 64a9 0172 1300 0000 da13  reshold..r......
-00002c80: 7365 6e73 6974 6976 655f 7468 7265 7368  sensitive_thresh
-00002c90: 6f6c 64a9 0172 3300 0000 72b1 0000 00da  old..r3...r.....
-00002ca0: 1173 656e 7369 7469 7665 5f63 6c75 7374  .sensitive_clust
-00002cb0: 6572 2906 720d 0000 0072 7c00 0000 7232  er).r....r|...r2
-00002cc0: 0000 0072 1300 0000 7239 0000 0072 3300  ...r....r9...r3.
-00002cd0: 0000 2904 7215 0000 0072 2c00 0000 da04  ..).r....r,.....
-00002ce0: 7072 6563 5a04 7365 6e73 7216 0000 0072  precZ.sensr....r
-00002cf0: 1600 0000 7217 0000 00da 1a63 6f6d 7075  ....r......compu
-00002d00: 7465 5f70 7265 635f 7365 6e73 5f63 6c75  te_prec_sens_clu
-00002d10: 7374 6572 7392 0100 0073 1400 0000 0009  sters....s......
-00002d20: 0201 14ff 0603 0201 1001 04fe 0604 1401  ................
-00002d30: 1401 7a21 4849 4c41 5279 2e63 6f6d 7075  ..z!HILARy.compu
-00002d40: 7465 5f70 7265 635f 7365 6e73 5f63 6c75  te_prec_sens_clu
-00002d50: 7374 6572 73e7 9a99 9999 9999 c93f 721d  sters........?r.
-00002d60: 0000 0072 1000 0000 2904 722c 0000 00da  ...r....).r,....
-00002d70: 146e 6f72 6d61 6c69 7a65 645f 7468 7265  .normalized_thre
-00002d80: 7368 6f6c 64da 0f66 6978 6564 5f74 6872  shold..fixed_thr
-00002d90: 6573 686f 6c64 7214 0000 0063 0400 0000  esholdr....c....
-00002da0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00002db0: 4300 0001 7382 0000 007c 0364 016b 0572  C...s....|.d.k.r
-00002dc0: 2474 00a0 0164 027c 039b 009d 02a1 0101  $t...d.|........
-00002dd0: 007c 037c 006a 0264 033c 006e 2a74 00a0  .|.|.j.d.<.n*t..
-00002de0: 0164 047c 029b 009d 02a1 0101 007c 006a  .d.|.........|.j
-00002df0: 0264 0519 007c 0214 00a0 0374 04a1 017c  .d...|.....t...|
-00002e00: 006a 0264 033c 0074 057c 006a 027c 006a  .j.d.<.t.|.j.|.j
-00002e10: 0664 0367 0117 0019 007c 006a 0764 068d  .d.g.....|.j.d..
-00002e20: 027d 047c 046a 087c 017c 006a 0964 078d  .}.|.j.|.|.j.d..
-00002e30: 027c 0164 083c 007c 0153 0029 0972 b800  .|.d.<.|.S.).r..
-00002e40: 0000 7201 0000 007a 2d55 7369 6e67 2063  ..r....z-Using c
-00002e50: 7275 6465 206d 6574 686f 6420 7769 7468  rude method with
-00002e60: 2061 2066 6978 6564 2074 6872 6573 686f   a fixed thresho
-00002e70: 6c64 206f 6620 72a9 0000 007a 3255 7369  ld of r....z2Usi
-00002e80: 6e67 2063 7275 6465 206d 6574 686f 6420  ng crude method 
-00002e90: 7769 7468 2061 206e 6f72 6d61 6c69 7a65  with a normalize
-00002ea0: 6420 7468 7265 7368 6f6c 6420 6f66 2072  d threshold of r
-00002eb0: 2300 0000 72ba 0000 0072 bc00 0000 da13  #...r....r......
-00002ec0: 6372 7564 655f 6d65 7468 6f64 5f66 616d  crude_method_fam
-00002ed0: 696c 7929 0ada 036c 6f67 da04 696e 666f  ily)...log..info
-00002ee0: 727c 0000 00da 0661 7374 7970 6572 1000  r|.....astyper..
-00002ef0: 0000 720d 0000 0072 3200 0000 7213 0000  ..r....r2...r...
-00002f00: 0072 3900 0000 7233 0000 0029 0572 1500  .r9...r3...).r..
-00002f10: 0000 722c 0000 0072 c100 0000 72c2 0000  ..r,...r....r...
-00002f20: 0072 be00 0000 7216 0000 0072 1600 0000  .r....r....r....
-00002f30: 7217 0000 00da 1d63 6f6d 7075 7465 5f63  r......compute_c
-00002f40: 7275 6465 5f6d 6574 686f 645f 636c 7573  rude_method_clus
-00002f50: 7465 7273 a601 0000 731e 0000 0000 0e08  ters....s.......
-00002f60: 0110 010c 0204 0108 ff04 040c ff02 0202  ................
-00002f70: fe0a 0302 0114 ff06 0314 017a 2448 494c  ...........z$HIL
-00002f80: 4152 792e 636f 6d70 7574 655f 6372 7564  ARy.compute_crud
-00002f90: 655f 6d65 7468 6f64 5f63 6c75 7374 6572  e_method_cluster
-00002fa0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00002fb0: 0000 0300 0000 4300 0001 7310 0000 0064  ......C...s....d
-00002fc0: 017c 0164 023c 007c 0164 0219 0053 0029  .|.d.<.|.d...S.)
-00002fd0: 0361 0501 0000 466c 6167 2061 6c6c 2069  .a....Flag all i
-00002fe0: 6e64 6963 6573 206f 6620 6120 7365 6e73  ndices of a sens
-00002ff0: 6974 6976 6520 636c 7573 7465 7220 6e6f  itive cluster no
-00003000: 7420 7265 6163 6869 6e67 2064 6573 6972  t reaching desir
-00003010: 6564 2073 656e 7369 7469 7669 7479 2e0a  ed sensitivity..
-00003020: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00003030: 2020 2020 2020 2020 2020 2064 6620 2870             df (p
-00003040: 642e 4461 7461 4672 616d 6529 3a20 4461  d.DataFrame): Da
-00003050: 7461 6672 616d 6520 6772 6f75 7065 6420  taframe grouped 
-00003060: 7265 7072 6573 656e 7469 6e67 2067 6976  representing giv
-00003070: 656e 2063 6c75 7374 6572 2e0a 0a20 2020  en cluster...   
-00003080: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00003090: 2020 2020 2020 2020 2020 7064 2e53 6572            pd.Ser
-000030a0: 6965 733a 2053 6572 6965 7320 666c 6167  ies: Series flag
-000030b0: 6769 6e67 2061 6c6c 2069 6e64 6963 6573  ging all indices
-000030c0: 206f 6620 6769 7665 6e20 636c 7573 7465   of given cluste
-000030d0: 722e 0a20 2020 2020 2020 2054 da0a 746f  r..        T..to
-000030e0: 5f72 6573 6f6c 7665 7216 0000 0029 0272  _resolver....).r
-000030f0: 1500 0000 722c 0000 0072 1600 0000 7216  ....r,...r....r.
-00003100: 0000 0072 1700 0000 da0a 6d61 726b 5f63  ...r......mark_c
-00003110: 6c61 7373 c401 0000 7304 0000 0000 0908  lass....s.......
-00003120: 017a 1148 494c 4152 792e 6d61 726b 5f63  .z.HILARy.mark_c
-00003130: 6c61 7373 7241 0000 007a 2f74 7570 6c65  lassrA...z/tuple
-00003140: 5b70 642e 4461 7461 4672 616d 652c 2070  [pd.DataFrame, p
-00003150: 642e 4461 7461 4672 616d 652c 2070 642e  d.DataFrame, pd.
-00003160: 4461 7461 4672 616d 655d 2902 da0e 7369  DataFrame])...si
-00003170: 7a65 5f74 6872 6573 686f 6c64 7214 0000  ze_thresholdr...
-00003180: 0063 0300 0000 0000 0000 0000 0000 0800  .c..............
-00003190: 0000 0600 0000 0300 0001 73a0 0000 0064  ..........s....d
-000031a0: 0188 0064 023c 0088 016a 006a 0172 1c74  ...d.<...j.j.r.t
-000031b0: 02a0 0364 03a1 0101 006e 3c74 0487 0087  ...d.....n<t....
-000031c0: 0166 0264 0464 0584 0888 016a 0044 0083  .f.d.d.....j.D..
-000031d0: 0188 016a 0564 0688 016a 0664 078d 0488  ...j.d...j.d....
-000031e0: 0064 023c 0088 006a 0764 0264 0169 0164  .d.<...j.d.d.i.d
-000031f0: 0664 088d 0201 0088 00a0 0864 09a1 01a0  .d.........d....
-00003200: 0988 016a 0a64 0a67 0117 00a1 017d 037c  ...j.d.g.....}.|
-00003210: 03a0 0ba1 007d 047c 047c 026b 047d 057c  .....}.|.|.k.}.|
-00003220: 047c 0519 006a 0c7d 067c 047c 050f 0019  .|...j.}.|.|....
-00003230: 006a 0c7d 0788 007c 077c 0666 0353 0029  .j.}...|.|.f.S.)
-00003240: 0b61 9001 0000 436c 6173 7369 6679 2073  .a....Classify s
-00003250: 656e 7369 7469 7665 2063 6c75 7374 6572  ensitive cluster
-00003260: 7320 6e6f 7420 7265 6163 6869 6e67 2064  s not reaching d
-00003270: 6573 6972 6564 2073 656e 7369 7469 7669  esired sensitivi
-00003280: 7479 2069 6e74 6f20 6269 6720 6f72 2073  ty into big or s
-00003290: 6d61 6c6c 2063 6c75 7374 6572 2e0a 0a20  mall cluster... 
-000032a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000032b0: 2020 2020 2020 2020 2064 6628 7064 2e44           df(pd.D
-000032c0: 6174 6146 7261 6d65 293a 4461 7461 6672  ataFrame):Datafr
-000032d0: 616d 6520 6f66 2073 6571 7565 6e63 6573  ame of sequences
-000032e0: 2e0a 2020 2020 2020 2020 2020 2020 7369  ..            si
-000032f0: 7a65 5f74 6872 6573 686f 6c64 2028 696e  ze_threshold (in
-00003300: 742c 206f 7074 696f 6e61 6c29 3a20 5468  t, optional): Th
-00003310: 7265 7368 6f6c 6420 746f 2073 6570 6172  reshold to separ
-00003320: 6174 6520 6269 6720 616e 6420 736d 616c  ate big and smal
-00003330: 6c20 636c 7573 7465 7273 2e0a 2020 2020  l clusters..    
-00003340: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00003350: 2074 6f20 3165 332e 0a0a 2020 2020 2020   to 1e3...      
-00003360: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00003370: 2020 2020 2020 2054 7570 6c65 5b70 642e         Tuple[pd.
-00003380: 4461 7461 4672 616d 652c 7064 2e44 6174  DataFrame,pd.Dat
-00003390: 6146 7261 6d65 5d3a 2052 6574 7572 6e73  aFrame]: Returns
-000033a0: 2069 6e64 6963 6573 206f 6620 736d 616c   indices of smal
-000033b0: 6c20 616e 6420 6269 6720 7365 6e73 6974  l and big sensit
-000033c0: 6976 6520 636c 7573 7465 7273 2e0a 2020  ive clusters..  
-000033d0: 2020 2020 2020 4672 c800 0000 7a1f 4e6f        Fr....z.No
-000033e0: 2063 6c61 7373 6573 2070 6173 7365 6420   classes passed 
-000033f0: 746f 2078 7920 6d65 7468 6f64 2e63 0100  to xy method.c..
-00003400: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00003410: 0000 1300 0001 731e 0000 0067 007c 005d  ......s....g.|.]
-00003420: 167d 0188 00a0 0088 016a 01a1 01a0 027c  .}.......j.....|
-00003430: 01a1 0191 0271 0453 0072 1600 0000 2903  .....q.S.r....).
-00003440: 7236 0000 0072 3200 0000 da09 6765 745f  r6...r2.....get_
-00003450: 6772 6f75 70a9 02da 022e 30da 0167 a902  group.....0..g..
-00003460: 722c 0000 0072 1500 0000 7216 0000 0072  r,...r....r....r
-00003470: 1700 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00003480: e401 0000 f300 0000 007a 2048 494c 4152  .........z HILAR
-00003490: 792e 746f 5f64 6f2e 3c6c 6f63 616c 733e  y.to_do.<locals>
-000034a0: 2e3c 6c69 7374 636f 6d70 3e54 7234 0000  .<listcomp>Tr4..
-000034b0: 00a9 02da 0576 616c 7565 da07 696e 706c  .....value..inpl
-000034c0: 6163 657a 1274 6f5f 7265 736f 6c76 6520  acez.to_resolve 
-000034d0: 3d3d 2054 7275 6572 bd00 0000 290d 7280  == Truer....).r.
-000034e0: 0000 00da 0565 6d70 7479 72c4 0000 0072  .....emptyr....r
-000034f0: c500 0000 720b 0000 0072 c900 0000 7213  ....r....r....r.
-00003500: 0000 00da 0666 696c 6c6e 6172 7e00 0000  .....fillnar~...
-00003510: 7236 0000 0072 3200 0000 7285 0000 0072  r6...r2...r....r
-00003520: 2700 0000 2908 7215 0000 0072 2c00 0000  '...).r....r,...
-00003530: 72ca 0000 00da 0964 6647 726f 7570 6564  r......dfGrouped
-00003540: da05 7369 7a65 73da 046d 6173 6bda 0b6c  ..sizes..mask..l
-00003550: 6172 6765 5f74 6f5f 646f da0b 736d 616c  arge_to_do..smal
-00003560: 6c5f 746f 5f64 6f72 1600 0000 72cf 0000  l_to_dor....r...
-00003570: 0072 1700 0000 da05 746f 5f64 6fd0 0100  .r......to_do...
-00003580: 0073 2400 0000 000f 0801 0801 0c02 0201  .s$.............
-00003590: 1401 0401 0201 04fc 0a06 1201 0a01 0aff  ................
-000035a0: 0403 0801 0801 0a01 0c01 7a0c 4849 4c41  ..........z.HILA
-000035b0: 5279 2e74 6f5f 646f 7272 0000 0063 0200  Ry.to_dorr...c..
-000035c0: 0000 0000 0000 0000 0000 0e00 0000 0700  ................
-000035d0: 0000 0300 0001 73a2 0100 007c 00a0 007c  ......s....|...|
-000035e0: 01a1 015c 037d 017d 027d 0374 017c 0164  ...\.}.}.}.t.|.d
-000035f0: 0119 006a 0264 0219 0083 017c 005f 0374  ...j.d.....|._.t
-00003600: 046a 0564 037c 006a 0364 048d 0201 0074  .j.d.|.j.d.....t
-00003610: 067c 0164 0519 0083 0173 6874 04a0 0764  .|.d.....sht...d
-00003620: 06a1 0101 007c 0164 0719 007c 0164 083c  .....|.d...|.d.<
-00003630: 007c 016a 0864 0967 0164 0a8d 017d 017c  .|.j.d.g.d...}.|
-00003640: 0153 007c 01a0 097c 006a 0a64 0b67 0117  .S.|...|.j.d.g..
-00003650: 00a1 0189 0074 04a0 0564 0ca1 0101 0074  .....t...d.....t
-00003660: 0b87 0066 0164 0d64 0e84 087c 0244 0083  ...f.d.d...|.D..
-00003670: 017c 006a 0c7c 006a 0d7c 006a 0e64 0f8d  .|.j.|.j.|.j.d..
-00003680: 047c 0164 103c 0074 04a0 0564 11a1 0101  .|.d.<.t...d....
-00003690: 0069 007d 047c 0344 005d 787d 057c 055c  .i.}.|.D.]x}.|.\
-000036a0: 047d 067d 077d 087d 097c 006a 0fa0 1064  .}.}.}.}.|.j...d
-000036b0: 12a1 0164 1319 006a 0264 0219 007d 0a74  ...d...j.d...}.t
-000036c0: 117c 087c 006a 0388 00a0 127c 05a1 0167  .|.|.j.....|...g
-000036d0: 0064 14a2 0119 007c 006a 0e64 158d 047d  .d.....|.j.d...}
-000036e0: 0b7c 0ba0 13a1 007d 0c7c 006a 1488 00a0  .|.....}.|.j....
-000036f0: 127c 05a1 016a 157c 0c7c 006a 037c 0a17  .|...j.|.|.j.|..
-00003700: 0064 168d 037d 0d7c 04a0 167c 0da1 0101  .d...}.|...|....
-00003710: 0071 be7c 016a 157c 0164 173c 007c 0164  .q.|.j.|.d.<.|.d
-00003720: 1019 00a0 177c 0164 1719 00a0 187c 04a1  .....|.d.....|..
-00003730: 01a1 017c 0164 103c 007c 016a 1764 1064  ...|.d.<.|.j.d.d
-00003740: 0269 0164 1864 198d 0201 007c 01a0 097c  .i.d.d.....|...|
-00003750: 006a 0a64 0b64 1067 0217 00a1 01a0 19a1  .j.d.d.g........
-00003760: 0064 1a17 007c 0164 083c 007c 016a 0864  .d...|.d.<.|.j.d
-00003770: 1067 0164 0a8d 017d 017c 0153 0029 1b61  .g.d...}.|.S.).a
-00003780: 0d02 0000 496e 6665 7220 6661 6d69 6c79  ....Infer family
-00003790: 2063 6c75 7374 6572 732e 0a0a 2020 2020   clusters...    
-000037a0: 2020 2020 4669 7273 742c 2066 6f72 2065      First, for e
-000037b0: 6163 6820 7365 6e73 6974 6976 6520 636c  ach sensitive cl
-000037c0: 7573 7465 7220 7468 6174 2064 6f65 7320  uster that does 
-000037d0: 6e6f 7420 7265 6163 6820 6465 7369 7265  not reach desire
-000037e0: 6420 7365 6e73 6974 6976 6974 792c 2067  d sensitivity, g
-000037f0: 726f 7570 2070 7265 6369 7365 0a20 2020  roup precise.   
-00003800: 2020 2020 2063 6c75 7374 6572 7320 746f       clusters to
-00003810: 6765 7468 6572 2077 6974 6820 6120 7369  gether with a si
-00003820: 6e67 6c65 206c 696e 6b61 6765 2061 6c67  ngle linkage alg
-00003830: 6f72 6974 686d 2e20 5468 6973 2067 726f  orithm. This gro
-00003840: 7570 696e 6720 6973 2064 6f6e 6520 6469  uping is done di
-00003850: 6666 6572 656e 746c 790a 2020 2020 2020  fferently.      
-00003860: 2020 6465 7065 6e64 696e 6720 6f6e 2077    depending on w
-00003870: 6865 7468 6572 2074 6865 2073 656e 7369  hether the sensi
-00003880: 7469 7665 2063 6c75 7374 6572 2069 7320  tive cluster is 
-00003890: 6c61 7267 6520 6f72 206e 6f74 2074 6f20  large or not to 
-000038a0: 7573 6520 7061 7261 6c6c 656c 697a 6174  use parallelizat
-000038b0: 696f 6e20 696e 2074 6865 0a20 2020 2020  ion in the.     
-000038c0: 2020 206d 6f73 7420 6566 6669 6369 656e     most efficien
-000038d0: 7420 7761 7920 706f 7373 6962 6c65 2e0a  t way possible..
-000038e0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000038f0: 2020 2020 2020 2020 2020 2064 6628 7064             df(pd
-00003900: 2e44 6174 6146 7261 6d65 293a 4461 7461  .DataFrame):Data
-00003910: 6672 616d 6520 6f66 2073 6571 7565 6e63  frame of sequenc
-00003920: 6573 2e0a 0a20 2020 2020 2020 2052 6574  es...        Ret
-00003930: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00003940: 2020 6466 2870 642e 4461 7461 4672 616d    df(pd.DataFram
-00003950: 6529 3a20 4461 7461 6672 616d 6520 7769  e): Dataframe wi
-00003960: 7468 2069 6e66 6572 7265 6420 636c 6f6e  th inferred clon
-00003970: 616c 2066 616d 696c 6965 7320 696e 2027  al families in '
-00003980: 6661 6d69 6c79 272e 0a20 2020 2020 2020  family'..       
-00003990: 2072 7a00 0000 7201 0000 007a 1a43 6865   rz...r....z.Che
-000039a0: 636b 696e 6720 616c 6967 6e6d 656e 7420  cking alignment 
-000039b0: 6c65 6e67 7468 2e29 0172 3f00 0000 72c8  length.).r?...r.
-000039c0: 0000 007a 2752 6574 7572 6e69 6e67 2063  ...z'Returning c
-000039d0: 6472 3320 6d65 7468 6f64 2070 7265 6369  dr3 method preci
-000039e0: 7365 2063 6c75 7374 6572 732e 72b1 0000  se clusters.r...
-000039f0: 00da 0666 616d 696c 7972 2f00 0000 72a1  ...familyr/...r.
-00003a00: 0000 0072 bd00 0000 7a2b 496e 6665 7272  ...r....z+Inferr
-00003a10: 696e 6720 6661 6d69 6c79 2063 6c75 7374  ing family clust
-00003a20: 6572 7320 666f 7220 736d 616c 6c20 6772  ers for small gr
-00003a30: 6f75 7073 2e63 0100 0000 0000 0000 0000  oups.c..........
-00003a40: 0000 0200 0000 0600 0000 1300 0001 731a  ..............s.
-00003a50: 0000 0067 007c 005d 127d 017c 0188 00a0  ...g.|.].}.|....
-00003a60: 007c 01a1 0166 0291 0271 0453 0072 1600  .|...f...q.S.r..
-00003a70: 0000 2901 72cb 0000 0072 cc00 0000 a901  ..).r....r......
-00003a80: 72d7 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00003a90: d000 0000 1102 0000 72d1 0000 007a 2048  ........r....z H
-00003aa0: 494c 4152 792e 696e 6665 722e 3c6c 6f63  ILARy.infer.<loc
-00003ab0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00003ac0: 3400 0000 5a0e 6661 6d69 6c79 5f63 6c75  4...Z.family_clu
-00003ad0: 7374 6572 7a2b 496e 6665 7272 696e 6720  sterz+Inferring 
-00003ae0: 6661 6d69 6c79 2063 6c75 7374 6572 7320  family clusters 
-00003af0: 666f 7220 6c61 7267 6520 6772 6f75 7073  for large groups
-00003b00: 2e72 b000 0000 72a0 0000 0029 0472 1c00  .r....r....).r..
-00003b10: 0000 727a 0000 0072 7b00 0000 72b1 0000  ..rz...r{...r...
-00003b20: 0029 0472 2b00 0000 723f 0000 0072 2c00  .).r+...r?...r,.
-00003b30: 0000 7213 0000 0029 0372 a800 0000 7268  ..r....).r....rh
-00003b40: 0000 0072 a900 0000 da09 6e65 775f 696e  ...r......new_in
-00003b50: 6465 7854 72d2 0000 0072 0e00 0000 291a  dexTr....r....).
-00003b60: 72dc 0000 0072 7d00 0000 7224 0000 0072  r....r}...r$...r
-00003b70: 3f00 0000 72c4 0000 00da 0564 6562 7567  ?...r......debug
-00003b80: 728c 0000 0072 c500 0000 da04 6472 6f70  r....r......drop
-00003b90: 7236 0000 0072 3200 0000 720b 0000 0072  r6...r2...r....r
-00003ba0: b700 0000 7233 0000 0072 1300 0000 727c  ....r3...r....r|
-00003bb0: 0000 0072 7e00 0000 723e 0000 0072 cb00  ...r~...r>...r..
-00003bc0: 0000 7276 0000 0072 af00 0000 7227 0000  ..rv...r....r'..
-00003bd0: 00da 0675 7064 6174 6572 d600 0000 7226  ...updater....r&
-00003be0: 0000 0072 3700 0000 290e 7215 0000 0072  ...r7...).r....r
-00003bf0: 2c00 0000 72db 0000 0072 da00 0000 5a0a  ,...r....r....Z.
-00003c00: 6c61 7267 655f 6469 6374 72ce 0000 0072  large_dictr....r
-00003c10: 2100 0000 7222 0000 0072 2b00 0000 72bd  !...r"...r+...r.
-00003c20: 0000 0072 a000 0000 da02 646d 726f 0000  ...r......dmro..
-00003c30: 0072 2e00 0000 7216 0000 0072 de00 0000  .r....r....r....
-00003c40: 7217 0000 0072 3900 0000 f301 0000 737a  r....r9.......sz
-00003c50: 0000 0000 0e10 0114 0110 010c 010a 010c  ................
-00003c60: 0104 0202 ff02 ff06 0504 0212 010a 0102  ................
-00003c70: 0110 0104 0104 0104 fc0a 060a 0104 0108  ................
-00003c80: 010c 0106 0102 ff02 0202 fe04 0202 fe04  ................
-00003c90: 0302 0102 0104 0108 0106 ff02 0804 f506  ................
-00003ca0: 0d08 0104 010a 0102 0108 fd06 050c 020a  ................
-00003cb0: 0108 010c ff08 0312 0204 010c ff06 0302  ................
-00003cc0: fd02 ff06 0604 0202 ff02 ff06 057a 0c48  .............z.H
-00003cd0: 494c 4152 792e 696e 6665 724e 2901 4629  ILARy.inferN).F)
-00003ce0: 0272 c000 0000 721d 0000 0029 0172 4100  .r....r....).rA.
-00003cf0: 0000 290e 723a 0000 0072 3b00 0000 723c  ..).r:...r;...r<
-00003d00: 0000 0072 3d00 0000 7218 0000 0072 9d00  ...r=...r....r..
-00003d10: 0000 72a7 0000 0072 af00 0000 72b7 0000  ..r....r....r...
-00003d20: 0072 bf00 0000 72c7 0000 0072 c900 0000  .r....r....r....
-00003d30: 72dc 0000 0072 3900 0000 7216 0000 0072  r....r9...r....r
-00003d40: 1600 0000 7216 0000 0072 1700 0000 7277  ....r....r....rw
-00003d50: 0000 00cc 0000 0073 1c00 0000 0801 0402  .......s........
-00003d60: 121f 0823 0831 1417 1039 1017 0001 00fc  ...#.1...9......
-00003d70: 161e 100f 00fd 1223 7277 0000 0029 2072  .......#rw...) r
-00003d80: 3d00 0000 da0a 5f5f 6675 7475 7265 5f5f  =.....__future__
-00003d90: 7202 0000 00da 0969 7465 7274 6f6f 6c73  r......itertools
-00003da0: 7203 0000 00da 0f6d 756c 7469 7072 6f63  r......multiproc
-00003db0: 6573 7369 6e67 7204 0000 00da 056e 756d  essingr......num
-00003dc0: 7079 724f 0000 00da 0670 616e 6461 7372  pyrO.....pandasr
-00003dd0: a300 0000 da09 7374 7275 6374 6c6f 675a  ......structlogZ
-00003de0: 0761 7472 6965 6763 7205 0000 0072 1e00  .atriegcr....r..
-00003df0: 0000 5a17 7363 6970 792e 636c 7573 7465  ..Z.scipy.cluste
-00003e00: 722e 6869 6572 6172 6368 7972 0600 0000  r.hierarchyr....
-00003e10: 7207 0000 005a 1673 6369 7079 2e73 7061  r....Z.scipy.spa
-00003e20: 7469 616c 2e64 6973 7461 6e63 6572 0800  tial.distancer..
-00003e30: 0000 da0c 7465 7874 6469 7374 616e 6365  ....textdistance
-00003e40: 7209 0000 00da 0e68 696c 6172 792e 6170  r......hilary.ap
-00003e50: 7269 6f72 6972 0a00 0000 da0c 6869 6c61  riorir......hila
-00003e60: 7279 2e75 7469 6c73 720b 0000 0072 0c00  ry.utilsr....r..
-00003e70: 0000 da0a 6765 745f 6c6f 6767 6572 72c4  ....get_loggerr.
-00003e80: 0000 0072 0d00 0000 723e 0000 0072 7700  ...r....r>...rw.
-00003e90: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00003ea0: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00003eb0: 0100 0000 7320 0000 0004 020c 020c 010c  ....s ..........
-00003ec0: 0208 0108 0108 010c 0110 010c 010c 020c  ................
-00003ed0: 0110 0408 030e 430e 71                   ......C.q
+00001cc0: 0d74 036a 086a 097c 0b64 0464 0785 0219  .t.j.j.|.d.d....
+00001cd0: 007c 0264 087c 0c64 098d 047d 0e7c 0d7c  .|.d.|.d...}.|.|
+00001ce0: 0e14 007c 071b 007d 0f74 036a 086a 0a7c  ...|...}.t.j.j.|
+00001cf0: 0f7c 0264 0a8d 027d 1074 03a0 0b7c 0fa1  .|.d...}.t...|..
+00001d00: 017d 117c 107c 0f18 007c 111b 007d 127c  .}.|.|...|...}.|
+00001d10: 006a 0c6a 0d7c 006a 0c64 0b19 007c 046b  .j.j.|.j.d...|.k
+00001d20: 0219 006a 0e64 0364 047c 0464 0417 0085  ...j.d.d.|.d....
+00001d30: 0266 0219 007d 1374 036a 0f7c 1364 0367  .f...}.t.j.|.d.g
+00001d40: 0164 0467 0164 0c8d 037d 1474 036a 086a  .d.g.d...}.t.j.j
+00001d50: 0974 03a0 047c 0464 0417 00a1 017c 0264  .t...|.d.....|.d
+00001d60: 087c 147c 14a0 07a1 001b 0064 098d 047d  .|.|.......d...}
+00001d70: 1574 03a0 107c 0d7c 0e17 0064 0d7c 1014  .t...|.|...d.|..
+00001d80: 0018 0064 03a1 027d 167c 047c 071b 007c  ...d...}.|.|...|
+00001d90: 1664 0417 0014 007d 1774 03a0 0b7c 177c  .d.....}.t...|.|
+00001da0: 047c 0717 0014 007c 071b 00a1 017d 187c  .|.....|.....}.|
+00001db0: 157c 1718 007c 181b 007d 197c 197c 1218  .|...|...}.|.|..
+00001dc0: 007d 1a74 03a0 117c 1aa1 0174 1274 007c  .}.t...|...t.t.|
+00001dd0: 0274 137c 0583 0114 0083 017c 0264 0418  .t.|.......|.d..
+00001de0: 0083 0219 007c 0866 0253 0029 0e4e 6700  .....|.f.S.).Ng.
+00001df0: 0000 0080 842e 41e9 6400 0000 7201 0000  ......A.d...r...
+00001e00: 0072 0f00 0000 2901 da04 6269 6e73 7243  .r....)...binsrC
+00001e10: 0000 0072 1e00 0000 5429 03da 0473 697a  ...r....T)...siz
+00001e20: 65da 0772 6570 6c61 6365 da01 7029 02da  e..replace..p)..
+00001e30: 036c 616d 7286 0000 0072 2c00 0000 2902  .lamr....r,...).
+00001e40: da07 7072 6570 656e 6472 6800 0000 7241  ..prependrh...rA
+00001e50: 0000 0029 1472 1100 0000 7283 0000 0072  ...).r....r....r
+00001e60: 7e00 0000 7250 0000 00da 0661 7261 6e67  ~...rP.....arang
+00001e70: 6572 4b00 0000 da09 6869 7374 6f67 7261  erK.....histogra
+00001e80: 6dda 0373 756d da06 7261 6e64 6f6d da06  m..sum..random..
+00001e90: 6368 6f69 6365 da07 706f 6973 736f 6e72  choice..poissonr
+00001ea0: 5100 0000 7282 0000 0072 2100 0000 7225  Q...r....r!...r%
+00001eb0: 0000 00da 0464 6966 66da 076d 6178 696d  .....diff..maxim
+00001ec0: 756d da04 736f 7274 7266 0000 0072 0d00  um..sortrf...r..
+00001ed0: 0000 291b 7216 0000 0072 1c00 0000 7286  ..).r....r....r.
+00001ee0: 0000 00da 015f 722c 0000 00da 0a70 7265  ....._r,.....pre
+00001ef0: 7661 6c65 6e63 65da 096d 7574 6174 696f  valence..mutatio
+00001f00: 6e73 7240 0000 00da 0863 6c61 7373 5f69  nsr@.....class_i
+00001f10: 6472 8500 0000 5a03 706e 695a 036e 6973  dr....Z.pniZ.nis
+00001f20: 7288 0000 005a 036e 3173 5a03 6e32 7372  r....Z.n1sZ.n2sr
+00001f30: 5e00 0000 5a03 6e30 7372 5f00 0000 da02  ^...Z.n0sr_.....
+00001f40: 7973 da03 6364 66da 0270 6eda 026e 735a  ys..cdf..pn..nsZ
+00001f50: 036e 4c73 725c 0000 0072 5d00 0000 da02  .nLsr\...r].....
+00001f60: 7873 da02 7a73 7217 0000 0072 1700 0000  xs..zsr....r....
+00001f70: 7218 0000 00da 0e73 696d 756c 6174 655f  r......simulate_
+00001f80: 7873 5f79 73ee 0000 0073 3a00 0000 0004  xs_ys....s:.....
+00001f90: 0801 1201 0801 1601 0801 1401 1201 1c01  ................
+00001fa0: 0c01 0801 1c01 1c01 0c01 1001 0a01 0c02  ................
+00001fb0: 2801 1401 0601 1aff 0603 1801 1001 1601  (...............
+00001fc0: 0c01 0802 2201 02fe 7a15 4849 4c41 5279  ...."...z.HILARy
+00001fd0: 2e73 696d 756c 6174 655f 7873 5f79 7363  .simulate_xs_ysc
+00001fe0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
+00001ff0: 0a00 0000 4300 0001 73ba 0000 0074 007c  ....C...s....t.|
+00002000: 0164 0119 006a 0164 0219 0083 017d 0267  .d...j.d.....}.g
+00002010: 007d 0374 027c 006a 0367 0064 03a2 0119  .}.t.|.j.g.d....
+00002020: 006a 0183 0144 005d 4c5c 057d 047d 057d  .j...D.]L\.}.}.}
+00002030: 067d 077d 087c 0464 046b 0272 507c 01a0  .}.}.|.d.k.rP|..
+00002040: 0464 05a1 0164 0619 007d 096e 0e7c 01a0  .d...d...}.n.|..
+00002050: 0464 07a1 0164 0619 007d 097c 03a0 057c  .d...d...}.|...|
+00002060: 047c 057c 067c 077c 097c 027c 0866 07a1  .|.|.|.|.|.|.f..
+00002070: 0101 0071 2a74 067c 037c 006a 077c 006a  ...q*t.|.|.j.|.j
+00002080: 087c 006a 0964 0864 098d 057d 0a74 0a6a  .|.j.d.d...}.t.j
+00002090: 0b7c 0a64 0a64 0b67 0264 0c8d 02a0 0c64  .|.d.d.g.d.....d
+000020a0: 0ba1 017d 0b7c 0b64 0a19 007c 006a 0364  ...}.|.d...|.j.d
+000020b0: 0a3c 0064 0053 0029 0d4e 727b 0000 0072  .<.d.S.).Nr{...r
+000020c0: 0100 0000 2905 7222 0000 0072 2300 0000  ....).r"...r#...
+000020d0: 7224 0000 00da 1465 6666 6563 7469 7665  r$.....effective
+000020e0: 5f70 7265 7661 6c65 6e63 6572 9700 0000  _prevalencer....
+000020f0: 7212 0000 007a 1963 6472 335f 6c65 6e67  r....z.cdr3_leng
+00002100: 7468 3d3d 4063 6472 335f 6c65 6e67 7468  th==@cdr3_length
+00002110: 727c 0000 007a 4176 5f67 656e 653d 3d40  r|...zAv_gene==@
+00002120: 765f 6765 6e65 2061 6e64 206a 5f67 656e  v_gene and j_gen
+00002130: 653d 3d40 6a5f 6765 6e65 2061 6e64 2063  e==@j_gene and c
+00002140: 6472 335f 6c65 6e67 7468 3d3d 4063 6472  dr3_length==@cdr
+00002150: 335f 6c65 6e67 7468 5429 0372 3600 0000  3_lengthT).r6...
+00002160: 7234 0000 00da 0569 7369 6e74 da0c 7879  r4.....isint..xy
+00002170: 5f74 6872 6573 686f 6c64 7297 0000 00a9  _thresholdr.....
+00002180: 01da 0763 6f6c 756d 6e73 290d 727e 0000  ...columns).r~..
+00002190: 0072 2500 0000 720a 0000 0072 7d00 0000  .r%...r....r}...
+000021a0: 727f 0000 0072 6800 0000 720c 0000 0072  r....rh...r....r
+000021b0: 9e00 0000 7214 0000 0072 3400 0000 da02  ....r....r4.....
+000021c0: 7064 da09 4461 7461 4672 616d 65da 0973  pd..DataFrame..s
+000021d0: 6574 5f69 6e64 6578 290c 7216 0000 0072  et_index).r....r
+000021e0: 2d00 0000 7240 0000 005a 116d 7574 6174  -...r@...Z.mutat
+000021f0: 696f 6e73 5f67 726f 7570 6564 7222 0000  ions_groupedr"..
+00002200: 0072 2300 0000 7224 0000 0072 9500 0000  .r#...r$...r....
+00002210: 7297 0000 0072 9600 0000 da06 7265 7375  r....r......resu
+00002220: 6c74 5a0f 7468 7265 7368 6f6c 6473 5f64  ltZ.thresholds_d
+00002230: 6174 6172 1700 0000 7217 0000 0072 1800  atar....r....r..
+00002240: 0000 da11 6765 745f 7879 5f74 6872 6573  ....get_xy_thres
+00002250: 686f 6c64 7312 0100 0073 5600 0000 0001  holds....sV.....
+00002260: 1201 0407 0201 0401 06ff 04ff 02fa 0601  ................
+00002270: 0201 0201 0201 0201 020c 0801 1002 0401  ................
+00002280: 02ff 0202 02fe 0403 0402 0201 0201 0201  ................
+00002290: 0201 0201 0201 02f9 02ff 060c 0201 0201  ................
+000022a0: 0401 0401 0401 02fb 0608 0401 08ff 0602  ................
+000022b0: 02fe 0403 7a18 4849 4c41 5279 2e67 6574  ....z.HILARy.get
+000022c0: 5f78 795f 7468 7265 7368 6f6c 6473 7272  _xy_thresholdsrr
+000022d0: 0000 0072 4d00 0000 7a0e 6469 6374 5b69  ...rM...z.dict[i
+000022e0: 6e74 2c20 696e 745d 2904 da07 696e 6469  nt, int])...indi
+000022f0: 6365 7372 6900 0000 da09 7468 7265 7368  cesri.....thresh
+00002300: 6f6c 6472 1500 0000 6304 0000 0000 0000  oldr....c.......
+00002310: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+00002320: 0173 2400 0000 7400 7401 7c02 6401 6402  .s$...t.t.|.d.d.
+00002330: 8d02 6403 7c03 6404 8d03 7d04 7402 7403  ..d.|.d...}.t.t.
+00002340: 7c01 7c04 8302 8301 5300 2905 61b2 0100  |.|.....S.).a...
+00002350: 004d 6170 2070 7265 6369 7365 2063 6c75  .Map precise clu
+00002360: 7374 6572 7320 746f 206e 6577 2070 7265  sters to new pre
+00002370: 6369 7365 2041 4e44 2073 656e 7369 7469  cise AND sensiti
+00002380: 7665 2063 6c75 7374 6572 7320 6279 206d  ve clusters by m
+00002390: 6572 6769 6e67 2063 6c75 7374 6572 7320  erging clusters 
+000023a0: 746f 6765 7468 6572 2e0a 0a20 2020 2020  together...     
+000023b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000023c0: 2020 2020 2069 6e64 6963 6573 2028 6e70       indices (np
+000023d0: 2e61 7272 6179 293a 2049 6e64 6963 6573  .array): Indices
+000023e0: 206f 6620 7072 6563 6973 6520 636c 7573   of precise clus
+000023f0: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
+00002400: 2020 6469 7374 2028 6e70 2e6e 6461 7272    dist (np.ndarr
+00002410: 6179 293a 2044 6973 7461 6e63 6573 2062  ay): Distances b
+00002420: 6574 7765 656e 2070 7265 6369 7365 2063  etween precise c
+00002430: 6c75 7374 6572 732e 0a20 2020 2020 2020  lusters..       
+00002440: 2020 2020 2074 6872 6573 686f 6c64 2028       threshold (
+00002450: 666c 6f61 7429 3a20 5468 7265 7368 6f6c  float): Threshol
+00002460: 6420 746f 206d 6572 6765 2074 776f 2070  d to merge two p
+00002470: 7265 6369 7365 2063 6c75 7374 6572 7320  recise clusters 
+00002480: 6966 2074 6865 2064 6973 7461 6e63 6520  if the distance 
+00002490: 6973 2073 6d61 6c6c 6572 2e0a 0a20 2020  is smaller...   
+000024a0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+000024b0: 2020 2020 2020 2020 2020 6469 6374 3a20            dict: 
+000024c0: 4469 6374 696f 6e61 7279 206d 6170 7069  Dictionary mappi
+000024d0: 6e67 2070 7265 6369 7365 2063 6c75 7374  ng precise clust
+000024e0: 6572 7320 746f 2074 6865 6972 206e 6577  ers to their new
+000024f0: 2063 6c75 7374 6572 732e 0a20 2020 2020   clusters..     
+00002500: 2020 20da 0673 696e 676c 6529 01da 066d     ..single)...m
+00002510: 6574 686f 64da 0864 6973 7461 6e63 6529  ethod..distance)
+00002520: 025a 0963 7269 7465 7269 6f6e 722e 0000  .Z.criterionr...
+00002530: 0029 0472 0600 0000 7207 0000 00da 0464  .).r....r......d
+00002540: 6963 74da 037a 6970 2905 7216 0000 0072  ict..zip).r....r
+00002550: a900 0000 7269 0000 0072 aa00 0000 7226  ....ri...r....r&
+00002560: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00002570: 0000 da0d 7369 6e67 6c65 4c69 6e6b 6167  ....singleLinkag
+00002580: 6545 0100 0073 0c00 0000 0010 0201 0a01  eE...s..........
+00002590: 0201 02fd 0605 7a14 4849 4c41 5279 2e73  ......z.HILARy.s
+000025a0: 696e 676c 654c 696e 6b61 6765 7a2e 7475  ingleLinkagez.tu
+000025b0: 706c 655b 7475 706c 655b 7374 722c 2073  ple[tuple[str, s
+000025c0: 7472 2c20 696e 742c 2069 6e74 5d2c 2070  tr, int, int], p
+000025d0: 642e 4461 7461 4672 616d 655d 721a 0000  d.DataFrame]r...
+000025e0: 0072 1b00 0000 6302 0000 0000 0000 0000  .r....c.........
+000025f0: 0000 0021 0000 0006 0000 0043 0000 0173  ...!.......C...s
+00002600: e001 0000 7c01 6401 1900 7d02 7c01 6402  ....|.d...}.|.d.
+00002610: 1900 5c04 7d03 7d04 7d05 7d06 7c00 6a00  ..\.}.}.}.}.|.j.
+00002620: a001 6403 a101 6404 1900 6a02 6402 1900  ..d...d...j.d...
+00002630: 7d07 7403 a004 7c02 6405 1900 a101 7d08  }.t...|.d.....}.
+00002640: 7405 7c08 8301 6401 6b01 7250 7c02 6405  t.|...d.k.rP|.d.
+00002650: 1900 5300 7406 7407 7c08 7408 7405 7c08  ..S.t.t.|.t.t.|.
+00002660: 8301 8301 8302 8301 7d09 7c02 6405 1900  ........}.|.d...
+00002670: a009 7c09 a101 7c02 6406 3c00 7405 7c08  ..|...|.d.<.t.|.
+00002680: 8301 7d0a 7403 6a0a 7c0a 7c0a 6602 740b  ..}.t.j.|.|.f.t.
+00002690: 6407 8d02 6408 7c00 6a0c 1400 1400 7d0b  d...d.|.j.....}.
+000026a0: 7408 7c0a 8301 4400 5d10 7d0c 6402 7c0b  t.|...D.].}.d.|.
+000026b0: 7c0c 7c0c 6602 3c00 71a4 740d 7c02 7c00  |.|.f.<.q.t.|.|.
+000026c0: 6a0e 1900 6a02 6408 8302 4400 5dee 5c02  j...j.d...D.].\.
+000026d0: 5c04 7d0d 7d0e 7d0f 7d10 5c04 7d11 7d12  \.}.}.}.}.\.}.}.
+000026e0: 7d13 7d14 7c10 7c14 6b03 72c8 7c0f 7c13  }.}.|.|.k.r.|.|.
+000026f0: 1400 7d15 7c15 6402 6b04 72c8 740f 7c0d  ..}.|.d.k.r.t.|.
+00002700: 7c11 8302 7d16 740f 7c0e 7c12 8302 7d17  |...}.t.|.|...}.
+00002710: 7c0f 7c13 1700 7c17 1800 6408 1b00 7d18  |.|...|...d...}.
+00002720: 7c05 7c00 6a0c 1b00 7c17 6401 1700 1400  |.|.j...|.d.....
+00002730: 7d19 7403 a010 7c19 7c05 7c00 6a0c 1700  }.t...|.|.|.j...
+00002740: 1400 7c00 6a0c 1b00 a101 7d1a 7c15 7c00  ..|.j.....}.|.|.
+00002750: 6a0c 1b00 7d1b 7403 a010 7c1b a101 7d1c  j...}.t...|...}.
+00002760: 7c16 7c19 1800 7c1a 1b00 7d1d 7c18 7c1b  |.|...|...}.|.|.
+00002770: 1800 7c1c 1b00 7d1e 7c1d 7c1e 1800 7c00  ..|...}.|.|...|.
+00002780: 6a0c 1700 7d1f 7411 7c1f 7c0b 7c10 7c14  j...}.t.|.|.|.|.
+00002790: 6602 1900 8302 7c0b 7c10 7c14 6602 3c00  f.....|.|.|.f.<.
+000027a0: 7411 7c1f 7c0b 7c14 7c10 6602 1900 8302  t.|.|.|.|.f.....
+000027b0: 7c0b 7c14 7c10 6602 3c00 71c8 7c00 6a12  |.|.|.f.<.q.|.j.
+000027c0: 7c08 7413 7c0b 8301 7c00 6a0c 7c07 1700  |.t.|...|.j.|...
+000027d0: 6409 8d03 7d20 7c02 6405 1900 a009 7c20  d...} |.d.....| 
+000027e0: a101 5300 290a 611e 0100 0047 726f 7570  ..S.).a....Group
+000027f0: 2070 7265 6369 7365 2063 6c75 7374 6572   precise cluster
+00002800: 7320 746f 6765 7468 6572 2e0a 0a20 2020  s together...   
+00002810: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00002820: 2020 2020 2020 2061 7267 7320 2854 7570         args (Tup
+00002830: 6c65 5b54 7570 6c65 5b73 7472 2c73 7472  le[Tuple[str,str
+00002840: 2c69 6e74 2c69 6e74 5d2c 7064 2e44 6174  ,int,int],pd.Dat
+00002850: 6146 7261 6d65 5d29 3a20 2856 6765 6e65  aFrame]): (Vgene
+00002860: 2c4a 6765 6e65 2c63 6472 336c 656e 6774  ,Jgene,cdr3lengt
+00002870: 6829 2c64 6174 6166 7261 6d65 0a20 2020  h),dataframe.   
+00002880: 2020 2020 2020 2020 2072 6570 7265 7365           represe
+00002890: 6e74 696e 6720 7365 6e73 6974 6976 6520  nting sensitive 
+000028a0: 636c 7573 7465 722e 0a0a 2020 2020 2020  cluster...      
+000028b0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000028c0: 2020 2020 2020 2070 642e 5365 7269 6573         pd.Series
+000028d0: 3a20 4e65 7720 636c 7573 7465 7273 206d  : New clusters m
+000028e0: 6164 6520 6f66 2067 726f 7570 6564 2070  ade of grouped p
+000028f0: 7265 6369 7365 2063 6c75 7374 6572 732e  recise clusters.
+00002900: 0a20 2020 2020 2020 2072 0f00 0000 7201  .        r....r.
+00002910: 0000 00fa 3776 5f67 656e 653d 3d40 765f  ....7v_gene==@v_
+00002920: 6765 6e65 2061 6e64 206a 5f67 656e 653d  gene and j_gene=
+00002930: 3d40 6a5f 6765 6e65 2061 6e64 2063 6472  =@j_gene and cdr
+00002940: 335f 6c65 6e67 7468 3d3d 406c 72a1 0000  3_length==@lr...
+00002950: 00da 0f70 7265 6369 7365 5f63 6c75 7374  ...precise_clust
+00002960: 6572 7228 0000 0029 01da 0564 7479 7065  err(...)...dtype
+00002970: 7241 0000 0029 0172 aa00 0000 2914 727d  rA...).r....).r}
+00002980: 0000 0072 7f00 0000 7225 0000 0072 5000  ...r....r%...rP.
+00002990: 0000 da06 756e 6971 7565 727e 0000 0072  ....uniquer~...r
+000029a0: ae00 0000 72af 0000 0072 6700 0000 7227  ....r....rg...r'
+000029b0: 0000 00da 046f 6e65 7372 4d00 0000 7240  .....onesrM...r@
+000029c0: 0000 0072 0300 0000 7239 0000 0072 0900  ...r....r9...r..
+000029d0: 0000 7251 0000 0072 6600 0000 72b0 0000  ..rQ...rf...r...
+000029e0: 0072 0800 0000 2921 7216 0000 0072 1c00  .r....)!r....r..
+000029f0: 0000 722d 0000 0072 2200 0000 7223 0000  ..r-...r"...r#..
+00002a00: 0072 2c00 0000 7294 0000 0072 a100 0000  .r,...r....r....
+00002a10: 72a9 0000 005a 1074 7261 6e73 6c61 7465  r....Z.translate
+00002a20: 496e 6469 6365 73da 0364 696d 5a0e 6469  Indices..dimZ.di
+00002a30: 7374 616e 6365 4d61 7472 6978 726d 0000  stanceMatrixrm..
+00002a40: 0072 5200 0000 7253 0000 0072 5400 0000  .rR...rS...rT...
+00002a50: 7255 0000 0072 5600 0000 7257 0000 0072  rU...rV...rW...r
+00002a60: 5800 0000 7259 0000 005a 046e 316e 3272  X...rY...Z.n1n2r
+00002a70: 4900 0000 725a 0000 0072 5b00 0000 725c  I...rZ...r[...r\
+00002a80: 0000 0072 5d00 0000 725e 0000 0072 5f00  ...r]...r^...r_.
+00002a90: 0000 7260 0000 0072 6100 0000 72ad 0000  ..r`...ra...r...
+00002aa0: 00da 0273 6c72 1700 0000 7217 0000 0072  ...slr....r....r
+00002ab0: 1800 0000 da0b 636c 6173 7332 7061 6972  ......class2pair
+00002ac0: 735c 0100 0073 5800 0000 000d 0801 1001  s\...sX.........
+00002ad0: 0601 02ff 0202 02fe 0402 02fe 0404 0e01  ................
+00002ae0: 0c01 0802 1601 1201 0801 1c01 0c01 0e01  ................
+00002af0: 0201 0cff 1c03 0801 0801 0801 0a01 0a01  ................
+00002b00: 1002 1201 0401 12ff 0403 0a01 0a01 0c01  ................
+00002b10: 0c01 0e01 1a01 1c01 0401 0201 0601 08fd  ................
+00002b20: 0605 7a12 4849 4c41 5279 2e63 6c61 7373  ..z.HILARy.class
+00002b30: 3270 6169 7273 7210 0000 0029 0272 2d00  2pairsr....).r-.
+00002b40: 0000 7215 0000 0063 0200 0000 0000 0000  ..r....c........
+00002b50: 0000 0000 0400 0000 0400 0000 4300 0001  ............C...
+00002b60: 7364 0000 0074 007c 006a 017c 006a 0264  sd...t.|.j.|.j.d
+00002b70: 0167 0117 0019 007c 006a 0364 028d 027d  .g.....|.j.d...}
+00002b80: 0274 007c 006a 017c 006a 0264 0367 0117  .t.|.j.|.j.d.g..
+00002b90: 0019 007c 006a 0364 028d 027d 037c 026a  ...|.j.d...}.|.j
+00002ba0: 047c 017c 006a 0564 048d 027c 0164 053c  .|.|.j.d...|.d.<
+00002bb0: 007c 036a 047c 017c 006a 0564 048d 027c  .|.j.|.|.j.d...|
+00002bc0: 0164 063c 007c 0153 0029 07fa c249 6e66  .d.<.|.S.)...Inf
+00002bd0: 6572 2070 7265 6369 7365 2061 6e64 2073  er precise and s
+00002be0: 656e 7369 7469 7665 2063 6c75 7374 6572  ensitive cluster
+00002bf0: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00002c00: 3a0a 2020 2020 2020 2020 2020 2020 6466  :.            df
+00002c10: 2870 642e 4461 7461 4672 616d 6529 3a44  (pd.DataFrame):D
+00002c20: 6174 6166 7261 6d65 206f 6620 7365 7175  ataframe of sequ
+00002c30: 656e 6365 732e 0a0a 2020 2020 2020 2020  ences...        
+00002c40: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00002c50: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
+00002c60: 6520 7769 7468 2073 656e 7369 7469 7665  e with sensitive
+00002c70: 2061 6e64 2070 7265 6369 7365 2063 6c75   and precise clu
+00002c80: 7374 6572 732e 0a20 2020 2020 2020 20da  sters..        .
+00002c90: 1170 7265 6369 7365 5f74 6872 6573 686f  .precise_thresho
+00002ca0: 6c64 a901 7214 0000 00da 1373 656e 7369  ld..r......sensi
+00002cb0: 7469 7665 5f74 6872 6573 686f 6c64 a901  tive_threshold..
+00002cc0: 7234 0000 0072 b200 0000 da11 7365 6e73  r4...r......sens
+00002cd0: 6974 6976 655f 636c 7573 7465 7229 0672  itive_cluster).r
+00002ce0: 0e00 0000 727d 0000 0072 3300 0000 7214  ....r}...r3...r.
+00002cf0: 0000 0072 3a00 0000 7234 0000 0029 0472  ...r:...r4...).r
+00002d00: 1600 0000 722d 0000 00da 0470 7265 635a  ....r-.....precZ
+00002d10: 0473 656e 7372 1700 0000 7217 0000 0072  .sensr....r....r
+00002d20: 1800 0000 da1a 636f 6d70 7574 655f 7072  ......compute_pr
+00002d30: 6563 5f73 656e 735f 636c 7573 7465 7273  ec_sens_clusters
+00002d40: 9501 0000 7314 0000 0000 0902 0114 ff06  ....s...........
+00002d50: 0302 0110 0104 fe06 0414 0114 017a 2148  .............z!H
+00002d60: 494c 4152 792e 636f 6d70 7574 655f 7072  ILARy.compute_pr
+00002d70: 6563 5f73 656e 735f 636c 7573 7465 7273  ec_sens_clusters
+00002d80: e79a 9999 9999 99c9 3f72 1e00 0000 7211  ........?r....r.
+00002d90: 0000 0029 0472 2d00 0000 da14 6e6f 726d  ...).r-.....norm
+00002da0: 616c 697a 6564 5f74 6872 6573 686f 6c64  alized_threshold
+00002db0: da0f 6669 7865 645f 7468 7265 7368 6f6c  ..fixed_threshol
+00002dc0: 6472 1500 0000 6304 0000 0000 0000 0000  dr....c.........
+00002dd0: 0000 0005 0000 0004 0000 0043 0000 0173  ...........C...s
+00002de0: 8200 0000 7c03 6401 6b05 7224 7400 a001  ....|.d.k.r$t...
+00002df0: 6402 7c03 9b00 9d02 a101 0100 7c03 7c00  d.|.........|.|.
+00002e00: 6a02 6403 3c00 6e2a 7400 a001 6404 7c02  j.d.<.n*t...d.|.
+00002e10: 9b00 9d02 a101 0100 7c00 6a02 6405 1900  ........|.j.d...
+00002e20: 7c02 1400 a003 7404 a101 7c00 6a02 6403  |.....t...|.j.d.
+00002e30: 3c00 7405 7c00 6a02 7c00 6a06 6403 6701  <.t.|.j.|.j.d.g.
+00002e40: 1700 1900 7c00 6a07 6406 8d02 7d04 7c04  ....|.j.d...}.|.
+00002e50: 6a08 7c01 7c00 6a09 6407 8d02 7c01 6408  j.|.|.j.d...|.d.
+00002e60: 3c00 7c01 5300 2909 72b9 0000 0072 0100  <.|.S.).r....r..
+00002e70: 0000 7a2d 5573 696e 6720 6372 7564 6520  ..z-Using crude 
+00002e80: 6d65 7468 6f64 2077 6974 6820 6120 6669  method with a fi
+00002e90: 7865 6420 7468 7265 7368 6f6c 6420 6f66  xed threshold of
+00002ea0: 2072 aa00 0000 7a32 5573 696e 6720 6372   r....z2Using cr
+00002eb0: 7564 6520 6d65 7468 6f64 2077 6974 6820  ude method with 
+00002ec0: 6120 6e6f 726d 616c 697a 6564 2074 6872  a normalized thr
+00002ed0: 6573 686f 6c64 206f 6620 7224 0000 0072  eshold of r$...r
+00002ee0: bb00 0000 72bd 0000 00da 1363 7275 6465  ....r......crude
+00002ef0: 5f6d 6574 686f 645f 6661 6d69 6c79 290a  _method_family).
+00002f00: da03 6c6f 67da 0469 6e66 6f72 7d00 0000  ..log..infor}...
+00002f10: da06 6173 7479 7065 7211 0000 0072 0e00  ..astyper....r..
+00002f20: 0000 7233 0000 0072 1400 0000 723a 0000  ..r3...r....r:..
+00002f30: 0072 3400 0000 2905 7216 0000 0072 2d00  .r4...).r....r-.
+00002f40: 0000 72c2 0000 0072 c300 0000 72bf 0000  ..r....r....r...
+00002f50: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002f60: da1d 636f 6d70 7574 655f 6372 7564 655f  ..compute_crude_
+00002f70: 6d65 7468 6f64 5f63 6c75 7374 6572 73a9  method_clusters.
+00002f80: 0100 0073 1e00 0000 000e 0801 1001 0c02  ...s............
+00002f90: 0401 08ff 0404 0cff 0202 02fe 0a03 0201  ................
+00002fa0: 14ff 0603 1401 7a24 4849 4c41 5279 2e63  ......z$HILARy.c
+00002fb0: 6f6d 7075 7465 5f63 7275 6465 5f6d 6574  ompute_crude_met
+00002fc0: 686f 645f 636c 7573 7465 7273 6302 0000  hod_clustersc...
+00002fd0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002fe0: 0043 0000 0173 1000 0000 6401 7c01 6402  .C...s....d.|.d.
+00002ff0: 3c00 7c01 6402 1900 5300 2903 6105 0100  <.|.d...S.).a...
+00003000: 0046 6c61 6720 616c 6c20 696e 6469 6365  .Flag all indice
+00003010: 7320 6f66 2061 2073 656e 7369 7469 7665  s of a sensitive
+00003020: 2063 6c75 7374 6572 206e 6f74 2072 6561   cluster not rea
+00003030: 6368 696e 6720 6465 7369 7265 6420 7365  ching desired se
+00003040: 6e73 6974 6976 6974 792e 0a0a 2020 2020  nsitivity...    
+00003050: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00003060: 2020 2020 2020 6466 2028 7064 2e44 6174        df (pd.Dat
+00003070: 6146 7261 6d65 293a 2044 6174 6166 7261  aFrame): Datafra
+00003080: 6d65 2067 726f 7570 6564 2072 6570 7265  me grouped repre
+00003090: 7365 6e74 696e 6720 6769 7665 6e20 636c  senting given cl
+000030a0: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
+000030b0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000030c0: 2020 2020 2070 642e 5365 7269 6573 3a20       pd.Series: 
+000030d0: 5365 7269 6573 2066 6c61 6767 696e 6720  Series flagging 
+000030e0: 616c 6c20 696e 6469 6365 7320 6f66 2067  all indices of g
+000030f0: 6976 656e 2063 6c75 7374 6572 2e0a 2020  iven cluster..  
+00003100: 2020 2020 2020 54da 0a74 6f5f 7265 736f        T..to_reso
+00003110: 6c76 6572 1700 0000 2902 7216 0000 0072  lver....).r....r
+00003120: 2d00 0000 7217 0000 0072 1700 0000 7218  -...r....r....r.
+00003130: 0000 00da 0a6d 6172 6b5f 636c 6173 73c7  .....mark_class.
+00003140: 0100 0073 0400 0000 0009 0801 7a11 4849  ...s........z.HI
+00003150: 4c41 5279 2e6d 6172 6b5f 636c 6173 7372  LARy.mark_classr
+00003160: 4200 0000 7a2f 7475 706c 655b 7064 2e44  B...z/tuple[pd.D
+00003170: 6174 6146 7261 6d65 2c20 7064 2e44 6174  ataFrame, pd.Dat
+00003180: 6146 7261 6d65 2c20 7064 2e44 6174 6146  aFrame, pd.DataF
+00003190: 7261 6d65 5d29 02da 0e73 697a 655f 7468  rame])...size_th
+000031a0: 7265 7368 6f6c 6472 1500 0000 6303 0000  resholdr....c...
+000031b0: 0000 0000 0000 0000 0008 0000 0006 0000  ................
+000031c0: 0003 0000 0173 a000 0000 6401 8800 6402  .....s....d...d.
+000031d0: 3c00 8801 6a00 6a01 721c 7402 a003 6403  <...j.j.r.t...d.
+000031e0: a101 0100 6e3c 7404 8700 8701 6602 6404  ....n<t.....f.d.
+000031f0: 6405 8408 8801 6a00 4400 8301 8801 6a05  d.....j.D.....j.
+00003200: 6406 8801 6a06 6407 8d04 8800 6402 3c00  d...j.d.....d.<.
+00003210: 8800 6a07 6402 6401 6901 6406 6408 8d02  ..j.d.d.i.d.d...
+00003220: 0100 8800 a008 6409 a101 a009 8801 6a0a  ......d.......j.
+00003230: 640a 6701 1700 a101 7d03 7c03 a00b a100  d.g.....}.|.....
+00003240: 7d04 7c04 7c02 6b04 7d05 7c04 7c05 1900  }.|.|.k.}.|.|...
+00003250: 6a0c 7d06 7c04 7c05 0f00 1900 6a0c 7d07  j.}.|.|.....j.}.
+00003260: 8800 7c07 7c06 6603 5300 290b 6190 0100  ..|.|.f.S.).a...
+00003270: 0043 6c61 7373 6966 7920 7365 6e73 6974  .Classify sensit
+00003280: 6976 6520 636c 7573 7465 7273 206e 6f74  ive clusters not
+00003290: 2072 6561 6368 696e 6720 6465 7369 7265   reaching desire
+000032a0: 6420 7365 6e73 6974 6976 6974 7920 696e  d sensitivity in
+000032b0: 746f 2062 6967 206f 7220 736d 616c 6c20  to big or small 
+000032c0: 636c 7573 7465 722e 0a0a 2020 2020 2020  cluster...      
+000032d0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000032e0: 2020 2020 6466 2870 642e 4461 7461 4672      df(pd.DataFr
+000032f0: 616d 6529 3a44 6174 6166 7261 6d65 206f  ame):Dataframe o
+00003300: 6620 7365 7175 656e 6365 732e 0a20 2020  f sequences..   
+00003310: 2020 2020 2020 2020 2073 697a 655f 7468           size_th
+00003320: 7265 7368 6f6c 6420 2869 6e74 2c20 6f70  reshold (int, op
+00003330: 7469 6f6e 616c 293a 2054 6872 6573 686f  tional): Thresho
+00003340: 6c64 2074 6f20 7365 7061 7261 7465 2062  ld to separate b
+00003350: 6967 2061 6e64 2073 6d61 6c6c 2063 6c75  ig and small clu
+00003360: 7374 6572 732e 0a20 2020 2020 2020 2020  sters..         
+00003370: 2020 2044 6566 6175 6c74 7320 746f 2031     Defaults to 1
+00003380: 6533 2e0a 0a20 2020 2020 2020 2052 6574  e3...        Ret
+00003390: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000033a0: 2020 5475 706c 655b 7064 2e44 6174 6146    Tuple[pd.DataF
+000033b0: 7261 6d65 2c70 642e 4461 7461 4672 616d  rame,pd.DataFram
+000033c0: 655d 3a20 5265 7475 726e 7320 696e 6469  e]: Returns indi
+000033d0: 6365 7320 6f66 2073 6d61 6c6c 2061 6e64  ces of small and
+000033e0: 2062 6967 2073 656e 7369 7469 7665 2063   big sensitive c
+000033f0: 6c75 7374 6572 732e 0a20 2020 2020 2020  lusters..       
+00003400: 2046 72c9 0000 007a 1f4e 6f20 636c 6173   Fr....z.No clas
+00003410: 7365 7320 7061 7373 6564 2074 6f20 7879  ses passed to xy
+00003420: 206d 6574 686f 642e 6301 0000 0000 0000   method.c.......
+00003430: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00003440: 0173 1e00 0000 6700 7c00 5d16 7d01 8800  .s....g.|.].}...
+00003450: a000 8801 6a01 a101 a002 7c01 a101 9102  ....j.....|.....
+00003460: 7104 5300 7217 0000 0029 0372 3700 0000  q.S.r....).r7...
+00003470: 7233 0000 00da 0967 6574 5f67 726f 7570  r3.....get_group
+00003480: a902 da02 2e30 da01 67a9 0272 2d00 0000  .....0..g..r-...
+00003490: 7216 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+000034a0: 0a3c 6c69 7374 636f 6d70 3ee7 0100 00f3  .<listcomp>.....
+000034b0: 0000 0000 7a20 4849 4c41 5279 2e74 6f5f  ....z HILARy.to_
+000034c0: 646f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  do.<locals>.<lis
+000034d0: 7463 6f6d 703e 5472 3500 0000 a902 da05  tcomp>Tr5.......
+000034e0: 7661 6c75 65da 0769 6e70 6c61 6365 7a12  value..inplacez.
+000034f0: 746f 5f72 6573 6f6c 7665 203d 3d20 5472  to_resolve == Tr
+00003500: 7565 72be 0000 0029 0d72 8100 0000 da05  uer....).r......
+00003510: 656d 7074 7972 c500 0000 72c6 0000 0072  emptyr....r....r
+00003520: 0c00 0000 72ca 0000 0072 1400 0000 da06  ....r....r......
+00003530: 6669 6c6c 6e61 727f 0000 0072 3700 0000  fillnar....r7...
+00003540: 7233 0000 0072 8600 0000 7228 0000 0029  r3...r....r(...)
+00003550: 0872 1600 0000 722d 0000 0072 cb00 0000  .r....r-...r....
+00003560: da09 6466 4772 6f75 7065 64da 0573 697a  ..dfGrouped..siz
+00003570: 6573 da04 6d61 736b da0b 6c61 7267 655f  es..mask..large_
+00003580: 746f 5f64 6fda 0b73 6d61 6c6c 5f74 6f5f  to_do..small_to_
+00003590: 646f 7217 0000 0072 d000 0000 7218 0000  dor....r....r...
+000035a0: 00da 0574 6f5f 646f d301 0000 7324 0000  ...to_do....s$..
+000035b0: 0000 0f08 0108 010c 0202 0114 0104 0102  ................
+000035c0: 0104 fc0a 0612 010a 010a ff04 0308 0108  ................
+000035d0: 010a 010c 017a 0c48 494c 4152 792e 746f  .....z.HILARy.to
+000035e0: 5f64 6f72 7300 0000 6302 0000 0000 0000  _dors...c.......
+000035f0: 0000 0000 000e 0000 0007 0000 0003 0000  ................
+00003600: 0173 a201 0000 7c00 a000 7c01 a101 5c03  .s....|...|...\.
+00003610: 7d01 7d02 7d03 7401 7c01 6401 1900 6a02  }.}.}.t.|.d...j.
+00003620: 6402 1900 8301 7c00 5f03 7404 6a05 6403  d.....|._.t.j.d.
+00003630: 7c00 6a03 6404 8d02 0100 7406 7c01 6405  |.j.d.....t.|.d.
+00003640: 1900 8301 7368 7404 a007 6406 a101 0100  ....sht...d.....
+00003650: 7c01 6407 1900 7c01 6408 3c00 7c01 6a08  |.d...|.d.<.|.j.
+00003660: 6409 6701 640a 8d01 7d01 7c01 5300 7c01  d.g.d...}.|.S.|.
+00003670: a009 7c00 6a0a 640b 6701 1700 a101 8900  ..|.j.d.g.......
+00003680: 7404 a005 640c a101 0100 740b 8700 6601  t...d.....t...f.
+00003690: 640d 640e 8408 7c02 4400 8301 7c00 6a0c  d.d...|.D...|.j.
+000036a0: 7c00 6a0d 7c00 6a0e 640f 8d04 7c01 6410  |.j.|.j.d...|.d.
+000036b0: 3c00 7404 a005 6411 a101 0100 6900 7d04  <.t...d.....i.}.
+000036c0: 7c03 4400 5d78 7d05 7c05 5c04 7d06 7d07  |.D.]x}.|.\.}.}.
+000036d0: 7d08 7d09 7c00 6a0f a010 6412 a101 6413  }.}.|.j...d...d.
+000036e0: 1900 6a02 6402 1900 7d0a 7411 7c08 7c00  ..j.d...}.t.|.|.
+000036f0: 6a03 8800 a012 7c05 a101 6700 6414 a201  j.....|...g.d...
+00003700: 1900 7c00 6a0e 6415 8d04 7d0b 7c0b a013  ..|.j.d...}.|...
+00003710: a100 7d0c 7c00 6a14 8800 a012 7c05 a101  ..}.|.j.....|...
+00003720: 6a15 7c0c 7c00 6a03 7c0a 1700 6416 8d03  j.|.|.j.|...d...
+00003730: 7d0d 7c04 a016 7c0d a101 0100 71be 7c01  }.|...|.....q.|.
+00003740: 6a15 7c01 6417 3c00 7c01 6410 1900 a017  j.|.d.<.|.d.....
+00003750: 7c01 6417 1900 a018 7c04 a101 a101 7c01  |.d.....|.....|.
+00003760: 6410 3c00 7c01 6a17 6410 6402 6901 6418  d.<.|.j.d.d.i.d.
+00003770: 6419 8d02 0100 7c01 a009 7c00 6a0a 640b  d.....|...|.j.d.
+00003780: 6410 6702 1700 a101 a019 a100 641a 1700  d.g.........d...
+00003790: 7c01 6408 3c00 7c01 6a08 6410 6701 640a  |.d.<.|.j.d.g.d.
+000037a0: 8d01 7d01 7c01 5300 291b 610d 0200 0049  ..}.|.S.).a....I
+000037b0: 6e66 6572 2066 616d 696c 7920 636c 7573  nfer family clus
+000037c0: 7465 7273 2e0a 0a20 2020 2020 2020 2046  ters...        F
+000037d0: 6972 7374 2c20 666f 7220 6561 6368 2073  irst, for each s
+000037e0: 656e 7369 7469 7665 2063 6c75 7374 6572  ensitive cluster
+000037f0: 2074 6861 7420 646f 6573 206e 6f74 2072   that does not r
+00003800: 6561 6368 2064 6573 6972 6564 2073 656e  each desired sen
+00003810: 7369 7469 7669 7479 2c20 6772 6f75 7020  sitivity, group 
+00003820: 7072 6563 6973 650a 2020 2020 2020 2020  precise.        
+00003830: 636c 7573 7465 7273 2074 6f67 6574 6865  clusters togethe
+00003840: 7220 7769 7468 2061 2073 696e 676c 6520  r with a single 
+00003850: 6c69 6e6b 6167 6520 616c 676f 7269 7468  linkage algorith
+00003860: 6d2e 2054 6869 7320 6772 6f75 7069 6e67  m. This grouping
+00003870: 2069 7320 646f 6e65 2064 6966 6665 7265   is done differe
+00003880: 6e74 6c79 0a20 2020 2020 2020 2064 6570  ntly.        dep
+00003890: 656e 6469 6e67 206f 6e20 7768 6574 6865  ending on whethe
+000038a0: 7220 7468 6520 7365 6e73 6974 6976 6520  r the sensitive 
+000038b0: 636c 7573 7465 7220 6973 206c 6172 6765  cluster is large
+000038c0: 206f 7220 6e6f 7420 746f 2075 7365 2070   or not to use p
+000038d0: 6172 616c 6c65 6c69 7a61 7469 6f6e 2069  arallelization i
+000038e0: 6e20 7468 650a 2020 2020 2020 2020 6d6f  n the.        mo
+000038f0: 7374 2065 6666 6963 6965 6e74 2077 6179  st efficient way
+00003900: 2070 6f73 7369 626c 652e 0a0a 2020 2020   possible...    
+00003910: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00003920: 2020 2020 2020 6466 2870 642e 4461 7461        df(pd.Data
+00003930: 4672 616d 6529 3a44 6174 6166 7261 6d65  Frame):Dataframe
+00003940: 206f 6620 7365 7175 656e 6365 732e 0a0a   of sequences...
+00003950: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003960: 0a20 2020 2020 2020 2020 2020 2064 6628  .            df(
+00003970: 7064 2e44 6174 6146 7261 6d65 293a 2044  pd.DataFrame): D
+00003980: 6174 6166 7261 6d65 2077 6974 6820 696e  ataframe with in
+00003990: 6665 7272 6564 2063 6c6f 6e61 6c20 6661  ferred clonal fa
+000039a0: 6d69 6c69 6573 2069 6e20 2766 616d 696c  milies in 'famil
+000039b0: 7927 2e0a 2020 2020 2020 2020 727b 0000  y'..        r{..
+000039c0: 0072 0100 0000 7a1a 4368 6563 6b69 6e67  .r....z.Checking
+000039d0: 2061 6c69 676e 6d65 6e74 206c 656e 6774   alignment lengt
+000039e0: 682e 2901 7240 0000 0072 c900 0000 7a27  h.).r@...r....z'
+000039f0: 5265 7475 726e 696e 6720 6364 7233 206d  Returning cdr3 m
+00003a00: 6574 686f 6420 7072 6563 6973 6520 636c  ethod precise cl
+00003a10: 7573 7465 7273 2e72 b200 0000 da06 6661  usters.r......fa
+00003a20: 6d69 6c79 7230 0000 0072 a200 0000 72be  milyr0...r....r.
+00003a30: 0000 007a 2b49 6e66 6572 7269 6e67 2066  ...z+Inferring f
+00003a40: 616d 696c 7920 636c 7573 7465 7273 2066  amily clusters f
+00003a50: 6f72 2073 6d61 6c6c 2067 726f 7570 732e  or small groups.
+00003a60: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00003a70: 0006 0000 0013 0000 0173 1a00 0000 6700  .........s....g.
+00003a80: 7c00 5d12 7d01 7c01 8800 a000 7c01 a101  |.].}.|.....|...
+00003a90: 6602 9102 7104 5300 7217 0000 0029 0172  f...q.S.r....).r
+00003aa0: cc00 0000 72cd 0000 00a9 0172 d800 0000  ....r......r....
+00003ab0: 7217 0000 0072 1800 0000 72d1 0000 0014  r....r....r.....
+00003ac0: 0200 0072 d200 0000 7a20 4849 4c41 5279  ...r....z HILARy
+00003ad0: 2e69 6e66 6572 2e3c 6c6f 6361 6c73 3e2e  .infer.<locals>.
+00003ae0: 3c6c 6973 7463 6f6d 703e 7235 0000 005a  <listcomp>r5...Z
+00003af0: 0e66 616d 696c 795f 636c 7573 7465 727a  .family_clusterz
+00003b00: 2b49 6e66 6572 7269 6e67 2066 616d 696c  +Inferring famil
+00003b10: 7920 636c 7573 7465 7273 2066 6f72 206c  y clusters for l
+00003b20: 6172 6765 2067 726f 7570 732e 72b1 0000  arge groups.r...
+00003b30: 0072 a100 0000 2904 721d 0000 0072 7b00  .r....).r....r{.
+00003b40: 0000 727c 0000 0072 b200 0000 2904 722c  ..r|...r....).r,
+00003b50: 0000 0072 4000 0000 722d 0000 0072 1400  ...r@...r-...r..
+00003b60: 0000 2903 72a9 0000 0072 6900 0000 72aa  ..).r....ri...r.
+00003b70: 0000 00da 096e 6577 5f69 6e64 6578 5472  .....new_indexTr
+00003b80: d300 0000 720f 0000 0029 1a72 dd00 0000  ....r....).r....
+00003b90: 727e 0000 0072 2500 0000 7240 0000 0072  r~...r%...r@...r
+00003ba0: c500 0000 da05 6465 6275 6772 8d00 0000  ......debugr....
+00003bb0: 72c6 0000 00da 0464 726f 7072 3700 0000  r......dropr7...
+00003bc0: 7233 0000 0072 0c00 0000 72b8 0000 0072  r3...r....r....r
+00003bd0: 3400 0000 7214 0000 0072 7d00 0000 727f  4...r....r}...r.
+00003be0: 0000 0072 3f00 0000 72cc 0000 0072 7700  ...r?...r....rw.
+00003bf0: 0000 72b0 0000 0072 2800 0000 da06 7570  ..r....r(.....up
+00003c00: 6461 7465 72d7 0000 0072 2700 0000 7238  dater....r'...r8
+00003c10: 0000 0029 0e72 1600 0000 722d 0000 0072  ...).r....r-...r
+00003c20: dc00 0000 72db 0000 005a 0a6c 6172 6765  ....r....Z.large
+00003c30: 5f64 6963 7472 cf00 0000 7222 0000 0072  _dictr....r"...r
+00003c40: 2300 0000 722c 0000 0072 be00 0000 72a1  #...r,...r....r.
+00003c50: 0000 00da 0264 6d72 7000 0000 722f 0000  .....dmrp...r/..
+00003c60: 0072 1700 0000 72df 0000 0072 1800 0000  .r....r....r....
+00003c70: 723a 0000 00f6 0100 0073 7a00 0000 000e  r:.......sz.....
+00003c80: 1001 1401 1001 0c01 0a01 0c01 0402 02ff  ................
+00003c90: 02ff 0605 0402 1201 0a01 0201 1001 0401  ................
+00003ca0: 0401 04fc 0a06 0a01 0401 0801 0c01 0601  ................
+00003cb0: 02ff 0202 02fe 0402 02fe 0403 0201 0201  ................
+00003cc0: 0401 0801 06ff 0208 04f5 060d 0801 0401  ................
+00003cd0: 0a01 0201 08fd 0605 0c02 0a01 0801 0cff  ................
+00003ce0: 0803 1202 0401 0cff 0603 02fd 02ff 0606  ................
+00003cf0: 0402 02ff 02ff 0605 7a0c 4849 4c41 5279  ........z.HILARy
+00003d00: 2e69 6e66 6572 4e29 0146 2902 72c1 0000  .inferN).F).r...
+00003d10: 0072 1e00 0000 2901 7242 0000 0029 0e72  .r....).rB...).r
+00003d20: 3b00 0000 723c 0000 0072 3d00 0000 723e  ;...r<...r=...r>
+00003d30: 0000 0072 1900 0000 729e 0000 0072 a800  ...r....r....r..
+00003d40: 0000 72b0 0000 0072 b800 0000 72c0 0000  ..r....r....r...
+00003d50: 0072 c800 0000 72ca 0000 0072 dd00 0000  .r....r....r....
+00003d60: 723a 0000 0072 1700 0000 7217 0000 0072  r:...r....r....r
+00003d70: 1700 0000 7218 0000 0072 7800 0000 cd00  ....r....rx.....
+00003d80: 0000 731c 0000 0008 0104 0212 1e08 2408  ..s...........$.
+00003d90: 3314 1710 3910 1700 0100 fc16 1e10 0f00  3...9...........
+00003da0: fd12 2372 7800 0000 2921 723e 0000 00da  ..#rx...)!r>....
+00003db0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+00003dc0: da09 6974 6572 746f 6f6c 7372 0300 0000  ..itertoolsr....
+00003dd0: da0f 6d75 6c74 6970 726f 6365 7373 696e  ..multiprocessin
+00003de0: 6772 0400 0000 da05 6e75 6d70 7972 5000  gr......numpyrP.
+00003df0: 0000 da06 7061 6e64 6173 72a4 0000 00da  ....pandasr.....
+00003e00: 0973 7472 7563 746c 6f67 5a07 6174 7269  .structlogZ.atri
+00003e10: 6567 6372 0500 0000 721f 0000 005a 1773  egcr....r....Z.s
+00003e20: 6369 7079 2e63 6c75 7374 6572 2e68 6965  cipy.cluster.hie
+00003e30: 7261 7263 6879 7206 0000 0072 0700 0000  rarchyr....r....
+00003e40: 5a16 7363 6970 792e 7370 6174 6961 6c2e  Z.scipy.spatial.
+00003e50: 6469 7374 616e 6365 7208 0000 00da 0c74  distancer......t
+00003e60: 6578 7464 6973 7461 6e63 6572 0900 0000  extdistancer....
+00003e70: 720a 0000 00da 0e68 696c 6172 792e 6170  r......hilary.ap
+00003e80: 7269 6f72 6972 0b00 0000 da0c 6869 6c61  riorir......hila
+00003e90: 7279 2e75 7469 6c73 720c 0000 0072 0d00  ry.utilsr....r..
+00003ea0: 0000 da0a 6765 745f 6c6f 6767 6572 72c5  ....get_loggerr.
+00003eb0: 0000 0072 0e00 0000 723f 0000 0072 7800  ...r....r?...rx.
+00003ec0: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00003ed0: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00003ee0: 0100 0000 7322 0000 0004 020c 020c 010c  ....s"..........
+00003ef0: 0208 0108 0108 010c 0110 010c 010c 010c  ................
+00003f00: 020c 0110 0408 030e 430e 71              ........C.q
```

### Comparing `hilary-1.2.0/hilary/__pycache__/utils.cpython-39.pyc` & `hilary-1.2.1/hilary/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Mar  7 00:55:59 2024 UTC, .py size: 7992 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 9f10 e965 381f 0000  a..........e8...
+00000000: 610d 0d0a 0000 0000 468f 0166 8f20 0000  a.......F..f. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 2201 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
@@ -117,335 +117,342 @@
 00000740: 1c00 0000 721d 0000 00da 0f63 6f75 6e74  ....r......count
 00000750: 5f6d 7574 6174 696f 6e73 3400 0000 730a  _mutations4...s.
 00000760: 0000 0000 0908 010c 0106 0102 fe72 2a00  .............r*.
 00000770: 0000 da04 626f 6f6c 2904 da09 6461 7461  ....bool)...data
 00000780: 6672 616d 6572 1a00 0000 da07 7468 7265  framer......thre
 00000790: 6164 7372 1200 0000 6303 0000 0000 0000  adsr....c.......
 000007a0: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
-000007b0: 0173 fe00 0000 7c00 a000 a100 7d03 6700  .s....|.....}.g.
-000007c0: 6401 a201 7d04 6402 7c03 6a01 7601 7236  d...}.d.|.j.v.r6
-000007d0: 7c03 6403 1900 6a02 6a03 6404 6405 6406  |.d...j.j.d.d.d.
-000007e0: 8d02 7c03 6402 6407 6702 3c00 6408 7c03  ..|.d.d.g.<.d.|.
-000007f0: 6a01 7601 725c 7c03 6409 1900 6a02 6a03  j.v.r\|.d...j.j.
-00000800: 6404 6405 6406 8d02 7c03 6408 6407 6702  d.d.d...|.d.d.g.
-00000810: 3c00 640a 7c03 6a01 7601 727c 7c03 640b  <.d.|.j.v.r||.d.
-00000820: 1900 6a02 640c 640d 8502 1900 7c03 640a  ..j.d.d.....|.d.
-00000830: 3c00 7c03 640a 1900 6a02 a004 a100 7c03  <.|.d...j.....|.
-00000840: 640e 3c00 640f 7c03 6a01 7601 72ac 7c03  d.<.d.|.j.v.r.|.
-00000850: 6410 1900 7c03 6411 1900 1700 7c03 640f  d...|.d.....|.d.
-00000860: 3c00 6412 7c03 6a01 7601 72ca 7c03 6413  <.d.|.j.v.r.|.d.
-00000870: 1900 7c03 6414 1900 1700 7c03 6412 3c00  ..|.d.....|.d.<.
-00000880: 7405 7c03 a006 6700 6415 a201 a101 7407  t.|...g.d.....t.
-00000890: 7c01 7c02 6416 8d04 7c03 6417 3c00 7c03  |.|.d...|.d.<.|.
-000008a0: 7c04 1900 a008 640e 7409 6901 a101 a00a  |.....d.t.i.....
-000008b0: a100 5300 2918 614c 0100 0050 726f 6365  ..S.).aL...Proce
-000008c0: 7373 2069 6e70 7574 2064 6174 6166 7261  ss input datafra
-000008d0: 6d65 2e0a 0a20 2020 2041 7267 733a 0a20  me...    Args:. 
-000008e0: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-000008f0: 2028 7064 2e44 6174 6146 7261 6d65 293a   (pd.DataFrame):
-00000900: 2049 6e70 7574 2064 6174 6166 7261 6d65   Input dataframe
-00000910: 206f 6620 7365 7175 656e 6365 732e 0a20   of sequences.. 
-00000920: 2020 2020 2020 2073 696c 656e 7420 2862         silent (b
-00000930: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00000940: 446f 206e 6f74 2073 686f 7720 7072 6f67  Do not show prog
-00000950: 7265 7373 2062 6172 2069 6620 7472 7565  ress bar if true
-00000960: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00000970: 6c73 652e 0a20 2020 2020 2020 2074 6872  lse..        thr
-00000980: 6561 6473 2028 696e 742c 206f 7074 696f  eads (int, optio
-00000990: 6e61 6c29 3a20 4e75 6d62 6572 206f 6620  nal): Number of 
-000009a0: 6370 7573 206f 6e20 7768 6963 6820 746f  cpus on which to
-000009b0: 2072 756e 2063 6f64 652c 2064 6566 6175   run code, defau
-000009c0: 6c74 7320 746f 2031 2e0a 0a20 2020 2052  lts to 1...    R
-000009d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000009e0: 7064 2e44 6174 6166 7261 6d65 3a20 7072  pd.Dataframe: pr
-000009f0: 6f63 6573 7365 6420 6461 7461 6672 616d  ocessed datafram
-00000a00: 652e 0a20 2020 2029 08da 0b73 6571 7565  e..    )...seque
-00000a10: 6e63 655f 6964 da06 765f 6765 6e65 da06  nce_id..v_gene..
-00000a20: 6a5f 6765 6e65 da0b 6364 7233 5f6c 656e  j_gene..cdr3_len
-00000a30: 6774 68da 0463 6472 3372 2000 0000 7221  gth..cdr3r ...r!
-00000a40: 0000 00da 0e6d 7574 6174 696f 6e5f 636f  .....mutation_co
-00000a50: 756e 7472 2f00 0000 5a06 765f 6361 6c6c  untr/...Z.v_call
-00000a60: da01 2a54 2901 da06 6578 7061 6e64 7228  ..*T)...expandr(
-00000a70: 0000 0072 3000 0000 5a06 6a5f 6361 6c6c  ...r0...Z.j_call
-00000a80: 7232 0000 005a 086a 756e 6374 696f 6ee9  r2...Z.junction.
-00000a90: 0300 0000 e9fd ffff ff72 3100 0000 7220  .........r1...r 
-00000aa0: 0000 005a 1476 5f73 6571 7565 6e63 655f  ...Z.v_sequence_
-00000ab0: 616c 6967 6e6d 656e 745a 146a 5f73 6571  alignmentZ.j_seq
-00000ac0: 7565 6e63 655f 616c 6967 6e6d 656e 7472  uence_alignmentr
-00000ad0: 2100 0000 5a14 765f 6765 726d 6c69 6e65  !...Z.v_germline
-00000ae0: 5f61 6c69 676e 6d65 6e74 5a14 6a5f 6765  _alignmentZ.j_ge
-00000af0: 726d 6c69 6e65 5f61 6c69 676e 6d65 6e74  rmline_alignment
-00000b00: a903 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00000b10: 0029 0272 1a00 0000 7211 0000 0072 3300  .).r....r....r3.
-00000b20: 0000 290b da04 636f 7079 da07 636f 6c75  ..)...copy..colu
-00000b30: 6d6e 73da 0373 7472 da05 7370 6c69 7472  mns..str..splitr
-00000b40: 1600 0000 721e 0000 00da 0767 726f 7570  ....r......group
-00000b50: 6279 722a 0000 00da 0661 7374 7970 6572  byr*.....astyper
-00000b60: 0e00 0000 da06 6472 6f70 6e61 2905 722c  ......dropna).r,
-00000b70: 0000 0072 1a00 0000 722d 0000 0072 2900  ...r....r-...r).
-00000b80: 0000 da07 7573 6563 6f6c 7372 1c00 0000  ....usecolsr....
-00000b90: 721c 0000 0072 1d00 0000 da0a 7072 6570  r....r......prep
-00000ba0: 726f 6365 7373 4400 0000 732c 0000 0000  rocessD...s,....
-00000bb0: 0f08 0108 0a0a 011c 010a 011c 010a 0116  ................
-00000bc0: 0112 010a 020e ff06 040a 020e ff06 0402  ................
-00000bd0: 010c 0102 0102 0102 fc0a 0672 4100 0000  ...........rA...
-00000be0: 7a0c 7064 2e44 6174 6166 7261 6d65 2902  z.pd.Dataframe).
-00000bf0: 7229 0000 0072 1200 0000 6301 0000 0000  r)...r....c.....
-00000c00: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00000c10: 0000 0173 a600 0000 7c00 a000 6700 6401  ...s....|...g.d.
-00000c20: a201 a101 a001 a100 a002 6402 a101 a003  ..........d.....
-00000c30: a100 7d01 7c01 6402 1900 a004 6403 6404  ..}.|.d.....d.d.
-00000c40: 8400 a101 a005 7406 a101 7c01 6405 3c00  ......t...|.d.<.
-00000c50: 7c01 a000 6406 a101 6402 6405 6702 1900  |...d...d.d.g...
-00000c60: a007 a100 a003 a100 7d02 6407 7c02 6408  ........}.d.|.d.
-00000c70: 3c00 6407 7c02 6409 3c00 7408 6a09 7c01  <.d.|.d.<.t.j.|.
-00000c80: 7c02 6702 640a 640b 8d02 6a0a 6402 640c  |.g.d.d...j.d.d.
-00000c90: 640d 8d02 7d01 740b 640e 740c 7c01 8301  d...}.t.d.t.|...
-00000ca0: 640e 1700 8302 7c01 640f 3c00 7c01 6a03  d.....|.d.<.|.j.
-00000cb0: 640a 640a 6410 8d02 0100 7c01 5300 2911  d.d.d.....|.S.).
-00000cc0: 7a9c 4372 6561 7465 2056 4a6c 2063 6c61  z.Create VJl cla
-00000cd0: 7373 6573 2e0a 0a20 2020 2041 7267 733a  sses...    Args:
-00000ce0: 0a20 2020 2020 2020 2064 6620 2870 642e  .        df (pd.
-00000cf0: 4461 7461 4672 616d 6529 3a20 5072 6f63  DataFrame): Proc
-00000d00: 6573 7365 6420 6461 7461 6672 616d 6520  essed dataframe 
-00000d10: 6f66 2073 6571 7565 6e63 6573 2e0a 0a20  of sequences... 
-00000d20: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00000d30: 2020 2020 7064 2e44 6174 6146 7261 6d65      pd.DataFrame
-00000d40: 3a20 4461 7461 6672 616d 6520 7769 7468  : Dataframe with
-00000d50: 2063 6c61 7373 6573 2e0a 2020 2020 7238   classes..    r8
-00000d60: 0000 005a 0e73 6571 7565 6e63 655f 636f  ...Z.sequence_co
-00000d70: 756e 7463 0100 0000 0000 0000 0000 0000  untc............
-00000d80: 0100 0000 0300 0000 5300 0001 730a 0000  ........S...s...
-00000d90: 0074 007c 0064 0183 0253 0029 024e e902  .t.|.d...S.).N..
-00000da0: 0000 0072 0700 0000 7222 0000 0072 1c00  ...r....r"...r..
-00000db0: 0000 721c 0000 0072 1d00 0000 7224 0000  ..r....r....r$..
-00000dc0: 0087 0000 0072 2500 0000 7a20 6372 6561  .....r%...z crea
-00000dd0: 7465 5f63 6c61 7373 6573 2e3c 6c6f 6361  te_classes.<loca
-00000de0: 6c73 3e2e 3c6c 616d 6264 613e da0a 7061  ls>.<lambda>..pa
-00000df0: 6972 5f63 6f75 6e74 7231 0000 00da 044e  ir_countr1.....N
-00000e00: 6f6e 6572 2f00 0000 7230 0000 0054 2901  oner/...r0...T).
-00000e10: da0c 6967 6e6f 7265 5f69 6e64 6578 4629  ..ignore_indexF)
-00000e20: 01da 0961 7363 656e 6469 6e67 720c 0000  ...ascendingr...
-00000e30: 00da 0863 6c61 7373 5f69 6429 02da 0464  ...class_id)...d
-00000e40: 726f 70da 0769 6e70 6c61 6365 290d 723d  rop..inplace).r=
-00000e50: 0000 00da 0473 697a 65da 0874 6f5f 6672  .....size..to_fr
-00000e60: 616d 65da 0b72 6573 6574 5f69 6e64 6578  ame..reset_index
-00000e70: 7227 0000 0072 3e00 0000 720e 0000 00da  r'...r>...r.....
-00000e80: 0373 756d 7217 0000 0072 1900 0000 da0b  .sumr....r......
-00000e90: 736f 7274 5f76 616c 7565 73da 0572 616e  sort_values..ran
-00000ea0: 6765 7216 0000 0029 0372 2900 0000 da07  ger....).r).....
-00000eb0: 636c 6173 7365 735a 096c 5f63 6c61 7373  classesZ.l_class
-00000ec0: 6573 721c 0000 0072 1c00 0000 721d 0000  esr....r....r...
-00000ed0: 00da 0e63 7265 6174 655f 636c 6173 7365  ...create_classe
-00000ee0: 7378 0000 0073 2200 0000 000a 1202 02fe  sx...s".........
-00000ef0: 02ff 0606 16ff 0604 18ff 0205 0801 0801  ................
-00000f00: 1201 0201 02fe 0604 1601 0e01 7251 0000  ............rQ..
-00000f10: 0072 0500 0000 2902 722c 0000 00da 0973  .r....).r,.....s
-00000f20: 6176 655f 7061 7468 6302 0000 0000 0000  ave_pathc.......
-00000f30: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000f40: 0173 7e00 0000 7c01 6a00 7d02 7c02 6401  .s~...|.j.}.|.d.
-00000f50: 6b02 721a 7c00 a001 7c01 a101 0100 6e60  k.r.|...|.....n`
-00000f60: 7c02 6402 6b02 7232 7c00 6a02 7c01 6403  |.d.k.r2|.j.|.d.
-00000f70: 6404 8d02 0100 6e48 7c02 6405 6b02 7246  d.....nH|.d.k.rF
-00000f80: 7c00 a002 7c01 a101 0100 6e34 7c02 6406  |...|.....n4|.d.
-00000f90: 6b02 726a 6405 7c01 6a03 7600 727a 7c00  k.rjd.|.j.v.rz|.
-00000fa0: a002 7c01 a004 6407 a101 a101 0100 6e10  ..|...d.......n.
-00000fb0: 7405 6408 7c02 9b00 6409 9d03 8301 8201  t.d.|...d.......
-00000fc0: 640a 5300 290b 7ae0 5361 7665 2064 6174  d.S.).z.Save dat
-00000fd0: 6166 7261 6d65 2064 6570 656e 6469 6e67  aframe depending
-00000fe0: 206f 6e20 7375 6666 6978 2e0a 0a20 2020   on suffix...   
-00000ff0: 2041 7267 733a 0a20 2020 2020 2020 2064   Args:.        d
-00001000: 6174 6166 7261 6d65 2028 7064 2e44 6174  ataframe (pd.Dat
-00001010: 6146 7261 6d65 293a 2044 6174 6166 7261  aFrame): Datafra
-00001020: 6d65 2074 6f20 7361 7665 2e0a 2020 2020  me to save..    
-00001030: 2020 2020 7361 7665 5f70 6174 6820 2850      save_path (P
-00001040: 6174 6829 3a20 5768 6572 6520 746f 2073  ath): Where to s
-00001050: 6176 6520 7468 6520 6461 7461 6672 616d  ave the datafram
-00001060: 652e 0a0a 2020 2020 5261 6973 6573 3a0a  e...    Raises:.
-00001070: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-00001080: 6f72 3a20 7361 7665 5f70 6174 6820 7375  or: save_path su
-00001090: 6666 6978 206e 6f74 2073 7570 706f 7274  ffix not support
-000010a0: 6564 2e0a 2020 2020 fa05 2e78 6c73 78fa  ed..    ...xlsx.
-000010b0: 042e 7473 76fa 0109 a901 da03 7365 70fa  ..tsv.......sep.
-000010c0: 042e 6373 76fa 032e 677a da00 fa07 466f  ..csv...gz....Fo
-000010d0: 726d 6174 207a 0f20 6e6f 7420 7375 7070  rmat z. not supp
-000010e0: 6f72 7465 642e 4e29 06da 0673 7566 6669  orted.N)...suffi
-000010f0: 78da 0874 6f5f 6578 6365 6cda 0674 6f5f  x..to_excel..to_
-00001100: 6373 76da 0873 7566 6669 7865 73da 0b77  csv..suffixes..w
-00001110: 6974 685f 7375 6666 6978 da0a 5661 6c75  ith_suffix..Valu
-00001120: 6545 7272 6f72 2903 722c 0000 0072 5200  eError).r,...rR.
-00001130: 0000 725c 0000 0072 1c00 0000 721c 0000  ..r\...r....r...
-00001140: 0072 1d00 0000 da0e 7361 7665 5f64 6174  .r......save_dat
-00001150: 6166 7261 6d65 9900 0000 731a 0000 0000  aframe....s.....
-00001160: 0a06 0108 010c 0108 0110 0108 010c 0108  ................
-00001170: 010a 0104 0108 ff06 0472 6200 0000 7a0b  .........rb...z.
-00001180: 5061 7468 207c 204e 6f6e 6529 03da 0a69  Path | None)...i
-00001190: 6e70 7574 5f70 6174 68da 0663 6f6e 6669  nput_path..confi
-000011a0: 6772 1200 0000 6302 0000 0000 0000 0000  gr....c.........
-000011b0: 0000 0007 0000 0008 0000 0043 0000 0173  ...........C...s
-000011c0: cc00 0000 7c00 6a00 7d02 7c02 6401 6b02  ....|.j.}.|.d.k.
-000011d0: 721a 7401 a002 7c00 a101 7d03 6e5a 7c02  r.t...|...}.nZ|.
-000011e0: 6402 6b02 7232 7401 6a03 7c00 6403 6404  d.k.r2t.j.|.d.d.
-000011f0: 8d02 7d03 6e42 7c02 6405 6b02 7246 7401  ..}.nB|.d.k.rFt.
-00001200: a003 7c00 a101 7d03 6e2e 7c02 6406 6b02  ..|...}.n.|.d.k.
-00001210: 7264 6405 7c00 6a04 7600 7274 7401 a003  rdd.|.j.v.rtt...
-00001220: 7c00 a101 7d03 6e10 7405 6407 7c02 9b00  |...}.n.t.d.|...
-00001230: 6408 9d03 8301 8201 7c01 72c8 7406 7c01  d.......|.r.t.|.
-00001240: 6409 640a 8d02 8f34 7d04 7407 a008 7c04  d.d....4}.t...|.
-00001250: a101 7d05 7c05 4400 5d14 7d06 7c03 7c06  ..}.|.D.].}.|.|.
-00001260: 1900 7c03 7c05 7c06 1900 3c00 7194 5700  ..|.|.|...<.q.W.
-00001270: 640b 0400 0400 8303 0100 6e10 3100 73be  d.........n.1.s.
-00001280: 3000 0100 0100 0100 5900 0100 7c03 5300  0.......Y...|.S.
-00001290: 290c 6130 0100 0052 6561 6420 696e 7075  ).a0...Read inpu
-000012a0: 7420 6669 6c65 2e0a 0a20 2020 2041 7267  t file...    Arg
-000012b0: 733a 0a20 2020 2020 2020 2069 6e70 7574  s:.        input
-000012c0: 5f70 6174 6820 2850 6174 6829 3a50 6174  _path (Path):Pat
-000012d0: 6820 6f66 2069 6e70 7574 2066 696c 652e  h of input file.
-000012e0: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
-000012f0: 2850 6174 6829 3a20 4a73 6f6e 2063 6f6e  (Path): Json con
-00001300: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00001310: 746f 2063 6861 6e67 6520 636f 6c75 6d6e  to change column
-00001320: 206e 616d 6573 206f 6620 796f 7572 2063   names of your c
-00001330: 7573 746f 6d20 7365 7175 656e 6365 2066  ustom sequence f
-00001340: 696c 652e 0a0a 2020 2020 5261 6973 6573  ile...    Raises
-00001350: 3a0a 2020 2020 2020 2020 5661 6c75 6545  :.        ValueE
-00001360: 7272 6f72 3a20 466f 726d 6174 206f 6620  rror: Format of 
-00001370: 696e 7075 7420 6669 6c65 2069 7320 6e6f  input file is no
-00001380: 7420 7375 7070 6f72 7465 642e 0a0a 2020  t supported...  
-00001390: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000013a0: 2020 2070 642e 4461 7461 4672 616d 653a     pd.DataFrame:
-000013b0: 2050 616e 6461 7320 6461 7461 6672 616d   Pandas datafram
-000013c0: 652e 0a20 2020 2072 5300 0000 7254 0000  e..    rS...rT..
-000013d0: 0072 5500 0000 7256 0000 0072 5800 0000  .rU...rV...rX...
-000013e0: 7259 0000 0072 5b00 0000 7a3f 206e 6f74  rY...r[...z? not
-000013f0: 2073 7570 706f 7274 6564 2e20 4578 7465   supported. Exte
-00001400: 6e73 696f 6e73 2073 7570 706f 7274 6564  nsions supported
-00001410: 2061 7265 2074 7376 2c20 786c 7378 2c20   are tsv, xlsx, 
-00001420: 6373 762c 2063 7376 2e67 7a7a 0575 7466  csv, csv.gzz.utf
-00001430: 2d38 2901 da08 656e 636f 6469 6e67 4e29  -8)...encodingN)
-00001440: 0972 5c00 0000 7217 0000 00da 0a72 6561  .r\...r......rea
-00001450: 645f 6578 6365 6cda 0872 6561 645f 6373  d_excel..read_cs
-00001460: 7672 5f00 0000 7261 0000 00da 046f 7065  vr_...ra.....ope
-00001470: 6eda 046a 736f 6eda 046c 6f61 6429 0772  n..json..load).r
-00001480: 6300 0000 7264 0000 0072 5c00 0000 722c  c...rd...r\...r,
-00001490: 0000 005a 0975 7365 725f 6669 6c65 5a0b  ...Z.user_fileZ.
-000014a0: 636f 6c75 6d6e 5f64 6963 74da 036b 6579  column_dict..key
-000014b0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-000014c0: 0a72 6561 645f 696e 7075 74b3 0000 0073  .read_input....s
-000014d0: 3400 0000 000d 0601 0801 0c01 0801 0401  4...............
-000014e0: 0201 02fe 0804 0801 0401 02ff 0603 0801  ................
-000014f0: 0a01 0401 02ff 0604 0201 0aff 0403 0401  ................
-00001500: 0e01 0a01 0801 3001 726c 0000 0072 3b00  ......0.rl...r;.
-00001510: 0000 2902 7229 0000 00da 0970 6172 7469  ..).r).....parti
-00001520: 7469 6f6e 6302 0000 0000 0000 0000 0000  tionc...........
-00001530: 0009 0000 0004 0000 0043 0000 0173 be00  .........C...s..
-00001540: 0000 6401 7c00 6a00 7601 7218 7401 a002  ..d.|.j.v.r.t...
-00001550: 6402 a101 0100 6403 5300 6404 7d02 7403  d.....d.S.d.}.t.
-00001560: 7c00 a004 6401 6701 a101 a005 a100 6405  |...d.g.......d.
-00001570: 8302 a006 a100 7d03 7403 7c00 a004 7c01  ......}.t.|...|.
-00001580: 6701 a101 a005 a100 6405 8302 a006 a100  g.......d.......
-00001590: 7d04 7407 7c00 a004 6401 6701 a101 6406  }.t.|...d.g...d.
-000015a0: 6407 8d02 4400 5d30 5c02 7d05 7d06 7408  d...D.]0\.}.}.t.
-000015b0: 7c06 7c01 1900 6405 8302 4400 5d18 5c02  |.|...d...D.].\.
-000015c0: 7d07 7d08 7c07 7c08 6b02 727a 7c02 6408  }.}.|.|.k.rz|.d.
-000015d0: 3700 7d02 717a 7164 7c04 73a6 7c03 6404  7.}.qzqd|.s.|.d.
-000015e0: 6b04 72a6 6409 5300 7c03 73ae 6403 5300  k.r.d.S.|.s.d.S.
-000015f0: 7c02 7c04 1b00 7c02 7c03 1b00 6602 5300  |.|...|.|...f.S.
-00001600: 290a 7af6 4576 616c 7561 7465 2070 6572  ).z.Evaluate per
-00001610: 666f 726d 616e 6365 2069 6620 6772 6f75  formance if grou
-00001620: 6e64 2074 7275 7468 2070 7265 7365 6e74  nd truth present
-00001630: 2069 6e20 6461 7461 6672 616d 652e 0a0a   in dataframe...
-00001640: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00001650: 2020 6466 2028 7064 2e44 6174 6146 7261    df (pd.DataFra
-00001660: 6d65 293a 2064 6174 6166 7261 6d65 2074  me): dataframe t
-00001670: 6f20 6576 616c 7561 7465 0a20 2020 2020  o evaluate.     
-00001680: 2020 2070 6172 7469 7469 6f6e 2028 7374     partition (st
-00001690: 7229 3a20 6e61 6d65 206f 6620 636f 6c75  r): name of colu
-000016a0: 6d6e 2063 6f72 7265 7370 6f6e 6469 6e67  mn corresponding
-000016b0: 2074 6f20 696e 6665 7272 6564 2070 6172   to inferred par
-000016c0: 7469 7469 6f6e 2e0a 0a20 2020 2052 6574  tition...    Ret
-000016d0: 7572 6e73 3a0a 2020 2020 2020 2020 2870  urns:.        (p
-000016e0: 7265 6369 7369 6f6e 2c73 656e 7369 7469  recision,sensiti
-000016f0: 7669 7479 290a 2020 2020 da08 636c 6f6e  vity).    ..clon
-00001700: 655f 6964 7a1c 436c 6f6e 6520 6964 206e  e_idz.Clone id n
-00001710: 6f74 2061 2063 6f6c 756d 6e20 7661 6c75  ot a column valu
-00001720: 652e 2902 4e4e 7201 0000 0072 4200 0000  e.).NNr....rB...
-00001730: 5429 0172 1400 0000 720c 0000 0029 0272  T).r....r....).r
-00001740: 0100 0000 6700 0000 0000 00f0 3f29 0972  ....g.......?).r
-00001750: 3a00 0000 da03 6c6f 67da 0564 6562 7567  :.....log..debug
-00001760: 7208 0000 0072 3d00 0000 724a 0000 0072  r....r=...rJ...r
-00001770: 4d00 0000 720b 0000 0072 0300 0000 2909  M...r....r....).
-00001780: 7229 0000 0072 6d00 0000 5a02 5450 da01  r)...rm...Z.TP..
-00001790: 505a 0554 505f 4650 7228 0000 00da 0666  PZ.TP_FPr(.....f
-000017a0: 616d 696c 79da 0272 31da 0272 3272 1c00  amily..r1..r2r..
-000017b0: 0000 721c 0000 0072 1d00 0000 da13 7061  ..r....r......pa
-000017c0: 6972 7769 7365 5f65 7661 6c75 6174 696f  irwise_evaluatio
-000017d0: 6edd 0000 0073 1e00 0000 000a 0a01 0a01  n....s..........
-000017e0: 0401 0401 1a01 1a01 1c01 1601 0801 0c02  ................
-000017f0: 0c01 0401 0401 0401 7275 0000 00e7 ae47  ........ru.....G
-00001800: e17a 14ae ef3f 6302 0000 0000 0000 0000  .z...?c.........
-00001810: 0000 0002 0000 0003 0000 0043 0000 0173  ...........C...s
-00001820: 1800 0000 7c00 6401 7c00 1800 1b00 6402  ....|.d.|.....d.
-00001830: 7c01 1800 1400 7c01 1b00 5300 2903 4e67  |.....|...S.).Ng
-00001840: 72c4 5a7c 0a00 f03f 720c 0000 0072 1c00  r.Z|...?r....r..
-00001850: 0000 2902 da03 7268 6fda 0270 6972 1c00  ..)...rho..pir..
-00001860: 0000 721c 0000 0072 1d00 0000 da09 7052  ..r....r......pR
-00001870: 6571 7569 7265 64f9 0000 0073 0200 0000  equired....s....
-00001880: 0001 7279 0000 0063 0200 0000 0000 0000  ..ry...c........
-00001890: 0000 0000 0500 0000 0700 0000 4300 0001  ............C...
-000018a0: 7388 0000 007c 0064 016b 0572 1074 006a  s....|.d.k.r.t.j
-000018b0: 017d 026e 167c 0064 026b 0272 2074 006a  .}.n.|.d.k.r t.j
-000018c0: 027d 026e 0674 006a 037d 027c 0172 3674  .}.n.t.j.}.|.r6t
-000018d0: 046a 05a0 06a1 007d 036e 0e74 046a 076a  .j.....}.n.t.j.j
-000018e0: 0864 0364 048d 017d 0374 046a 0974 04a0  .d.d...}.t.j.t..
-000018f0: 0a7c 02a1 0174 046a 0b6a 0c74 046a 0ba0  .|...t.j.j.t.j..
-00001900: 0da1 0074 046a 056a 0e64 0564 068d 0174  ...t.j.j.d.d...t
-00001910: 046a 05a0 0fa1 007c 0367 0564 078d 0201  .j.....|.g.d....
-00001920: 0074 04a0 10a1 007d 047c 0453 0029 084e  .t.....}.|.S.).N
-00001930: 7242 0000 0072 0c00 0000 4629 01da 0973  rB...r....F)...s
-00001940: 6f72 745f 6b65 7973 da03 6973 6f29 01da  ort_keys..iso)..
-00001950: 0366 6d74 2902 da0d 7772 6170 7065 725f  .fmt)...wrapper_
-00001960: 636c 6173 73da 0a70 726f 6365 7373 6f72  class..processor
-00001970: 7329 11da 076c 6f67 6769 6e67 da05 4445  s)...logging..DE
-00001980: 4255 47da 0449 4e46 4fda 0757 4152 4e49  BUG..INFO..WARNI
-00001990: 4e47 da09 7374 7275 6374 6c6f 6772 7e00  NG..structlogr~.
-000019a0: 0000 da0c 4a53 4f4e 5265 6e64 6572 6572  ....JSONRenderer
-000019b0: da03 6465 76da 0f43 6f6e 736f 6c65 5265  ..dev..ConsoleRe
-000019c0: 6e64 6572 6572 da09 636f 6e66 6967 7572  nderer..configur
-000019d0: 65da 1b6d 616b 655f 6669 6c74 6572 696e  e..make_filterin
-000019e0: 675f 626f 756e 645f 6c6f 6767 6572 da06  g_bound_logger..
-000019f0: 7374 646c 6962 da0d 6164 645f 6c6f 675f  stdlib..add_log_
-00001a00: 6c65 7665 6cda 1c50 6f73 6974 696f 6e61  level..Positiona
-00001a10: 6c41 7267 756d 656e 7473 466f 726d 6174  lArgumentsFormat
-00001a20: 7465 72da 0b54 696d 6553 7461 6d70 6572  ter..TimeStamper
-00001a30: da11 5374 6163 6b49 6e66 6f52 656e 6465  ..StackInfoRende
-00001a40: 7265 72da 0a67 6574 5f6c 6f67 6765 7229  rer..get_logger)
-00001a50: 05da 0776 6572 626f 7365 da08 7573 655f  ...verbose..use_
-00001a60: 6a73 6f6e 5a0d 6c6f 6767 696e 675f 6c65  jsonZ.logging_le
-00001a70: 7665 6c5a 0872 656e 6465 7265 7272 6f00  velZ.rendererro.
-00001a80: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00001a90: 0072 8e00 0000 fd00 0000 7326 0000 0000  .r........s&....
-00001aa0: 0108 0108 0108 0108 0206 0104 010c 020e  ................
-00001ab0: 0104 0108 0206 0108 010c 0108 0102 fb02  ................
-00001ac0: fe06 0a08 0172 8e00 0000 2903 720c 0000  .....r....).r...
-00001ad0: 0046 4629 0246 720c 0000 0029 014e 2901  .FF).Fr....).N).
-00001ae0: 7276 0000 0029 20da 075f 5f64 6f63 5f5f  rv...) ..__doc__
-00001af0: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
-00001b00: 0072 6900 0000 727f 0000 00da 0969 7465  .ri...r......ite
-00001b10: 7274 6f6f 6c73 7203 0000 00da 0f6d 756c  rtoolsr......mul
-00001b20: 7469 7072 6f63 6573 7369 6e67 7204 0000  tiprocessingr...
-00001b30: 00da 0770 6174 686c 6962 7205 0000 00da  ...pathlibr.....
-00001b40: 0674 7970 696e 6772 0600 0000 da06 7061  .typingr......pa
-00001b50: 6e64 6173 7217 0000 0072 8300 0000 da0d  ndasr....r......
-00001b60: 7363 6970 792e 7370 6563 6961 6c72 0800  scipy.specialr..
-00001b70: 0000 da0c 7465 7874 6469 7374 616e 6365  ....textdistance
-00001b80: 720a 0000 0072 0b00 0000 728e 0000 00da  r....r....r.....
-00001b90: 085f 5f6e 616d 655f 5f72 6f00 0000 721e  .__name__ro...r.
-00001ba0: 0000 0072 2a00 0000 7241 0000 0072 5100  ...r*...rA...rQ.
-00001bb0: 0000 7262 0000 0072 6c00 0000 7275 0000  ..rb...rl...ru..
-00001bc0: 0072 7900 0000 721c 0000 0072 1c00 0000  .ry...r....r....
-00001bd0: 721c 0000 0072 1d00 0000 da08 3c6d 6f64  r....r......<mod
-00001be0: 756c 653e 0100 0000 7336 0000 0004 020c  ule>....s6......
-00001bf0: 0208 0108 010c 010c 010c 010c 0208 0108  ................
-00001c00: 010c 010c 010c 020a 0800 0100 0100 fb16  ................
-00001c10: 1d0e 1200 0100 fd16 3410 2110 1a14 2a10  ........4.!...*.
-00001c20: 1c0a 04                                  ...
+000007b0: 0173 5801 0000 7c00 a000 a100 7d03 6700  .sX...|.....}.g.
+000007c0: 6401 a201 7d04 6402 7c03 6a01 7601 7248  d...}.d.|.j.v.rH
+000007d0: 7c03 6a02 6403 6701 6404 6405 8d02 0100  |.j.d.g.d.d.....
+000007e0: 7c03 6403 1900 6a03 6a04 6406 6404 6407  |.d...j.j.d.d.d.
+000007f0: 6408 8d03 7c03 6402 6409 6702 3c00 640a  d...|.d.d.g.<.d.
+00000800: 7c03 6a01 7601 7280 7c03 6a02 640b 6701  |.j.v.r.|.j.d.g.
+00000810: 6404 6405 8d02 0100 7c03 640b 1900 6a03  d.d.....|.d...j.
+00000820: 6a04 6406 6404 6407 6408 8d03 7c03 640a  j.d.d.d.d...|.d.
+00000830: 6409 6702 3c00 640c 7c03 6a01 7601 72b0  d.g.<.d.|.j.v.r.
+00000840: 7c03 6a02 640d 6701 6404 6405 8d02 0100  |.j.d.g.d.d.....
+00000850: 7c03 640d 1900 6a03 640e 640f 8502 1900  |.d...j.d.d.....
+00000860: 7c03 640c 3c00 7c03 640c 1900 6a03 a005  |.d.<.|.d...j...
+00000870: a100 7c03 6410 3c00 6411 7c03 6a01 7601  ..|.d.<.d.|.j.v.
+00000880: 72f2 7c03 6a02 6412 6413 6702 6404 6405  r.|.j.d.d.g.d.d.
+00000890: 8d02 0100 7c03 6412 1900 7c03 6413 1900  ....|.d...|.d...
+000008a0: 1700 7c03 6411 3c00 6414 7c03 6a01 7601  ..|.d.<.d.|.j.v.
+000008b0: 9001 7224 7c03 6a02 6415 6416 6702 6404  ..r$|.j.d.d.g.d.
+000008c0: 6405 8d02 0100 7c03 6415 1900 7c03 6416  d.....|.d...|.d.
+000008d0: 1900 1700 7c03 6414 3c00 7406 7c03 a007  ....|.d.<.t.|...
+000008e0: 6700 6417 a201 a101 7408 7c01 7c02 6418  g.d.....t.|.|.d.
+000008f0: 8d04 7c03 6419 3c00 7c03 7c04 1900 a002  ..|.d.<.|.|.....
+00000900: a100 a009 6410 740a 6901 a101 5300 291a  ....d.t.i...S.).
+00000910: 614c 0100 0050 726f 6365 7373 2069 6e70  aL...Process inp
+00000920: 7574 2064 6174 6166 7261 6d65 2e0a 0a20  ut dataframe... 
+00000930: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000940: 2064 6174 6166 7261 6d65 2028 7064 2e44   dataframe (pd.D
+00000950: 6174 6146 7261 6d65 293a 2049 6e70 7574  ataFrame): Input
+00000960: 2064 6174 6166 7261 6d65 206f 6620 7365   dataframe of se
+00000970: 7175 656e 6365 732e 0a20 2020 2020 2020  quences..       
+00000980: 2073 696c 656e 7420 2862 6f6f 6c2c 206f   silent (bool, o
+00000990: 7074 696f 6e61 6c29 3a20 446f 206e 6f74  ptional): Do not
+000009a0: 2073 686f 7720 7072 6f67 7265 7373 2062   show progress b
+000009b0: 6172 2069 6620 7472 7565 2e20 4465 6661  ar if true. Defa
+000009c0: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
+000009d0: 2020 2020 2020 2074 6872 6561 6473 2028         threads (
+000009e0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+000009f0: 4e75 6d62 6572 206f 6620 6370 7573 206f  Number of cpus o
+00000a00: 6e20 7768 6963 6820 746f 2072 756e 2063  n which to run c
+00000a10: 6f64 652c 2064 6566 6175 6c74 7320 746f  ode, defaults to
+00000a20: 2031 2e0a 0a20 2020 2052 6574 7572 6e73   1...    Returns
+00000a30: 3a0a 2020 2020 2020 2020 7064 2e44 6174  :.        pd.Dat
+00000a40: 6166 7261 6d65 3a20 7072 6f63 6573 7365  aframe: processe
+00000a50: 6420 6461 7461 6672 616d 652e 0a20 2020  d dataframe..   
+00000a60: 2029 08da 0b73 6571 7565 6e63 655f 6964   )...sequence_id
+00000a70: da06 765f 6765 6e65 da06 6a5f 6765 6e65  ..v_gene..j_gene
+00000a80: da0b 6364 7233 5f6c 656e 6774 68da 0463  ..cdr3_length..c
+00000a90: 6472 3372 2000 0000 7221 0000 00da 0e6d  dr3r ...r!.....m
+00000aa0: 7574 6174 696f 6e5f 636f 756e 7472 2f00  utation_countr/.
+00000ab0: 0000 5a06 765f 6361 6c6c 5429 02da 0673  ..Z.v_callT)...s
+00000ac0: 7562 7365 74da 0769 6e70 6c61 6365 da01  ubset..inplace..
+00000ad0: 2a72 0c00 0000 2902 da06 6578 7061 6e64  *r....)...expand
+00000ae0: da01 6e72 2800 0000 7230 0000 005a 066a  ..nr(...r0...Z.j
+00000af0: 5f63 616c 6c72 3200 0000 5a08 6a75 6e63  _callr2...Z.junc
+00000b00: 7469 6f6e e903 0000 00e9 fdff ffff 7231  tion..........r1
+00000b10: 0000 0072 2000 0000 5a14 765f 7365 7175  ...r ...Z.v_sequ
+00000b20: 656e 6365 5f61 6c69 676e 6d65 6e74 5a14  ence_alignmentZ.
+00000b30: 6a5f 7365 7175 656e 6365 5f61 6c69 676e  j_sequence_align
+00000b40: 6d65 6e74 7221 0000 005a 1476 5f67 6572  mentr!...Z.v_ger
+00000b50: 6d6c 696e 655f 616c 6967 6e6d 656e 745a  mline_alignmentZ
+00000b60: 146a 5f67 6572 6d6c 696e 655f 616c 6967  .j_germline_alig
+00000b70: 6e6d 656e 74a9 0372 2f00 0000 7230 0000  nment..r/...r0..
+00000b80: 0072 3100 0000 2902 721a 0000 0072 1100  .r1...).r....r..
+00000b90: 0000 7233 0000 0029 0bda 0463 6f70 79da  ..r3...)...copy.
+00000ba0: 0763 6f6c 756d 6e73 da06 6472 6f70 6e61  .columns..dropna
+00000bb0: da03 7374 72da 0573 706c 6974 7216 0000  ..str..splitr...
+00000bc0: 0072 1e00 0000 da07 6772 6f75 7062 7972  .r......groupbyr
+00000bd0: 2a00 0000 da06 6173 7479 7065 720e 0000  *.....astyper...
+00000be0: 0029 0572 2c00 0000 721a 0000 0072 2d00  .).r,...r....r-.
+00000bf0: 0000 7229 0000 00da 0775 7365 636f 6c73  ..r).....usecols
+00000c00: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00000c10: 0a70 7265 7072 6f63 6573 7344 0000 0073  .preprocessD...s
+00000c20: 3600 0000 000f 0801 080a 0a01 1001 1e01  6...............
+00000c30: 0a01 1001 1e01 0a01 1001 1601 1201 0a01  ................
+00000c40: 1202 0eff 0604 0c01 1202 0eff 0604 0201  ................
+00000c50: 0c01 0201 0201 02fc 0a06 7244 0000 007a  ..........rD...z
+00000c60: 0c70 642e 4461 7461 6672 616d 6529 0272  .pd.Dataframe).r
+00000c70: 2900 0000 7212 0000 0063 0100 0000 0000  )...r....c......
+00000c80: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000c90: 0001 73a6 0000 007c 00a0 0067 0064 01a2  ..s....|...g.d..
+00000ca0: 01a1 01a0 01a1 00a0 0264 02a1 01a0 03a1  .........d......
+00000cb0: 007d 017c 0164 0219 00a0 0464 0364 0484  .}.|.d.....d.d..
+00000cc0: 00a1 01a0 0574 06a1 017c 0164 053c 007c  .....t...|.d.<.|
+00000cd0: 01a0 0064 06a1 0164 0264 0567 0219 00a0  ...d...d.d.g....
+00000ce0: 07a1 00a0 03a1 007d 0264 077c 0264 083c  .......}.d.|.d.<
+00000cf0: 0064 077c 0264 093c 0074 086a 097c 017c  .d.|.d.<.t.j.|.|
+00000d00: 0267 0264 0a64 0b8d 026a 0a64 0264 0c64  .g.d.d...j.d.d.d
+00000d10: 0d8d 027d 0174 0b64 0e74 0c7c 0183 0164  ...}.t.d.t.|...d
+00000d20: 0e17 0083 027c 0164 0f3c 007c 016a 0364  .....|.d.<.|.j.d
+00000d30: 0a64 0a64 108d 0201 007c 0153 0029 117a  .d.d.....|.S.).z
+00000d40: 9c43 7265 6174 6520 564a 6c20 636c 6173  .Create VJl clas
+00000d50: 7365 732e 0a0a 2020 2020 4172 6773 3a0a  ses...    Args:.
+00000d60: 2020 2020 2020 2020 6466 2028 7064 2e44          df (pd.D
+00000d70: 6174 6146 7261 6d65 293a 2050 726f 6365  ataFrame): Proce
+00000d80: 7373 6564 2064 6174 6166 7261 6d65 206f  ssed dataframe o
+00000d90: 6620 7365 7175 656e 6365 732e 0a0a 2020  f sequences...  
+00000da0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00000db0: 2020 2070 642e 4461 7461 4672 616d 653a     pd.DataFrame:
+00000dc0: 2044 6174 6166 7261 6d65 2077 6974 6820   Dataframe with 
+00000dd0: 636c 6173 7365 732e 0a20 2020 2072 3b00  classes..    r;.
+00000de0: 0000 5a0e 7365 7175 656e 6365 5f63 6f75  ..Z.sequence_cou
+00000df0: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
+00000e00: 0000 0003 0000 0053 0000 0173 0a00 0000  .......S...s....
+00000e10: 7400 7c00 6401 8302 5300 2902 4ee9 0200  t.|.d...S.).N...
+00000e20: 0000 7207 0000 0072 2200 0000 721c 0000  ..r....r"...r...
+00000e30: 0072 1c00 0000 721d 0000 0072 2400 0000  .r....r....r$...
+00000e40: 8c00 0000 7225 0000 007a 2063 7265 6174  ....r%...z creat
+00000e50: 655f 636c 6173 7365 732e 3c6c 6f63 616c  e_classes.<local
+00000e60: 733e 2e3c 6c61 6d62 6461 3eda 0a70 6169  s>.<lambda>..pai
+00000e70: 725f 636f 756e 7472 3100 0000 da04 4e6f  r_countr1.....No
+00000e80: 6e65 722f 0000 0072 3000 0000 5429 01da  ner/...r0...T)..
+00000e90: 0c69 676e 6f72 655f 696e 6465 7846 2901  .ignore_indexF).
+00000ea0: da09 6173 6365 6e64 696e 6772 0c00 0000  ..ascendingr....
+00000eb0: da08 636c 6173 735f 6964 2902 da04 6472  ..class_id)...dr
+00000ec0: 6f70 7235 0000 0029 0d72 4100 0000 da04  opr5...).rA.....
+00000ed0: 7369 7a65 da08 746f 5f66 7261 6d65 da0b  size..to_frame..
+00000ee0: 7265 7365 745f 696e 6465 7872 2700 0000  reset_indexr'...
+00000ef0: 7242 0000 0072 0e00 0000 da03 7375 6d72  rB...r......sumr
+00000f00: 1700 0000 7219 0000 00da 0b73 6f72 745f  ....r......sort_
+00000f10: 7661 6c75 6573 da05 7261 6e67 6572 1600  values..ranger..
+00000f20: 0000 2903 7229 0000 00da 0763 6c61 7373  ..).r).....class
+00000f30: 6573 5a09 6c5f 636c 6173 7365 7372 1c00  esZ.l_classesr..
+00000f40: 0000 721c 0000 0072 1d00 0000 da0e 6372  ..r....r......cr
+00000f50: 6561 7465 5f63 6c61 7373 6573 7d00 0000  eate_classes}...
+00000f60: 7322 0000 0000 0a12 0202 fe02 ff06 0616  s"..............
+00000f70: ff06 0418 ff02 0508 0108 0112 0102 0102  ................
+00000f80: fe06 0416 010e 0172 5300 0000 7205 0000  .......rS...r...
+00000f90: 0029 0272 2c00 0000 da09 7361 7665 5f70  .).r,.....save_p
+00000fa0: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
+00000fb0: 0300 0000 0500 0000 4300 0001 737e 0000  ........C...s~..
+00000fc0: 007c 016a 007d 027c 0264 016b 0272 1a7c  .|.j.}.|.d.k.r.|
+00000fd0: 00a0 017c 01a1 0101 006e 607c 0264 026b  ...|.....n`|.d.k
+00000fe0: 0272 327c 006a 027c 0164 0364 048d 0201  .r2|.j.|.d.d....
+00000ff0: 006e 487c 0264 056b 0272 467c 00a0 027c  .nH|.d.k.rF|...|
+00001000: 01a1 0101 006e 347c 0264 066b 0272 6a64  .....n4|.d.k.rjd
+00001010: 057c 016a 0376 0072 7a7c 00a0 027c 01a0  .|.j.v.rz|...|..
+00001020: 0464 07a1 01a1 0101 006e 1074 0564 087c  .d.......n.t.d.|
+00001030: 029b 0064 099d 0383 0182 0164 0a53 0029  ...d.......d.S.)
+00001040: 0b7a e053 6176 6520 6461 7461 6672 616d  .z.Save datafram
+00001050: 6520 6465 7065 6e64 696e 6720 6f6e 2073  e depending on s
+00001060: 7566 6669 782e 0a0a 2020 2020 4172 6773  uffix...    Args
+00001070: 3a0a 2020 2020 2020 2020 6461 7461 6672  :.        datafr
+00001080: 616d 6520 2870 642e 4461 7461 4672 616d  ame (pd.DataFram
+00001090: 6529 3a20 4461 7461 6672 616d 6520 746f  e): Dataframe to
+000010a0: 2073 6176 652e 0a20 2020 2020 2020 2073   save..        s
+000010b0: 6176 655f 7061 7468 2028 5061 7468 293a  ave_path (Path):
+000010c0: 2057 6865 7265 2074 6f20 7361 7665 2074   Where to save t
+000010d0: 6865 2064 6174 6166 7261 6d65 2e0a 0a20  he dataframe... 
+000010e0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+000010f0: 2020 2056 616c 7565 4572 726f 723a 2073     ValueError: s
+00001100: 6176 655f 7061 7468 2073 7566 6669 7820  ave_path suffix 
+00001110: 6e6f 7420 7375 7070 6f72 7465 642e 0a20  not supported.. 
+00001120: 2020 20fa 052e 786c 7378 fa04 2e74 7376     ...xlsx...tsv
+00001130: fa01 09a9 01da 0373 6570 fa04 2e63 7376  .......sep...csv
+00001140: fa03 2e67 7ada 00fa 0746 6f72 6d61 7420  ...gz....Format 
+00001150: 7a0f 206e 6f74 2073 7570 706f 7274 6564  z. not supported
+00001160: 2e4e 2906 da06 7375 6666 6978 da08 746f  .N)...suffix..to
+00001170: 5f65 7863 656c da06 746f 5f63 7376 da08  _excel..to_csv..
+00001180: 7375 6666 6978 6573 da0b 7769 7468 5f73  suffixes..with_s
+00001190: 7566 6669 78da 0a56 616c 7565 4572 726f  uffix..ValueErro
+000011a0: 7229 0372 2c00 0000 7254 0000 0072 5e00  r).r,...rT...r^.
+000011b0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000011c0: 00da 0e73 6176 655f 6461 7461 6672 616d  ...save_datafram
+000011d0: 659e 0000 0073 1a00 0000 000a 0601 0801  e....s..........
+000011e0: 0c01 0801 1001 0801 0c01 0801 0a01 0401  ................
+000011f0: 08ff 0604 7264 0000 007a 0b50 6174 6820  ....rd...z.Path 
+00001200: 7c20 4e6f 6e65 2903 da0a 696e 7075 745f  | None)...input_
+00001210: 7061 7468 da06 636f 6e66 6967 7212 0000  path..configr...
+00001220: 0063 0200 0000 0000 0000 0000 0000 0700  .c..............
+00001230: 0000 0800 0000 4300 0001 73cc 0000 007c  ......C...s....|
+00001240: 006a 007d 027c 0264 016b 0272 1a74 01a0  .j.}.|.d.k.r.t..
+00001250: 027c 00a1 017d 036e 5a7c 0264 026b 0272  .|...}.nZ|.d.k.r
+00001260: 3274 016a 037c 0064 0364 048d 027d 036e  2t.j.|.d.d...}.n
+00001270: 427c 0264 056b 0272 4674 01a0 037c 00a1  B|.d.k.rFt...|..
+00001280: 017d 036e 2e7c 0264 066b 0272 6464 057c  .}.n.|.d.k.rdd.|
+00001290: 006a 0476 0072 7474 01a0 037c 00a1 017d  .j.v.rtt...|...}
+000012a0: 036e 1074 0564 077c 029b 0064 089d 0383  .n.t.d.|...d....
+000012b0: 0182 017c 0172 c874 067c 0164 0964 0a8d  ...|.r.t.|.d.d..
+000012c0: 028f 347d 0474 07a0 087c 04a1 017d 057c  ..4}.t...|...}.|
+000012d0: 0544 005d 147d 067c 037c 0619 007c 037c  .D.].}.|.|...|.|
+000012e0: 057c 0619 003c 0071 9457 0064 0b04 0004  .|...<.q.W.d....
+000012f0: 0083 0301 006e 1031 0073 be30 0001 0001  .....n.1.s.0....
+00001300: 0001 0059 0001 007c 0353 0029 0c61 3001  ...Y...|.S.).a0.
+00001310: 0000 5265 6164 2069 6e70 7574 2066 696c  ..Read input fil
+00001320: 652e 0a0a 2020 2020 4172 6773 3a0a 2020  e...    Args:.  
+00001330: 2020 2020 2020 696e 7075 745f 7061 7468        input_path
+00001340: 2028 5061 7468 293a 5061 7468 206f 6620   (Path):Path of 
+00001350: 696e 7075 7420 6669 6c65 2e0a 2020 2020  input file..    
+00001360: 2020 2020 636f 6e66 6967 2028 5061 7468      config (Path
+00001370: 293a 204a 736f 6e20 636f 6e66 6967 7572  ): Json configur
+00001380: 6174 696f 6e20 6669 6c65 2074 6f20 6368  ation file to ch
+00001390: 616e 6765 2063 6f6c 756d 6e20 6e61 6d65  ange column name
+000013a0: 7320 6f66 2079 6f75 7220 6375 7374 6f6d  s of your custom
+000013b0: 2073 6571 7565 6e63 6520 6669 6c65 2e0a   sequence file..
+000013c0: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+000013d0: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
+000013e0: 2046 6f72 6d61 7420 6f66 2069 6e70 7574   Format of input
+000013f0: 2066 696c 6520 6973 206e 6f74 2073 7570   file is not sup
+00001400: 706f 7274 6564 2e0a 0a20 2020 2052 6574  ported...    Ret
+00001410: 7572 6e73 3a0a 2020 2020 2020 2020 7064  urns:.        pd
+00001420: 2e44 6174 6146 7261 6d65 3a20 5061 6e64  .DataFrame: Pand
+00001430: 6173 2064 6174 6166 7261 6d65 2e0a 2020  as dataframe..  
+00001440: 2020 7255 0000 0072 5600 0000 7257 0000    rU...rV...rW..
+00001450: 0072 5800 0000 725a 0000 0072 5b00 0000  .rX...rZ...r[...
+00001460: 725d 0000 007a 3f20 6e6f 7420 7375 7070  r]...z? not supp
+00001470: 6f72 7465 642e 2045 7874 656e 7369 6f6e  orted. Extension
+00001480: 7320 7375 7070 6f72 7465 6420 6172 6520  s supported are 
+00001490: 7473 762c 2078 6c73 782c 2063 7376 2c20  tsv, xlsx, csv, 
+000014a0: 6373 762e 677a 7a05 7574 662d 3829 01da  csv.gzz.utf-8)..
+000014b0: 0865 6e63 6f64 696e 674e 2909 725e 0000  .encodingN).r^..
+000014c0: 0072 1700 0000 da0a 7265 6164 5f65 7863  .r......read_exc
+000014d0: 656c da08 7265 6164 5f63 7376 7261 0000  el..read_csvra..
+000014e0: 0072 6300 0000 da04 6f70 656e da04 6a73  .rc.....open..js
+000014f0: 6f6e da04 6c6f 6164 2907 7265 0000 0072  on..load).re...r
+00001500: 6600 0000 725e 0000 0072 2c00 0000 5a09  f...r^...r,...Z.
+00001510: 7573 6572 5f66 696c 655a 0b63 6f6c 756d  user_fileZ.colum
+00001520: 6e5f 6469 6374 da03 6b65 7972 1c00 0000  n_dict..keyr....
+00001530: 721c 0000 0072 1d00 0000 da0a 7265 6164  r....r......read
+00001540: 5f69 6e70 7574 b800 0000 7334 0000 0000  _input....s4....
+00001550: 0d06 0108 010c 0108 0104 0102 0102 fe08  ................
+00001560: 0408 0104 0102 ff06 0308 010a 0104 0102  ................
+00001570: ff06 0402 010a ff04 0304 010e 010a 0108  ................
+00001580: 0130 0172 6e00 0000 723f 0000 0029 0272  .0.rn...r?...).r
+00001590: 2900 0000 da09 7061 7274 6974 696f 6e63  ).....partitionc
+000015a0: 0200 0000 0000 0000 0000 0000 0900 0000  ................
+000015b0: 0400 0000 4300 0001 73be 0000 0064 017c  ....C...s....d.|
+000015c0: 006a 0076 0172 1874 01a0 0264 02a1 0101  .j.v.r.t...d....
+000015d0: 0064 0353 0064 047d 0274 037c 00a0 0464  .d.S.d.}.t.|...d
+000015e0: 0167 01a1 01a0 05a1 0064 0583 02a0 06a1  .g.......d......
+000015f0: 007d 0374 037c 00a0 047c 0167 01a1 01a0  .}.t.|...|.g....
+00001600: 05a1 0064 0583 02a0 06a1 007d 0474 077c  ...d.......}.t.|
+00001610: 00a0 0464 0167 01a1 0164 0664 078d 0244  ...d.g...d.d...D
+00001620: 005d 305c 027d 057d 0674 087c 067c 0119  .]0\.}.}.t.|.|..
+00001630: 0064 0583 0244 005d 185c 027d 077d 087c  .d...D.].\.}.}.|
+00001640: 077c 086b 0272 7a7c 0264 0837 007d 0271  .|.k.rz|.d.7.}.q
+00001650: 7a71 647c 0473 a67c 0364 046b 0472 a664  zqd|.s.|.d.k.r.d
+00001660: 0953 007c 0373 ae64 0353 007c 027c 041b  .S.|.s.d.S.|.|..
+00001670: 007c 027c 031b 0066 0253 0029 0a7a f645  .|.|...f.S.).z.E
+00001680: 7661 6c75 6174 6520 7065 7266 6f72 6d61  valuate performa
+00001690: 6e63 6520 6966 2067 726f 756e 6420 7472  nce if ground tr
+000016a0: 7574 6820 7072 6573 656e 7420 696e 2064  uth present in d
+000016b0: 6174 6166 7261 6d65 2e0a 0a20 2020 2041  ataframe...    A
+000016c0: 7267 733a 0a20 2020 2020 2020 2064 6620  rgs:.        df 
+000016d0: 2870 642e 4461 7461 4672 616d 6529 3a20  (pd.DataFrame): 
+000016e0: 6461 7461 6672 616d 6520 746f 2065 7661  dataframe to eva
+000016f0: 6c75 6174 650a 2020 2020 2020 2020 7061  luate.        pa
+00001700: 7274 6974 696f 6e20 2873 7472 293a 206e  rtition (str): n
+00001710: 616d 6520 6f66 2063 6f6c 756d 6e20 636f  ame of column co
+00001720: 7272 6573 706f 6e64 696e 6720 746f 2069  rresponding to i
+00001730: 6e66 6572 7265 6420 7061 7274 6974 696f  nferred partitio
+00001740: 6e2e 0a0a 2020 2020 5265 7475 726e 733a  n...    Returns:
+00001750: 0a20 2020 2020 2020 2028 7072 6563 6973  .        (precis
+00001760: 696f 6e2c 7365 6e73 6974 6976 6974 7929  ion,sensitivity)
+00001770: 0a20 2020 20da 0863 6c6f 6e65 5f69 647a  .    ..clone_idz
+00001780: 1c43 6c6f 6e65 2069 6420 6e6f 7420 6120  .Clone id not a 
+00001790: 636f 6c75 6d6e 2076 616c 7565 2e29 024e  column value.).N
+000017a0: 4e72 0100 0000 7245 0000 0054 2901 7214  Nr....rE...T).r.
+000017b0: 0000 0072 0c00 0000 2902 7201 0000 0067  ...r....).r....g
+000017c0: 0000 0000 0000 f03f 2909 723d 0000 00da  .......?).r=....
+000017d0: 036c 6f67 da05 6465 6275 6772 0800 0000  .log..debugr....
+000017e0: 7241 0000 0072 4c00 0000 724f 0000 0072  rA...rL...rO...r
+000017f0: 0b00 0000 7203 0000 0029 0972 2900 0000  ....r....).r)...
+00001800: 726f 0000 005a 0254 50da 0150 5a05 5450  ro...Z.TP..PZ.TP
+00001810: 5f46 5072 2800 0000 da06 6661 6d69 6c79  _FPr(.....family
+00001820: da02 7231 da02 7232 721c 0000 0072 1c00  ..r1..r2r....r..
+00001830: 0000 721d 0000 00da 1370 6169 7277 6973  ..r......pairwis
+00001840: 655f 6576 616c 7561 7469 6f6e e200 0000  e_evaluation....
+00001850: 731e 0000 0000 0a0a 010a 0104 0104 011a  s...............
+00001860: 011a 011c 0116 0108 010c 020c 0104 0104  ................
+00001870: 0104 0172 7700 0000 e7ae 47e1 7a14 aeef  ...rw.....G.z...
+00001880: 3f63 0200 0000 0000 0000 0000 0000 0200  ?c..............
+00001890: 0000 0300 0000 4300 0001 7318 0000 007c  ......C...s....|
+000018a0: 0064 017c 0018 001b 0064 027c 0118 0014  .d.|.....d.|....
+000018b0: 007c 011b 0053 0029 034e 6772 c45a 7c0a  .|...S.).Ngr.Z|.
+000018c0: 00f0 3f72 0c00 0000 721c 0000 0029 02da  ..?r....r....)..
+000018d0: 0372 686f da02 7069 721c 0000 0072 1c00  .rho..pir....r..
+000018e0: 0000 721d 0000 00da 0970 5265 7175 6972  ..r......pRequir
+000018f0: 6564 fe00 0000 7302 0000 0000 0172 7b00  ed....s......r{.
+00001900: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
+00001910: 0000 0007 0000 0043 0000 0173 8800 0000  .......C...s....
+00001920: 7c00 6401 6b05 7210 7400 6a01 7d02 6e16  |.d.k.r.t.j.}.n.
+00001930: 7c00 6402 6b02 7220 7400 6a02 7d02 6e06  |.d.k.r t.j.}.n.
+00001940: 7400 6a03 7d02 7c01 7236 7404 6a05 a006  t.j.}.|.r6t.j...
+00001950: a100 7d03 6e0e 7404 6a07 6a08 6403 6404  ..}.n.t.j.j.d.d.
+00001960: 8d01 7d03 7404 6a09 7404 a00a 7c02 a101  ..}.t.j.t...|...
+00001970: 7404 6a0b 6a0c 7404 6a0b a00d a100 7404  t.j.j.t.j.....t.
+00001980: 6a05 6a0e 6405 6406 8d01 7404 6a05 a00f  j.j.d.d...t.j...
+00001990: a100 7c03 6705 6407 8d02 0100 7404 a010  ..|.g.d.....t...
+000019a0: a100 7d04 7c04 5300 2908 4e72 4500 0000  ..}.|.S.).NrE...
+000019b0: 720c 0000 0046 2901 da09 736f 7274 5f6b  r....F)...sort_k
+000019c0: 6579 73da 0369 736f 2901 da03 666d 7429  eys..iso)...fmt)
+000019d0: 02da 0d77 7261 7070 6572 5f63 6c61 7373  ...wrapper_class
+000019e0: da0a 7072 6f63 6573 736f 7273 2911 da07  ..processors)...
+000019f0: 6c6f 6767 696e 67da 0544 4542 5547 da04  logging..DEBUG..
+00001a00: 494e 464f da07 5741 524e 494e 47da 0973  INFO..WARNING..s
+00001a10: 7472 7563 746c 6f67 7280 0000 00da 0c4a  tructlogr......J
+00001a20: 534f 4e52 656e 6465 7265 72da 0364 6576  SONRenderer..dev
+00001a30: da0f 436f 6e73 6f6c 6552 656e 6465 7265  ..ConsoleRendere
+00001a40: 72da 0963 6f6e 6669 6775 7265 da1b 6d61  r..configure..ma
+00001a50: 6b65 5f66 696c 7465 7269 6e67 5f62 6f75  ke_filtering_bou
+00001a60: 6e64 5f6c 6f67 6765 72da 0673 7464 6c69  nd_logger..stdli
+00001a70: 62da 0d61 6464 5f6c 6f67 5f6c 6576 656c  b..add_log_level
+00001a80: da1c 506f 7369 7469 6f6e 616c 4172 6775  ..PositionalArgu
+00001a90: 6d65 6e74 7346 6f72 6d61 7474 6572 da0b  mentsFormatter..
+00001aa0: 5469 6d65 5374 616d 7065 72da 1153 7461  TimeStamper..Sta
+00001ab0: 636b 496e 666f 5265 6e64 6572 6572 da0a  ckInfoRenderer..
+00001ac0: 6765 745f 6c6f 6767 6572 2905 da07 7665  get_logger)...ve
+00001ad0: 7262 6f73 65da 0875 7365 5f6a 736f 6e5a  rbose..use_jsonZ
+00001ae0: 0d6c 6f67 6769 6e67 5f6c 6576 656c 5a08  .logging_levelZ.
+00001af0: 7265 6e64 6572 6572 7271 0000 0072 1c00  rendererrq...r..
+00001b00: 0000 721c 0000 0072 1d00 0000 7290 0000  ..r....r....r...
+00001b10: 0002 0100 0073 2600 0000 0001 0801 0801  .....s&.........
+00001b20: 0801 0802 0601 0401 0c02 0e01 0401 0802  ................
+00001b30: 0601 0801 0c01 0801 02fb 02fe 060a 0801  ................
+00001b40: 7290 0000 0029 0372 0c00 0000 4646 2902  r....).r....FF).
+00001b50: 4672 0c00 0000 2901 4e29 0172 7800 0000  Fr....).N).rx...
+00001b60: 2920 da07 5f5f 646f 635f 5fda 0a5f 5f66  ) ..__doc__..__f
+00001b70: 7574 7572 655f 5f72 0200 0000 726b 0000  uture__r....rk..
+00001b80: 0072 8100 0000 da09 6974 6572 746f 6f6c  .r......itertool
+00001b90: 7372 0300 0000 da0f 6d75 6c74 6970 726f  sr......multipro
+00001ba0: 6365 7373 696e 6772 0400 0000 da07 7061  cessingr......pa
+00001bb0: 7468 6c69 6272 0500 0000 da06 7479 7069  thlibr......typi
+00001bc0: 6e67 7206 0000 00da 0670 616e 6461 7372  ngr......pandasr
+00001bd0: 1700 0000 7285 0000 00da 0d73 6369 7079  ....r......scipy
+00001be0: 2e73 7065 6369 616c 7208 0000 00da 0c74  .specialr......t
+00001bf0: 6578 7464 6973 7461 6e63 6572 0a00 0000  extdistancer....
+00001c00: 720b 0000 0072 9000 0000 da08 5f5f 6e61  r....r......__na
+00001c10: 6d65 5f5f 7271 0000 0072 1e00 0000 722a  me__rq...r....r*
+00001c20: 0000 0072 4400 0000 7253 0000 0072 6400  ...rD...rS...rd.
+00001c30: 0000 726e 0000 0072 7700 0000 727b 0000  ..rn...rw...r{..
+00001c40: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+00001c50: 721d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001c60: 0000 0073 3600 0000 0402 0c02 0801 0801  ...s6...........
+00001c70: 0c01 0c01 0c01 0c02 0801 0801 0c01 0c01  ................
+00001c80: 0c02 0a08 0001 0001 00fb 161d 0e12 0001  ................
+00001c90: 00fd 1639 1021 101a 142a 101c 0a04       ...9.!...*....
```

### Comparing `hilary-1.2.0/hilary/apriori.py` & `hilary-1.2.1/hilary/apriori.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,16 @@
 
         Args:
             args tuple[tuple[int],pd.DataFrame]: length, dataframe grouped by length.
         Returns:
             pd.DataFrame: Precise and sensitive thresholds.
         """
         tuple_l, ldf = args
-        l = tuple_l[0]
+        l = int(tuple_l[0])
+
         if l > self.lengths[-1] or l < self.lengths[0] or l % 3:
             ldf[["precise_threshold", "sensitive_threshold"]] = (
                 np.ones((len(ldf), 2), dtype=int) * l // 5
             )
             return ldf[["precise_threshold", "sensitive_threshold"]]
 
         rhos = ldf["effective_prevalence"]
```

### Comparing `hilary-1.2.0/hilary/cdfs_326651.csv` & `hilary-1.2.1/hilary/cdfs_326651.csv`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/hilary/cdfs_326713.csv` & `hilary-1.2.1/hilary/cdfs_326713.csv`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/hilary/cdfs_paired.csv` & `hilary-1.2.1/hilary/cdfs_paired.csv`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/hilary/cdfs_paired_post_50K.csv` & `hilary-1.2.1/hilary/cdfs_paired_post_50K.csv`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/hilary/expectmax.py` & `hilary-1.2.1/hilary/expectmax.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,12 +102,12 @@
 
     def error(self, theta):
         """Estimate goodness of fit
         By default returns rescaled root MSE"""
         y1 = self.h / sum(self.h)
         y2 = self.discreteMix(self.b, theta)
         mask = self.b < 0.2 * self.l
-        logy1, logy2 = np.log(y1[mask] + 5), np.log(y2[mask] + 5)
+        y1m, y2m = y1[mask], y2[mask]
 
-        mse = ((logy1 - logy2) ** 2).sum()
+        mse = ((y1m - y2m) ** 2).sum()
         rrmse = np.sqrt(mse)
         return rrmse
```

### Comparing `hilary-1.2.0/hilary/inference.py` & `hilary-1.2.1/hilary/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import pandas as pd
 import structlog
 from atriegc import TrieNucl as Trie
 from scipy.cluster.hierarchy import fcluster, linkage
 from scipy.spatial.distance import squareform
 from textdistance import hamming
+from tqdm import tqdm
 
 from hilary.apriori import Apriori
 from hilary.utils import applyParallel, pRequired
 
 # pylint: disable=invalid-name
 
 log = structlog.get_logger()
@@ -225,26 +226,26 @@
                 self.classes.query(
                     "v_gene != 'None' and precise_threshold < sensitive_threshold and pair_count > 0",
                 )
                 .groupby(self.group)
                 .first()
                 .index
             )
-
         self.silent = apriori.silent
         self.cdfs = apriori.cdfs
         self.lengths = apriori.lengths
         self.threads = apriori.threads
 
     def simulate_xs_ys(
         self,
         args,
     ):
         size = int(1e6)
         (_, _, l, prevalence, mutations, alignment_length, class_id) = args
+        l = int(l)
         if l not in self.lengths or (len(mutations) < 100):
             return (0, class_id)
         bins = np.arange(np.max(mutations) + 1)
         pni, nis = np.histogram(mutations, bins=bins)
         p = pni[1:] / sum(pni[1:])
         if len(nis) < 3:
             return (0, class_id)
@@ -275,23 +276,25 @@
         mutations_grouped = []
         for (
             v_gene,
             j_gene,
             cdr3_length,
             prevalence,
             class_id,
-        ) in self.classes[
-            [
-                "v_gene",
-                "j_gene",
-                "cdr3_length",
-                "effective_prevalence",
-                "class_id",
-            ]
-        ].values:
+        ) in tqdm(
+            self.classes[
+                [
+                    "v_gene",
+                    "j_gene",
+                    "cdr3_length",
+                    "effective_prevalence",
+                    "class_id",
+                ]
+            ].values
+        ):
             if v_gene == "None":
                 mutations = df.query("cdr3_length==@cdr3_length")["mutation_count"]
             else:
                 mutations = df.query(
                     "v_gene==@v_gene and j_gene==@j_gene and cdr3_length==@cdr3_length"
                 )["mutation_count"]
             mutations_grouped.append(
```

### Comparing `hilary-1.2.0/hilary/utils.py` & `hilary-1.2.1/hilary/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,37 +88,42 @@
         "cdr3_length",
         "cdr3",
         "alt_sequence_alignment",
         "alt_germline_alignment",
         "mutation_count",
     ]
     if "v_gene" not in df.columns:
-        df[["v_gene", "_"]] = df["v_call"].str.split("*", expand=True)
+        df.dropna(subset=["v_call"], inplace=True)
+        df[["v_gene", "_"]] = df["v_call"].str.split("*", expand=True, n=1)
     if "j_gene" not in df.columns:
-        df[["j_gene", "_"]] = df["j_call"].str.split("*", expand=True)
+        df.dropna(subset=["j_call"], inplace=True)
+        df[["j_gene", "_"]] = df["j_call"].str.split("*", expand=True, n=1)
     if "cdr3" not in df.columns:
+        df.dropna(subset=["junction"], inplace=True)
         df["cdr3"] = df["junction"].str[3:-3]
     df["cdr3_length"] = df["cdr3"].str.len()
     if "alt_sequence_alignment" not in df.columns:
+        df.dropna(subset=["v_sequence_alignment", "j_sequence_alignment"], inplace=True)
         df["alt_sequence_alignment"] = (
             df["v_sequence_alignment"] + df["j_sequence_alignment"]
         )
 
     if "alt_germline_alignment" not in df.columns:
+        df.dropna(subset=["v_germline_alignment", "j_germline_alignment"], inplace=True)
         df["alt_germline_alignment"] = (
             df["v_germline_alignment"] + df["j_germline_alignment"]
         )
 
     df["mutation_count"] = applyParallel(
         df.groupby(["v_gene", "j_gene", "cdr3_length"]),
         count_mutations,
         silent=silent,
         cpuCount=threads,
     )
-    return df[usecols].astype({"cdr3_length": int}).dropna()
+    return df[usecols].dropna().astype({"cdr3_length": int})
 
 
 def create_classes(df: pd.DataFrame) -> pd.Dataframe:
     """Create VJl classes.
 
     Args:
         df (pd.DataFrame): Processed dataframe of sequences.
```

### Comparing `hilary-1.2.0/hilary.egg-info/SOURCES.txt` & `hilary-1.2.1/hilary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hilary-1.2.0/setup.py` & `hilary-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,25 @@
         "textdistance>=4.6,<5",
         "tqdm>=4.66,<5",
         "typer>=0.9,<1",
         "atriegc>=0.0.3,<1.0.0",
         "scipy>1.11,<2",
     ],
     name="hilary",
-    version="1.2.0",
+    version="1.2.1",
     url="https://github.com/statbiophys/HILARy/",
-    author="Natanael Spisak, Gabriel Athènes",
-    author_email="natanael.spisak@gmail.com, gabriel.athenes@polytechnique.edu",
+    author="Gabriel Athènes,Natanael Spisak",
+    author_email="gabriel.athenes@polytechnique.edu,natanael.spisak@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "infer-lineages=hilary.__main__:app",
         ],
     },
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
     ],
 )
```

