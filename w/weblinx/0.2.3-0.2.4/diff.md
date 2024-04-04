# Comparing `tmp/weblinx-0.2.3.tar.gz` & `tmp/weblinx-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblinx-0.2.3.tar", last modified: Mon Mar 25 22:27:00 2024, max compression
+gzip compressed data, was "weblinx-0.2.4.tar", last modified: Thu Apr  4 22:06:29 2024, max compression
```

## Comparing `weblinx-0.2.3.tar` & `weblinx-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.250287 weblinx-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-25 22:27:00.250287 weblinx-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-25 22:26:45.000000 weblinx-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 22:27:00.250287 weblinx-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-25 22:26:45.000000 weblinx-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.246287 weblinx-0.2.3/weblinx/
--rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.246287 weblinx-0.2.3/weblinx/_data/
--rw-r--r--   0 runner    (1001) docker     (127)    38206 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/_data/splits.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.246287 weblinx-0.2.3/weblinx/eval/
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/eval/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.250287 weblinx-0.2.3/weblinx/processing/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/dom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24575 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/processing/truncation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.250287 weblinx-0.2.3/weblinx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/envs.py
--rw-r--r--   0 runner    (1001) docker     (127)    33979 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-03-25 22:26:45.000000 weblinx-0.2.3/weblinx/utils/video.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 22:26:46.000000 weblinx-0.2.3/weblinx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:00.246287 weblinx-0.2.3/weblinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-25 22:27:00.000000 weblinx-0.2.3/weblinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-25 22:27:00.000000 weblinx-0.2.3/weblinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 22:27:00.000000 weblinx-0.2.3/weblinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-25 22:27:00.000000 weblinx-0.2.3/weblinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 22:27:00.000000 weblinx-0.2.3/weblinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.734953 weblinx-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 22:06:20.000000 weblinx-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-04 22:06:29.734953 weblinx-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-04 22:06:20.000000 weblinx-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:06:29.734953 weblinx-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 22:06:20.000000 weblinx-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/
+-rw-r--r--   0 runner    (1001) docker     (127)    47300 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    38206 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/_data/splits.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/dom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24575 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/processing/truncation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.734953 weblinx-0.2.4/weblinx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34112 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-04-04 22:06:20.000000 weblinx-0.2.4/weblinx/utils/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 22:06:21.000000 weblinx-0.2.4/weblinx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:06:29.730954 weblinx-0.2.4/weblinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 22:06:29.000000 weblinx-0.2.4/weblinx.egg-info/top_level.txt
```

### Comparing `weblinx-0.2.3/PKG-INFO` & `weblinx-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: weblinx
-Version: 0.2.3
+Version: 0.2.4
 Summary: The official weblinx library
 Home-page: https://github.com/McGill-NLP/weblinx
 Author: McGill NLP
 Author-email: weblinx@googlegroups.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: video
 Provides-Extra: processing
 Provides-Extra: eval
 Provides-Extra: all
+License-File: LICENSE
 
 <div align="center">
 
 # WebLINX
 
-| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) |
-| :--: | :--: | :--: |
-| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) |
-
-
-> **[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
-> *[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
-> _\*Equal contribution_
+| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) | [**📓Colab**](https://colab.research.google.com/github/McGill-NLP/weblinx/blob/main/examples/WebLINX_Colab_Notebook.ipynb) |
+| :--: | :--: | :--: | :--: |
+| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) | [**🏆Leaderboard**](https://paperswithcode.com/sota/conversational-web-navigation-on-weblinx) |
+
+<br>
+
+**[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
+*[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
+_\*Equal contribution_
 
 <img src="https://github.com/McGill-NLP/weblinx/raw/main/docs/assets/images/webnav.demo.svg" width="80%" alt="Sample conversation between a user and an agent" />
 
 </div>
 
 ### Installation
```

### Comparing `weblinx-0.2.3/README.md` & `weblinx-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 <div align="center">
 
 # WebLINX
 
-| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) |
-| :--: | :--: | :--: |
-| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) |
-
-
-> **[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
-> *[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
-> _\*Equal contribution_
+| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) | [**📓Colab**](https://colab.research.google.com/github/McGill-NLP/weblinx/blob/main/examples/WebLINX_Colab_Notebook.ipynb) |
+| :--: | :--: | :--: | :--: |
+| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) | [**🏆Leaderboard**](https://paperswithcode.com/sota/conversational-web-navigation-on-weblinx) |
+
+<br>
+
+**[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
+*[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
+_\*Equal contribution_
 
 <img src="https://github.com/McGill-NLP/weblinx/raw/main/docs/assets/images/webnav.demo.svg" width="80%" alt="Sample conversation between a user and an agent" />
 
 </div>
 
 ### Installation
```

### Comparing `weblinx-0.2.3/setup.py` & `weblinx-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/__init__.py` & `weblinx-0.2.4/weblinx/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/_data/splits.json` & `weblinx-0.2.4/weblinx/_data/splits.json`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/eval/__init__.py` & `weblinx-0.2.4/weblinx/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/eval/__main__.py` & `weblinx-0.2.4/weblinx/eval/__main__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/eval/metrics.py` & `weblinx-0.2.4/weblinx/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/processing/__init__.py` & `weblinx-0.2.4/weblinx/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/processing/dom.py` & `weblinx-0.2.4/weblinx/processing/dom.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/processing/intent.py` & `weblinx-0.2.4/weblinx/processing/intent.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/processing/outputs.py` & `weblinx-0.2.4/weblinx/processing/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     Given a uid_key for an element, retrieve additional information about the element from the HTML which can be used for evaluation.
 
     Extracts only the information needed for evaluation.
     """
     if not uid:
         return None
 
-    xpaths_dict = turn.get_xpaths_dict(cache_dir=cache_dir)
+    xpaths_dict = turn.get_xpaths_dict(cache_dir=cache_dir, uid_key=uid_key)
 
     if len(xpaths_dict) == 0:
         return None
 
     if uid not in xpaths_dict:
         return None
 
@@ -304,15 +304,15 @@
             else:
                 uid = None
 
         else:
             uid = None
 
         if uid is not None:
-            element = get_element_info(turn, uid)
+            element = get_element_info(turn, uid, uid_key=uid_key)
 
     return element
 
 
 def extract_action_from_turn(turn: "Turn", uid_key="data-webtasks-id"):
     """
     Creates an action from a turn in a demonstration (i.e. the ground truth action).
```

### Comparing `weblinx-0.2.3/weblinx/processing/prompt.py` & `weblinx-0.2.4/weblinx/processing/prompt.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/processing/truncation.py` & `weblinx-0.2.4/weblinx/processing/truncation.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/__init__.py` & `weblinx-0.2.4/weblinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/envs.py` & `weblinx-0.2.4/weblinx/utils/envs.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/format.py` & `weblinx-0.2.4/weblinx/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,14 +464,16 @@
         Whether to return the formatted element as a string or a dictionary.
 
     Returns
     -------
     formatted : str or dict
         A string or dictionary representing the uid.
     """
+    if turn.element is None:
+        raise ValueError(f"format_uid received a turn object with turn.element missing (None): {turn}")
     output = {"uid": turn.element.get("attributes", {}).get(uid_key, None)}
 
     return format_output_dictionary(output, return_as=return_as)
 
 
 def format_timestamp(
     turn,
```

### Comparing `weblinx-0.2.3/weblinx/utils/html.py` & `weblinx-0.2.4/weblinx/utils/html.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/hydra.py` & `weblinx-0.2.4/weblinx/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/recs.py` & `weblinx-0.2.4/weblinx/utils/recs.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/url.py` & `weblinx-0.2.4/weblinx/utils/url.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx/utils/video.py` & `weblinx-0.2.4/weblinx/utils/video.py`

 * *Files identical despite different names*

### Comparing `weblinx-0.2.3/weblinx.egg-info/PKG-INFO` & `weblinx-0.2.4/weblinx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: weblinx
-Version: 0.2.3
+Version: 0.2.4
 Summary: The official weblinx library
 Home-page: https://github.com/McGill-NLP/weblinx
 Author: McGill NLP
 Author-email: weblinx@googlegroups.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: video
 Provides-Extra: processing
 Provides-Extra: eval
 Provides-Extra: all
+License-File: LICENSE
 
 <div align="center">
 
 # WebLINX
 
-| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) |
-| :--: | :--: | :--: |
-| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) |
-
-
-> **[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
-> *[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
-> _\*Equal contribution_
+| [**🤗Dataset**](https://huggingface.co/datasets/McGill-NLP/WebLINX) | [**📄Paper**](https://arxiv.org/abs/2402.05930) | [**🌐Website**](https://mcgill-nlp.github.io/weblinx) | [**📓Colab**](https://colab.research.google.com/github/McGill-NLP/weblinx/blob/main/examples/WebLINX_Colab_Notebook.ipynb) |
+| :--: | :--: | :--: | :--: |
+| [**🤖Models**](https://huggingface.co/collections/McGill-NLP/weblinx-models-65c57d4afeeb282d1dcf8434) | [**💻Explorer**](https://huggingface.co/spaces/McGill-NLP/weblinx-explorer) | [**🐦Tweets**](https://twitter.com/sivareddyg/status/1755799365031965140) | [**🏆Leaderboard**](https://paperswithcode.com/sota/conversational-web-navigation-on-weblinx) |
+
+<br>
+
+**[WebLINX: Real-World Website Navigation with Multi-Turn Dialogue](https://mcgill-nlp.github.io/weblinx)**\
+*[Xing Han Lù*](https://xinghanlu.com), [Zdeněk Kasner*](https://kasnerz.github.io/), [Siva Reddy](https://sivareddy.in)*\
+_\*Equal contribution_
 
 <img src="https://github.com/McGill-NLP/weblinx/raw/main/docs/assets/images/webnav.demo.svg" width="80%" alt="Sample conversation between a user and an agent" />
 
 </div>
 
 ### Installation
```

### Comparing `weblinx-0.2.3/weblinx.egg-info/SOURCES.txt` & `weblinx-0.2.4/weblinx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 weblinx/__init__.py
 weblinx/version.py
 weblinx.egg-info/PKG-INFO
 weblinx.egg-info/SOURCES.txt
 weblinx.egg-info/dependency_links.txt
```

