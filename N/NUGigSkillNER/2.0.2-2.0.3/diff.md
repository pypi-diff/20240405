# Comparing `tmp/NUGigSkillNER-2.0.2.tar.gz` & `tmp/NUGigSkillNER-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NUGigSkillNER-2.0.2.tar", last modified: Fri Apr  5 01:02:46 2024, max compression
+gzip compressed data, was "NUGigSkillNER-2.0.3.tar", last modified: Fri Apr  5 01:28:05 2024, max compression
```

## Comparing `NUGigSkillNER-2.0.2.tar` & `NUGigSkillNER-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.241968 NUGigSkillNER-2.0.2/
--rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.201966 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/
--rw-rw-rw-   0        0        0     7268 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.220993 NUGigSkillNER-2.0.2/NuGigSkillNER/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/__init__.py
--rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/cleaner.py
--rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/general_params.py
--rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/matcher_class.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.225161 NUGigSkillNER-2.0.2/NuGigSkillNER/network/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/network/__init__.py
--rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/network/remote_db.py
--rw-rw-rw-   0        0        0     8098 2024-04-05 01:00:17.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/skill_extractor_class.py
--rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/text_class.py
--rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/utils.py
--rw-rw-rw-   0        0        0     7268 2024-04-05 01:02:46.241968 NUGigSkillNER-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.2/README.md
--rw-rw-rw-   0        0        0      169 2024-04-05 01:02:46.247239 NUGigSkillNER-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-04-05 01:02:05.000000 NUGigSkillNER-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.241793 NUGigSkillNER-2.0.2/skills_processor/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/skills_processor/__init__.py
--rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.2/skills_processor/create_new_skill.py
--rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/skills_processor/create_surf_db.py
--rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.2/skills_processor/create_token_dist.py
--rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.2/skills_processor/fetch_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.136765 NUGigSkillNER-2.0.3/
+-rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.096910 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/
+-rw-rw-rw-   0        0        0     7268 2024-04-05 01:28:04.000000 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-05 01:28:04.000000 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:28:04.000000 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-05 01:28:04.000000 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-05 01:28:04.000000 NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.122469 NUGigSkillNER-2.0.3/NuGigSkillNER/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/__init__.py
+-rw-rw-rw-   0        0        0     8839 2024-04-05 01:26:12.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/cleaner.py
+-rw-rw-rw-   0        0        0     5282 2024-04-05 01:26:22.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/general_params.py
+-rw-rw-rw-   0        0        0    11448 2024-04-05 01:25:11.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/matcher_class.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.124405 NUGigSkillNER-2.0.3/NuGigSkillNER/network/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/network/__init__.py
+-rw-rw-rw-   0        0        0     1954 2024-04-05 01:26:48.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/network/remote_db.py
+-rw-rw-rw-   0        0        0     8072 2024-04-05 01:26:34.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/skill_extractor_class.py
+-rw-rw-rw-   0        0        0    10053 2024-04-05 01:26:41.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/text_class.py
+-rw-rw-rw-   0        0        0     8835 2024-04-05 01:26:06.000000 NUGigSkillNER-2.0.3/NuGigSkillNER/utils.py
+-rw-rw-rw-   0        0        0     7268 2024-04-05 01:28:05.136765 NUGigSkillNER-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.3/README.md
+-rw-rw-rw-   0        0        0      169 2024-04-05 01:28:05.139509 NUGigSkillNER-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-04-05 01:27:23.000000 NUGigSkillNER-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:28:05.133975 NUGigSkillNER-2.0.3/skills_processor/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.3/skills_processor/__init__.py
+-rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.3/skills_processor/create_new_skill.py
+-rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.3/skills_processor/create_surf_db.py
+-rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.3/skills_processor/create_token_dist.py
+-rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.3/skills_processor/fetch_raw_data.py
```

### Comparing `NUGigSkillNER-2.0.2/LICENSE` & `NUGigSkillNER-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/PKG-INFO` & `NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.2
+Version: 2.0.3
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/SOURCES.txt` & `NUGigSkillNER-2.0.3/NUGigSkillNER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/cleaner.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # installed packs
 from nltk.stem import PorterStemmer
 # import en_core_web_lg
 # native packs
 from typing import List
 # my pack
-from skillNer.general_params import S_GRAM_REDUNDANT, LIST_PUNCTUATIONS
+from general_params import S_GRAM_REDUNDANT, LIST_PUNCTUATIONS
 
 
 # load nlp
 # nlp = en_core_web_lg.load()
 # list of cleaning functions names
 all_cleaning = [
     "remove_punctuation",
@@ -36,18 +36,18 @@
     Returns
     -------
     str
         returns a the provided text after removing all punctuations
 
     Examples
     --------
-    >>> from SkillNer.cleaner import remove_punctuation
-    >>> text = "Hello there, I am SkillNer! Annoation, annotation, annotation ..."
+    >>> from NuGigSkillNER.cleaner import remove_punctuation
+    >>> text = "Hello there, I am NuGigSkillNER! Annoation, annotation, annotation ..."
     >>> print(remove_punctuation(text))
-    Hello there  I am SkillNer  Annoation  annotation  annotation
+    Hello there  I am NuGigSkillNER  Annoation  annotation  annotation
     """
 
     for punc in list_punctuations:
         text = text.replace(punc, " ")
 
     # use .strip() to remove extra space in the begining/end of the text
     return text.strip()
@@ -70,15 +70,15 @@
     Returns
     -------
     str
         returns text after removing all redundant words provided in `list_redundant_words`
 
     Examples
     --------
-    >>> from SkillNer.cleaner import remove_redundant
+    >>> from NuGigSkillNER.cleaner import remove_redundant
     >>> text = "you have professional experience building React apps, you are familiar with version control using git and GitHub"
     >>> print(remove_redundant(text))
     building React apps,  familiar with version control using git and GitHub
     """
 
     for phrase in list_redundant_words:
         text = text.replace(phrase, "")
@@ -104,15 +104,15 @@
     Returns
     -------
     str
         returns text after stemming it.
 
     Examples
     --------
-    >>> from SkillNer.cleaner import stem_text
+    >>> from NuGigSkillNER.cleaner import stem_text
     >>> text = "you have professional experience building React apps, you are familiar with version control using git and GitHub"
     >>> print(stem_text(text))
     you have profession experi build react apps, you are familiar with version control use git and github
     """
 
     return " ".join([stemmer.stem(word) for word in text.split(" ")])
 
@@ -134,15 +134,15 @@
     Returns
     -------
     str
         returns text after lemming it.
 
     Examples
     --------
-    >>> from SkillNer.cleaner import lem_text
+    >>> from NuGigSkillNER.cleaner import lem_text
     >>> import spacy
     >>> nlp = spacy.load("en_core_web_sm")
     >>> text = "you have professional experience building React apps, you are familiar with version control using git and GitHub"
     >>> print(lem_text(text, nlp))
     you have professional experience building react app , you be familiar with version control use git and GitHub
     """
 
@@ -164,15 +164,15 @@
     Returns
     -------
     str
         returns text after removing all redundant spaces.
 
     Examples
     --------
-    >>> from SkillNer.cleaner import remove_extra_space
+    >>> from NuGigSkillNER.cleaner import remove_extra_space
     >>> text = " I am   sentence with   a lot of  annoying extra    spaces    ."
     >>> print(remove_extra_space(text))
     I am sentence with a lot of annoying extra spaces .
     """
 
     return " ".join(text.split())
 
@@ -205,15 +205,15 @@
     Returns
     -------
     List[int]
         returns a list of the indexes of words in phrase. An empty list is returned if phrase is not in text.
 
     Examples
     --------
-    >>> from SkillNer.cleaner import find_index_phrase
+    >>> from NuGigSkillNER.cleaner import find_index_phrase
     >>> text = "you have professional experience building React apps, you are familiar with version control using git and GitHub"
     >>> phrase = "experience building"
     >>> find_index_phrase(phrase, text)
     [3, 4]
     >>> find_index_phrase(phrase="Hello World", text)
     []
     """
@@ -274,15 +274,15 @@
         Returns
         -------
         str
             returns the text after applying all cleaning operations on it.
 
         Examples
         -------
-        >>> from skillNer.cleaner import Cleaner
+        >>> from NuGigSkillNER.cleaner import Cleaner
         >>> cleaner = Cleaner(
                         to_lowercase=True,
                         include_cleaning_functions=["remove_punctuation", "remove_extra_space"]
                     )
         >>> text = " I am   sentence with   a lot of  annoying extra    spaces    , and !! some ,., meaningless punctuation ?! .! AH AH AH"
         >>> cleaner(text)
         'i am sentence with a lot of annoying extra spaces and some meaningless punctuation ah ah ah'
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/general_params.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/general_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # native packs
 import os
 import json
 from posixpath import dirname
 # installed packs
 #
 # my packs
-from skillNer.network.remote_db import RemoteBucket
+from network.remote_db import RemoteBucket
 
 # mapping skill and color
 SKILL_TO_COLOR = {
     'Hard Skill': '#818CF8',
     'Soft Skill': '#F472B6',
     'Certification': "#552448"
 }
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/matcher_class.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/matcher_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # native packs
 from typing import List
 # installed packs
 #
 # my packs
-from skillNer.text_class import Text
+from NuGigSkillNER.text_class import Text
 
 
 class Matchers:
     """class to instanciate a matcher pipeline used to annotate text.
     """
 
     def __init__(
@@ -67,16 +67,16 @@
         Returns
         -------
         dict
             returns a dictionnary where the keys are the name of matchers and the values are the matchers
 
         Examples
         --------
-        >>> from skillNer.matcher_class import Matchers
-        >>> from skillNer.general_params import SKILL_DB
+        >>> from NuGigSkillNER.matcher_class import Matchers
+        >>> from NuGigSkillNER.general_params import SKILL_DB
         >>> import spacy
         >>> from spacy.matcher import PhraseMatcher
         >>> nlp = spacy.load('en_core_web_sm')
         >>> matcher_pipeline = Matchers(nlp, SKILL_DB, PhraseMatcher)
         >>> matcher_pipeline.load_matchers()
         loading full_matcher ...
         loading abv_matcher ...
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/network/remote_db.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/network/remote_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
 
         # save params
         self.token = token
         self.branch = branch
 
         # construct endpoint
-        self.end_point = f"https://raw.githubusercontent.com/AnasAito/SkillNER/{self.branch}"
+        self.end_point = f"https://raw.githubusercontent.com/AnasAito/NuGigSkillNER/{self.branch}"
         return
 
     def fetch_remote(
         self,
         db_name: str
     ) -> dict:
         """Function to fetch db
@@ -49,15 +49,15 @@
         Returns
         -------
         dict
             returns the db in format of a python dict object
 
         Examples
         --------
-        >>> from skillNer.network.remote_db import RemoteBucket
+        >>> from NuGigSkillNER.network.remote_db import RemoteBucket
         >>> buckets = RemoteBucket(
             branch="master"
         )
         >>> buckets.fetch_remote("SKILL_DB")
         ...
         """
         # request props
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/skill_extractor_class.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/skill_extractor_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # native packs
 #
 # installed packs
 from spacy import displacy
 # my packs
-from skillNer.text_class import Text
-from skillNer.matcher_class import Matchers, SkillsGetter
-from skillNer.utils import Utils
-from skillNer.general_params import SKILL_TO_COLOR
+from text_class import Text
+from matcher_class import Matchers, SkillsGetter
+from utils import Utils
+from general_params import SKILL_TO_COLOR
 
 
 class SkillExtractor:
     """Main class to annotate skills in a given text and visualize them.
     """
 
     def __init__(
@@ -74,16 +74,16 @@
         dict
             returns a dictionnary with the text that was used and the annotated skills (see example).
 
         Examples
         --------
         >>> import spacy
         >>> from spacy.matcher import PhraseMatcher
-        >>> from skillNer.skill_extractor_class import SkillExtractor
-        >>> from skillNer.general_params import SKILL_DB
+        >>> from NuGigSkillNER.skill_extractor_class import SkillExtractor
+        >>> from NuGigSkillNER.general_params import SKILL_DB
         >>> nlp = spacy.load('en_core_web_sm')
         >>> skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
         loading full_matcher ...
         loading abv_matcher ...
         loading full_uni_matcher ...
         loading low_form_matcher ...
         loading token_matcher ...
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/text_class.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/text_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # native packs
 from typing import List
 # installed packs
 #
 # my packs
-from skillNer.cleaner import Cleaner, stem_text, find_index_phrase
-from skillNer.general_params import S_GRAM_REDUNDANT
+from cleaner import Cleaner, stem_text, find_index_phrase
+from general_params import S_GRAM_REDUNDANT
 
 
 # building block of text
 class Word:
     """Main data structure to hold metadata of words
     """
 
@@ -21,15 +21,15 @@
         Parameters
         ----------
         word : str
             The word is given as string
 
         Examples
         --------
-        >>> from skillNer.text_class import Word
+        >>> from NuGigSkillNER.text_class import Word
         >>> word_obj = Word("Hello")
         """
 
         # immutable version of word
         self.word = word
 
         # attributes
@@ -51,15 +51,15 @@
         Returns
         -------
         dict
             dictionnary containing all metadata of object. Look at the example to see the returned keys
 
         Examples
         --------
-        >>> from skillNer.text_class import Word
+        >>> from NuGigSkillNER.text_class import Word
         >>> word_obj = Word("Hello")
         >>> word_obj.metadata().keys()
         dict_keys(['lemmed', 'stemmed', 'is_stop_word', 'is_matachable'])
         """
 
         return {
             "lemmed": self.lemmed,
@@ -75,15 +75,15 @@
         Returns
         -------
         str
             raw form of word
 
         Examples
         --------
-        >>> from skillNer.text_class import Word
+        >>> from NuGigSkillNER.text_class import Word
         >>> word_obj = Word("Hello")
         >>> print(word_obj)
         Hello
         """
         return self.word
 
     # give the len of the word
@@ -93,15 +93,15 @@
         Returns
         -------
         int
             returns the number of characters in word
 
         Examples
         --------
-        >>> from skillNer.text_class import Word
+        >>> from NuGigSkillNER.text_class import Word
         >>> word_obj = Word("Hello")
         >>> len(word_obj)
         5
         """
         return len(self.word)
 
 
@@ -124,15 +124,15 @@
         nlp : [type]
             An NLP object instanciated from Spacy.
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         """
 
         # immutable version of text
         self.immutable_text = text
 
         # transformed text: lower + punctuation + extra space
@@ -197,15 +197,15 @@
         str | List[str]
             return the stemmed text in the specified form by the argument `as_list`.
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         >>> text_obj.stemmed()
         'fluenci in both english and french is mandatori'
         >>> text_obj.stemmed(as_list=True)
         ['fluenci', 'in', 'both', 'english', 'and', 'french', 'is', 'mandatori']
         """
 
@@ -233,15 +233,15 @@
         str | List[str]
             return the lemmed text in the specified form by the argument `as_list`
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         >>> text_obj.lemmed()
         'fluency in both english and french be mandatory'
         >>> text_obj.lemmed(as_list=True)
         ['fluency', 'in', 'both', 'english', 'and', 'french', 'be', 'mandatory']
         """
 
@@ -261,15 +261,15 @@
         str
             returns the raw version of text
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         >>> print(text_obj)
         Fluency in both English and French is mandatory
         """
 
         return self.immutable_text
 
@@ -291,18 +291,18 @@
         Word
             returns thhe word object in the index-position
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         >>> text_obj[3]
-        <skillNer.text_class.Word at 0x1cf13a9bd60>
+        <NuGigSkillNER.text_class.Word at 0x1cf13a9bd60>
         >>> print(text_obj[3])
         english
         """
         return self.list_words[index]
 
     # len of a text is the number of words in it
     def __len__(self) -> int:
@@ -313,15 +313,15 @@
         int
             returns the number of words in text
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
+        >>> from NuGigSkillNER.text_class import Text
         >>> text_obj = Text("Fluency in both English and French is mandatory")
         >>> len(text_obj)
         8
         """
 
         return len(self.list_words)
 
@@ -342,16 +342,16 @@
             Returns a list of words where in each word the `start` and `end` 
             properties were filled by the starting and ending position of the word.
 
         Examples
         --------
         >>> import spacy
         >>> nlp = spacy.load('en_core_web_sm')
-        >>> from skillNer.text_class import Text
-        >>> list_words = Text.words_start_end_position("Hello World I am SkillNer")
+        >>> from NuGigSkillNER.text_class import Text
+        >>> list_words = Text.words_start_end_position("Hello World I am NuGigSkillNER")
         >>> word_1 = list_words[0]
         >>> print(word_1.start, word_1.end)
         0 5
         """
         # words in text
         list_words = []
```

### Comparing `NUGigSkillNER-2.0.2/NuGigSkillNER/utils.py` & `NUGigSkillNER-2.0.3/NuGigSkillNER/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import functools
 import math
 
 # installed packs
 import numpy as np
 import jellyfish
 # my packs
-from skillNer.text_class import Text
-from skillNer.general_params import TOKEN_DIST
+from text_class import Text
+from general_params import TOKEN_DIST
 from scipy.sparse import csr_matrix
 import pandas as pd
 
 class Utils:
     def __init__(self, nlp, skills_db):
         self.nlp = nlp
         self.skills_db = skills_db
```

### Comparing `NUGigSkillNER-2.0.2/PKG-INFO` & `NUGigSkillNER-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.2
+Version: 2.0.3
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.2/README.md` & `NUGigSkillNER-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/setup.py` & `NUGigSkillNER-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "spacy",
     "jellyfish",
     "scipy"
 ]
 
 setuptools.setup(
     name="NUGigSkillNER",
-    version="2.0.2",
+    version="2.0.3",
     author="Ethan Mandel",
     author_email="emandel2630@gmail.com",
     description="An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes",
     url="https://github.com/emandel2630/NUGigSkillNER",
     keywords=["skillNer", 'python', 'NLP', "NER",
               "skills-extraction", "job-description"],
     packages=setuptools.find_packages(),
```

### Comparing `NUGigSkillNER-2.0.2/skills_processor/create_new_skill.py` & `NUGigSkillNER-2.0.3/skills_processor/create_new_skill.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/skills_processor/create_surf_db.py` & `NUGigSkillNER-2.0.3/skills_processor/create_surf_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/skills_processor/create_token_dist.py` & `NUGigSkillNER-2.0.3/skills_processor/create_token_dist.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.2/skills_processor/fetch_raw_data.py` & `NUGigSkillNER-2.0.3/skills_processor/fetch_raw_data.py`

 * *Files identical despite different names*

