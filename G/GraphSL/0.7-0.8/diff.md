# Comparing `tmp/GraphSL-0.7.tar.gz` & `tmp/GraphSL-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSL-0.7.tar", last modified: Thu Apr  4 22:08:12 2024, max compression
+gzip compressed data, was "GraphSL-0.8.tar", last modified: Fri Apr  5 01:28:38 2024, max compression
```

## Comparing `GraphSL-0.7.tar` & `GraphSL-0.8.tar`

### file list

```diff
@@ -1,12 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 22:08:12.184435 GraphSL-0.7/
-drwxrwxrwx   0        0        0        0 2024-04-04 22:08:12.180382 GraphSL-0.7/GraphSL.egg-info/
--rw-rw-rw-   0        0        0      732 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 22:08:12.000000 GraphSL-0.7/GraphSL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.7/LICENSE
--rw-rw-rw-   0        0        0      732 2024-04-04 22:08:12.184435 GraphSL-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.7/README.md
--rw-rw-rw-   0        0        0       86 2024-04-04 22:08:12.186496 GraphSL-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1729 2024-04-04 22:08:07.000000 GraphSL-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.762250 GraphSL-0.8/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.693724 GraphSL-0.8/GraphSL/
+-rw-rw-rw-   0        0        0      628 2024-04-02 03:37:06.000000 GraphSL-0.8/GraphSL/Evaluation.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.711631 GraphSL-0.8/GraphSL/GNN/
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.719314 GraphSL-0.8/GraphSL/GNN/GCNSI/
+-rw-rw-rw-   0        0        0       41 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/__init__.py
+-rw-rw-rw-   0        0        0    10598 2024-04-04 22:13:16.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/main.py
+-rw-rw-rw-   0        0        0     2842 2024-04-03 23:42:30.000000 GraphSL-0.8/GraphSL/GNN/GCNSI/model.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.742178 GraphSL-0.8/GraphSL/GNN/IVGD/
+-rw-rw-rw-   0        0        0      185 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/IVGD/__init__.py
+-rw-rw-rw-   0        0        0     1592 2024-04-03 23:40:52.000000 GraphSL-0.8/GraphSL/GNN/IVGD/correction.py
+-rw-rw-rw-   0        0        0     4000 2024-03-30 18:14:05.000000 GraphSL-0.8/GraphSL/GNN/IVGD/earlystopping.py
+-rw-rw-rw-   0        0        0     6267 2024-04-03 23:40:52.000000 GraphSL-0.8/GraphSL/GNN/IVGD/i_deepis.py
+-rw-rw-rw-   0        0        0    16718 2024-04-04 22:13:43.000000 GraphSL-0.8/GraphSL/GNN/IVGD/main.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.746256 GraphSL-0.8/GraphSL/GNN/IVGD/model/
+-rw-rw-rw-   0        0        0     4840 2024-03-21 02:09:16.000000 GraphSL-0.8/GraphSL/GNN/IVGD/model/MLP.py
+-rw-rw-rw-   0        0        0       18 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/IVGD/model/__init__.py
+-rw-rw-rw-   0        0        0     2780 2024-03-30 20:31:33.000000 GraphSL-0.8/GraphSL/GNN/IVGD/preprocessing.py
+-rw-rw-rw-   0        0        0    16726 2024-03-30 21:24:24.000000 GraphSL-0.8/GraphSL/GNN/IVGD/training.py
+-rw-rw-rw-   0        0        0     3985 2024-04-05 00:03:14.000000 GraphSL-0.8/GraphSL/GNN/IVGD/validity_net.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.755664 GraphSL-0.8/GraphSL/GNN/SLVAE/
+-rw-rw-rw-   0        0        0       41 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/__init__.py
+-rw-rw-rw-   0        0        0    16056 2024-04-04 22:14:01.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/main.py
+-rw-rw-rw-   0        0        0    13014 2024-04-03 23:43:48.000000 GraphSL-0.8/GraphSL/GNN/SLVAE/model.py
+-rw-rw-rw-   0        0        0        0 2024-03-24 17:30:45.000000 GraphSL-0.8/GraphSL/GNN/__init__.py
+-rw-rw-rw-   0        0        0    22346 2024-04-04 22:12:39.000000 GraphSL-0.8/GraphSL/Prescribed.py
+-rw-rw-rw-   0        0        0       52 2024-04-05 00:09:46.000000 GraphSL-0.8/GraphSL/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.760193 GraphSL-0.8/GraphSL/data/
+-rw-rw-rw-   0        0        0       20 2024-04-05 00:02:34.000000 GraphSL-0.8/GraphSL/data/__init__.py
+-rw-rw-rw-   0        0        0     7110 2024-04-04 22:33:31.000000 GraphSL-0.8/GraphSL/data/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:38.709948 GraphSL-0.8/GraphSL.egg-info/
+-rw-rw-rw-   0        0        0      732 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 01:28:38.000000 GraphSL-0.8/GraphSL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.8/LICENSE
+-rw-rw-rw-   0        0        0      732 2024-04-05 01:28:38.763307 GraphSL-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.8/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-05 01:28:38.764241 GraphSL-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1729 2024-04-05 01:28:15.000000 GraphSL-0.8/setup.py
```

### Comparing `GraphSL-0.7/GraphSL.egg-info/PKG-INFO` & `GraphSL-0.8/GraphSL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.7
+Version: 0.8
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
-Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.6.tar.gz
+Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.8.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `GraphSL-0.7/LICENSE` & `GraphSL-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `GraphSL-0.7/PKG-INFO` & `GraphSL-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.7
+Version: 0.8
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
-Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.6.tar.gz
+Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.8.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `GraphSL-0.7/README.md` & `GraphSL-0.8/README.md`

 * *Files identical despite different names*

### Comparing `GraphSL-0.7/setup.py` & `GraphSL-0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'GraphSL',         # How you named your package folder (MyLib)
   packages = find_packages(),   # Chose the same as "name"
-  version = '0.7',      # Start with a small number and increase it with every change you make
+  version = '0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Graph Source Localization Approaches and Benchmark Datasets',   # Give a short description about your library
   author = 'Junxiang Wang',                   # Type in your name
   author_email = 'junxiang.wang@alumni.emory.edu',      # Type in your E-Mail
   url = 'https://xianggebenben.github.io/Junxiang_Wang.github.io/',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.6.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.8.tar.gz',    # I explain this later on
   keywords = ['Graph Diffusion', 'Graph Source Localization', 'Prescribed Methods', 'GNN Methods','Benchmark'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'networkx',
           'ndlib',
           'torch',
           'scikit-learn',
```

