# Comparing `tmp/llm2vec-0.1.0.tar.gz` & `tmp/llm2vec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.0.tar", last modified: Thu Apr  4 15:27:48 2024, max compression
+gzip compressed data, was "llm2vec-0.1.1.tar", last modified: Thu Apr  4 20:26:27 2024, max compression
```

## Comparing `llm2vec-0.1.0.tar` & `llm2vec-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pbehna   (1447425) nogroup  (65534)        0 2024-04-04 15:27:48.818218 llm2vec-0.1.0/
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)     1067 2024-04-03 23:14:45.000000 llm2vec-0.1.0/LICENSE
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)      825 2024-04-04 15:27:48.818218 llm2vec-0.1.0/PKG-INFO
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)      257 2024-04-04 15:15:48.000000 llm2vec-0.1.0/README.md
-drwxr-xr-x   0 pbehna   (1447425) nogroup  (65534)        0 2024-04-04 15:27:48.814218 llm2vec-0.1.0/llm2vec/
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)       28 2024-04-03 23:15:41.000000 llm2vec-0.1.0/llm2vec/__init__.py
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)    10346 2024-04-03 23:15:41.000000 llm2vec-0.1.0/llm2vec/llm2vec.py
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)       21 2024-04-03 23:18:45.000000 llm2vec-0.1.0/llm2vec/version.py
-drwxr-xr-x   0 pbehna   (1447425) nogroup  (65534)        0 2024-04-04 15:27:48.818218 llm2vec-0.1.0/llm2vec.egg-info/
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)      825 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)      278 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)        1 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)        1 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)       43 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/requires.txt
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)        8 2024-04-04 15:27:48.000000 llm2vec-0.1.0/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)       79 2024-04-04 15:27:48.818218 llm2vec-0.1.0/setup.cfg
--rw-r--r--   0 pbehna   (1447425) nogroup  (65534)     1024 2024-04-04 15:26:20.000000 llm2vec-0.1.0/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 20:26:27.197601 llm2vec-0.1.1/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-04 20:24:53.000000 llm2vec-0.1.1/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4920 2024-04-04 20:26:27.197973 llm2vec-0.1.1/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4470 2024-04-04 20:25:54.000000 llm2vec-0.1.1/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 20:26:27.191287 llm2vec-0.1.1/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       28 2024-04-04 20:24:53.000000 llm2vec-0.1.1/llm2vec/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10433 2024-04-04 20:24:53.000000 llm2vec-0.1.1/llm2vec/llm2vec.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-04 20:26:17.000000 llm2vec-0.1.1/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 20:26:27.196855 llm2vec-0.1.1/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4920 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      278 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       43 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-04 20:26:27.000000 llm2vec-0.1.1/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-04 20:26:27.199122 llm2vec-0.1.1/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1024 2024-04-04 20:24:53.000000 llm2vec-0.1.1/setup.py
```

### Comparing `llm2vec-0.1.0/LICENSE` & `llm2vec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.0/llm2vec/llm2vec.py` & `llm2vec-0.1.1/llm2vec/llm2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,25 @@
             tokenized_q_length = len(tokenized_q["input_ids"][0])
     
         return f"{instruction.strip()} !@#$%^&*(){text}"
 
     def encode(self, sentences: Union[str, List[str]],
                batch_size: int = 32,
                show_progress_bar: bool = True,
-               convert_to_numpy: bool = True,
+               convert_to_numpy: bool = False,
                convert_to_tensor: bool = False,
     ):
         if isinstance(sentences[0],str) and isinstance(sentences[-1],int):
             sentences = [sentences]
         # required for MEDI version of MTEB
         if isinstance(sentences[0],list):
             concatenated_input_texts = []
             for sentence in sentences:
+                if len(sentence) == 1:
+                    sentence = [""] + sentence
                 assert isinstance(sentence[0], str)
                 assert isinstance(sentence[1], str)
                 concatenated_input_texts.append(self._convert_to_str(sentence[0], sentence[1]))
             sentences = concatenated_input_texts
         
         self.eval()
         show_progress_bar = True
```

### Comparing `llm2vec-0.1.0/setup.py` & `llm2vec-0.1.1/setup.py`

 * *Files identical despite different names*

