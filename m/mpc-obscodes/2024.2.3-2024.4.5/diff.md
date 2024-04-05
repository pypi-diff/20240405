# Comparing `tmp/mpc_obscodes-2024.2.3.tar.gz` & `tmp/mpc_obscodes-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2024.2.3.tar", last modified: Sat Feb  3 02:21:47 2024, max compression
+gzip compressed data, was "mpc_obscodes-2024.4.5.tar", last modified: Fri Apr  5 02:22:26 2024, max compression
```

## Comparing `mpc_obscodes-2024.2.3.tar` & `mpc_obscodes-2024.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:21:47.311730 mpc_obscodes-2024.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-03 02:21:47.311730 mpc_obscodes-2024.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:21:47.307729 mpc_obscodes-2024.2.3/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)   250744 2024-02-03 02:21:37.000000 mpc_obscodes-2024.2.3/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-03 02:21:37.000000 mpc_obscodes-2024.2.3/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:21:47.307729 mpc_obscodes-2024.2.3/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-03 02:21:35.000000 mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:21:47.307729 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-03 02:21:47.000000 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-03 02:21:47.000000 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 02:21:47.000000 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-03 02:21:47.000000 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-03 02:21:47.000000 mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-03 02:21:37.000000 mpc_obscodes-2024.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 02:21:47.311730 mpc_obscodes-2024.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.240371 mpc_obscodes-2024.4.5/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253345 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/setup.cfg
```

### Comparing `mpc_obscodes-2024.2.3/PKG-INFO` & `mpc_obscodes-2024.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.2.3
+Version: 2024.4.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.2.3/README.md` & `mpc_obscodes-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/compare.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/fetch.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894461077844311%*

 * *Differences: {"'203'": "{'Longitude': 8.99548, 'cos': 0.701614, 'sin': 0.710215}",*

 * * "'204'": "{'Longitude': 8.76972, 'cos': 0.697648, 'sin': 0.714307}",*

 * * "'703'": "{'cos': 0.845311, 'sin': 0.533211}",*

 * * "'958'": "{'Longitude': 358.96947, 'cos': 0.724214, 'sin': 0.687282}",*

 * * "'A17'": "{'Longitude': 8.68147, 'cos': 0.650133, 'sin': 0.757328}",*

 * * "'C65'": "{'cos': 0.743847, 'sin': 0.666488}",*

 * * "'C82'": "{'Longitude': 14.35759, 'cos': 0.760172, 'sin': 0.647614}",*

 * * "'C95'": "{'cos': 0.721406, 'sin': 0.69035}",*

 * * "'D03'": "{'Lon […]*

```diff
@@ -1214,24 +1214,24 @@
     "202": {
         "Longitude": 5.8997,
         "Name": "Tamaris Observatoire, La Seyne sur Mer",
         "cos": 0.73137,
         "sin": 0.67971
     },
     "203": {
-        "Longitude": 8.9955,
+        "Longitude": 8.99548,
         "Name": "GiaGa Observatory",
-        "cos": 0.70161,
-        "sin": 0.71021
+        "cos": 0.701614,
+        "sin": 0.710215
     },
     "204": {
-        "Longitude": 8.7708,
+        "Longitude": 8.76972,
         "Name": "Schiaparelli Observatory",
-        "cos": 0.69765,
-        "sin": 0.7143
+        "cos": 0.697648,
+        "sin": 0.714307
     },
     "205": {
         "Longitude": 11.2731,
         "Name": "Obs. Casalecchio di Reno, Bologna",
         "cos": 0.71478,
         "sin": 0.69703
     },
@@ -4039,16 +4039,16 @@
         "Name": "Joint Obs. for cometary research, Socorro",
         "cos": 0.8305,
         "sin": 0.5561
     },
     "703": {
         "Longitude": 249.26736,
         "Name": "Catalina Sky Survey",
-        "cos": 0.845315,
-        "sin": 0.533213
+        "cos": 0.845311,
+        "sin": 0.533211
     },
     "704": {
         "Longitude": 253.34093,
         "Name": "Lincoln Laboratory ETS, New Mexico",
         "cos": 0.831869,
         "sin": 0.553542
     },
@@ -5567,18 +5567,18 @@
     "957": {
         "Longitude": 359.3506,
         "Name": "Merignac",
         "cos": 0.71047,
         "sin": 0.70137
     },
     "958": {
-        "Longitude": 358.96961,
+        "Longitude": 358.96947,
         "Name": "Observatoire de Dax",
-        "cos": 0.724206,
-        "sin": 0.687273
+        "cos": 0.724214,
+        "sin": 0.687282
     },
     "959": {
         "Longitude": 1.4653,
         "Name": "Ramonville Saint Agne",
         "cos": 0.72596,
         "sin": 0.68548
     },
@@ -5921,18 +5921,18 @@
     "A16": {
         "Longitude": 7.1922,
         "Name": "Tentlingen",
         "cos": 0.68622,
         "sin": 0.72511
     },
     "A17": {
-        "Longitude": 8.68152,
+        "Longitude": 8.68147,
         "Name": "Guidestar Observatory, Weinheim",
-        "cos": 0.650125,
-        "sin": 0.757317
+        "cos": 0.650133,
+        "sin": 0.757328
     },
     "A18": {
         "Longitude": 7.1761,
         "Name": "Herne",
         "cos": 0.62342,
         "sin": 0.77928
     },
@@ -7375,16 +7375,16 @@
         "Name": "Puchenstuben",
         "cos": 0.67138,
         "sin": 0.738819
     },
     "C65": {
         "Longitude": 0.72965,
         "Name": "Observatori Astronomic del Montsec",
-        "cos": 0.743841,
-        "sin": 0.666482
+        "cos": 0.743847,
+        "sin": 0.666488
     },
     "C66": {
         "Longitude": 2.805,
         "Name": "Observatorio El Cielo de Consell",
         "cos": 0.77084,
         "sin": 0.63493
     },
@@ -7475,18 +7475,18 @@
     "C81": {
         "Longitude": 10.84098,
         "Name": "Dolomites Astronomical Observatory",
         "cos": 0.693023,
         "sin": 0.718872
     },
     "C82": {
-        "Longitude": 14.35763,
+        "Longitude": 14.35759,
         "Name": "Osservatorio Astronomico Nastro Verde, Sorrento",
-        "cos": 0.760171,
-        "sin": 0.647611
+        "cos": 0.760172,
+        "sin": 0.647614
     },
     "C83": {
         "Longitude": 91.8425,
         "Name": "Badalozhnyj Observatory",
         "cos": 0.5593,
         "sin": 0.82626
     },
@@ -7555,16 +7555,16 @@
         "Name": "MASTER-II Observatory, Tunka",
         "cos": 0.61962,
         "sin": 0.78241
     },
     "C95": {
         "Longitude": 5.71239,
         "Name": "SATINO Remote Observatory, Haute Provence",
-        "cos": 0.721401,
-        "sin": 0.690345
+        "cos": 0.721406,
+        "sin": 0.69035
     },
     "C96": {
         "Longitude": 13.8786,
         "Name": "OACL Observatory, Mosciano Sant Angelo",
         "cos": 0.73544,
         "sin": 0.67537
     },
@@ -7601,18 +7601,18 @@
     "D02": {
         "Longitude": 2.05189,
         "Name": "Observatori Petit Sant Feliu",
         "cos": 0.751414,
         "sin": 0.657647
     },
     "D03": {
-        "Longitude": 10.5889,
+        "Longitude": 10.58892,
         "Name": "Rantiga Osservatorio, Tincana",
-        "cos": 0.71522,
-        "sin": 0.6967
+        "cos": 0.715223,
+        "sin": 0.696709
     },
     "D04": {
         "Longitude": 38.8569,
         "Name": "Krasnodar",
         "cos": 0.7096,
         "sin": 0.70225
     },
@@ -7762,14 +7762,26 @@
     },
     "D29": {
         "Longitude": 118.4639,
         "Name": "Purple Mountain Observatory, XuYi Station",
         "cos": 0.84204,
         "sin": 0.53767
     },
+    "D30": {
+        "Longitude": 11.0835,
+        "Name": "Sternwarte Silbergraben, Erfurt",
+        "cos": 0.631405,
+        "sin": 0.772922
+    },
+    "D31": {
+        "Longitude": 10.09797,
+        "Name": "Osservatorio Aldebaran, Rivalba",
+        "cos": 0.714476,
+        "sin": 0.69752
+    },
     "D32": {
         "Longitude": 119.59975,
         "Name": "JiangNanTianChi Observatory, Mt. Getianling",
         "cos": 0.86277,
         "sin": 0.504193
     },
     "D33": {
@@ -7810,20 +7822,56 @@
     },
     "D39": {
         "Longitude": 122.04961,
         "Name": "Shandong University Observatory, Weihai",
         "cos": 0.793971,
         "sin": 0.605943
     },
+    "D40": {
+        "Longitude": 13.33772,
+        "Name": "Frosinone",
+        "cos": 0.748318,
+        "sin": 0.661176
+    },
+    "D41": {
+        "Longitude": 10.71704,
+        "Name": "Osservatorio Astronomico Orciatico",
+        "cos": 0.727431,
+        "sin": 0.683991
+    },
+    "D42": {
+        "Longitude": 11.19084,
+        "Name": "Piero Angela Observatory, Scandicci",
+        "cos": 0.723565,
+        "sin": 0.68797
+    },
+    "D43": {
+        "Longitude": 7.7706,
+        "Name": "45th Parallel Obs., Pino Torinese",
+        "cos": 0.70781,
+        "sin": 0.70416
+    },
     "D44": {
         "Longitude": 124.13928,
         "Name": "Ishigakijima Astronomical Observatory",
         "cos": 0.911427,
         "sin": 0.410157
     },
+    "D45": {
+        "Longitude": 21.49325,
+        "Name": "Kamyk, Trzesn",
+        "cos": 0.639594,
+        "sin": 0.766177
+    },
+    "D46": {
+        "Longitude": 9.90265,
+        "Name": "Observatory Bad Wurzach",
+        "cos": 0.671664,
+        "sin": 0.738525
+    },
     "D53": {
         "Longitude": 127.482,
         "Name": "ISON-Blagoveschensk Observatory",
         "cos": 0.63981,
         "sin": 0.766
     },
     "D54": {
@@ -7858,14 +7906,20 @@
     },
     "D62": {
         "Longitude": 130.4494,
         "Name": "Miyaki-Argenteus",
         "cos": 0.83676,
         "sin": 0.54575
     },
+    "D63": {
+        "Longitude": 10.46138,
+        "Name": "G. Pascoli Observatory, Barga (since June 2023)",
+        "cos": 0.719553,
+        "sin": 0.692176
+    },
     "D67": {
         "Longitude": 37.62472,
         "Name": "Tula Rooftop Observatory, Tula",
         "cos": 0.586136,
         "sin": 0.80753
     },
     "D70": {
@@ -9641,18 +9695,18 @@
     "I32": {
         "Longitude": 299.3464,
         "Name": "Observatorio Beta Orionis, Rosario",
         "cos": 0.83969,
         "sin": -0.54125
     },
     "I33": {
-        "Longitude": 289.2608,
+        "Longitude": 289.26631,
         "Name": "SOAR, Cerro Pachon",
-        "cos": 0.86504,
-        "sin": -0.50086
+        "cos": 0.865052,
+        "sin": -0.500865
     },
     "I34": {
         "Longitude": 284.1297,
         "Name": "Morgantown",
         "cos": 0.76548,
         "sin": 0.64134
     },
@@ -10001,18 +10055,18 @@
     "I92": {
         "Longitude": 353.95289,
         "Name": "Astreo Observatory, Mairena del Aljarafe",
         "cos": 0.795987,
         "sin": 0.603315
     },
     "I93": {
-        "Longitude": 359.797,
+        "Longitude": 359.79704,
         "Name": "St Pardon de Conques",
-        "cos": 0.713711,
-        "sin": 0.698096
+        "cos": 0.713717,
+        "sin": 0.698101
     },
     "I94": {
         "Longitude": 356.1367,
         "Name": "Observatorio Rho Ophiocus, Las Rozas de Madrid",
         "cos": 0.76162,
         "sin": 0.64603
     },
@@ -11021,18 +11075,18 @@
     "K62": {
         "Longitude": 13.84675,
         "Name": "Teplice Observatory",
         "cos": 0.635514,
         "sin": 0.769557
     },
     "K63": {
-        "Longitude": 10.462,
-        "Name": "G. Pascoli Observatory, Castelvecchio Pascoli",
-        "cos": 0.71953,
-        "sin": 0.69218
+        "Longitude": 10.46252,
+        "Name": "G. Pascoli Observatory, Barga (before June 2023)",
+        "cos": 0.719536,
+        "sin": 0.692195
     },
     "K64": {
         "Longitude": 11.74397,
         "Name": "Waizenreuth",
         "cos": 0.644963,
         "sin": 0.761748
     },
@@ -11569,16 +11623,16 @@
         "Name": "Lomazzo Observatory, Como",
         "cos": 0.699589,
         "sin": 0.712226
     },
     "L54": {
         "Longitude": 22.88878,
         "Name": "Berthelot Observatory, Hunedoara",
-        "cos": 0.700705,
-        "sin": 0.711157
+        "cos": 0.700704,
+        "sin": 0.711156
     },
     "L55": {
         "Longitude": 35.0875,
         "Name": "Sura Gardens, Dnipro",
         "cos": 0.666222,
         "sin": 0.743283
     },
@@ -12208,14 +12262,20 @@
     },
     "M63": {
         "Longitude": 18.36969,
         "Name": "RPF Observatory, Gagliano del Capo",
         "cos": 0.768886,
         "sin": 0.637286
     },
+    "M64": {
+        "Longitude": 0.23964,
+        "Name": "Holbrook, Heathfield",
+        "cos": 0.631065,
+        "sin": 0.77317
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
@@ -12262,14 +12322,20 @@
     },
     "N51": {
         "Longitude": 78.96461,
         "Name": "GROWTH India Telescope, IAO, Hanle",
         "cos": 0.842178,
         "sin": 0.538687
     },
+    "N54": {
+        "Longitude": 80.02674,
+        "Name": "Purple Mountain Observatory, Jiama'erdeng",
+        "cos": 0.846505,
+        "sin": 0.532071
+    },
     "N55": {
         "Longitude": 80.02623,
         "Name": "Corona Borealis Observatory, Ngari, Tibet",
         "cos": 0.846497,
         "sin": 0.532089
     },
     "N56": {
@@ -12340,14 +12406,32 @@
     },
     "O37": {
         "Longitude": 98.48553,
         "Name": "TRT-NEO, Chiangmai",
         "cos": 0.948521,
         "sin": 0.316891
     },
+    "O40": {
+        "Longitude": 100.22861,
+        "Name": "Xingyuan, Daocheng",
+        "cos": 0.875727,
+        "sin": 0.482435
+    },
+    "O41": {
+        "Longitude": 99.46556,
+        "Name": "Choakanan Observatory, Lampang",
+        "cos": 0.949569,
+        "sin": 0.312613
+    },
+    "O42": {
+        "Longitude": 100.029,
+        "Name": "Gaomeigu Gemini Observatory, LiJiang",
+        "cos": 0.894239,
+        "sin": 0.447183
+    },
     "O43": {
         "Longitude": 99.78111,
         "Name": "Observatori Negara, Langkawi",
         "cos": 0.994005,
         "sin": 0.109127
     },
     "O44": {
@@ -12400,14 +12484,26 @@
     },
     "O52": {
         "Longitude": 100.72972,
         "Name": "Astro820, Samut Prakan",
         "cos": 0.972224,
         "sin": 0.23325
     },
+    "O53": {
+        "Longitude": 101.40403,
+        "Name": "Pakchong, Nachonratchasima",
+        "cos": 0.967655,
+        "sin": 0.25161
+    },
+    "O54": {
+        "Longitude": 100.94939,
+        "Name": "TSky Observatory, Chonburi",
+        "cos": 0.97337,
+        "sin": 0.22846
+    },
     "O68": {
         "Longitude": 105.3309,
         "Name": "LW-2, NAOC-Zhongwei",
         "cos": 0.793121,
         "sin": 0.607347
     },
     "O72": {
@@ -12430,14 +12526,26 @@
     },
     "P07": {
         "Longitude": 114.08987,
         "Name": "Space Surveillance Telescope, HEH Station",
         "cos": 0.928304,
         "sin": -0.370597
     },
+    "P13": {
+        "Longitude": 115.57333,
+        "Name": "Baihuashan Observatory, Beijing",
+        "cos": 0.769058,
+        "sin": 0.637315
+    },
+    "P14": {
+        "Longitude": 115.81167,
+        "Name": "Nedlands Observatory, Perth",
+        "cos": 0.848989,
+        "sin": -0.526638
+    },
     "P18": {
         "Longitude": 116.61083,
         "Name": "Birch Forest Observatory, LaBaGouMen",
         "cos": 0.75701,
         "sin": 0.651328
     },
     "P21": {
@@ -12604,14 +12712,20 @@
     },
     "Q19": {
         "Longitude": 139.439,
         "Name": "Machida",
         "cos": 0.8143,
         "sin": 0.57852
     },
+    "Q20": {
+        "Longitude": 139.57008,
+        "Name": "Swan Reach Imaging, Glenalta",
+        "cos": 0.824585,
+        "sin": -0.563856
+    },
     "Q21": {
         "Longitude": 139.85335,
         "Name": "Southern Utsunomiya",
         "cos": 0.804747,
         "sin": 0.591654
     },
     "Q23": {
@@ -13301,18 +13415,18 @@
     "V38": {
         "Longitude": 255.98493,
         "Name": "McDonald Observatory-LCO ELP Aqawan A #1",
         "cos": 0.861051,
         "sin": 0.507431
     },
     "V39": {
-        "Longitude": 255.98452,
+        "Longitude": 255.98483,
         "Name": "McDonald Observatory-LCO ELP B",
-        "cos": 0.861051,
-        "sin": 0.50743
+        "cos": 0.861053,
+        "sin": 0.507427
     },
     "V40": {
         "Longitude": 255.91873,
         "Name": "Divine Creation Observatory, Fort Davis",
         "cos": 0.861839,
         "sin": 0.506046
     },
@@ -14002,14 +14116,20 @@
     },
     "X16": {
         "Longitude": 293.8497,
         "Name": "Astronomia Sigma Octante, Cochabamba",
         "cos": 0.95511,
         "sin": -0.29667
     },
+    "X17": {
+        "Longitude": 289.26208,
+        "Name": "BlackGEM",
+        "cos": 0.873456,
+        "sin": -0.486033
+    },
     "X31": {
         "Longitude": 299.47934,
         "Name": "Galileo Galilei Observatory, Oro Verde",
         "cos": 0.850485,
         "sin": -0.524263
     },
     "X33": {
@@ -14164,14 +14284,26 @@
     },
     "Y85": {
         "Longitude": 351.85389,
         "Name": "Magalofes Observatory, Fene",
         "cos": 0.727084,
         "sin": 0.684321
     },
+    "Y86": {
+        "Longitude": 357.48003,
+        "Name": "Observatorio de Seron",
+        "cos": 0.79601,
+        "sin": 0.603469
+    },
+    "Y87": {
+        "Longitude": 353.01194,
+        "Name": "Trevinca Skies-Amalthea, Trevinca",
+        "cos": 0.741821,
+        "sin": 0.668656
+    },
     "Y88": {
         "Longitude": 353.01194,
         "Name": "ASERO, Valdin",
         "cos": 0.741819,
         "sin": 0.668659
     },
     "Y89": {
@@ -14212,14 +14344,26 @@
     },
     "Y95": {
         "Longitude": 357.99864,
         "Name": "Pradillos Ferez",
         "cos": 0.785356,
         "sin": 0.617157
     },
+    "Y96": {
+        "Longitude": 358.08932,
+        "Name": "Observatorio de Vega del Codorno",
+        "cos": 0.762606,
+        "sin": 0.645079
+    },
+    "Y97": {
+        "Longitude": 359.64303,
+        "Name": "Bommes Observatory, Bommes",
+        "cos": 0.713822,
+        "sin": 0.697993
+    },
     "Y98": {
         "Longitude": 358.68692,
         "Name": "Southside Observatory, Steeple Aston",
         "cos": 0.617953,
         "sin": 0.783613
     },
     "Y99": {
```

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.2.3/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.2.3
+Version: 2024.4.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.2.3/pyproject.toml` & `mpc_obscodes-2024.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2024.02.03"
+version = "2024.04.05"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

