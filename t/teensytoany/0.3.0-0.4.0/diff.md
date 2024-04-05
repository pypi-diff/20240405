# Comparing `tmp/teensytoany-0.3.0.tar.gz` & `tmp/teensytoany-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teensytoany-0.3.0.tar", last modified: Tue Apr  2 15:02:51 2024, max compression
+gzip compressed data, was "teensytoany-0.4.0.tar", last modified: Fri Apr  5 13:07:32 2024, max compression
```

## Comparing `teensytoany-0.3.0.tar` & `teensytoany-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-02 15:02:47.000000 teensytoany-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-02 15:02:47.000000 teensytoany-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-02 15:02:47.000000 teensytoany-0.3.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-02 15:02:47.000000 teensytoany-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 15:02:47.000000 teensytoany-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-02 15:02:51.372447 teensytoany-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-02 15:02:47.000000 teensytoany-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.368447 teensytoany-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4964 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 15:02:47.000000 teensytoany-0.3.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 15:02:51.372447 teensytoany-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-02 15:02:47.000000 teensytoany-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/teensypower.py
--rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-04-02 15:02:47.000000 teensytoany-0.3.0/teensytoany/teensytoany.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:02:51.372447 teensytoany-0.3.0/teensytoany.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 15:02:51.000000 teensytoany-0.3.0/teensytoany.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:32.159868 teensytoany-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-05 13:07:21.000000 teensytoany-0.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-05 13:07:21.000000 teensytoany-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-05 13:07:21.000000 teensytoany-0.4.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-05 13:07:21.000000 teensytoany-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 13:07:21.000000 teensytoany-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-05 13:07:32.159868 teensytoany-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-05 13:07:21.000000 teensytoany-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:32.155868 teensytoany-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4964 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 13:07:21.000000 teensytoany-0.4.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 13:07:32.159868 teensytoany-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-05 13:07:21.000000 teensytoany-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:32.159868 teensytoany-0.4.0/teensytoany/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 13:07:21.000000 teensytoany-0.4.0/teensytoany/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 13:07:32.159868 teensytoany-0.4.0/teensytoany/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-05 13:07:21.000000 teensytoany-0.4.0/teensytoany/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-05 13:07:21.000000 teensytoany-0.4.0/teensytoany/programmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-05 13:07:21.000000 teensytoany-0.4.0/teensytoany/teensypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26840 2024-04-05 13:07:21.000000 teensytoany-0.4.0/teensytoany/teensytoany.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:32.159868 teensytoany-0.4.0/teensytoany.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 13:07:32.000000 teensytoany-0.4.0/teensytoany.egg-info/top_level.txt
```

### Comparing `teensytoany-0.3.0/CONTRIBUTING.md` & `teensytoany-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/HISTORY.md` & `teensytoany-0.4.0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.4.0 (2024-04-05)
+
+* Provide functions to fetch local and remote firmware versions.
+* Provide a static method to program the latest firmware version and a CLI to
+  do so from the terminal.
+
 ## 0.3.0 (2024-04-02)
 
 * Add a `timeout` property to the functions that deal with updating the firmware.
 
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
```

### Comparing `teensytoany-0.3.0/LICENSE` & `teensytoany-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/PKG-INFO` & `teensytoany-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teensytoany
-Version: 0.3.0
+Version: 0.4.0
 Summary: A pythonic way to access the teensytoany board
 Home-page: https://github.com/ramonaoptics/python-teensytoany
 Author: Ramona Optics Inc.
 Author-email: info@ramonaoptics.com
 License: BSD license
 Keywords: teensytoany
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -24,21 +24,33 @@
 
 # Python TeensyToAny
 
 
 [![pypi](https://img.shields.io/pypi/v/teensytoany.svg)](https://pypi.python.org/pypi/teensytoany)
 [![Travis](https://travis-ci.com/ramonaoptics/python-teensytoany.svg?branch=master)](https://travis-ci.com/ramonaoptics/python-teensytoany)
 [![Docs](https://readthedocs.org/projects/python-teensytoany/badge/?version=latest)](https://python-teensytoany.readthedocs.io/en/latest/?badge=latest)
-  
 
 A pythonic way to access the teensytoany board
 
-* Documentation: https://python-teensytoany.readthedocs.io.
 * See: https://github.com/ramonaoptics/teensy-to-any
 
+To program the teensy to any devices you will need the following additional dependencies:
+
+* `click`
+* `appdirs`
+* `requests`
+
+You can install them with:
+
+```bash
+conda install click appdirs requests
+# or
+pip install click appdirs requests
+```
+
 Features
 --------
 
 * TODO
 
 Credits
 -------
@@ -48,14 +60,20 @@
 [hmaarrfk/cookiecutter-pypackage](https://github.com/hmaarrfk/cookiecutter-pypackage)
 project template.
 
 
 
 # History
 
+## 0.4.0 (2024-04-05)
+
+* Provide functions to fetch local and remote firmware versions.
+* Provide a static method to program the latest firmware version and a CLI to
+  do so from the terminal.
+
 ## 0.3.0 (2024-04-02)
 
 * Add a `timeout` property to the functions that deal with updating the firmware.
 
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
```

### Comparing `teensytoany-0.3.0/docs/Makefile` & `teensytoany-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/docs/conf.py` & `teensytoany-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/docs/installation.rst` & `teensytoany-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/docs/make.bat` & `teensytoany-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/setup.py` & `teensytoany-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,19 @@
     install_requires=requirements,
     license="BSD license",
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='teensytoany',
     name='teensytoany',
+    entry_points={
+        'console_scripts': [
+            'teensytoany_programmer=teensytoany.programmer:teensytoany_programmer',
+        ],
+    },
     packages=find_packages(include=['teensytoany']),
     tests_require=test_requirements,
     url='https://github.com/ramonaoptics/python-teensytoany',
     version=version,
     cmdclass=cmdclass,
     zip_safe=False,
 )
```

### Comparing `teensytoany-0.3.0/teensytoany/_version.py` & `teensytoany-0.4.0/teensytoany/_version.py`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/teensytoany/teensypower.py` & `teensytoany-0.4.0/teensytoany/teensypower.py`

 * *Files identical despite different names*

### Comparing `teensytoany-0.3.0/teensytoany/teensytoany.py` & `teensytoany-0.4.0/teensytoany/teensytoany.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import subprocess
-import tempfile
 from time import sleep
 from typing import Sequence
 
 from packaging.version import Version
 from serial import LF, Serial
 from serial.tools.list_ports import comports
 
@@ -130,15 +129,38 @@
         """
         pairs = TeensyToAny._device_serial_number_pairs(
             serial_numbers=serial_numbers, device_name=device_name)
         _, serial_numbers = zip(*pairs)
         return serial_numbers
 
     @staticmethod
-    def _get_latest_available_firmware(*, timeout=2):
+    def get_latest_available_firmware_version(
+        *, mcu='TEENSY40', online=True, local=True, timeout=2
+    ):
+        if local:
+            local_versions = TeensyToAny._find_local_versions(mcu=mcu)
+            if len(local_versions) > 0:
+                latest = local_versions[-1]
+        try:
+            if online:
+                latest = TeensyToAny._get_latest_available_firmware_online(
+                    timeout=timeout)
+        except Exception:  # pylint: disable=broad-except
+            pass
+
+        if latest is None:
+            raise RuntimeError(
+                "Failed to fetch the latest release information. "
+                "Please check your internet connection and try again."
+            )
+
+        return latest
+
+    @staticmethod
+    def _get_latest_available_firmware_online(*, timeout=2):
         import requests  # pylint: disable=import-outside-toplevel
 
         repo_url = "https://api.github.com/repos/ramonaoptics/teensy-to-any"
         releases_url = f"{repo_url}/releases/latest"
 
         response = requests.get(releases_url, timeout=timeout)
 
@@ -170,64 +192,134 @@
         return pairs
 
     @property
     def mcu(self):
         return self._ask('mcu')
 
     def _update_firmware(self, *, mcu=None, force=False, timeout=2):
-        import requests  # pylint: disable=import-outside-toplevel
-
         current_version = self.version
+        serial_number = self.serial_number
         if mcu is None:
             mcu = self.mcu
 
         if mcu is None:
             raise RuntimeError(
                 "The current microcontroller is unknown, please specify it "
                 "before attempting to update the firmware.")
 
-        if os.name == 'nt':
-            # We do supporting updating, but it is "scary" to do so since
-            # there is no serial number specificity
-            raise RuntimeError("We do not supporting updating MCUs on windows")
-
-        latest_version = self._get_latest_available_firmware(timeout=timeout)
+        latest_version = self.get_latest_available_firmware_version(mcu=mcu, timeout=timeout)
         if not force:
             if Version(current_version) >= Version(latest_version):
                 return
 
-        file_url = f"https://github.com/ramonaoptics/teensy-to-any/releases/download/{latest_version}/firmware_{mcu.lower()}.hex"  # noqa # pylint: disable=line-too-long
+        self.close()
+        self._requested_serial_number = serial_number
+        try:
+            self.program_firmware(
+                serial_number,
+                mcu=mcu,
+                version=latest_version,
+                timeout=timeout
+            )
+            # Reraise any exceptions that were caught
+        finally:
+            self.open()
+
+    @staticmethod
+    def _find_local_versions(*, mcu=None):
+        firmware_dir = TeensyToAny._generate_firmware_directory(mcu=mcu)
+        if not firmware_dir.is_dir():
+            return []
+
+        versions = [
+            d.name
+            for d in firmware_dir.iterdir()
+            if d.is_dir() and (d / 'firmware.hex').is_file()
+        ]
 
-        firmware_filename = tempfile.mktemp(suffix='.hex')
+        versions.sort(key=Version)
+        return versions
+
+    @staticmethod
+    def _generate_firmware_filename(*, mcu, version):
+        firmware_dir = TeensyToAny._generate_firmware_directory(mcu=mcu)
+        firmware_filename = firmware_dir / f"{version}" / "firmware.hex"
+        return firmware_filename
 
+    @staticmethod
+    def _generate_firmware_directory(*, mcu):
+        from pathlib import Path  # pylint: disable=import-outside-toplevel
+
+        from appdirs import AppDirs  # pylint: disable=import-outside-toplevel
+        app = AppDirs('teensytoany', 'ramonaoptics')
+        cache_dir = Path(app.user_cache_dir)
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        firmware_dir = cache_dir / f"{mcu.lower()}"
+        firmware_dir.mkdir(parents=True, exist_ok=True)
+        return firmware_dir
+
+    @staticmethod
+    def download_firmware(*, mcu, version, timeout=2):
+        firmware_filename = TeensyToAny._generate_firmware_filename(mcu=mcu, version=version)
+
+        import requests  # pylint: disable=import-outside-toplevel
+        file_url = f"https://github.com/ramonaoptics/teensy-to-any/releases/download/{version}/firmware_{mcu.lower()}.hex"  # noqa # pylint: disable=line-too-long
         response = requests.get(file_url, timeout=timeout)
         if response.status_code != 200:
             raise RuntimeError("Failed to download firmware")
 
+        firmware_filename.parent.mkdir(parents=True, exist_ok=True)
         # Open the file for binary writing
         with open(firmware_filename, 'wb') as file:
             # Write the content to the file in chunks
             for chunk in response.iter_content(chunk_size=4096):
                 file.write(chunk)
 
-        requested_serial_number = self.serial_number
+        return firmware_filename
+
+    @staticmethod
+    def program_firmware(serial_number=None, *, mcu=None, version=None, timeout=2):
+        if serial_number is None:
+            available_serial_numbers = TeensyToAny.list_all_serial_numbers()
+            if len(available_serial_numbers) == 0:
+                raise RuntimeError("No TeensyToAny devices found.")
+            if len(available_serial_numbers) > 1:
+                raise RuntimeError(
+                    "Multiple TeensyToAny devices found. Please specify the "
+                    "serial number of the device you would like to program."
+                )
+            serial_number = available_serial_numbers[0]
+
+        if mcu is None:
+            raise RuntimeError("mcu must be provided and cannot be left as None.")
+
+        if version is None:
+            version = TeensyToAny.get_latest_available_firmware_version(timeout=timeout)
+
+        if os.name == 'nt':
+            # We do supporting updating, but it is "scary" to do so since
+            # there is no serial number specificity
+            raise RuntimeError("We do not supporting programing TeensyToAny devices on Windows")
+
+        firmware_filename = TeensyToAny._generate_firmware_filename(mcu=mcu, version=version)
+
+        if not firmware_filename.is_file():
+            TeensyToAny.download_firmware(mcu=mcu, version=version, timeout=timeout)
+
         cmd_list = [
             'teensy_loader_cli',
             '-s',
             f'--mcu={mcu}',
-            f'--serial-number={requested_serial_number}',
-            firmware_filename,
+            f'--serial-number={serial_number}',
+            str(firmware_filename),
         ]
 
-        self.close()
         subprocess.check_call(cmd_list)
         # Wait for the device to reboot
         sleep(1)
-        self._requested_serial_number = requested_serial_number
-        self.open()
 
     def __init__(
         self,
         serial_number=None, *,
         baudrate=115200,
         timeout=0.205,
         open=True,  # pylint: disable=redefined-builtin
```

### Comparing `teensytoany-0.3.0/teensytoany.egg-info/PKG-INFO` & `teensytoany-0.4.0/teensytoany.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teensytoany
-Version: 0.3.0
+Version: 0.4.0
 Summary: A pythonic way to access the teensytoany board
 Home-page: https://github.com/ramonaoptics/python-teensytoany
 Author: Ramona Optics Inc.
 Author-email: info@ramonaoptics.com
 License: BSD license
 Keywords: teensytoany
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -24,21 +24,33 @@
 
 # Python TeensyToAny
 
 
 [![pypi](https://img.shields.io/pypi/v/teensytoany.svg)](https://pypi.python.org/pypi/teensytoany)
 [![Travis](https://travis-ci.com/ramonaoptics/python-teensytoany.svg?branch=master)](https://travis-ci.com/ramonaoptics/python-teensytoany)
 [![Docs](https://readthedocs.org/projects/python-teensytoany/badge/?version=latest)](https://python-teensytoany.readthedocs.io/en/latest/?badge=latest)
-  
 
 A pythonic way to access the teensytoany board
 
-* Documentation: https://python-teensytoany.readthedocs.io.
 * See: https://github.com/ramonaoptics/teensy-to-any
 
+To program the teensy to any devices you will need the following additional dependencies:
+
+* `click`
+* `appdirs`
+* `requests`
+
+You can install them with:
+
+```bash
+conda install click appdirs requests
+# or
+pip install click appdirs requests
+```
+
 Features
 --------
 
 * TODO
 
 Credits
 -------
@@ -48,14 +60,20 @@
 [hmaarrfk/cookiecutter-pypackage](https://github.com/hmaarrfk/cookiecutter-pypackage)
 project template.
 
 
 
 # History
 
+## 0.4.0 (2024-04-05)
+
+* Provide functions to fetch local and remote firmware versions.
+* Provide a static method to program the latest firmware version and a CLI to
+  do so from the terminal.
+
 ## 0.3.0 (2024-04-02)
 
 * Add a `timeout` property to the functions that deal with updating the firmware.
 
 ## 0.2.0 (2023-11-07)
 
 * Add a `timeout` property to simplify modifying the command timeout.
```

### Comparing `teensytoany-0.3.0/teensytoany.egg-info/SOURCES.txt` & `teensytoany-0.4.0/teensytoany.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 teensytoany/__init__.py
 teensytoany/_static_version.py
 teensytoany/_version.py
+teensytoany/programmer.py
 teensytoany/teensypower.py
 teensytoany/teensytoany.py
 teensytoany.egg-info/PKG-INFO
 teensytoany.egg-info/SOURCES.txt
 teensytoany.egg-info/dependency_links.txt
+teensytoany.egg-info/entry_points.txt
 teensytoany.egg-info/not-zip-safe
 teensytoany.egg-info/requires.txt
 teensytoany.egg-info/top_level.txt
```

