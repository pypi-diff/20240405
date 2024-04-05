# Comparing `tmp/AIPySdeAnalyzer-0.3.0.tar.gz` & `tmp/AIPySdeAnalyzer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPySdeAnalyzer-0.3.0.tar", last modified: Thu Mar 21 11:57:53 2024, max compression
+gzip compressed data, was "AIPySdeAnalyzer-0.3.1.tar", last modified: Fri Apr  5 13:05:04 2024, max compression
```

## Comparing `AIPySdeAnalyzer-0.3.0.tar` & `AIPySdeAnalyzer-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.151122 AIPySdeAnalyzer-0.3.0/
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.115257 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     4303 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      107 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-21 11:57:52.000000 AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-03-21 11:55:37.000000 AIPySdeAnalyzer-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     4303 2024-03-21 11:57:53.151122 AIPySdeAnalyzer-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.000616 AIPySdeAnalyzer-0.3.0/aipys_analyse/
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.051285 AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/__init__.py
--rw-rw-rw-   0        0        0     3059 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/loadParametres.py
--rw-rw-rw-   0        0        0     5903 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/setParameters.py
--rw-rw-rw-   0        0        0     4881 2024-03-18 09:47:02.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/SimInit.py
--rw-rw-rw-   0        0        0        0 2024-03-07 22:29:43.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.081789 AIPySdeAnalyzer-0.3.0/aipys_analyse/func/
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/func/__init__.py
--rw-rw-rw-   0        0        0     2633 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/func/mapSgRNA.py
--rw-rw-rw-   0        0        0     2364 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/func/unPacking.py
-drwxrwxrwx   0        0        0        0 2024-03-21 11:57:53.112763 AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/
--rw-rw-rw-   0        0        0     7929 2024-03-20 20:40:38.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/Simulate.py
--rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/__init__.py
--rw-rw-rw-   0        0        0     2342 2024-03-18 09:14:26.000000 AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/runSimulation.py
--rw-rw-rw-   0        0        0       42 2024-03-21 11:57:53.151122 AIPySdeAnalyzer-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-03-21 11:57:10.000000 AIPySdeAnalyzer-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.993665 AIPySdeAnalyzer-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.952434 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     4328 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 13:05:04.000000 AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-03-21 11:55:37.000000 AIPySdeAnalyzer-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4328 2024-04-05 13:05:04.990574 AIPySdeAnalyzer-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.836592 AIPySdeAnalyzer-0.3.1/aipys_analyse/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.865115 AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/__init__.py
+-rw-rw-rw-   0        0        0     3059 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/loadParametres.py
+-rw-rw-rw-   0        0        0     5903 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/setParameters.py
+-rw-rw-rw-   0        0        0     4881 2024-03-18 09:47:02.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/SimInit.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 22:29:43.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.916118 AIPySdeAnalyzer-0.3.1/aipys_analyse/func/
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/func/__init__.py
+-rw-rw-rw-   0        0        0     2633 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/func/mapSgRNA.py
+-rw-rw-rw-   0        0        0     2364 2024-03-07 19:26:44.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/func/unPacking.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:05:04.949442 AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/
+-rw-rw-rw-   0        0        0     7929 2024-03-20 20:40:38.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/Simulate.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 19:26:43.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/__init__.py
+-rw-rw-rw-   0        0        0     2391 2024-04-05 13:02:47.000000 AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/runSimulation.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:05:04.993665 AIPySdeAnalyzer-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-04-05 13:04:47.000000 AIPySdeAnalyzer-0.3.1/setup.py
```

### Comparing `AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/PKG-INFO` & `AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPySdeAnalyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: AI Powered Photoswitchable Screen analysis
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Requires-Dist: IPython
 Requires-Dist: openpyxl
 Requires-Dist: tables
 Requires-Dist: tqdm
 Requires-Dist: imageio
 Requires-Dist: numpyro
 Requires-Dist: bnlearn
+Requires-Dist: requests
 
 # CRISPR Screen Analysis Tool
 
 Gregor Mendel laid the foundation for the genetics field by demonstrating how traits are carried through generations unchanged. Building on Mendel's work, modern science, employing techniques like CRISPR and RNAi screens, delves into gene functions at a molecular level. Our program aids in analyzing CRISPR screens where cells mixed with different gRNAs are exposed to challenging conditions to assess a gene's influence on cellular "fitness". This tool encapsulates a part of the intricate journey from Mendel's observations to deciphering genetic blueprints through molecular biology.
 
 ## Overview
```

### Comparing `AIPySdeAnalyzer-0.3.0/AIPySdeAnalyzer.egg-info/SOURCES.txt` & `AIPySdeAnalyzer-0.3.1/AIPySdeAnalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/LICENSE` & `AIPySdeAnalyzer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/PKG-INFO` & `AIPySdeAnalyzer-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPySdeAnalyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: AI Powered Photoswitchable Screen analysis
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 Requires-Dist: IPython
 Requires-Dist: openpyxl
 Requires-Dist: tables
 Requires-Dist: tqdm
 Requires-Dist: imageio
 Requires-Dist: numpyro
 Requires-Dist: bnlearn
+Requires-Dist: requests
 
 # CRISPR Screen Analysis Tool
 
 Gregor Mendel laid the foundation for the genetics field by demonstrating how traits are carried through generations unchanged. Building on Mendel's work, modern science, employing techniques like CRISPR and RNAi screens, delves into gene functions at a molecular level. Our program aids in analyzing CRISPR screens where cells mixed with different gRNAs are exposed to challenging conditions to assess a gene's influence on cellular "fitness". This tool encapsulates a part of the intricate journey from Mendel's observations to deciphering genetic blueprints through molecular biology.
 
 ## Overview
```

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/loadParametres.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/loadParametres.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/CLI/setParameters.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/CLI/setParameters.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/SimInit.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/SimInit.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/func/mapSgRNA.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/func/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/func/unPacking.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/func/unPacking.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/Simulate.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/Simulate.py`

 * *Files identical despite different names*

### Comparing `AIPySdeAnalyzer-0.3.0/aipys_analyse/simulation/runSimulation.py` & `AIPySdeAnalyzer-0.3.1/aipys_analyse/simulation/runSimulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 RANDOM_SEED = 8927
 np.random.seed(RANDOM_SEED)
 
 class runSimulation(Simulate):
     def __init__(self,*args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.dfTall = self.dataReady()
+        self.dfTall, self.dfWide = self.dataReady()
         #self.dataHandle()
     
     def dataHandle(self):
         """
         dforig: 'sgRNA', 'count'
         dfQ2:'sgID', 'Q2_Reads'
         df_m:'sgID''count_sim'
@@ -46,18 +46,19 @@
     
     def dataReady(self):
         data_list = self.dataHandle()
         sampleId = MapSimMOI(data_list)
         df = pd.DataFrame(sampleId.df_map)
         df['Gene'] = [re.sub('_._.*','', sg) for sg in df.sgRNA.values]
         df.loc[df.sgRNA.str.contains('non'),'Gene'] = 'non'
+        dfWide = df.copy()
         df = pd.melt(df,id_vars = ['Gene','sgRNA'], value_vars=['df1_orig','df2_orig','df3_orig',
                                                      'df1', 'df2', 'df3','df1_M','df2_M','df3_M'])
         df["log"] = np.log(df["value"].values+2)
         df["condition"] = 1
         df.loc[df.variable.str.contains('orig'),"condition"] = 0
         df.loc[df.variable.str.contains('M'),"condition"] = 2
         dftall = df.rename(columns = ({"variable":"class","value":"readCount","log":"logRcount","condition":"tag"}))
         mapping = {0: "Ht0", 1: "Ht1", 2: "M"}
         dftall["class"] = dftall["tag"].replace(mapping)
-        return dftall
+        return dftall, dfWide
```

### Comparing `AIPySdeAnalyzer-0.3.0/setup.py` & `AIPySdeAnalyzer-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages,find_namespace_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPySdeAnalyzer",
-    version="0.3.0",
+    version="0.3.1",
     install_requires=required,
     packages=find_packages(include=['aipys_analyse','aipys_analyse.simulation','aipys_analyse.CLI','aipys_analyse.func']),
     entry_points={
         'console_scripts': [
         'updateParameters=aipys_analyse.CLI.setParameters:update_user_parameters',
         'load-parameters=aipys_analyse.CLI.loadParametres:main', 
             ],
```

