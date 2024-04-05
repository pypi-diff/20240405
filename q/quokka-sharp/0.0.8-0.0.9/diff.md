# Comparing `tmp/quokka_sharp-0.0.8.tar.gz` & `tmp/quokka_sharp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka_sharp-0.0.8.tar", last modified: Wed Feb 28 17:06:55 2024, max compression
+gzip compressed data, was "quokka_sharp-0.0.9.tar", last modified: Wed Feb 28 17:21:23 2024, max compression
```

## Comparing `quokka_sharp-0.0.8.tar` & `quokka_sharp-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:06:55.021121 quokka_sharp-0.0.8/
--rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:06:55.020806 quokka_sharp-0.0.8/PKG-INFO
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:06:55.017196 quokka_sharp-0.0.8/quokka_sharp/
--rw-r--r--   0 meij     (1596456755) 208802054      108 2024-02-28 16:43:51.000000 quokka_sharp-0.0.8/quokka_sharp/__init__.py
--rw-r--r--   0 meij     (1596456755) 208802054     4080 2024-02-28 17:06:15.000000 quokka_sharp-0.0.8/quokka_sharp/ecmc.py
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:06:55.020326 quokka_sharp-0.0.8/quokka_sharp/encoding/
--rw-r--r--   0 meij     (1596456755) 208802054      138 2024-02-16 14:29:26.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/__init__.py
--rw-r--r--   0 meij     (1596456755) 208802054     9090 2024-02-15 09:34:01.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/cliffordt2cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     8910 2024-02-18 14:22:12.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/cliffordt2cnf_py_codegen.py
--rw-r--r--   0 meij     (1596456755) 208802054     3293 2024-02-15 17:19:49.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     1115 2024-01-31 13:15:02.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/memory.py
--rw-r--r--   0 meij     (1596456755) 208802054     4061 2024-02-28 16:39:25.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/qasm2cnf.py
--rw-r--r--   0 meij     (1596456755) 208802054     6155 2024-02-27 11:17:06.000000 quokka_sharp-0.0.8/quokka_sharp/encoding/qasm_parser.py
--rw-r--r--   0 meij     (1596456755) 208802054     2760 2024-02-28 17:06:00.000000 quokka_sharp-0.0.8/quokka_sharp/qcmc.py
--rw-r--r--   0 meij     (1596456755) 208802054       14 2024-02-28 16:40:47.000000 quokka_sharp-0.0.8/quokka_sharp/settings.py
-drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:06:55.018196 quokka_sharp-0.0.8/quokka_sharp.egg-info/
--rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:06:54.000000 quokka_sharp-0.0.8/quokka_sharp.egg-info/PKG-INFO
--rw-r--r--   0 meij     (1596456755) 208802054      534 2024-02-28 17:06:54.000000 quokka_sharp-0.0.8/quokka_sharp.egg-info/SOURCES.txt
--rw-r--r--   0 meij     (1596456755) 208802054        1 2024-02-28 17:06:54.000000 quokka_sharp-0.0.8/quokka_sharp.egg-info/dependency_links.txt
--rw-r--r--   0 meij     (1596456755) 208802054       12 2024-02-28 17:06:54.000000 quokka_sharp-0.0.8/quokka_sharp.egg-info/requires.txt
--rw-r--r--   0 meij     (1596456755) 208802054       13 2024-02-28 17:06:54.000000 quokka_sharp-0.0.8/quokka_sharp.egg-info/top_level.txt
--rw-r--r--   0 meij     (1596456755) 208802054       38 2024-02-28 17:06:55.021180 quokka_sharp-0.0.8/setup.cfg
--rw-r--r--   0 meij     (1596456755) 208802054     1059 2024-02-28 17:06:33.000000 quokka_sharp-0.0.8/setup.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.757800 quokka_sharp-0.0.9/
+-rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:21:23.757518 quokka_sharp-0.0.9/PKG-INFO
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.753909 quokka_sharp-0.0.9/quokka_sharp/
+-rw-r--r--   0 meij     (1596456755) 208802054       76 2024-02-28 17:12:12.000000 quokka_sharp-0.0.9/quokka_sharp/__init__.py
+-rw-r--r--   0 meij     (1596456755) 208802054     4047 2024-02-28 17:18:34.000000 quokka_sharp-0.0.9/quokka_sharp/ecmc.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.757035 quokka_sharp-0.0.9/quokka_sharp/encoding/
+-rw-r--r--   0 meij     (1596456755) 208802054      138 2024-02-16 14:29:26.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/__init__.py
+-rw-r--r--   0 meij     (1596456755) 208802054     9090 2024-02-15 09:34:01.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     8910 2024-02-18 14:22:12.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf_py_codegen.py
+-rw-r--r--   0 meij     (1596456755) 208802054     3293 2024-02-15 17:19:49.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     1115 2024-01-31 13:15:02.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/memory.py
+-rw-r--r--   0 meij     (1596456755) 208802054     4061 2024-02-28 16:39:25.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/qasm2cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     6155 2024-02-27 11:17:06.000000 quokka_sharp-0.0.9/quokka_sharp/encoding/qasm_parser.py
+-rw-r--r--   0 meij     (1596456755) 208802054     2839 2024-02-28 17:20:31.000000 quokka_sharp-0.0.9/quokka_sharp/qcmc.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-02-28 17:21:23.754909 quokka_sharp-0.0.9/quokka_sharp.egg-info/
+-rw-r--r--   0 meij     (1596456755) 208802054      760 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/PKG-INFO
+-rw-r--r--   0 meij     (1596456755) 208802054      509 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/SOURCES.txt
+-rw-r--r--   0 meij     (1596456755) 208802054        1 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/dependency_links.txt
+-rw-r--r--   0 meij     (1596456755) 208802054       12 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/requires.txt
+-rw-r--r--   0 meij     (1596456755) 208802054       13 2024-02-28 17:21:23.000000 quokka_sharp-0.0.9/quokka_sharp.egg-info/top_level.txt
+-rw-r--r--   0 meij     (1596456755) 208802054       38 2024-02-28 17:21:23.757854 quokka_sharp-0.0.9/setup.cfg
+-rw-r--r--   0 meij     (1596456755) 208802054     1059 2024-02-28 17:20:58.000000 quokka_sharp-0.0.9/setup.py
```

### Comparing `quokka_sharp-0.0.8/PKG-INFO` & `quokka_sharp-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka_sharp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quokka Sharp
 Author: System Verification Lab
 Author-email: j.mei@liacs.leidenuniv.nl
 Keywords: python,quantum circuits
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quokka_sharp-0.0.8/quokka_sharp/ecmc.py` & `quokka_sharp-0.0.9/quokka_sharp/ecmc.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 import time
 from .encoding.qasm_parser import QASMparser
 from .encoding.qasm2cnf import QASM2CNF
 from subprocess import PIPE, Popen
 from queue import Queue
 from .encoding.memory import ReturnValueThread, memory_monitor
 
+class Result:
+    def __init__(self, time, result):
+        self.time = time
+        if result:
+            self.result = "equivalent"
+        else:
+            self.result = "not_equivalent"
 
 def GPMC(cnf_file):
     # gpmc_path = shutil.which("gpmc")
     # if gpmc_path == None:
     #     sys.exit("Binary gpmc not found in path.")
     gpmc_path = TOOL_PATH
     proc = Popen([gpmc_path, "-mode=1", cnf_file], stdout= PIPE, stderr=PIPE)
@@ -109,20 +116,16 @@
         procdict[pid].terminate()
     
     end = time.time()
 
     queue.put('stop')
     max_rss = monitor_thread.join()
 
-    G1 = len(circuit1.circ)
-    G2 = len(circuit2.circ)
-    print(  ' {"time":', (end - start) + encode_time,
-            ', "result":' + ' "' + str(result) + '"',
-            ', "MaxRSS":', max_rss / 1024 / 1024,
-            ', "N":', cnf.n, ', "G1":', G1, ', "G2":', G2, "}")
+    res = Result(end - start, result)
+    return res
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='ECMC: The quantum circuit Equivalence Checker based on Model Counting from the Quokka-Sharp (Quokka#) package')
     parser.add_argument('toolpath')
     parser.add_argument('qasmfile1')
     parser.add_argument('qasmfile2')
     args = parser.parse_args()
```

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/cliffordt2cnf.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/cliffordt2cnf_py_codegen.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/cliffordt2cnf_py_codegen.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/cnf.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/cnf.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/memory.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/memory.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/qasm2cnf.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/qasm2cnf.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/encoding/qasm_parser.py` & `quokka_sharp-0.0.9/quokka_sharp/encoding/qasm_parser.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-0.0.8/quokka_sharp/qcmc.py` & `quokka_sharp-0.0.9/quokka_sharp/qcmc.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from .encoding.qasm_parser import QASMparser
 from .encoding.qasm2cnf import QASM2CNF
 from .encoding.memory import ReturnValueThread, memory_monitor
 from queue import Queue
 from time import sleep
 from subprocess import Popen, PIPE, TimeoutExpired
 
+class Result:
+    def __init__(self, time, prob, memory):
+        self.time = time
+        self.prob = prob
+        self.memory = memory
+
 def QC2SAT(qasm_file, multi_or_single):
     wmc_file = qasm_file + ".cnf"
     prep_start = time.time()
     circuit = QASMparser(qasm_file, True)
     circuit.add_measurement(multi_or_single)
     cnf = QASM2CNF(circuit)
     cnf.leftProjectAllZero()
@@ -60,19 +66,17 @@
     encode_time, n = QC2SAT(qasm_file, multi_or_single)
     gpmc_time, prob = GPMC(toolpath, qasm_file, n, multi_or_single)
     
     time = encode_time + gpmc_time
     
     queue.put('stop')
     max_rss = monitor_thread.join()
-    
-    print(qasm_file.split("/")[-1], 
-            ' time:', time,
-            ' prob:', prob,
-            ' Max RSS:', max_rss / 1024 / 1024, "MB")
+    memory = max_rss / 1024 / 1024, "MB"
+    res = Result(time, prob, memory)
+    return res
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='QCMC: The Quantum Circuit simulator based on Model Counting from the Quokka-Sharp (Quokka#) package')
     parser.add_argument('toolpath')
     parser.add_argument('filename')
     parser.add_argument('-m', '--measurement', choices=['firstzero', 'allzero'])
     args = parser.parse_args()
```

### Comparing `quokka_sharp-0.0.8/quokka_sharp.egg-info/PKG-INFO` & `quokka_sharp-0.0.9/quokka_sharp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-sharp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quokka Sharp
 Author: System Verification Lab
 Author-email: j.mei@liacs.leidenuniv.nl
 Keywords: python,quantum circuits
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quokka_sharp-0.0.8/setup.py` & `quokka_sharp-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Quokka Sharp'
 LONG_DESCRIPTION = '''
                     Quokka Sharp for simulating and equivalence checking 
                     of quantum circuits based on weighted model counting.
                     You have to intall a weighted model counting tool first.
                     '''
```

