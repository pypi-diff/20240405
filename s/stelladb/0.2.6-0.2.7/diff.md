# Comparing `tmp/stelladb-0.2.6.tar.gz` & `tmp/stelladb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stelladb-0.2.6.tar", last modified: Tue Apr  2 02:22:42 2024, max compression
+gzip compressed data, was "stelladb-0.2.7.tar", last modified: Thu Apr  4 19:47:24 2024, max compression
```

## Comparing `stelladb-0.2.6.tar` & `stelladb-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:42.678329 stelladb-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 02:21:49.000000 stelladb-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 02:22:42.678329 stelladb-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 02:21:49.000000 stelladb-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 02:22:42.678329 stelladb-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 02:21:49.000000 stelladb-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:42.678329 stelladb-0.2.6/stelladb/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 02:21:49.000000 stelladb-0.2.6/stelladb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-02 02:22:42.678329 stelladb-0.2.6/stelladb/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    26426 2024-04-02 02:21:49.000000 stelladb-0.2.6/stelladb/db_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-02 02:21:49.000000 stelladb-0.2.6/stelladb/db_vmec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:22:42.678329 stelladb-0.2.6/stelladb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 02:22:42.000000 stelladb-0.2.6/stelladb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 02:22:42.000000 stelladb-0.2.6/stelladb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:22:42.000000 stelladb-0.2.6/stelladb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 02:22:42.000000 stelladb-0.2.6/stelladb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 02:22:42.000000 stelladb-0.2.6/stelladb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:47:24.021346 stelladb-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 19:46:33.000000 stelladb-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-04 19:47:24.021346 stelladb-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-04 19:46:33.000000 stelladb-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 19:47:24.021346 stelladb-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-04 19:46:33.000000 stelladb-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:47:24.021346 stelladb-0.2.7/stelladb/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 19:46:33.000000 stelladb-0.2.7/stelladb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 19:47:24.021346 stelladb-0.2.7/stelladb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21583 2024-04-04 19:46:33.000000 stelladb-0.2.7/stelladb/db_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-04-04 19:46:33.000000 stelladb-0.2.7/stelladb/db_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-04 19:46:33.000000 stelladb-0.2.7/stelladb/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-04 19:46:33.000000 stelladb-0.2.7/stelladb/getters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:47:24.021346 stelladb-0.2.7/stelladb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-04 19:47:24.000000 stelladb-0.2.7/stelladb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 19:47:24.000000 stelladb-0.2.7/stelladb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:47:24.000000 stelladb-0.2.7/stelladb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 19:47:24.000000 stelladb-0.2.7/stelladb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 19:47:24.000000 stelladb-0.2.7/stelladb.egg-info/top_level.txt
```

### Comparing `stelladb-0.2.6/LICENSE` & `stelladb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.6/PKG-INFO` & `stelladb-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.6
+Version: 0.2.7
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
```

### Comparing `stelladb-0.2.6/README.md` & `stelladb-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.6/setup.py` & `stelladb-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `stelladb-0.2.6/stelladb/db_desc.py` & `stelladb-0.2.7/stelladb/db_desc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
-from desc.equilibrium import Equilibrium, EquilibriaFamily
-from desc.grid import LinearGrid
-from desc.vmec_utils import ptolemy_identity_rev, zernike_to_fourier
+import numpy as np
+import csv
 import zipfile
-import warnings
+from datetime import date
 
-from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
+from desc.equilibrium import Equilibrium, EquilibriaFamily
+from desc.grid import LinearGrid
+from desc.vmec_utils import ptolemy_identity_rev, zernike_to_fourier
 from desc.io.hdf5_io import hdf5Reader
 from desc.io.equilibrium_io import load
-import numpy as np
-import csv
-from datetime import date
+
+from .getters import get_hash_config, get_driver, get_hash_desc
+from .device import device_or_concept_to_csv
 
 
 def save_to_db_desc(  # pragma: no cover
     eq,
     config_name,
     user,
     isDeviceNew=False,
@@ -256,24 +257,14 @@
             os.remove(zip_filename)
             os.remove(csv_filename)
             os.remove(config_csv_filename)
             os.remove(inputfilename)
             if isDeviceNew:
                 os.remove(device_csv_filename)
 
-    if os.path.exists("auto_save.h5"):
-        os.remove("auto_save.h5")
-    if not copy:
-        os.remove(zip_filename)
-        os.remove(csv_filename)
-        os.remove(config_csv_filename)
-        os.remove(inputfilename)
-        if isDeviceNew:
-            os.remove(device_csv_filename)
-
 
 def desc_to_csv(  # noqa
     eq,
     name=None,
     provenance=None,
     description=None,
     inputfilename=None,
@@ -571,166 +562,7 @@
             if not configurations_csv_exists:
                 writer.writeheader()  # only need header if file did not exist already
             writer.writerow(data_configurations)
     except OSError:
         print("I/O error")
 
     return None
-
-
-def device_or_concept_to_csv(  # noqa
-    deviceid,
-    name=None,
-    device_class=None,
-    NFP=None,
-    description=None,
-    stell_sym=False,
-    user_created=None,
-    user_updated=None,
-):
-    """Save DESC as a csv with relevant information.
-
-    Args
-    ----
-        name : str
-            name of the device
-        device_class (str): 
-            class of device i.e. quasisymmetry (QA, QH, QP)
-            or omnigenity (QI, OT, OH) or axisymmetry (AS).
-        NFP : (int)
-            (Nominal) number of field periods for the device/concept
-        description : (str)
-            description of the device/concept
-        stell_sym : (bool)
-            (Nominal) stellarator symmetry of the device
-            (stellarator symmetry defined as R(theta, zeta) = R(-theta,-zeta)
-            and Z(theta, zeta) = -Z(-theta,-zeta))
-
-    Returns
-    -------
-        None
-    """
-    # data dicts for each table
-    devices_and_concepts = {}
-
-    devices_csv_name = "devices_and_concepts.csv"
-
-    devices_and_concepts["deviceid"] = deviceid
-    devices_and_concepts["name"] = name if name is not None else deviceid
-    devices_and_concepts["class"] = device_class
-
-    devices_and_concepts["NFP"] = NFP
-    devices_and_concepts["stell_sym"] = bool(stell_sym)
-
-    devices_and_concepts["description"] = description
-    if user_created is not None:
-        devices_and_concepts["user_created"] = user_created
-    if user_updated is not None:
-        devices_and_concepts["user_updated"] = user_updated
-
-    today = date.today()
-    devices_and_concepts["date_created"] = today
-    devices_and_concepts["date_updated"] = today
-
-    devices_and_concepts["hashkey"] = get_hash_device(devices_and_concepts)
-
-    csv_columns_desc_runs = list(devices_and_concepts.keys())
-    csv_columns_desc_runs.sort()
-    desc_runs_csv_exists = os.path.isfile(devices_csv_name)
-
-    try:
-        with open(devices_csv_name, "a+") as csvfile:
-            writer = csv.DictWriter(csvfile, fieldnames=csv_columns_desc_runs)
-            if not desc_runs_csv_exists:
-                writer.writeheader()  # only need header if file did not exist already
-            writer.writerow(devices_and_concepts)
-    except OSError:
-        print("I/O error")
-
-    return None
-
-
-def get_hash_desc(eq, data_desc_runs, config_hash):
-    """Get a unique identifier for a DESC equilibrium."""
-    if not isinstance(eq, Equilibrium):
-        warnings.warn(f"Expected type Equilibrium for eq, got type {type(eq)}")
-
-    unique_id = (
-        f"{eq.L}{eq.M}{eq.N}{eq.NFP}{config_hash}{data_desc_runs['current_profile']}"
-        + f"{data_desc_runs['iota_profile']}{data_desc_runs['pressure_profile']}{eq.params_dict}"
-    )
-
-    return hash(unique_id)
-
-
-def get_hash_config(data_configurations):
-    """Get a unique identifier for configuration."""
-
-    unique_id = ""
-    for key in data_configurations.keys():
-        if key not in [
-            "config_name",
-            "name",
-            "provenance",
-            "description",
-            "device_name",
-            "date_created",
-            "date_updated",
-            "user_created",
-            "user_updated",
-        ]:
-            unique_id += f"{data_configurations[key]}"
-
-    return hash(unique_id)
-
-
-def get_hash_device(devices_and_concepts):
-    """Get a unique identifier for configuration."""
-
-    unique_id = ""
-    for key in devices_and_concepts.keys():
-        if key not in [
-            "date_created",
-            "date_updated",
-            "user_created",
-            "user_updated",
-        ]:
-            unique_id += f"{devices_and_concepts[key]}"
-
-    return hash(unique_id)
-
-
-def get_driver():  # pragma: no cover
-    """Initialize a webdriver for use in uploading to the database."""
-
-    try:
-        options = webdriver.ChromeOptions()
-        options.headless = True
-        return webdriver.Chrome(options=options)
-    except:  # noqa: E722
-        pass
-
-    try:
-        options = webdriver.FirefoxOptions()
-        options.headless = True
-        return webdriver.Firefox(options=options)
-    except:  # noqa: E722
-        pass
-
-    try:
-        return webdriver.Safari()
-    except:  # noqa: E722
-        pass
-
-    try:
-        options = webdriver.EdgeOptions()
-        options.use_chromium = True
-        options.add_argument("headless")
-        return webdriver.Edge(options=options)
-    except:  # noqa: E722
-        warnings.warn(
-            "Failed to initialize any webdriver! Consider installing "
-            + "Chrome, Safari, Firefox, or Edge."
-        )
-
-    # If no browser was successfully initialized, return None
-    return None
```

### Comparing `stelladb-0.2.6/stelladb/db_vmec.py` & `stelladb-0.2.7/stelladb/db_vmec.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 from datetime import date
 
 import numpy as np
 from scipy.interpolate import InterpolatedUnivariateSpline
 from simsopt.mhd.vmec import Vmec
 
+from .device import device_or_concept_to_csv
+
 # TODO: add threshold to truncate at what amplitude surface Fourier coefficient
 # that it is working
 
 # TODO: make arrays stored in one line
 
 # TODO: either make separate utilities for desc_runs csv and configurations csv,
 # or have the utility somehow check for if the configuration exists already,
@@ -288,62 +290,7 @@
             if not configurations_csv_exists:
                 writer.writeheader()  # only need header if file did not exist already
             writer.writerow(data_configurations)
     except OSError:
         print("I/O error")
 
     return None
-
-
-def device_or_concept_to_csv(  # noqa
-    name,
-    device_class=None,
-    NFP=None,
-    description=None,
-    stell_sym=False,
-    deviceid=None,
-):
-    """Save concept as a csv with relevant information.
-
-    Args
-    ----
-        device_class (str): class of device i.e. quasisymmetry (QA, QH, QP)
-            or omnigenity (QI, OT, OH) or axisymmetry (AS).
-        NFP (int): (Nominal) number of field periods for the device/concept
-        description (str): description of the device/concept
-        stell_sym (bool): (Nominal) stellarator symmetry of the device
-            (stellarator symmetry defined as R(theta, zeta) = R(-theta,-zeta)
-            and Z(theta, zeta) = -Z(-theta,-zeta))
-        deviceid (str): unique identifier for this device
-
-    Returns
-    -------
-        None
-    """
-    # data dicts for each table
-    devices_and_concepts = {}
-
-    devices_csv_name = "devices_and_concepts.csv"
-
-    devices_and_concepts["name"] = name
-    devices_and_concepts["class"] = device_class
-
-    devices_and_concepts["NFP"] = NFP
-    devices_and_concepts["stell_sym"] = bool(stell_sym)
-
-    devices_and_concepts["description"] = description
-    devices_and_concepts["deviceid"] = deviceid
-
-    csv_columns_runs = list(devices_and_concepts.keys())
-    csv_columns_runs.sort()
-    runs_csv_exists = os.path.isfile(devices_csv_name)
-
-    try:
-        with open(devices_csv_name, "a+") as csvfile:
-            writer = csv.DictWriter(csvfile, fieldnames=csv_columns_runs)
-            if not runs_csv_exists:
-                writer.writeheader()  # only need header if file did not exist already
-            writer.writerow(devices_and_concepts)
-    except OSError:
-        print("I/O error")
-
-    return None
```

### Comparing `stelladb-0.2.6/stelladb.egg-info/PKG-INFO` & `stelladb-0.2.7/stelladb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stelladb
-Version: 0.2.6
+Version: 0.2.7
 Summary: Includes functions to upload DESC and VMEC data to the stellarator database.
 Home-page: https://github.com/PlasmaControl/Stellarator-Database/
 Author: Yigit Gunsur Elmacioglu, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Keywords: stellarator tokamak equilibrium perturbation mhd magnetohydrodynamics stability confinement plasma physics optimization design fusion data database
 Requires-Python: >=3.9
```

