# Comparing `tmp/Xdcheckin-1.5.3.tar.gz` & `tmp/Xdcheckin-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xdcheckin-1.5.3.tar", last modified: Thu Mar 28 01:37:22 2024, max compression
+gzip compressed data, was "Xdcheckin-2.0.1.tar", last modified: Fri Apr  5 14:44:29 2024, max compression
```

## Comparing `Xdcheckin-1.5.3.tar` & `Xdcheckin-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.558842 Xdcheckin-1.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 01:37:22.000000 Xdcheckin-1.5.3/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.562842 Xdcheckin-1.5.3/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.562842 Xdcheckin-1.5.3/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.562842 Xdcheckin-1.5.3/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:37:22.566842 Xdcheckin-1.5.3/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-28 01:37:16.000000 Xdcheckin-1.5.3/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.730143 Xdcheckin-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.730143 Xdcheckin-2.0.1/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33265 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/util/chaoxing_captcha.py
```

### Comparing `Xdcheckin-1.5.3/LICENSE` & `Xdcheckin-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/PKG-INFO` & `Xdcheckin-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 1.5.3
+Version: 2.0.1
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
@@ -14,14 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=3.0.0
 Requires-Dist: flask-session==0.6.0
 Requires-Dist: pillow>=8.4.0
 Requires-Dist: pycryptodome>=3.9.4
+Requires-Dist: pyjsbitwise>=1.0.1
 Requires-Dist: pyzbar>=0.1.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-cache>=1.2.0
 Requires-Dist: waitress>=3.0.0
 
 # Xdcheckin
 Don't use.
```

### Comparing `Xdcheckin-1.5.3/README.md` & `Xdcheckin-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/pyproject.toml` & `Xdcheckin-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 5864 6368 6563 6b69 6e22 0d0a 7665   "Xdcheckin"..ve
-00000080: 7273 696f 6e20 3d20 2231 2e35 2e33 220d  rsion = "1.5.3".
+00000080: 7273 696f 6e20 3d20 2232 2e30 2e31 220d  rsion = "2.0.1".
 00000090: 0a61 7574 686f 7273 203d 205b 0d0a 097b  .authors = [...{
 000000a0: 6e61 6d65 203d 2022 5061 6972 6d61 6e22  name = "Pairman"
 000000b0: 2c20 656d 6169 6c20 3d20 2270 6169 726d  , email = "pairm
 000000c0: 616e 786c 7240 676d 6169 6c2e 636f 6d22  anxlr@gmail.com"
 000000d0: 7d0d 0a5d 0d0a 7265 6164 6d65 203d 2022  }..]..readme = "
 000000e0: 5245 4144 4d45 2e6d 6422 0d0a 6465 7363  README.md"..desc
 000000f0: 7269 7074 696f 6e20 3d20 2243 6861 6f78  ription = "Chaox
@@ -39,324 +39,327 @@
 00000260: 223e 3d33 2e38 220d 0a64 6570 656e 6465  ">=3.8"..depende
 00000270: 6e63 6965 7320 3d20 5b0d 0a09 2266 6c61  ncies = [..."fla
 00000280: 736b 203e 3d20 332e 302e 3022 2c0d 0a09  sk >= 3.0.0",...
 00000290: 2266 6c61 736b 2d73 6573 7369 6f6e 203d  "flask-session =
 000002a0: 3d20 302e 362e 3022 2c0d 0a09 2270 696c  = 0.6.0",..."pil
 000002b0: 6c6f 7720 3e3d 2038 2e34 2e30 222c 0d0a  low >= 8.4.0",..
 000002c0: 0922 7079 6372 7970 746f 646f 6d65 203e  ."pycryptodome >
-000002d0: 3d20 332e 392e 3422 2c0d 0a09 2270 797a  = 3.9.4",..."pyz
-000002e0: 6261 7220 3e3d 2030 2e31 2e38 222c 0d0a  bar >= 0.1.8",..
-000002f0: 0922 7265 7175 6573 7473 203e 3d20 322e  ."requests >= 2.
-00000300: 3331 2e30 222c 0d0a 0922 7265 7175 6573  31.0",..."reques
-00000310: 7473 2d63 6163 6865 203e 3d20 312e 322e  ts-cache >= 1.2.
-00000320: 3022 2c0d 0a09 2277 6169 7472 6573 7320  0",..."waitress 
-00000330: 3e3d 2033 2e30 2e30 222c 0d0a 5d0d 0a0d  >= 3.0.0",..]...
-00000340: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000350: 0a48 6f6d 6570 6167 6520 3d20 2268 7474  .Homepage = "htt
-00000360: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000370: 5061 6972 6d61 6e2f 5864 6368 6563 6b69  Pairman/Xdchecki
-00000380: 6e22 0d0a 4368 616e 6765 6c6f 6720 3d20  n"..Changelog = 
-00000390: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000003a0: 636f 6d2f 5061 6972 6d61 6e2f 5864 6368  com/Pairman/Xdch
-000003b0: 6563 6b69 6e2f 626c 6f62 2f6d 6169 6e2f  eckin/blob/main/
-000003c0: 4348 414e 4745 4c4f 472e 6d64 220d 0a0d  CHANGELOG.md"...
-000003d0: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
-000003e0: 735d 0d0a 7864 6368 6563 6b69 6e2d 7365  s]..xdcheckin-se
-000003f0: 7276 6572 203d 2022 7864 6368 6563 6b69  rver = "xdchecki
-00000400: 6e2e 7365 7276 6572 2e73 6572 7665 723a  n.server.server:
-00000410: 6d61 696e 220d 0a0d 0a5b 746f 6f6c 2e73  main"....[tool.s
-00000420: 6574 7570 746f 6f6c 732e 7061 636b 6167  etuptools.packag
-00000430: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000440: 3d20 5b22 7372 6322 5d0d 0a69 6e63 6c75  = ["src"]..inclu
-00000450: 6465 203d 205b 0d0a 0922 7864 6368 6563  de = [..."xdchec
-00000460: 6b69 6e2a 222c 0d0a 0922 7864 6368 6563  kin*",..."xdchec
-00000470: 6b69 6e2e 636f 7265 2a22 2c0d 0a09 2278  kin.core*",..."x
-00000480: 6463 6865 636b 696e 2e73 6572 7665 722a  dcheckin.server*
-00000490: 222c 0d0a 5d0d 0a65 7863 6c75 6465 203d  ",..]..exclude =
-000004a0: 205b 0d0a 0922 7864 6368 6563 6b69 6e2e   [..."xdcheckin.
-000004b0: 6170 702a 222c 0d0a 0922 7864 6368 6563  app*",..."xdchec
-000004c0: 6b69 6e2e 5f5f 6d61 696e 5f5f 222c 0d0a  kin.__main__",..
-000004d0: 205d 0d0a 0d0a 5b74 6f6f 6c2e 7365 7475   ]....[tool.setu
-000004e0: 7074 6f6f 6c73 2e70 6163 6b61 6765 2d64  ptools.package-d
-000004f0: 6174 615d 0d0a 2278 6463 6865 636b 696e  ata].."xdcheckin
-00000500: 2e73 6572 7665 7222 203d 205b 2273 7461  .server" = ["sta
-00000510: 7469 632f 2a22 2c20 2274 656d 706c 6174  tic/*", "templat
-00000520: 6573 2f2a 225d 0d0a 0d0a 5b74 6f6f 6c2e  es/*"]....[tool.
-00000530: 6272 6965 6663 6173 655d 0d0a 7072 6f6a  briefcase]..proj
-00000540: 6563 745f 6e61 6d65 203d 2022 5864 6368  ect_name = "Xdch
-00000550: 6563 6b69 6e22 0d0a 6275 6e64 6c65 203d  eckin"..bundle =
-00000560: 2022 6f72 672e 6575 2e70 6e78 6c72 2e67   "org.eu.pnxlr.g
-00000570: 6974 220d 0a0d 0a5b 746f 6f6c 2e62 7269  it"....[tool.bri
-00000580: 6566 6361 7365 2e61 7070 2e78 6463 6865  efcase.app.xdche
-00000590: 636b 696e 5d0d 0a66 6f72 6d61 6c5f 6e61  ckin]..formal_na
-000005a0: 6d65 203d 2022 5864 6368 6563 6b69 6e22  me = "Xdcheckin"
-000005b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000005c0: 6f6e 203d 2022 2222 4368 616f 7869 6e67  on = """Chaoxing
-000005d0: 2043 6865 636b 696e 2054 6f6f 6c20 666f   Checkin Tool fo
-000005e0: 7220 5844 552e 0d0a 2222 220d 0a69 636f  r XDU..."""..ico
-000005f0: 6e20 3d20 2273 7263 2f78 6463 6865 636b  n = "src/xdcheck
-00000600: 696e 2f61 7070 2f72 6573 6f75 7263 6573  in/app/resources
-00000610: 2f78 6463 6865 636b 696e 220d 0a73 6f75  /xdcheckin"..sou
-00000620: 7263 6573 203d 205b 0d0a 0922 7372 632f  rces = [..."src/
-00000630: 7864 6368 6563 6b69 6e22 2c0d 0a5d 0d0a  xdcheckin",..]..
-00000640: 2320 7465 7374 5f73 6f75 7263 6573 203d  # test_sources =
-00000650: 205b 5d0d 0a72 6571 7569 7265 7320 3d20   []..requires = 
-00000660: 5b0d 0a09 2266 6c61 736b 203e 3d20 332e  [..."flask >= 3.
-00000670: 302e 3022 2c0d 0a09 2266 6c61 736b 2d73  0.0",..."flask-s
-00000680: 6573 7369 6f6e 203d 3d20 302e 362e 3022  ession == 0.6.0"
-00000690: 2c0d 0a09 2270 696c 6c6f 7720 3e3d 2038  ,..."pillow >= 8
-000006a0: 2e34 2e30 222c 0d0a 0922 7079 6372 7970  .4.0",..."pycryp
-000006b0: 746f 646f 6d65 203e 3d20 332e 392e 3422  todome >= 3.9.4"
-000006c0: 2c0d 0a09 2270 797a 6261 7220 3e3d 2030  ,..."pyzbar >= 0
-000006d0: 2e31 2e38 222c 0d0a 0922 7265 7175 6573  .1.8",..."reques
-000006e0: 7473 203e 3d20 322e 3331 2e30 222c 0d0a  ts >= 2.31.0",..
-000006f0: 0922 7265 7175 6573 7473 2d63 6163 6865  ."requests-cache
-00000700: 203e 3d20 312e 322e 3022 2c0d 0a09 2277   >= 1.2.0",..."w
-00000710: 6169 7472 6573 7320 3e3d 2033 2e30 2e30  aitress >= 3.0.0
-00000720: 222c 0d0a 5d0d 0a23 2074 6573 745f 7265  ",..]..# test_re
-00000730: 7175 6972 6573 203d 205b 5d0d 0a0d 0a5b  quires = []....[
-00000740: 746f 6f6c 2e62 7269 6566 6361 7365 2e61  tool.briefcase.a
-00000750: 7070 2e78 6463 6865 636b 696e 2e6d 6163  pp.xdcheckin.mac
-00000760: 4f53 5d0d 0a75 6e69 7665 7273 616c 5f62  OS]..universal_b
-00000770: 7569 6c64 203d 2074 7275 650d 0a72 6571  uild = true..req
-00000780: 7569 7265 7320 3d20 5b0d 0a09 2274 6f67  uires = [..."tog
-00000790: 612d 636f 636f 617e 3d30 2e34 2e30 222c  a-cocoa~=0.4.0",
-000007a0: 0d0a 0922 7374 642d 6e73 6c6f 677e 3d31  ..."std-nslog~=1
-000007b0: 2e30 2e30 222c 0d0a 5d0d 0a0d 0a5b 746f  .0.0",..]....[to
-000007c0: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
-000007d0: 2e78 6463 6865 636b 696e 2e6c 696e 7578  .xdcheckin.linux
-000007e0: 5d0d 0a72 6571 7569 7265 7320 3d20 5b0d  ]..requires = [.
-000007f0: 0a09 2274 6f67 612d 6774 6b7e 3d30 2e34  .."toga-gtk~=0.4
-00000800: 2e30 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  .0",..]....[tool
-00000810: 2e62 7269 6566 6361 7365 2e61 7070 2e78  .briefcase.app.x
-00000820: 6463 6865 636b 696e 2e6c 696e 7578 2e73  dcheckin.linux.s
-00000830: 7973 7465 6d2e 6465 6269 616e 5d0d 0a73  ystem.debian]..s
-00000840: 7973 7465 6d5f 7265 7175 6972 6573 203d  ystem_requires =
-00000850: 205b 0d0a 0923 204e 6565 6465 6420 746f   [...# Needed to
-00000860: 2063 6f6d 7069 6c65 2070 7963 6169 726f   compile pycairo
-00000870: 2077 6865 656c 0d0a 0922 6c69 6263 6169   wheel..."libcai
-00000880: 726f 322d 6465 7622 2c0d 0a09 2320 4e65  ro2-dev",...# Ne
-00000890: 6564 6564 2074 6f20 636f 6d70 696c 6520  eded to compile 
-000008a0: 5079 474f 626a 6563 7420 7768 6565 6c0d  PyGObject wheel.
-000008b0: 0a09 226c 6962 6769 7265 706f 7369 746f  .."libgireposito
-000008c0: 7279 312e 302d 6465 7622 2c0d 0a5d 0d0a  ry1.0-dev",..]..
-000008d0: 0d0a 7379 7374 656d 5f72 756e 7469 6d65  ..system_runtime
-000008e0: 5f72 6571 7569 7265 7320 3d20 5b0d 0a09  _requires = [...
-000008f0: 2320 4e65 6564 6564 2074 6f20 7072 6f76  # Needed to prov
-00000900: 6964 6520 4754 4b20 616e 6420 6974 7320  ide GTK and its 
-00000910: 4749 2062 696e 6469 6e67 730d 0a09 2267  GI bindings..."g
-00000920: 6972 312e 322d 6774 6b2d 332e 3022 2c0d  ir1.2-gtk-3.0",.
-00000930: 0a09 226c 6962 6769 7265 706f 7369 746f  .."libgireposito
-00000940: 7279 2d31 2e30 2d31 222c 0d0a 0923 2044  ry-1.0-1",...# D
-00000950: 6570 656e 6465 6e63 6965 7320 7468 6174  ependencies that
-00000960: 2047 544b 206c 6f6f 6b73 2066 6f72 2061   GTK looks for a
-00000970: 7420 7275 6e74 696d 650d 0a09 226c 6962  t runtime..."lib
-00000980: 6361 6e62 6572 7261 2d67 746b 332d 6d6f  canberra-gtk3-mo
-00000990: 6475 6c65 222c 0d0a 0923 204e 6565 6465  dule",...# Neede
-000009a0: 6420 746f 2070 726f 7669 6465 2057 6562  d to provide Web
-000009b0: 4b69 7432 2061 7420 7275 6e74 696d 650d  Kit2 at runtime.
-000009c0: 0a09 2320 2267 6972 312e 322d 7765 626b  ..# "gir1.2-webk
-000009d0: 6974 322d 342e 3022 2c0d 0a09 2320 4e65  it2-4.0",...# Ne
-000009e0: 6564 6564 2066 6f72 2070 797a 6261 7220  eded for pyzbar 
-000009f0: 6174 2072 756e 7469 6d65 0d0a 0922 6c69  at runtime..."li
-00000a00: 627a 6261 7230 222c 0d0a 5d0d 0a0d 0a5b  bzbar0",..]....[
-00000a10: 746f 6f6c 2e62 7269 6566 6361 7365 2e61  tool.briefcase.a
-00000a20: 7070 2e78 6463 6865 636b 696e 2e6c 696e  pp.xdcheckin.lin
-00000a30: 7578 2e73 7973 7465 6d2e 7268 656c 5d0d  ux.system.rhel].
-00000a40: 0a73 7973 7465 6d5f 7265 7175 6972 6573  .system_requires
-00000a50: 203d 205b 0d0a 0923 204e 6565 6465 6420   = [...# Needed 
-00000a60: 746f 2063 6f6d 7069 6c65 2070 7963 6169  to compile pycai
-00000a70: 726f 2077 6865 656c 0d0a 0922 6361 6972  ro wheel..."cair
-00000a80: 6f2d 676f 626a 6563 742d 6465 7665 6c22  o-gobject-devel"
-00000a90: 2c0d 0a09 2320 4e65 6564 6564 2074 6f20  ,...# Needed to 
-00000aa0: 636f 6d70 696c 6520 5079 474f 626a 6563  compile PyGObjec
-00000ab0: 7420 7768 6565 6c0d 0a09 2267 6f62 6a65  t wheel..."gobje
-00000ac0: 6374 2d69 6e74 726f 7370 6563 7469 6f6e  ct-introspection
-00000ad0: 2d64 6576 656c 222c 0d0a 5d0d 0a0d 0a73  -devel",..]....s
-00000ae0: 7973 7465 6d5f 7275 6e74 696d 655f 7265  ystem_runtime_re
-00000af0: 7175 6972 6573 203d 205b 0d0a 0923 204e  quires = [...# N
-00000b00: 6565 6465 6420 746f 2073 7570 706f 7274  eeded to support
-00000b10: 2050 7974 686f 6e20 6269 6e64 696e 6773   Python bindings
-00000b20: 2074 6f20 4754 4b0d 0a09 2267 6f62 6a65   to GTK..."gobje
-00000b30: 6374 2d69 6e74 726f 7370 6563 7469 6f6e  ct-introspection
-00000b40: 222c 0d0a 0923 204e 6565 6465 6420 746f  ",...# Needed to
-00000b50: 2070 726f 7669 6465 2047 544b 0d0a 0922   provide GTK..."
-00000b60: 6774 6b33 222c 0d0a 0923 2044 6570 656e  gtk3",...# Depen
-00000b70: 6465 6e63 6965 7320 7468 6174 2047 544b  dencies that GTK
-00000b80: 206c 6f6f 6b73 2066 6f72 2061 7420 7275   looks for at ru
-00000b90: 6e74 696d 650d 0a09 226c 6962 6361 6e62  ntime..."libcanb
-00000ba0: 6572 7261 2d67 746b 3322 2c0d 0a09 2320  erra-gtk3",...# 
-00000bb0: 4e65 6564 6564 2074 6f20 7072 6f76 6964  Needed to provid
-00000bc0: 6520 5765 624b 6974 3220 6174 2072 756e  e WebKit2 at run
-00000bd0: 7469 6d65 0d0a 0923 2022 7765 626b 6974  time...# "webkit
-00000be0: 3267 746b 3322 2c0d 0a09 2320 4e65 6564  2gtk3",...# Need
-00000bf0: 6564 2066 6f72 2070 797a 6261 7220 6174  ed for pyzbar at
-00000c00: 2072 756e 7469 6d65 0d0a 0922 7a62 6172   runtime..."zbar
-00000c10: 2d6c 6962 7322 2c0d 0a5d 0d0a 0d0a 5b74  -libs",..]....[t
-00000c20: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
-00000c30: 702e 7864 6368 6563 6b69 6e2e 6c69 6e75  p.xdcheckin.linu
-00000c40: 782e 7379 7374 656d 2e73 7573 655d 0d0a  x.system.suse]..
-00000c50: 7379 7374 656d 5f72 6571 7569 7265 7320  system_requires 
-00000c60: 3d20 5b0d 0a09 2320 4e65 6564 6564 2074  = [...# Needed t
-00000c70: 6f20 636f 6d70 696c 6520 7079 6361 6972  o compile pycair
-00000c80: 6f20 7768 6565 6c0d 0a09 2263 6169 726f  o wheel..."cairo
-00000c90: 2d64 6576 656c 222c 0d0a 0923 204e 6565  -devel",...# Nee
-00000ca0: 6465 6420 746f 2063 6f6d 7069 6c65 2050  ded to compile P
-00000cb0: 7947 4f62 6a65 6374 2077 6865 656c 0d0a  yGObject wheel..
-00000cc0: 0922 676f 626a 6563 742d 696e 7472 6f73  ."gobject-intros
-00000cd0: 7065 6374 696f 6e2d 6465 7665 6c22 2c0d  pection-devel",.
-00000ce0: 0a5d 0d0a 0d0a 7379 7374 656d 5f72 756e  .]....system_run
-00000cf0: 7469 6d65 5f72 6571 7569 7265 7320 3d20  time_requires = 
-00000d00: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
-00000d10: 7072 6f76 6964 6520 4754 4b0d 0a09 2267  provide GTK..."g
-00000d20: 746b 3322 2c0d 0a09 2320 4e65 6564 6564  tk3",...# Needed
-00000d30: 2074 6f20 7375 7070 6f72 7420 5079 7468   to support Pyth
-00000d40: 6f6e 2062 696e 6469 6e67 7320 746f 2047  on bindings to G
-00000d50: 544b 0d0a 0922 676f 626a 6563 742d 696e  TK..."gobject-in
-00000d60: 7472 6f73 7065 6374 696f 6e22 2c20 2274  trospection", "t
-00000d70: 7970 656c 6962 2847 746b 293d 332e 3022  ypelib(Gtk)=3.0"
-00000d80: 2c0d 0a09 2320 4465 7065 6e64 656e 6369  ,...# Dependenci
-00000d90: 6573 2074 6861 7420 4754 4b20 6c6f 6f6b  es that GTK look
-00000da0: 7320 666f 7220 6174 2072 756e 7469 6d65  s for at runtime
-00000db0: 0d0a 0922 6c69 6263 616e 6265 7272 612d  ..."libcanberra-
-00000dc0: 6774 6b33 2d30 222c 0d0a 0923 204e 6565  gtk3-0",...# Nee
-00000dd0: 6465 6420 746f 2070 726f 7669 6465 2057  ded to provide W
-00000de0: 6562 4b69 7432 2061 7420 7275 6e74 696d  ebKit2 at runtim
-00000df0: 650d 0a09 2320 226c 6962 7765 626b 6974  e...# "libwebkit
-00000e00: 3267 746b 3322 2c0d 0a09 2320 2274 7970  2gtk3",...# "typ
-00000e10: 656c 6962 2857 6562 4b69 7432 2922 2c0d  elib(WebKit2)",.
-00000e20: 0a09 2320 4e65 6564 6564 2066 6f72 2070  ..# Needed for p
-00000e30: 797a 6261 7220 6174 2072 756e 7469 6d65  yzbar at runtime
-00000e40: 0d0a 0922 6c69 627a 6261 7230 222c 0d0a  ..."libzbar0",..
-00000e50: 5d0d 0a0d 0a5b 746f 6f6c 2e62 7269 6566  ]....[tool.brief
-00000e60: 6361 7365 2e61 7070 2e78 6463 6865 636b  case.app.xdcheck
-00000e70: 696e 2e6c 696e 7578 2e73 7973 7465 6d2e  in.linux.system.
-00000e80: 6172 6368 5d0d 0a73 7973 7465 6d5f 7265  arch]..system_re
-00000e90: 7175 6972 6573 203d 205b 0d0a 0923 204e  quires = [...# N
-00000ea0: 6565 6465 6420 746f 2063 6f6d 7069 6c65  eeded to compile
-00000eb0: 2070 7963 6169 726f 2077 6865 656c 0d0a   pycairo wheel..
-00000ec0: 0922 6361 6972 6f22 2c0d 0a09 2320 4e65  ."cairo",...# Ne
+000002d0: 3d20 332e 392e 3422 2c0d 0a09 2270 796a  = 3.9.4",..."pyj
+000002e0: 7362 6974 7769 7365 203e 3d20 312e 302e  sbitwise >= 1.0.
+000002f0: 3122 2c0d 0a09 2270 797a 6261 7220 3e3d  1",..."pyzbar >=
+00000300: 2030 2e31 2e38 222c 0d0a 0922 7265 7175   0.1.8",..."requ
+00000310: 6573 7473 203e 3d20 322e 3331 2e30 222c  ests >= 2.31.0",
+00000320: 0d0a 0922 7265 7175 6573 7473 2d63 6163  ..."requests-cac
+00000330: 6865 203e 3d20 312e 322e 3022 2c0d 0a09  he >= 1.2.0",...
+00000340: 2277 6169 7472 6573 7320 3e3d 2033 2e30  "waitress >= 3.0
+00000350: 2e30 222c 0d0a 5d0d 0a0d 0a5b 7072 6f6a  .0",..]....[proj
+00000360: 6563 742e 7572 6c73 5d0d 0a48 6f6d 6570  ect.urls]..Homep
+00000370: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
+00000380: 6974 6875 622e 636f 6d2f 5061 6972 6d61  ithub.com/Pairma
+00000390: 6e2f 5864 6368 6563 6b69 6e22 0d0a 4368  n/Xdcheckin"..Ch
+000003a0: 616e 6765 6c6f 6720 3d20 2268 7474 7073  angelog = "https
+000003b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+000003c0: 6972 6d61 6e2f 5864 6368 6563 6b69 6e2f  irman/Xdcheckin/
+000003d0: 626c 6f62 2f6d 6169 6e2f 4348 414e 4745  blob/main/CHANGE
+000003e0: 4c4f 472e 6d64 220d 0a0d 0a5b 7072 6f6a  LOG.md"....[proj
+000003f0: 6563 742e 7363 7269 7074 735d 0d0a 7864  ect.scripts]..xd
+00000400: 6368 6563 6b69 6e2d 7365 7276 6572 203d  checkin-server =
+00000410: 2022 7864 6368 6563 6b69 6e2e 7365 7276   "xdcheckin.serv
+00000420: 6572 2e73 6572 7665 723a 6d61 696e 220d  er.server:main".
+00000430: 0a0d 0a5b 746f 6f6c 2e73 6574 7570 746f  ...[tool.setupto
+00000440: 6f6c 732e 7061 636b 6167 6573 2e66 696e  ols.packages.fin
+00000450: 645d 0d0a 7768 6572 6520 3d20 5b22 7372  d]..where = ["sr
+00000460: 6322 5d0d 0a69 6e63 6c75 6465 203d 205b  c"]..include = [
+00000470: 0d0a 0922 7864 6368 6563 6b69 6e2a 222c  ..."xdcheckin*",
+00000480: 0d0a 0922 7864 6368 6563 6b69 6e2e 636f  ..."xdcheckin.co
+00000490: 7265 2a22 2c0d 0a09 2278 6463 6865 636b  re*",..."xdcheck
+000004a0: 696e 2e73 6572 7665 722a 222c 0d0a 0922  in.server*",..."
+000004b0: 7864 6368 6563 6b69 6e2e 7574 696c 2a22  xdcheckin.util*"
+000004c0: 2c0d 0a5d 0d0a 6578 636c 7564 6520 3d20  ,..]..exclude = 
+000004d0: 5b0d 0a09 2278 6463 6865 636b 696e 2e61  [..."xdcheckin.a
+000004e0: 7070 2a22 2c0d 0a09 2278 6463 6865 636b  pp*",..."xdcheck
+000004f0: 696e 2e5f 5f6d 6169 6e5f 5f22 2c0d 0a20  in.__main__",.. 
+00000500: 5d0d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  ]....[tool.setup
+00000510: 746f 6f6c 732e 7061 636b 6167 652d 6461  tools.package-da
+00000520: 7461 5d0d 0a22 7864 6368 6563 6b69 6e2e  ta].."xdcheckin.
+00000530: 7365 7276 6572 2220 3d20 5b22 7374 6174  server" = ["stat
+00000540: 6963 2f2a 222c 2022 7465 6d70 6c61 7465  ic/*", "template
+00000550: 732f 2a22 5d0d 0a0d 0a5b 746f 6f6c 2e62  s/*"]....[tool.b
+00000560: 7269 6566 6361 7365 5d0d 0a70 726f 6a65  riefcase]..proje
+00000570: 6374 5f6e 616d 6520 3d20 2258 6463 6865  ct_name = "Xdche
+00000580: 636b 696e 220d 0a62 756e 646c 6520 3d20  ckin"..bundle = 
+00000590: 226f 7267 2e65 752e 706e 786c 722e 6769  "org.eu.pnxlr.gi
+000005a0: 7422 0d0a 0d0a 5b74 6f6f 6c2e 6272 6965  t"....[tool.brie
+000005b0: 6663 6173 652e 6170 702e 7864 6368 6563  fcase.app.xdchec
+000005c0: 6b69 6e5d 0d0a 666f 726d 616c 5f6e 616d  kin]..formal_nam
+000005d0: 6520 3d20 2258 6463 6865 636b 696e 220d  e = "Xdcheckin".
+000005e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000005f0: 6e20 3d20 2222 2243 6861 6f78 696e 6720  n = """Chaoxing 
+00000600: 4368 6563 6b69 6e20 546f 6f6c 2066 6f72  Checkin Tool for
+00000610: 2058 4455 2e0d 0a22 2222 0d0a 6963 6f6e   XDU..."""..icon
+00000620: 203d 2022 7372 632f 7864 6368 6563 6b69   = "src/xdchecki
+00000630: 6e2f 6170 702f 7265 736f 7572 6365 732f  n/app/resources/
+00000640: 7864 6368 6563 6b69 6e22 0d0a 736f 7572  xdcheckin"..sour
+00000650: 6365 7320 3d20 5b0d 0a09 2273 7263 2f78  ces = [..."src/x
+00000660: 6463 6865 636b 696e 222c 0d0a 5d0d 0a23  dcheckin",..]..#
+00000670: 2074 6573 745f 736f 7572 6365 7320 3d20   test_sources = 
+00000680: 5b5d 0d0a 7265 7175 6972 6573 203d 205b  []..requires = [
+00000690: 0d0a 0922 666c 6173 6b20 3e3d 2033 2e30  ..."flask >= 3.0
+000006a0: 2e30 222c 0d0a 0922 666c 6173 6b2d 7365  .0",..."flask-se
+000006b0: 7373 696f 6e20 3d3d 2030 2e36 2e30 222c  ssion == 0.6.0",
+000006c0: 0d0a 0922 7069 6c6c 6f77 203e 3d20 382e  ..."pillow >= 8.
+000006d0: 342e 3022 2c0d 0a09 2270 7963 7279 7074  4.0",..."pycrypt
+000006e0: 6f64 6f6d 6520 3e3d 2033 2e39 2e34 222c  odome >= 3.9.4",
+000006f0: 0d0a 0922 7079 7a62 6172 203e 3d20 302e  ..."pyzbar >= 0.
+00000700: 312e 3822 2c0d 0a09 2272 6571 7565 7374  1.8",..."request
+00000710: 7320 3e3d 2032 2e33 312e 3022 2c0d 0a09  s >= 2.31.0",...
+00000720: 2272 6571 7565 7374 732d 6361 6368 6520  "requests-cache 
+00000730: 3e3d 2031 2e32 2e30 222c 0d0a 0922 7761  >= 1.2.0",..."wa
+00000740: 6974 7265 7373 203e 3d20 332e 302e 3022  itress >= 3.0.0"
+00000750: 2c0d 0a5d 0d0a 2320 7465 7374 5f72 6571  ,..]..# test_req
+00000760: 7569 7265 7320 3d20 5b5d 0d0a 0d0a 5b74  uires = []....[t
+00000770: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
+00000780: 702e 7864 6368 6563 6b69 6e2e 6d61 634f  p.xdcheckin.macO
+00000790: 535d 0d0a 756e 6976 6572 7361 6c5f 6275  S]..universal_bu
+000007a0: 696c 6420 3d20 7472 7565 0d0a 7265 7175  ild = true..requ
+000007b0: 6972 6573 203d 205b 0d0a 0922 746f 6761  ires = [..."toga
+000007c0: 2d63 6f63 6f61 7e3d 302e 342e 3022 2c0d  -cocoa~=0.4.0",.
+000007d0: 0a09 2273 7464 2d6e 736c 6f67 7e3d 312e  .."std-nslog~=1.
+000007e0: 302e 3022 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  0.0",..]....[too
+000007f0: 6c2e 6272 6965 6663 6173 652e 6170 702e  l.briefcase.app.
+00000800: 7864 6368 6563 6b69 6e2e 6c69 6e75 785d  xdcheckin.linux]
+00000810: 0d0a 7265 7175 6972 6573 203d 205b 0d0a  ..requires = [..
+00000820: 0922 746f 6761 2d67 746b 7e3d 302e 342e  ."toga-gtk~=0.4.
+00000830: 3022 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e  0",..]....[tool.
+00000840: 6272 6965 6663 6173 652e 6170 702e 7864  briefcase.app.xd
+00000850: 6368 6563 6b69 6e2e 6c69 6e75 782e 7379  checkin.linux.sy
+00000860: 7374 656d 2e64 6562 6961 6e5d 0d0a 7379  stem.debian]..sy
+00000870: 7374 656d 5f72 6571 7569 7265 7320 3d20  stem_requires = 
+00000880: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
+00000890: 636f 6d70 696c 6520 7079 6361 6972 6f20  compile pycairo 
+000008a0: 7768 6565 6c0d 0a09 226c 6962 6361 6972  wheel..."libcair
+000008b0: 6f32 2d64 6576 222c 0d0a 0923 204e 6565  o2-dev",...# Nee
+000008c0: 6465 6420 746f 2063 6f6d 7069 6c65 2050  ded to compile P
+000008d0: 7947 4f62 6a65 6374 2077 6865 656c 0d0a  yGObject wheel..
+000008e0: 0922 6c69 6267 6972 6570 6f73 6974 6f72  ."libgirepositor
+000008f0: 7931 2e30 2d64 6576 222c 0d0a 5d0d 0a0d  y1.0-dev",..]...
+00000900: 0a73 7973 7465 6d5f 7275 6e74 696d 655f  .system_runtime_
+00000910: 7265 7175 6972 6573 203d 205b 0d0a 0923  requires = [...#
+00000920: 204e 6565 6465 6420 746f 2070 726f 7669   Needed to provi
+00000930: 6465 2047 544b 2061 6e64 2069 7473 2047  de GTK and its G
+00000940: 4920 6269 6e64 696e 6773 0d0a 0922 6769  I bindings..."gi
+00000950: 7231 2e32 2d67 746b 2d33 2e30 222c 0d0a  r1.2-gtk-3.0",..
+00000960: 0922 6c69 6267 6972 6570 6f73 6974 6f72  ."libgirepositor
+00000970: 792d 312e 302d 3122 2c0d 0a09 2320 4465  y-1.0-1",...# De
+00000980: 7065 6e64 656e 6369 6573 2074 6861 7420  pendencies that 
+00000990: 4754 4b20 6c6f 6f6b 7320 666f 7220 6174  GTK looks for at
+000009a0: 2072 756e 7469 6d65 0d0a 0922 6c69 6263   runtime..."libc
+000009b0: 616e 6265 7272 612d 6774 6b33 2d6d 6f64  anberra-gtk3-mod
+000009c0: 756c 6522 2c0d 0a09 2320 4e65 6564 6564  ule",...# Needed
+000009d0: 2074 6f20 7072 6f76 6964 6520 5765 624b   to provide WebK
+000009e0: 6974 3220 6174 2072 756e 7469 6d65 0d0a  it2 at runtime..
+000009f0: 0923 2022 6769 7231 2e32 2d77 6562 6b69  .# "gir1.2-webki
+00000a00: 7432 2d34 2e30 222c 0d0a 0923 204e 6565  t2-4.0",...# Nee
+00000a10: 6465 6420 666f 7220 7079 7a62 6172 2061  ded for pyzbar a
+00000a20: 7420 7275 6e74 696d 650d 0a09 226c 6962  t runtime..."lib
+00000a30: 7a62 6172 3022 2c0d 0a5d 0d0a 0d0a 5b74  zbar0",..]....[t
+00000a40: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
+00000a50: 702e 7864 6368 6563 6b69 6e2e 6c69 6e75  p.xdcheckin.linu
+00000a60: 782e 7379 7374 656d 2e72 6865 6c5d 0d0a  x.system.rhel]..
+00000a70: 7379 7374 656d 5f72 6571 7569 7265 7320  system_requires 
+00000a80: 3d20 5b0d 0a09 2320 4e65 6564 6564 2074  = [...# Needed t
+00000a90: 6f20 636f 6d70 696c 6520 7079 6361 6972  o compile pycair
+00000aa0: 6f20 7768 6565 6c0d 0a09 2263 6169 726f  o wheel..."cairo
+00000ab0: 2d67 6f62 6a65 6374 2d64 6576 656c 222c  -gobject-devel",
+00000ac0: 0d0a 0923 204e 6565 6465 6420 746f 2063  ...# Needed to c
+00000ad0: 6f6d 7069 6c65 2050 7947 4f62 6a65 6374  ompile PyGObject
+00000ae0: 2077 6865 656c 0d0a 0922 676f 626a 6563   wheel..."gobjec
+00000af0: 742d 696e 7472 6f73 7065 6374 696f 6e2d  t-introspection-
+00000b00: 6465 7665 6c22 2c0d 0a5d 0d0a 0d0a 7379  devel",..]....sy
+00000b10: 7374 656d 5f72 756e 7469 6d65 5f72 6571  stem_runtime_req
+00000b20: 7569 7265 7320 3d20 5b0d 0a09 2320 4e65  uires = [...# Ne
+00000b30: 6564 6564 2074 6f20 7375 7070 6f72 7420  eded to support 
+00000b40: 5079 7468 6f6e 2062 696e 6469 6e67 7320  Python bindings 
+00000b50: 746f 2047 544b 0d0a 0922 676f 626a 6563  to GTK..."gobjec
+00000b60: 742d 696e 7472 6f73 7065 6374 696f 6e22  t-introspection"
+00000b70: 2c0d 0a09 2320 4e65 6564 6564 2074 6f20  ,...# Needed to 
+00000b80: 7072 6f76 6964 6520 4754 4b0d 0a09 2267  provide GTK..."g
+00000b90: 746b 3322 2c0d 0a09 2320 4465 7065 6e64  tk3",...# Depend
+00000ba0: 656e 6369 6573 2074 6861 7420 4754 4b20  encies that GTK 
+00000bb0: 6c6f 6f6b 7320 666f 7220 6174 2072 756e  looks for at run
+00000bc0: 7469 6d65 0d0a 0922 6c69 6263 616e 6265  time..."libcanbe
+00000bd0: 7272 612d 6774 6b33 222c 0d0a 0923 204e  rra-gtk3",...# N
+00000be0: 6565 6465 6420 746f 2070 726f 7669 6465  eeded to provide
+00000bf0: 2057 6562 4b69 7432 2061 7420 7275 6e74   WebKit2 at runt
+00000c00: 696d 650d 0a09 2320 2277 6562 6b69 7432  ime...# "webkit2
+00000c10: 6774 6b33 222c 0d0a 0923 204e 6565 6465  gtk3",...# Neede
+00000c20: 6420 666f 7220 7079 7a62 6172 2061 7420  d for pyzbar at 
+00000c30: 7275 6e74 696d 650d 0a09 227a 6261 722d  runtime..."zbar-
+00000c40: 6c69 6273 222c 0d0a 5d0d 0a0d 0a5b 746f  libs",..]....[to
+00000c50: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
+00000c60: 2e78 6463 6865 636b 696e 2e6c 696e 7578  .xdcheckin.linux
+00000c70: 2e73 7973 7465 6d2e 7375 7365 5d0d 0a73  .system.suse]..s
+00000c80: 7973 7465 6d5f 7265 7175 6972 6573 203d  ystem_requires =
+00000c90: 205b 0d0a 0923 204e 6565 6465 6420 746f   [...# Needed to
+00000ca0: 2063 6f6d 7069 6c65 2070 7963 6169 726f   compile pycairo
+00000cb0: 2077 6865 656c 0d0a 0922 6361 6972 6f2d   wheel..."cairo-
+00000cc0: 6465 7665 6c22 2c0d 0a09 2320 4e65 6564  devel",...# Need
+00000cd0: 6564 2074 6f20 636f 6d70 696c 6520 5079  ed to compile Py
+00000ce0: 474f 626a 6563 7420 7768 6565 6c0d 0a09  GObject wheel...
+00000cf0: 2267 6f62 6a65 6374 2d69 6e74 726f 7370  "gobject-introsp
+00000d00: 6563 7469 6f6e 2d64 6576 656c 222c 0d0a  ection-devel",..
+00000d10: 5d0d 0a0d 0a73 7973 7465 6d5f 7275 6e74  ]....system_runt
+00000d20: 696d 655f 7265 7175 6972 6573 203d 205b  ime_requires = [
+00000d30: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
+00000d40: 726f 7669 6465 2047 544b 0d0a 0922 6774  rovide GTK..."gt
+00000d50: 6b33 222c 0d0a 0923 204e 6565 6465 6420  k3",...# Needed 
+00000d60: 746f 2073 7570 706f 7274 2050 7974 686f  to support Pytho
+00000d70: 6e20 6269 6e64 696e 6773 2074 6f20 4754  n bindings to GT
+00000d80: 4b0d 0a09 2267 6f62 6a65 6374 2d69 6e74  K..."gobject-int
+00000d90: 726f 7370 6563 7469 6f6e 222c 2022 7479  rospection", "ty
+00000da0: 7065 6c69 6228 4774 6b29 3d33 2e30 222c  pelib(Gtk)=3.0",
+00000db0: 0d0a 0923 2044 6570 656e 6465 6e63 6965  ...# Dependencie
+00000dc0: 7320 7468 6174 2047 544b 206c 6f6f 6b73  s that GTK looks
+00000dd0: 2066 6f72 2061 7420 7275 6e74 696d 650d   for at runtime.
+00000de0: 0a09 226c 6962 6361 6e62 6572 7261 2d67  .."libcanberra-g
+00000df0: 746b 332d 3022 2c0d 0a09 2320 4e65 6564  tk3-0",...# Need
+00000e00: 6564 2074 6f20 7072 6f76 6964 6520 5765  ed to provide We
+00000e10: 624b 6974 3220 6174 2072 756e 7469 6d65  bKit2 at runtime
+00000e20: 0d0a 0923 2022 6c69 6277 6562 6b69 7432  ...# "libwebkit2
+00000e30: 6774 6b33 222c 0d0a 0923 2022 7479 7065  gtk3",...# "type
+00000e40: 6c69 6228 5765 624b 6974 3229 222c 0d0a  lib(WebKit2)",..
+00000e50: 0923 204e 6565 6465 6420 666f 7220 7079  .# Needed for py
+00000e60: 7a62 6172 2061 7420 7275 6e74 696d 650d  zbar at runtime.
+00000e70: 0a09 226c 6962 7a62 6172 3022 2c0d 0a5d  .."libzbar0",..]
+00000e80: 0d0a 0d0a 5b74 6f6f 6c2e 6272 6965 6663  ....[tool.briefc
+00000e90: 6173 652e 6170 702e 7864 6368 6563 6b69  ase.app.xdchecki
+00000ea0: 6e2e 6c69 6e75 782e 7379 7374 656d 2e61  n.linux.system.a
+00000eb0: 7263 685d 0d0a 7379 7374 656d 5f72 6571  rch]..system_req
+00000ec0: 7569 7265 7320 3d20 5b0d 0a09 2320 4e65  uires = [...# Ne
 00000ed0: 6564 6564 2074 6f20 636f 6d70 696c 6520  eded to compile 
-00000ee0: 5079 474f 626a 6563 7420 7768 6565 6c0d  PyGObject wheel.
-00000ef0: 0a09 2267 6f62 6a65 6374 2d69 6e74 726f  .."gobject-intro
-00000f00: 7370 6563 7469 6f6e 222c 0d0a 0923 2052  spection",...# R
-00000f10: 756e 7469 6d65 2064 6570 656e 6465 6e63  untime dependenc
-00000f20: 6965 7320 7468 6174 206e 6565 6420 746f  ies that need to
-00000f30: 2065 7869 7374 2073 6f20 7468 6174 2074   exist so that t
-00000f40: 6865 0d0a 0923 2041 7263 6820 7061 636b  he...# Arch pack
-00000f50: 6167 6520 7061 7373 6573 2066 696e 616c  age passes final
-00000f60: 2076 616c 6964 6174 696f 6e2e 0d0a 0923   validation....#
-00000f70: 204e 6565 6465 6420 746f 2070 726f 7669   Needed to provi
-00000f80: 6465 2047 544b 0d0a 0922 6774 6b33 222c  de GTK..."gtk3",
-00000f90: 0d0a 0923 2044 6570 656e 6465 6e63 6965  ...# Dependencie
-00000fa0: 7320 7468 6174 2047 544b 206c 6f6f 6b73  s that GTK looks
-00000fb0: 2066 6f72 2061 7420 7275 6e74 696d 650d   for at runtime.
-00000fc0: 0a09 226c 6962 6361 6e62 6572 7261 222c  .."libcanberra",
-00000fd0: 0d0a 0923 204e 6565 6465 6420 746f 2070  ...# Needed to p
-00000fe0: 726f 7669 6465 2057 6562 4b69 7432 0d0a  rovide WebKit2..
-00000ff0: 0923 2022 7765 626b 6974 3267 746b 222c  .# "webkit2gtk",
-00001000: 0d0a 5d0d 0a0d 0a73 7973 7465 6d5f 7275  ..]....system_ru
-00001010: 6e74 696d 655f 7265 7175 6972 6573 203d  ntime_requires =
-00001020: 205b 0d0a 0923 204e 6565 6465 6420 746f   [...# Needed to
-00001030: 2070 726f 7669 6465 2047 544b 0d0a 0922   provide GTK..."
-00001040: 6774 6b33 222c 0d0a 0923 204e 6565 6465  gtk3",...# Neede
-00001050: 6420 746f 2070 726f 7669 6465 2050 7947  d to provide PyG
-00001060: 4f62 6a65 6374 2062 696e 6469 6e67 730d  Object bindings.
-00001070: 0a09 2267 6f62 6a65 6374 2d69 6e74 726f  .."gobject-intro
-00001080: 7370 6563 7469 6f6e 2d72 756e 7469 6d65  spection-runtime
-00001090: 222c 0d0a 0923 2044 6570 656e 6465 6e63  ",...# Dependenc
-000010a0: 6965 7320 7468 6174 2047 544b 206c 6f6f  ies that GTK loo
-000010b0: 6b73 2066 6f72 2061 7420 7275 6e74 696d  ks for at runtim
-000010c0: 650d 0a09 226c 6962 6361 6e62 6572 7261  e..."libcanberra
-000010d0: 222c 0d0a 0923 204e 6565 6465 6420 746f  ",...# Needed to
-000010e0: 2070 726f 7669 6465 2057 6562 4b69 7432   provide WebKit2
-000010f0: 2061 7420 7275 6e74 696d 650d 0a09 2320   at runtime...# 
-00001100: 2277 6562 6b69 7432 6774 6b22 2c0d 0a09  "webkit2gtk",...
-00001110: 2320 4e65 6564 6564 2066 6f72 2070 797a  # Needed for pyz
-00001120: 6261 7220 6174 2072 756e 7469 6d65 0d0a  bar at runtime..
-00001130: 0922 7a62 6172 222c 0d0a 5d0d 0a0d 0a5b  ."zbar",..]....[
-00001140: 746f 6f6c 2e62 7269 6566 6361 7365 2e61  tool.briefcase.a
-00001150: 7070 2e78 6463 6865 636b 696e 2e6c 696e  pp.xdcheckin.lin
-00001160: 7578 2e61 7070 696d 6167 655d 0d0a 6d61  ux.appimage]..ma
-00001170: 6e79 6c69 6e75 7820 3d20 226d 616e 796c  nylinux = "manyl
-00001180: 696e 7578 5f32 5f32 3822 0d0a 0d0a 7379  inux_2_28"....sy
-00001190: 7374 656d 5f72 6571 7569 7265 7320 3d20  stem_requires = 
-000011a0: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
-000011b0: 636f 6d70 696c 6520 7079 6361 6972 6f20  compile pycairo 
-000011c0: 7768 6565 6c0d 0a09 2263 6169 726f 2d67  wheel..."cairo-g
-000011d0: 6f62 6a65 6374 2d64 6576 656c 222c 0d0a  object-devel",..
-000011e0: 0923 204e 6565 6465 6420 746f 2063 6f6d  .# Needed to com
-000011f0: 7069 6c65 2050 7947 4f62 6a65 6374 2077  pile PyGObject w
-00001200: 6865 656c 0d0a 0922 676f 626a 6563 742d  heel..."gobject-
-00001210: 696e 7472 6f73 7065 6374 696f 6e2d 6465  introspection-de
-00001220: 7665 6c22 2c0d 0a09 2320 4e65 6564 6564  vel",...# Needed
-00001230: 2074 6f20 7072 6f76 6964 6520 4754 4b0d   to provide GTK.
-00001240: 0a09 2267 746b 332d 6465 7665 6c22 2c0d  .."gtk3-devel",.
-00001250: 0a09 2320 4465 7065 6e64 656e 6369 6573  ..# Dependencies
-00001260: 2074 6861 7420 4754 4b20 6c6f 6f6b 7320   that GTK looks 
-00001270: 666f 7220 6174 2072 756e 7469 6d65 2c20  for at runtime, 
-00001280: 7468 6174 206e 6565 6420 746f 2062 650d  that need to be.
-00001290: 0a09 2320 696e 2074 6865 2062 7569 6c64  ..# in the build
-000012a0: 2065 6e76 6972 6f6e 6d65 6e74 2074 6f20   environment to 
-000012b0: 6265 2070 6963 6b65 6420 7570 2062 7920  be picked up by 
-000012c0: 6c69 6e75 7864 6570 6c6f 790d 0a09 226c  linuxdeploy..."l
-000012d0: 6962 6361 6e62 6572 7261 2d67 746b 3322  ibcanberra-gtk3"
-000012e0: 2c0d 0a09 2250 6163 6b61 6765 4b69 742d  ,..."PackageKit-
-000012f0: 6774 6b33 2d6d 6f64 756c 6522 2c0d 0a09  gtk3-module",...
-00001300: 2267 7666 732d 636c 6965 6e74 222c 0d0a  "gvfs-client",..
-00001310: 0923 204e 6565 6465 6420 666f 7220 7079  .# Needed for py
-00001320: 7a62 6172 2061 7420 7275 6e74 696d 650d  zbar at runtime.
-00001330: 0a09 227a 6261 7222 2c0d 0a5d 0d0a 0d0a  .."zbar",..]....
-00001340: 6c69 6e75 7864 6570 6c6f 795f 706c 7567  linuxdeploy_plug
-00001350: 696e 7320 3d20 5b0d 0a09 2244 4550 4c4f  ins = [..."DEPLO
-00001360: 595f 4754 4b5f 5645 5253 494f 4e3d 3320  Y_GTK_VERSION=3 
-00001370: 6774 6b22 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  gtk",..]....[too
-00001380: 6c2e 6272 6965 6663 6173 652e 6170 702e  l.briefcase.app.
-00001390: 7864 6368 6563 6b69 6e2e 6c69 6e75 782e  xdcheckin.linux.
-000013a0: 666c 6174 7061 6b5d 0d0a 666c 6174 7061  flatpak]..flatpa
-000013b0: 6b5f 7275 6e74 696d 6520 3d20 226f 7267  k_runtime = "org
-000013c0: 2e67 6e6f 6d65 2e50 6c61 7466 6f72 6d22  .gnome.Platform"
-000013d0: 0d0a 666c 6174 7061 6b5f 7275 6e74 696d  ..flatpak_runtim
-000013e0: 655f 7665 7273 696f 6e20 3d20 2234 3522  e_version = "45"
-000013f0: 0d0a 666c 6174 7061 6b5f 7364 6b20 3d20  ..flatpak_sdk = 
-00001400: 226f 7267 2e67 6e6f 6d65 2e53 646b 220d  "org.gnome.Sdk".
-00001410: 0a0d 0a5b 746f 6f6c 2e62 7269 6566 6361  ...[tool.briefca
-00001420: 7365 2e61 7070 2e78 6463 6865 636b 696e  se.app.xdcheckin
-00001430: 2e77 696e 646f 7773 5d0d 0a72 6571 7569  .windows]..requi
-00001440: 7265 7320 3d20 5b0d 0a09 2274 6f67 612d  res = [..."toga-
-00001450: 7769 6e66 6f72 6d73 7e3d 302e 342e 3022  winforms~=0.4.0"
-00001460: 2c0d 0a5d 0d0a 0d0a 2320 4d6f 6269 6c65  ,..]....# Mobile
-00001470: 2064 6570 6c6f 796d 656e 7473 0d0a 5b74   deployments..[t
-00001480: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
-00001490: 702e 7864 6368 6563 6b69 6e2e 694f 535d  p.xdcheckin.iOS]
-000014a0: 0d0a 7265 7175 6972 6573 203d 205b 0d0a  ..requires = [..
-000014b0: 0922 746f 6761 2d69 4f53 7e3d 302e 342e  ."toga-iOS~=0.4.
-000014c0: 3022 2c0d 0a09 2273 7464 2d6e 736c 6f67  0",..."std-nslog
-000014d0: 7e3d 312e 302e 3022 2c0d 0a5d 0d0a 0d0a  ~=1.0.0",..]....
-000014e0: 5b74 6f6f 6c2e 6272 6965 6663 6173 652e  [tool.briefcase.
-000014f0: 6170 702e 7864 6368 6563 6b69 6e2e 616e  app.xdcheckin.an
-00001500: 6472 6f69 645d 0d0a 7265 7175 6972 6573  droid]..requires
-00001510: 203d 205b 0d0a 0922 746f 6761 2d61 6e64   = [..."toga-and
-00001520: 726f 6964 7e3d 302e 342e 3022 2c0d 0a5d  roid~=0.4.0",..]
-00001530: 0d0a 0d0a 6275 696c 645f 6772 6164 6c65  ....build_gradle
-00001540: 5f64 6570 656e 6465 6e63 6965 7320 3d20  _dependencies = 
-00001550: 5b0d 0a09 2261 6e64 726f 6964 782e 6170  [..."androidx.ap
-00001560: 7063 6f6d 7061 743a 6170 7063 6f6d 7061  pcompat:appcompa
-00001570: 743a 312e 302e 3222 2c0d 0a09 2261 6e64  t:1.0.2",..."and
-00001580: 726f 6964 782e 636f 6e73 7472 6169 6e74  roidx.constraint
-00001590: 6c61 796f 7574 3a63 6f6e 7374 7261 696e  layout:constrain
-000015a0: 746c 6179 6f75 743a 312e 312e 3322 2c0d  tlayout:1.1.3",.
-000015b0: 0a5d 0d0a 0d0a 6275 696c 645f 6772 6164  .]....build_grad
-000015c0: 6c65 5f65 7874 7261 5f63 6f6e 7465 6e74  le_extra_content
-000015d0: 203d 2022 2222 0d0a 616e 6472 6f69 642e   = """..android.
-000015e0: 6465 6661 756c 7443 6f6e 6669 672e 6e64  defaultConfig.nd
-000015f0: 6b2e 6162 6946 696c 7465 7273 203d 205b  k.abiFilters = [
-00001600: 2761 726d 3634 2d76 3861 275d 0d0a 2222  'arm64-v8a']..""
-00001610: 220d 0a0d 0a23 2057 6562 2064 6570 6c6f  "....# Web deplo
-00001620: 796d 656e 7473 0d0a 5b74 6f6f 6c2e 6272  yments..[tool.br
-00001630: 6965 6663 6173 652e 6170 702e 7864 6368  iefcase.app.xdch
-00001640: 6563 6b69 6e2e 7765 625d 0d0a 7265 7175  eckin.web]..requ
-00001650: 6972 6573 203d 205b 0d0a 0922 746f 6761  ires = [..."toga
-00001660: 2d77 6562 7e3d 302e 342e 3022 2c0d 0a5d  -web~=0.4.0",..]
-00001670: 0d0a 0d0a 7374 796c 655f 6672 616d 6577  ....style_framew
-00001680: 6f72 6b20 3d20 2253 686f 656c 6163 6520  ork = "Shoelace 
-00001690: 7632 2e33 220d 0a                        v2.3"..
+00000ee0: 7079 6361 6972 6f20 7768 6565 6c0d 0a09  pycairo wheel...
+00000ef0: 2263 6169 726f 222c 0d0a 0923 204e 6565  "cairo",...# Nee
+00000f00: 6465 6420 746f 2063 6f6d 7069 6c65 2050  ded to compile P
+00000f10: 7947 4f62 6a65 6374 2077 6865 656c 0d0a  yGObject wheel..
+00000f20: 0922 676f 626a 6563 742d 696e 7472 6f73  ."gobject-intros
+00000f30: 7065 6374 696f 6e22 2c0d 0a09 2320 5275  pection",...# Ru
+00000f40: 6e74 696d 6520 6465 7065 6e64 656e 6369  ntime dependenci
+00000f50: 6573 2074 6861 7420 6e65 6564 2074 6f20  es that need to 
+00000f60: 6578 6973 7420 736f 2074 6861 7420 7468  exist so that th
+00000f70: 650d 0a09 2320 4172 6368 2070 6163 6b61  e...# Arch packa
+00000f80: 6765 2070 6173 7365 7320 6669 6e61 6c20  ge passes final 
+00000f90: 7661 6c69 6461 7469 6f6e 2e0d 0a09 2320  validation....# 
+00000fa0: 4e65 6564 6564 2074 6f20 7072 6f76 6964  Needed to provid
+00000fb0: 6520 4754 4b0d 0a09 2267 746b 3322 2c0d  e GTK..."gtk3",.
+00000fc0: 0a09 2320 4465 7065 6e64 656e 6369 6573  ..# Dependencies
+00000fd0: 2074 6861 7420 4754 4b20 6c6f 6f6b 7320   that GTK looks 
+00000fe0: 666f 7220 6174 2072 756e 7469 6d65 0d0a  for at runtime..
+00000ff0: 0922 6c69 6263 616e 6265 7272 6122 2c0d  ."libcanberra",.
+00001000: 0a09 2320 4e65 6564 6564 2074 6f20 7072  ..# Needed to pr
+00001010: 6f76 6964 6520 5765 624b 6974 320d 0a09  ovide WebKit2...
+00001020: 2320 2277 6562 6b69 7432 6774 6b22 2c0d  # "webkit2gtk",.
+00001030: 0a5d 0d0a 0d0a 7379 7374 656d 5f72 756e  .]....system_run
+00001040: 7469 6d65 5f72 6571 7569 7265 7320 3d20  time_requires = 
+00001050: 5b0d 0a09 2320 4e65 6564 6564 2074 6f20  [...# Needed to 
+00001060: 7072 6f76 6964 6520 4754 4b0d 0a09 2267  provide GTK..."g
+00001070: 746b 3322 2c0d 0a09 2320 4e65 6564 6564  tk3",...# Needed
+00001080: 2074 6f20 7072 6f76 6964 6520 5079 474f   to provide PyGO
+00001090: 626a 6563 7420 6269 6e64 696e 6773 0d0a  bject bindings..
+000010a0: 0922 676f 626a 6563 742d 696e 7472 6f73  ."gobject-intros
+000010b0: 7065 6374 696f 6e2d 7275 6e74 696d 6522  pection-runtime"
+000010c0: 2c0d 0a09 2320 4465 7065 6e64 656e 6369  ,...# Dependenci
+000010d0: 6573 2074 6861 7420 4754 4b20 6c6f 6f6b  es that GTK look
+000010e0: 7320 666f 7220 6174 2072 756e 7469 6d65  s for at runtime
+000010f0: 0d0a 0922 6c69 6263 616e 6265 7272 6122  ..."libcanberra"
+00001100: 2c0d 0a09 2320 4e65 6564 6564 2074 6f20  ,...# Needed to 
+00001110: 7072 6f76 6964 6520 5765 624b 6974 3220  provide WebKit2 
+00001120: 6174 2072 756e 7469 6d65 0d0a 0923 2022  at runtime...# "
+00001130: 7765 626b 6974 3267 746b 222c 0d0a 0923  webkit2gtk",...#
+00001140: 204e 6565 6465 6420 666f 7220 7079 7a62   Needed for pyzb
+00001150: 6172 2061 7420 7275 6e74 696d 650d 0a09  ar at runtime...
+00001160: 227a 6261 7222 2c0d 0a5d 0d0a 0d0a 5b74  "zbar",..]....[t
+00001170: 6f6f 6c2e 6272 6965 6663 6173 652e 6170  ool.briefcase.ap
+00001180: 702e 7864 6368 6563 6b69 6e2e 6c69 6e75  p.xdcheckin.linu
+00001190: 782e 6170 7069 6d61 6765 5d0d 0a6d 616e  x.appimage]..man
+000011a0: 796c 696e 7578 203d 2022 6d61 6e79 6c69  ylinux = "manyli
+000011b0: 6e75 785f 325f 3238 220d 0a0d 0a73 7973  nux_2_28"....sys
+000011c0: 7465 6d5f 7265 7175 6972 6573 203d 205b  tem_requires = [
+000011d0: 0d0a 0923 204e 6565 6465 6420 746f 2063  ...# Needed to c
+000011e0: 6f6d 7069 6c65 2070 7963 6169 726f 2077  ompile pycairo w
+000011f0: 6865 656c 0d0a 0922 6361 6972 6f2d 676f  heel..."cairo-go
+00001200: 626a 6563 742d 6465 7665 6c22 2c0d 0a09  bject-devel",...
+00001210: 2320 4e65 6564 6564 2074 6f20 636f 6d70  # Needed to comp
+00001220: 696c 6520 5079 474f 626a 6563 7420 7768  ile PyGObject wh
+00001230: 6565 6c0d 0a09 2267 6f62 6a65 6374 2d69  eel..."gobject-i
+00001240: 6e74 726f 7370 6563 7469 6f6e 2d64 6576  ntrospection-dev
+00001250: 656c 222c 0d0a 0923 204e 6565 6465 6420  el",...# Needed 
+00001260: 746f 2070 726f 7669 6465 2047 544b 0d0a  to provide GTK..
+00001270: 0922 6774 6b33 2d64 6576 656c 222c 0d0a  ."gtk3-devel",..
+00001280: 0923 2044 6570 656e 6465 6e63 6965 7320  .# Dependencies 
+00001290: 7468 6174 2047 544b 206c 6f6f 6b73 2066  that GTK looks f
+000012a0: 6f72 2061 7420 7275 6e74 696d 652c 2074  or at runtime, t
+000012b0: 6861 7420 6e65 6564 2074 6f20 6265 0d0a  hat need to be..
+000012c0: 0923 2069 6e20 7468 6520 6275 696c 6420  .# in the build 
+000012d0: 656e 7669 726f 6e6d 656e 7420 746f 2062  environment to b
+000012e0: 6520 7069 636b 6564 2075 7020 6279 206c  e picked up by l
+000012f0: 696e 7578 6465 706c 6f79 0d0a 0922 6c69  inuxdeploy..."li
+00001300: 6263 616e 6265 7272 612d 6774 6b33 222c  bcanberra-gtk3",
+00001310: 0d0a 0922 5061 636b 6167 654b 6974 2d67  ..."PackageKit-g
+00001320: 746b 332d 6d6f 6475 6c65 222c 0d0a 0922  tk3-module",..."
+00001330: 6776 6673 2d63 6c69 656e 7422 2c0d 0a09  gvfs-client",...
+00001340: 2320 4e65 6564 6564 2066 6f72 2070 797a  # Needed for pyz
+00001350: 6261 7220 6174 2072 756e 7469 6d65 0d0a  bar at runtime..
+00001360: 0922 7a62 6172 222c 0d0a 5d0d 0a0d 0a6c  ."zbar",..]....l
+00001370: 696e 7578 6465 706c 6f79 5f70 6c75 6769  inuxdeploy_plugi
+00001380: 6e73 203d 205b 0d0a 0922 4445 504c 4f59  ns = [..."DEPLOY
+00001390: 5f47 544b 5f56 4552 5349 4f4e 3d33 2067  _GTK_VERSION=3 g
+000013a0: 746b 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  tk",..]....[tool
+000013b0: 2e62 7269 6566 6361 7365 2e61 7070 2e78  .briefcase.app.x
+000013c0: 6463 6865 636b 696e 2e6c 696e 7578 2e66  dcheckin.linux.f
+000013d0: 6c61 7470 616b 5d0d 0a66 6c61 7470 616b  latpak]..flatpak
+000013e0: 5f72 756e 7469 6d65 203d 2022 6f72 672e  _runtime = "org.
+000013f0: 676e 6f6d 652e 506c 6174 666f 726d 220d  gnome.Platform".
+00001400: 0a66 6c61 7470 616b 5f72 756e 7469 6d65  .flatpak_runtime
+00001410: 5f76 6572 7369 6f6e 203d 2022 3435 220d  _version = "45".
+00001420: 0a66 6c61 7470 616b 5f73 646b 203d 2022  .flatpak_sdk = "
+00001430: 6f72 672e 676e 6f6d 652e 5364 6b22 0d0a  org.gnome.Sdk"..
+00001440: 0d0a 5b74 6f6f 6c2e 6272 6965 6663 6173  ..[tool.briefcas
+00001450: 652e 6170 702e 7864 6368 6563 6b69 6e2e  e.app.xdcheckin.
+00001460: 7769 6e64 6f77 735d 0d0a 7265 7175 6972  windows]..requir
+00001470: 6573 203d 205b 0d0a 0922 746f 6761 2d77  es = [..."toga-w
+00001480: 696e 666f 726d 737e 3d30 2e34 2e30 222c  informs~=0.4.0",
+00001490: 0d0a 5d0d 0a0d 0a23 204d 6f62 696c 6520  ..]....# Mobile 
+000014a0: 6465 706c 6f79 6d65 6e74 730d 0a5b 746f  deployments..[to
+000014b0: 6f6c 2e62 7269 6566 6361 7365 2e61 7070  ol.briefcase.app
+000014c0: 2e78 6463 6865 636b 696e 2e69 4f53 5d0d  .xdcheckin.iOS].
+000014d0: 0a72 6571 7569 7265 7320 3d20 5b0d 0a09  .requires = [...
+000014e0: 2274 6f67 612d 694f 537e 3d30 2e34 2e30  "toga-iOS~=0.4.0
+000014f0: 222c 0d0a 0922 7374 642d 6e73 6c6f 677e  ",..."std-nslog~
+00001500: 3d31 2e30 2e30 222c 0d0a 5d0d 0a0d 0a5b  =1.0.0",..]....[
+00001510: 746f 6f6c 2e62 7269 6566 6361 7365 2e61  tool.briefcase.a
+00001520: 7070 2e78 6463 6865 636b 696e 2e61 6e64  pp.xdcheckin.and
+00001530: 726f 6964 5d0d 0a72 6571 7569 7265 7320  roid]..requires 
+00001540: 3d20 5b0d 0a09 2274 6f67 612d 616e 6472  = [..."toga-andr
+00001550: 6f69 647e 3d30 2e34 2e30 222c 0d0a 5d0d  oid~=0.4.0",..].
+00001560: 0a0d 0a62 7569 6c64 5f67 7261 646c 655f  ...build_gradle_
+00001570: 6465 7065 6e64 656e 6369 6573 203d 205b  dependencies = [
+00001580: 0d0a 0922 616e 6472 6f69 6478 2e61 7070  ..."androidx.app
+00001590: 636f 6d70 6174 3a61 7070 636f 6d70 6174  compat:appcompat
+000015a0: 3a31 2e30 2e32 222c 0d0a 0922 616e 6472  :1.0.2",..."andr
+000015b0: 6f69 6478 2e63 6f6e 7374 7261 696e 746c  oidx.constraintl
+000015c0: 6179 6f75 743a 636f 6e73 7472 6169 6e74  ayout:constraint
+000015d0: 6c61 796f 7574 3a31 2e31 2e33 222c 0d0a  layout:1.1.3",..
+000015e0: 5d0d 0a0d 0a62 7569 6c64 5f67 7261 646c  ]....build_gradl
+000015f0: 655f 6578 7472 615f 636f 6e74 656e 7420  e_extra_content 
+00001600: 3d20 2222 220d 0a61 6e64 726f 6964 2e64  = """..android.d
+00001610: 6566 6175 6c74 436f 6e66 6967 2e6e 646b  efaultConfig.ndk
+00001620: 2e61 6269 4669 6c74 6572 7320 3d20 5b27  .abiFilters = ['
+00001630: 6172 6d36 342d 7638 6127 5d0d 0a22 2222  arm64-v8a'].."""
+00001640: 0d0a 0d0a 2320 5765 6220 6465 706c 6f79  ....# Web deploy
+00001650: 6d65 6e74 730d 0a5b 746f 6f6c 2e62 7269  ments..[tool.bri
+00001660: 6566 6361 7365 2e61 7070 2e78 6463 6865  efcase.app.xdche
+00001670: 636b 696e 2e77 6562 5d0d 0a72 6571 7569  ckin.web]..requi
+00001680: 7265 7320 3d20 5b0d 0a09 2274 6f67 612d  res = [..."toga-
+00001690: 7765 627e 3d30 2e34 2e30 222c 0d0a 5d0d  web~=0.4.0",..].
+000016a0: 0a0d 0a73 7479 6c65 5f66 7261 6d65 776f  ...style_framewo
+000016b0: 726b 203d 2022 5368 6f65 6c61 6365 2076  rk = "Shoelace v
+000016c0: 322e 3322 0d0a                           2.3"..
```

### Comparing `Xdcheckin-1.5.3/src/Xdcheckin.egg-info/PKG-INFO` & `Xdcheckin-2.0.1/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 1.5.3
+Version: 2.0.1
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
@@ -14,14 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask>=3.0.0
 Requires-Dist: flask-session==0.6.0
 Requires-Dist: pillow>=8.4.0
 Requires-Dist: pycryptodome>=3.9.4
+Requires-Dist: pyjsbitwise>=1.0.1
 Requires-Dist: pyzbar>=0.1.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-cache>=1.2.0
 Requires-Dist: waitress>=3.0.0
 
 # Xdcheckin
 Don't use.
```

### Comparing `Xdcheckin-1.5.3/src/Xdcheckin.egg-info/SOURCES.txt` & `Xdcheckin-2.0.1/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 src/xdcheckin/server/static/global.js
 src/xdcheckin/server/static/location.js
 src/xdcheckin/server/static/login.js
 src/xdcheckin/server/static/misc.js
 src/xdcheckin/server/static/player.js
 src/xdcheckin/server/static/style.css
 src/xdcheckin/server/static/util.js
-src/xdcheckin/server/templates/index.html
+src/xdcheckin/server/templates/index.html
+src/xdcheckin/util/__init__.py
+src/xdcheckin/util/chaoxing_captcha.py
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/core/chaoxing.py` & `Xdcheckin-2.0.1/src/xdcheckin/core/chaoxing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 
+from ast import literal_eval
 from base64 import b64encode
 from Crypto.Cipher.AES import new as AES_new, block_size as AES_block_size, MODE_CBC as AES_MODE_CBC
 from Crypto.Util.Padding import pad
 from datetime import datetime
 from json import dumps
 from random import choice, uniform
 from re import findall, search, DOTALL
 from requests import Response
 from requests.exceptions import RequestException
 from requests_cache.session import CachedSession
 from threading import Thread
+from xdcheckin.util.chaoxing_captcha import generate_secrets
 
 class Chaoxing:
 	"""Common Chaoxing APIs.
 	"""
 	requests_session = name = cookies = courses = logined = None
 	config = {
 		"requests_headers": {
@@ -348,30 +350,32 @@
 		:return: Dictionary of curriculum details and lessons containing course IDs, names, classroom locations, teachers and time.
 		"""
 		def _add_lesson(lesson: dict = {}):
 			lesson_class_id = str(lesson["classId"])
 			lesson = {
 				"course_id": str(lesson["courseId"]),
 				"name": lesson["name"],
-				"location": lesson["location"],
+				"locations": [lesson["location"]],
 				"invite_code": lesson["meetCode"],
-				"teacher": [lesson["teacherName"]],
-				"time":[{
+				"teachers": [lesson["teacherName"]],
+				"times": [{
 					"day": str(lesson["dayOfWeek"]),
 					"period_begin": str(lesson["beginNumber"]),
 					"period_end": str(lesson["beginNumber"] + lesson["length"] - 1)
 				}]
 			}
 			if not lesson_class_id in curriculum["lessons"]:
 				curriculum["lessons"][lesson_class_id] = lesson
 				return
-			if not lesson["teacher"][0] in curriculum["lessons"][lesson_class_id]["teacher"]:
-				curriculum["lessons"][lesson_class_id]["teacher"].append(lesson["teacher"][0])
-			if not lesson["time"][0] in curriculum["lessons"][lesson_class_id]["time"]:
-				curriculum["lessons"][lesson_class_id]["time"].append(lesson["time"][0])
+			if not lesson["locations"][0] in curriculum["lessons"][lesson_class_id]["locations"]:
+				curriculum["lessons"][lesson_class_id]["locations"].append(lesson["locations"][0])
+			if not lesson["teachers"][0] in curriculum["lessons"][lesson_class_id]["teachers"]:
+				curriculum["lessons"][lesson_class_id]["teachers"].append(lesson["teachers"][0])
+			if not lesson["times"][0] in curriculum["lessons"][lesson_class_id]["times"]:
+				curriculum["lessons"][lesson_class_id]["times"].append(lesson["times"][0])
 		url = "https://kb.chaoxing.com/curriculum/getMyLessons"
 		params = {
 			"week": week
 		}
 		res = self.get(url = url, params = params, expire_after = 86400)
 		data = res.json().get("data") or {}
 		details = data["curriculum"]
@@ -385,15 +389,15 @@
 				"time": {
 					"period_max": str(details["maxLength"]),
 					"timetable": details["lessonTimeConfigArray"][1 : -1]
 				}
 			},
 			"lessons": {}
 		}
-		lessons = data.get("lessonArray", [])
+		lessons = data.get("lessonArray") or []
 		for lesson in lessons:
 			_add_lesson(lesson = lesson)
 			for conflict in lesson.get("conflictLessons") or {}:
 				_add_lesson(lesson = conflict)
 		return curriculum
 
 	def course_get_courses(self):
@@ -561,20 +565,20 @@
 		:return: Checkin details including class ID on success.
 		"""
 		url = "https://mobilelearn.chaoxing.com/newsign/signDetail"
 		params = {
 			"activePrimaryId": activity["active_id"],
 			"type": 1
 		}
-		res = self.get(url = url, params = params, expire_after = 60)
+		res = self.get(url = url, params = params, expire_after = 300)
 		return res.json()
 
 	def checkin_get_pptactiveinfo(self, activity: dict = {"active_id": ""}):
 		"""Get PPT acitvity info.
-		:param active_id: Activity ID in dictionary.
+		:param activity: Activity ID in dictionary.
 		:return: Checkin PPT activity info including class ID and ranged option on success.
 		"""
 		url = "https://mobilelearn.chaoxing.com/v2/apis/active/getPPTActiveInfo"
 		params = {
 			"activeId": activity["active_id"]
 		}
 		res = self.get(url = url, params = params, expire_after = 60)
@@ -663,165 +667,276 @@
 			"code": ""
 		}
 		res1 = self.get(url = url1, params = params1, expire_after = 1800)
 		params2["code"] = search(r"([0-9a-f]{32})", res1.text).group(1)
 		res2 = self.get(url = url2, params = params2, expire_after = 1800)
 		return res2.text == "success"
 
+	def checkin_get_captcha(self, captcha: dict = {"captcha_id": ""}):
+		"""Get CAPTCHA for checkin.
+		:param captcha: CAPTCHA ID in dictionary.
+		:return: CAPTCHA with CAPTCHA images and token.
+		"""
+		url1 = "https://captcha.chaoxing.com/captcha/get/conf"
+		params1 = {
+			"callback": "f",
+			"captchaId": captcha["captcha_id"],
+			"_": int(datetime.now().timestamp() * 1000)
+		}
+		res1 = self.get(url = url1, params = params1, expire_after = 300)
+		server_time = search(r"t\":(\d+)", res1.text).group(1)
+		url2 = "https://captcha.chaoxing.com/captcha/get/verification/image"
+		params2 = {
+			"callback": "f",
+			"captchaId": captcha["captcha_id"],
+			"captchaKey": "",
+			"token": "",
+			"type": "slide",
+			"version": "1.1.16",
+			"referer": "https://mobilelearn.chaoxing.com",
+			"_": int(datetime.now().timestamp() * 1000)
+		}
+		captcha_new = {
+			**captcha,
+			"server_time": server_time,
+			"type": "slide"
+		}
+		captcha_key, token = generate_secrets(captcha = captcha_new)
+		params2.update({
+			"captchaKey": captcha_key,
+			"token": token
+		})
+		res2 = self.get(url = url2, params = params2)
+		data2 = literal_eval(res2.text[2 : -1])
+		return {
+			**captcha_new,
+			"token": data2["token"],
+			"big_img_src": data2["imageVerificationVo"]["shadeImage"],
+			"small_img_src": data2["imageVerificationVo"]["cutoutImage"]
+		}
+
+	def checkin_submit_captcha(
+		self, captcha = {"captcha_id": "", "token": "", "vcode": ""}
+	):
+		"""Submit and verify CAPTCHA.
+		:param captcha: CAPTCHA ID, and verification code (e.g. slider offset) in dictionary.
+		:return: CAPTCHA with validation code on success.
+		"""
+		url = "https://captcha.chaoxing.com/captcha/check/verification/result"
+		params = {
+			"callback": "f",
+			"captchaId": captcha["captcha_id"],
+			"token": captcha["token"],
+			"textClickArr": f"[{{\"x\": {captcha['vcode']}}}]",
+			"type": "slide",
+			"coordinate": "[]",
+			"version": "1.1.16",
+			"runEnv": 10,
+			"_": int(datetime.now().timestamp() * 1000)
+		}
+		res = self.get(url = url, params = params, headers = {
+			**self.config["requests_headers"],
+			"Referer": "https://mobilelearn.chaoxing.com"
+		})
+		return "result\":true" in res.text, {
+			**captcha,
+			"validate": f"validate_{captcha['captcha_id']}_{captcha['token']}"
+		}
+
 	def checkin_do_presign(
 		self, activity: dict = {"active_id": ""},
 		course: dict ={"course_id": "", "class_id": ""}
 	):
 		"""Do checkin pre-sign.
 		:param activity: Activity ID in dictionary.
 		:param course: Course ID (will be filled if not given) and class ID in dictionary.
-		:return: 2 if checked-in, otherwise checkin location containing address, latitude, longitude, range and ranged option on success.
+		:return: Presign state (2 if checked-in and 1 on success), checkin location and CAPTCHA.
 		"""
 		url = "https://mobilelearn.chaoxing.com/newsign/preSign"
 		params = {
 			"courseId": self.course_get_course_id(course = course),
 			"classId": course["class_id"],
 			"activePrimaryId": activity["active_id"],
 			"general": 1,
 			"sys": 1,
 			"ls": 1,
 			"appType": 15,
 			"tid": "",
 			"uid": self.cookies["UID"],
 			"ut": "s"
 		}
+		location = {
+			"latitude": -1,
+			"longitude": -1,
+			"address": "",
+			"ranged": 0,
+			"range": 0
+		}
+		captcha = {
+			"captcha_id": ""
+		}
 		res = self.get(url = url, params = params)
 		if res.status_code != 200:
-			return 0
-		match = search(r"ifopenAddress\" value=\"(\d)\"(?:.*?locationText\" value=\"(.*?)\".*?locationLatitude\" value=\"(\d+\.\d+)\".*?locationLongitude\" value=\"(\d+\.\d+)\".*?locationRange\" value=\"(\d+))?|(zsign_success)", res.text, DOTALL)
+			return 0, location, captcha
+		state = 1
+		match = search(r"ifopenAddress\" value=\"(\d)\"(?:.*?locationText\" value=\"(.*?)\".*?locationLatitude\" value=\"(\d+\.\d+)\".*?locationLongitude\" value=\"(\d+\.\d+)\".*?locationRange\" value=\"(\d+))?.*?captchaId: '([0-9A-Za-z]{32})|(zsign_success)", res.text, DOTALL)
 		if match:
-			if match.group(6):
-				return 2
+			if match.group(7):
+				state = 2
 			if match.group(1) == "1":
-				return {
+				location.update({
 					"latitude": float(match.group(3) or -1),
 					"longitude": float(match.group(4) or -1),
 					"address": match.group(2) or "",
 					"ranged": int(match.group(1)),
 					"range": int(match.group(5) or 0)
-				}
-		return {
+				})
+			captcha["captcha_id"] = match.group(6)
+		return state, location, captcha
+
+	def checkin_do_sign(
+		self, activity: dict = {"active_id": "", "type": ""},
+		location: dict = {"latitude": -1, "longitude": -1, "address": "", "ranged": 0},
+		old_params: dict = {"name": "", "uid": "", "fid": "", "...": "..."}
+	):
+		"""Do checkin sign.
+		:param activity: Activity ID and type in dictionary.
+		:param location: Address, latitude, longitude and ranged option in dictionary.
+		:param prev_params: Reuse previously returned params. Overrides activity and location.
+		:return: Sign state (True on success), success / error message and payload.
+		"""
+		url = "https://mobilelearn.chaoxing.com/pptSign/stuSignajax"
+		params = old_params if old_params.get("activeId") else {
+			"name": self.name,
+			"uid": self.cookies["_uid"],
+			"fid": self.cookies.get("fid") or 0,
+			"activeId": activity["active_id"],
+			"enc": activity.get("enc") or "",
+			"enc2": "",
+			"address": "",
 			"latitude": -1,
 			"longitude": -1,
-			"address": "",
-			"ranged": 0,
-			"range": 0
+			"location": "",
+			"ifTiJiao": 0,
+			"appType": 15,
+			"clientip": "",
+			"validate": "",
 		}
+		try:
+			if not old_params.get("activeId"):
+				if activity["type"] == "4":
+					params.update({
+						"address": location["address"],
+						"latitude": location["latitude"],
+						"longitude": location["longitude"],
+						"ifTiJiao": location["ranged"]
+					})
+				elif activity["type"] == "2":
+					params.update({
+						"location": str(location),
+						"ifTiJiao": location["ranged"]
+					} if location["ranged"] else {
+						"address": location["address"],
+						"latitude": location["latitude"],
+						"longitude": location["longitude"]
+					})
+			res = self.get(url = url, params = params)
+			assert res.text in ("success", "您已签到过了"), res.text
+			return True, {
+				"msg": f"Checkin success. ({res.text})",
+				"params": params
+			}
+		except Exception as e:
+			if type(e) is AssertionError:
+				match = search(r"validate_([0-9A-Fa-f]{32})", str(e))
+				if match:
+					params["enc2"] = match.group(1)
+				msg = f"Checkin failure. {dumps(activity), dumps(location), dumps(params), str(e)}"
+			else:
+				msg = str(e)
+			return False, {
+				"msg": msg,
+				"params": params
+			}
 
 	def checkin_checkin_location(
 		self, activity: dict = {"active_id": ""},
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Location checkin.
-		:param active_id: Activity ID in dictionary.
+		:param activity: Activity ID in dictionary.
 		:param location: Address, latitude and longitude in dictionary. Overriden by server-side location if any.
-		:return: True and error message on success, otherwise False and error message.
+		:return: Checkin state (True on success), success / error message and payload (placeholder).
 		"""
-		url = "https://mobilelearn.chaoxing.com/pptSign/stuSignajax"
-		params = {
-			"name": self.name,
-			"address": "",
-			"activeId": activity["active_id"],
-			"uid": self.cookies["_uid"],
-			"clientip": "",
-			"latitude": -1,
-			"longitude": -1,
-			"fid": self.cookies.get("fid") or 0,
-			"appType": 15,
-			"ifTiJiao": 0,
-			"validate": ""
-		}
 		try:
 			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			presign = self.checkin_do_presign(activity = activity, course = {"class_id": str(info["clazzId"])})
-			assert presign, f"Presign failure. {dumps(activity), dumps(location), dumps(info), dumps(presign)}"
-			if presign == 2:
+			assert presign[0], f"Presign failure. {dumps(activity), dumps(location), dumps(presign)}"
+			if presign[0] == 2:
 				return True, "Checkin success. (Already checked in.)"
-			if presign["ranged"]:
-				location_new = self.checkin_format_location(location = location, location_new = presign)
-				ranged = 1
-			else:
-				location_new = location
-				ranged = 0
-			params.update({
-				"address": location_new["address"],
-				"latitude": location_new["latitude"],
-				"longitude": location_new["longitude"],
-				"ifTiJiao": ranged
-			})
+			location_new = {
+				**(self.checkin_format_location(location = location, location_new = presign[1]) if presign[1]["ranged"] else location),
+				"ranged": presign[1]["ranged"]
+			}
 			thread_analysis.join()
-			res = self.get(url = url, params = params)
-			assert res.text in ("success", "您已签到过了"), f"Checkin failure. {dumps(activity), dumps(location), dumps(info), dumps(presign), dumps(location_new), dumps(params), res.text}"
-			return True, f"Checkin success. ({res.text})"
+			result = self.checkin_do_sign(activity = {**activity, "type": "4"}, location = location_new)
+			result[1]["captcha"] = presign[2]
+			return result
 		except Exception as e:
-			return False, str(e)
+			return False, {
+				"msg": str(e),
+				"params": {},
+				"captcha": {}
+			}
 
 	def checkin_checkin_qrcode(
 		self, activity: dict = {"active_id": "", "enc": ""},
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Qrcode checkin.
-		:param active_id: Activity ID and ENC code in dictionary.
+		:param activity: Activity ID and ENC code in dictionary.
 		:param location: Same as checkin_checkin_location().
 		:return: Same as checkin_checkin_location().
 		"""
 		def _get_location():
 			nonlocal location_new
 			location_new = self.checkin_format_location(
 				location = location,
 				location_new = self.checkin_get_location(activity = activity, course = course)
 			)
-		url = "https://mobilelearn.chaoxing.com/pptSign/stuSignajax"
-		params = {
-			"enc": activity["enc"],
-			"name": self.name,
-			"activeId": activity["active_id"],
-			"uid": self.cookies["_uid"],
-			"clientip": "",
-			"location": "",
-			"latitude": -1,
-			"longitude": -1,
-			"fid": self.cookies.get("fid") or 0,
-			"appType": 15
-		}
 		try:
 			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
-			info = self.checkin_get_pptactiveinfo(activity = activity)
-			assert info["status"] == 1 and not info["isdelete"], "Activity ended or deleted."
-			course, location_new = {"class_id": str(info["clazzid"])}, {}
+			info = self.checkin_get_details(activity = activity)
+			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
+			course, location_new = {"class_id": str(info["clazzId"])}, {}
 			thread_location = Thread(target = _get_location)
 			thread_location.start()
 			presign = self.checkin_do_presign(activity = activity, course = course)
-			assert presign, f"Presign failure. {dumps(activity), dumps(location), dumps(info), presign}"
-			if presign == 2:
+			assert presign[0], f"Presign failure. {dumps(activity), dumps(location), dumps(presign)}"
+			if presign[0] == 2:
 				return True, "Checkin success. (Already checked in.)"
-			if info["ifopenAddress"]:
-				thread_location.join()
-				params["location"] = str(location_new)
-			else:
-				location_new = location
-				params.update({
-					"latitude": location_new["latitude"],
-					"longitude": location_new["longitude"]
-				})
+			location_new = {
+				**(thread_location.join() or self.checkin_format_location(location = location, location_new = location_new) if presign[1]["ranged"] else location),
+				"ranged": presign[1]["ranged"]
+			}
 			thread_analysis.join()
-			res = self.get(url = url, params = params)
-			assert res.text in ("success", "您已签到过了"), f"Checkin failure. {dumps(activity), dumps(location), dumps(info), dumps(presign), dumps(location_new), dumps(params), res.text}"
-			return True, f"Checkin success. ({res.text})"
+			result = self.checkin_do_sign(activity = {**activity, "type": "2"}, location = location_new)
+			print(result)
+			result[1]["captcha"] = presign[2]
+			return result
 		except Exception as e:
-			return False, str(e)
+			return False, {
+				"msg": str(e),
+				"params": {},
+				"captcha": {}
+			}
 
 	def checkin_checkin_qrcode_url(
 		self, url: str = "",
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Qrcode checkin.
 		:param url: URL from Qrcode.
@@ -832,8 +947,12 @@
 			assert "mobilelearn.chaoxing.com/widget/sign/e" in url, f"Checkin failure. {'Invalid URL.', url, dumps(location)}"
 			match = search(r"id=(\d+).*?([0-9A-F]{32})", url)
 			return self.checkin_checkin_qrcode(activity = {
 				"active_id": match.group(1),
 				"enc": match.group(2)
 			}, location = location)
 		except Exception as e:
-			return False, str(e)
+			return False, {
+				"msg": str(e),
+				"params": {},
+				"captcha": {}
+			}
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/core/locations.py` & `Xdcheckin-2.0.1/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/core/xidian.py` & `Xdcheckin-2.0.1/src/xdcheckin/core/xidian.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,18 +246,24 @@
 			"url": res2.text,
 			"live_id": params1["liveId"],
 			"device": params2["deviceCode"]
 		}
 
 	def curriculum_get_curriculum(self):
 		"""Get curriculum with livestream URLs.
-		:return: Chaoxing curriculum with livestream URL, live ID and CCTV device ID for lessons.
+		:return: Chaoxing curriculum with livestreams for lessons.
 		"""
 		def _get_livestream_wrapper(class_id: str = "", live_id: str = ""):
-			curriculum["lessons"][class_id]["livestream"] = self.livestream_get_live_url(livestream = {"live_id": live_id})
+			if not curriculum["lessons"][class_id].get("livestreams"):
+				curriculum["lessons"][class_id]["livestreams"] = []
+			livestream = self.livestream_get_live_url(livestream = {"live_id": live_id})
+			for ls in curriculum["lessons"][class_id]["livestreams"]:
+				if ls["url"] == livestream["url"]:
+					return
+			curriculum["lessons"][class_id]["livestreams"].append(livestream)
 		url = "https://newesxidian.chaoxing.com/frontLive/listStudentCourseLivePage"
 		params = {
 			"fid": 16820,
 			"userId": self.chaoxing_session.cookies["UID"],
 			"termYear": 0,
 			"termId": 0,
 			"week": 0
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/server.py` & `Xdcheckin-2.0.1/src/xdcheckin/server/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from flask_session import Session
 from importlib.metadata import version
 from io import BytesIO
 from json import loads, dumps
 from os import listdir, remove, makedirs
 from os.path import exists, join
 from PIL.Image import open
-from pyzbar.pyzbar import decode
+from pyzbar.pyzbar import decode, ZBarSymbol
 from requests import get, post
 from tempfile import gettempdir
 from urllib3 import disable_warnings
 from uuid import uuid4
 from waitress import serve
 from xdcheckin.core.chaoxing import Chaoxing
 from xdcheckin.core.xidian import IDSSession, Newesxidian
@@ -179,47 +179,118 @@
 			res.status_code = 200
 		except Exception:
 			res = make_response("{}")
 			res.status_code = 500
 		finally:
 			return res
 
+	@server.route("/chaoxing/checkin_get_captcha", methods = ["POST"])
+	def chaoxing_checkin_get_captcha():
+		try:
+			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			assert chaoxing.logined
+			data = request.get_json(force = True)
+			assert data["captcha"]
+			captcha = chaoxing.checkin_get_captcha(captcha = data["captcha"])
+			res = make_response(dumps(captcha))
+			res.status_code = 200
+		except Exception:
+			res = make_response("{}")
+			res.status_code = 500
+		finally:
+			return res
+
+	@server.route("/chaoxing/checkin_submit_captcha", methods = ["POST"])
+	def chaoxing_checkin_submit_captcha():
+		try:
+			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			assert chaoxing.logined
+			data = request.get_json(force = True)
+			assert data["captcha"]
+			result = chaoxing.checkin_submit_captcha(captcha = data["captcha"])
+			assert result[0]
+			res = make_response(dumps(result[1]))
+			res.status_code = 200
+		except Exception as e:
+			res = make_response("{}")
+			res.status_code = 500
+		finally:
+			return res
+
+	@server.route("/chaoxing/checkin_do_sign", methods = ["POST"])
+	def chaoxing_checkin_do_sign():
+		try:
+			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
+			assert chaoxing.logined, "Not logged in."
+			data = request.get_json(force = True)
+			assert data["params"], "No parameters given"
+			result = chaoxing.checkin_do_sign(old_params = data["params"])
+			res = make_response(dumps({
+				"msg": f"{result[1]['msg'][: -1]}, {data['params']['activeId']})",
+				"params": result[1]["params"]
+			}))
+		except Exception as e:
+			res = make_response(dumps({
+				"msg": f"Checkin error. ({str(e)})",
+				"params": {}
+			}))
+		finally:
+			res.status_code = 200
+			return res
+						
+
 	@server.route("/chaoxing/checkin_checkin_location", methods = ["POST"])
 	def chaoxing_checkin_checkin_location():
 		try:
 			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined, "Not logged in."
 			data = request.get_json(force = True)
 			assert data["activity"]["active_id"], "No activity ID given."
 			data["activity"]["active_id"] = str(data["activity"]["active_id"])
 			result = chaoxing.checkin_checkin_location(activity = data["activity"], location = data["location"])
-			res = make_response(f"{result[1][: -1]}, {data['activity']['active_id']})")
+			res = make_response(dumps({
+				"msg": f"{result[1]['msg'][: -1]}, {data['activity']['active_id']})",
+				"params": result[1]["params"],
+				"captcha": result[1]["captcha"]
+			}))
 		except Exception as e:
-			res = make_response(f"Checkin error. ({str(e)})")
+			res = make_response(dumps({
+				"msg": f"Checkin error. ({str(e)})",
+				"params": {},
+				"captcha": {}
+			}))
 		finally:
 			res.status_code = 200
 			return res
 
 	@server.route("/chaoxing/checkin_checkin_qrcode_img", methods = ["POST"])
 	def chaoxing_checkin_checkin_qrcode_img():
 		try:
 			chaoxing = server.config["XDCHECKIN_SESSION"][session["xdcheckin_uuid"]]["chaoxing"]
 			assert chaoxing.logined, "Not logged in."
 			img_src = request.files["img_src"]
 			assert img_src, "No image given."
 			with open(BytesIO(img_src.read())) as img:
 				assert img.height and img.width, "Empty image."
-				urls = decode(img)
+				urls = decode(img, symbols = [ZBarSymbol.QRCODE])
 			assert urls, "No Qrcode detected."
 			urls = [s.data.decode("utf-8") for s in urls if b"mobilelearn.chaoxing.com/widget/sign/e" in s.data]
 			assert urls, "No checkin URL found."
 			result = chaoxing.checkin_checkin_qrcode_url(url = urls[0], location = loads(request.form["location"]))
-			res = make_response(f"{result[1][: -1]}, {urls[0]})")
+			res = make_response(dumps({
+				"msg": f"{result[1]['msg'][: -1]}, {urls[0]})",
+				"params": result[1]["params"],
+				"captcha": result[1]["captcha"]
+			}))
 		except Exception as e:
-			res = make_response(f"Checkin error. ({str(e)})")
+			res = make_response(dumps({
+				"msg": f"Checkin error. ({str(e)})",
+				"params": {},
+				"captcha": {}
+			}))
 		finally:
 			res.status_code = 200
 			return res
 
 	return server
 
 def start_server(host: str = "127.0.0.1", port: int = 5001):
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/classroom.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/curriculum.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/curriculum.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -21,37 +21,43 @@
     let timetable = curriculum.details.time.timetable;
     for (let class_id in curriculum.lessons) {
         let lesson = curriculum.lessons[class_id];
         let tr = tb.appendChild(newElement("tr"));
         let td = tr.appendChild(newElement("td"));
         td.appendChild(document.createTextNode(lesson.name));
         td = tr.appendChild(newElement("td"));
-        lesson.teacher.forEach((v, i) => {
+        lesson.teachers.forEach((v, i) => {
             if (i)
                 td.appendChild(newElement("br"));
-            td.appendChild(document.createTextNode(`${v}`));
+            td.appendChild(document.createTextNode(v));
         });
         td = tr.appendChild(newElement("td"));
-        lesson.time.forEach((v, i) => {
+        lesson.times.forEach((v, i) => {
             if (i)
                 td.appendChild(newElement("br"));
             let bgn = timetable[v.period_begin - 1].slice(0, 5);
             let end = timetable[v.period_end - 1].slice(6, 11);
             td.appendChild(document.createTextNode(`${v.day}  ` +
                 `${bgn}-${end}`));
 
         });
         td = tr.appendChild(newElement("td"));
-        if (with_live && "livestream" in lesson) {
-            let url = lesson.livestream.url;
-            let name = lesson.location;
+        lesson.locations.forEach((v, i) => {
+            if (i)
+                td.appendChild(newElement("br"));
+            td.appendChild(document.createTextNode(v));
+        });
+        if (!with_live)
+            continue;
+        td = tr.appendChild(newElement("td"));
+        lesson.livestreams.forEach((v, i) => {
+            if (i)
+                td.appendChild(newElement("br"));
             td.appendChild(newElement("button", {
-                innerText: name,
-                onclick: () => setClassroom(url, name)
+                innerText: v.live_id,
+                onclick: () => setClassroom(v.url, v.live_id)
             }));
-        } else
-            td.appendChild(document.createTextNode(
-                lesson.location));
+        });
     }
     document.getElementById("curriculum-list-div").appendChild(table);
     getCurriculum.calling = false;
 }
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/g_classroom_urls.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/location.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/login.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/misc.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/player.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/style.css` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/style.css`

 * *Files 16% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 	border-collapse: collapse;
 	text-align: center;
 }
 table {
 	width: 100%;
 }
 
-#ids-login-captcha-container-div {
+.captcha-container-div {
 	position: relative;
 	width: 100%;
 }
-#ids-login-captcha-img {
+.captcha-img {
 	height: auto;
 	width: 100%;
 }
-#ids-login-captcha-small-img {
+.captcha-small-img {
 	position: absolute;
 	height: 100%;
 	top: -2.5px;
 }
-#ids-login-captcha-input {
+.captcha-input {
 	justify-content: center;
 	align-items: center;
 	display: flex;
 	width: 70%;
 }
 
 #xdcheckin-title-div {
```

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/static/util.js` & `Xdcheckin-2.0.1/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-1.5.3/src/xdcheckin/server/templates/index.html` & `Xdcheckin-2.0.1/src/xdcheckin/server/templates/index.html`

 * *Files 24% similar despite different names*

```diff
@@ -32,21 +32,32 @@
 			<button id="activities-button" onclick="
 				if (document.getElementById('activities-list-div').style.display == 'none')
 					getActivities().then(hideOtherLists('activities-list-div'));
 				else
 					displayTag('activities-list-div');
 			" style="display: none">Activities</button>
 		</div>
+		<div id="activities-checkin-captcha-div" style="display: none">
+			<div id="activities-checkin-captcha-container-div" class="captcha-container-div">
+				<img id="activities-checkin-captcha-img" class="captcha-img" src="">
+				<img id="activities-checkin-captcha-small-img" class="captcha-small-img" src="">
+			</div>
+			<div class="div-center">
+				<input id="activities-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
+				&emsp;
+				<button id="activities-checkin-captcha-button">Verify</button>
+			</div>
+		</div>
 		<div id="ids-login-captcha-div" style="display: none">
-			<div id="ids-login-captcha-container-div">
-				<img id="ids-login-captcha-img" src="">
-				<img id="ids-login-captcha-small-img" src="">
+			<div id="ids-login-captcha-container-div" class="captcha-container-div">
+				<img id="ids-login-captcha-img" class="captcha-img" src="">
+				<img id="ids-login-captcha-small-img" class="captcha-small-img" src="">
 			</div>
 			<div class="div-center">
-				<input id="ids-login-captcha-input" type="range" min="0" max="280" step="1" value="0">
+				<input id="ids-login-captcha-input" class="captcha-input" type="range" min="0" max="280" step="1" value="0">
 				&emsp;
 				<button id="ids-login-captcha-button">Verify</button>
 			</div>
 		</div>
 		<div id="curriculum-list-div" style="display: none"></div>
 		<div id="locations-list-div" style="display: none">
 			<div id="location-current-div"></div>
@@ -72,14 +83,25 @@
 			<button onclick="g_players[0].mute()">Mute</button>
 			<button id="player0-scan-button" onclick="
 				chaoxingCheckinQrcodeWrapper(g_players[0].tag, 1, 'player0-scanresult-div');
 				onclickCooldown(this.id);
 			" style="display: none">Scan</button>
 		</div>
 		<div id="player0-div"></div>
+		<div id="player0-checkin-captcha-div" style="display: none">
+			<div id="player0-checkin-captcha-container-div" class="captcha-container-div">
+				<img id="player0-checkin-captcha-img" class="captcha-img" src="">
+				<img id="player0-checkin-captcha-small-img" class="captcha-small-img" src="">
+			</div>
+			<div class="div-center">
+				<input id="player0-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
+				&emsp;
+				<button id="player0-checkin-captcha-button">Verify</button>
+			</div>
+		</div>
 		<div id="player0-scanresult-div" class="scanresult-div"></div>
 
 		<div id="player1-buttons-div" class="div-center" style="display: none">
 			<B style="font-size:40px; font-family: sans-serif">TeacherTrack</B>
 			&emsp;
 			<button onclick="g_players[1].initPlay()">Play</button>
 			<button onclick="g_players[1].stop()">Stop</button>
@@ -117,14 +139,25 @@
 				chaoxingCheckinQrcodeWrapper(document.getElementById('camera-video'), 0.65, 'camera-scanresult-div');
 				onclickCooldown(this.id);
 			" style="display: none">Scan</button>
 		</div>
 		<div id="camera-div" style="display: none">
 			<video id="camera-video" width="640" height="480" autoplay></video>
 		</div>
+		<div id="camera-checkin-captcha-div" style="display: none">
+			<div id="camera-checkin-captcha-container-div" class="captcha-container-div">
+				<img id="camera-checkin-captcha-img" class="captcha-img" src="">
+				<img id="camera-checkin-captcha-small-img" class="captcha-small-img" src="">
+			</div>
+			<div class="div-center">
+				<input id="camera-checkin-captcha-input" class="captcha-input" type="range" min="0" max="320" step="1" value="0">
+				&emsp;
+				<button id="camera-checkin-captcha-button">Verify</button>
+			</div>
+		</div>
 		<div id="camera-scanresult-div" class="scanresult-div" style="display: none"></div>
 
 		<div id="footer-div" class="div-center">
 			<a id="footer-link-a" href="https://github.com/Pairman/Xdcheckin">Xdcheckin</a>
 			&emsp;(C) 2024 Pairman
 		</div>
 	</body>
```

#### html2text {}

```diff
@@ -1,13 +1,19 @@
 Login Logout Curriculum Location Activities
 [Image][Image]
 [Unknown INPUT type]  Verify
+[Image][Image]
+[Unknown INPUT type]  Verify
 Xdcheckin
  
 Classroom Play All Stop All
 
 PPPPTTVViiddeeoo   Play Stop Unmute Mute Scan
+[Image][Image]
+[Unknown INPUT type]  Verify
 TTeeaacchheerrTTrraacckk   Play Stop Unmute Mute
 TTeeaacchheerrFFuullll   Play Stop Unmute Mute
 SSttuuddeennttFFuullll   Play Stop Unmute Mute
 CCaammeerraa   On Off Scan
+[Image][Image]
+[Unknown INPUT type]  Verify
 _X_d_c_h_e_c_k_i_n  (C) 2024 Pairman
```

