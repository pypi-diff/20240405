# Comparing `tmp/FactScoreLite-0.2.1.tar.gz` & `tmp/FactScoreLite-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FactScoreLite-0.2.1.tar", last modified: Wed Apr  3 03:15:05 2024, max compression
+gzip compressed data, was "FactScoreLite-0.3.0.tar", last modified: Thu Apr  4 23:00:56 2024, max compression
```

## Comparing `FactScoreLite-0.2.1.tar` & `FactScoreLite-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/FactScoreLite/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/FactScoreLite/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/data/demons.json
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/data/demons_generation_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/FactScoreLite/openai_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/FactScoreLite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 03:15:05.000000 FactScoreLite-0.2.1/FactScoreLite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-03 03:15:05.000000 FactScoreLite-0.2.1/FactScoreLite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:15:05.000000 FactScoreLite-0.2.1/FactScoreLite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 03:15:05.000000 FactScoreLite-0.2.1/FactScoreLite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 03:15:05.000000 FactScoreLite-0.2.1/FactScoreLite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:15:05.166205 FactScoreLite-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/tests/test_atomic_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-03 03:14:55.000000 FactScoreLite-0.2.1/tests/test_openai_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:56.520270 FactScoreLite-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:56.516270 FactScoreLite-0.3.0/FactScoreLite/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:56.516270 FactScoreLite-0.3.0/FactScoreLite/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/data/demons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/data/demons_generation_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/FactScoreLite/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:56.520270 FactScoreLite-0.3.0/FactScoreLite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 23:00:56.000000 FactScoreLite-0.3.0/FactScoreLite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-04 23:00:56.000000 FactScoreLite-0.3.0/FactScoreLite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:00:56.000000 FactScoreLite-0.3.0/FactScoreLite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 23:00:56.000000 FactScoreLite-0.3.0/FactScoreLite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 23:00:56.000000 FactScoreLite-0.3.0/FactScoreLite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 23:00:56.520270 FactScoreLite-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 23:00:56.520270 FactScoreLite-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:56.520270 FactScoreLite-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/tests/test_atomic_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/tests/test_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-04 23:00:52.000000 FactScoreLite-0.3.0/tests/test_scorer.py
```

### Comparing `FactScoreLite-0.2.1/FactScoreLite/atomic_facts.py` & `FactScoreLite-0.3.0/FactScoreLite/atomic_facts.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,65 @@
 from .openai_agent import OpenAIAgent
 from . import configs
 import json
 
 
 class AtomicFactGenerator:
     def __init__(self):
+        # Examples (demonstrations) that is used in prompt generation
         self.demons = self.load_demons()
+        # To interact with OpenAI APIs
         self.openai_agent = OpenAIAgent()
 
-    def run(self, text):
+    def run(self, text: str) -> list:
+        """
+        Extracts atomic facts from a text.
+
+        Args:
+            text (str): The text to extract atomic facts from.
+
+        Returns:
+            list: A list of atomic facts and the associatated sentence extracted from the text.
+        """
+
         sentences = []
 
         initials = self.detect_initials(text)
         sentences = sent_tokenize(text)
         sentences = self.fix_sentence_splitter(sentences, initials)
 
         atoms = []
         for sent in sentences:
             atom = self.get_sentence_af(sent)
             atoms.append((sent, atom))
 
         return atoms
 
     def load_demons(self):
+        """
+        Load examples (demonstrations) from a JSON file.
+        This will be used in the prompt generation.
+
+        Returns:
+            list: A list of examples (demonstrations).
+        """
         with open(configs.demons_path, "r") as file:
             demons = json.load(file)
 
         return demons
 
-    def get_instructions(self):
-        # n = 8
+    def get_instructions(self) -> str:
+        """
+        Prepare instructions for the prompt generation.
+        Instructions include the examples given in the demons.json file.
+
+        Returns:
+            str: The instructions for the prompt generation.
+        """
+
         instructions = (
             "Please breakdown the following sentence into independent facts:\n\n"
         )
 
         for demon in self.demons:
             sentence = demon["Sentence"]
             facts = demon["Independent Facts"]
@@ -48,44 +74,82 @@
             for fact in facts:
                 instructions += "- {}\n".format(fact)
 
             instructions += "\n\n"
 
         return instructions
 
-    def get_sentence_af(self, sent):
+    def get_sentence_af(self, sent: str) -> list:
+        """
+        Gets atomic facts for a sentence using OpenAI APIs.
+
+        Args:
+            sent (str): The sentence to extract atomic facts from.
+
+        Returns:
+            list: A list of atomic facts extracted from the sentence.
+        """
         atoms = None
         instructions = self.get_instructions()
 
         prompt = instructions + f"Sentence: {sent}\nIndependent Facts:"
 
         output = self.openai_agent.generate(prompt)
         atoms = self.gpt_output_to_sentences(output)
 
         return atoms
 
-    def gpt_output_to_sentences(self, text):
+    def gpt_output_to_sentences(self, text: str) -> list:
+        """
+        Clears the output from GPT and returns a list of cleaned sentences.
+
+        Args:
+            text (str): The output from GPT.
+
+        Returns:
+            list: A list of cleaned sentences.
+        """
         sentences = text.split("- ")[1:]
         sentences = [
             sent.strip()[:-1] if sent.strip()[-1] == "\n" else sent.strip()
             for sent in sentences
         ]
-        if len(sentences) > 0:
-            if sentences[-1][-1] != ".":
-                sentences[-1] = sentences[-1] + "."
-        else:
-            sentences = []
+
+        sentences = [sent + "." if sent[-1] != "." else sent for sent in sentences]
 
         return sentences
 
-    def detect_initials(self, text):
+    def detect_initials(self, text: str) -> list:
+        """
+        Detects initials in the text.
+
+        Args:
+            text (str): The text to detect initials in.
+
+        Returns:
+            list: A list of detected initials.
+        """
         pattern = r"[A-Z]\. ?[A-Z]\."
         return re.findall(pattern, text)
 
-    def fix_sentence_splitter(self, sentences, initials):
+    def fix_sentence_splitter(self, sentences: list, initials: list) -> list:
+        """
+        Fixes sentence splitting issues based on detected initials, handling special cases.
+
+        Args:
+            sentences (list): List of sentences to fix.
+            initials (list): List of detected initials.
+
+        Returns:
+            list: Sentences with corrected splitting issues.
+
+        This method corrects sentence splitting issues by merging incorrectly split sentences
+        based on detected initials. It also addresses special cases such as sentences
+        containing only one word or starting with a lowercase letter to ensure proper formatting.
+        """
         for initial in initials:
             if not np.any([initial in sent for sent in sentences]):
                 alpha1, alpha2 = [
                     t.strip() for t in initial.split(".") if len(t.strip()) > 0
                 ]
                 for i, (sent1, sent2) in enumerate(zip(sentences, sentences[1:])):
                     if sent1.endswith(alpha1 + ".") and sent2.startswith(alpha2 + "."):
@@ -104,15 +168,15 @@
             if len(sent.split()) <= 1 and sent_idx == 0:
                 assert not combine_with_previous
                 combine_with_previous = True
                 results.append(sent)
             elif len(sent.split()) <= 1:
                 assert sent_idx > 0
                 results[-1] += " " + sent
-                combined_with_previous = False
+                combine_with_previous = False
             elif sent[0].isalpha() and not sent[0].isupper() and sent_idx > 0:
                 assert sent_idx > 0, results
                 results[-1] += " " + sent
                 combine_with_previous = False
             elif combine_with_previous:
                 assert sent_idx > 0
                 results[-1] += " " + sent
@@ -123,18 +187,18 @@
 
         return results
 
 
 if __name__ == "__main__":
     generator = AtomicFactGenerator()
     text = """
-To winterize your battery and prevent damage:
- 
- 1. **For the Li-ion battery**:
-  - Avoid storing the vehicle in temperatures below -13°F (-25°C) for more than seven days to prevent the Li-ion battery from freezing.
-  - Move the vehicle to a warm location if the outside temperature is -13°F (-25°C) or below, as it may freeze and be unable to charge or power the vehicle.
- 
- 2. **For the 12-volt battery**:
-  - Ensure it is fully charged during extremely cold weather conditions to prevent the battery fluid from freezing and possibly causing damage to the battery.
-""".strip()
+        To winterize your battery and prevent damage:
+        
+        1. **For the Li-ion battery**:
+        - Avoid storing the vehicle in temperatures below -13°F (-25°C) for more than seven days to prevent the Li-ion battery from freezing.
+        - Move the vehicle to a warm location if the outside temperature is -13°F (-25°C) or below, as it may freeze and be unable to charge or power the vehicle.
+        
+        2. **For the 12-volt battery**:
+        - Ensure it is fully charged during extremely cold weather conditions to prevent the battery fluid from freezing and possibly causing damage to the battery.
+        """.strip()
 
     print(generator.run(text))
```

### Comparing `FactScoreLite-0.2.1/FactScoreLite/data/demons.json` & `FactScoreLite-0.3.0/FactScoreLite/data/demons.json`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.2.1/FactScoreLite/data/demons_generation_prompt.txt` & `FactScoreLite-0.3.0/FactScoreLite/data/demons_generation_prompt.txt`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.2.1/FactScoreLite/openai_agent.py` & `FactScoreLite-0.3.0/FactScoreLite/openai_agent.py`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.2.1/LICENSE` & `FactScoreLite-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.2.1/tests/test_atomic_facts.py` & `FactScoreLite-0.3.0/tests/test_atomic_facts.py`

 * *Files identical despite different names*

### Comparing `FactScoreLite-0.2.1/tests/test_openai_agent.py` & `FactScoreLite-0.3.0/tests/test_openai_agent.py`

 * *Files identical despite different names*

