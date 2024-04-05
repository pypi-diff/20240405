# Comparing `tmp/vrfy-0.3.1.tar.gz` & `tmp/vrfy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vrfy-0.3.1.tar", last modified: Sun Jan  7 20:35:09 2024, max compression
+gzip compressed data, was "vrfy-0.4.0.tar", last modified: Fri Apr  5 16:29:13 2024, max compression
```

## Comparing `vrfy-0.3.1.tar` & `vrfy-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 20:35:09.300867 vrfy-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-01-07 20:34:55.000000 vrfy-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-01-07 20:35:09.300867 vrfy-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-01-07 20:34:55.000000 vrfy-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 20:35:09.300867 vrfy-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-07 20:34:55.000000 vrfy-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 20:35:09.296867 vrfy-0.3.1/vrfy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 20:35:09.300867 vrfy-0.3.1/vrfy/vrfy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-01-07 20:35:09.000000 vrfy-0.3.1/vrfy/vrfy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-07 20:35:09.000000 vrfy-0.3.1/vrfy/vrfy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 20:35:09.000000 vrfy-0.3.1/vrfy/vrfy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-07 20:35:09.000000 vrfy-0.3.1/vrfy/vrfy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-07 20:35:09.000000 vrfy-0.3.1/vrfy/vrfy.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    24794 2024-01-07 20:34:55.000000 vrfy-0.3.1/vrfy/vrfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:29:13.988989 vrfy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-05 16:29:07.000000 vrfy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-05 16:29:13.988989 vrfy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-05 16:29:07.000000 vrfy-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:29:13.988989 vrfy-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 16:29:07.000000 vrfy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:29:13.984989 vrfy-0.4.0/vrfy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:29:07.000000 vrfy-0.4.0/vrfy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:29:13.988989 vrfy-0.4.0/vrfy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:29:07.000000 vrfy-0.4.0/vrfy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-05 16:29:07.000000 vrfy-0.4.0/vrfy/cli/vrfyCli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18207 2024-04-05 16:29:07.000000 vrfy-0.4.0/vrfy/vrfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:29:13.988989 vrfy-0.4.0/vrfy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-05 16:29:13.000000 vrfy-0.4.0/vrfy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-05 16:29:13.000000 vrfy-0.4.0/vrfy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:29:13.000000 vrfy-0.4.0/vrfy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 16:29:13.000000 vrfy-0.4.0/vrfy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 16:29:13.000000 vrfy-0.4.0/vrfy.egg-info/top_level.txt
```

### Comparing `vrfy-0.3.1/LICENSE` & `vrfy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vrfy-0.3.1/PKG-INFO` & `vrfy-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrfy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Verify with VRFY: Ensure the integrity of your file copies, hash by hash!
 Home-page: https://github.com/BumblebeeMan/vrfy
 Author: BumblebeeMan (Dennis Koerner)
 Author-email: dennis@bumblebeeman.dev
 Keywords: vrfy,verify,check,directory,hash
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# Verify with VRFY: Ensure the integrity of your file copies, hash by hash!
 
 When beginning to explore cloud storage (or other methods of remotely storing files), one may become concerned about file integrity at some point. When dealing with a large number of individual files, how can one be certain that no file becomes corrupted during the storage process, and that downloaded files remain identical to their uploaded versions? This concern is particularly relevant after undergoing multiple segmentation and encryption/decryption processes. It's impractical to manually verify all files, making file corruption a common worry, especially for those using smaller cloud providers. 
@@ -40,27 +41,23 @@
 ## Installation
 ### PIP: 
 Install **vrfy** using pip:
 ```bash
 pip install vrfy --user
 ```
  
-## Usage
+## Usage the CLI
 ### 1. Verifing that two directories are identical
-Verifing that the contents of '/path/of/clone' are identical to those of '/path/of/master'. For example, '/path/of/master' might be a local backup, whereas '/path/of/clone' might be loaded from cloud storage. 
+Verifing that the contents of '/path/of/backup' are identical to those of '/path/of/master'. For example, '/path/of/master' might be a local backup, whereas '/path/of/backup' might be loaded from cloud storage.
 ```bash
-vrfy /path/of/master /path/of/clone
+vrfy -m /path/of/master -b /path/of/backup -r
 ```
-or
+or (mismatched checksums are printed to console)
 ```bash
-vrfy -m /path/of/master -c /path/of/clone -r
-```
-or (checksums are printed to console)
-```bash
-vrfy -m /path/of/master -c /path/of/clone -r -p
+vrfy -m /path/of/master -b /path/of/backup -r -p
 ```
 
 ### 2. Storing checksums for future verification
 Creating a file that lists checksums for all files within a directory:
 ```bash
 vrfy -c /path/of/data
 ```
@@ -74,15 +71,15 @@
 ```bash
 vrfy -v /path/of/data
 ```
 Using option **-r** (recursive) all sub-directories are verified as well:
 ```bash
 vrfy -r -v /path/of/data
 ```
-Using option **-p** (print) all checksums are printed to console for further inspection:
+Using option **-p** (print) all mismatched checksums are printed to console for further inspection:
 ```bash
 vrfy -p -r -v /path/of/data
 ```
 Verifying the current working directory and all its sub-directories:
 ```bash
 vrfy
 ```
@@ -94,13 +91,51 @@
 - A string containing the expected sha256 hash digest.
 - A *.sha256sum-file that includes the expected hash digest.
 - A sums.csv-file created by **vrfy** that includes the expected hash digest.
 
 ### 4. Other CLI options
 Display version of vrfy:
 ```bash
-vrfy -version
+vrfy --version
 ```
 Display checksum for given file:
 ```bash
 vrfy -p -f /path/of/file/filename
 ```
+Display help:
+```bash
+vrfy -h
+```
+
+## Using the python package
+### Getting started
+```python
+from vrfy.vrfy import vrfy
+vf = vrfy()
+
+# Get version string
+versionStr = vf.GetVersion()
+
+# Verify a single file to an expected checksum
+Result = vf.VerifyFile("/path/and/fileName.xyz", "expectedChecksum")
+
+# Verify contents of a directory to stored checksums
+Result = VerifyFilesAgainstChecksums("path/to/directory")
+
+# Create/store checksum file for later file verification
+Result = WriteChecksumFile("path/to/directory")
+
+# Verify that files within master and backup directories are identical
+Result = VerifyFiles("path/to/directory/master", "path/to/directory/backup")
+```
+where
+```python
+class Result:
+    self.Result: bool            # Determines whether operation was successful (True) or not (False).
+    self.Path: str               # Path the result object corresponds to. 
+    self.PathError: bool         # True: Path is a valid directory, False otherwise.
+    self.MissingFiles: list      # Missing files in (backup) directory that are included in master directory / checksum list.
+    self.AdditionalFiles: list   # Additional files in (backup) directory that are NOT included in master directory / checksum list.
+    self.ChecksumMismatch: list  # List of files with mismachting checksums.
+    self.MasterChecksums: dict   # Dictionary of files within master directory and their checksums.
+    self.BackupChecksums: dict   # Dictionary of files within backup directory and their checksums.
+```
```

### Comparing `vrfy-0.3.1/setup.py` & `vrfy-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 from setuptools import setup
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
-    name = 'vrfy',
-    version = '0.3.1',
-    description = 'Verify with VRFY: Ensure the integrity of your file copies, hash by hash!',
-    long_description = long_description,
+    name='vrfy',
+    version='0.4.0',
+    description='Verify with VRFY: Ensure the integrity of your file copies, hash by hash!',
+    long_description=long_description,
     long_description_content_type='text/markdown',
 
-    py_modules = ["vrfy"],
-    package_dir = {'': 'vrfy'},
+    packages=['vrfy', 'vrfy.cli'],
 
-    author="BumblebeeMan (Dennis Koerner)", 
-    author_email="dennis@bumblebeeman.dev",     
+    author="BumblebeeMan (Dennis Koerner)",
+    author_email="dennis@bumblebeeman.dev",
     url="https://github.com/BumblebeeMan/vrfy",
 
-    #install_requires=["requests >= 2.30.0", "psutil >= 5.9.0"],
-    
     entry_points={
         'console_scripts': [
-            'vrfy = vrfy:main',
+            'vrfy = vrfy.cli.vrfyCli:main',
         ],
     },
 
     python_requires=">=3.7",
 
     keywords=["vrfy", "verify", "check", "directory", "hash"],
 
@@ -44,9 +41,10 @@
                  "Programming Language :: Python :: 3",
                  "Programming Language :: Python :: 3 :: Only",
                  "Programming Language :: Python :: 3.7",
                  "Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
                  "Programming Language :: Python :: 3.11",
-                 ]  
+                 "Programming Language :: Python :: 3.12",
+                 ]
 )
```

### Comparing `vrfy-0.3.1/vrfy/vrfy.egg-info/PKG-INFO` & `vrfy-0.4.0/vrfy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrfy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Verify with VRFY: Ensure the integrity of your file copies, hash by hash!
 Home-page: https://github.com/BumblebeeMan/vrfy
 Author: BumblebeeMan (Dennis Koerner)
 Author-email: dennis@bumblebeeman.dev
 Keywords: vrfy,verify,check,directory,hash
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ﻿# Verify with VRFY: Ensure the integrity of your file copies, hash by hash!
 
 When beginning to explore cloud storage (or other methods of remotely storing files), one may become concerned about file integrity at some point. When dealing with a large number of individual files, how can one be certain that no file becomes corrupted during the storage process, and that downloaded files remain identical to their uploaded versions? This concern is particularly relevant after undergoing multiple segmentation and encryption/decryption processes. It's impractical to manually verify all files, making file corruption a common worry, especially for those using smaller cloud providers. 
@@ -40,27 +41,23 @@
 ## Installation
 ### PIP: 
 Install **vrfy** using pip:
 ```bash
 pip install vrfy --user
 ```
  
-## Usage
+## Usage the CLI
 ### 1. Verifing that two directories are identical
-Verifing that the contents of '/path/of/clone' are identical to those of '/path/of/master'. For example, '/path/of/master' might be a local backup, whereas '/path/of/clone' might be loaded from cloud storage. 
+Verifing that the contents of '/path/of/backup' are identical to those of '/path/of/master'. For example, '/path/of/master' might be a local backup, whereas '/path/of/backup' might be loaded from cloud storage.
 ```bash
-vrfy /path/of/master /path/of/clone
+vrfy -m /path/of/master -b /path/of/backup -r
 ```
-or
+or (mismatched checksums are printed to console)
 ```bash
-vrfy -m /path/of/master -c /path/of/clone -r
-```
-or (checksums are printed to console)
-```bash
-vrfy -m /path/of/master -c /path/of/clone -r -p
+vrfy -m /path/of/master -b /path/of/backup -r -p
 ```
 
 ### 2. Storing checksums for future verification
 Creating a file that lists checksums for all files within a directory:
 ```bash
 vrfy -c /path/of/data
 ```
@@ -74,15 +71,15 @@
 ```bash
 vrfy -v /path/of/data
 ```
 Using option **-r** (recursive) all sub-directories are verified as well:
 ```bash
 vrfy -r -v /path/of/data
 ```
-Using option **-p** (print) all checksums are printed to console for further inspection:
+Using option **-p** (print) all mismatched checksums are printed to console for further inspection:
 ```bash
 vrfy -p -r -v /path/of/data
 ```
 Verifying the current working directory and all its sub-directories:
 ```bash
 vrfy
 ```
@@ -94,13 +91,51 @@
 - A string containing the expected sha256 hash digest.
 - A *.sha256sum-file that includes the expected hash digest.
 - A sums.csv-file created by **vrfy** that includes the expected hash digest.
 
 ### 4. Other CLI options
 Display version of vrfy:
 ```bash
-vrfy -version
+vrfy --version
 ```
 Display checksum for given file:
 ```bash
 vrfy -p -f /path/of/file/filename
 ```
+Display help:
+```bash
+vrfy -h
+```
+
+## Using the python package
+### Getting started
+```python
+from vrfy.vrfy import vrfy
+vf = vrfy()
+
+# Get version string
+versionStr = vf.GetVersion()
+
+# Verify a single file to an expected checksum
+Result = vf.VerifyFile("/path/and/fileName.xyz", "expectedChecksum")
+
+# Verify contents of a directory to stored checksums
+Result = VerifyFilesAgainstChecksums("path/to/directory")
+
+# Create/store checksum file for later file verification
+Result = WriteChecksumFile("path/to/directory")
+
+# Verify that files within master and backup directories are identical
+Result = VerifyFiles("path/to/directory/master", "path/to/directory/backup")
+```
+where
+```python
+class Result:
+    self.Result: bool            # Determines whether operation was successful (True) or not (False).
+    self.Path: str               # Path the result object corresponds to. 
+    self.PathError: bool         # True: Path is a valid directory, False otherwise.
+    self.MissingFiles: list      # Missing files in (backup) directory that are included in master directory / checksum list.
+    self.AdditionalFiles: list   # Additional files in (backup) directory that are NOT included in master directory / checksum list.
+    self.ChecksumMismatch: list  # List of files with mismachting checksums.
+    self.MasterChecksums: dict   # Dictionary of files within master directory and their checksums.
+    self.BackupChecksums: dict   # Dictionary of files within backup directory and their checksums.
+```
```

