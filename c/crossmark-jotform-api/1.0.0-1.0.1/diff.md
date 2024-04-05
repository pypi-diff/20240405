# Comparing `tmp/crossmark-jotform-api-1.0.0.tar.gz` & `tmp/crossmark-jotform-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-1.0.0.tar", last modified: Fri Apr  5 13:25:30 2024, max compression
+gzip compressed data, was "crossmark-jotform-api-1.0.1.tar", last modified: Fri Apr  5 14:06:29 2024, max compression
```

## Comparing `crossmark-jotform-api-1.0.0.tar` & `crossmark-jotform-api-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:25:30.839792 crossmark-jotform-api-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-04-05 12:44:23.000000 crossmark-jotform-api-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2173 2024-04-05 13:25:30.837253 crossmark-jotform-api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-05 13:08:51.000000 crossmark-jotform-api-1.0.0/README.md
--rw-rw-rw-   0        0        0      828 2024-04-05 13:20:41.000000 crossmark-jotform-api-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 13:25:30.839792 crossmark-jotform-api-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 13:25:30.769292 crossmark-jotform-api-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:25:30.792238 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    16774 2024-04-05 13:06:55.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:25:30.834253 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2173 2024-04-05 13:25:30.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-04-05 13:25:30.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:25:30.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 13:25:30.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-05 13:25:30.000000 crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 14:06:29.590551 crossmark-jotform-api-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 12:44:23.000000 crossmark-jotform-api-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2173 2024-04-05 14:06:29.589531 crossmark-jotform-api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-05 13:08:51.000000 crossmark-jotform-api-1.0.1/README.md
+-rw-rw-rw-   0        0        0      829 2024-04-05 14:05:16.000000 crossmark-jotform-api-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:06:29.590551 crossmark-jotform-api-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 14:06:29.529715 crossmark-jotform-api-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 14:06:29.550729 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    16770 2024-04-05 14:04:52.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:06:29.587531 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2173 2024-04-05 14:06:29.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-05 14:06:29.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:06:29.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-05 14:06:29.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-05 14:06:29.000000 crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-1.0.0/LICENSE` & `crossmark-jotform-api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-1.0.0/PKG-INFO` & `crossmark-jotform-api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-1.0.0/pyproject.toml` & `crossmark-jotform-api-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "1.0.0"
+version = "1.0.01"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-1.0.0/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-1.0.1/src/crossmark_jotform_api/jotForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,21 +60,21 @@
         return requests.get("https://api.jotform.com/submission/" +
                      submission_id + "?apiKey=" + self.api_key, timeout=self.timeout)
 
     def get_submission(self, submission_id):
         return self.submission_data[submission_id]
 
     def get_submission_id_by_text(self, text):
-        for key, submission_object in self.submission_data.items():
+        for _, submission_object in self.submission_data.items():
             if submission_object.get_answer_by_text(text):
                 return submission_object
         return None
 
     def get_submission_by_case_id(self, case_id, tried=0):
-        for key, submission_object in self.submission_data.items():
+        for _, submission_object in self.submission_data.items():
             if submission_object.case_id == case_id:
                 return submission_object
         if not tried:
             self.request_submission_by_case_id(case_id)
             return self.get_submission_by_case_id(case_id, 1)
         return None
```

### Comparing `crossmark-jotform-api-1.0.0/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-1.0.1/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

