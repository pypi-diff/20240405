# Comparing `tmp/pynxtools-mpes-0.0.2.tar.gz` & `tmp/pynxtools-mpes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools-mpes-0.0.2.tar", last modified: Thu Apr  4 05:52:37 2024, max compression
+gzip compressed data, was "pynxtools-mpes-0.0.3.tar", last modified: Fri Apr  5 12:54:55 2024, max compression
```

## Comparing `pynxtools-mpes-0.0.2.tar` & `pynxtools-mpes-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.673642 pynxtools-mpes-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/pynxtools_mpes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pynxtools_mpes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pynxtools_mpes/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.685643 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 05:52:37.000000 pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:52:37.689643 pynxtools-mpes-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:52:37.677642 pynxtools-mpes-0.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   310749 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/Ref_nexus_mpes.log
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/config_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/eln_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)  6533728 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/data/xarray_saved_small_calibration.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-04 05:52:32.000000 pynxtools-mpes-0.0.2/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.496806 pynxtools-mpes-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.484806 pynxtools-mpes-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.488806 pynxtools-mpes-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.488806 pynxtools-mpes-0.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 12:54:55.496806 pynxtools-mpes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.488806 pynxtools-mpes-0.0.3/pynxtools_mpes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/pynxtools_mpes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/pynxtools_mpes/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.496806 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 12:54:55.000000 pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:54:55.496806 pynxtools-mpes-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.488806 pynxtools-mpes-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:54:55.488806 pynxtools-mpes-0.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   310749 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/tests/data/Ref_nexus_mpes.log
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/tests/data/config_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/tests/data/eln_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)  6533728 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/tests/data/xarray_saved_small_calibration.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-05 12:54:48.000000 pynxtools-mpes-0.0.3/tests/test_reader.py
```

### Comparing `pynxtools-mpes-0.0.2/.github/workflows/publish.yml` & `pynxtools-mpes-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/.github/workflows/pylint.yml` & `pynxtools-mpes-0.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/.github/workflows/pytest.yml` & `pynxtools-mpes-0.0.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/.gitignore` & `pynxtools-mpes-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/PKG-INFO` & `pynxtools-mpes-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-mpes
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>, Abeer Aurora <arora@fhi-berlin.mpg.de>, Laurenz Rettig <rettig@fhi-berlin.mpg.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-mpes
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-mpes/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pynxtools-mpes-0.0.2/dev-requirements.txt` & `pynxtools-mpes-0.0.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/pynxtools_mpes/reader.py` & `pynxtools-mpes-0.0.3/pynxtools_mpes/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,30 +177,38 @@
     "Sample": "SAMPLE[sample]",
     "Source": "source_TYPE[source]",
     "User": "USER[user]",
     "energy_resolution": "energy_resolution/resolution",
     "momentum_resolution": "RESOLUTION[momentum_resolution]/resolution",
     "temporal_resolution": "RESOLUTION[temporal_resolution]/resolution",
     "spatial_resolution": "RESOLUTION[spatial_resolution]/resolution",
+    "angular_resolution": "RESOLUTION[angular_resolution]/resolution",
     "sample_temperature": "temperature_sensor/value",
+    "drain_current": "drain_current_amperemeter/value",
 }
 
 REPLACE_NESTED = {
     "SAMPLE[sample]/chemical_formula": "SAMPLE[sample]/SUBSTANCE[substance]/molecular_formula_hill",
     "source_TYPE[source]/Probe": "source_TYPE[source_probe]",
     "source_TYPE[source]/Pump": "source_TYPE[source_pump]",
     "beam_TYPE[beam]/Probe": "beam_TYPE[beam_probe]",
     "beam_TYPE[beam]/Pump": "beam_TYPE[beam_pump]",
     "sample_history": "sample_history/notes",
+    "ELECTRONANALYSER[electronanalyser]/RESOLUTION[energy_resolution]": (
+        "ELECTRONANALYSER[electronanalyser]/energy_resolution"
+    ),
     "ELECTRONANALYSER[electronanalyser]/RESOLUTION[momentum_resolution]": (
         "ELECTRONANALYSER[electronanalyser]/momentum_resolution"
     ),
     "ELECTRONANALYSER[electronanalyser]/RESOLUTION[spatial_resolution]": (
         "ELECTRONANALYSER[electronanalyser]/spatial_resolution"
     ),
+    "ELECTRONANALYSER[electronanalyser]/RESOLUTION[angular_resolution]": (
+        "ELECTRONANALYSER[electronanalyser]/angular_resolution"
+    ),
     "SAMPLE[sample]/gas_pressure": "INSTRUMENT[instrument]/pressure_gauge/value",
     "SAMPLE[sample]/temperature": (
         "INSTRUMENT[instrument]/MANIPULATOR[manipulator]/temperature_sensor/value"
     ),
 }
```

### Comparing `pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/PKG-INFO` & `pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-mpes
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>, Abeer Aurora <arora@fhi-berlin.mpg.de>, Laurenz Rettig <rettig@fhi-berlin.mpg.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-mpes
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-mpes/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pynxtools-mpes-0.0.2/pynxtools_mpes.egg-info/SOURCES.txt` & `pynxtools-mpes-0.0.3/pynxtools_mpes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/pyproject.toml` & `pynxtools-mpes-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/tests/data/Ref_nexus_mpes.log` & `pynxtools-mpes-0.0.3/tests/data/Ref_nexus_mpes.log`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/tests/data/config_file.json` & `pynxtools-mpes-0.0.3/tests/data/config_file.json`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/tests/data/eln_data.yaml` & `pynxtools-mpes-0.0.3/tests/data/eln_data.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/tests/data/xarray_saved_small_calibration.h5` & `pynxtools-mpes-0.0.3/tests/data/xarray_saved_small_calibration.h5`

 * *Files identical despite different names*

### Comparing `pynxtools-mpes-0.0.2/tests/test_reader.py` & `pynxtools-mpes-0.0.3/tests/test_reader.py`

 * *Files identical despite different names*

