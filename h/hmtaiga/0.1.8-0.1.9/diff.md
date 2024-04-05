# Comparing `tmp/hmtaiga-0.1.8.tar.gz` & `tmp/hmtaiga-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.8.tar", last modified: Thu Apr  4 03:07:09 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.9.tar", last modified: Fri Apr  5 05:31:48 2024, max compression
```

## Comparing `hmtaiga-0.1.8.tar` & `hmtaiga-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.766259 hmtaiga-0.1.8/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 03:07:09.766088 hmtaiga-0.1.8/PKG-INFO
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.762482 hmtaiga-0.1.8/auth/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/auth/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      895 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/auth/authenticate.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765921 hmtaiga-0.1.8/hmtaiga.egg-info/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 shikhaverma   (501) staff       (20)      608 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       51 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/top_level.txt
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763340 hmtaiga-0.1.8/issues/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/issues/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2328 2024-03-25 04:07:28.000000 hmtaiga-0.1.8/issues/get_issues.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763632 hmtaiga-0.1.8/milestone/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/milestone/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      644 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/milestone/get_milestone.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763915 hmtaiga-0.1.8/project/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/project/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/project/getProjectBySlug.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-04 03:07:09.766297 hmtaiga-0.1.8/setup.cfg
--rw-r--r--   0 shikhaverma   (501) staff       (20)      183 2024-04-04 03:04:50.000000 hmtaiga-0.1.8/setup.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.764439 hmtaiga-0.1.8/tasks/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765363 hmtaiga-0.1.8/test/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     8896 2024-04-04 03:04:40.000000 hmtaiga-0.1.8/test/test_getIssues.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      939 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_getProjectBySlug.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      527 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_milestone.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765706 hmtaiga-0.1.8/userStory/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/getBusinessValue.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/get_user_story_history.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.449163 hmtaiga-0.1.9/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-05 05:31:48.448971 hmtaiga-0.1.9/PKG-INFO
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.445257 hmtaiga-0.1.9/auth/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/auth/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      895 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/auth/authenticate.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.448762 hmtaiga-0.1.9/hmtaiga.egg-info/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-05 05:31:48.000000 hmtaiga-0.1.9/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      608 2024-04-05 05:31:48.000000 hmtaiga-0.1.9/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        1 2024-04-05 05:31:48.000000 hmtaiga-0.1.9/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       51 2024-04-05 05:31:48.000000 hmtaiga-0.1.9/hmtaiga.egg-info/top_level.txt
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.446068 hmtaiga-0.1.9/issues/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/issues/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     2328 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/issues/get_issues.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.446375 hmtaiga-0.1.9/milestone/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/milestone/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      644 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/milestone/get_milestone.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.446645 hmtaiga-0.1.9/project/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/project/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     1213 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/project/getProjectBySlug.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       38 2024-04-05 05:31:48.449206 hmtaiga-0.1.9/setup.cfg
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      183 2024-04-05 05:31:42.000000 hmtaiga-0.1.9/setup.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.447035 hmtaiga-0.1.9/tasks/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/tasks/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     5914 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/tasks/get_task_history.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     2446 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/tasks/get_tasks.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.447978 hmtaiga-0.1.9/test/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     8896 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/test_getIssues.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      939 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/test_getProjectBySlug.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      527 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/test_get_milestone.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     4839 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/test_get_task_history.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     4571 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/test/test_get_tasks.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:31:48.448423 hmtaiga-0.1.9/userStory/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/userStory/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      855 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/userStory/getBusinessValue.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     2298 2024-04-05 05:19:49.000000 hmtaiga-0.1.9/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.8/auth/authenticate.py` & `hmtaiga-0.1.9/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/hmtaiga.egg-info/SOURCES.txt` & `hmtaiga-0.1.9/hmtaiga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/issues/get_issues.py` & `hmtaiga-0.1.9/issues/get_issues.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/milestone/get_milestone.py` & `hmtaiga-0.1.9/milestone/get_milestone.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/project/getProjectBySlug.py` & `hmtaiga-0.1.9/project/getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/tasks/get_task_history.py` & `hmtaiga-0.1.9/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/tasks/get_tasks.py` & `hmtaiga-0.1.9/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/test/test_getIssues.py` & `hmtaiga-0.1.9/test/test_getIssues.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/test/test_getProjectBySlug.py` & `hmtaiga-0.1.9/test/test_getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/test/test_get_milestone.py` & `hmtaiga-0.1.9/test/test_get_milestone.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/test/test_get_task_history.py` & `hmtaiga-0.1.9/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/test/test_get_tasks.py` & `hmtaiga-0.1.9/test/test_get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/userStory/getBusinessValue.py` & `hmtaiga-0.1.9/userStory/getBusinessValue.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.8/userStory/get_user_story_history.py` & `hmtaiga-0.1.9/userStory/get_user_story_history.py`

 * *Files identical despite different names*

