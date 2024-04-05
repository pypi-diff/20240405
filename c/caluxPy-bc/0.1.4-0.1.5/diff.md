# Comparing `tmp/caluxPy_bc-0.1.4.tar.gz` & `tmp/caluxPy_bc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxPy_bc-0.1.4.tar", last modified: Fri Apr  5 15:28:07 2024, max compression
+gzip compressed data, was "caluxPy_bc-0.1.5.tar", last modified: Fri Apr  5 15:54:08 2024, max compression
```

## Comparing `caluxPy_bc-0.1.4.tar` & `caluxPy_bc-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.816577 caluxPy_bc-0.1.4/
--rw-rw-rw-   0        0        0     1106 2024-01-11 15:50:15.000000 caluxPy_bc-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4600 2024-04-05 15:28:07.815502 caluxPy_bc-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2727 2024-02-08 19:40:01.000000 caluxPy_bc-0.1.4/README.md
--rw-rw-rw-   0        0        0      727 2024-04-05 15:27:32.000000 caluxPy_bc-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 15:28:07.816577 caluxPy_bc-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.779184 caluxPy_bc-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.801680 caluxPy_bc-0.1.4/src/caluxPy_bc/
--rw-rw-rw-   0        0        0    20398 2024-04-05 15:27:10.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/CalculoPosicion.py
--rw-rw-rw-   0        0        0    10564 2024-02-09 14:29:14.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/ExtraccionBGD.py
--rw-rw-rw-   0        0        0        0 2024-02-08 19:55:55.000000 caluxPy_bc-0.1.4/src/caluxPy_bc/__initi__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:28:07.809605 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/
--rw-rw-rw-   0        0        0     4600 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 15:28:07.000000 caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 15:54:08.114677 caluxPy_bc-0.1.5/
+-rw-rw-rw-   0        0        0     1106 2024-01-11 15:50:15.000000 caluxPy_bc-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4600 2024-04-05 15:54:08.114677 caluxPy_bc-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2727 2024-02-08 19:40:01.000000 caluxPy_bc-0.1.5/README.md
+-rw-rw-rw-   0        0        0      727 2024-04-05 15:48:49.000000 caluxPy_bc-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:54:08.114677 caluxPy_bc-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 15:54:08.069775 caluxPy_bc-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 15:54:08.097941 caluxPy_bc-0.1.5/src/caluxPy_bc/
+-rw-rw-rw-   0        0        0    20398 2024-04-05 15:47:01.000000 caluxPy_bc-0.1.5/src/caluxPy_bc/CalculoPosicion.py
+-rw-rw-rw-   0        0        0    10564 2024-04-05 15:47:34.000000 caluxPy_bc-0.1.5/src/caluxPy_bc/ExtraccionBGD.py
+-rw-rw-rw-   0        0        0        0 2024-02-08 19:55:55.000000 caluxPy_bc-0.1.5/src/caluxPy_bc/__initi__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:54:08.114677 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/
+-rw-rw-rw-   0        0        0     4600 2024-04-05 15:54:08.000000 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-05 15:54:08.000000 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:54:08.000000 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-05 15:54:08.000000 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-05 15:54:08.000000 caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/top_level.txt
```

### Comparing `caluxPy_bc-0.1.4/LICENSE.txt` & `caluxPy_bc-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.4/PKG-INFO` & `caluxPy_bc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_bc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Extraction Tool
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxPy_bc-0.1.4/README.md` & `caluxPy_bc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.4/pyproject.toml` & `caluxPy_bc-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_bc"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Data Extraction Tool"
```

### Comparing `caluxPy_bc-0.1.4/src/caluxPy_bc/CalculoPosicion.py` & `caluxPy_bc-0.1.5/src/caluxPy_bc/CalculoPosicion.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -323,22 +323,22 @@
         capital_subsector = pd.concat([capital_diario, capital_mensual])
         informaciones_entidad['Entidad'] = entidad
         informaciones_entidad[['Subsector', 'Entidad']] = informaciones_entidad['Entidad'].str.split(' ', n = 1, expand = True)
         informaciones_entidad = informaciones_entidad[['Fecha', 
                                                        'Periodicidad', 
                                                        'Entidad', 
                                                        'Subsector',
-                                                       'AyC',
-                                                       'PyC',
                                                        'Posicion', 
                                                        'Capital', 
                                                        'Capital + Add',
                                                        '%Capital', 
                                                        '%Capital + Add',
                                                        'Tipo Cambio'
+                                                       'AyC',
+                                                       'PyC',
                                                        ]]#, 'Variacion']]
 
         return informaciones_entidad, capital_subsector
 
     def calculo_subsector_sistema(self, df_entidades):
         df_total = pd.DataFrame()
```

### Comparing `caluxPy_bc-0.1.4/src/caluxPy_bc/ExtraccionBGD.py` & `caluxPy_bc-0.1.5/src/caluxPy_bc/ExtraccionBGD.py`

 * *Files identical despite different names*

### Comparing `caluxPy_bc-0.1.4/src/caluxPy_bc.egg-info/PKG-INFO` & `caluxPy_bc-0.1.5/src/caluxPy_bc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_bc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Extraction Tool
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

