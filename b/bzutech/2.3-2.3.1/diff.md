# Comparing `tmp/bzutech-2.3.tar.gz` & `tmp/bzutech-2.3.1.tar.gz`

## Comparing `bzutech-2.3.tar` & `bzutech-2.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.3/setup.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bzutech-2.3/test.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3/build/lib/bzutech/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/__init__.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/bzutechapi/BzuTechAPI.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/bzutechapi/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/device/Device.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/device/__init__.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/sensor/Sensor.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech/sensor/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/PKG-INFO
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/requires.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3/bzutech.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bzutech-2.3/tests/main.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.3/README.md
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bzutech-2.3/pyproject.toml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bzutech-2.3/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.3.1/setup.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 bzutech-2.3.1/test.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.1/build/lib/bzutech/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/bzutechapi/BzuTechAPI.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/bzutechapi/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/device/Device.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/device/__init__.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/sensor/Sensor.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech/sensor/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech.egg-info/requires.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.1/bzutech.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bzutech-2.3.1/tests/main.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.3.1/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 bzutech-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bzutech-2.3.1/PKG-INFO
```

### Comparing `bzutech-2.3/bzutech/bzutechapi/BzuTechAPI.py` & `bzutech-2.3.1/bzutech/bzutechapi/BzuTechAPI.py`

 * *Files identical despite different names*

### Comparing `bzutech-2.3/bzutech/device/Device.py` & `bzutech-2.3.1/bzutech/device/Device.py`

 * *Files identical despite different names*

### Comparing `bzutech-2.3/bzutech/sensor/Sensor.py` & `bzutech-2.3.1/bzutech/sensor/Sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from aiohttp import ClientSession
 class Sensor:
     def __init__(self, chipid: int, canal: str, apelido: str, token:dict) -> None:
         self.chipid = "11000"[0 : 8 - len(str(chipid))] + str(chipid)
         self.apelido = canal
         self.httpheaders = token
         self.porta = canal[-1]
+        self.last_reading = 0
 
         tipos_sensores = {
             "TMP": "Temperatura",
             "HUM": "Humidade",
             "VOT": "Voltagem",
             "CO2": "CO2",
             "CUR": "Corrente",
@@ -97,21 +98,23 @@
 
         try:
             self.tipo = tipos_sensores[canal.split("-")[1]]
             self.sensorref = canal[-1] + "00" + cod_sensores[canal[0:-2]]
         except KeyError:
             self.tipo = tipos_sensores["PIR"]
             self.sensorref = canal[-1] + "00" + cod_sensores["SR602-PIR"]
-            
+             
 
     async def get_leitura(self):
         url = (
             "https://back-prd.bzutech.com.br/logs/ultima_medicao/"
             + self.chipid
             + "/"
             + self.sensorref
         )
-        client = ClientSession()
+        client = ClientSession( )
         async with client.get(url, headers = self.httpheaders) as resp:
             resposta = await resp.json()
             await client.close()
-            return(int(resposta["medicao"]) / 1000000)
+            if("medicao" in resposta):
+                last_reading = int(resposta["medicao"]) / 1000000
+            return last_reading
```

### Comparing `bzutech-2.3/bzutech.egg-info/PKG-INFO` & `bzutech-2.3.1/bzutech.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bzutech-2.3/pyproject.toml` & `bzutech-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["bzutech"]
 
 [project]
 name = "bzutech"
-version = "2.3"
+version = "2.3.1"
 dependencies = [
     "aiohttp",
     "paho-mqtt"
 ]  
 authors = [
   { name="Ênio Ferreira", email="e.nioferreira@hotmail.com" },
 ]
```

### Comparing `bzutech-2.3/PKG-INFO` & `bzutech-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bzutech
-Version: 2.3
+Version: 2.3.1
 Summary: Integration package for bzutech services
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Ênio Ferreira <e.nioferreira@hotmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

