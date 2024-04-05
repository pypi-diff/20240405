# Comparing `tmp/ariston-0.19.2.tar.gz` & `tmp/ariston-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.19.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.19.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.19.2.tar` & `ariston-0.19.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2024-03-01 16:36:27.881389 ariston-0.19.2/LICENSE
--rw-r--r--   0        0        0     3539 2024-03-01 16:36:27.881389 ariston-0.19.2/README.md
--rw-r--r--   0        0        0     5962 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/__init__.py
--rw-r--r--   0        0        0    31033 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/ariston_api.py
--rw-r--r--   0        0        0    12128 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/base_device.py
--rw-r--r--   0        0        0    15230 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/bsb_device.py
--rw-r--r--   0        0        0    18190 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/const.py
--rw-r--r--   0        0        0     1927 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/device.py
--rw-r--r--   0        0        0     4024 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/evo_device.py
--rw-r--r--   0        0        0     1331 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0     3923 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/evo_one_device.py
--rw-r--r--   0        0        0    38267 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/galevo_device.py
--rw-r--r--   0        0        0      830 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/lux2_device.py
--rw-r--r--   0        0        0     1515 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/lux_device.py
--rw-r--r--   0        0        0    11270 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0    10247 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     3545 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/velis_base_device.py
--rw-r--r--   0        0        0     4552 2024-03-01 16:36:27.881389 ariston-0.19.2/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2024-03-01 16:36:27.881389 ariston-0.19.2/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 ariston-0.19.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-05 18:38:09.051755 ariston-0.19.3/LICENSE
+-rw-r--r--   0        0        0     3539 2024-04-05 18:38:09.051755 ariston-0.19.3/README.md
+-rw-r--r--   0        0        0     5962 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/__init__.py
+-rw-r--r--   0        0        0    31109 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/ariston_api.py
+-rw-r--r--   0        0        0    12128 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/base_device.py
+-rw-r--r--   0        0        0    15230 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/bsb_device.py
+-rw-r--r--   0        0        0    18190 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/const.py
+-rw-r--r--   0        0        0     1927 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/device.py
+-rw-r--r--   0        0        0     4024 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_device.py
+-rw-r--r--   0        0        0     1331 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0     3923 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/evo_one_device.py
+-rw-r--r--   0        0        0    38267 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/galevo_device.py
+-rw-r--r--   0        0        0      830 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lux2_device.py
+-rw-r--r--   0        0        0     1515 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lux_device.py
+-rw-r--r--   0        0        0    11270 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0    10247 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     3545 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/velis_base_device.py
+-rw-r--r--   0        0        0     4552 2024-04-05 18:38:09.051755 ariston-0.19.3/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2024-04-05 18:38:09.051755 ariston-0.19.3/pyproject.toml
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 ariston-0.19.3/PKG-INFO
```

### Comparing `ariston-0.19.2/LICENSE` & `ariston-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/README.md` & `ariston-0.19.3/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/__init__.py` & `ariston-0.19.3/ariston/__init__.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/ariston_api.py` & `ariston-0.19.3/ariston/ariston_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,15 @@
         method: str,
         path: str,
         params: Optional[dict[str, Any]] = None,
         body: Any = None,
         is_retry: bool = False,
     ) -> Optional[dict[str, Any]]:
         """Request with requests"""
-        headers = {"ar.authToken": self.__token}
+        headers = {"User-Agent": "RestSharp/106.11.7.0", "ar.authToken": self.__token}
 
         _LOGGER.debug(
             "Request method %s, path: %s, params: %s",
             method,
             path,
             params,
         )
@@ -868,15 +868,15 @@
         method: str,
         path: str,
         params: Optional[dict[str, Any]] = None,
         body: Any = None,
         is_retry: bool = False,
     ) -> Optional[dict[str, Any]]:
         """Async request with aiohttp"""
-        headers = {"ar.authToken": self.__token}
+        headers = {"User-Agent": "RestSharp/106.11.7.0", "ar.authToken": self.__token}
 
         _LOGGER.debug(
             "Request method %s, path: %s, params: %s",
             method,
             path,
             params,
         )
```

### Comparing `ariston-0.19.2/ariston/base_device.py` & `ariston-0.19.3/ariston/base_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/bsb_device.py` & `ariston-0.19.3/ariston/bsb_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/const.py` & `ariston-0.19.3/ariston/const.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/device.py` & `ariston-0.19.3/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/evo_device.py` & `ariston-0.19.3/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/evo_lydos_device.py` & `ariston-0.19.3/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/evo_one_device.py` & `ariston-0.19.3/ariston/evo_one_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/galevo_device.py` & `ariston-0.19.3/ariston/galevo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/lux2_device.py` & `ariston-0.19.3/ariston/lux2_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/lux_device.py` & `ariston-0.19.3/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/lydos_hybrid_device.py` & `ariston-0.19.3/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/nuos_split_device.py` & `ariston-0.19.3/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/velis_base_device.py` & `ariston-0.19.3/ariston/velis_base_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/ariston/velis_device.py` & `ariston-0.19.3/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.19.2/PKG-INFO` & `ariston-0.19.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.19.2
+Version: 0.19.3
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

