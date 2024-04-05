# Comparing `tmp/minijson-2.9.tar.gz` & `tmp/minijson-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minijson-2.9.tar", last modified: Fri Aug  6 16:57:23 2021, max compression
+gzip compressed data, was "minijson-3.0.tar", last modified: Fri Apr  5 10:23:31 2024, max compression
```

## Comparing `minijson-2.9.tar` & `minijson-3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:57:23.000000 minijson-2.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2021-08-06 16:57:23.000000 minijson-2.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2021-08-06 16:56:57.000000 minijson-2.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-08-06 16:57:23.000000 minijson-2.9/minijson.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3050 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2021-08-06 16:57:22.000000 minijson-2.9/minijson.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   803310 2021-08-06 16:57:17.000000 minijson-2.9/minijson.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2021-08-06 16:57:23.000000 minijson-2.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2021-08-06 16:56:57.000000 minijson-2.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2021-08-06 16:56:57.000000 minijson-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.347436 minijson-3.0/
+-rw-rw-rw-   0        0        0     1119 2024-04-05 08:25:52.000000 minijson-3.0/LICENSE
+-rw-rw-rw-   0        0        0     3410 2024-04-05 10:23:31.344481 minijson-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2024-04-05 09:24:04.000000 minijson-3.0/README.md
+-rw-rw-rw-   0        0        0  1073249 2024-04-05 10:19:07.000000 minijson-3.0/minijson.c
+drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.338521 minijson-3.0/minijson.egg-info/
+-rw-rw-rw-   0        0        0     3410 2024-04-05 10:23:30.000000 minijson-3.0/minijson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-04-05 10:23:31.000000 minijson-3.0/minijson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 10:23:30.000000 minijson-3.0/minijson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-05 10:23:31.000000 minijson-3.0/minijson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1389 2024-04-05 10:23:31.353291 minijson-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      678 2024-04-05 10:06:36.000000 minijson-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:23:31.333490 minijson-3.0/tests/
+-rw-rw-rw-   0        0        0    10808 2024-04-05 07:56:56.000000 minijson-3.0/tests/test_minijson.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `minijson-2.9/PKG-INFO` & `minijson-3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,43 @@
-Metadata-Version: 2.1
-Name: minijson
-Version: 2.9
-Summary: A library for serializing JSON in a small binary format
-Home-page: https://github.com/Dronehub/minijson
-Author: Piotr Maślanka
-Author-email: piotr.maslanka@dronehub.ai
-License: UNKNOWN
-Project-URL: Documentation, https://minijson.readthedocs.io/
-Project-URL: Code, https://github.com/Dronehub/minijson
-Project-URL: Issue tracker, https://github.com/Dronehub/minijson/issues
-Description: MiniJSON
-        ========
-        
-        [![Build Status](https://travis-ci.com/Dronehub/minijson.svg)](https://travis-ci.com/Dronehub/minijson)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/minijson/test_coverage)
-        [![Issue Count](https://codeclimate.com/github/Dronehub/minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/minijson)
-        [![Documentation Status](https://readthedocs.org/projects/minijson/badge/?version=latest)](http://minijson.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/pyversions/minijson.svg)](https://pypi.python.org/pypi/minijson)
-        [![PyPI version](https://badge.fury.io/py/minijson.svg)](https://badge.fury.io/py/minijson)
-        [![PyPI](https://img.shields.io/pypi/implementation/minijson.svg)](https://pypi.python.org/pypi/minijson)
-        [![PyPI](https://img.shields.io/pypi/wheel/minijson.svg)]()
-        [![License](https://img.shields.io/pypi/l/minijson)](https://github.com/Dronehub/minijson)
-        
-        
-        MiniJSON is a codec for a compact binary representation of a superset of JSON (binary values)
-        are supported.
-        
-        Usage
-        -----
-        
-        Refer to the [documentation](http://minijson.readthedocs.io/en/latest/?badge=latest)
-        for use.
-        
-        If there are no binary wheels precompiled for this platform, you will need to
-        compile it yourself.
-        Alternatively, you can
-        [file an issue](https://github.com/Dronehub/minijson/issues/new)
-        and I'll do my best to compile a wheel for you.
-        
-        In order to do that you must have `Cython` installed.
-        
-        Run the Dockerfile to launch unit tests locally.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: !=2.7.*,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
-Description-Content-Type: text/markdown; charset=UTF-8
+MiniJSON
+========
+
+![Passing CI](https://github.com/smok-serwis/minijson/actions/workflows/main.yml/badge.svg)
+[![Maintainability](https://api.codeclimate.com/v1/badges/20392a075de646680403/maintainability)](https://codeclimate.com/github/smok-serwis/minijson/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/20392a075de646680403/test_coverage)](https://codeclimate.com/github/smok-serwis/minijson/test_coverage)
+[![Issue Count](https://codeclimate.com/github/smok-serwis/minijson/badges/issue_count.svg)](https://codeclimate.com/github/smok-serwis/minijson)
+[![Documentation Status](https://readthedocs.org/projects/minijson/badge/?version=latest)](http://minijson.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/pyversions/minijson.svg)](https://pypi.python.org/pypi/minijson)
+[![PyPI version](https://badge.fury.io/py/minijson.svg)](https://badge.fury.io/py/minijson)
+[![PyPI](https://img.shields.io/pypi/implementation/minijson.svg)](https://pypi.python.org/pypi/minijson)
+[![PyPI](https://img.shields.io/pypi/wheel/minijson.svg)]()
+[![License](https://img.shields.io/pypi/l/minijson)](https://github.com/smok-serwis/minijson)
+
+MiniJSON is a codec for a compact binary representation of a superset of JSON
+(binary values) are supported.
+
+Note
+----
+
+Active development of **minijson** is moved to this fork.
+[Dronehub](https://github.com/Dronehub) has no interest in further developing this awesome
+technology.
+
+Usage
+-----
+
+Refer to the [documentation](http://minijson.readthedocs.io/en/latest/?badge=latest)
+for use.
+
+If there are no binary wheels precompiled for this platform, you will need to
+compile it yourself.
+Alternatively, you can
+[file an issue](https://github.com/Dronehub/minijson/issues/new)
+and I'll do my best to compile a wheel for you.
+
+Compiling own wheels
+--------------------
+
+If there's no wheel, and you'd like to compile it on your own, you'll
+require [Cython](https://cython.org/) installed.
+
+Run the Dockerfile to launch unit tests locally.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `minijson-2.9/setup.cfg` & `minijson-3.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,87 @@
-00000000: 5b6d 6574 6164 6174 615d 0a76 6572 7369  [metadata].versi
-00000010: 6f6e 203d 2032 2e39 0a6e 616d 6520 3d20  on = 2.9.name = 
-00000020: 6d69 6e69 6a73 6f6e 0a6c 6f6e 675f 6465  minijson.long_de
-00000030: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-00000040: 3a20 5245 4144 4d45 2e6d 640a 6c6f 6e67  : README.md.long
-00000050: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-00000060: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000070: 2f6d 6172 6b64 6f77 6e3b 2063 6861 7273  /markdown; chars
-00000080: 6574 3d55 5446 2d38 0a61 7574 686f 7220  et=UTF-8.author 
-00000090: 3d20 5069 6f74 7220 4d61 c59b 6c61 6e6b  = Piotr Ma..lank
-000000a0: 610a 6c69 6365 6e73 655f 6669 6c65 7320  a.license_files 
-000000b0: 3d20 0a09 4c49 4345 4e53 450a 6175 7468  = ..LICENSE.auth
-000000c0: 6f72 5f65 6d61 696c 203d 2070 696f 7472  or_email = piotr
-000000d0: 2e6d 6173 6c61 6e6b 6140 6472 6f6e 6568  .maslanka@droneh
-000000e0: 7562 2e61 690a 6465 7363 7269 7074 696f  ub.ai.descriptio
-000000f0: 6e20 3d20 4120 6c69 6272 6172 7920 666f  n = A library fo
-00000100: 7220 7365 7269 616c 697a 696e 6720 4a53  r serializing JS
-00000110: 4f4e 2069 6e20 6120 736d 616c 6c20 6269  ON in a small bi
-00000120: 6e61 7279 2066 6f72 6d61 740a 7572 6c20  nary format.url 
-00000130: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000140: 2e63 6f6d 2f44 726f 6e65 6875 622f 6d69  .com/Dronehub/mi
-00000150: 6e69 6a73 6f6e 0a70 726f 6a65 6374 5f75  nijson.project_u
-00000160: 726c 7320 3d20 0a09 446f 6375 6d65 6e74  rls = ..Document
-00000170: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
-00000180: 6d69 6e69 6a73 6f6e 2e72 6561 6474 6865  minijson.readthe
-00000190: 646f 6373 2e69 6f2f 0a09 436f 6465 203d  docs.io/..Code =
-000001a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000001b0: 636f 6d2f 4472 6f6e 6568 7562 2f6d 696e  com/Dronehub/min
-000001c0: 696a 736f 6e0a 0949 7373 7565 2074 7261  ijson..Issue tra
-000001d0: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-000001e0: 6974 6875 622e 636f 6d2f 4472 6f6e 6568  ithub.com/Droneh
-000001f0: 7562 2f6d 696e 696a 736f 6e2f 6973 7375  ub/minijson/issu
-00000200: 6573 0a63 6c61 7373 6966 6965 7220 3d20  es.classifier = 
-00000210: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
-00000220: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
-00000230: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000240: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000250: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000270: 203a 3a20 332e 350a 0950 726f 6772 616d   :: 3.5..Program
-00000280: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000290: 2050 7974 686f 6e20 3a3a 2033 2e36 0a09   Python :: 3.6..
-000002a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002c0: 3a20 332e 370a 0950 726f 6772 616d 6d69  : 3.7..Programmi
-000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002e0: 7974 686f 6e20 3a3a 2033 2e38 0a09 5072  ython :: 3.8..Pr
-000002f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000300: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000310: 332e 390a 0950 726f 6772 616d 6d69 6e67  3.9..Programming
-00000320: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000330: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-00000340: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-00000350: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000360: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000370: 203a 3a20 496d 706c 656d 656e 7461 7469   :: Implementati
-00000380: 6f6e 203a 3a20 5079 5079 0a09 4f70 6572  on :: PyPy..Oper
-00000390: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000003a0: 4f53 2049 6e64 6570 656e 6465 6e74 0a09  OS Independent..
-000003b0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000003c0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000003d0: 6963 656e 7365 0a09 546f 7069 6320 3a3a  icense..Topic ::
-000003e0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-000003f0: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
-00000400: 6573 0a0a 5b70 7963 6f64 6573 7479 6c65  es..[pycodestyle
-00000410: 5d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ].max-line-lengt
-00000420: 6820 3d20 3130 300a 0a5b 7065 7038 5d0a  h = 100..[pep8].
-00000430: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-00000440: 3d20 3130 300a 0a5b 6264 6973 745f 7768  = 100..[bdist_wh
-00000450: 6565 6c5d 0a75 6e69 7665 7273 616c 203d  eel].universal =
-00000460: 2030 0a0a 5b6f 7074 696f 6e73 5d0a 7079   0..[options].py
-00000470: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000480: 213d 322e 372e 2a2c 213d 332e 302e 2a2c  !=2.7.*,!=3.0.*,
-00000490: 213d 332e 312e 2a2c 213d 332e 322e 2a2c  !=3.1.*,!=3.2.*,
-000004a0: 213d 332e 332e 2a2c 213d 332e 342e 2a0a  !=3.3.*,!=3.4.*.
-000004b0: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
-000004c0: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
-000004d0: 6520 3d20 300a 0a                        e = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
+00000010: 696f 6e20 3d20 332e 300d 0a6e 616d 6520  ion = 3.0..name 
+00000020: 3d20 6d69 6e69 6a73 6f6e 0d0a 6c6f 6e67  = minijson..long
+00000030: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000040: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000050: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000060: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000070: 7465 7874 2f6d 6172 6b64 6f77 6e3b 2063  text/markdown; c
+00000080: 6861 7273 6574 3d55 5446 2d38 0d0a 6175  harset=UTF-8..au
+00000090: 7468 6f72 203d 2050 696f 7472 204d 61c5  thor = Piotr Ma.
+000000a0: 9b6c 616e 6b61 0d0a 6c69 6365 6e73 655f  .lanka..license_
+000000b0: 6669 6c65 7320 3d20 0d0a 094c 4943 454e  files = ...LICEN
+000000c0: 5345 0d0a 6175 7468 6f72 5f65 6d61 696c  SE..author_email
+000000d0: 203d 2070 696f 7472 2e6d 6173 6c61 6e6b   = piotr.maslank
+000000e0: 6140 6472 6f6e 6568 7562 2e61 690d 0a64  a@dronehub.ai..d
+000000f0: 6573 6372 6970 7469 6f6e 203d 2041 206c  escription = A l
+00000100: 6962 7261 7279 2066 6f72 2073 6572 6961  ibrary for seria
+00000110: 6c69 7a69 6e67 204a 534f 4e20 696e 2061  lizing JSON in a
+00000120: 2073 6d61 6c6c 2062 696e 6172 7920 666f   small binary fo
+00000130: 726d 6174 0d0a 7572 6c20 3d20 6874 7470  rmat..url = http
+00000140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000150: 6d6f 6b2d 7365 7277 6973 2f6d 696e 696a  mok-serwis/minij
+00000160: 736f 6e0d 0a70 726f 6a65 6374 5f75 726c  son..project_url
+00000170: 7320 3d20 0d0a 0944 6f63 756d 656e 7461  s = ...Documenta
+00000180: 7469 6f6e 203d 2068 7474 7073 3a2f 2f6d  tion = https://m
+00000190: 696e 696a 736f 6e2e 7265 6164 7468 6564  inijson.readthed
+000001a0: 6f63 732e 696f 2f0d 0a09 436f 6465 203d  ocs.io/...Code =
+000001b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000001c0: 636f 6d2f 736d 6f6b 2d73 6572 7769 732f  com/smok-serwis/
+000001d0: 6d69 6e69 6a73 6f6e 0d0a 0949 7373 7565  minijson...Issue
+000001e0: 2074 7261 636b 6572 203d 2068 7474 7073   tracker = https
+000001f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 736d  ://github.com/sm
+00000200: 6f6b 2d73 6572 7769 732f 6d69 6e69 6a73  ok-serwis/minijs
+00000210: 6f6e 2f69 7373 7565 730d 0a63 6c61 7373  on/issues..class
+00000220: 6966 6965 7220 3d20 0d0a 0944 6576 656c  ifier = ...Devel
+00000230: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000240: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+00000250: 5374 6162 6c65 0d0a 0950 726f 6772 616d  Stable...Program
+00000260: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000270: 2050 7974 686f 6e0d 0a09 5072 6f67 7261   Python...Progra
+00000280: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000290: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
+000002a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002c0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
+000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000310: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
+00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000340: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000350: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000360: 6e20 3a3a 2033 2e31 310d 0a09 5072 6f67  n :: 3.11...Prog
+00000370: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000380: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000390: 3132 0d0a 0950 726f 6772 616d 6d69 6e67  12...Programming
+000003a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003b0: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+000003c0: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
+000003d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000003e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000003f0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
+00000400: 696f 6e20 3a3a 2050 7950 790d 0a09 4f70  ion :: PyPy...Op
+00000410: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000420: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000430: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+00000440: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000450: 5420 4c69 6365 6e73 650d 0a09 546f 7069  T License...Topi
+00000460: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000470: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000480: 7261 7269 6573 0d0a 0d0a 5b70 7963 6f64  raries....[pycod
+00000490: 6573 7479 6c65 5d0d 0a6d 6178 2d6c 696e  estyle]..max-lin
+000004a0: 652d 6c65 6e67 7468 203d 2031 3030 0d0a  e-length = 100..
+000004b0: 0d0a 5b70 6570 385d 0d0a 6d61 782d 6c69  ..[pep8]..max-li
+000004c0: 6e65 2d6c 656e 6774 6820 3d20 3130 300d  ne-length = 100.
+000004d0: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
+000004e0: 0d0a 756e 6976 6572 7361 6c20 3d20 300d  ..universal = 0.
+000004f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
+00000500: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000510: 213d 322e 372e 2a2c 213d 332e 302e 2a2c  !=2.7.*,!=3.0.*,
+00000520: 213d 332e 312e 2a2c 213d 332e 322e 2a2c  !=3.1.*,!=3.2.*,
+00000530: 213d 332e 332e 2a2c 213d 332e 342e 2a0d  !=3.3.*,!=3.4.*.
+00000540: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000550: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000560: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `minijson-2.9/LICENSE` & `minijson-3.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
 Copyright (c) 2021 Dronehub Group sp. z o. o.
+Copyright (c) 2024 SMOK sp. z o. o.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

