# Comparing `tmp/vagen-0.0.1.tar.gz` & `tmp/vagen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagen-0.0.1.tar", last modified: Sat Sep 16 23:20:50 2023, max compression
+gzip compressed data, was "vagen-0.1.0.tar", last modified: Fri Apr  5 17:21:20 2024, max compression
```

## Comparing `vagen-0.0.1.tar` & `vagen-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-09-16 23:20:50.747352 vagen-0.0.1/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1079 2023-08-05 15:00:17.000000 vagen-0.0.1/LICENSE
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     4032 2023-09-16 23:20:50.747352 vagen-0.0.1/PKG-INFO
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     3491 2023-09-16 23:05:50.000000 vagen-0.0.1/README.md
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      608 2023-09-16 23:10:27.000000 vagen-0.0.1/pyproject.toml
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-09-16 23:20:50.747352 vagen-0.0.1/setup.cfg
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-09-16 23:20:50.747352 vagen-0.0.1/tests/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    18103 2023-08-25 20:24:20.000000 vagen-0.0.1/tests/testHiLevelMod.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    53314 2023-09-08 11:22:47.000000 vagen-0.0.1/tests/testVA.py
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-09-16 23:20:50.747352 vagen-0.0.1/vagen/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     3212 2023-08-09 12:16:49.000000 vagen-0.0.1/vagen/__init__.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    82287 2023-09-09 23:16:43.000000 vagen-0.0.1/vagen/hilevelmod.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)   122215 2023-09-09 16:36:01.000000 vagen-0.0.1/vagen/veriloga.py
-drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-09-16 23:20:50.747352 vagen-0.0.1/vagen.egg-info/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     4032 2023-09-16 23:20:50.000000 vagen-0.0.1/vagen.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      272 2023-09-16 23:20:50.000000 vagen-0.0.1/vagen.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-09-16 23:20:50.000000 vagen-0.0.1/vagen.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       30 2023-09-16 23:20:50.000000 vagen-0.0.1/vagen.egg-info/requires.txt
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        6 2023-09-16 23:20:50.000000 vagen-0.0.1/vagen.egg-info/top_level.txt
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2024-04-05 17:21:20.732781 vagen-0.1.0/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1079 2023-08-05 15:00:17.000000 vagen-0.1.0/LICENSE
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     4021 2024-04-05 17:21:20.728781 vagen-0.1.0/PKG-INFO
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     3480 2024-03-19 19:42:32.000000 vagen-0.1.0/README.md
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      608 2024-04-05 17:19:22.000000 vagen-0.1.0/pyproject.toml
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       38 2024-04-05 17:21:20.732781 vagen-0.1.0/setup.cfg
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2024-04-05 17:21:20.728781 vagen-0.1.0/tests/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    18103 2023-08-25 20:24:03.000000 vagen-0.1.0/tests/testHiLevelMod.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    53342 2024-03-19 19:52:11.000000 vagen-0.1.0/tests/testVA.py
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2024-04-05 17:21:20.728781 vagen-0.1.0/vagen/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     3212 2023-08-09 12:16:49.000000 vagen-0.1.0/vagen/__init__.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    82287 2023-09-09 23:16:43.000000 vagen-0.1.0/vagen/hilevelmod.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)   122229 2024-03-19 19:43:58.000000 vagen-0.1.0/vagen/veriloga.py
+drwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2024-04-05 17:21:20.728781 vagen-0.1.0/vagen.egg-info/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     4021 2024-04-05 17:21:20.000000 vagen-0.1.0/vagen.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)      272 2024-04-05 17:21:20.000000 vagen-0.1.0/vagen.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        1 2024-04-05 17:21:20.000000 vagen-0.1.0/vagen.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)       30 2024-04-05 17:21:20.000000 vagen-0.1.0/vagen.egg-info/requires.txt
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)        6 2024-04-05 17:21:20.000000 vagen-0.1.0/vagen.egg-info/top_level.txt
```

### Comparing `vagen-0.0.1/LICENSE` & `vagen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vagen-0.0.1/PKG-INFO` & `vagen-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagen
-Version: 0.0.1
+Version: 0.1.0
 Summary: Generates verilogA testbench for verification of analog IPs (VLSI design)
 Author-email: Rodrigo Pedroso Mendes <roedroso@gmail.com>
 Project-URL: Homepage, https://github.com/rpm2003rpm/vagen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -46,18 +46,18 @@
 
 #Create a module     
 mod = va.HiLevelMod("DCDC_STML")
 
 #Create pins
 VDD = mod.vdc(name = "VDD", width = 1, direction = "inout")
 OUT = mod.idc(name = "OUT", width = 1, direction = "inout")
-CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-15, fall = 100e-15))
-RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-12, fall = 100e-12))
+RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 READY = mod.dig(name = "READY", domain = VDD, width = 1, direction = "input")
-CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 
 #READY positive event
 EVNT_READY = va.Cross(READY.diffHalfDomain, "rising")
 
 #Sequence
 mod.seq(True)(
     VDD.setRiseFall(10e-6, 10e-6),
@@ -113,15 +113,15 @@
 #Create a module
 mod = va.HiLevelMod("CONFIG_RES")
 
 #Create pins
 VDD = mod.electrical(name = "VDD", width = 1, direction = "inout")
 IN1 = mod.electrical(name = "IN1", width = 1, direction = "inout")
 IN2 = mod.electrical(name = "IN2", width = 1, direction = "inout")
-CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, value = 0, inCap = 100e-15, direction = "input")
+CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, inCap = 100e-15, direction = "input")
 
 #Parameters
 alfa = mod.par(name = "alfa", value = 10.0)
 
 #Analog block
 mod.analog(
     va.Branch(IN1, IN2).vCont(va.Branch(IN1, IN2).i*(va.Real(CONFIG.read(signed = False)) + 1)*alfa)
```

### Comparing `vagen-0.0.1/README.md` & `vagen-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 
 #Create a module     
 mod = va.HiLevelMod("DCDC_STML")
 
 #Create pins
 VDD = mod.vdc(name = "VDD", width = 1, direction = "inout")
 OUT = mod.idc(name = "OUT", width = 1, direction = "inout")
-CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-15, fall = 100e-15))
-RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-12, fall = 100e-12))
+RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 READY = mod.dig(name = "READY", domain = VDD, width = 1, direction = "input")
-CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 
 #READY positive event
 EVNT_READY = va.Cross(READY.diffHalfDomain, "rising")
 
 #Sequence
 mod.seq(True)(
     VDD.setRiseFall(10e-6, 10e-6),
@@ -98,15 +98,15 @@
 #Create a module
 mod = va.HiLevelMod("CONFIG_RES")
 
 #Create pins
 VDD = mod.electrical(name = "VDD", width = 1, direction = "inout")
 IN1 = mod.electrical(name = "IN1", width = 1, direction = "inout")
 IN2 = mod.electrical(name = "IN2", width = 1, direction = "inout")
-CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, value = 0, inCap = 100e-15, direction = "input")
+CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, inCap = 100e-15, direction = "input")
 
 #Parameters
 alfa = mod.par(name = "alfa", value = 10.0)
 
 #Analog block
 mod.analog(
     va.Branch(IN1, IN2).vCont(va.Branch(IN1, IN2).i*(va.Real(CONFIG.read(signed = False)) + 1)*alfa)
```

### Comparing `vagen-0.0.1/pyproject.toml` & `vagen-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools >= 58.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vagen"
-version = "0.0.1"
+version = "0.1.0"
 authors = [{name="Rodrigo Pedroso Mendes", email="roedroso@gmail.com"}]
 description = "Generates verilogA testbench for verification of analog IPs (VLSI design)"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["regex>=2023.6.3", "datetime>=5.2"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `vagen-0.0.1/tests/testHiLevelMod.py` & `vagen-0.1.0/tests/testHiLevelMod.py`

 * *Files identical despite different names*

### Comparing `vagen-0.0.1/tests/testVA.py` & `vagen-0.1.0/tests/testVA.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,18 +295,18 @@
         a = Integer('a')
         b = Integer('b')
         c = 6
         self.assertEqual(type(a**b), Integer)
         self.assertEqual(type(b**a), Integer)
         self.assertEqual(type(b**c), Integer)
         self.assertEqual(type(c**a), Integer)
-        self.assertEqual(str(a**b), 'pow(a, b)')
-        self.assertEqual(str(b**a), 'pow(b, a)')
-        self.assertEqual(str(b**c), 'pow(b, {:d})'.format(c))
-        self.assertEqual(str(c**a), 'pow({:d}, a)'.format(c))
+        self.assertEqual(str(a**b), '_rtoi(pow(a, b))')
+        self.assertEqual(str(b**a), '_rtoi(pow(b, a))')
+        self.assertEqual(str(b**c), '_rtoi(pow(b, {:d}))'.format(c))
+        self.assertEqual(str(c**a), '_rtoi(pow({:d}, a))'.format(c))
 
     def testIntegerRShift(self):
         a = Integer('a')
         b = Integer('b')
         c = 6
         self.assertEqual(type(a>>b), Integer)
         self.assertEqual(type(b>>a), Integer)
```

### Comparing `vagen-0.0.1/vagen/__init__.py` & `vagen-0.1.0/vagen/__init__.py`

 * *Files identical despite different names*

### Comparing `vagen-0.0.1/vagen/hilevelmod.py` & `vagen-0.1.0/vagen/hilevelmod.py`

 * *Files identical despite different names*

### Comparing `vagen-0.0.1/vagen/veriloga.py` & `vagen-0.1.0/vagen/veriloga.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,26 +901,26 @@
     #  @param self Base object pointer.
     #  @param other Exponent. 
     #  @return expression representing the power.
     #
     #---------------------------------------------------------------------------
     def __pow__(self, other):
         other = parseInteger("other", other)
-        return Integer(f'pow({self}, {other})')
+        return Integer(f'_rtoi(pow({self}, {other}))')
         
     #---------------------------------------------------------------------------
     ## Reverse pow override.
     #  @param self Exponent object pointer.
     #  @param other Base. 
     #  @return expression representing the power.
     #
     #---------------------------------------------------------------------------
     def __rpow__(self, other):
         other = parseInteger("other", other)
-        return Integer(f'pow({other}, {self})')
+        return Integer(f'_rtoi(pow({other}, {self}))')
         
     #---------------------------------------------------------------------------
     ## right shift override.
     #  @param self Integer to be shifted.
     #  @param other number of times the number will be shifted.
     #  @return expression representing the shift.
     #
```

### Comparing `vagen-0.0.1/vagen.egg-info/PKG-INFO` & `vagen-0.1.0/vagen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagen
-Version: 0.0.1
+Version: 0.1.0
 Summary: Generates verilogA testbench for verification of analog IPs (VLSI design)
 Author-email: Rodrigo Pedroso Mendes <roedroso@gmail.com>
 Project-URL: Homepage, https://github.com/rpm2003rpm/vagen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -46,18 +46,18 @@
 
 #Create a module     
 mod = va.HiLevelMod("DCDC_STML")
 
 #Create pins
 VDD = mod.vdc(name = "VDD", width = 1, direction = "inout")
 OUT = mod.idc(name = "OUT", width = 1, direction = "inout")
-CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-15, fall = 100e-15))
-RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CLK = mod.clock(mod.dig(name = "CLK", domain = VDD, width = 1, direction = "output", rise = 100e-12, fall = 100e-12))
+RST = mod.dig(name = "RST", domain = VDD, width = 1, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 READY = mod.dig(name = "READY", domain = VDD, width = 1, direction = "input")
-CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-15, fall = 100e-15)
+CONFIG_VOUT = mod.dig(name = "CONFIG_VOUT", domain = VDD, width = 4, value = 0, direction = "output", rise = 100e-12, fall = 100e-12)
 
 #READY positive event
 EVNT_READY = va.Cross(READY.diffHalfDomain, "rising")
 
 #Sequence
 mod.seq(True)(
     VDD.setRiseFall(10e-6, 10e-6),
@@ -113,15 +113,15 @@
 #Create a module
 mod = va.HiLevelMod("CONFIG_RES")
 
 #Create pins
 VDD = mod.electrical(name = "VDD", width = 1, direction = "inout")
 IN1 = mod.electrical(name = "IN1", width = 1, direction = "inout")
 IN2 = mod.electrical(name = "IN2", width = 1, direction = "inout")
-CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, value = 0, inCap = 100e-15, direction = "input")
+CONFIG = mod.dig(name = "CONFIG", domain = VDD, width = 4, inCap = 100e-15, direction = "input")
 
 #Parameters
 alfa = mod.par(name = "alfa", value = 10.0)
 
 #Analog block
 mod.analog(
     va.Branch(IN1, IN2).vCont(va.Branch(IN1, IN2).i*(va.Real(CONFIG.read(signed = False)) + 1)*alfa)
```

