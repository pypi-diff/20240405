# Comparing `tmp/HinetPy-0.8.0.tar.gz` & `tmp/HinetPy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HinetPy-0.8.0.tar", last modified: Thu Mar 28 12:58:08 2024, max compression
+gzip compressed data, was "HinetPy-0.8.1.tar", last modified: Sun Mar 31 06:49:07 2024, max compression
```

## Comparing `HinetPy-0.8.0.tar` & `HinetPy-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:58:08.410553 HinetPy-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:58:08.406553 HinetPy-0.8.0/HinetPy/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    47835 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-03-28 12:57:59.000000 HinetPy-0.8.0/HinetPy/win32.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:58:08.410553 HinetPy-0.8.0/HinetPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-28 12:58:08.000000 HinetPy-0.8.0/HinetPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 12:58:08.000000 HinetPy-0.8.0/HinetPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:58:08.000000 HinetPy-0.8.0/HinetPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 12:58:08.000000 HinetPy-0.8.0/HinetPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 12:58:08.000000 HinetPy-0.8.0/HinetPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-28 12:57:59.000000 HinetPy-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-28 12:57:59.000000 HinetPy-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-28 12:58:08.410553 HinetPy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-03-28 12:57:59.000000 HinetPy-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-03-28 12:57:59.000000 HinetPy-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 12:58:08.410553 HinetPy-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:49:07.237436 HinetPy-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:49:07.237436 HinetPy-0.8.1/HinetPy/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47835 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15381 2024-03-31 06:49:00.000000 HinetPy-0.8.1/HinetPy/win32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 06:49:07.237436 HinetPy-0.8.1/HinetPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-03-31 06:49:07.000000 HinetPy-0.8.1/HinetPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-31 06:49:07.000000 HinetPy-0.8.1/HinetPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 06:49:07.000000 HinetPy-0.8.1/HinetPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-31 06:49:07.000000 HinetPy-0.8.1/HinetPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 06:49:07.000000 HinetPy-0.8.1/HinetPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-31 06:49:00.000000 HinetPy-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 06:49:00.000000 HinetPy-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-03-31 06:49:07.237436 HinetPy-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-31 06:49:00.000000 HinetPy-0.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-31 06:49:00.000000 HinetPy-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 06:49:07.237436 HinetPy-0.8.1/setup.cfg
```

### Comparing `HinetPy-0.8.0/HinetPy/__init__.py` & `HinetPy-0.8.1/HinetPy/__init__.py`

 * *Files identical despite different names*

### Comparing `HinetPy-0.8.0/HinetPy/channel.py` & `HinetPy-0.8.1/HinetPy/channel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,20 @@
+"""
+Class for channels.
+"""
+
 from __future__ import annotations
 
-import logging
 import math
-
-# Setup the logger
-FORMAT = "[%(asctime)s] %(levelname)s: %(message)s"
-logging.basicConfig(level=logging.INFO, format=FORMAT, datefmt="%Y-%m-%d %H:%M:%S")
-logger = logging.getLogger(__name__)
+import warnings
 
 
 class Channel:
     """
-    Channel information for a single channel.
-
-    The information can be used to generate SAC polezero files.
+    Information for a single channel.
     """
 
     def __init__(  # noqa: PLR0913
         self,
         id: str,  # noqa: A002
         name: str,
         component: str,
@@ -27,16 +24,14 @@
         gain: float | str,
         damping: float | str,
         period: float | str,
         preamplification: float | str,
         lsb_value: float | str,
     ):
         """
-        Initialize a channel.
-
         Parameters
         ----------
         id
             Channel ID.
         name
             Station Name.
         component
@@ -56,67 +51,73 @@
         preamplification
             Preamplification value.
         lsb_value
             LSB value.
 
         Notes
         -----
-        The Hi-net website uses the moving-coil velocity-type seismometer.
-        See :doc:`/appendix/response` for details.
+        The Hi-net website uses the moving-coil velocity-type seismometer. See
+        :doc:`/appendix/response` for details.
         """
         self.id = id
         self.name = name
         self.component = component
         self.latitude = float(latitude)
         self.longitude = float(longitude)
         self.unit = unit
         self.gain = float(gain)
         self.damping = float(damping)
         self.period = float(period)
         self.preamplification = float(preamplification)
         self.lsb_value = float(lsb_value)
 
+    def _get_polezero(self):
+        """
+        Determine the polezero parameters.
+        """
+        # Calculate natural frequency
+        freq = 2.0 * math.pi / self.period
+
+        # Calculate poles by finding roots of equation s^2+2hws+w^2=0
+        self.zeros = 3
+        self.poles = 2
+        self.real = 0.0 - self.damping * freq
+        self.imaginary = freq * math.sqrt(1.0 - self.damping**2.0)
+
+        # Calculate the CONSTANT
+        fn = 20.0  # alaways assume normalization frequency is 20 Hz
+        s = complex(0, 2 * math.pi * fn)
+        self.a0 = abs((s**2 + 2 * self.damping * freq * s + freq**2) / s**2)
+        self.sensitivity = (
+            self.gain * math.pow(10, self.preamplification / 20.0) / self.lsb_value
+        )
+
     def write_sacpz(self, pzfile, keep_sensitivity=False):
         """
         Write channel information into a SAC polezero file.
 
         Parameters
         ----------
         pzfile: str
             Name of the SAC polezero file.
-        keep_sensitivity: bool
+        k9.999513e-01eep_sensitivity: bool
             Keep sensitivity in the SAC polezero "CONSTANT" or not.
         """
         chan_info = f"{self.name}.{self.component} ({self.id})"
         # Hi-net uses a moving-coil velocity-type seismometer.
         if self.unit != "m/s":
-            logger.warning(
-                "%s: Unit is not velocity. The PZ file may be wrong.", chan_info
-            )
-
-        try:
-            freq = 2.0 * math.pi / self.period
-        except ZeroDivisionError:
-            logger.warning("%s: Natural period = 0. Skipped.", chan_info)
+            msg = f"{chan_info}: Unit is not velocity. The PZ file may be wrong."
+            warnings.warn(msg, category=RuntimeWarning, stacklevel=2)
+        if self.period == 0.0:
+            msg = f"{chan_info}): Natural period = 0.0. Skipped."
+            warnings.warn(message=msg, category=RuntimeWarning, stacklevel=2)
             return
 
-        # calculate poles by finding roots of equation s^2+2hws+w^2=0
-        real = 0.0 - self.damping * freq
-        imaginary = freq * math.sqrt(1.0 - self.damping**2.0)
-
-        # calculate the CONSTANT
-        fn = 20.0  # alaways assume normalization frequency is 20 Hz
-        s = complex(0, 2 * math.pi * fn)
-        a0 = abs((s**2 + 2 * self.damping * freq * s + freq**2) / s**2)
-        if keep_sensitivity:
-            factor = math.pow(10, self.preamplification / 20.0)
-            constant = a0 * self.gain * factor / self.lsb_value
-        else:
-            constant = a0
-
+        self._get_polezero()
+        constant = self.a0 * self.sensitivity if keep_sensitivity else self.a0
         # write information to a SAC PZ file
         with open(pzfile, "w", encoding="utf8") as pz:
-            pz.write("ZEROS 3\n")
-            pz.write("POLES 2\n")
-            pz.write(f"{real:9.6f} {imaginary:9.6f}\n")
-            pz.write(f"{real:9.6f} {-imaginary:9.6f}\n")
+            pz.write(f"ZEROS {self.zeros}\n")
+            pz.write(f"POLES {self.poles}\n")
+            pz.write(f"{self.real:9.6f} {self.imaginary:9.6f}\n")
+            pz.write(f"{self.real:9.6f} {-self.imaginary:9.6f}\n")
             pz.write(f"CONSTANT {constant:e}\n")
```

### Comparing `HinetPy-0.8.0/HinetPy/client.py` & `HinetPy-0.8.1/HinetPy/client.py`

 * *Files identical despite different names*

### Comparing `HinetPy-0.8.0/HinetPy/header.py` & `HinetPy-0.8.1/HinetPy/header.py`

 * *Files identical despite different names*

### Comparing `HinetPy-0.8.0/HinetPy/utils.py` & `HinetPy-0.8.1/HinetPy/utils.py`

 * *Files identical despite different names*

### Comparing `HinetPy-0.8.0/HinetPy/win32.py` & `HinetPy-0.8.1/HinetPy/win32.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     >>> extract_sac(
     ...     "0101_201001010000_5.cnt",
     ...     "0101_20100101.ch",
     ...     filter_by_name="N.NA*",
     ...     filter_by_component="[NE]",
     ... )
     """
-    if not (data and ctable):
+    if data is None or ctable is None:
         logger.error("data or ctable is `None'. Data requests may fail. Skipped.")
         return
 
     channels = read_ctable(ctable)
     logger.info("%s channels found in %s.", len(channels), ctable)
     if filter_by_id or filter_by_name or filter_by_component:
         channels = _filter_channels(
@@ -191,15 +191,15 @@
 
     Extract only specified channels:
 
     >>> extract_sacpz(
     ...     "0101_20100101.ch", filter_by_name="N.NA*", filter_by_component="[NE]"
     ... )
     """
-    if not ctable:
+    if ctable is None:
         logger.error("ctable is `None'. Data requests may fail. Skipped.")
         return
 
     channels = read_ctable(ctable)
     if filter_by_chid or filter_by_name or filter_by_component:
         channels = _filter_channels(
             channels, filter_by_chid, filter_by_name, filter_by_component
@@ -292,36 +292,30 @@
     filter_by_name: list or str
         Filter channels by name. It can be a list of names or a wildcard.
     filter_by_component: list or str
         Filter channels by component. It can be a list of component names or a wildcard.
     """
 
     def _filter(channels, key, filters):
-        filtered_channels = []
+        """
+        Filter channels by filters, which can be either a list or a wildcard.
+        """
         if isinstance(filters, list):  # filter by list
-            filtered_channels = [
-                channel for channel in channels if getattr(channel, key) in filters
-            ]
-        elif isinstance(filters, str):  # filter by wildcard
-            filtered_channels = [
-                channel
-                for channel in channels
-                if fnmatch(getattr(channel, key), filters)
-            ]
-        else:
-            raise ValueError("Only list and wildcard filter are supported.")
-        return filtered_channels
-
-    if filter_by_id:
-        channels = _filter(channels, "id", filter_by_id)
-    if filter_by_name:
-        channels = _filter(channels, "name", filter_by_name)
-    if filter_by_component:
-        channels = _filter(channels, "component", filter_by_component)
-
+            return [chn for chn in channels if getattr(chn, key) in filters]
+        if isinstance(filters, str):  # filter by wildcard
+            return [chn for chn in channels if fnmatch(getattr(chn, key), filters)]
+        raise ValueError("Only list and wildcard filter are supported.")
+
+    for key, filter_by in (
+        ("id", filter_by_id),
+        ("name", filter_by_name),
+        ("component", filter_by_component),
+    ):
+        if filter_by is not None:
+            channels = _filter(channels, key, filter_by)
     return channels
 
 
 def _write_winprm(ctable, prmfile="win.prm"):
     """
     Write a four-line parameter file.
     """
```

### Comparing `HinetPy-0.8.0/HinetPy.egg-info/PKG-INFO` & `HinetPy-0.8.1/HinetPy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: HinetPy
-Version: 0.8.0
-Summary: A Python package to request and process seismic waveform data from NIED Hi-neta
+Version: 0.8.1
+Summary: A Python package to request and process seismic waveform data from NIED Hi-net
 Author-email: Dongdong Tian <seisman.info@gmail.com>
 Project-URL: homepage, https://seisman.github.io/HinetPy/
 Project-URL: documentation, https://seisman.github.io/HinetPy/
 Project-URL: repository, https://github.com/seisman/HinetPy
 Keywords: seismology,NIED,Hi-net,waveform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,24 +26,24 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: packaging
 Requires-Dist: requests
 
 .. image:: https://github.com/seisman/HinetPy/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/seisman/HinetPy/actions/workflows/tests.yml
-.. image:: https://codecov.io/gh/seisman/HinetPy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/seisman/HinetPy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/seisman/HinetPy
 .. image:: https://img.shields.io/github/release/seisman/HinetPy.svg
     :target: https://github.com/seisman/HinetPy/releases
 .. image:: https://img.shields.io/pypi/v/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/pypi/pyversions/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/github/license/seisman/HinetPy.svg
-    :target: https://github.com/seisman/HinetPy/blob/master/LICENSE
+    :target: https://github.com/seisman/HinetPy/blob/main/LICENSE
 .. image:: https://zenodo.org/badge/23509035.svg
     :target: https://zenodo.org/badge/latestdoi/23509035
 
 .. placeholder-for-doc-index
 
 `NIED Hi-net <https://www.hinet.bosai.go.jp/>`__ |
 `Source Code <https://github.com/seisman/HinetPy>`__ |
```

### Comparing `HinetPy-0.8.0/LICENSE` & `HinetPy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HinetPy-0.8.0/PKG-INFO` & `HinetPy-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: HinetPy
-Version: 0.8.0
-Summary: A Python package to request and process seismic waveform data from NIED Hi-neta
+Version: 0.8.1
+Summary: A Python package to request and process seismic waveform data from NIED Hi-net
 Author-email: Dongdong Tian <seisman.info@gmail.com>
 Project-URL: homepage, https://seisman.github.io/HinetPy/
 Project-URL: documentation, https://seisman.github.io/HinetPy/
 Project-URL: repository, https://github.com/seisman/HinetPy
 Keywords: seismology,NIED,Hi-net,waveform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -25,24 +26,24 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: packaging
 Requires-Dist: requests
 
 .. image:: https://github.com/seisman/HinetPy/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/seisman/HinetPy/actions/workflows/tests.yml
-.. image:: https://codecov.io/gh/seisman/HinetPy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/seisman/HinetPy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/seisman/HinetPy
 .. image:: https://img.shields.io/github/release/seisman/HinetPy.svg
     :target: https://github.com/seisman/HinetPy/releases
 .. image:: https://img.shields.io/pypi/v/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/pypi/pyversions/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/github/license/seisman/HinetPy.svg
-    :target: https://github.com/seisman/HinetPy/blob/master/LICENSE
+    :target: https://github.com/seisman/HinetPy/blob/main/LICENSE
 .. image:: https://zenodo.org/badge/23509035.svg
     :target: https://zenodo.org/badge/latestdoi/23509035
 
 .. placeholder-for-doc-index
 
 `NIED Hi-net <https://www.hinet.bosai.go.jp/>`__ |
 `Source Code <https://github.com/seisman/HinetPy>`__ |
```

### Comparing `HinetPy-0.8.0/README.rst` & `HinetPy-0.8.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .. image:: https://github.com/seisman/HinetPy/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/seisman/HinetPy/actions/workflows/tests.yml
-.. image:: https://codecov.io/gh/seisman/HinetPy/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/seisman/HinetPy/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/seisman/HinetPy
 .. image:: https://img.shields.io/github/release/seisman/HinetPy.svg
     :target: https://github.com/seisman/HinetPy/releases
 .. image:: https://img.shields.io/pypi/v/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/pypi/pyversions/HinetPy.svg
     :target: https://pypi.org/project/HinetPy/
 .. image:: https://img.shields.io/github/license/seisman/HinetPy.svg
-    :target: https://github.com/seisman/HinetPy/blob/master/LICENSE
+    :target: https://github.com/seisman/HinetPy/blob/main/LICENSE
 .. image:: https://zenodo.org/badge/23509035.svg
     :target: https://zenodo.org/badge/latestdoi/23509035
 
 .. placeholder-for-doc-index
 
 `NIED Hi-net <https://www.hinet.bosai.go.jp/>`__ |
 `Source Code <https://github.com/seisman/HinetPy>`__ |
```

### Comparing `HinetPy-0.8.0/pyproject.toml` & `HinetPy-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HinetPy"
-description = "A Python package to request and process seismic waveform data from NIED Hi-neta"
+description = "A Python package to request and process seismic waveform data from NIED Hi-net"
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [{name = "Dongdong Tian", email = "seisman.info@gmail.com"}]
 keywords = ["seismology", "NIED", "Hi-net", "waveform"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
```

