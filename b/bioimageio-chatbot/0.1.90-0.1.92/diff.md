# Comparing `tmp/bioimageio-chatbot-0.1.90.tar.gz` & `tmp/bioimageio-chatbot-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.90.tar", last modified: Tue Apr  2 20:35:31 2024, max compression
+gzip compressed data, was "bioimageio-chatbot-0.1.92.tar", last modified: Fri Apr  5 20:49:17 2024, max compression
```

## Comparing `bioimageio-chatbot-0.1.90.tar` & `bioimageio-chatbot-0.1.92.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.884356 bioimageio-chatbot-0.1.90/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/vision_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-02 20:35:31.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-02 20:35:31.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:35:31.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 20:35:31.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 20:35:31.000000 bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:35:31.888356 bioimageio-chatbot-0.1.90/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 20:35:18.000000 bioimageio-chatbot-0.1.90/tests/test_knowledge_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/bia_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/biii_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/docs_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/vision_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.668400 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/gpts_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/jsonschema_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 20:49:17.000000 bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:49:17.672400 bioimageio-chatbot-0.1.92/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_chatbot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_eval_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-05 20:49:06.000000 bioimageio-chatbot-0.1.92/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.90/LICENSE` & `bioimageio-chatbot-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/PKG-INFO` & `bioimageio-chatbot-0.1.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.90
+Version: 0.1.92
 Summary: Your Personal Assistant in BioImage Analysis.
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: schema-agents>=0.1.45
+Requires-Dist: schema-agents>=0.1.46
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
 Requires-Dist: pillow
 Requires-Dist: matplotlib
 Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm
@@ -21,15 +21,15 @@
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31
 Requires-Dist: langchain-community>=0.0.27
 Requires-Dist: html2text
 
 # 🦒 BioImage.IO Chatbot 🤖
 
-**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
 ## Your Personal Assistant in BioImage Analysis
 
 Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
 
@@ -282,15 +282,15 @@
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
 
 ## Publication
 
-For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032227']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032227.svg" alt="10.5281/zenodo.10032227"></a>**
 
 
 To reproduce the use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063) in the manuscript, please refer to the [reproducing example usage scenarios](./docs/figure-2-use-cases.md).
 
 <img style="width:300px;" src="https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.90 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.92 Summary: Your
 Personal Assistant in BioImage Analysis. Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.45 Requires-
+markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31 Requires-Dist: langchain-
 community>=0.0.27 Requires-Dist: html2text # ð¦ BioImage.IO Chatbot ð¤
@@ -168,15 +168,15 @@
 you have any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
-(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** To reproduce the
+(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
 use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&h=1063) in the manuscript,
 please refer to the [reproducing example usage scenarios](./docs/figure-2-use-
 cases.md). [https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063]## Cite Us If you
```

### Comparing `bioimageio-chatbot-0.1.90/README.md` & `bioimageio-chatbot-0.1.92/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 🦒 BioImage.IO Chatbot 🤖
 
-**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
 ## Your Personal Assistant in BioImage Analysis
 
 Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
 
@@ -257,15 +257,15 @@
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
 
 ## Publication
 
-For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032227']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032227.svg" alt="10.5281/zenodo.10032227"></a>**
 
 
 To reproduce the use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063) in the manuscript, please refer to the [reproducing example usage scenarios](./docs/figure-2-use-cases.md).
 
 <img style="width:300px;" src="https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063">
```

#### html2text {}

```diff
@@ -158,15 +158,15 @@
 you have any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
-(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** To reproduce the
+(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
 use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&h=1063) in the manuscript,
 please refer to the [reproducing example usage scenarios](./docs/figure-2-use-
 cases.md). [https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063]## Cite Us If you
```

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/__main__.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,19 +384,21 @@
         if login_required and context and context.get("user"):
             assert check_permission(
                 context.get("user")
             ), "You don't have permission to use the chatbot, please sign up and wait for approval"
         return "pong"
 
     assistant_keys = ["name", "extensions", "alias", "icon", "welcome_message", "code_interpreter"]
+    version = pkg_resources.get_distribution("bioimageio-chatbot").version
     hypha_service_info = await server.register_service(
         {
             "name": "BioImage.IO Chatbot",
             "id": "bioimageio-chatbot",
             "config": {"visibility": "public", "require_context": True},
+            "version": version,
             "ping": ping,
             "chat": chat,
             "report": report,
             "assistants": {
                 a["name"]: {k: a[k] for k in assistant_keys}
                 for a in assistants
             },
```

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/__init__.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/bia_extension.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/bia_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/biii_extension.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/biii_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/docs_extension.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/docs_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/vision_extension.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/vision_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         assert isinstance(message, str), "Message must be a string."
         user_message.append({"type": "text", "text": message})
 
     response = await aclient.chat.completions.create(
         model="gpt-4-1106-vision-preview",
         messages=[
             {
+                "role": "system",
+                "content": "You are a helpful AI assistant that help user to inspect the provided images visually based on the context, make insightful comments and answer questions about the provided images."
+            },
+            {
                 "role": "user",
                 "content": user_message
             }
         ],
         max_tokens=max_tokens,
     )
     return response.choices[0].message.content
```

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/evaluation.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/evaluation.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/gpts_action.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/gpts_action.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/jsonschema_pydantic.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/jsonschema_pydantic.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/knowledge_base.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot/utils.py` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/PKG-INFO` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.90
+Version: 0.1.92
 Summary: Your Personal Assistant in BioImage Analysis.
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: schema-agents>=0.1.45
+Requires-Dist: schema-agents>=0.1.46
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
 Requires-Dist: pillow
 Requires-Dist: matplotlib
 Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm
@@ -21,15 +21,15 @@
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31
 Requires-Dist: langchain-community>=0.0.27
 Requires-Dist: html2text
 
 # 🦒 BioImage.IO Chatbot 🤖
 
-**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+**📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
 ## Your Personal Assistant in BioImage Analysis
 
 Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
 
@@ -282,15 +282,15 @@
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
 
 ## Publication
 
-For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032228" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
+For detailed description of our work, please read our preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032227']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032227.svg" alt="10.5281/zenodo.10032227"></a>**
 
 
 To reproduce the use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063) in the manuscript, please refer to the [reproducing example usage scenarios](./docs/figure-2-use-cases.md).
 
 <img style="width:300px;" src="https://docs.google.com/drawings/d/e/2PACX-1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.90 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.92 Summary: Your
 Personal Assistant in BioImage Analysis. Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.45 Requires-
+markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31 Requires-Dist: langchain-
 community>=0.0.27 Requires-Dist: html2text # ð¦ BioImage.IO Chatbot ð¤
@@ -168,15 +168,15 @@
 you have any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
-(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** To reproduce the
+(https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
 use cases described in [Figure 2](https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&h=1063) in the manuscript,
 please refer to the [reproducing example usage scenarios](./docs/figure-2-use-
 cases.md). [https://docs.google.com/drawings/d/e/2PACX-
 1vTIRwRldQBnTFqz0hvS01znGOEdoeDMJmZC-PlBM-
 O59u_xo7DfJlUEE9SlRsy6xO1hT2HuSOBrLmUz/pub?w=1324&amp;h=1063]## Cite Us If you
```

### Comparing `bioimageio-chatbot-0.1.90/bioimageio_chatbot.egg-info/SOURCES.txt` & `bioimageio-chatbot-0.1.92/bioimageio_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/pyproject.toml` & `bioimageio-chatbot-0.1.92/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bioimageio-chatbot"
-version = "0.1.90"
+version = "0.1.92"
 readme = "README.md"
 description = "Your Personal Assistant in BioImage Analysis."
 dependencies = [
-  "schema-agents>=0.1.45",
+  "schema-agents>=0.1.46",
   "imjoy-rpc>=0.5.48.post2",
   "requests",
   "pypdf",
   "pillow",
   "matplotlib",
   "hypha>=0.15.50",
   "tqdm",
```

### Comparing `bioimageio-chatbot-0.1.90/tests/test_chatbot.py` & `bioimageio-chatbot-0.1.92/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/tests/test_chatbot_answer.py` & `bioimageio-chatbot-0.1.92/tests/test_chatbot_answer.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.90/tests/test_eval_agent.py` & `bioimageio-chatbot-0.1.92/tests/test_eval_agent.py`

 * *Files identical despite different names*

