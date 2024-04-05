# Comparing `tmp/avoca-0.1.0.tar.gz` & `tmp/avoca-0.2.0.tar.gz`

## Comparing `avoca-0.1.0.tar` & `avoca-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 avoca-0.1.0/qa_nilu.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 avoca-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/export_nas.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/flags.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/io.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/logging.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/manager.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/requirements.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/settings.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/bindings/ebas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/__init__.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/abstract.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/concs.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/generate_classes_doc.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/rt.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/test.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/qa_class/zscore.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.1.0/avoca/utils/torch_models.py
--rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.1.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
--rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.1.0/data/voc_jan2jun_2023.csv
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 avoca-0.1.0/data/.avoca/config.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/quickstart.ipynb
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/bindings/ebas.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/bindings/gcwerks.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.1.0/docs/source/bindings/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.1.0/examples/config.yaml
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.1.0/examples/data_qa.ipynb
--rw-r--r--   0        0        0   396649 2020-02-02 00:00:00.000000 avoca-0.1.0/examples/read_nas.ipynb
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 avoca-0.1.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.1.0/LICENCE.txt
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 avoca-0.1.0/README.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 avoca-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 avoca-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 avoca-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/export_nas.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/flags.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/io.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/logging.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/manager.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/requirements.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/settings.py
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/bindings/ebas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/__init__.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/abstract.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/concs.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/generate_classes_doc.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/rt.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/test.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/zscore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/testing/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/testing/df.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/utils/torch_models.py
+-rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.2.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
+-rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.2.0/data/voc_jan2jun_2023.csv
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.2.0/data/.avoca/config.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/quickstart.ipynb
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/ebas.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/gcwerks.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/config.yaml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/data_qa.ipynb
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/read_nas.ipynb
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.2.0/tests/test_io.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.2.0/LICENCE.txt
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 avoca-0.2.0/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 avoca-0.2.0/PKG-INFO
```

### Comparing `avoca-0.1.0/avoca/flags.py` & `avoca-0.2.0/avoca/flags.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/manager.py` & `avoca-0.2.0/avoca/manager.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/requirements.py` & `avoca-0.2.0/avoca/requirements.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/settings.py` & `avoca-0.2.0/avoca/settings.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/bindings/ebas.py` & `avoca-0.2.0/avoca/bindings/ebas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module to handle data of the format required by ebas."""
 
 from __future__ import annotations
 
 import datetime
 import logging
-from datetime import timedelta
+import re
+from datetime import datetime, timedelta
 from enum import IntEnum
 from os import PathLike
 from pathlib import Path
 from typing import Any
 from warnings import warn
 
 import numpy as np
@@ -27,42 +28,57 @@
     QA_Flag.ZERO_NEG_CONC_EXT: 999,
     QA_Flag.INVALIDATED_EXT: 900,  # 	H 	Hidden and invalidated by data originator
     QA_Flag.EXTREME_VALUE: 458,  # V 	Extremely high value, outside four times standard deviation in a lognormal distribution
     QA_Flag.CALIBRATION: 683,  # 	I 	Invalid due to calibration. Used for Level 0.
     QA_Flag.BLANK: 684,  #  	Invalid due to zero/span check. Used for Level 0.
     QA_Flag.HEIGHT_INTEGRATION: 0,  # 	Valid
     QA_Flag.UNCORRELATED: 0,  # 	Valid
+    QA_Flag.MET_OFFICE_BASELINE: 0,  # 	Valid
+    QA_Flag.BELOW_DETECTION_LIMIT: 147,  # 	B 	Below detection limit
+    QA_Flag.POLLUTION: 900,
+    QA_Flag.SUSPICIOUS_RT: 900,
 }
 
 ebas_flag_to_avoca: dict[int, QA_Flag] = {
     ebas_flag: avoca_flag for avoca_flag, ebas_flag in flags_to_ebas.items()
 }
 # Set some flags with Multiple values to the same value
 ebas_flag_to_avoca.pop(0)  # 0 is valid in avoca
 ebas_flag_to_avoca[999] = QA_Flag.MISSING
+ebas_flag_to_avoca[900] = QA_Flag.INVALIDATED_EXT
 
-if not all([f in flags_to_ebas for f in QA_Flag]):
-    warn("Not all QA flags are mapped to Ebas flags")
+missing_flags = set(QA_Flag) - set(flags_to_ebas.keys())
+if missing_flags:
+    raise RuntimeError(
+        f"Not all QA flags are mapped to Ebas flags. Missing: {missing_flags}"
+    )
 
 
 class DataLevel(IntEnum):
     """Values for different type of data used by ebas."""
 
     AREAS = 0
     CONCS = 1
     QA_CONCS = 2
 
 
+def data_level_after_qa(data_level: DataLevel) -> DataLevel:
+    """Return the data level after the QA."""
+    if data_level == DataLevel.CONCS:
+        return DataLevel.QA_CONCS
+    return data_level
+
+
 def set_dataframe(
     nas,
     df_export: pd.DataFrame,
     compounds: dict[str, str],
     data_level: DataLevel,
-    start_offset: timedelta = timedelta(minutes=-30),
-    end_offset: timedelta = timedelta(minutes=-10),
+    start_offset: timedelta | None = None,
+    end_offset: timedelta | None = None,
     flag_all: list[int] = [],
 ):
     """Put the data from the export dataframe into the nas object.
 
     :arg nas: The nas object to fill
     :arg df_export: The dataframe with the data to export. Format follows the
         other avoca format.
@@ -70,22 +86,32 @@
         the names in df_export. Values are the names in ebas.
     :arg data_level: The level of the data to export.
     :arg start_offset: The offset to add to the start time
     :arg end_offset: The offset to add to the end time
 
     """
 
-    df_export[("-", "start_datetime")] = df_export.index + start_offset
-    df_export[("-", "end_datetime")] = df_export.index + end_offset
+    if ("-", "start_datetime") not in df_export.columns:
+        if start_offset is None:
+            raise ValueError(
+                "start_offset is required if start_datetime is not in df_export"
+            )
+        df_export[("-", "start_datetime")] = df_export.index + start_offset
+    if ("-", "end_datetime") not in df_export.columns:
+        if end_offset is None:
+            raise ValueError(
+                "end_offset is required if end_datetime is not in df_export"
+            )
+        df_export[("-", "end_datetime")] = df_export.index + end_offset
 
     nas.sample_times = [
         DatetimeInterval(start, end)
         for start, end in zip(
-            df_export[("-", "start_datetime")].dt.to_pydatetime(),
-            df_export[("-", "end_datetime")].dt.to_pydatetime(),
+            df_export[("-", "start_datetime")],
+            df_export[("-", "end_datetime")],
         )
     ]
 
     vars_to_export = {
         DataLevel.AREAS: ["area", "rt", "w"],
         DataLevel.CONCS: ["C"],
     }
@@ -207,14 +233,21 @@
     We use for that the calibration flag suggested by ebas.
     We have to assume that this flag is the same for all compounds.
     """
 
     logger = logging.getLogger(__name__)
     clean_for_df = {}
 
+    ebas_name_to_avoca = {
+        "pa": "area",
+        "pw": "w",
+        "rt": "rt",
+        "C": "C",
+    }
+
     compounds = []
 
     for var in nas.variables:
         if "metadata" not in var:
             continue
 
         metadata = var["metadata"]
@@ -234,14 +267,19 @@
             print("passing", title)
             continue
 
         compund, variable = title
         if compund not in compounds:
             compounds.append(compund)
 
+        # Convert the variable name to the avoca format
+        if variable not in ebas_name_to_avoca:
+            raise ValueError(f"Variable {variable} not recognized")
+        variable = ebas_name_to_avoca[variable]
+
         clean_for_df[(compund, variable)] = values
 
         flag_serie = pd.Series(
             [
                 sum([ebas_flag_to_avoca[f].value for f in flag_row])
                 for flag_row in var["flags"]
             ],
@@ -251,14 +289,16 @@
         if flag_col not in clean_for_df:
             clean_for_df[flag_col] = flag_serie
         else:
             clean_for_df[flag_col] |= flag_serie
 
     # Use the start of the intervals as the datetime (use 1 for the end)
     clean_for_df[("-", "datetime")] = [dt[0] for dt in nas.sample_times]
+    clean_for_df[("-", "start_datetime")] = clean_for_df[("-", "datetime")]
+    clean_for_df[("-", "end_datetime")] = [dt[1] for dt in nas.sample_times]
 
     is_calibration = {
         compound: (QA_Flag.CALIBRATION.value & clean_for_df[(compound, "flag")]).astype(
             bool
         )
         for compound in compounds
     }
@@ -331,7 +371,36 @@
         # Set values to nan when flagged missing
         # df_out.loc[(df_out[(c, 'flag')] & (QA_Flag.MISSING.value | QA_Flag.BELOW_DETECTION_LIMIT.value)) != 0, (c, 'C')] = np.nan
         df_out.loc[df_out[(c, "flag")] != 0, (c, "C")] = np.nan
 
     df_out[("-", "type")] = "air"
 
     return df_out
+
+
+def extract_concentration_field(text: str) -> dict[str, float]:
+    """Extract the concentrations from the text.
+
+    This is a temporary solution that we found to communicate the concentrations
+    of the standards thgrough the nas files.
+    """
+    # Define the regular expression pattern to match the concentrations field
+    concentration_pattern = r"Concentrations:\s*\{([^}]*)\}"
+    # Search for the concentration field in the text
+    concentration_match = re.search(concentration_pattern, text)
+    if concentration_match:
+        # Extract the concentration substring
+        concentration_substring = concentration_match.group(1)
+        # Split the substring by comma to separate individual concentrations
+        concentration_list = concentration_substring.split(",")
+        # Initialize an empty dictionary to store concentrations
+        concentrations = {}
+        for concentration in concentration_list:
+            # Split each concentration by '=' to separate compound and value
+            compound, value = concentration.split("=")
+            # Remove leading and trailing whitespaces
+            compound = compound.strip()
+            value = float(value.strip())  # Convert value to float
+            concentrations[compound] = value
+        return concentrations
+    else:
+        return {}
```

### Comparing `avoca-0.1.0/avoca/qa_class/abstract.py` & `avoca-0.2.0/avoca/qa_class/abstract.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/qa_class/concs.py` & `avoca-0.2.0/avoca/qa_class/concs.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/qa_class/generate_classes_doc.py` & `avoca-0.2.0/avoca/qa_class/generate_classes_doc.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 import logging
 from pathlib import Path
 
 import avoca
 from avoca.manager import AssignerManager
 
 
-def main():
+def main(directory: Path | None = None):
     logging.basicConfig(level=logging.INFO)
-    # Add the path to the avoca package
-    avoca_path = Path(*avoca.__path__).parent
-    qa_class_file = avoca_path / "docs" / "source" / "qa_classes.md"
+    if directory is None:
+        # Add the path to the avoca package
+        avoca_path = Path(*avoca.__path__).parent
+        directory = avoca_path / "docs" / "source"
+    else:
+        directory = Path(directory)
+    qa_class_file = directory / "qa_classes.md"
     logging.getLogger(__name__).info(f"Writing the QA classes to {qa_class_file}")
 
     # Get all the classes in the qa_class module
     assigners = AssignerManager._assigners_importpath
 
     # Write the rst file
     with open(qa_class_file, "w") as file:
-        # Write a link to this 
+        # Write a link to this
         file.write("(Models)=\n")
         file.write("# QA Classes\n\n")
 
         for assigner, assigner_importpath in assigners.items():
             # Get the docsting of the class
             # assigner_module = __import__(assigner_importpath, fromlist=[""])
             # assigner_class = getattr(assigner_module, assigner)
```

### Comparing `avoca-0.1.0/avoca/qa_class/rt.py` & `avoca-0.2.0/avoca/qa_class/rt.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/qa_class/test.py` & `avoca-0.2.0/avoca/qa_class/test.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/qa_class/zscore.py` & `avoca-0.2.0/avoca/qa_class/zscore.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/utils/__init__.py` & `avoca-0.2.0/avoca/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/avoca/utils/torch_models.py` & `avoca-0.2.0/avoca/utils/torch_models.py`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas` & `avoca-0.2.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/data/voc_jan2jun_2023.csv` & `avoca-0.2.0/data/voc_jan2jun_2023.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/docs/Makefile` & `avoca-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/docs/make.bat` & `avoca-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/docs/source/conf.py` & `avoca-0.2.0/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
+from pathlib import Path
+
 from avoca.qa_class import generate_classes_doc
 
-generate_classes_doc.main()
+this_path = Path(__file__).parent
+generate_classes_doc.main(this_path)
 
 project = "@voc@"
 copyright = "2024, Lionel Constantin, Empa"
 author = "Lionel Constantin, Empa"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "myst_nb",
-    #"myst_parser",
+    # "myst_parser",
     "sphinx.ext.autodoc",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = []
```

### Comparing `avoca-0.1.0/docs/source/index.rst` & `avoca-0.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/docs/source/quickstart.ipynb` & `avoca-0.2.0/docs/source/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/docs/source/bindings/ebas.md` & `avoca-0.2.0/docs/source/bindings/ebas.md`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/examples/data_qa.ipynb` & `avoca-0.2.0/examples/data_qa.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/LICENCE.txt` & `avoca-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `avoca-0.1.0/PKG-INFO` & `avoca-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.3
 Name: avoca
-Version: 0.1.0
+Version: 0.2.0
 Summary: @voc@: Quality assessement of measurement data
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://gitlab.com/empa503/atmospheric-measurements/avoca
+Project-URL: Bug Tracker, https://gitlab.com/empa503/atmospheric-measurements/avoca/-/issues
+Project-URL: Documentation, http://avoca.readthedocs.io/
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>
 License-File: LICENCE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: pandas
 Requires-Dist: pydantic
+Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

