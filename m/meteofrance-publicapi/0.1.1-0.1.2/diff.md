# Comparing `tmp/meteofrance-publicapi-0.1.1.tar.gz` & `tmp/meteofrance-publicapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteofrance-publicapi-0.1.1.tar", last modified: Thu Apr  4 10:02:44 2024, max compression
+gzip compressed data, was "meteofrance-publicapi-0.1.2.tar", last modified: Fri Apr  5 14:35:34 2024, max compression
```

## Comparing `meteofrance-publicapi-0.1.1.tar` & `meteofrance-publicapi-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:02:44.839872 meteofrance-publicapi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44843 2024-04-04 10:02:44.839872 meteofrance-publicapi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:02:44.839872 meteofrance-publicapi-0.1.1/meteofrance_publicapi/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/arome.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:02:44.839872 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44843 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 10:02:44.000000 meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-04 10:02:37.000000 meteofrance-publicapi-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:02:44.839872 meteofrance-publicapi-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/meteofrance_publicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/arome.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/meteofrance_publicapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/tests/__inti__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-05 14:35:34.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 14:35:34.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:35:34.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:35:33.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 14:35:34.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 14:35:34.000000 meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-05 14:35:26.000000 meteofrance-publicapi-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:35:34.199699 meteofrance-publicapi-0.1.2/setup.cfg
```

### Comparing `meteofrance-publicapi-0.1.1/LICENSE` & `meteofrance-publicapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.1/PKG-INFO` & `meteofrance-publicapi-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteofrance-publicapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper of the portail-api.meteofrance.fr datasets
 Author: Antoine Tavant
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,69 +676,95 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/antoinetavant/meteofranceapi
 Project-URL: Bug Tracker, https://github.com/antoinetavant/meteofranceapi/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: deprecation
 Requires-Dist: requests
+Requires-Dist: xmltodict
+Requires-Dist: rasterio
+Requires-Dist: cartopy
+Requires-Dist: matplotlib
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
 Requires-Dist: sphinx_design; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: python-dotenv; extra == "test"
 Provides-Extra: all
-Requires-Dist: meteofranceapi[doc,test]; extra == "all"
+Requires-Dist: meteofrance_publicapi[doc,test]; extra == "all"
+
+# MeteoFrance_PublicAPI: A Python Wrapper for the MétéoFrance API !
+
+![Supported Python versions](https://img.shields.io/pypi/pyversions/meteofrance-publicapi.svg?color=%2334D058) ![License](https://img.shields.io/pypi/l/meteofrance-publicapi
+) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/antoinetavant/meteofranceapi/python-test.yml)
 
-# meteofranceapi
 
 python wrapper of the portail-api.meteofrance.fr datasets
 
+It especially allows to manage easily the API key.
+
+**Documentation**:  [antoinetavant.github.io/meteofranceapi](https://antoinetavant.github.io/meteofranceapi/) (WIP)
+
+**Source Code**: [github.com/antoinetavant/meteofranceapi](https://github.com/antoinetavant/meteofranceapi)
+
 ## Disclaimer
 
-The tool is not officialy provided by MétéoFrance.
+The tool is not officially provided by MétéoFrance.
 
-It is build by trials-and-errors.
+It is build by trials-and-errors and revers-engineering by an amateur.
 
-Most of the functionalities should work, but it may not be the best way to achieve  it.
+Most of the functionalities should work, but it may not be the best way to achieve it.
 
 # Installation
 
-Using `pip``
+Using `pip`
 ```
 pip install meteofrance-publicapi
 ```
 
 # Usage
+To use the ressources, you need an account at MeteoFrance. It is free (as in free-beer).
 
-## Register an account and get the API key
-You need an account on https://portail-api.meteofrance.fr/
+## How to get the API key
+First register on [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 
 Once your account is activated, several options are possible to use `meteofrance-publicapi` :
 - an API key for the API requested
 - a token for the API requested (limited to max 1 hour)
 - an Application ID to the classes which will manage the API token.
 
-The Application ID is the recommended use.
+The Application ID is the recommended use, as it allows to requests dynamically new tokens.
+
+However, you need to keep it a secret !
 
 ### Obtaining the Application ID
 
-From the website https://portail-api.meteofrance.fr/
+From the website  [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 - click on the _Bonjour User Name_ button (upper right corner)
 - click _Mes API_
 - click "Générer Token" for _any API_
 - scroll down to the `curl` field
 - The Application Key is the last field of the curl commend :
     `curl -k -X POST [... ... ...] "Authorization: Basic <YourAPPLICATION_ID>`
 
@@ -764,13 +790,15 @@
 | ...        | ...      | ...       | ...                     | ...        | ...        | ...            | ...        | ...    |
 | 2098       | 98832004 | 91588     | MTGNE SOURCES           | -22.143833 | 166.593167 | 773            | 1989-08-01 | ETENDU |
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
+### Accessing Arome Forecasts
 
+See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.1/README.md` & `meteofrance-publicapi-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,54 @@
-# meteofranceapi
+# MeteoFrance_PublicAPI: A Python Wrapper for the MétéoFrance API !
+
+![Supported Python versions](https://img.shields.io/pypi/pyversions/meteofrance-publicapi.svg?color=%2334D058) ![License](https://img.shields.io/pypi/l/meteofrance-publicapi
+) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/antoinetavant/meteofranceapi/python-test.yml)
+
 
 python wrapper of the portail-api.meteofrance.fr datasets
 
+It especially allows to manage easily the API key.
+
+**Documentation**:  [antoinetavant.github.io/meteofranceapi](https://antoinetavant.github.io/meteofranceapi/) (WIP)
+
+**Source Code**: [github.com/antoinetavant/meteofranceapi](https://github.com/antoinetavant/meteofranceapi)
+
 ## Disclaimer
 
-The tool is not officialy provided by MétéoFrance.
+The tool is not officially provided by MétéoFrance.
 
-It is build by trials-and-errors.
+It is build by trials-and-errors and revers-engineering by an amateur.
 
-Most of the functionalities should work, but it may not be the best way to achieve  it.
+Most of the functionalities should work, but it may not be the best way to achieve it.
 
 # Installation
 
-Using `pip``
+Using `pip`
 ```
 pip install meteofrance-publicapi
 ```
 
 # Usage
+To use the ressources, you need an account at MeteoFrance. It is free (as in free-beer).
 
-## Register an account and get the API key
-You need an account on https://portail-api.meteofrance.fr/
+## How to get the API key
+First register on [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 
 Once your account is activated, several options are possible to use `meteofrance-publicapi` :
 - an API key for the API requested
 - a token for the API requested (limited to max 1 hour)
 - an Application ID to the classes which will manage the API token.
 
-The Application ID is the recommended use.
+The Application ID is the recommended use, as it allows to requests dynamically new tokens.
+
+However, you need to keep it a secret !
 
 ### Obtaining the Application ID
 
-From the website https://portail-api.meteofrance.fr/
+From the website  [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 - click on the _Bonjour User Name_ button (upper right corner)
 - click _Mes API_
 - click "Générer Token" for _any API_
 - scroll down to the `curl` field
 - The Application Key is the last field of the curl commend :
     `curl -k -X POST [... ... ...] "Authorization: Basic <YourAPPLICATION_ID>`
 
@@ -61,13 +74,15 @@
 | ...        | ...      | ...       | ...                     | ...        | ...        | ...            | ...        | ...    |
 | 2098       | 98832004 | 91588     | MTGNE SOURCES           | -22.143833 | 166.593167 | 773            | 1989-08-01 | ETENDU |
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
+### Accessing Arome Forecasts
 
+See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.1/meteofrance_publicapi/core.py` & `meteofrance-publicapi-0.1.2/meteofrance_publicapi/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Core module for the meteofranceapi package."""
 from pathlib import Path
 import time
 import requests
 import logging
 from .const import EXPIRED_TOKEN_CODE, SUCCESS_CODE, PARAMETER_ERROR_CODE, MISSING_DATA_CODE
-from .errors import MissingParameterError
+from .errors import MissingParameterError, MissingDataError
 logger = logging.getLogger(__name__)
 
 class MeteoFranceAPI:
     def __init__(self,
                  api_key: str | None = None,
                  token: str | None = None,
                  application_id: str | None = None,
@@ -71,14 +71,15 @@
         self.token = res.json()["access_token"]
         # save token to file
         local_tmp_cache.mkdir(parents=True, exist_ok=True)
         with open(cache_filename, "w") as f:
             f.write(self.token)
         with open(cache_time_filename, "w") as f:
             f.write(str(time.time()))
+        return self.token
 
 
     def _get_request(self, url, params=None):
         """Make a get request to the API.
 
         Parameters
         ----------
@@ -99,18 +100,21 @@
             self.get_token()
             self.connect()
             res = self.session.get(url, params=params)
         if self._token_expired(res):
             raise ValueError("token expired but could not get a new one")
         error_code = res.status_code
         if error_code == SUCCESS_CODE:
-            logging.debug("request successful")
+            logger.debug("request successful")
         if error_code == PARAMETER_ERROR_CODE:
-            logging.error("parameter error")
+            logger.error("parameter error")
             raise MissingParameterError(res.text)
+        if error_code == MISSING_DATA_CODE:
+            logger.error("missing data")
+            raise MissingDataError(res.text)
         return res
 
 
     def _token_expired(self, res):
         """Check if the token is expired.
 
         Returns
```

### Comparing `meteofrance-publicapi-0.1.1/meteofrance_publicapi/observations.py` & `meteofrance-publicapi-0.1.2/meteofrance_publicapi/observations.py`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.1/meteofrance_publicapi/raster.py` & `meteofrance-publicapi-0.1.2/meteofrance_publicapi/raster.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,31 @@
 def plot_tiff_file(filename, data_type="temperature"):
     """Open a tiff file an plot it.
 
     .. note::
         This Function is more an "How-To" rather than a tool to use as is.
 
     """
-    # Open the file:
     data_field, transform = open_tiff_file(filename=filename)
-
     # Display the source image with cartopy using the geotransform from the source dataset
     fig = plt.figure(figsize=(10, 10))
     ax = fig.add_subplot(1, 1, 1, projection=ccrs.PlateCarree())
-
     im = ax.imshow(data_field,
                    cmap='jet',
                    extent=[transform[2],
                            transform[2] + transform[0]*data_field.shape[1],
                            transform[5] + transform[4]*data_field.shape[0],
                            transform[5]])
-
     ax.add_feature(feature.BORDERS.with_scale('10m'), color='black', linewidth=1)
     ax.add_feature(feature.COASTLINE.with_scale('10m'), color='black', linewidth=1)
-
     cbar = plt.colorbar(im, ax=ax, shrink=0.5)
-
-    lyon_coord = [4.8357, 45.7640]
-    paris_coord = [2.3522, 48.8566]
-
-    ax.plot(lyon_coord[0], lyon_coord[1], 'bo', transform=ccrs.PlateCarree())
-    ax.plot(paris_coord[0], paris_coord[1], 'bo', transform=ccrs.PlateCarree())
-
+    date = filename.stem.split("_")[-1]
+    if data_type == "temperature":
+        cbar.set_label("Temperature (°C)")
+        ax.set_title(f"Temperature at 2m above ground \n at {date} ")
+    add_city_location = False
+    if add_city_location:
+        lyon_coord = [4.8357, 45.7640]
+        paris_coord = [2.3522, 48.8566]
+        ax.plot(lyon_coord[0], lyon_coord[1], 'bo', transform=ccrs.PlateCarree())
+        ax.plot(paris_coord[0], paris_coord[1], 'bo', transform=ccrs.PlateCarree())
+    return ax
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/PKG-INFO` & `meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteofrance-publicapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper of the portail-api.meteofrance.fr datasets
 Author: Antoine Tavant
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,69 +676,95 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/antoinetavant/meteofranceapi
 Project-URL: Bug Tracker, https://github.com/antoinetavant/meteofranceapi/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: deprecation
 Requires-Dist: requests
+Requires-Dist: xmltodict
+Requires-Dist: rasterio
+Requires-Dist: cartopy
+Requires-Dist: matplotlib
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
 Requires-Dist: sphinx_design; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: python-dotenv; extra == "test"
 Provides-Extra: all
-Requires-Dist: meteofranceapi[doc,test]; extra == "all"
+Requires-Dist: meteofrance_publicapi[doc,test]; extra == "all"
+
+# MeteoFrance_PublicAPI: A Python Wrapper for the MétéoFrance API !
+
+![Supported Python versions](https://img.shields.io/pypi/pyversions/meteofrance-publicapi.svg?color=%2334D058) ![License](https://img.shields.io/pypi/l/meteofrance-publicapi
+) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/antoinetavant/meteofranceapi/python-test.yml)
 
-# meteofranceapi
 
 python wrapper of the portail-api.meteofrance.fr datasets
 
+It especially allows to manage easily the API key.
+
+**Documentation**:  [antoinetavant.github.io/meteofranceapi](https://antoinetavant.github.io/meteofranceapi/) (WIP)
+
+**Source Code**: [github.com/antoinetavant/meteofranceapi](https://github.com/antoinetavant/meteofranceapi)
+
 ## Disclaimer
 
-The tool is not officialy provided by MétéoFrance.
+The tool is not officially provided by MétéoFrance.
 
-It is build by trials-and-errors.
+It is build by trials-and-errors and revers-engineering by an amateur.
 
-Most of the functionalities should work, but it may not be the best way to achieve  it.
+Most of the functionalities should work, but it may not be the best way to achieve it.
 
 # Installation
 
-Using `pip``
+Using `pip`
 ```
 pip install meteofrance-publicapi
 ```
 
 # Usage
+To use the ressources, you need an account at MeteoFrance. It is free (as in free-beer).
 
-## Register an account and get the API key
-You need an account on https://portail-api.meteofrance.fr/
+## How to get the API key
+First register on [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 
 Once your account is activated, several options are possible to use `meteofrance-publicapi` :
 - an API key for the API requested
 - a token for the API requested (limited to max 1 hour)
 - an Application ID to the classes which will manage the API token.
 
-The Application ID is the recommended use.
+The Application ID is the recommended use, as it allows to requests dynamically new tokens.
+
+However, you need to keep it a secret !
 
 ### Obtaining the Application ID
 
-From the website https://portail-api.meteofrance.fr/
+From the website  [portail-api.meteofrance.fr](https://portail-api.meteofrance.fr/)
 - click on the _Bonjour User Name_ button (upper right corner)
 - click _Mes API_
 - click "Générer Token" for _any API_
 - scroll down to the `curl` field
 - The Application Key is the last field of the curl commend :
     `curl -k -X POST [... ... ...] "Authorization: Basic <YourAPPLICATION_ID>`
 
@@ -764,13 +790,15 @@
 | ...        | ...      | ...       | ...                     | ...        | ...        | ...            | ...        | ...    |
 | 2098       | 98832004 | 91588     | MTGNE SOURCES           | -22.143833 | 166.593167 | 773            | 1989-08-01 | ETENDU |
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
+### Accessing Arome Forecasts
 
+See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.1/meteofrance_publicapi.egg-info/SOURCES.txt` & `meteofrance-publicapi-0.1.2/meteofrance_publicapi.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 meteofrance_publicapi/observations.py
 meteofrance_publicapi/raster.py
 meteofrance_publicapi.egg-info/PKG-INFO
 meteofrance_publicapi.egg-info/SOURCES.txt
 meteofrance_publicapi.egg-info/dependency_links.txt
 meteofrance_publicapi.egg-info/not-zip-safe
 meteofrance_publicapi.egg-info/requires.txt
-meteofrance_publicapi.egg-info/top_level.txt
+meteofrance_publicapi.egg-info/top_level.txt
+meteofrance_publicapi/tests/__inti__.py
+meteofrance_publicapi/tests/test_import.py
```

### Comparing `meteofrance-publicapi-0.1.1/pyproject.toml` & `meteofrance-publicapi-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,43 +8,56 @@
 authors = [
   { name="Antoine Tavant"},
 ]
 readme = "README.md"
 license = {file = 'LICENSE'}
 requires-python = ">=3.9"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+    "Development Status :: 2 - Pre-Alpha",
+    "Topic :: Scientific/Engineering :: Atmospheric Science",
 ]
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "deprecation",
     "requests",
+    "xmltodict",
+    "rasterio",
+    "cartopy",
+    "matplotlib",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/antoinetavant/meteofranceapi"
 "Bug Tracker" = "https://github.com/antoinetavant/meteofranceapi/issues"
 
 [project.optional-dependencies]
 doc = [
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx_design",
+    "nbsphinx",
 ]
 test = [
     "pytest",
     "pytest-cov",
     "python-dotenv",
 ]
 all = [
-    "meteofranceapi[test,doc]"
+    "meteofrance_publicapi[test,doc]"
 ]
 
 [tool.setuptools]
 zip-safe = false
 [tool.setuptools.packages.find]
 where = ["./"]
 include = ["meteofrance_publicapi*"]
```

