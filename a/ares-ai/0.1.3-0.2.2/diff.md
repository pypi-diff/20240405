# Comparing `tmp/ares-ai-0.1.3.tar.gz` & `tmp/ares-ai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares-ai-0.1.3.tar", last modified: Fri Apr  5 09:34:42 2024, max compression
+gzip compressed data, was "ares-ai-0.2.2.tar", last modified: Fri Apr  5 09:30:08 2024, max compression
```

## Comparing `ares-ai-0.1.3.tar` & `ares-ai-0.2.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.106645 ares-ai-0.1.3/
--rw-rw-rw-   0 manihani (23549) future   (20099)     3691 2024-03-16 07:48:22.000000 ares-ai-0.1.3/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-03-09 08:06:02.000000 ares-ai-0.1.3/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares-ai-0.1.3/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       47 2024-04-05 05:51:22.000000 ares-ai-0.1.3/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    26337 2024-04-05 09:34:42.105645 ares-ai-0.1.3/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    10931 2024-03-24 06:16:10.000000 ares-ai-0.1.3/README.md
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:41.972651 ares-ai-0.1.3/ares/
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:41.982651 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6823 2024-03-29 05:33:41.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    29174 2024-03-29 08:05:57.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    25374 2024-04-05 05:56:20.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    17164 2024-02-16 01:17:04.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-01-20 21:27:59.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.002650 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4592 2024-03-29 05:35:38.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    17042 2024-03-29 08:06:45.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11989 2024-04-04 23:25:45.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9401 2024-02-16 01:20:25.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-01-20 22:03:41.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     2238 2024-01-13 21:15:48.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-01-08 23:19:52.000000 ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.016649 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    12696 2024-04-02 19:32:06.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    32941 2024-03-29 07:47:29.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-03-23 06:55:25.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-03-23 00:30:05.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7085 2024-03-22 22:57:24.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-01-08 23:19:52.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-01-20 21:28:14.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.042648 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     5214 2024-04-02 19:33:25.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    20212 2024-03-29 07:48:32.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-03-23 00:31:33.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     4245 2024-03-22 23:34:21.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      153 2024-01-20 21:58:30.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     8961 2024-02-04 12:22:14.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-02-02 23:33:13.000000 ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-03-10 08:23:02.000000 ares-ai-0.1.3/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares-ai-0.1.3/ares/__init__.pyc
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.069647 ares-ai-0.1.3/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-03-10 09:27:12.000000 ares-ai-0.1.3/ares/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares-ai-0.1.3/ares/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     6981 2024-03-29 07:15:11.000000 ares-ai-0.1.3/ares/__pycache__/ares.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares-ai-0.1.3/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2148 2024-03-29 07:15:16.000000 ares-ai-0.1.3/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares-ai-0.1.3/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      371 2024-03-22 09:54:17.000000 ares-ai-0.1.3/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares-ai-0.1.3/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     1624 2024-03-10 09:27:18.000000 ares-ai-0.1.3/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares-ai-0.1.3/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      356 2024-03-22 22:53:44.000000 ares-ai-0.1.3/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares-ai-0.1.3/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2465 2024-04-04 23:23:41.000000 ares-ai-0.1.3/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares-ai-0.1.3/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3225 2024-04-02 19:33:25.000000 ares-ai-0.1.3/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares-ai-0.1.3/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10825 2024-03-29 06:55:21.000000 ares-ai-0.1.3/ares/ares.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.079646 ares-ai-0.1.3/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares-ai-0.1.3/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8135 2024-04-04 21:04:16.000000 ares-ai-0.1.3/ares/binary_classifier.py
--rw-r--r--   0 manihani (23549) future   (20099)      154 2024-03-22 09:52:41.000000 ares-ai-0.1.3/ares/kilt_filter.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.085646 ares-ai-0.1.3/ares/ppi/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-01-08 23:19:52.000000 ares-ai-0.1.3/ares/ppi/.DS_Store
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-02-03 23:36:27.000000 ares-ai-0.1.3/ares/ppi/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-01-08 23:19:52.000000 ares-ai-0.1.3/ares/ppi/ppi_testing.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     2823 2024-03-10 04:35:41.000000 ares-ai-0.1.3/ares/rag_scoring.py
--rw-r--r--   0 manihani (23549) future   (20099)      134 2024-03-22 22:40:11.000000 ares-ai-0.1.3/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-04-04 23:58:15.000000 ares-ai-0.1.3/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     5696 2024-04-02 19:30:03.000000 ares-ai-0.1.3/ares/ues_idp.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:34:42.102645 ares-ai-0.1.3/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26337 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)     4189 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      645 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 09:34:41.000000 ares-ai-0.1.3/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     2791 2024-04-05 09:33:48.000000 ares-ai-0.1.3/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5048 2024-03-16 09:02:36.000000 ares-ai-0.1.3/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-05 09:34:42.108645 ares-ai-0.1.3/setup.cfg
--rwxrwxrwx   0 manihani (23549) future   (20099)     7754 2024-03-29 08:09:58.000000 ares-ai-0.1.3/test.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.488153 ares-ai-0.2.2/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3691 2024-03-16 07:48:22.000000 ares-ai-0.2.2/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-03-09 08:06:02.000000 ares-ai-0.2.2/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares-ai-0.2.2/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       47 2024-04-05 05:51:22.000000 ares-ai-0.2.2/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    26337 2024-04-05 09:30:08.487152 ares-ai-0.2.2/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10931 2024-03-24 06:16:10.000000 ares-ai-0.2.2/README.md
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:07.678190 ares-ai-0.2.2/ares/
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:07.755186 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6823 2024-03-29 05:33:41.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    29174 2024-03-29 08:05:57.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    25374 2024-04-05 05:56:20.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17164 2024-02-16 01:17:04.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-01-20 21:27:59.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:07.876181 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4592 2024-03-29 05:35:38.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17042 2024-03-29 08:06:45.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11989 2024-04-04 23:25:45.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9401 2024-02-16 01:20:25.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-01-20 22:03:41.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     2238 2024-01-13 21:15:48.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-01-08 23:19:52.000000 ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:07.977176 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    12696 2024-04-02 19:32:06.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    32941 2024-03-29 07:47:29.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-03-23 06:55:25.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-03-23 00:30:05.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7085 2024-03-22 22:57:24.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-01-08 23:19:52.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-01-20 21:28:14.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.175167 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5214 2024-04-02 19:33:25.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    20212 2024-03-29 07:48:32.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-03-23 00:31:33.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     4245 2024-03-22 23:34:21.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      153 2024-01-20 21:58:30.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8961 2024-02-04 12:22:14.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-02-02 23:33:13.000000 ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-03-10 08:23:02.000000 ares-ai-0.2.2/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares-ai-0.2.2/ares/__init__.pyc
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.342159 ares-ai-0.2.2/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-03-10 09:27:12.000000 ares-ai-0.2.2/ares/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares-ai-0.2.2/ares/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6981 2024-03-29 07:15:11.000000 ares-ai-0.2.2/ares/__pycache__/ares.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares-ai-0.2.2/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2148 2024-03-29 07:15:16.000000 ares-ai-0.2.2/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares-ai-0.2.2/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      371 2024-03-22 09:54:17.000000 ares-ai-0.2.2/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares-ai-0.2.2/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1624 2024-03-10 09:27:18.000000 ares-ai-0.2.2/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares-ai-0.2.2/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      356 2024-03-22 22:53:44.000000 ares-ai-0.2.2/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares-ai-0.2.2/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2465 2024-04-04 23:23:41.000000 ares-ai-0.2.2/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares-ai-0.2.2/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3225 2024-04-02 19:33:25.000000 ares-ai-0.2.2/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares-ai-0.2.2/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10825 2024-03-29 06:55:21.000000 ares-ai-0.2.2/ares/ares.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.407156 ares-ai-0.2.2/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares-ai-0.2.2/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8135 2024-04-04 21:04:16.000000 ares-ai-0.2.2/ares/binary_classifier.py
+-rw-r--r--   0 manihani (23549) future   (20099)      154 2024-03-22 09:52:41.000000 ares-ai-0.2.2/ares/kilt_filter.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.447154 ares-ai-0.2.2/ares/ppi/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-01-08 23:19:52.000000 ares-ai-0.2.2/ares/ppi/.DS_Store
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-02-03 23:36:27.000000 ares-ai-0.2.2/ares/ppi/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-01-08 23:19:52.000000 ares-ai-0.2.2/ares/ppi/ppi_testing.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2823 2024-03-10 04:35:41.000000 ares-ai-0.2.2/ares/rag_scoring.py
+-rw-r--r--   0 manihani (23549) future   (20099)      134 2024-03-22 22:40:11.000000 ares-ai-0.2.2/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-04-04 23:58:15.000000 ares-ai-0.2.2/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5696 2024-04-02 19:30:03.000000 ares-ai-0.2.2/ares/ues_idp.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-05 09:30:08.484153 ares-ai-0.2.2/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26337 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4189 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      645 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 09:30:07.000000 ares-ai-0.2.2/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2791 2024-04-05 08:56:51.000000 ares-ai-0.2.2/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5048 2024-03-16 09:02:36.000000 ares-ai-0.2.2/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-05 09:30:08.490152 ares-ai-0.2.2/setup.cfg
+-rwxrwxrwx   0 manihani (23549) future   (20099)     7754 2024-03-29 08:09:58.000000 ares-ai-0.2.2/test.py
```

### Comparing `ares-ai-0.1.3/.gitignore` & `ares-ai-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/LICENSE` & `ares-ai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/PKG-INFO` & `ares-ai-0.2.2/ares/ares_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.1.3
+Version: 0.1.8
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,15 +227,14 @@
 Requires-Dist: matplotlib<4.0.0,>=3.7.1
 Requires-Dist: matplotlib-inline<0.2.0,>=0.1.6
 Requires-Dist: nltk<4.0.0,>=3.8.1
 Requires-Dist: numexpr<3.0.0,>=2.8.4
 Requires-Dist: numpy<2.0.0,>=1.20.0
 Requires-Dist: openai==1.14.2
 Requires-Dist: pandas>=2.0.1
-Requires-Dist: protobuf>=4.21.10
 Requires-Dist: pydantic<2.0.0,>=1.10.7
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
 Requires-Dist: pytorch-ranger<0.2.0,>=0.1.1
 Requires-Dist: pytz<2024.0,>=2023.3
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: scikit-learn<1.3.0,>=1.2.2
```

### Comparing `ares-ai-0.1.3/README.md` & `ares-ai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares-ai-0.2.2/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/RAG_Automatic_Evaluation/ppi.py` & `ares-ai-0.2.2/ares/RAG_Automatic_Evaluation/ppi.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/ares.cpython-310.pyc` & `ares-ai-0.2.2/ares/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/ares.cpython-311.pyc` & `ares-ai-0.2.2/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/binary_classifier.cpython-310.pyc` & `ares-ai-0.2.2/ares/__pycache__/binary_classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares-ai-0.2.2/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/rag_scoring.cpython-310.pyc` & `ares-ai-0.2.2/ares/__pycache__/rag_scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares-ai-0.2.2/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/synthetic_generator.cpython-310.pyc` & `ares-ai-0.2.2/ares/__pycache__/synthetic_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares-ai-0.2.2/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/ues_idp.cpython-310.pyc` & `ares-ai-0.2.2/ares/__pycache__/ues_idp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares-ai-0.2.2/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ares.py` & `ares-ai-0.2.2/ares/ares.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ares_ai.egg-info/PKG-INFO` & `ares-ai-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.1.8
+Version: 0.2.2
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,14 +227,15 @@
 Requires-Dist: matplotlib<4.0.0,>=3.7.1
 Requires-Dist: matplotlib-inline<0.2.0,>=0.1.6
 Requires-Dist: nltk<4.0.0,>=3.8.1
 Requires-Dist: numexpr<3.0.0,>=2.8.4
 Requires-Dist: numpy<2.0.0,>=1.20.0
 Requires-Dist: openai==1.14.2
 Requires-Dist: pandas>=2.0.1
+Requires-Dist: protobuf>=4.21.10
 Requires-Dist: pydantic<2.0.0,>=1.10.7
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
 Requires-Dist: pytorch-ranger<0.2.0,>=0.1.1
 Requires-Dist: pytz<2024.0,>=2023.3
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: requests<3.0.0,>=2.25.1
 Requires-Dist: scikit-learn<1.3.0,>=1.2.2
```

### Comparing `ares-ai-0.1.3/ares/ares_ai.egg-info/requires.txt` & `ares-ai-0.2.2/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/binary_classifier.py` & `ares-ai-0.2.2/ares/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ppi/.DS_Store` & `ares-ai-0.2.2/ares/ppi/.DS_Store`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ppi/ppi.py` & `ares-ai-0.2.2/ares/ppi/ppi.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ppi/ppi_testing.py` & `ares-ai-0.2.2/ares/ppi/ppi_testing.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/rag_scoring.py` & `ares-ai-0.2.2/ares/rag_scoring.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/synthetic_generator.py` & `ares-ai-0.2.2/ares/synthetic_generator.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares/ues_idp.py` & `ares-ai-0.2.2/ares/ues_idp.py`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares_ai.egg-info/PKG-INFO` & `ares-ai-0.2.2/ares_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.1.3
+Version: 0.2.2
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ares-ai-0.1.3/ares_ai.egg-info/SOURCES.txt` & `ares-ai-0.2.2/ares_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/ares_ai.egg-info/requires.txt` & `ares-ai-0.2.2/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/pyproject.toml` & `ares-ai-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.1.3"
+version = "0.2.2"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
```

### Comparing `ares-ai-0.1.3/requirements.txt` & `ares-ai-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ares-ai-0.1.3/test.py` & `ares-ai-0.2.2/test.py`

 * *Files identical despite different names*

