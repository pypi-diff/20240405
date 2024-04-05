# Comparing `tmp/NUGigSkillNER-2.0.0.tar.gz` & `tmp/NUGigSkillNER-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NUGigSkillNER-2.0.0.tar", last modified: Thu Apr  4 18:43:52 2024, max compression
+gzip compressed data, was "NUGigSkillNER-2.0.1.tar", last modified: Fri Apr  5 00:37:30 2024, max compression
```

## Comparing `NUGigSkillNER-2.0.0.tar` & `NUGigSkillNER-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/
--rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.710717 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/
--rw-rw-rw-   0        0        0     7268 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-04 18:43:52.000000 NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7268 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.0/README.md
--rw-rw-rw-   0        0        0      169 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-04-04 18:33:46.000000 NUGigSkillNER-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.718710 NUGigSkillNER-2.0.0/skillNer/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/__init__.py
--rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/cleaner.py
--rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/general_params.py
--rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.0/skillNer/matcher_class.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.719913 NUGigSkillNER-2.0.0/skillNer/network/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/network/__init__.py
--rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/network/remote_db.py
--rw-rw-rw-   0        0        0     8036 2024-02-20 20:51:07.000000 NUGigSkillNER-2.0.0/skillNer/skill_extractor_class.py
--rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.0/skillNer/text_class.py
--rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.723548 NUGigSkillNER-2.0.0/skillNer/visualizer/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/__init__.py
--rw-rw-rw-   0        0        0     3159 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/html_elements.py
--rw-rw-rw-   0        0        0     7192 2024-02-20 20:50:59.000000 NUGigSkillNER-2.0.0/skillNer/visualizer/phrase_class.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:43:52.724827 NUGigSkillNER-2.0.0/skills_processor/
--rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skills_processor/__init__.py
--rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.0/skills_processor/create_new_skill.py
--rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.0/skills_processor/create_surf_db.py
--rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.0/skills_processor/create_token_dist.py
--rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.0/skills_processor/fetch_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/
+-rw-rw-rw-   0        0        0     1114 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.664450 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/
+-rw-rw-rw-   0        0        0     7268 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-05 00:37:30.000000 NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7268 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6668 2024-02-14 18:15:55.000000 NUGigSkillNER-2.0.1/README.md
+-rw-rw-rw-   0        0        0      169 2024-04-05 00:37:30.711042 NUGigSkillNER-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-04-05 00:36:43.000000 NUGigSkillNER-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/__init__.py
+-rw-rw-rw-   0        0        0     8803 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/cleaner.py
+-rw-rw-rw-   0        0        0     5291 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/general_params.py
+-rw-rw-rw-   0        0        0    11433 2024-02-20 20:51:25.000000 NUGigSkillNER-2.0.1/skillNer/matcher_class.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/network/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/network/__init__.py
+-rw-rw-rw-   0        0        0     1944 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/network/remote_db.py
+-rw-rw-rw-   0        0        0     8036 2024-02-20 20:51:07.000000 NUGigSkillNER-2.0.1/skillNer/skill_extractor_class.py
+-rw-rw-rw-   0        0        0    10006 2024-02-18 19:41:05.000000 NUGigSkillNER-2.0.1/skillNer/text_class.py
+-rw-rw-rw-   0        0        0     8853 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.680113 NUGigSkillNER-2.0.1/skillNer/visualizer/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/__init__.py
+-rw-rw-rw-   0        0        0     3159 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/html_elements.py
+-rw-rw-rw-   0        0        0     7192 2024-02-20 20:50:59.000000 NUGigSkillNER-2.0.1/skillNer/visualizer/phrase_class.py
+drwxrwxrwx   0        0        0        0 2024-04-05 00:37:30.703171 NUGigSkillNER-2.0.1/skills_processor/
+-rw-rw-rw-   0        0        0        0 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skills_processor/__init__.py
+-rw-rw-rw-   0        0        0     1365 2024-02-21 15:45:38.000000 NUGigSkillNER-2.0.1/skills_processor/create_new_skill.py
+-rw-rw-rw-   0        0        0     4377 2024-02-17 14:43:40.000000 NUGigSkillNER-2.0.1/skills_processor/create_surf_db.py
+-rw-rw-rw-   0        0        0      779 2024-02-21 15:39:27.000000 NUGigSkillNER-2.0.1/skills_processor/create_token_dist.py
+-rw-rw-rw-   0        0        0     1536 2024-02-17 14:43:41.000000 NUGigSkillNER-2.0.1/skills_processor/fetch_raw_data.py
```

### Comparing `NUGigSkillNER-2.0.0/LICENSE` & `NUGigSkillNER-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/PKG-INFO` & `NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.0
+Version: 2.0.1
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.0/NUGigSkillNER.egg-info/SOURCES.txt` & `NUGigSkillNER-2.0.1/NUGigSkillNER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/PKG-INFO` & `NUGigSkillNER-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NUGigSkillNER
-Version: 2.0.0
+Version: 2.0.1
 Summary: An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes
 Home-page: https://github.com/emandel2630/NUGigSkillNER
 Author: Ethan Mandel
 Author-email: emandel2630@gmail.com
 Keywords: skillNer,python,NLP,NER,skills-extraction,job-description
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NUGigSkillNER-2.0.0/README.md` & `NUGigSkillNER-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/setup.py` & `NUGigSkillNER-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "spacy",
     "jellyfish",
     "scipy"
 ]
 
 setuptools.setup(
     name="NUGigSkillNER",
-    version="2.0.0",
+    version="2.0.1",
     author="Ethan Mandel",
     author_email="emandel2630@gmail.com",
     description="An NLP module to automatically Extract skills and certifications from unstructured job postings, texts, and applicant's resumes",
     url="https://github.com/emandel2630/NUGigSkillNER",
     keywords=["skillNer", 'python', 'NLP', "NER",
               "skills-extraction", "job-description"],
     packages=setuptools.find_packages(),
```

### Comparing `NUGigSkillNER-2.0.0/skillNer/cleaner.py` & `NUGigSkillNER-2.0.1/skillNer/cleaner.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/general_params.py` & `NUGigSkillNER-2.0.1/skillNer/general_params.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/matcher_class.py` & `NUGigSkillNER-2.0.1/skillNer/matcher_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/network/remote_db.py` & `NUGigSkillNER-2.0.1/skillNer/network/remote_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/skill_extractor_class.py` & `NUGigSkillNER-2.0.1/skillNer/skill_extractor_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/text_class.py` & `NUGigSkillNER-2.0.1/skillNer/text_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/utils.py` & `NUGigSkillNER-2.0.1/skillNer/utils.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/visualizer/html_elements.py` & `NUGigSkillNER-2.0.1/skillNer/visualizer/html_elements.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skillNer/visualizer/phrase_class.py` & `NUGigSkillNER-2.0.1/skillNer/visualizer/phrase_class.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skills_processor/create_new_skill.py` & `NUGigSkillNER-2.0.1/skills_processor/create_new_skill.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skills_processor/create_surf_db.py` & `NUGigSkillNER-2.0.1/skills_processor/create_surf_db.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skills_processor/create_token_dist.py` & `NUGigSkillNER-2.0.1/skills_processor/create_token_dist.py`

 * *Files identical despite different names*

### Comparing `NUGigSkillNER-2.0.0/skills_processor/fetch_raw_data.py` & `NUGigSkillNER-2.0.1/skills_processor/fetch_raw_data.py`

 * *Files identical despite different names*

