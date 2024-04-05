# Comparing `tmp/humemai-0.0.0.tar.gz` & `tmp/humemai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humemai-0.0.0.tar", last modified: Thu Apr  4 13:55:21 2024, max compression
+gzip compressed data, was "humemai-1.0.0.tar", last modified: Fri Apr  5 15:12:11 2024, max compression
```

## Comparing `humemai-0.0.0.tar` & `humemai-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2024-04-04 13:55:21.081116 humemai-0.0.0/
--rw-rw-r--   0 tk        (1000) tk        (1000)    11357 2024-03-23 15:28:22.000000 humemai-0.0.0/LICENSE
--rw-r--r--   0 tk        (1000) tk        (1000)     2356 2024-04-04 13:55:21.081116 humemai-0.0.0/PKG-INFO
--rw-rw-r--   0 tk        (1000) tk        (1000)     1686 2024-03-26 18:11:22.000000 humemai-0.0.0/README.md
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2024-04-04 13:55:21.081116 humemai-0.0.0/humemai/
--rw-rw-r--   0 tk        (1000) tk        (1000)        0 2024-03-26 16:51:46.000000 humemai-0.0.0/humemai/__init__.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    29982 2024-04-02 11:53:03.000000 humemai-0.0.0/humemai/memory.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    14656 2024-03-23 15:28:22.000000 humemai-0.0.0/humemai/policy.py
--rw-rw-r--   0 tk        (1000) tk        (1000)     8651 2024-03-26 19:32:11.000000 humemai-0.0.0/humemai/utils.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2024-04-04 13:55:21.081116 humemai-0.0.0/humemai.egg-info/
--rw-r--r--   0 tk        (1000) tk        (1000)     2356 2024-04-04 13:55:21.000000 humemai-0.0.0/humemai.egg-info/PKG-INFO
--rw-rw-r--   0 tk        (1000) tk        (1000)      322 2024-04-04 13:55:21.000000 humemai-0.0.0/humemai.egg-info/SOURCES.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)        1 2024-04-04 13:55:21.000000 humemai-0.0.0/humemai.egg-info/dependency_links.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)       83 2024-04-04 13:55:21.000000 humemai-0.0.0/humemai.egg-info/requires.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)        8 2024-04-04 13:55:21.000000 humemai-0.0.0/humemai.egg-info/top_level.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)      710 2024-04-04 13:55:21.081116 humemai-0.0.0/setup.cfg
--rw-rw-r--   0 tk        (1000) tk        (1000)       69 2024-03-23 15:28:22.000000 humemai-0.0.0/setup.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2024-04-04 13:55:21.081116 humemai-0.0.0/test/
--rw-rw-r--   0 tk        (1000) tk        (1000)    42568 2024-03-26 11:34:46.000000 humemai-0.0.0/test/test_memory.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    29843 2024-03-26 10:53:31.000000 humemai-0.0.0/test/test_policy.py
--rw-rw-r--   0 tk        (1000) tk        (1000)      906 2024-03-26 10:53:52.000000 humemai-0.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 15:11:59.000000 humemai-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-05 15:12:11.207245 humemai-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-05 15:11:59.000000 humemai-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/humemai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29982 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14656 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-05 15:11:59.000000 humemai-1.0.0/humemai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/humemai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 15:12:11.000000 humemai-1.0.0/humemai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 15:12:11.211245 humemai-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:11:59.000000 humemai-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:12:11.207245 humemai-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    42568 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29843 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-05 15:11:59.000000 humemai-1.0.0/test/test_utils.py
```

### Comparing `humemai-0.0.0/LICENSE` & `humemai-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/PKG-INFO` & `humemai-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gymnasium>=0.27.1
-Requires-Dist: torch>=1.12.1
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: tqdm
-Requires-Dist: ipython>=8.20.0
-Requires-Dist: matplotlib>=3.8.2
 
 # humemai
 
 [![DOI](https://zenodo.org/badge/614376180.svg)](https://zenodo.org/doi/10.5281/zenodo.10876440)
 
 This repo hosts a package `humemai`, a human-like memory systems that are modeled with
 knowledge knoweldge graphs (KGs). At the moment they are nothing but a Python list of
@@ -32,15 +26,15 @@
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
   Systems"](https://doi.org/10.1609/aaai.v37i1.25075).
 - ["Capturing Dynamic Knowledge Graphs with Human-like Memory Systems by Reinforcement
-  Learning"]().
+  Learning"](<>).
 
 ## List of applications that use HumemAI
 
 ## pdoc documentation
 
 Click on [this link](https://humemai.github.io/humemai) to see the HTML rendered
 docstrings
```

### Comparing `humemai-0.0.0/README.md` & `humemai-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
   Systems"](https://doi.org/10.1609/aaai.v37i1.25075).
 - ["Capturing Dynamic Knowledge Graphs with Human-like Memory Systems by Reinforcement
-  Learning"]().
+  Learning"](<>).
 
 ## List of applications that use HumemAI
 
 ## pdoc documentation
 
 Click on [this link](https://humemai.github.io/humemai) to see the HTML rendered
 docstrings
```

### Comparing `humemai-0.0.0/humemai/memory.py` & `humemai-1.0.0/humemai/memory.py`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/humemai/policy.py` & `humemai-1.0.0/humemai/policy.py`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/humemai/utils.py` & `humemai-1.0.0/humemai/utils.py`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/humemai.egg-info/PKG-INFO` & `humemai-1.0.0/humemai.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: humemai
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Machine With Human-Like Memory Systems.
 Home-page: https://github.com/humemai/humemai
 Author: Taewoon Kim
 Author-email: info@humem.ai
 Project-URL: Bug Tracker, https://github.com/humemai/humemai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gymnasium>=0.27.1
-Requires-Dist: torch>=1.12.1
-Requires-Dist: PyYAML>=6.0
-Requires-Dist: tqdm
-Requires-Dist: ipython>=8.20.0
-Requires-Dist: matplotlib>=3.8.2
 
 # humemai
 
 [![DOI](https://zenodo.org/badge/614376180.svg)](https://zenodo.org/doi/10.5281/zenodo.10876440)
 
 This repo hosts a package `humemai`, a human-like memory systems that are modeled with
 knowledge knoweldge graphs (KGs). At the moment they are nothing but a Python list of
@@ -32,15 +26,15 @@
 
 ## List of academic papers that use HumemAI
 
 - ["A Machine With Human-Like Memory Systems"](https://arxiv.org/abs/2204.01611).
 - ["A Machine with Short-Term, Episodic, and Semantic Memory
   Systems"](https://doi.org/10.1609/aaai.v37i1.25075).
 - ["Capturing Dynamic Knowledge Graphs with Human-like Memory Systems by Reinforcement
-  Learning"]().
+  Learning"](<>).
 
 ## List of applications that use HumemAI
 
 ## pdoc documentation
 
 Click on [this link](https://humemai.github.io/humemai) to see the HTML rendered
 docstrings
```

### Comparing `humemai-0.0.0/setup.cfg` & `humemai-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = humemai
-version = 
+version = 1.0.0
 author = Taewoon Kim
 author_email = info@humem.ai
 description = A Machine With Human-Like Memory Systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/humemai/humemai
 project_urls =
```

### Comparing `humemai-0.0.0/test/test_memory.py` & `humemai-1.0.0/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/test/test_policy.py` & `humemai-1.0.0/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `humemai-0.0.0/test/test_utils.py` & `humemai-1.0.0/test/test_utils.py`

 * *Files identical despite different names*

