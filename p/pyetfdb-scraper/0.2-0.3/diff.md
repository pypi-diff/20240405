# Comparing `tmp/pyetfdb_scraper-0.2.tar.gz` & `tmp/pyetfdb_scraper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetfdb_scraper-0.2.tar", last modified: Fri Feb  9 16:16:32 2024, max compression
+gzip compressed data, was "pyetfdb_scraper-0.3.tar", last modified: Fri Apr  5 10:39:22 2024, max compression
```

## Comparing `pyetfdb_scraper-0.2.tar` & `pyetfdb_scraper-0.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.246143 pyetfdb_scraper-0.2/
--rw-r--r--   0 lohyikuang   (501) staff       (20)    35148 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/LICENSE
--rw-r--r--   0 lohyikuang   (501) staff       (20)       24 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/MANIFEST.in
--rw-r--r--   0 lohyikuang   (501) staff       (20)    21950 2024-02-09 16:16:32.245769 pyetfdb_scraper-0.2/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)    21672 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/README.md
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1040 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/pyproject.toml
--rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2024-02-09 16:16:32.246219 pyetfdb_scraper-0.2/setup.cfg
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1073 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/setup.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.224955 pyetfdb_scraper-0.2/src/
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.232543 pyetfdb_scraper-0.2/src/pyetfdb_scraper/
--rw-r--r--   0 lohyikuang   (501) staff       (20)       20 2024-02-09 16:16:14.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.235496 pyetfdb_scraper-0.2/src/pyetfdb_scraper/data/
--rw-r--r--   0 lohyikuang   (501) staff       (20)   567933 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/data/etfdb.json
--rw-r--r--   0 lohyikuang   (501) staff       (20)     2010 2024-01-29 08:44:31.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/etf.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     3902 2024-01-29 11:49:27.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/etf_scraper.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.239913 pyetfdb_scraper-0.2/src/pyetfdb_scraper/models/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      120 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/models/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      360 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/models/expense.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1792 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/models/info.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.245152 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      473 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      855 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/dividend.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1669 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/expense.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      939 2024-01-29 06:20:26.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/holding_analysis.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     5175 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/holdings.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)    11489 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/info.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1152 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/performance.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      544 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/realtime_ratings.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1408 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/technicals.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     4800 2024-01-29 08:44:30.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper/utils.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-02-09 16:16:32.234932 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/
--rw-r--r--   0 lohyikuang   (501) staff       (20)    21950 2024-02-09 16:16:32.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)      887 2024-02-09 16:16:32.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2024-02-09 16:16:32.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       13 2024-02-09 16:16:32.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/requires.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       16 2024-02-09 16:16:32.000000 pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.756721 pyetfdb_scraper-0.3/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    35148 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/LICENSE
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       49 2024-04-05 10:32:32.000000 pyetfdb_scraper-0.3/MANIFEST.in
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22764 2024-04-05 10:39:22.755588 pyetfdb_scraper-0.3/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22345 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/README.md
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1040 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/pyproject.toml
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2024-04-05 10:39:22.756990 pyetfdb_scraper-0.3/setup.cfg
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1193 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/setup.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.720262 pyetfdb_scraper-0.3/src/
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.726622 pyetfdb_scraper-0.3/src/pyetfdb_scraper/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       19 2024-04-05 10:30:36.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.737279 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)   567933 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/etfdb.json
+-rw-r--r--   0 lohyikuang   (501) staff       (20)   110530 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/user-agents.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     2010 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     3902 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf_scraper.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.740463 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      120 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      360 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/expense.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1792 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/info.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.751258 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      473 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      855 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/dividend.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1669 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/expense.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      939 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holding_analysis.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     5175 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holdings.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    11489 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/info.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1152 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/performance.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      544 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/realtime_ratings.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1408 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/technicals.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     4800 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/utils.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.752701 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22764 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      928 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       37 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/requires.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       16 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/top_level.txt
```

### Comparing `pyetfdb_scraper-0.2/LICENSE` & `pyetfdb_scraper-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/PKG-INFO` & `pyetfdb_scraper-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 Metadata-Version: 2.1
 Name: pyetfdb_scraper
-Version: 0.2
+Version: 0.3
 Summary: Scrape ETFs from ETFDB
 Home-page: https://github.com/lvxhnat/pyetf-scraper
 Author: Yi Kuang
 Author-email: yikuang5@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: bs4
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
-# pyetfdb_scraper
+# pyetfdb_scraper: Free ETF data at your fingertips
 ```pyetfdb_scraper``` is a Python library for extracting ETF data directly from [ETFDB](https://etfdb.com/), a website providing one of the largest ETF Databases containing ETFs from a vast range of asset classes, industries, issuers, and investment styles.
 
-## Quick Start 
+## Quick Start
 Install with ```pip``` as a package pip. See the pip package here https://pypi.org/project/pyetfdb-scraper/.
 
 ```
 pip install pyetfdb-scraper
 ```
 
 ```python
 from pyetfdb_scraper import etf
 ```
 
 ## Example Usage
 
 ```python
-from pyetfdb_scraper.etf import ETF,load_etfs 
+from pyetfdb_scraper.etf import ETF,load_etfs
 # returns list of available ETFs.
 etfs = load_etfs()
-# load etf
+```
+```
+>>> ['SPY', 'IVV', 'VTI', 'VOO', 'QQQ', 'VEA', 'IEFA', ...]
+```
+### Retrieve info about a single ticker
+``` python
+# Load ETF
 ivv = ETF('IVV')
-# Get basic ETF information
+```
+
+```python
 print(ivv.info)
+```
+
+<details>
+<summary>  Results </summary>
 
+```
 >>> {
     "vitals": {
         "etf_name": "iShares Core S&P 500 ETF",
         "issuer": "BlackRock, Inc.",
         "issuer_link": "/issuer/blackrock-inc/",
         "brand": "iShares",
         "brand_link": "/issuer/ishares/",
@@ -152,16 +170,27 @@
             "assets": "$16.0 M",
             "avg_daily_volume": "4,800",
             "ytd_return": "7.15%",
         },
     ],
 }
 
+```
+</details>
+
+
+<br/>
+
+```python
 print(ivv.to_dict())
+```
+<details>
+<summary>Results</summary>
 
+```
 >>> {
     "info": {
         "vitals": {
             "issuer": "BlackRock, Inc.",
             "issuer_link": "/issuer/blackrock-inc/",
             "brand": "iShares",
             "brand_link": "/issuer/ishares/",
@@ -617,22 +646,26 @@
         {
             "metric": "Concentration",
             "metric_realtime_rating": "A-",
             "a+_metric_rated_etf": "VT",
         },
     ],
 }
-
 ```
+</details>
+
 ## Help Needed!
-I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as: 
+I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as:
 * Unit tests for the current code
 * ETF Category has yet to be updated
 
-## Disclaimer 
-This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package creted by Jakub Pluta, which has since not been actively maintained.
-
 ## Contributing
-Pull requests are welcome.
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
+
+If you are simply looking to start working with the codebase, navigate to the GitHub "issues" tab and start looking through interesting issues. You can also triage issues which may include reproducing bug reports, or asking for vital information such as version numbers or reproduction instructions. To read more about contributing, you can refer to [CONTRIBUTING](./CONTRIBUTING.md)
 
 ## License
-MIT License
+GPLv3
+
+## Disclaimer
+This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package.
```

### Comparing `pyetfdb_scraper-0.2/README.md` & `pyetfdb_scraper-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-# pyetfdb_scraper
+# pyetfdb_scraper: Free ETF data at your fingertips
 ```pyetfdb_scraper``` is a Python library for extracting ETF data directly from [ETFDB](https://etfdb.com/), a website providing one of the largest ETF Databases containing ETFs from a vast range of asset classes, industries, issuers, and investment styles.
 
-## Quick Start 
+## Quick Start
 Install with ```pip``` as a package pip. See the pip package here https://pypi.org/project/pyetfdb-scraper/.
 
 ```
 pip install pyetfdb-scraper
 ```
 
 ```python
 from pyetfdb_scraper import etf
 ```
 
 ## Example Usage
 
 ```python
-from pyetfdb_scraper.etf import ETF,load_etfs 
+from pyetfdb_scraper.etf import ETF,load_etfs
 # returns list of available ETFs.
 etfs = load_etfs()
-# load etf
+```
+```
+>>> ['SPY', 'IVV', 'VTI', 'VOO', 'QQQ', 'VEA', 'IEFA', ...]
+```
+### Retrieve info about a single ticker
+``` python
+# Load ETF
 ivv = ETF('IVV')
-# Get basic ETF information
+```
+
+```python
 print(ivv.info)
+```
+
+<details>
+<summary>  Results </summary>
 
+```
 >>> {
     "vitals": {
         "etf_name": "iShares Core S&P 500 ETF",
         "issuer": "BlackRock, Inc.",
         "issuer_link": "/issuer/blackrock-inc/",
         "brand": "iShares",
         "brand_link": "/issuer/ishares/",
@@ -141,16 +154,27 @@
             "assets": "$16.0 M",
             "avg_daily_volume": "4,800",
             "ytd_return": "7.15%",
         },
     ],
 }
 
+```
+</details>
+
+
+<br/>
+
+```python
 print(ivv.to_dict())
+```
+<details>
+<summary>Results</summary>
 
+```
 >>> {
     "info": {
         "vitals": {
             "issuer": "BlackRock, Inc.",
             "issuer_link": "/issuer/blackrock-inc/",
             "brand": "iShares",
             "brand_link": "/issuer/ishares/",
@@ -606,22 +630,26 @@
         {
             "metric": "Concentration",
             "metric_realtime_rating": "A-",
             "a+_metric_rated_etf": "VT",
         },
     ],
 }
-
 ```
+</details>
+
 ## Help Needed!
-I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as: 
+I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as:
 * Unit tests for the current code
 * ETF Category has yet to be updated
 
-## Disclaimer 
-This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package creted by Jakub Pluta, which has since not been actively maintained.
-
 ## Contributing
-Pull requests are welcome.
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
+
+If you are simply looking to start working with the codebase, navigate to the GitHub "issues" tab and start looking through interesting issues. You can also triage issues which may include reproducing bug reports, or asking for vital information such as version numbers or reproduction instructions. To read more about contributing, you can refer to [CONTRIBUTING](./CONTRIBUTING.md)
 
 ## License
-MIT License
+GPLv3
+
+## Disclaimer
+This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package.
```

### Comparing `pyetfdb_scraper-0.2/pyproject.toml` & `pyetfdb_scraper-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/setup.py` & `pyetfdb_scraper-0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,25 +16,28 @@
     result = re.search(r'__version__ = ["\']([^"\']+)', f.read())
 
     if not result:
         raise ValueError(f"Can't find the version in {name}/__init__.py")
 
     version = result.group(1)
 
+dev_requirements = {"black", "pre-commit"}
+
 setup(
     name=name,
     version=version,
     author="Yi Kuang",
     author_email="yikuang5@gmail.com",
     description="Scrape ETFs from ETFDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lvxhnat/pyetf-scraper",
     package_dir={"": "src"},
     packages=find_packages("src", exclude=["*tests"]),
-    package_data={name: ["data/etfdb.json"]},
+    package_data={name: ["data/etfdb.json", "data/user-agents.txt"]},
     python_requires=">=3.7",
     install_requires=[
         "requests",
         "bs4",
     ],
+    extras_require={"dev": list(dev_requirements)},
 )
```

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/data/etfdb.json` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/etfdb.json`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/etf.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/etf_scraper.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf_scraper.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/models/info.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/info.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/dividend.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/dividend.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/expense.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/expense.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/holding_analysis.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holding_analysis.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/holdings.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holdings.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/info.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/info.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/performance.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/performance.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/realtime_ratings.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/realtime_ratings.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/tabs/technicals.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/technicals.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper/utils.py` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/PKG-INFO` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 Metadata-Version: 2.1
-Name: pyetfdb-scraper
-Version: 0.2
+Name: pyetfdb_scraper
+Version: 0.3
 Summary: Scrape ETFs from ETFDB
 Home-page: https://github.com/lvxhnat/pyetf-scraper
 Author: Yi Kuang
 Author-email: yikuang5@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: bs4
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
-# pyetfdb_scraper
+# pyetfdb_scraper: Free ETF data at your fingertips
 ```pyetfdb_scraper``` is a Python library for extracting ETF data directly from [ETFDB](https://etfdb.com/), a website providing one of the largest ETF Databases containing ETFs from a vast range of asset classes, industries, issuers, and investment styles.
 
-## Quick Start 
+## Quick Start
 Install with ```pip``` as a package pip. See the pip package here https://pypi.org/project/pyetfdb-scraper/.
 
 ```
 pip install pyetfdb-scraper
 ```
 
 ```python
 from pyetfdb_scraper import etf
 ```
 
 ## Example Usage
 
 ```python
-from pyetfdb_scraper.etf import ETF,load_etfs 
+from pyetfdb_scraper.etf import ETF,load_etfs
 # returns list of available ETFs.
 etfs = load_etfs()
-# load etf
+```
+```
+>>> ['SPY', 'IVV', 'VTI', 'VOO', 'QQQ', 'VEA', 'IEFA', ...]
+```
+### Retrieve info about a single ticker
+``` python
+# Load ETF
 ivv = ETF('IVV')
-# Get basic ETF information
+```
+
+```python
 print(ivv.info)
+```
+
+<details>
+<summary>  Results </summary>
 
+```
 >>> {
     "vitals": {
         "etf_name": "iShares Core S&P 500 ETF",
         "issuer": "BlackRock, Inc.",
         "issuer_link": "/issuer/blackrock-inc/",
         "brand": "iShares",
         "brand_link": "/issuer/ishares/",
@@ -152,16 +170,27 @@
             "assets": "$16.0 M",
             "avg_daily_volume": "4,800",
             "ytd_return": "7.15%",
         },
     ],
 }
 
+```
+</details>
+
+
+<br/>
+
+```python
 print(ivv.to_dict())
+```
+<details>
+<summary>Results</summary>
 
+```
 >>> {
     "info": {
         "vitals": {
             "issuer": "BlackRock, Inc.",
             "issuer_link": "/issuer/blackrock-inc/",
             "brand": "iShares",
             "brand_link": "/issuer/ishares/",
@@ -617,22 +646,26 @@
         {
             "metric": "Concentration",
             "metric_realtime_rating": "A-",
             "a+_metric_rated_etf": "VT",
         },
     ],
 }
-
 ```
+</details>
+
 ## Help Needed!
-I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as: 
+I am working full-time, and as such don't have much time to constantly push commits or updates. I will appreciate if some help can be provided, such as:
 * Unit tests for the current code
 * ETF Category has yet to be updated
 
-## Disclaimer 
-This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package creted by Jakub Pluta, which has since not been actively maintained.
-
 ## Contributing
-Pull requests are welcome.
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.
+
+If you are simply looking to start working with the codebase, navigate to the GitHub "issues" tab and start looking through interesting issues. You can also triage issues which may include reproducing bug reports, or asking for vital information such as version numbers or reproduction instructions. To read more about contributing, you can refer to [CONTRIBUTING](./CONTRIBUTING.md)
 
 ## License
-MIT License
+GPLv3
+
+## Disclaimer
+This package is built with some reference to the existing [pyetf](https://github.com/JakubPluta/pyetf) package.
```

### Comparing `pyetfdb_scraper-0.2/src/pyetfdb_scraper.egg-info/SOURCES.txt` & `pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/pyetfdb_scraper/utils.py
 src/pyetfdb_scraper.egg-info/PKG-INFO
 src/pyetfdb_scraper.egg-info/SOURCES.txt
 src/pyetfdb_scraper.egg-info/dependency_links.txt
 src/pyetfdb_scraper.egg-info/requires.txt
 src/pyetfdb_scraper.egg-info/top_level.txt
 src/pyetfdb_scraper/data/etfdb.json
+src/pyetfdb_scraper/data/user-agents.txt
 src/pyetfdb_scraper/models/__init__.py
 src/pyetfdb_scraper/models/expense.py
 src/pyetfdb_scraper/models/info.py
 src/pyetfdb_scraper/tabs/__init__.py
 src/pyetfdb_scraper/tabs/dividend.py
 src/pyetfdb_scraper/tabs/expense.py
 src/pyetfdb_scraper/tabs/holding_analysis.py
```

