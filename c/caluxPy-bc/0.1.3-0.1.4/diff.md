# Comparing `tmp/caluxPy_bc-0.1.3.tar.gz` & `tmp/caluxPy_bc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxPy_bc-0.1.3.tar", last modified: Fri Apr  5 15:21:41 2024, max compression
+gzip compressed data, was "caluxPy_bc-0.1.4.tar", last modified: Fri Apr  5 15:28:07 2024, max compression
```

## Comparing `caluxPy_bc-0.1.3.tar` & `caluxPy_bc-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:21:41.822390 caluxPy_bc-0.1.3/
--rw-rw-rw-   0        0        0     1106 2024-01-11 15:50:15.000000 caluxPy_bc-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4600 2024-04-05 15:21:41.814655 caluxPy_bc-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2727 2024-02-08 19:40:01.000000 caluxPy_bc-0.1.3/README.md
--rw-rw-rw-   0        0        0      727 2024-04-05 14:56:50.000000 caluxPy_bc-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 15:21:41.822390 caluxPy_bc-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 15:21:41.767831 caluxPy_bc-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:21:41.803649 caluxPy_bc-0.1.3/src/caluxPy_bc/
--rw-rw-rw-   0        0        0    20398 2024-04-05 15:20:28.000000 caluxPy_bc-0.1.3/src/caluxPy_bc/CalculoPosicion.py
--rw-rw-rw-   0        0        0    10564 2024-02-09 14:29:14.000000 caluxPy_bc-0.1.3/src/caluxPy_bc/ExtraccionBGD.py
--rw-rw-rw-   0        0        0        0 2024-02-08 19:55:55.000000 caluxPy_bc-0.1.3/src/caluxPy_bc/__initi__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:21:41.814655 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/
--rw-rw-rw-   0        0        0     4600 2024-04-05 15:21:41.000000 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-04-05 15:21:41.000000 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:21:41.000000 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-05 15:21:41.000000 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 15:21:41.000000 caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.816577 caluxPy_bc-0.1.4/
+-rw-rw-rw-   0        0        0     1106 2024-01-11 15:50:15.000000 caluxPy_bc-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4600 2024-04-05 15:28:07.815502 caluxPy_bc-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2727 2024-02-08 19:40:01.000000 caluxPy_bc-0.1.4/README.md
+-rw-rw-rw-   0        0        0      727 2024-04-05 15:27:32.000000 caluxPy_bc-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:28:07.816577 caluxPy_bc-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.779184 caluxPy_bc-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.801680 caluxPy_bc-0.1.4/src/caluxPy_bc/
+-rw-rw-rw-   0        0        0    20398 2024-04-05 15:27:10.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/CalculoPosicion.py
+-rw-rw-rw-   0        0        0    10564 2024-02-09 14:29:14.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/ExtraccionBGD.py
+-rw-rw-rw-   0        0        0        0 2024-02-08 19:55:55.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/__initi__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.809605 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/
+-rw-rw-rw-   0        0        0     4600 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/top_level.txt
```

### Comparing `caluxPy_bc-0.1.3/LICENSE.txt` & `caluxPy_bc-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.3/PKG-INFO` & `caluxPy_bc-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_bc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Extraction Tool
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxPy_bc-0.1.3/README.md` & `caluxPy_bc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.3/pyproject.toml` & `caluxPy_bc-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_bc"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Data Extraction Tool"
```

### Comparing `caluxPy_bc-0.1.3/src/caluxPy_bc/CalculoPosicion.py` & `caluxPy_bc-0.1.4/src/caluxPy_bc/CalculoPosicion.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         informaciones_entidad['Entidad'] = entidad
         informaciones_entidad[['Subsector', 'Entidad']] = informaciones_entidad['Entidad'].str.split(' ', n = 1, expand = True)
         informaciones_entidad = informaciones_entidad[['Fecha', 
                                                        'Periodicidad', 
                                                        'Entidad', 
                                                        'Subsector',
                                                        'AyC',
-                                                       'PyC' 
+                                                       'PyC',
                                                        'Posicion', 
                                                        'Capital', 
                                                        'Capital + Add',
                                                        '%Capital', 
                                                        '%Capital + Add',
                                                        'Tipo Cambio'
                                                        ]]#, 'Variacion']]
```

### Comparing `caluxPy_bc-0.1.3/src/caluxPy_bc/ExtraccionBGD.py` & `caluxPy_bc-0.1.4/src/caluxPy_bc/ExtraccionBGD.py`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.3/src/caluxPy_bc.egg-info/PKG-INFO` & `caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_bc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Extraction Tool
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

