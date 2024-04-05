# Comparing `tmp/py_valid_proxy-0.2.9.tar.gz` & `tmp/py_valid_proxy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_valid_proxy-0.2.9.tar", max compression
+gzip compressed data, was "py_valid_proxy-0.3.0.tar", max compression
```

## Comparing `py_valid_proxy-0.2.9.tar` & `py_valid_proxy-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1460 2024-04-04 08:02:21.206608 py_valid_proxy-0.2.9/README.md
--rw-r--r--   0        0        0      503 2024-04-04 15:10:20.716793 py_valid_proxy-0.2.9/py_valid_proxy/__init__.py
--rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.2.9/py_valid_proxy/__main__.py
--rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.2.9/py_valid_proxy/data/GeoLite2-Country.mmdb
--rw-r--r--   0        0        0     2459 2024-04-04 07:46:27.183964 py_valid_proxy-0.2.9/py_valid_proxy/main.py
--rw-r--r--   0        0        0     4128 2024-04-04 07:39:33.487215 py_valid_proxy-0.2.9/py_valid_proxy/valid_proxy.py
--rw-r--r--   0        0        0      524 2024-04-04 15:10:16.188741 py_valid_proxy-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 py_valid_proxy-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1460 2024-04-04 08:02:21.206608 py_valid_proxy-0.3.0/README.md
+-rw-r--r--   0        0        0      503 2024-04-05 07:22:23.388944 py_valid_proxy-0.3.0/py_valid_proxy/__init__.py
+-rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.3.0/py_valid_proxy/__main__.py
+-rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.3.0/py_valid_proxy/data/GeoLite2-Country.mmdb
+-rw-r--r--   0        0        0     2459 2024-04-04 07:46:27.183964 py_valid_proxy-0.3.0/py_valid_proxy/main.py
+-rw-r--r--   0        0        0     4128 2024-04-04 07:39:33.487215 py_valid_proxy-0.3.0/py_valid_proxy/valid_proxy.py
+-rw-r--r--   0        0        0      523 2024-04-05 07:22:14.640843 py_valid_proxy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 py_valid_proxy-0.3.0/PKG-INFO
```

### Comparing `py_valid_proxy-0.2.9/README.md` & `py_valid_proxy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.9/py_valid_proxy/data/GeoLite2-Country.mmdb` & `py_valid_proxy-0.3.0/py_valid_proxy/data/GeoLite2-Country.mmdb`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.9/py_valid_proxy/main.py` & `py_valid_proxy-0.3.0/py_valid_proxy/main.py`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.9/py_valid_proxy/valid_proxy.py` & `py_valid_proxy-0.3.0/py_valid_proxy/valid_proxy.py`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.9/pyproject.toml` & `py_valid_proxy-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "py-valid-proxy"
-version = "0.2.9"
+version = "0.3.0"
 description = "Valid proxy server ('alive' or 'dead')"
 authors = ["Suvorinov Oleg <suvorinovoleg@yandex.ru>"]
 homepage="https://github.com/suvorinov/py_valid_proxy.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 requests = "^2.31.0"
 geoip2 = "^4.7.0"
 dataclasses-json = "^0.6.3"
 rich = "^13.7.0"
 
 [tool.poetry.scripts]
 valid_proxy = "py_valid_proxy.main:main"
```

### Comparing `py_valid_proxy-0.2.9/PKG-INFO` & `py_valid_proxy-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: py-valid-proxy
-Version: 0.2.9
+Version: 0.3.0
 Summary: Valid proxy server ('alive' or 'dead')
 Home-page: https://github.com/suvorinov/py_valid_proxy.git
 Author: Suvorinov Oleg
 Author-email: suvorinovoleg@yandex.ru
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
 Requires-Dist: geoip2 (>=4.7.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Description-Content-Type: text/markdown
```

