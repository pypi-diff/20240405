# Comparing `tmp/libWiiPy-0.2.0.tar.gz` & `tmp/libWiiPy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libWiiPy-0.2.0.tar", last modified: Wed Apr  3 22:16:31 2024, max compression
+gzip compressed data, was "libWiiPy-0.2.1.tar", last modified: Fri Apr  5 05:07:12 2024, max compression
```

## Comparing `libWiiPy-0.2.0.tar` & `libWiiPy-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libWiiPy-0.2.0/LICENSE
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4537 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)     3903 2024-04-03 22:05:00.000000 libWiiPy-0.2.0/README.md
--rw-r--r--   0 campbell  (1000) campbell  (1000)      738 2024-03-08 05:11:53.000000 libWiiPy-0.2.0/pyproject.toml
--rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/setup.cfg
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/libWiiPy/
--rw-r--r--   0 campbell  (1000) campbell  (1000)      331 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/__init__.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/commonkeys.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/content.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4301 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/crypto.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/shared.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/ticket.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     9062 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/title.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    13738 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/tmd.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/types.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)    12583 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/wad.py
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/libWiiPy.egg-info/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     4537 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)      440 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/SOURCES.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/dependency_links.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)       13 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/requires.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/top_level.txt
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libWiiPy-0.2.1/LICENSE
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4599 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     3942 2024-04-04 03:07:12.000000 libWiiPy-0.2.1/README.md
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      752 2024-04-03 23:07:45.000000 libWiiPy-0.2.1/pyproject.toml
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/setup.cfg
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/libWiiPy/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      350 2024-04-04 01:06:05.000000 libWiiPy-0.2.1/src/libWiiPy/__init__.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/commonkeys.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/content.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4301 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/crypto.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     7776 2024-04-05 04:04:30.000000 libWiiPy-0.2.1/src/libWiiPy/nus.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/shared.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/ticket.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     9062 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/title.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    13738 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/tmd.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:17:05.000000 libWiiPy-0.2.1/src/libWiiPy/types.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    12515 2024-04-05 05:06:09.000000 libWiiPy-0.2.1/src/libWiiPy/wad.py
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-05 05:07:12.885474 libWiiPy-0.2.1/src/libWiiPy.egg-info/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4599 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      460 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       21 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/requires.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-04-05 05:07:12.000000 libWiiPy-0.2.1/src/libWiiPy.egg-info/top_level.txt
```

### Comparing `libWiiPy-0.2.0/LICENSE` & `libWiiPy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/PKG-INFO` & `libWiiPy-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome
+Requires-Dist: urllib3
 
 ![libWiiPy](https://github.com/NinjaCheetah/libWiiPy/assets/58050615/80093c68-b86e-4b96-87b7-db3855382ca8)
 # libWiiPy
 libWiiPy is a modern Python 3 library for interacting with and editing files from the Wii. It aims to be simple to use, well maintained, and offer as many features as reasonably possible in one library, so that a newly-written Python program could reasonably do 100% of its Wii-related work with just one library. It also aims to be fully cross-platform, so that any tools written with it can also be cross-platform.
 
 libWiiPy is inspired by [libWiiSharp](https://github.com/TheShadowEevee/libWiiSharp), originally created by `Leathl`, now maintained by [@TheShadowEevee](https://github.com/TheShadowEevee). libWiiSharp is absolutely the way to go if you need a C# library for Wii files.
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
+- Downloading free titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
```

### Comparing `libWiiPy-0.2.0/README.md` & `libWiiPy-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
+- Downloading free titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
```

### Comparing `libWiiPy-0.2.0/pyproject.toml` & `libWiiPy-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "libWiiPy"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="NinjaCheetah", email="ninjacheetah@ncxprogramming.com" },
     { name="Lillian Skinner", email="lillian@randommeaninglesscharacters.com" }
 ]
 description = "A modern Python library for handling files used by the Wii"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pycryptodome",
+    "urllib3"
 ]
 
 [project.urls]
 Homepage = "https://github.com/NinjaCheetah/libWiiPy"
 Issues = "https://github.com/NinjaCheetah/libWiipy/issues"
 
 [build-system]
```

### Comparing `libWiiPy-0.2.0/src/libWiiPy/commonkeys.py` & `libWiiPy-0.2.1/src/libWiiPy/commonkeys.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/content.py` & `libWiiPy-0.2.1/src/libWiiPy/content.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/crypto.py` & `libWiiPy-0.2.1/src/libWiiPy/crypto.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/shared.py` & `libWiiPy-0.2.1/src/libWiiPy/shared.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/ticket.py` & `libWiiPy-0.2.1/src/libWiiPy/ticket.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/title.py` & `libWiiPy-0.2.1/src/libWiiPy/title.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/tmd.py` & `libWiiPy-0.2.1/src/libWiiPy/tmd.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/types.py` & `libWiiPy-0.2.1/src/libWiiPy/types.py`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.2.0/src/libWiiPy/wad.py` & `libWiiPy-0.2.1/src/libWiiPy/wad.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,16 @@
         with io.BytesIO(wad_data) as wad_data:
             # Read the first 8 bytes of the file to ensure that it's a WAD. This will currently reject boot2 WADs, but
             # this tool cannot handle them correctly right now anyway.
             wad_data.seek(0x0)
             wad_magic_bin = wad_data.read(8)
             wad_magic_hex = binascii.hexlify(wad_magic_bin)
             wad_magic = str(wad_magic_hex.decode())
-            if wad_magic != "0000002049730000":
-                raise TypeError("This does not appear to be a valid WAD file, or is a boot2 WAD, which is not currently"
-                                " supported by this library.")
+            if wad_magic != "0000002049730000" and wad_magic != "0000002069620000":
+                raise TypeError("This does not appear to be a valid WAD file.")
             # ====================================================================================
             # Get the sizes of each data region contained within the WAD.
             # ====================================================================================
             # Header length, which will always be 64 bytes, as it is padded out if it is shorter.
             self.wad_hdr_size = 64
             # WAD type, denoting whether this WAD contains boot2 ("ib"), or anything else ("Is").
             wad_data.seek(0x04)
```

### Comparing `libWiiPy-0.2.0/src/libWiiPy.egg-info/PKG-INFO` & `libWiiPy-0.2.1/src/libWiiPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: libWiiPy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A modern Python library for handling files used by the Wii
 Author-email: NinjaCheetah <ninjacheetah@ncxprogramming.com>, Lillian Skinner <lillian@randommeaninglesscharacters.com>
 Project-URL: Homepage, https://github.com/NinjaCheetah/libWiiPy
 Project-URL: Issues, https://github.com/NinjaCheetah/libWiipy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome
+Requires-Dist: urllib3
 
 ![libWiiPy](https://github.com/NinjaCheetah/libWiiPy/assets/58050615/80093c68-b86e-4b96-87b7-db3855382ca8)
 # libWiiPy
 libWiiPy is a modern Python 3 library for interacting with and editing files from the Wii. It aims to be simple to use, well maintained, and offer as many features as reasonably possible in one library, so that a newly-written Python program could reasonably do 100% of its Wii-related work with just one library. It also aims to be fully cross-platform, so that any tools written with it can also be cross-platform.
 
 libWiiPy is inspired by [libWiiSharp](https://github.com/TheShadowEevee/libWiiSharp), originally created by `Leathl`, now maintained by [@TheShadowEevee](https://github.com/TheShadowEevee). libWiiSharp is absolutely the way to go if you need a C# library for Wii files.
 
 **Note:** While libWiiPy is directly inspired by libWiiSharp and aims to have feature parity with it, no code from either libWiiSharp or Wii.py was used in the making of this library. All code is original and is written by [@NinjaCheetah](https://github.com/NinjaCheetah), [@rvtr](https://github.com/rvtr), and any other GitHub contributors.
 
 # Features
 This list will expand as libWiiPy is developed, but these features are currently available:
 - TMD, ticket, and WAD parsing
 - WAD content extraction, decryption, re-encryption, and packing
+- Downloading free titles from the NUS
 
 # Usage
 A wiki, and in the future a potential documenation site, is being worked on, and can be accessed [here](https://github.com/NinjaCheetah/libWiiPy/wiki). It is currently fairly barebones, but it will be improved in the future.
 
 The easiest way to get libWiiPy for your project is to install the latest version of the library from PyPI, as shown below. 
 ```sh
 pip install -U libWiiPy
```

