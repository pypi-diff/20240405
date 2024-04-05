# Comparing `tmp/NUGigSkillNER-2.0.1.tar.gz` & `tmp/NUGigSkillNER-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NUGigSkillNER-2.0.1.tar", last modified: Fri Apr  5 00:37:30 2024, max compression
+gzip compressed data, was "NUGigSkillNER-2.0.2.tar", last modified: Fri Apr  5 01:02:46 2024, max compression
```

## Comparing `NUGigSkillNER-2.0.1.tar` & `NUGigSkillNER-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/
--rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.664450 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/
--rw-rw-rw-   0        0        0     7268 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7268 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.1/README.md
--rw-rw-rw-   0        0        0      169 2024-04-05 00:37:30.711042 NUGigSkillNER-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-04-05 00:36:43.000000 NUGigSkillNER-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/__init__.py
--rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/cleaner.py
--rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/general_params.py
--rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.1/skillNer/matcher_class.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/network/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/network/__init__.py
--rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/network/remote_db.py
--rw-rw-rw-   0        0        0     8036 2024-02-20 20:51:07.000000 NUGigSkillNER-2.0.1/skillNer/skill_extractor_class.py
--rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.1/skillNer/text_class.py
--rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/visualizer/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/__init__.py
--rw-rw-rw-   0        0        0     3159 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/html_elements.py
--rw-rw-rw-   0        0        0     7192 2024-02-20 20:50:59.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/phrase_class.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/skills_processor/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skills_processor/__init__.py
--rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.1/skills_processor/create_new_skill.py
--rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skills_processor/create_surf_db.py
--rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.1/skills_processor/create_token_dist.py
--rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.1/skills_processor/fetch_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.241968 NUGigSkillNER-2.0.2/
+-rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.201966 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/
+-rw-rw-rw-   0        0        0     7268 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-05 01:02:45.000000 NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.220993 NUGigSkillNER-2.0.2/NuGigSkillNER/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/__init__.py
+-rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/cleaner.py
+-rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/general_params.py
+-rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/matcher_class.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.225161 NUGigSkillNER-2.0.2/NuGigSkillNER/network/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/network/__init__.py
+-rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/network/remote_db.py
+-rw-rw-rw-   0        0        0     8098 2024-04-05 01:00:17.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/skill_extractor_class.py
+-rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/text_class.py
+-rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/NuGigSkillNER/utils.py
+-rw-rw-rw-   0        0        0     7268 2024-04-05 01:02:46.241968 NUGigSkillNER-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.2/README.md
+-rw-rw-rw-   0        0        0      169 2024-04-05 01:02:46.247239 NUGigSkillNER-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-04-05 01:02:05.000000 NUGigSkillNER-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:02:46.241793 NUGigSkillNER-2.0.2/skills_processor/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/skills_processor/__init__.py
+-rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.2/skills_processor/create_new_skill.py
+-rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.2/skills_processor/create_surf_db.py
+-rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.2/skills_processor/create_token_dist.py
+-rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.2/skills_processor/fetch_raw_data.py
```

### Comparing `NUGigSkillNER-2.0.1/LICENSE` & `NUGigSkillNER-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/PKG-INFO` & `NUGigSkillNER-2.0.2/NUGigSkillNER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.1
+Version: 2.0.2
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.1/PKG-INFO` & `NUGigSkillNER-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.1
+Version: 2.0.2
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.1/README.md` & `NUGigSkillNER-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/setup.py` & `NUGigSkillNER-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "spacy",
     "jellyfish",
     "scipy"
 ]
 
 setuptools.setup(
     name="NUGigSkillNER",
-    version="2.0.1",
+    version="2.0.2",
     author="Ethan Mandel",
     author_email="emandel2630@gmail.com",
     description="An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes",
     url="https://github.com/emandel2630/NUGigSkillNER",
     keywords=["skillNer", 'python', 'NLP', "NER",
               "skills-extraction", "job-description"],
     packages=setuptools.find_packages(),
```

### Comparing `NUGigSkillNER-2.0.1/skillNer/cleaner.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/cleaner.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skillNer/general_params.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/general_params.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skillNer/matcher_class.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/matcher_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skillNer/network/remote_db.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/network/remote_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skillNer/skill_extractor_class.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/skill_extractor_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from spacy import displacy
 # my packs
 from skillNer.text_class import Text
 from skillNer.matcher_class import Matchers, SkillsGetter
 from skillNer.utils import Utils
 from skillNer.general_params import SKILL_TO_COLOR
 
-from skillNer.visualizer.html_elements import DOM, render_phrase
-from skillNer.visualizer.phrase_class import Phrase
-
 
 class SkillExtractor:
     """Main class to annotate skills in a given text and visualize them.
     """
 
     def __init__(
         self,
@@ -147,115 +144,115 @@
             'text': text_obj.transformed_text,
             'results': {
                 'full_matches': full_sk,
                 'ngram_scored': [match for match in process_n_gram if match['score'] >= tresh],
             }
         }
 
-    def display(
-        self,
-        results: dict
-    ):
-        """To display the annotated skills. 
-        This method uses built-in classes of spacy to render annotated text, namely `displacy`.
-
-        Parameters
-        ----------
-        results : dict
-            results is the dictionnary resulting from applying `.annotate()` to a text.
-
-        Results
-        -------
-        None 
-            render the text with annotated skills.
-        """
-
-        # explode result object
-        text = results["text"]
-        skill_extractor_results = results['results']
-
-        # words and their positions
-        words_position = Text.words_start_end_position(text)
-
-        # get matches
-        matches = []
-        for match_type in skill_extractor_results.keys():
-            for match in skill_extractor_results[match_type]:
-                matches.append(match)
-
-        # displacy render params
-        entities = []
-        colors = {}
-        colors_id = []
-
-        # fill params
-        for match in matches:
-            # skill id
-            skill_id = match["skill_id"]
-
-            # index of words in skill
-            index_start_word, index_end_word = match['doc_node_id'][0], match['doc_node_id'][-1]
-
-            # build/append entity
-            entity = {
-                "start": words_position[index_start_word].start,
-                "end": words_position[index_end_word].end,
-                "label": self.skills_db[skill_id]['skill_name']
-            }
-            entities.append(entity)
-
-            # highlight matched skills
-            colors[entity['label']
-                   ] = SKILL_TO_COLOR[self.skills_db[skill_id]['skill_type']]
-            colors_id.append(entity['label'])
-
-        # prepare params
-        entities.sort(key=lambda x: x['start'], reverse=False)
-        options = {"ents": colors_id, "colors": colors}
-        ex = {
-            "text": text,
-            "ents": entities,
-            "title": None
-        }
-
-        # render
-        html = displacy.render(ex, style="ent", manual=True, options=options)
-
-    def describe(
-        self,
-        annotations: dict,
-        annotationType = 'text',
-    ):
-        """To display more details about the annotated skills.
-        This method uses HTML, CSS, JavaScript combined with IPython to render the annotated skills.
-
-        Parameters
-        ----------
-        annotations : dict
-            annotations is the dictionnary resulting from applying `.annotate()` to a text.
-
-        Returns
-        -------
-        [type]
-            render text with annotated skills.
-        """
-
-        # build phrases to display from annotations
-        if annotationType == "cleaned text":
-            arr_phrases = Phrase.split_updated_text_to_phare(
-            annotations,
-            self.skills_db,
-        )
-        else:
-            arr_phrases = Phrase.split_text_to_phare(
-            annotations,
-            self.skills_db,
-        )
-
-        # create DOM
-        document = DOM(children=[
-            render_phrase(phrase)
-            for phrase in arr_phrases
-        ])
+    # def display(
+    #     self,
+    #     results: dict
+    # ):
+    #     """To display the annotated skills. 
+    #     This method uses built-in classes of spacy to render annotated text, namely `displacy`.
+
+    #     Parameters
+    #     ----------
+    #     results : dict
+    #         results is the dictionnary resulting from applying `.annotate()` to a text.
+
+    #     Results
+    #     -------
+    #     None 
+    #         render the text with annotated skills.
+    #     """
+
+    #     # explode result object
+    #     text = results["text"]
+    #     skill_extractor_results = results['results']
+
+    #     # words and their positions
+    #     words_position = Text.words_start_end_position(text)
+
+    #     # get matches
+    #     matches = []
+    #     for match_type in skill_extractor_results.keys():
+    #         for match in skill_extractor_results[match_type]:
+    #             matches.append(match)
+
+    #     # displacy render params
+    #     entities = []
+    #     colors = {}
+    #     colors_id = []
+
+    #     # fill params
+    #     for match in matches:
+    #         # skill id
+    #         skill_id = match["skill_id"]
+
+    #         # index of words in skill
+    #         index_start_word, index_end_word = match['doc_node_id'][0], match['doc_node_id'][-1]
+
+    #         # build/append entity
+    #         entity = {
+    #             "start": words_position[index_start_word].start,
+    #             "end": words_position[index_end_word].end,
+    #             "label": self.skills_db[skill_id]['skill_name']
+    #         }
+    #         entities.append(entity)
+
+    #         # highlight matched skills
+    #         colors[entity['label']
+    #                ] = SKILL_TO_COLOR[self.skills_db[skill_id]['skill_type']]
+    #         colors_id.append(entity['label'])
+
+    #     # prepare params
+    #     entities.sort(key=lambda x: x['start'], reverse=False)
+    #     options = {"ents": colors_id, "colors": colors}
+    #     ex = {
+    #         "text": text,
+    #         "ents": entities,
+    #         "title": None
+    #     }
+
+    #     # render
+    #     html = displacy.render(ex, style="ent", manual=True, options=options)
+
+    # def describe(
+    #     self,
+    #     annotations: dict,
+    #     annotationType = 'text',
+    # ):
+    #     """To display more details about the annotated skills.
+    #     This method uses HTML, CSS, JavaScript combined with IPython to render the annotated skills.
+
+    #     Parameters
+    #     ----------
+    #     annotations : dict
+    #         annotations is the dictionnary resulting from applying `.annotate()` to a text.
+
+    #     Returns
+    #     -------
+    #     [type]
+    #         render text with annotated skills.
+    #     """
+
+    #     # build phrases to display from annotations
+    #     if annotationType == "cleaned text":
+    #         arr_phrases = Phrase.split_updated_text_to_phare(
+    #         annotations,
+    #         self.skills_db,
+    #     )
+    #     else:
+    #         arr_phrases = Phrase.split_text_to_phare(
+    #         annotations,
+    #         self.skills_db,
+    #     )
+
+    #     # create DOM
+    #     document = DOM(children=[
+    #         render_phrase(phrase)
+    #         for phrase in arr_phrases
+    #     ])
 
-        # render
-        return document
+    #     # render
+    #     return document
```

### Comparing `NUGigSkillNER-2.0.1/skillNer/text_class.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/text_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skillNer/utils.py` & `NUGigSkillNER-2.0.2/NuGigSkillNER/utils.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skills_processor/create_new_skill.py` & `NUGigSkillNER-2.0.2/skills_processor/create_new_skill.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skills_processor/create_surf_db.py` & `NUGigSkillNER-2.0.2/skills_processor/create_surf_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skills_processor/create_token_dist.py` & `NUGigSkillNER-2.0.2/skills_processor/create_token_dist.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.1/skills_processor/fetch_raw_data.py` & `NUGigSkillNER-2.0.2/skills_processor/fetch_raw_data.py`

 * *Files identical despite different names*

