# Comparing `tmp/dream-tools-2.1.8.tar.gz` & `tmp/dream-tools-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream-tools-2.1.8.tar", last modified: Thu Oct 26 19:19:32 2023, max compression
+gzip compressed data, was "dream-tools-2.1.9.tar", last modified: Fri Apr  5 09:41:23 2024, max compression
```

## Comparing `dream-tools-2.1.8.tar` & `dream-tools-2.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.886450 dream-tools-2.1.8/
--rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.1.8/LICENSE
--rw-rw-rw-   0        0        0     1370 2023-10-26 19:19:32.885460 dream-tools-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      877 2023-02-28 12:24:28.000000 dream-tools-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.777812 dream-tools-2.1.8/dream_tools.egg-info/
--rw-rw-rw-   0        0        0     1370 2023-10-26 19:19:32.000000 dream-tools-2.1.8/dream_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2023-10-26 19:19:32.000000 dream-tools-2.1.8/dream_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-26 19:19:32.000000 dream-tools-2.1.8/dream_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-10-26 19:19:32.000000 dream-tools-2.1.8/dream_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-26 19:19:32.000000 dream-tools-2.1.8/dream_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.781800 dream-tools-2.1.8/dreamtools/
--rw-rw-rw-   0        0        0      681 2023-10-26 19:19:25.000000 dream-tools-2.1.8/dreamtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.823662 dream-tools-2.1.8/dreamtools/gamY/
--rw-rw-rw-   0        0        0       29 2020-01-24 14:37:03.000000 dream-tools-2.1.8/dreamtools/gamY/__init__.py
--rw-rw-rw-   0        0        0     3814 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/classes.py
--rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2488 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/extract_equations.py
--rw-rw-rw-   0        0        0     1062 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/extract_variables.py
--rw-rw-rw-   0        0        0    55936 2022-12-13 10:01:56.000000 dream-tools-2.1.8/dreamtools/gamY/gamY.py
--rw-rw-rw-   0        0        0     1541 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/gekko_endo_exo.py
--rw-rw-rw-   0        0        0     4532 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/patterns.py
--rw-rw-rw-   0        0        0     1135 2022-12-13 11:41:07.000000 dream-tools-2.1.8/dreamtools/gamY/rename_set.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.839622 dream-tools-2.1.8/dreamtools/gams_excel/
--rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.1.8/dreamtools/gams_excel/__init__.py
--rw-rw-rw-   0        0        0     3036 2022-02-09 15:48:57.000000 dream-tools-2.1.8/dreamtools/gams_excel/excel_endo_exo.py
--rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.1.8/dreamtools/gams_excel/gams_excel.py
--rw-rw-rw-   0        0        0     4045 2023-10-22 19:05:11.000000 dream-tools-2.1.8/dreamtools/gams_excel/gdx_to_excel.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.854557 dream-tools-2.1.8/dreamtools/gams_pandas/
--rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/gams_pandas/__init__.py
--rw-rw-rw-   0        0        0    17195 2023-10-26 19:19:14.000000 dream-tools-2.1.8/dreamtools/gams_pandas/gams_pandas.py
--rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/gams_pandas/gdx.py
--rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.1.8/dreamtools/gams_pandas/test_gams_pandas.py
--rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/gams_pandas/utility.py
-drwxrwxrwx   0        0        0        0 2023-10-26 19:19:32.883458 dream-tools-2.1.8/dreamtools/multiindex_plotly/
--rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/age_plot.py
--rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/dream_plotly_template.py
--rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/dream_settings.py
--rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/makro_settings.py
--rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/plotly_util.py
--rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/reporting.py
--rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/scratch.py
--rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/test_plot.py
--rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/test_timeseries_analysis.py
--rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.1.8/dreamtools/multiindex_plotly/timeseries_analysis.py
--rw-rw-rw-   0        0        0       42 2023-10-26 19:19:32.887446 dream-tools-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-03-01 09:02:40.000000 dream-tools-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.823083 dream-tools-2.1.9/
+-rw-rw-rw-   0        0        0     1093 2020-08-12 11:00:01.000000 dream-tools-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1438 2024-04-05 09:41:23.819110 dream-tools-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2023-02-28 12:24:28.000000 dream-tools-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.816130 dream-tools-2.1.9/dream_tools.egg-info/
+-rw-rw-rw-   0        0        0     1438 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1337 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 09:41:23.000000 dream-tools-2.1.9/dream_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.718737 dream-tools-2.1.9/dreamtools/
+-rw-rw-rw-   0        0        0      681 2024-04-05 09:33:37.000000 dream-tools-2.1.9/dreamtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.748118 dream-tools-2.1.9/dreamtools/gamY/
+-rw-rw-rw-   0        0        0       29 2020-01-24 14:37:03.000000 dream-tools-2.1.9/dreamtools/gamY/__init__.py
+-rw-rw-rw-   0        0        0     3814 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/classes.py
+-rw-rw-rw-   0        0        0     4423 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2488 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/extract_equations.py
+-rw-rw-rw-   0        0        0     1062 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/extract_variables.py
+-rw-rw-rw-   0        0        0    55936 2022-12-13 10:01:56.000000 dream-tools-2.1.9/dreamtools/gamY/gamY.py
+-rw-rw-rw-   0        0        0     1541 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/gekko_endo_exo.py
+-rw-rw-rw-   0        0        0     4532 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/patterns.py
+-rw-rw-rw-   0        0        0     1135 2022-12-13 11:41:07.000000 dream-tools-2.1.9/dreamtools/gamY/rename_set.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.761235 dream-tools-2.1.9/dreamtools/gams_excel/
+-rw-rw-rw-   0        0        0       25 2020-01-31 12:41:21.000000 dream-tools-2.1.9/dreamtools/gams_excel/__init__.py
+-rw-rw-rw-   0        0        0     3138 2024-04-05 09:32:29.000000 dream-tools-2.1.9/dreamtools/gams_excel/excel_endo_exo.py
+-rw-rw-rw-   0        0        0     2666 2020-10-09 09:58:26.000000 dream-tools-2.1.9/dreamtools/gams_excel/gams_excel.py
+-rw-rw-rw-   0        0        0     4045 2023-10-22 19:05:11.000000 dream-tools-2.1.9/dreamtools/gams_excel/gdx_to_excel.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.777317 dream-tools-2.1.9/dreamtools/gams_pandas/
+-rw-rw-rw-   0        0        0       89 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/__init__.py
+-rw-rw-rw-   0        0        0    17187 2024-04-05 09:32:21.000000 dream-tools-2.1.9/dreamtools/gams_pandas/gams_pandas.py
+-rw-rw-rw-   0        0        0     1481 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/gdx.py
+-rw-rw-rw-   0        0        0    11969 2023-10-26 19:08:17.000000 dream-tools-2.1.9/dreamtools/gams_pandas/test_gams_pandas.py
+-rw-rw-rw-   0        0        0     3321 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/gams_pandas/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:41:23.811984 dream-tools-2.1.9/dreamtools/multiindex_plotly/
+-rw-rw-rw-   0        0        0      385 2023-03-01 08:59:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/__init__.py
+-rw-rw-rw-   0        0        0     2854 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/age_plot.py
+-rw-rw-rw-   0        0        0     2084 2023-02-24 13:26:37.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_plotly_template.py
+-rw-rw-rw-   0        0        0    22704 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_settings.py
+-rw-rw-rw-   0        0        0      891 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/makro_settings.py
+-rw-rw-rw-   0        0        0        3 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/plotly_util.py
+-rw-rw-rw-   0        0        0     4445 2023-09-14 08:18:26.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/reporting.py
+-rw-rw-rw-   0        0        0     7201 2023-01-13 09:23:38.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/scratch.py
+-rw-rw-rw-   0        0        0     1897 2023-03-01 10:04:19.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/test_plot.py
+-rw-rw-rw-   0        0        0     2330 2023-01-25 09:50:54.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/test_timeseries_analysis.py
+-rw-rw-rw-   0        0        0    10640 2023-03-01 10:03:09.000000 dream-tools-2.1.9/dreamtools/multiindex_plotly/timeseries_analysis.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 09:41:23.823580 dream-tools-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-03-01 09:02:40.000000 dream-tools-2.1.9/setup.py
```

### Comparing `dream-tools-2.1.8/LICENSE` & `dream-tools-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/PKG-INFO` & `dream-tools-2.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.1.8
+Version: 2.1.9
 Summary: A collection of tools used by the Danish institute for economic modelling and forecasting, DREAM (http://dreammodel.dk).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: plotly
 
 # DREAM-tools
 A collection of tools used by [the Danish institute for economic modelling and forecasting, DREAM](http://dreammodel.dk).
 
 ## Gams-Pandas
 A wrapper around the [GAMS Python api](https://www.gams.com/latest/docs/API_PY_OVERVIEW.html) to move smoothly between GAMS and [Pandas](https://pandas.pydata.org/).
 GAMS parameters are represented as Pandas Series, using a MultiIndex in cases of multiple sets.
```

### Comparing `dream-tools-2.1.8/README.md` & `dream-tools-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dream_tools.egg-info/PKG-INFO` & `dream-tools-2.1.9/dream_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: dream-tools
-Version: 2.1.8
+Version: 2.1.9
 Summary: A collection of tools used by the Danish institute for economic modelling and forecasting, DREAM (http://dreammodel.dk).
 Home-page: https://github.com/MartinBonde/dream-tools
 Author: Martin Kirk Bonde
 Author-email: martin@bonde.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: plotly
 
 # DREAM-tools
 A collection of tools used by [the Danish institute for economic modelling and forecasting, DREAM](http://dreammodel.dk).
 
 ## Gams-Pandas
 A wrapper around the [GAMS Python api](https://www.gams.com/latest/docs/API_PY_OVERVIEW.html) to move smoothly between GAMS and [Pandas](https://pandas.pydata.org/).
 GAMS parameters are represented as Pandas Series, using a MultiIndex in cases of multiple sets.
```

### Comparing `dream-tools-2.1.8/dream_tools.egg-info/SOURCES.txt` & `dream-tools-2.1.9/dream_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/__init__.py` & `dream-tools-2.1.9/dreamtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .gams_pandas import *
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 
 # Global setting controlling the default name of the time index
 X_AXIS_NAME = "t"
 # Default axis position if no level named dt.X_AXIS_NAME is found
 X_AXIS_INDEX = -1 #  (-1 = last index is time)
 
 # Time settings, used for plot and prt functions
```

### Comparing `dream-tools-2.1.8/dreamtools/gamY/classes.py` & `dream-tools-2.1.9/dreamtools/gamY/classes.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/excel_endo_exo.py` & `dream-tools-2.1.9/dreamtools/gamY/excel_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/extract_equations.py` & `dream-tools-2.1.9/dreamtools/gamY/extract_equations.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/extract_variables.py` & `dream-tools-2.1.9/dreamtools/gamY/extract_variables.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/gamY.py` & `dream-tools-2.1.9/dreamtools/gamY/gamY.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/gekko_endo_exo.py` & `dream-tools-2.1.9/dreamtools/gamY/gekko_endo_exo.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/patterns.py` & `dream-tools-2.1.9/dreamtools/gamY/patterns.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gamY/rename_set.py` & `dream-tools-2.1.9/dreamtools/gamY/rename_set.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gams_excel/excel_endo_exo.py` & `dream-tools-2.1.9/dreamtools/gams_excel/excel_endo_exo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-"""
-Transform Excel work sheet into GAMS code to perform endo exo operations and change variable levels.
-"""
-import os
-import sys
-import pandas as pd
-import xlwings as xw
-
-
-def main():
-  #  Read execution parameters
-  workbook_path = os.path.abspath(sys.argv[1])
-  assert os.path.splitext(workbook_path)[1].lower() in [".xls", ".xlsx", ".xlsm"], \
-    f"{workbook_path} is not an Excel workbook"
-
-  output_path = os.path.abspath(sys.argv[2])
-
-  # Read Excel file
-  print(f"Read endo_exo sheet from {workbook_path}")
-  app = xw.App(visible=False)
-  workbook = xw.Book(workbook_path)
-  endo_exo = workbook.sheets["endo_exo"].range("B4:CK5000").options(pd.DataFrame, index=False).value
-  app.quit()
-
-  # Cast years in column header to ints
-  header = list(endo_exo)
-  year_columns_index = 4
-  header[year_columns_index:] = [int(i) for i in header[year_columns_index:]]
-  endo_exo.columns = header
-
-  endo_exo_strings = endo_exo.apply(row_to_GAMS, axis=1, result_type="reduce", year_columns_index=year_columns_index)
-
-  with open(output_path, "w") as file:
-    print(f"Write to {output_path}")
-    file.write("\n".join(endo_exo_strings))
-
-
-def row_to_GAMS(row, year_columns_index, comment_char="#"):
-  """Return GAMS code from row"""
-  endo_exo_strings = []
-  for interval in split_intervals(row[year_columns_index:]):
-    if interval and not row['#']:
-      interval_string = f"{interval[0]} <= t.val and t.val <= {interval[1]}"
-      if row.endo:
-        endo_exo_strings += [f"UNFIX {row.endo}$({interval_string});"]
-      if row.exo:
-        for t in interval:
-          val = row.loc[t]
-          name, elements = split_name(row.exo)
-          var_input = row.exo.strip()
-          if var_input.endswith("]")
-            var = f"{var_input[:-1]},'{t}']"
-            lagged = f"{var_input[:-1]},'{t-1}']"
-          else
-            var = f"{var_input}['{t}']"
-            lagged = f"{var_input}['{t-1}']"
-          if row.printcode == "dummy":
-            pass
-          elif row.printcode == "p":
-            endo_exo_strings += [f"{var}$(t.val = {t}) = (1 + {val}/100) * ;"]
-          elif row.printcode == "n":
-            endo_exo_strings += [f"{var}$() = {val};"]
-      else # Transfer comments
-      endo_exo_strings += [f"{comment_char} {i}" for i in row.dropna()]
-
-  return "\n".join(endo_exo_strings)
-
-def split_name(input):
-  """
-  Split Gekko syntax name
-  Return symbol name and a list of elements
-  Example:
-    >>> split_name("qI[#i,CON]")
-    "qI", ["#i", "'CON'"]
-  """
-  if "[" in input:
-    name, elements = input.strip().split("[", 1)
-    elements = elements[:-1].split(",")
-    elements = [e[1:] if (e[0] == "#") else f"'{e}'" for e in elements]
-  else:
-    name = input
-    elements = []
-  return name, elements
-
-
-def split_intervals(series):
-  interval = []
-  for year in series.dropna().index:
-    if (year - 1) not in interval:
-      if interval:
-        yield interval
-        interval = []
-    interval += [year]
-  yield interval
-
-
-def error(msg):
-  exit(f"ERROR! {msg}")
-
-
-if __name__ == "__main__":
-  main()
+"""
+Transform Excel work sheet into GAMS code to perform endo exo operations and change variable levels.
+"""
+import os
+import sys
+import pandas as pd
+import xlwings as xw
+
+
+def main():
+  #  Read execution parameters
+  workbook_path = os.path.abspath(sys.argv[1])
+  assert os.path.splitext(workbook_path)[1].lower() in [".xls", ".xlsx", ".xlsm"], \
+    f"{workbook_path} is not an Excel workbook"
+
+  output_path = os.path.abspath(sys.argv[2])
+
+  # Read Excel file
+  print(f"Read endo_exo sheet from {workbook_path}")
+  app = xw.App(visible=False)
+  workbook = xw.Book(workbook_path)
+  endo_exo = workbook.sheets["endo_exo"].range("B4:CK5000").options(pd.DataFrame, index=False).value
+  app.quit()
+
+  # Cast years in column header to ints
+  header = list(endo_exo)
+  year_columns_index = 4
+  header[year_columns_index:] = [int(i) for i in header[year_columns_index:]]
+  endo_exo.columns = header
+
+  endo_exo_strings = endo_exo.apply(row_to_GAMS, axis=1, result_type="reduce", year_columns_index=year_columns_index)
+
+  with open(output_path, "w") as file:
+    print(f"Write to {output_path}")
+    file.write("\n".join(endo_exo_strings))
+
+
+def row_to_GAMS(row, year_columns_index, comment_char="#"):
+  """Return GAMS code from row"""
+  endo_exo_strings = []
+  for interval in split_intervals(row[year_columns_index:]):
+    if interval and not row['#']:
+      interval_string = f"{interval[0]} <= t.val and t.val <= {interval[1]}"
+      if row.endo:
+        endo_exo_strings += [f"UNFIX {row.endo}$({interval_string});"]
+      if row.exo:
+        for t in interval:
+          val = row.loc[t]
+          name, elements = split_name(row.exo)
+          var_input = row.exo.strip()
+          if var_input.endswith("]")
+            var = f"{var_input[:-1]},'{t}']"
+            lagged = f"{var_input[:-1]},'{t-1}']"
+          else
+            var = f"{var_input}['{t}']"
+            lagged = f"{var_input}['{t-1}']"
+          if row.printcode == "dummy":
+            pass
+          elif row.printcode == "p":
+            endo_exo_strings += [f"{var}$(t.val = {t}) = (1 + {val}/100) * ;"]
+          elif row.printcode == "n":
+            endo_exo_strings += [f"{var}$() = {val};"]
+      else # Transfer comments
+      endo_exo_strings += [f"{comment_char} {i}" for i in row.dropna()]
+
+  return "\n".join(endo_exo_strings)
+
+def split_name(input):
+  """
+  Split Gekko syntax name
+  Return symbol name and a list of elements
+  Example:
+    >>> split_name("qI[#i,CON]")
+    "qI", ["#i", "'CON'"]
+  """
+  if "[" in input:
+    name, elements = input.strip().split("[", 1)
+    elements = elements[:-1].split(",")
+    elements = [e[1:] if (e[0] == "#") else f"'{e}'" for e in elements]
+  else:
+    name = input
+    elements = []
+  return name, elements
+
+
+def split_intervals(series):
+  interval = []
+  for year in series.dropna().index:
+    if (year - 1) not in interval:
+      if interval:
+        yield interval
+        interval = []
+    interval += [year]
+  yield interval
+
+
+def error(msg):
+  exit(f"ERROR! {msg}")
+
+
+if __name__ == "__main__":
+  main()
```

### Comparing `dream-tools-2.1.8/dreamtools/gams_excel/gams_excel.py` & `dream-tools-2.1.9/dreamtools/gams_excel/gams_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gams_excel/gdx_to_excel.py` & `dream-tools-2.1.9/dreamtools/gams_excel/gdx_to_excel.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gams_pandas/gams_pandas.py` & `dream-tools-2.1.9/dreamtools/gams_pandas/gams_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import gams
 import logging
 import builtins
 import time
 from copy import deepcopy
 from .utility import index_from_symbol, symbol_is_scalar, is_iterable, map_lowest_level, index_names_from_symbol, \
   all_na, map_to_int_where_possible
-import gams.transfer.numpy
+import gams.core.numpy
 
 logger = logging.getLogger(__name__)
 
 class GamsPandasDatabase:
   """
   GamsPandasDatabase converts sets, parameters, and variables between a GAMS database and Pandas series.
   When as symbol is first retrieved it is converted to a Pandas series and stored in self.series
@@ -24,15 +24,15 @@
 
   def __init__(self, database=None, workspace=None, auto_sort_index=True, sparse=True, reference_database=None):
     if database is None:
       if workspace is None:
         workspace = gams.GamsWorkspace()
       database = workspace.add_database()
     self.database = database
-    self.gams2numpy = gams.transfer.numpy.Gams2Numpy(database.workspace.system_directory)
+    self.gams2numpy = gams.core.numpy.Gams2Numpy(database.workspace.system_directory)
     self.auto_sort_index = auto_sort_index
     self.sparse = sparse
     self.reference_database = reference_database
     self.series = {}
 
   def __getattr__(self, item):
     return self[item]
```

### Comparing `dream-tools-2.1.8/dreamtools/gams_pandas/gdx.py` & `dream-tools-2.1.9/dreamtools/gams_pandas/gdx.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gams_pandas/test_gams_pandas.py` & `dream-tools-2.1.9/dreamtools/gams_pandas/test_gams_pandas.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/gams_pandas/utility.py` & `dream-tools-2.1.9/dreamtools/gams_pandas/utility.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/age_plot.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/age_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/dream_plotly_template.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_plotly_template.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/dream_settings.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/dream_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/makro_settings.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/makro_settings.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/reporting.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/reporting.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/scratch.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/scratch.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/test_plot.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/test_plot.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/test_timeseries_analysis.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/test_timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/dreamtools/multiindex_plotly/timeseries_analysis.py` & `dream-tools-2.1.9/dreamtools/multiindex_plotly/timeseries_analysis.py`

 * *Files identical despite different names*

### Comparing `dream-tools-2.1.8/setup.py` & `dream-tools-2.1.9/setup.py`

 * *Files identical despite different names*

