# Comparing `tmp/justai-3.2.8.tar.gz` & `tmp/justai-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.2.8.tar", last modified: Fri Apr  5 09:49:12 2024, max compression
+gzip compressed data, was "justai-3.2.9.tar", last modified: Fri Apr  5 11:22:35 2024, max compression
```

## Comparing `justai-3.2.8.tar` & `justai-3.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.954539 justai-3.2.8/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.8/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.8/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 09:49:12.954273 justai-3.2.8/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-05 09:49:11.000000 justai-3.2.8/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.946875 justai-3.2.8/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.8/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.948410 justai-3.2.8/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.8/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.8/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.8/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.949186 justai-3.2.8/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.8/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.8/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.8/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.950634 justai-3.2.8/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2833 2024-04-05 09:47:29.000000 justai-3.2.8/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.8/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.8/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.8/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.2.8/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.951978 justai-3.2.8/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.8/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.8/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.8/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.8/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.8/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.953220 justai-3.2.8/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.8/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.8/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.2.8/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    14332 2024-04-04 21:45:33.000000 justai-3.2.8/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.8/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 09:49:12.953664 justai-3.2.8/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-05 09:49:12.000000 justai-3.2.8/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-05 09:49:11.000000 justai-3.2.8/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-05 09:49:12.954597 justai-3.2.8/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.561756 justai-3.2.9/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.9/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.9/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 11:22:35.561535 justai-3.2.9/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-05 11:22:34.000000 justai-3.2.9/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.554285 justai-3.2.9/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.9/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.555878 justai-3.2.9/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.9/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.9/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.9/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.556505 justai-3.2.9/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.9/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.9/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.9/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.557916 justai-3.2.9/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2833 2024-04-05 09:47:29.000000 justai-3.2.9/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.9/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.9/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.9/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.2.9/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.559411 justai-3.2.9/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.9/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.9/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.9/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.9/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.9/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.560631 justai-3.2.9/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.9/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.9/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.2.9/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    14480 2024-04-05 11:22:16.000000 justai-3.2.9/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.9/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.560986 justai-3.2.9/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-05 11:22:34.000000 justai-3.2.9/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-05 11:22:35.561797 justai-3.2.9/setup.cfg
```

### Comparing `justai-3.2.8/LICENSE` & `justai-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/PKG-INFO` & `justai-3.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.8
+Version: 3.2.9
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.8
+Current version: 3.2.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.8/README.md` & `justai-3.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.8
+Current version: 3.2.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.8/justai/__init__.py` & `justai-3.2.9/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/agent/agent.py` & `justai-3.2.9/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/agent/message.py` & `justai-3.2.9/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/interactive/commands.py` & `justai-3.2.9/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/interactive/repl.py` & `justai-3.2.9/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/models/anthropic_models.py` & `justai-3.2.9/justai/models/anthropic_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/models/gguf_models.py` & `justai-3.2.9/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/models/model.py` & `justai-3.2.9/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/models/modelfactory.py` & `justai-3.2.9/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/models/openai_models.py` & `justai-3.2.9/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/tools/cache.py` & `justai-3.2.9/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/tools/display.py` & `justai-3.2.9/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/tools/log.py` & `justai-3.2.9/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/tools/prompts.py` & `justai-3.2.9/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/translator/languages.py` & `justai-3.2.9/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/translator/prompts.toml` & `justai-3.2.9/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai/translator/translator.py` & `justai-3.2.9/justai/translator/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,54 +56,57 @@
         segment_name = 'trans-unit' if self.version == '1.2' else 'segment'
 
         if self.version >= '2.0':
             root.attrib['trgLang'] = LANGUAGES.get(language)
 
         # Verzamel teksten als lijst van samengevoegde strings per <source>
         all_texts = []
-        translatable_texts = []
+        translatable = []
         for source in root.xpath('.//ns:source', namespaces=namespaces):
-            texts = collect_texts_from_element(source)
-            all_texts.append(texts)
+            texts_from_source_element = collect_texts_from_element(source)
+            all_texts.append(texts_from_source_element)
             # Verzamel alleen de teksten die ook echt vertaald moeten worden
-            translatable_text = "||".join(text for text in texts if is_translatable(text))
-            if translatable_text:
-                translatable_texts.append(translatable_text)
+            translatable_from_source_element = [text for text in texts_from_source_element if is_translatable(text)]
+            if translatable_from_source_element:
+                translatable.append("||".join(translatable_from_source_element))
         log.info('translate - all_texts', all_texts)
-        log.info('translate - translatable_texts', translatable_texts)
+        log.info('translate - translatable_texts', translatable)
 
-        # Vertaal de lijst van samengevoegde strings
-        translated_texts = self.do_translate(translatable_texts, language, string_cached=string_cached)
+        # Vertaal de lijst van met || samengevoegde strings
+        flattened_all_texts = self.do_translate(translatable, language, string_cached=string_cached)
 
-        # Zet nu de delen die niet vertaald hoefden te worden terug in de lijst
-        for i1, line in enumerate(all_texts):
-            if any(is_translatable(text) for text in line):
-                sc = len([l for l in line if is_translatable(l)])
-                tc = len(translated_texts[0].split("||"))
+        # Zet nu de vertaalde delen terug in all_texts
+        index_in_translated_texts = 0
+        for texts_from_source_element in all_texts:
+            translatable_from_source_element = [text for text in texts_from_source_element if is_translatable(text)]
+            if translatable_from_source_element:
+                translated_version = flattened_all_texts[index_in_translated_texts].split("||")
+
+                # Check
+                sc = len(translatable_from_source_element)
+                tc = len(translated_version)
                 if sc != tc:
                     log.error('translate - mismatch',
-                              f'Translated texts ({sc}) does not match number of source texts ({tc})')
-                    log.info('translate - line', line)
-                    log.info('translate - Original:', [l for l in line if is_translatable(l)])
-                    log.info('translate - Translated:', translated_texts[0].split("||"))
-                assert len([l for l in line if is_translatable(l)]) == len(
-                    translated_texts[0].split("||")), 'Mismatch see log'
+                              f'Source texts ({sc}) does not match number of translated texts ({tc})')
+                    log.info('translate - translatable_from_source_element:', translatable_from_source_element)
+                    log.info('translate - translated_version:', translated_version)
+                assert sc==tc, 'Mismatch see log'
 
-                translated = translated_texts.pop(0).split("||")
-                for index, text in enumerate(line):
+                for index, text in enumerate(texts_from_source_element):
                     if is_translatable(text):
-                        line[index] = translated.pop(0)
-        translated_texts = [item for sublist in all_texts for item in sublist]  # And flatten
+                        texts_from_source_element[index] = translated_version.pop(0)
+                index_in_translated_texts += 1
+        flattened_all_texts = [item for sublist in all_texts for item in sublist]  # And flatten
 
         # Plaats vertaalde teksten in nieuwe <target> elementen met behoud van structuur
         counter = [0]
         for segment in root.xpath(f'.//ns:{segment_name}', namespaces=namespaces):
             source = segment.xpath('.//ns:source', namespaces=namespaces)[0]
             target = etree.SubElement(segment, f'{{urn:oasis:names:tc:xliff:document:{self.version}}}target')
-            copy_structure_with_texts(source, target, translated_texts, counter)
+            copy_structure_with_texts(source, target, flattened_all_texts, counter)
 
         updated_xml = etree.tostring(root, pretty_print=True, xml_declaration=True, encoding='UTF-8').decode('utf-8')
         return updated_xml
 
     def do_translate(self, texts, language: str, string_cached=False):
         log = self.logger
 
@@ -160,18 +163,17 @@
 
                 # Zorg dat de vertaling dezelfde whitespace aan het begin en eind heeft als de bron
                 for i, (source_part, translation_part) in enumerate(zip(source_parts, translation_parts)):
                     if source_part.strip() and (source_part[0] == ' ' or source_part[-1] == ' '):
                         start_spaces = (len(source_part) - len(source_part.lstrip(' '))) * ' '
                         end_spaces = (len(source_part) - len(source_part.rstrip(' '))) * ' '
                         translation_parts[i] = start_spaces + translation_part.strip() + end_spaces
-                log.info('do_translate - translation_parts', source_parts)
+                log.info('do_translate - translation_parts', translation_parts)
                 translation = '||'.join(translation_parts)
 
-                log.info('', f'{count}. [{source}] -> [{translation}]')
                 count += 1
                 ratio = len(source) / len(translation)
                 if ratio >= 1.5 or ratio <= 0.7:
                     log.warning('', f'Vertaling van {source} naar {translation} is onverwacht lang of kort')
 
             cache.update(translation_dict)
             if string_cached:
```

### Comparing `justai-3.2.8/justai/translator/xliff.py` & `justai-3.2.9/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/justai.egg-info/PKG-INFO` & `justai-3.2.9/justai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.8
+Version: 3.2.9
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.8
+Current version: 3.2.9
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.8/justai.egg-info/SOURCES.txt` & `justai-3.2.9/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.2.8/pyproject.toml` & `justai-3.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.2.8"
+version = "3.2.9"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

