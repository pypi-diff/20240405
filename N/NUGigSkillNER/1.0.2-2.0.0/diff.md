# Comparing `tmp/NUGigSkillNER-1.0.2.tar.gz` & `tmp/NUGigSkillNER-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NUGigSkillNER-1.0.2.tar", last modified: Thu Aug 10 19:02:11 2023, max compression
+gzip compressed data, was "NUGigSkillNER-2.0.0.tar", last modified: Thu Apr  4 18:43:52 2024, max compression
```

## Comparing `NUGigSkillNER-1.0.2.tar` & `NUGigSkillNER-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     1106 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/LICENSE
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/NUGigSkillNER/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/__init__.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     8803 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/cleaner.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     5291 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/general_params.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)    11010 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/matcher_class.py
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/NUGigSkillNER/network/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/network/__init__.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     1944 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/network/remote_db.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     4590 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/skill_extractor_class.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)    10005 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/text_class.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     8853 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/utils.py
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/NUGigSkillNER/visualizer/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/visualizer/__init__.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     4062 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/NUGigSkillNER/visualizer/phrase_class.py
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     7127 2023-08-10 19:02:11.000000 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/PKG-INFO
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)      708 2023-08-10 19:02:11.000000 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/SOURCES.txt
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)        1 2023-08-10 19:02:11.000000 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/dependency_links.txt
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)       40 2023-08-10 19:02:11.000000 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/requires.txt
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)       31 2023-08-10 19:02:11.000000 NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/top_level.txt
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     7127 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/PKG-INFO
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     6506 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/README.md
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)      160 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/setup.cfg
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)      809 2023-08-10 19:01:53.000000 NUGigSkillNER-1.0.2/setup.py
-drwxr-xr-x   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 19:02:11.567368 NUGigSkillNER-1.0.2/skills_processor/
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)        0 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/skills_processor/__init__.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     4377 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/skills_processor/create_surf_db.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)      773 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/skills_processor/create_token_dist.py
--rw-r--r--   0 emandel2630  (1000) emandel2630  (1000)     1536 2023-08-10 18:44:45.000000 NUGigSkillNER-1.0.2/skills_processor/fetch_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/
+-rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.710717 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/
+-rw-rw-rw-   0        0        0     7268 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7268 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.0/README.md
+-rw-rw-rw-   0        0        0      169 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-04-04 18:33:46.000000 NUGigSkillNER-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.718710 NUGigSkillNER-2.0.0/skillNer/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/__init__.py
+-rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/cleaner.py
+-rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/general_params.py
+-rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.0/skillNer/matcher_class.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.719913 NUGigSkillNER-2.0.0/skillNer/network/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/network/__init__.py
+-rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/network/remote_db.py
+-rw-rw-rw-   0        0        0     8036 2024-02-20 20:51:07.000000 NUGigSkillNER-2.0.0/skillNer/skill_extractor_class.py
+-rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.0/skillNer/text_class.py
+-rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.723548 NUGigSkillNER-2.0.0/skillNer/visualizer/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/__init__.py
+-rw-rw-rw-   0        0        0     3159 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/html_elements.py
+-rw-rw-rw-   0        0        0     7192 2024-02-20 20:50:59.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/phrase_class.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/skills_processor/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skills_processor/__init__.py
+-rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.0/skills_processor/create_new_skill.py
+-rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skills_processor/create_surf_db.py
+-rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.0/skills_processor/create_token_dist.py
+-rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.0/skills_processor/fetch_raw_data.py
```

### Comparing `NUGigSkillNER-1.0.2/LICENSE` & `NUGigSkillNER-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-Copyright (c) 2021, Anas AIT AOMAR & Badr MOUFAD.
-All rights reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+MIT License
+Copyright (c) 2021, Anas AIT AOMAR & Badr MOUFAD.
+All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/cleaner.py` & `NUGigSkillNER-2.0.0/skillNer/cleaner.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/general_params.py` & `NUGigSkillNER-2.0.0/skillNer/general_params.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/matcher_class.py` & `NUGigSkillNER-2.0.0/skillNer/matcher_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,46 +226,61 @@
         nlp
     ):
 
         # param
         self.nlp = nlp
         return
 
+    
+    def get_lemmed_text(
+            self,
+        text_obj: Text,
+    ):
+        return self.nlp(text_obj.lemmed())
+        
+
     def get_full_match_skills(
         self,
         text_obj: Text,
         matcher
     ):
 
         skills = []
         doc = self.nlp(text_obj.lemmed())
 
+
         for match_id, start, end in matcher(doc):
             id_ = matcher.vocab.strings[match_id]
             # add full_match to store
             skills.append({'skill_id': id_,
                            'doc_node_value': str(doc[start:end]),
                            'score': 1,
                            'doc_node_id': list(range(start, end))})
+            
             # mutate text tokens metadata (unmatch attr)
             for token in text_obj[start:end]:
                 token.is_matchable = False
 
+
         return skills, text_obj
 
     def get_abv_match_skills(
         self,
         text_obj: Text,
         matcher
     ):
         skills = []
 
         doc = self.nlp(text_obj.abv_text)
         for match_id, start, end in matcher(doc):
             id_ = matcher.vocab.strings[match_id]
+
+            if start >=len(text_obj)-1:
+                break
+
             if text_obj[start].is_matchable:
                 skills.append({'skill_id': id_,
                                'score': 1,
                                'doc_node_value': str(doc[start:end]),
                                'doc_node_id': [start]})
                 # mutate matched tokens
                 for token in text_obj[start:end]:
@@ -280,14 +295,18 @@
     ):
 
         skills = []
 
         doc = self.nlp(text_obj.transformed_text)
         for match_id, start, end in matcher(doc):
             id_ = matcher.vocab.strings[match_id]
+
+            if start >=len(text_obj)-1:
+                break
+
             if text_obj[start].is_matchable:
                 skills.append({'skill_id': id_+'_fullUni',
                                'score': 1,
                                'doc_node_value': str(doc[start:end]),
                                'doc_node_id': [start],
                                'type': 'full_uni'})
 
@@ -301,18 +320,23 @@
 
         skills_full = []
         skills = []
         sub_matches = []
         full_matches = []
 
         doc = self.nlp(text_obj.lemmed())
+        
         for match_id, start, end in matcher(doc):
             id_ = matcher.vocab.strings[match_id]
 
             # add
+
+            if start >=len(text_obj)-1:
+                break
+
             if text_obj[start].is_matchable:
                 skills.append({'skill_id': id_+'_oneToken',
                                'doc_node_value': str(doc[start:end]),
                                'doc_node_id': [start],
                                'type': 'one_token'})
 
         return skills
@@ -326,14 +350,17 @@
         skills = []
         doc = self.nlp(text_obj.stemmed())
 
         for match_id, start, end in matcher(doc):
             id_ = matcher.vocab.strings[match_id]
             # handle skill in the end of phrase
             start = start if start < len(text_obj) else start - 1
+            if start >=len(text_obj)-1:
+                break
+            
             if text_obj[start].is_matchable:
                 skills.append({'skill_id': id_+'_lowSurf',
                                'doc_node_value': str(doc[start:end]),
                                'doc_node_id': list(range(start, end)),
                                'type': 'lw_surf'})
 
         return skills, text_obj
```

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/network/remote_db.py` & `NUGigSkillNER-2.0.0/skillNer/network/remote_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/text_class.py` & `NUGigSkillNER-2.0.0/skillNer/text_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
                 "remove_punctuation",
                 "remove_extra_space"
             ],
             to_lowercase=False
         )
 
         self.transformed_text = cleaner(text).lower()
+
         # abv version
         self.abv_text = cleaner(text)
 
         # list that holds all words within text
         self.list_words = []
 
         # construct list of words and create meta data object
```

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER/utils.py` & `NUGigSkillNER-2.0.0/skillNer/utils.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/PKG-INFO` & `NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,180 +1,177 @@
-Metadata-Version: 2.1
-Name: NUGigSkillNER
-Version: 1.0.2
-Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
-Home-page: https://github.com/emandel2630/NUGigSkillNER
-Author: Ethan Mandel
-Author-email: emandel2630@gmail.com
-License: UNKNOWN
-Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
-
-[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
-
-----------------------
-
-
-[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
-
-SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
-
-Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
-
-
-
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
-
-
-## Installation
-
-It is easy to get started with **SkillNer** and take advantage of its features.
-
-1. First, install **SkillNer** through the ``pip``
-
-```bash
-pip install skillNer
-```
-
-2. Next, run the following command to install ``spacy en_core_web_lg ``
-which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
-customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
-
-```bash
-python -m spacy download en_core_web_lg
-```
-
-**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
-
-
-## Example of usage
-
-With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
-
-Let’s say you want to extract skills from the following job posting:
-
-    “You are a Python developer with a solid experience in web development and can manage projects. 
-    You quickly adapt to new environments and speak fluently English and French”
-
-### Annotating skills
-
-We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
-
-**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
-
-
-
-```python
-# imports
-import spacy
-from spacy.matcher import PhraseMatcher
-
-# load default skills data base
-from skillNer.general_params import SKILL_DB
-# import skill extractor
-from skillNer.skill_extractor_class import SkillExtractor
-
-# init params of skill extractor
-nlp = spacy.load("en_core_web_lg")
-# init skill extractor
-skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
-
-# extract skills from job_description
-job_description = """
-You are a Python developer with a solid experience in web development
-and can manage projects. You quickly adapt to new environments
-and speak fluently English and French
-"""
-
-annotations = skill_extractor.annotate(job_description)
-
-```
-
-
-
-### Exploit annotations
-
-Voilà! Now you can inspect results by rendering the text with the annotated skills.
-You can acheive that through the ``.describe`` method. Note that the output of this method is 
-litteraly an HTML document that gets rendered in your notebook.
-
-
-<p align="center">
-    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
-</p>
-
-
-Besides, you can use the raw result of the annotations. 
-Below is the value of the ``annotations`` variable from the code above.
-
-
-```python
-# output
-{
-    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
-    'results': {
-        'full_matches': [
-            {
-                'skill_id': 'KS122Z36QK3N5097B5JH', 
-                'doc_node_value': 'web development', 
-                'score': 1, 'doc_node_id': [10, 11]
-            }
-        ], '
-        ngram_scored': [
-            {
-                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
-                'doc_node_id': [3], 
-                'doc_node_value': 'python', 
-                'type': 'fullUni', 
-                'score': 1, 
-                'len': 1
-            }, 
-        # the other annotated skills
-        # ...
-        ]
-    }
-}
-```
-
-# Contribure
-
-SkillNer is the first **Open Source** skill extractor. 
-Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
-
-We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
-make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
-and broaden its usage. 
-
-
-You can contribute to SkillNer either by
-
-1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
-
-2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
-
-
-3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
-
-
-
-Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
-
-
-Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
-
-
-## Useful links
-
-- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
-- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
-- [Test our Demo](https://share.streamlit.io/anasaito/skillner_demo/index.py) to see some of SkillNer capabilities
-
+Metadata-Version: 2.1
+Name: NUGigSkillNER
+Version: 2.0.0
+Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
+Home-page: https://github.com/emandel2630/NUGigSkillNER
+Author: Ethan Mandel
+Author-email: emandel2630@gmail.com
+Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
+
+[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
+
+----------------------
+
+
+[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
+
+SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
+
+Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
+
+
+
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
+
+
+## Installation
+
+It is easy to get started with **SkillNer** and take advantage of its features.
+
+1. First, install **SkillNer** through the ``pip``
+
+```bash
+pip install skillNer
+```
+
+2. Next, run the following command to install ``spacy en_core_web_lg ``
+which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
+customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
+
+```bash
+python -m spacy download en_core_web_lg
+```
+
+**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
+
+
+## Example of usage
+
+With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
+
+Let’s say you want to extract skills from the following job posting:
+
+    “You are a Python developer with a solid experience in web development and can manage projects. 
+    You quickly adapt to new environments and speak fluently English and French”
+
+### Annotating skills
+
+We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
+
+**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
+
+
+
+```python
+# imports
+import spacy
+from spacy.matcher import PhraseMatcher
+
+# load default skills data base
+from skillNer.general_params import SKILL_DB
+# import skill extractor
+from skillNer.skill_extractor_class import SkillExtractor
+
+# init params of skill extractor
+nlp = spacy.load("en_core_web_lg")
+# init skill extractor
+skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
+
+# extract skills from job_description
+job_description = """
+You are a Python developer with a solid experience in web development
+and can manage projects. You quickly adapt to new environments
+and speak fluently English and French
+"""
+
+annotations = skill_extractor.annotate(job_description)
+
+```
+
+
+
+### Exploit annotations
+
+Voilà! Now you can inspect results by rendering the text with the annotated skills.
+You can acheive that through the ``.describe`` method. Note that the output of this method is 
+litteraly an HTML document that gets rendered in your notebook.
+
+
+<p align="center">
+    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
+</p>
+
+
+Besides, you can use the raw result of the annotations. 
+Below is the value of the ``annotations`` variable from the code above.
+
+
+```python
+# output
+{
+    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
+    'results': {
+        'full_matches': [
+            {
+                'skill_id': 'KS122Z36QK3N5097B5JH', 
+                'doc_node_value': 'web development', 
+                'score': 1, 'doc_node_id': [10, 11]
+            }
+        ], '
+        ngram_scored': [
+            {
+                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
+                'doc_node_id': [3], 
+                'doc_node_value': 'python', 
+                'type': 'fullUni', 
+                'score': 1, 
+                'len': 1
+            }, 
+        # the other annotated skills
+        # ...
+        ]
+    }
+}
+```
+
+# Contribure
+
+SkillNer is the first **Open Source** skill extractor. 
+Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
+
+We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
+make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
+and broaden its usage. 
+
+
+You can contribute to SkillNer either by
+
+1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
+
+2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
+
+
+3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
+
+
+
+Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
+
+
+Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
+
+
+## Useful links
+
+- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
+- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
+- [Test our Demo](https://share.streamlit.io/anasaito/skillner_demo/index.py) to see some of SkillNer capabilities
```

### Comparing `NUGigSkillNER-1.0.2/NUGigSkillNER.egg-info/SOURCES.txt` & `NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-NUGigSkillNER/__init__.py
-NUGigSkillNER/cleaner.py
-NUGigSkillNER/general_params.py
-NUGigSkillNER/matcher_class.py
-NUGigSkillNER/skill_extractor_class.py
-NUGigSkillNER/text_class.py
-NUGigSkillNER/utils.py
 NUGigSkillNER.egg-info/PKG-INFO
 NUGigSkillNER.egg-info/SOURCES.txt
 NUGigSkillNER.egg-info/dependency_links.txt
 NUGigSkillNER.egg-info/requires.txt
 NUGigSkillNER.egg-info/top_level.txt
-NUGigSkillNER/network/__init__.py
-NUGigSkillNER/network/remote_db.py
-NUGigSkillNER/visualizer/__init__.py
-NUGigSkillNER/visualizer/phrase_class.py
+skillNer/__init__.py
+skillNer/cleaner.py
+skillNer/general_params.py
+skillNer/matcher_class.py
+skillNer/skill_extractor_class.py
+skillNer/text_class.py
+skillNer/utils.py
+skillNer/network/__init__.py
+skillNer/network/remote_db.py
+skillNer/visualizer/__init__.py
+skillNer/visualizer/html_elements.py
+skillNer/visualizer/phrase_class.py
 skills_processor/__init__.py
+skills_processor/create_new_skill.py
 skills_processor/create_surf_db.py
 skills_processor/create_token_dist.py
 skills_processor/fetch_raw_data.py
```

### Comparing `NUGigSkillNER-1.0.2/PKG-INFO` & `NUGigSkillNER-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,180 +1,177 @@
-Metadata-Version: 2.1
-Name: NUGigSkillNER
-Version: 1.0.2
-Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
-Home-page: https://github.com/emandel2630/NUGigSkillNER
-Author: Ethan Mandel
-Author-email: emandel2630@gmail.com
-License: UNKNOWN
-Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
-
-[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
-
-----------------------
-
-
-[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
-
-SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
-
-Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
-
-
-
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
-
-
-## Installation
-
-It is easy to get started with **SkillNer** and take advantage of its features.
-
-1. First, install **SkillNer** through the ``pip``
-
-```bash
-pip install skillNer
-```
-
-2. Next, run the following command to install ``spacy en_core_web_lg ``
-which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
-customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
-
-```bash
-python -m spacy download en_core_web_lg
-```
-
-**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
-
-
-## Example of usage
-
-With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
-
-Let’s say you want to extract skills from the following job posting:
-
-    “You are a Python developer with a solid experience in web development and can manage projects. 
-    You quickly adapt to new environments and speak fluently English and French”
-
-### Annotating skills
-
-We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
-
-**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
-
-
-
-```python
-# imports
-import spacy
-from spacy.matcher import PhraseMatcher
-
-# load default skills data base
-from skillNer.general_params import SKILL_DB
-# import skill extractor
-from skillNer.skill_extractor_class import SkillExtractor
-
-# init params of skill extractor
-nlp = spacy.load("en_core_web_lg")
-# init skill extractor
-skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
-
-# extract skills from job_description
-job_description = """
-You are a Python developer with a solid experience in web development
-and can manage projects. You quickly adapt to new environments
-and speak fluently English and French
-"""
-
-annotations = skill_extractor.annotate(job_description)
-
-```
-
-
-
-### Exploit annotations
-
-Voilà! Now you can inspect results by rendering the text with the annotated skills.
-You can acheive that through the ``.describe`` method. Note that the output of this method is 
-litteraly an HTML document that gets rendered in your notebook.
-
-
-<p align="center">
-    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
-</p>
-
-
-Besides, you can use the raw result of the annotations. 
-Below is the value of the ``annotations`` variable from the code above.
-
-
-```python
-# output
-{
-    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
-    'results': {
-        'full_matches': [
-            {
-                'skill_id': 'KS122Z36QK3N5097B5JH', 
-                'doc_node_value': 'web development', 
-                'score': 1, 'doc_node_id': [10, 11]
-            }
-        ], '
-        ngram_scored': [
-            {
-                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
-                'doc_node_id': [3], 
-                'doc_node_value': 'python', 
-                'type': 'fullUni', 
-                'score': 1, 
-                'len': 1
-            }, 
-        # the other annotated skills
-        # ...
-        ]
-    }
-}
-```
-
-# Contribure
-
-SkillNer is the first **Open Source** skill extractor. 
-Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
-
-We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
-make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
-and broaden its usage. 
-
-
-You can contribute to SkillNer either by
-
-1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
-
-2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
-
-
-3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
-
-
-
-Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
-
-
-Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
-
-
-## Useful links
-
-- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
-- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
-- [Test our Demo](https://share.streamlit.io/anasaito/skillner_demo/index.py) to see some of SkillNer capabilities
-
+Metadata-Version: 2.1
+Name: NUGigSkillNER
+Version: 2.0.0
+Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
+Home-page: https://github.com/emandel2630/NUGigSkillNER
+Author: Ethan Mandel
+Author-email: emandel2630@gmail.com
+Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
+
+[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
+
+----------------------
+
+
+[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
+
+SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
+
+Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
+
+
+
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
+
+
+## Installation
+
+It is easy to get started with **SkillNer** and take advantage of its features.
+
+1. First, install **SkillNer** through the ``pip``
+
+```bash
+pip install skillNer
+```
+
+2. Next, run the following command to install ``spacy en_core_web_lg ``
+which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
+customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
+
+```bash
+python -m spacy download en_core_web_lg
+```
+
+**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
+
+
+## Example of usage
+
+With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
+
+Let’s say you want to extract skills from the following job posting:
+
+    “You are a Python developer with a solid experience in web development and can manage projects. 
+    You quickly adapt to new environments and speak fluently English and French”
+
+### Annotating skills
+
+We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
+
+**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
+
+
+
+```python
+# imports
+import spacy
+from spacy.matcher import PhraseMatcher
+
+# load default skills data base
+from skillNer.general_params import SKILL_DB
+# import skill extractor
+from skillNer.skill_extractor_class import SkillExtractor
+
+# init params of skill extractor
+nlp = spacy.load("en_core_web_lg")
+# init skill extractor
+skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
+
+# extract skills from job_description
+job_description = """
+You are a Python developer with a solid experience in web development
+and can manage projects. You quickly adapt to new environments
+and speak fluently English and French
+"""
+
+annotations = skill_extractor.annotate(job_description)
+
+```
+
+
+
+### Exploit annotations
+
+Voilà! Now you can inspect results by rendering the text with the annotated skills.
+You can acheive that through the ``.describe`` method. Note that the output of this method is 
+litteraly an HTML document that gets rendered in your notebook.
+
+
+<p align="center">
+    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
+</p>
+
+
+Besides, you can use the raw result of the annotations. 
+Below is the value of the ``annotations`` variable from the code above.
+
+
+```python
+# output
+{
+    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
+    'results': {
+        'full_matches': [
+            {
+                'skill_id': 'KS122Z36QK3N5097B5JH', 
+                'doc_node_value': 'web development', 
+                'score': 1, 'doc_node_id': [10, 11]
+            }
+        ], '
+        ngram_scored': [
+            {
+                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
+                'doc_node_id': [3], 
+                'doc_node_value': 'python', 
+                'type': 'fullUni', 
+                'score': 1, 
+                'len': 1
+            }, 
+        # the other annotated skills
+        # ...
+        ]
+    }
+}
+```
+
+# Contribure
+
+SkillNer is the first **Open Source** skill extractor. 
+Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
+
+We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
+make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
+and broaden its usage. 
+
+
+You can contribute to SkillNer either by
+
+1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
+
+2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
+
+
+3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
+
+
+
+Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
+
+
+Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
+
+
+## Useful links
+
+- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
+- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
+- [Test our Demo](https://share.streamlit.io/anasaito/skillner_demo/index.py) to see some of SkillNer capabilities
```

### Comparing `NUGigSkillNER-1.0.2/README.md` & `NUGigSkillNER-2.0.0/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
-
-[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
-
-----------------------
-
-
-[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
-
-SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
-
-Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
-
-
-
-<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
-
-
-## Installation
-
-It is easy to get started with **SkillNer** and take advantage of its features.
-
-1. First, install **SkillNer** through the ``pip``
-
-```bash
-pip install skillNer
-```
-
-2. Next, run the following command to install ``spacy en_core_web_lg ``
-which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
-customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
-
-```bash
-python -m spacy download en_core_web_lg
-```
-
-**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
-
-
-## Example of usage
-
-With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
-
-Let’s say you want to extract skills from the following job posting:
-
-    “You are a Python developer with a solid experience in web development and can manage projects. 
-    You quickly adapt to new environments and speak fluently English and French”
-
-### Annotating skills
-
-We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
-
-**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
-
-
-
-```python
-# imports
-import spacy
-from spacy.matcher import PhraseMatcher
-
-# load default skills data base
-from skillNer.general_params import SKILL_DB
-# import skill extractor
-from skillNer.skill_extractor_class import SkillExtractor
-
-# init params of skill extractor
-nlp = spacy.load("en_core_web_lg")
-# init skill extractor
-skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
-
-# extract skills from job_description
-job_description = """
-You are a Python developer with a solid experience in web development
-and can manage projects. You quickly adapt to new environments
-and speak fluently English and French
-"""
-
-annotations = skill_extractor.annotate(job_description)
-
-```
-
-
-
-### Exploit annotations
-
-Voilà! Now you can inspect results by rendering the text with the annotated skills.
-You can acheive that through the ``.describe`` method. Note that the output of this method is 
-litteraly an HTML document that gets rendered in your notebook.
-
-
-<p align="center">
-    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
-</p>
-
-
-Besides, you can use the raw result of the annotations. 
-Below is the value of the ``annotations`` variable from the code above.
-
-
-```python
-# output
-{
-    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
-    'results': {
-        'full_matches': [
-            {
-                'skill_id': 'KS122Z36QK3N5097B5JH', 
-                'doc_node_value': 'web development', 
-                'score': 1, 'doc_node_id': [10, 11]
-            }
-        ], '
-        ngram_scored': [
-            {
-                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
-                'doc_node_id': [3], 
-                'doc_node_value': 'python', 
-                'type': 'fullUni', 
-                'score': 1, 
-                'len': 1
-            }, 
-        # the other annotated skills
-        # ...
-        ]
-    }
-}
-```
-
-# Contribure
-
-SkillNer is the first **Open Source** skill extractor. 
-Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
-
-We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
-make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
-and broaden its usage. 
-
-
-You can contribute to SkillNer either by
-
-1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
-
-2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
-
-
-3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
-
-
-
-Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
-
-
-Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
-
-
-## Useful links
-
-- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
-- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/128958594-79813e72-b688-4a9a-9267-324f098d4b0c.png" /></p>
+
+[**Live demo**](https://share.streamlit.io/anasaito/skillner_demo/index.py) | [**Documentation**](https://badr-moufad.github.io/SkillNER/get_started.html) | [**Website**](https://skillner.vercel.app/)
+
+----------------------
+
+
+[![Downloads](https://static.pepy.tech/personalized-badge/skillner?period=month&units=international_system&left_color=blue&right_color=green&left_text=Downloads%20/%20months)](https://pepy.tech/project/skillner)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+**Just looking to test out SkillNer? Check out our [demo](https://anasaito-skillner-demo-index-4fiwi3.streamlit.app/)**.
+
+SkillNer is an NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes.
+
+Skillner uses [EMSI](https://skills.emsidata.com/) databse (an open source skill database) as a knowldge base linker to prevent skill duplications.
+
+
+
+<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/56308112/138768792-a25d25e7-1e43-4a44-aa46-8de9895ffe88.png" /></p>
+
+
+## Installation
+
+It is easy to get started with **SkillNer** and take advantage of its features.
+
+1. First, install **SkillNer** through the ``pip``
+
+```bash
+pip install skillNer
+```
+
+2. Next, run the following command to install ``spacy en_core_web_lg ``
+which is one of the main plugins of SkillNer. Thanks its modular nature, you can 
+customize SkillNer behavior just by adjusting  | plugin | unplugin modules. Don't worry about these details, we will discuss them in details in the an **upcomming Tutorial section**.
+
+```bash
+python -m spacy download en_core_web_lg
+```
+
+**Note:** The later installation will take few seconds before it get done since ``spacy en_core_web_lg `` is a bit too large (800 MB). Yet, you need to wait only one time.
+
+
+## Example of usage
+
+With these initial steps being accomplished, let’s dive a bit deeper into skillNer through a worked example.
+
+Let’s say you want to extract skills from the following job posting:
+
+    “You are a Python developer with a solid experience in web development and can manage projects. 
+    You quickly adapt to new environments and speak fluently English and French”
+
+### Annotating skills
+
+We start first by importing modules, particularly spacy and SkillExtractor. Note that if you are using skillNer for the first time, it might take a while to download SKILL_DB.
+
+**SKILL_DB** is SkillNer default skills database. It was built upon [EMSI skills database ](https://skills.emsidata.com/).
+
+
+
+```python
+# imports
+import spacy
+from spacy.matcher import PhraseMatcher
+
+# load default skills data base
+from skillNer.general_params import SKILL_DB
+# import skill extractor
+from skillNer.skill_extractor_class import SkillExtractor
+
+# init params of skill extractor
+nlp = spacy.load("en_core_web_lg")
+# init skill extractor
+skill_extractor = SkillExtractor(nlp, SKILL_DB, PhraseMatcher)
+
+# extract skills from job_description
+job_description = """
+You are a Python developer with a solid experience in web development
+and can manage projects. You quickly adapt to new environments
+and speak fluently English and French
+"""
+
+annotations = skill_extractor.annotate(job_description)
+
+```
+
+
+
+### Exploit annotations
+
+Voilà! Now you can inspect results by rendering the text with the annotated skills.
+You can acheive that through the ``.describe`` method. Note that the output of this method is 
+litteraly an HTML document that gets rendered in your notebook.
+
+
+<p align="center">
+    <img src="./screenshots/output-describe.gif" alt="example output skillNer"/>
+</p>
+
+
+Besides, you can use the raw result of the annotations. 
+Below is the value of the ``annotations`` variable from the code above.
+
+
+```python
+# output
+{
+    'text': 'you are a python developer with a solid experience in web development and can manage projects you quickly adapt to new environments and speak fluently english and french',
+    'results': {
+        'full_matches': [
+            {
+                'skill_id': 'KS122Z36QK3N5097B5JH', 
+                'doc_node_value': 'web development', 
+                'score': 1, 'doc_node_id': [10, 11]
+            }
+        ], '
+        ngram_scored': [
+            {
+                'skill_id': 'KS125LS6N7WP4S6SFTCK', 
+                'doc_node_id': [3], 
+                'doc_node_value': 'python', 
+                'type': 'fullUni', 
+                'score': 1, 
+                'len': 1
+            }, 
+        # the other annotated skills
+        # ...
+        ]
+    }
+}
+```
+
+# Contribure
+
+SkillNer is the first **Open Source** skill extractor. 
+Hence it is a tool dedicated to the community and thereby relies on its contribution to evolve.
+
+We did our best to adapt SkillNer for usage and fixed many of its bugs. Therefore, we believe its key features 
+make it ready for a diversity of use cases. However, it still has not reached 100% stability. SkillNer needs the assistance of the community to be adapted further
+and broaden its usage. 
+
+
+You can contribute to SkillNer either by
+
+1. Reporting issues. Indeed, you may encounter one while you are using SkillNer. So do not hesitate to mention them in the [issue section of our GitHub repository](https://github.com/AnasAito/SkillNER/issues). Also, you can use the issue as a way to suggest new features to be added.
+
+2. Pushing code to our repository through pull requests. In case you fixed an issue or wanted to extend SkillNer features.
+
+
+3. A third (friendly and not technical) option to contribute to SkillNer will be soon released. *So, stay tuned...*
+
+
+
+Finally, make sure to read carefully [our guidelines](https://badr-moufad.github.io/SkillNER/contribute.html) before contributing. It will specifies standards to follow so that we can understand what you want to say.
+
+
+Besides, it will help you setup SkillNer on your local machine, in case you are willing to push code.
+
+
+## Useful links
+
+- [Visit our website](https://skillner.vercel.app/) to learn about SkillNer features, how it works, and particularly explore our roadmap
+- Get started with SkillNer and get to know its API by visiting the [Documentation](https://badr-moufad.github.io/SkillNER/get_started.html)
 - [Test our Demo](https://share.streamlit.io/anasaito/skillner_demo/index.py) to see some of SkillNer capabilities
```

### Comparing `NUGigSkillNER-1.0.2/setup.py` & `NUGigSkillNER-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import setuptools
-
-
-dependencies = [
-    "numpy",
-    "pandas",
-    "nltk",
-    "spacy",
-    "jellyfish",
-    "scipy"
-]
-
-setuptools.setup(
-    name="NUGigSkillNER",
-    version="1.0.2",
-    author="Ethan Mandel",
-    author_email="emandel2630@gmail.com",
-    description="An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes",
-    url="https://github.com/emandel2630/NUGigSkillNER",
-    keywords=["skillNer", 'python', 'NLP', "NER",
-              "skills-extraction", "job-description"],
-    packages=setuptools.find_packages(),
-    install_requires=dependencies,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        'License :: OSI Approved :: MIT License',
-        "Operating System :: OS Independent",
-    ],
-)
+import setuptools
+
+
+dependencies = [
+    "numpy",
+    "pandas",
+    "nltk",
+    "spacy",
+    "jellyfish",
+    "scipy"
+]
+
+setuptools.setup(
+    name="NUGigSkillNER",
+    version="2.0.0",
+    author="Ethan Mandel",
+    author_email="emandel2630@gmail.com",
+    description="An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes",
+    url="https://github.com/emandel2630/NUGigSkillNER",
+    keywords=["skillNer", 'python', 'NLP', "NER",
+              "skills-extraction", "job-description"],
+    packages=setuptools.find_packages(),
+    install_requires=dependencies,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        'License :: OSI Approved :: MIT License',
+        "Operating System :: OS Independent",
+    ],
+)
```

### Comparing `NUGigSkillNER-1.0.2/skills_processor/create_surf_db.py` & `NUGigSkillNER-2.0.0/skills_processor/create_surf_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-1.0.2/skills_processor/create_token_dist.py` & `NUGigSkillNER-2.0.0/skills_processor/create_token_dist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ============
 # Script to generate token frequency dict suing n_gram skill fullname
 # ============
 
 import json
 import collections
 
-with open('./skillNer/data/skill_db_relax_20.json', 'r+') as f:
+with open('./skillNer/buckets/skill_db_relax_20.json', 'r+') as f:
     skills_db = json.load(f)
 
 
 def get_dist_new(array):
     words = []
     for val in array:
         vals = val.split(' ')
@@ -23,9 +23,9 @@
     return counter
 
 
 n_grams = [skills_db[key]['high_surfce_forms']['full']
            for key in skills_db if skills_db[key]['skill_len'] > 1]
 n_gram_dist = get_dist_new(n_grams)
 # save
-with open('./skillNer/data/token_dist.json', 'w', encoding='utf-8') as f:
+with open('./skillNer/buckets/token_dist.json', 'w', encoding='utf-8') as f:
     json.dump(n_gram_dist, f, ensure_ascii=False, indent=4)
```

### Comparing `NUGigSkillNER-1.0.2/skills_processor/fetch_raw_data.py` & `NUGigSkillNER-2.0.0/skills_processor/fetch_raw_data.py`

 * *Files identical despite different names*

