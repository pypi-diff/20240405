# Comparing `tmp/minijson-3.0.tar.gz` & `tmp/minijson-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minijson-3.0.tar", last modified: Fri Apr  5 10:23:31 2024, max compression
+gzip compressed data, was "minijson-3.0.1.tar", last modified: Fri Apr  5 11:36:04 2024, max compression
```

## Comparing `minijson-3.0.tar` & `minijson-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.347436 minijson-3.0/
--rw-rw-rw-   0        0        0     1119 2024-04-05 08:25:52.000000 minijson-3.0/LICENSE
--rw-rw-rw-   0        0        0     3410 2024-04-05 10:23:31.344481 minijson-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2024 2024-04-05 09:24:04.000000 minijson-3.0/README.md
--rw-rw-rw-   0        0        0  1073249 2024-04-05 10:19:07.000000 minijson-3.0/minijson.c
-drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.338521 minijson-3.0/minijson.egg-info/
--rw-rw-rw-   0        0        0     3410 2024-04-05 10:23:30.000000 minijson-3.0/minijson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-04-05 10:23:31.000000 minijson-3.0/minijson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 10:23:30.000000 minijson-3.0/minijson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 10:23:31.000000 minijson-3.0/minijson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1389 2024-04-05 10:23:31.353291 minijson-3.0/setup.cfg
--rw-rw-rw-   0        0        0      678 2024-04-05 10:06:36.000000 minijson-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.333490 minijson-3.0/tests/
--rw-rw-rw-   0        0        0    10808 2024-04-05 07:56:56.000000 minijson-3.0/tests/test_minijson.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:36:04.571832 minijson-3.0.1/
+-rw-rw-rw-   0        0        0     1119 2024-04-05 08:25:52.000000 minijson-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3415 2024-04-05 11:36:04.569727 minijson-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2027 2024-04-05 10:47:39.000000 minijson-3.0.1/README.md
+-rw-rw-rw-   0        0        0  1073249 2024-04-05 11:34:56.000000 minijson-3.0.1/minijson.c
+drwxrwxrwx   0        0        0        0 2024-04-05 11:36:04.565571 minijson-3.0.1/minijson.egg-info/
+-rw-rw-rw-   0        0        0     3415 2024-04-05 11:36:04.000000 minijson-3.0.1/minijson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-04-05 11:36:04.000000 minijson-3.0.1/minijson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 11:36:04.000000 minijson-3.0.1/minijson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 11:36:04.000000 minijson-3.0.1/minijson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1391 2024-04-05 11:36:04.573973 minijson-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      678 2024-04-05 10:06:36.000000 minijson-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 11:36:04.560393 minijson-3.0.1/tests/
+-rw-rw-rw-   0        0        0    10808 2024-04-05 07:56:56.000000 minijson-3.0.1/tests/test_minijson.py
```

### Comparing `minijson-3.0/LICENSE` & `minijson-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minijson-3.0/PKG-INFO` & `minijson-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijson
-Version: 3.0
+Version: 3.0.1
 Summary: A library for serializing JSON in a small binary format
 Home-page: https://github.com/smok-serwis/minijson
 Author: Piotr Maślanka
 Author-email: piotr.maslanka@dronehub.ai
 Project-URL: Documentation, https://minijson.readthedocs.io/
 Project-URL: Code, https://github.com/smok-serwis/minijson
 Project-URL: Issue tracker, https://github.com/smok-serwis/minijson/issues
@@ -55,15 +55,15 @@
 
 Refer to the [documentation](http://minijson.readthedocs.io/en/latest/?badge=latest)
 for use.
 
 If there are no binary wheels precompiled for this platform, you will need to
 compile it yourself.
 Alternatively, you can
-[file an issue](https://github.com/Dronehub/minijson/issues/new)
+[file an issue](https://github.com/smok-serwis/minijson/issues/new)
 and I'll do my best to compile a wheel for you.
 
 Compiling own wheels
 --------------------
 
 If there's no wheel, and you'd like to compile it on your own, you'll
 require [Cython](https://cython.org/) installed.
```

### Comparing `minijson-3.0/README.md` & `minijson-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 Refer to the [documentation](http://minijson.readthedocs.io/en/latest/?badge=latest)
 for use.
 
 If there are no binary wheels precompiled for this platform, you will need to
 compile it yourself.
 Alternatively, you can
-[file an issue](https://github.com/Dronehub/minijson/issues/new)
+[file an issue](https://github.com/smok-serwis/minijson/issues/new)
 and I'll do my best to compile a wheel for you.
 
 Compiling own wheels
 --------------------
 
 If there's no wheel, and you'd like to compile it on your own, you'll
 require [Cython](https://cython.org/) installed.
```

### Comparing `minijson-3.0/minijson.c` & `minijson-3.0.1/minijson.c`

 * *Files identical despite different names*

### Comparing `minijson-3.0/minijson.egg-info/PKG-INFO` & `minijson-3.0.1/minijson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minijson
-Version: 3.0
+Version: 3.0.1
 Summary: A library for serializing JSON in a small binary format
 Home-page: https://github.com/smok-serwis/minijson
 Author: Piotr Maślanka
 Author-email: piotr.maslanka@dronehub.ai
 Project-URL: Documentation, https://minijson.readthedocs.io/
 Project-URL: Code, https://github.com/smok-serwis/minijson
 Project-URL: Issue tracker, https://github.com/smok-serwis/minijson/issues
@@ -55,15 +55,15 @@
 
 Refer to the [documentation](http://minijson.readthedocs.io/en/latest/?badge=latest)
 for use.
 
 If there are no binary wheels precompiled for this platform, you will need to
 compile it yourself.
 Alternatively, you can
-[file an issue](https://github.com/Dronehub/minijson/issues/new)
+[file an issue](https://github.com/smok-serwis/minijson/issues/new)
 and I'll do my best to compile a wheel for you.
 
 Compiling own wheels
 --------------------
 
 If there's no wheel, and you'd like to compile it on your own, you'll
 require [Cython](https://cython.org/) installed.
```

### Comparing `minijson-3.0/setup.cfg` & `minijson-3.0.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 332e 300d 0a6e 616d 6520  ion = 3.0..name 
-00000020: 3d20 6d69 6e69 6a73 6f6e 0d0a 6c6f 6e67  = minijson..long
-00000030: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000040: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000050: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000060: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000070: 7465 7874 2f6d 6172 6b64 6f77 6e3b 2063  text/markdown; c
-00000080: 6861 7273 6574 3d55 5446 2d38 0d0a 6175  harset=UTF-8..au
-00000090: 7468 6f72 203d 2050 696f 7472 204d 61c5  thor = Piotr Ma.
-000000a0: 9b6c 616e 6b61 0d0a 6c69 6365 6e73 655f  .lanka..license_
-000000b0: 6669 6c65 7320 3d20 0d0a 094c 4943 454e  files = ...LICEN
-000000c0: 5345 0d0a 6175 7468 6f72 5f65 6d61 696c  SE..author_email
-000000d0: 203d 2070 696f 7472 2e6d 6173 6c61 6e6b   = piotr.maslank
-000000e0: 6140 6472 6f6e 6568 7562 2e61 690d 0a64  a@dronehub.ai..d
-000000f0: 6573 6372 6970 7469 6f6e 203d 2041 206c  escription = A l
-00000100: 6962 7261 7279 2066 6f72 2073 6572 6961  ibrary for seria
-00000110: 6c69 7a69 6e67 204a 534f 4e20 696e 2061  lizing JSON in a
-00000120: 2073 6d61 6c6c 2062 696e 6172 7920 666f   small binary fo
-00000130: 726d 6174 0d0a 7572 6c20 3d20 6874 7470  rmat..url = http
-00000140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000150: 6d6f 6b2d 7365 7277 6973 2f6d 696e 696a  mok-serwis/minij
-00000160: 736f 6e0d 0a70 726f 6a65 6374 5f75 726c  son..project_url
-00000170: 7320 3d20 0d0a 0944 6f63 756d 656e 7461  s = ...Documenta
-00000180: 7469 6f6e 203d 2068 7474 7073 3a2f 2f6d  tion = https://m
-00000190: 696e 696a 736f 6e2e 7265 6164 7468 6564  inijson.readthed
-000001a0: 6f63 732e 696f 2f0d 0a09 436f 6465 203d  ocs.io/...Code =
-000001b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001c0: 636f 6d2f 736d 6f6b 2d73 6572 7769 732f  com/smok-serwis/
-000001d0: 6d69 6e69 6a73 6f6e 0d0a 0949 7373 7565  minijson...Issue
-000001e0: 2074 7261 636b 6572 203d 2068 7474 7073   tracker = https
-000001f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 736d  ://github.com/sm
-00000200: 6f6b 2d73 6572 7769 732f 6d69 6e69 6a73  ok-serwis/minijs
-00000210: 6f6e 2f69 7373 7565 730d 0a63 6c61 7373  on/issues..class
-00000220: 6966 6965 7220 3d20 0d0a 0944 6576 656c  ifier = ...Devel
-00000230: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000240: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
-00000250: 5374 6162 6c65 0d0a 0950 726f 6772 616d  Stable...Program
-00000260: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000270: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
-00000280: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000290: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
-000002a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002c0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000310: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000340: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000350: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000360: 6e20 3a3a 2033 2e31 310d 0a09 5072 6f67  n :: 3.11...Prog
-00000370: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000380: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000390: 3132 0d0a 0950 726f 6772 616d 6d69 6e67  12...Programming
-000003a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000003b0: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-000003c0: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-000003d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000003e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003f0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
-00000400: 696f 6e20 3a3a 2050 7950 790d 0a09 4f70  ion :: PyPy...Op
-00000410: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000420: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000430: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000440: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000450: 5420 4c69 6365 6e73 650d 0a09 546f 7069  T License...Topi
-00000460: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
-00000470: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
-00000480: 7261 7269 6573 0d0a 0d0a 5b70 7963 6f64  raries....[pycod
-00000490: 6573 7479 6c65 5d0d 0a6d 6178 2d6c 696e  estyle]..max-lin
-000004a0: 652d 6c65 6e67 7468 203d 2031 3030 0d0a  e-length = 100..
-000004b0: 0d0a 5b70 6570 385d 0d0a 6d61 782d 6c69  ..[pep8]..max-li
-000004c0: 6e65 2d6c 656e 6774 6820 3d20 3130 300d  ne-length = 100.
-000004d0: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
-000004e0: 0d0a 756e 6976 6572 7361 6c20 3d20 300d  ..universal = 0.
-000004f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
-00000500: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000510: 213d 322e 372e 2a2c 213d 332e 302e 2a2c  !=2.7.*,!=3.0.*,
-00000520: 213d 332e 312e 2a2c 213d 332e 322e 2a2c  !=3.1.*,!=3.2.*,
-00000530: 213d 332e 332e 2a2c 213d 332e 342e 2a0d  !=3.3.*,!=3.4.*.
-00000540: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000550: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000560: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000010: 696f 6e20 3d20 332e 302e 310d 0a6e 616d  ion = 3.0.1..nam
+00000020: 6520 3d20 6d69 6e69 6a73 6f6e 0d0a 6c6f  e = minijson..lo
+00000030: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000040: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+00000050: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000060: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000070: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e3b  = text/markdown;
+00000080: 2063 6861 7273 6574 3d55 5446 2d38 0d0a   charset=UTF-8..
+00000090: 6175 7468 6f72 203d 2050 696f 7472 204d  author = Piotr M
+000000a0: 61c5 9b6c 616e 6b61 0d0a 6c69 6365 6e73  a..lanka..licens
+000000b0: 655f 6669 6c65 7320 3d20 0d0a 094c 4943  e_files = ...LIC
+000000c0: 454e 5345 0d0a 6175 7468 6f72 5f65 6d61  ENSE..author_ema
+000000d0: 696c 203d 2070 696f 7472 2e6d 6173 6c61  il = piotr.masla
+000000e0: 6e6b 6140 6472 6f6e 6568 7562 2e61 690d  nka@dronehub.ai.
+000000f0: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000100: 206c 6962 7261 7279 2066 6f72 2073 6572   library for ser
+00000110: 6961 6c69 7a69 6e67 204a 534f 4e20 696e  ializing JSON in
+00000120: 2061 2073 6d61 6c6c 2062 696e 6172 7920   a small binary 
+00000130: 666f 726d 6174 0d0a 7572 6c20 3d20 6874  format..url = ht
+00000140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000150: 2f73 6d6f 6b2d 7365 7277 6973 2f6d 696e  /smok-serwis/min
+00000160: 696a 736f 6e0d 0a70 726f 6a65 6374 5f75  ijson..project_u
+00000170: 726c 7320 3d20 0d0a 0944 6f63 756d 656e  rls = ...Documen
+00000180: 7461 7469 6f6e 203d 2068 7474 7073 3a2f  tation = https:/
+00000190: 2f6d 696e 696a 736f 6e2e 7265 6164 7468  /minijson.readth
+000001a0: 6564 6f63 732e 696f 2f0d 0a09 436f 6465  edocs.io/...Code
+000001b0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000001c0: 622e 636f 6d2f 736d 6f6b 2d73 6572 7769  b.com/smok-serwi
+000001d0: 732f 6d69 6e69 6a73 6f6e 0d0a 0949 7373  s/minijson...Iss
+000001e0: 7565 2074 7261 636b 6572 203d 2068 7474  ue tracker = htt
+000001f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000200: 736d 6f6b 2d73 6572 7769 732f 6d69 6e69  smok-serwis/mini
+00000210: 6a73 6f6e 2f69 7373 7565 730d 0a63 6c61  json/issues..cla
+00000220: 7373 6966 6965 7220 3d20 0d0a 0944 6576  ssifier = ...Dev
+00000230: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+00000240: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
+00000250: 6e2f 5374 6162 6c65 0d0a 0950 726f 6772  n/Stable...Progr
+00000260: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000270: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002a0: 360d 0a09 5072 6f67 7261 6d6d 696e 6720  6...Programming 
+000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002c0: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002f0: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000310: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000340: 3130 0d0a 0950 726f 6772 616d 6d69 6e67  10...Programming
+00000350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000360: 686f 6e20 3a3a 2033 2e31 310d 0a09 5072  hon :: 3.11...Pr
+00000370: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000380: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000390: 332e 3132 0d0a 0950 726f 6772 616d 6d69  3.12...Programmi
+000003a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003b0: 7974 686f 6e20 3a3a 2049 6d70 6c65 6d65  ython :: Impleme
+000003c0: 6e74 6174 696f 6e20 3a3a 2043 5079 7468  ntation :: CPyth
+000003d0: 6f6e 0d0a 0950 726f 6772 616d 6d69 6e67  on...Programming
+000003e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003f0: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+00000400: 6174 696f 6e20 3a3a 2050 7950 790d 0a09  ation :: PyPy...
+00000410: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000420: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000430: 6e74 0d0a 094c 6963 656e 7365 203a 3a20  nt...License :: 
+00000440: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000450: 4d49 5420 4c69 6365 6e73 650d 0a09 546f  MIT License...To
+00000460: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000470: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000480: 6962 7261 7269 6573 0d0a 0d0a 5b70 7963  ibraries....[pyc
+00000490: 6f64 6573 7479 6c65 5d0d 0a6d 6178 2d6c  odestyle]..max-l
+000004a0: 696e 652d 6c65 6e67 7468 203d 2031 3030  ine-length = 100
+000004b0: 0d0a 0d0a 5b70 6570 385d 0d0a 6d61 782d  ....[pep8]..max-
+000004c0: 6c69 6e65 2d6c 656e 6774 6820 3d20 3130  line-length = 10
+000004d0: 300d 0a0d 0a5b 6264 6973 745f 7768 6565  0....[bdist_whee
+000004e0: 6c5d 0d0a 756e 6976 6572 7361 6c20 3d20  l]..universal = 
+000004f0: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
+00000500: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000510: 3d20 213d 322e 372e 2a2c 213d 332e 302e  = !=2.7.*,!=3.0.
+00000520: 2a2c 213d 332e 312e 2a2c 213d 332e 322e  *,!=3.1.*,!=3.2.
+00000530: 2a2c 213d 332e 332e 2a2c 213d 332e 342e  *,!=3.3.*,!=3.4.
+00000540: 2a0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  *....[egg_info].
+00000550: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000560: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `minijson-3.0/setup.py` & `minijson-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `minijson-3.0/tests/test_minijson.py` & `minijson-3.0.1/tests/test_minijson.py`

 * *Files identical despite different names*

