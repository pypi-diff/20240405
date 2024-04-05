# Comparing `tmp/diversity-0.1.19.tar.gz` & `tmp/diversity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diversity-0.1.19.tar", max compression
+gzip compressed data, was "diversity-0.1.2.tar", max compression
```

## Comparing `diversity-0.1.19.tar` & `diversity-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4027 2024-04-02 18:29:23.764260 diversity-0.1.19/README.md
--rw-r--r--   0        0        0      337 2024-04-02 18:31:59.889652 diversity-0.1.19/diversity/__init__.py
--rw-r--r--   0        0        0     1726 2023-11-01 21:29:51.363577 diversity-0.1.19/diversity/compression.py
--rw-r--r--   0        0        0     3371 2024-04-02 18:19:39.171871 diversity-0.1.19/diversity/functions.py
--rw-r--r--   0        0        0     3217 2023-11-14 16:35:10.728417 diversity-0.1.19/diversity/homogenization.py
--rw-r--r--   0        0        0      724 2023-11-01 21:29:53.363660 diversity-0.1.19/diversity/ngram_diversity.py
--rw-r--r--   0        0        0       84 2023-10-04 17:47:31.256275 diversity-0.1.19/diversity/patterns/__init__.py
--rw-r--r--   0        0        0     2155 2023-10-07 17:22:30.499800 diversity-0.1.19/diversity/patterns/part_of_speech.py
--rw-r--r--   0        0        0      821 2023-10-07 17:23:14.046690 diversity-0.1.19/diversity/patterns/token.py
--rw-r--r--   0        0        0       30 2023-10-10 18:40:51.809862 diversity-0.1.19/diversity/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-02-26 15:03:39.741528 diversity-0.1.19/diversity/utils/memoize.py
--rw-r--r--   0        0        0      454 2024-04-02 18:32:38.904055 diversity-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 diversity-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0     4027 2024-04-02 18:29:23.764260 diversity-0.1.2/README.md
+-rw-r--r--   0        0        0      337 2024-04-02 18:31:59.889652 diversity-0.1.2/diversity/__init__.py
+-rw-r--r--   0        0        0     1726 2023-11-01 21:29:51.363577 diversity-0.1.2/diversity/compression.py
+-rw-r--r--   0        0        0     3395 2024-04-05 13:35:39.273797 diversity-0.1.2/diversity/functions.py
+-rw-r--r--   0        0        0     3217 2023-11-14 16:35:10.728417 diversity-0.1.2/diversity/homogenization.py
+-rw-r--r--   0        0        0      724 2023-11-01 21:29:53.363660 diversity-0.1.2/diversity/ngram_diversity.py
+-rw-r--r--   0        0        0       84 2023-10-04 17:47:31.256275 diversity-0.1.2/diversity/patterns/__init__.py
+-rw-r--r--   0        0        0     2155 2023-10-07 17:22:30.499800 diversity-0.1.2/diversity/patterns/part_of_speech.py
+-rw-r--r--   0        0        0      821 2023-10-07 17:23:14.046690 diversity-0.1.2/diversity/patterns/token.py
+-rw-r--r--   0        0        0       30 2023-10-10 18:40:51.809862 diversity-0.1.2/diversity/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-02-26 15:03:39.741528 diversity-0.1.2/diversity/utils/memoize.py
+-rw-r--r--   0        0        0      453 2024-04-05 13:35:44.738997 diversity-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 diversity-0.1.2/PKG-INFO
```

### Comparing `diversity-0.1.19/README.md` & `diversity-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/compression.py` & `diversity-0.1.2/diversity/compression.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/functions.py` & `diversity-0.1.2/diversity/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Functions for extracting patterns and matching text to patterns. """
 
 import numpy as np
 import itertools
 from typing import List, Optional
 from tqdm import tqdm
-from pattern import token_patterns, get_pos, pos_patterns
+from patterns import token_patterns, get_pos, pos_patterns
 from nltk.tokenize import sent_tokenize
 
 def extract_patterns(text: List[str], 
                      n: int = 5,
                      top_n: int = 100
 ) -> dict:
     """ Extracts text and part-of-speech patterns from text input. 
@@ -58,15 +58,15 @@
     return text_matches
 
 
 def match_patterns(text: str, 
                    patterns: dict
 ) -> List[tuple]:
     """ Matches text to part-of-speech patterns extracted from the `extract_patterns` function.
-        Used to identify which patterns appears in a single input text. 
+        Given set of patterns, used to identify which patterns appears in a single input text. 
     Args:
         text (str): Text to match patterns to.
         patterns (dict): Dictionary of patterns and their corresponding text.
     Returns:
         List[tuple]: List of tuples with the pattern and the text that matched.
 
     Example Usage:
```

### Comparing `diversity-0.1.19/diversity/homogenization.py` & `diversity-0.1.2/diversity/homogenization.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/ngram_diversity.py` & `diversity-0.1.2/diversity/ngram_diversity.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/patterns/part_of_speech.py` & `diversity-0.1.2/diversity/patterns/part_of_speech.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/patterns/token.py` & `diversity-0.1.2/diversity/patterns/token.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/diversity/utils/memoize.py` & `diversity-0.1.2/diversity/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `diversity-0.1.19/PKG-INFO` & `diversity-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diversity
-Version: 0.1.19
+Version: 0.1.2
 Summary: 
 Author: Chantal Shaib
 Author-email: shaib.c@northeastern.edu
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

