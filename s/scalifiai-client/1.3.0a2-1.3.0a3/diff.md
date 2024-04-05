# Comparing `tmp/scalifiai-client-1.3.0a2.tar.gz` & `tmp/scalifiai-client-1.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.3.0a2.tar", last modified: Tue Apr  2 08:04:31 2024, max compression
+gzip compressed data, was "scalifiai-client-1.3.0a3.tar", last modified: Fri Apr  5 09:36:21 2024, max compression
```

## Comparing `scalifiai-client-1.3.0a2.tar` & `scalifiai-client-1.3.0a3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.096494 scalifiai-client-1.3.0a2/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-02 08:04:31.096494 scalifiai-client-1.3.0a2/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      982 2024-04-02 08:03:48.000000 scalifiai-client-1.3.0a2/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.088498 scalifiai-client-1.3.0a2/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6401 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.088498 scalifiai-client-1.3.0a2/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.088498 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.092496 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9083 2024-04-02 08:03:00.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1800 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.092496 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13378 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.092496 scalifiai-client-1.3.0a2/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34019 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.096494 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28660 2024-04-02 07:54:09.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a2/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 08:04:31.096494 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-02 08:04:31.000000 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-02 08:04:31.000000 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-02 08:04:31.000000 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      147 2024-04-02 08:04:31.000000 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-02 08:04:31.000000 scalifiai-client-1.3.0a2/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-02 08:04:31.096494 scalifiai-client-1.3.0a2/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      982 2024-04-05 09:35:58.000000 scalifiai-client-1.3.0a3/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9490 2024-04-05 09:32:04.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2144 2024-04-05 09:33:28.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-02 08:09:55.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      147 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/setup.cfg
```

### Comparing `scalifiai-client-1.3.0a2/PKG-INFO` & `scalifiai-client-1.3.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a2
+Version: 1.3.0a3
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a2/pyproject.toml` & `scalifiai-client-1.3.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.3.0-alpha.2"
+version = "1.3.0-alpha.3"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/base.py` & `scalifiai-client-1.3.0a3/scalifiai/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,17 @@
     def convert_datetime(self, value):
 
         if pd.isna(value) == False:
             value = pd.to_datetime(value)
             if (datetime.now(self.local_timezone) - value).days > 0:
                 value = humanize.naturaldate(value)
             else:
-                value = humanize.naturaltime(value, when=datetime.now(self.local_timezone))
+                value = humanize.naturaltime(
+                    value, when=datetime.now(self.local_timezone)
+                )
 
         return value
 
     def convert_size(self, value):
 
         if pd.isna(value) == False:
             value = humanize.naturalsize(value)
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/credentials.py` & `scalifiai-client-1.3.0a3/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,25 @@
             tf.double: DataType.FLOAT64,
             tf.complex64: DataType.COMPLEX64,
             tf.complex128: DataType.COMPLEX128,
             tf.string: DataType.STRING,
             tf.bool: DataType.BOOL,
             tf.variant: DataType.VARIANT,
         }
+    
+    @classmethod
+    def check_model_instance(cls, *, model_instance):
+
+        try:
+            import tensorflow as tf
+        except Exception:
+            print("Skipping Tensorflow check as Tensorflow installation is not detected")
+            return False
+        
+        return isinstance(model_instance, tf.keras.Model)
 
     def infer_data_type(self, *, dtype):
 
         data_type = self.DATA_TYPE_CONVERSION.get(dtype, None)
 
         if data_type == None:
             raise KerasInvalidDataTypeModelException(
@@ -211,15 +222,18 @@
                 model_version_instance = ModelVersion(
                     resp_data["id"], api_key=request_manager.credential_manager.api_key
                 )
 
                 for file in files_data:
 
                     model_version_instance.add_metadata_storage(
-                        data_type="file", key=file["file_relative_path"], file_path=file["file_full_path"], _model_core_file=True
+                        data_type="file",
+                        key=file["file_relative_path"],
+                        file_path=file["file_full_path"],
+                        _model_core_file=True,
                     )
 
             except Exception as ex:
                 model_instance.complete_model_version_creation(
                     version_id=resp_data["id"]
                 )
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,46 @@
 
         obj._value_ = value
         obj.verbose_name = verbose_name
         obj.wrapper_class = wrapper_class
 
         return obj
 
+    # KERAS = (
+    #     [
+    #         "keras.src.engine.sequential",
+    #         "keras.src.engine.functional",
+    #         "keras.src.models.sequential",
+    #         "keras.src.models.functional",
+    #         "tensorflow.python.keras.engine.sequential",
+    #         "tensorflow.python.keras.engine.functional",
+    #         "keras.engine.sequential",
+    #         "keras.engine.functional",
+    #     ],
+    #     "Keras - Tensorflow",
+    #     KerasModelWrapper,
+    # )
+
+    # @classmethod
+    # def match_model(cls, model):
+    #     for member in cls:
+    #         if model.__class__.__module__ in member.value:
+    #             return member
+    #     return None
+
     KERAS = (
-        [
-            "keras.src.engine.sequential",
-            "keras.src.engine.functional",
-            "keras.src.models.sequential",
-            "keras.src.models.functional",
-            "tensorflow.python.keras.engine.sequential",
-            "tensorflow.python.keras.engine.functional",
-            "keras.engine.sequential",
-            "keras.engine.functional"
-        ],
+        "keras",
         "Keras - Tensorflow",
         KerasModelWrapper,
     )
 
     @classmethod
     def match_model(cls, model):
         for member in cls:
-            if model.__class__.__module__ in member.value:
+            if member.wrapper_class.check_model_instance(model_instance=model):
                 return member
         return None
 
     @classmethod
     def match_key(cls, key):
         for member in cls:
             if key == member.wrapper_class.framework_key:
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/main.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,17 @@
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key in ["created_at", "updated_at"]:
                 final_value = pd.to_datetime(final_value)
                 if (datetime.now(self.local_timezone) - final_value).days > 0:
                     final_value = humanize.naturaldate(final_value)
                 else:
-                    final_value = humanize.naturaltime(final_value, when=datetime.now(self.local_timezone))
+                    final_value = humanize.naturaltime(
+                        final_value, when=datetime.now(self.local_timezone)
+                    )
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key == "properties__file_size":
                 final_value = humanize.naturalsize(final_value)
 
             html_content += f"<tr><th>{final_key}</th><td>{final_value}</td></tr>"
         html_content += "</table>"
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model/main.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,17 @@
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key in ["created_at", "updated_at"]:
                 final_value = pd.to_datetime(final_value)
                 if (datetime.now(self.local_timezone) - final_value).days > 0:
                     final_value = humanize.naturaldate(final_value)
                 else:
-                    final_value = humanize.naturaltime(final_value, when=datetime.now(self.local_timezone))
+                    final_value = humanize.naturaltime(
+                        final_value, when=datetime.now(self.local_timezone)
+                    )
 
             html_content += f"<tr><th>{final_key}</th><td>{final_value}</td></tr>"
         html_content += "</table>"
         return HTML(html_content)
 
     # TODO[VIMPORTANT] ADD THIS PROPERTY TO ALL SUB-MODULES
     @property
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,17 @@
 
             # TODO[VIMPORTANT] GENERALIZE THIS SO THAT WE CAN APPLY ANY FUNCTION TO ANY FIELDS BY SPECIFYINGIT IN THE VERBOSE COLUMNS CONFIG, CAN ALSO USE FUNCTIONS OF TABLE IN base.py
             if key in ["created_at", "updated_at"]:
                 final_value = pd.to_datetime(final_value)
                 if (datetime.now(self.local_timezone) - final_value).days > 0:
                     final_value = humanize.naturaldate(final_value)
                 else:
-                    final_value = humanize.naturaltime(final_value, when=datetime.now(self.local_timezone))
+                    final_value = humanize.naturaltime(
+                        final_value, when=datetime.now(self.local_timezone)
+                    )
 
             html_content += f"<tr><th>{final_key}</th><td>{final_value}</td></tr>"
         html_content += "</table>"
         return HTML(html_content)
 
     # TODO[VIMPORTANT] ADD THIS PROPERTY TO ALL SUB-MODULES
     @property
@@ -324,15 +326,17 @@
         else:
             raise_custom_exception(response=resp, action=self.add_metadata_url_slug)
 
         return Metadata(
             data["metadata_id"], api_key=self.request_manager.credential_manager.api_key
         )
 
-    def add_metadata_storage(self, *, data_type=None, key=None, file_path=None, _model_core_file=False):
+    def add_metadata_storage(
+        self, *, data_type=None, key=None, file_path=None, _model_core_file=False
+    ):
         self.validate()
 
         # TODO[VIMPORTANT] ADD CHECK FOR KWARGS TO THIS METHOD, THINK OF DOING THIS BY PYDANTIC
 
         try:
             metadata_obj = CreateMetadataStorage(
                 key=key, data_type=data_type, file_path=file_path
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai/request_manager.py` & `scalifiai-client-1.3.0a3/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a2/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.3.0a3/scalifiai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a2
+Version: 1.3.0a3
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a2/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.3.0a3/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

