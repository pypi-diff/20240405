# Comparing `tmp/cfr-2024.4.3.tar.gz` & `tmp/cfr-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2024.4.3.tar", last modified: Wed Apr  3 20:14:11 2024, max compression
+gzip compressed data, was "cfr-2024.4.4.tar", last modified: Fri Apr  5 00:39:53 2024, max compression
```

## Comparing `cfr-2024.4.3.tar` & `cfr-2024.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.879259 cfr-2024.4.3/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-2024.4.3/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-03 20:14:11.877837 cfr-2024.4.3/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1421 2024-03-13 16:55:21.000000 cfr-2024.4.3/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.790999 cfr-2024.4.3/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5134 2023-07-10 00:08:10.000000 cfr-2024.4.3/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.807922 cfr-2024.4.3/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      732 2023-07-10 00:08:10.000000 cfr-2024.4.3/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    27431 2024-04-03 20:06:27.000000 cfr-2024.4.3/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.873979 cfr-2024.4.3/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-2024.4.3/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-2024.4.3/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-2024.4.3/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-2024.4.3/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    80829 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    45544 2024-04-03 20:12:58.000000 cfr-2024.4.3/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60527 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6083 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    19837 2023-07-10 00:08:11.000000 cfr-2024.4.3/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    25886 2024-04-03 20:09:47.000000 cfr-2024.4.3/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    62418 2024-03-13 16:55:21.000000 cfr-2024.4.3/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-03 20:14:11.876168 cfr-2024.4.3/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-2024.4.3/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      201 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2024-04-03 20:14:10.000000 cfr-2024.4.3/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-03 20:14:11.879402 cfr-2024.4.3/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1453 2024-04-03 20:10:08.000000 cfr-2024.4.3/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.146807 cfr-2024.4.4/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-2024.4.4/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-05 00:39:53.145863 cfr-2024.4.4/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1421 2024-03-13 16:55:21.000000 cfr-2024.4.4/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.088819 cfr-2024.4.4/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5134 2023-07-10 00:08:10.000000 cfr-2024.4.4/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.127561 cfr-2024.4.4/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      732 2023-07-10 00:08:10.000000 cfr-2024.4.4/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    27431 2024-04-03 20:06:27.000000 cfr-2024.4.4/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.141879 cfr-2024.4.4/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-2024.4.4/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-2024.4.4/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-2024.4.4/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-2024.4.4/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    81175 2024-04-04 23:19:07.000000 cfr-2024.4.4/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49870 2024-04-04 23:42:37.000000 cfr-2024.4.4/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60527 2024-03-13 16:55:21.000000 cfr-2024.4.4/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6083 2024-03-13 16:55:21.000000 cfr-2024.4.4/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    19837 2023-07-10 00:08:11.000000 cfr-2024.4.4/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    25886 2024-04-03 20:09:47.000000 cfr-2024.4.4/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    62601 2024-04-04 21:58:32.000000 cfr-2024.4.4/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2024-04-05 00:39:53.143906 cfr-2024.4.4/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2683 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      373 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-2024.4.4/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      201 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2024-04-05 00:39:51.000000 cfr-2024.4.4/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2024-04-05 00:39:53.146914 cfr-2024.4.4/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1453 2024-04-05 00:39:18.000000 cfr-2024.4.4/setup.py
```

### Comparing `cfr-2024.4.3/LICENSE` & `cfr-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/PKG-INFO` & `cfr-2024.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2024.4.3/README.md` & `cfr-2024.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/bin/cfr` & `cfr-2024.4.4/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/__init__.py` & `cfr-2024.4.4/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/climate.py` & `cfr-2024.4.4/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/da/enkf.py` & `cfr-2024.4.4/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/gcm.py` & `cfr-2024.4.4/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/ml.py` & `cfr-2024.4.4/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/proxy.py` & `cfr-2024.4.4/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         ('glacier ice', 'deterium excess'): 'ice.d-excess',
         ('glacier ice', 'isotope diffusion'): 'ice.isotope_diffusion',
         ('glacier ice', 'hybrid-ice'): 'ice.hybrid',
         ('glacier ice', '15N/40Ar fractionation'): 'ice.15N40Ar',
         ('speleothem', 'd18O'): 'speleothem.d18O',
         ('speleothem', 'dD'): 'speleothem.dD',
         ('marine sediment', 'TEX86'): 'marine.TEX86',
+        ('marine sediment', 'UK37'): 'marine.UK37',
         ('marine sediment', 'Mg/Ca'): 'marine.MgCa',
         ('marine sediment', 'foram Mg/Ca'): 'marine.MgCa',
         ('marine sediment', 'd18O'): 'marine.d18O',
         ('marine sediment', 'dynocist MAT'): 'marine.MAT',
         ('marine sediment', 'alkenone'): 'marine.alkenone',
         ('marine sediment', 'planktonic foraminifera'): 'marine.foram',
         ('marine sediment', 'foraminifera'): 'marine.foram',
@@ -473,15 +474,15 @@
         
         for field in fields:
             name = field.da.name
             if tag is not None:
                 name = f'{tag}.{name}'
 
             nda = field.da.sel(lat=self.lat, lon=self.lon, **_kwargs)
-            if np.all(np.isnan(nda.values)):
+            if np.all(np.isnan(nda.values)) and search_dist is not None:
                 for i in range(1, search_dist+1):
                     p_header(f'{self.pid} >>> Nearest climate is NaN. Searching around within distance of {i} deg ...')
                     da_cond = field.da.where(np.abs(field.da.lat - self.lat)<= i).where(
                         np.abs(field.da.lon - self.lon) <= i
                     )
                     nda = utils.geo_mean(da_cond)
                     nda.coords['lat'] = self.lat
@@ -489,17 +490,21 @@
                     if not np.all(np.isnan(nda.values)):
                         p_success(f'{self.pid} >>> Found nearest climate within distance of {i} deg.')
                         break
 
             if not hasattr(self, 'clim'):
                 self.clim = {}
 
-            self.clim[name] = ClimateField(nda)
-            if load: self.clim[name].da.load()
-            if verbose: utils.p_success(f'{self.pid} >>> ProxyRecord.clim["{name}"] created.')
+            if 'nda' in locals():
+                self.clim[name] = ClimateField(nda)
+                if load: self.clim[name].da.load()
+                if verbose: utils.p_success(f'{self.pid} >>> ProxyRecord.clim["{name}"] created.')
+            else:
+                self.clim[name] = None
+                utils.p_fail(f'{self.pid} >>> ProxyRecord.clim["{name}"] = None')
 
     def correct_elev_tas(self, t_rate=-9.8, verbose=False):
         ''' Correct the tas with t_rate = -9.8 degC/km upward by default.
 
         Args:
             t_rage (float): the temperature adjustment rate based on elevation bias.
             verbose (bool, optional): print verbose information. Defaults to False.
@@ -1191,14 +1196,17 @@
             time = row[time_column]
             if type(time) is str:
                 time = utils.arr_str2np(time)
             value = row[value_column]
             if type(value) is str:
                 value = utils.arr_str2np(value)
 
+            time = np.atleast_1d(time)
+            value = np.atleast_1d(value)
+
             if len(time) != len(value):
                 print(row[value_column])
                 print(value)
 
             time, value = utils.clean_ts(time, value)
             value_name=row[value_name_column] if value_name_column in row else None
             value_unit=row[value_unit_column] if value_name_column in row else None
```

### Comparing `cfr-2024.4.3/cfr/psm.py` & `cfr-2024.4.4/cfr/psm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tqdm import tqdm
 from multiprocessing import cpu_count
 try:
     import statsmodels.formula.api as smf
     from pathos.multiprocessing import ProcessingPool as Pool
     import fbm
     import PyVSL
+    import pybaywatch as pb
 except:
     pass
 
 from . import utils
 from .proxy import ProxyRecord
 
 def clean_df(df, mask=None):
@@ -1138,8 +1139,129 @@
             ptype=self.pobj.ptype,
             value_name=self.pobj.value_name,
             value_unit=self.pobj.value_unit,
             time_name=self.pobj.time_name,
             time_unit=self.pobj.time_unit,
         )
 
+        return pp
+
+
+class BayTEX86:
+    ''' Baysian PSM for TEX86
+    
+    References:
+        Tierney, J. E. & Tingley, M. P. A Bayesian, spatially-varying calibration model for the TEX86 proxy. Geochimica et Cosmochimica Acta 127, 83-106 (2014).
+    '''
+    def __init__(self, pobj=None, climate_required=['sst']):
+        self.pobj = pobj
+        self.climate_required = climate_required
+
+    def forward(self, seed=2333, type='SST', mode='analog', tolerance=1):
+        vn = f'model.{self.climate_required[0]}'
+        res = pb.TEX_forward(self.pobj.lat, self.pobj.lon, self.pobj.clim[vn].da.values, seed=seed, type=type, mode=mode, tolerance=tolerance)
+        pct = np.percentile(res, q=[5, 50, 95], axis=1)
+
+        pp = ProxyRecord(
+            pid=self.pobj.pid,
+            time=self.pobj.clim[vn].da.time,
+            value=pct[1],  # median
+            lat=self.pobj.lat,
+            lon=self.pobj.lon,
+            ptype=self.pobj.ptype,
+            value_name=self.pobj.value_name,
+            value_unit=self.pobj.value_unit,
+            time_name=self.pobj.time_name,
+            time_unit=self.pobj.time_unit,
+        )
+        return pp
+
+class BayUK37:
+    ''' Baysian PSM for UK37
+    
+    References:
+        Tierney, J. E. & Tingley, M. P. BAYSPLINE: A New Calibration for the Alkenone Paleothermometer. Paleoceanography and Paleoclimatology 33, 281-301 (2018).
+    '''
+    def __init__(self, pobj=None, climate_required=['sst']):
+        self.pobj = pobj
+        self.climate_required = climate_required
+
+    def forward(self, seed=2333):
+        vn = f'model.{self.climate_required[0]}'
+        res = pb.UK_forward(self.pobj.clim[vn].da.values, seed=seed)
+        pct = np.percentile(res, q=[5, 50, 95], axis=1)
+
+        pp = ProxyRecord(
+            pid=self.pobj.pid,
+            time=self.pobj.clim[vn].da.time,
+            value=pct[1],  # median
+            lat=self.pobj.lat,
+            lon=self.pobj.lon,
+            ptype=self.pobj.ptype,
+            value_name=self.pobj.value_name,
+            value_unit=self.pobj.value_unit,
+            time_name=self.pobj.time_name,
+            time_unit=self.pobj.time_unit,
+        )
+        return pp
+
+
+class BayD18O:
+    ''' Baysian PSM for foram d18O
+    
+    References:
+    '''
+    def __init__(self, pobj=None, climate_required=['sst', 'd18Osw']):
+        self.pobj = pobj
+        self.climate_required = climate_required
+
+    def forward(self, seed=2333, species='all_sea'):
+        vn1 = f'model.{self.climate_required[0]}'
+        vn2 = f'model.{self.climate_required[1]}'
+        res = pb.d18Oc_forward(sst=self.pobj.clim[vn1].da.values, d18Osw=self.pobj.clim[vn2].da.values, seed=seed, species=species)
+        pct = np.percentile(res, q=[5, 50, 95], axis=1)
+
+        pp = ProxyRecord(
+            pid=self.pobj.pid,
+            time=self.pobj.clim[vn1].da.time,
+            value=pct[1],  # median
+            lat=self.pobj.lat,
+            lon=self.pobj.lon,
+            ptype=self.pobj.ptype,
+            value_name=self.pobj.value_name,
+            value_unit=self.pobj.value_unit,
+            time_name=self.pobj.time_name,
+            time_unit=self.pobj.time_unit,
+        )
+        return pp
+
+class BayMgCa:
+    ''' Baysian PSM for Mg/Ca
+    
+    References:
+    '''
+    def __init__(self, pobj=None, climate_required=['sst', 'sss']):
+        self.pobj = pobj
+        self.climate_required = climate_required
+
+    def forward(self, seed=2333, species='all_sea', clean=1, pH=1, omega=1, sw=2, H=1, age=15):
+        vn1 = f'model.{self.climate_required[0]}'
+        vn2 = f'model.{self.climate_required[0]}'
+        res = pb.MgCa_forward(
+            age=age, sst=self.pobj.clim[vn1].da.values, salinity=self.pobj.clim[vn2].da.values,
+            clean=clean, pH=pH, omega=omega, species=species, sw=sw, H=H, seed=seed,
+        )
+        pct = np.percentile(res, q=[5, 50, 95], axis=1)
+
+        pp = ProxyRecord(
+            pid=self.pobj.pid,
+            time=self.pobj.clim[vn1].da.time,
+            value=pct[1],  # median
+            lat=self.pobj.lat,
+            lon=self.pobj.lon,
+            ptype=self.pobj.ptype,
+            value_name=self.pobj.value_name,
+            value_unit=self.pobj.value_unit,
+            time_name=self.pobj.time_name,
+            time_unit=self.pobj.time_unit,
+        )
         return pp
```

### Comparing `cfr-2024.4.3/cfr/reconjob.py` & `cfr-2024.4.4/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/reconres.py` & `cfr-2024.4.4/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/ts.py` & `cfr-2024.4.4/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/utils.py` & `cfr-2024.4.4/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-2024.4.3/cfr/visual.py` & `cfr-2024.4.4/cfr/visual.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         'ocean.temp': sns.xkcd_rgb['blue'],
         'tas': sns.xkcd_rgb['pale red'],
         'pr': sns.xkcd_rgb['aqua'],
         'speleothem.d18O': sns.xkcd_rgb['light brown'],
         'speleothem.dD': sns.xkcd_rgb['brown'],
         'bivalve.d18O': sns.xkcd_rgb['gold'],
         'marine.TEX86': sns.xkcd_rgb['brown'],
+        'marine.UK37': sns.xkcd_rgb['brown'],
         'marine.MgCa': sns.xkcd_rgb['brown'],
         'marine.d18O': sns.xkcd_rgb['brown'],
         'marine.MAT': sns.xkcd_rgb['brown'],
         'marine.alkenone': sns.xkcd_rgb['brown'],
         'marine.foram': sns.xkcd_rgb['brown'],
         'marine.diatom': sns.xkcd_rgb['brown'],
         'marine.dinocyst': sns.xkcd_rgb['brown'],
@@ -127,15 +128,16 @@
         'land.temp': 'o',
         'ocean.temp': 'v',
         'tas': '^',
         'pr': 'o',
         'speleothem.d18O': 'o',
         'speleothem.dD': '>',
         'bivalve.d18O': 'o',
-        'marine.TEX86': '*',
+        'marine.TEX86': 's',
+        'marine.UK37': 'P',
         'marine.MgCa': 'v',
         'marine.d18O': 'o',
         'marine.MAT': 'H',
         'marine.alkenone': 'h',
         'marine.foram': '8',
         'marine.diatom': '^',
         'marine.dinocyst': '>',
@@ -263,15 +265,16 @@
                    site_lats=None, site_lons=None, site_marker='o',
                    site_markersize=50, site_color=sns.xkcd_rgb['amber'],
                    projection='Robinson', transform=ccrs.PlateCarree(),
                    proj_args=None, latlon_range=None, central_longitude=180,
                    lon_ticks=[0, 60, 120, 180, 240, 300], lat_ticks=[-90, 45, 0, 45, 90],
                    land_color=sns.xkcd_rgb['light grey'], ocean_color=sns.xkcd_rgb['light grey'],
                    land_zorder=None, ocean_zorder=None, signif_values=None, signif_range=[0.05, 9999], hatch='..',
-                   clim=None, cmap=None, cmap_under=None, cmap_over=None, cmap_bad=None, extend='both', mode=None, add_gridlines=False,
+                   clim=None, cmap=None, cmap_under=None, cmap_over=None, cmap_bad=None, extend='both', mode=None,
+                   add_gridlines=False, add_coastlines=True,
                    plot_cbar=True, cbar_labels=None, cbar_pad=0.05, cbar_orientation='vertical', cbar_aspect=10,
                    cbar_fraction=0.15, cbar_shrink=0.5, cbar_title=None, cbar_title_x=0.5, cbar_title_y=1.05,
                    fig=None, ax=None):
     ''' Visualize a field on a map.
 
     Args:
         field_var (numpy.ndarray): field data array
@@ -403,15 +406,16 @@
             ax.set_xticks(lon_ticks[mask_lon], crs=ccrs.PlateCarree())
             ax.set_yticks(lat_ticks[mask_lat], crs=ccrs.PlateCarree())
     else:
         ax.set_global()
 
     ax.add_feature(cfeature.LAND, facecolor=land_color, edgecolor=land_color, zorder=land_zorder)
     ax.add_feature(cfeature.OCEAN, facecolor=ocean_color, edgecolor=ocean_color, zorder=ocean_zorder)
-    ax.coastlines(zorder=99)
+    if add_coastlines:
+        ax.coastlines(zorder=99)
 
     if add_gridlines:
         ax.gridlines(edgecolor='gray', linestyle=':', crs=transform)
 
     if cmap is not None:
         cmap = plt.get_cmap(cmap)
     if cmap_under is not None:
@@ -503,15 +507,15 @@
 
 def plot_proxies(df, year=np.arange(2001), lon_col='lon', lat_col='lat', type_col='type', time_col='time',
                  title=None, title_weight='normal', markers_dict=None, colors_dict=None,
                  plot_timespan=None,  plot_xticks=[850, 1000, 1200, 1400, 1600, 1800, 2000],
                  figsize=[10, 10], projection='Robinson', proj_args=None, central_longitude=180, markersize=50,
                  plot_count=False, nrow=2, ncol=1, wspace=0.5, hspace=0.3, return_gs=False,
                  lgd_ncol=None, lgd_anchor_upper=(1, 0), lgd_anchor_lower=(1, -0.05),lgd_frameon=False,
-                 enumerate_ax=False, enumerate_prop={'weight': 'bold', 'size': 30}, p=STYLE, stock_img=True,
+                 enumerate_ax=False, enumerate_prop={'weight': 'bold', 'size': 30}, p=STYLE, stock_img=True, modern_topo=True,
                  enumerate_anchor_map=[0, 1], enumerate_anchor_count=[0, 1], map_grid_idx=0, count_grid_idx=1):
     ''' Visualize proxies.
 
     Args:
         df (pandas.DataFrame): proxy database in `pandas.DataFrame`.
         year (list): the years for counting proxy numbers.
         p (object): the style object that contains dictionaries of markers and colors
@@ -537,15 +541,16 @@
     if stock_img:
         ax['map'].stock_img()
 
     if title:
         ax['map'].set_title(title, fontweight=title_weight)
 
     ax['map'].set_global()
-    ax['map'].add_feature(cfeature.LAND, facecolor='gray', alpha=0.3)
+    if modern_topo:
+        ax['map'].add_feature(cfeature.LAND, facecolor='gray', alpha=0.3)
 
     # plot markers by archive types
     if markers_dict is None:
         markers_dict = p.markers_dict
     if colors_dict is None:
         colors_dict = p.colors_dict
```

### Comparing `cfr-2024.4.3/cfr.egg-info/PKG-INFO` & `cfr-2024.4.4/cfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2024.4.3/setup.py` & `cfr-2024.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2024.4.3',
+    version='2024.4.4',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

