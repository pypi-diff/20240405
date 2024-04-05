# Comparing `tmp/simple-alto-parser-0.0.8.tar.gz` & `tmp/simple-alto-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-alto-parser-0.0.8.tar", last modified: Mon Jul 17 13:30:49 2023, max compression
+gzip compressed data, was "simple-alto-parser-0.0.9.tar", last modified: Fri Apr  5 13:56:41 2024, max compression
```

## Comparing `simple-alto-parser-0.0.8.tar` & `simple-alto-parser-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/simple_alto_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/dictionary_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/dictionary_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/nlp_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/pattern_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:41.491351 simple-alto-parser-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 13:56:34.000000 simple-alto-parser-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 13:56:34.000000 simple-alto-parser-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-05 13:56:41.491351 simple-alto-parser-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-05 13:56:34.000000 simple-alto-parser-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 13:56:41.491351 simple-alto-parser-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:41.491351 simple-alto-parser-0.0.9/simple_alto_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/alto_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/alto_file_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/alto_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/dictionary_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/dictionary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/nlp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/pattern_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 13:56:35.000000 simple-alto-parser-0.0.9/simple_alto_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:41.491351 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-05 13:56:41.000000 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-05 13:56:41.000000 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:56:41.000000 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 13:56:41.000000 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 13:56:41.000000 simple-alto-parser-0.0.9/simple_alto_parser.egg-info/top_level.txt
```

### Comparing `simple-alto-parser-0.0.8/LICENSE` & `simple-alto-parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/setup.cfg` & `simple-alto-parser-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/alto_file.py` & `simple-alto-parser-0.0.9/simple_alto_parser/alto_file.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/alto_file_exporter.py` & `simple-alto-parser-0.0.9/simple_alto_parser/alto_file_exporter.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/alto_file_parser.py` & `simple-alto-parser-0.0.9/simple_alto_parser/alto_file_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/base_parser.py` & `simple-alto-parser-0.0.9/simple_alto_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/dictionary_creator.py` & `simple-alto-parser-0.0.9/simple_alto_parser/dictionary_creator.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/dictionary_parser.py` & `simple-alto-parser-0.0.9/simple_alto_parser/dictionary_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/nlp_parser.py` & `simple-alto-parser-0.0.9/simple_alto_parser/nlp_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import os
 import webbrowser
 
-import spacy
-from spacy import displacy
-
 from simple_alto_parser import BaseParser
 from simple_alto_parser.base_parser import ParserMatch
 
 
 class AltoNLPParser(BaseParser):
 
     model = None
@@ -15,15 +12,15 @@
     last_parse_render = None
 
     def __init__(self, parser, model=None):
         super().__init__(parser)
         if model is None:
             model = "en_core_web_trf"
         self.model = model
-        self.spacy_nlp = spacy.load(self.model)
+        # self.spacy_nlp = spacy.load(self.model)
         self.last_parse_render = ''
 
     def parse(self, label=None):
         if type(label) is str:
             label = [label, ]
 
         html_render = ''
@@ -33,26 +30,27 @@
             line_id = 0
             for line in file.get_text_lines():
                 doc = self.spacy_nlp(line.get_text())
                 html_render += f'<strong><code>{line.get_text()}</code></strong><br/>'
                 for word in doc.ents:
                     if label is None or word.label_ == label:
                         self.matches.append(NLPMatch(file_id, line_id, word))
-                html_render += displacy.render(doc, style="ent") + "<br><hr>"
+                # html_render += displacy.render(doc, style="ent") + "<br><hr>"
                 line_id += 1
             html_render += '<br/>'
             file_id += 1
 
         self.last_parse_render = html_render
 
     def print_matches(self):
         path = os.path.abspath('temp.html')
         url = 'file://' + path
 
         with open(path, 'w') as f:
             f.write(self.last_parse_render)
         webbrowser.open(url)
 
+
 class NLPMatch(ParserMatch):
 
     def __init__(self, line_id, file_id, match):
         super().__init__(line_id, file_id, match)
```

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/pattern_parser.py` & `simple-alto-parser-0.0.9/simple_alto_parser/pattern_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser/utils.py` & `simple-alto-parser-0.0.9/simple_alto_parser/utils.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.8/simple_alto_parser.egg-info/SOURCES.txt` & `simple-alto-parser-0.0.9/simple_alto_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

