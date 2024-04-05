# Comparing `tmp/c2-4apr24-0.1.1.tar.gz` & `tmp/c2-4apr24-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2-4apr24-0.1.1.tar", last modified: Fri Apr  5 10:34:54 2024, max compression
+gzip compressed data, was "c2-4apr24-0.1.2.tar", last modified: Fri Apr  5 12:34:02 2024, max compression
```

## Comparing `c2-4apr24-0.1.1.tar` & `c2-4apr24-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.542894 c2-4apr24-0.1.1/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.1/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 10:34:54.542180 c2-4apr24-0.1.1/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.1/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.540517 c2-4apr24-0.1.1/c2_4apr24.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      384 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       10 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/top_level.txt
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.528809 c2-4apr24-0.1.1/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       90 2024-04-04 12:18:52.000000 c2-4apr24-0.1.1/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      780 2024-04-04 10:26:37.000000 c2-4apr24-0.1.1/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     9971 2024-04-04 15:19:30.000000 c2-4apr24-0.1.1/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.533154 c2-4apr24-0.1.1/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      165 2024-04-04 12:18:42.000000 c2-4apr24-0.1.1/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7598 2024-04-04 15:16:35.000000 c2-4apr24-0.1.1/dqc/utils/_generic.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1359 2024-03-20 17:25:30.000000 c2-4apr24-0.1.1/dqc/utils/_sklearn_artifacts.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1218 2024-04-05 10:34:22.000000 c2-4apr24-0.1.1/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-05 10:34:54.543022 c2-4apr24-0.1.1/setup.cfg
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1499 2024-04-04 13:05:07.000000 c2-4apr24-0.1.1/setup.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.537585 c2-4apr24-0.1.1/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.1/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-02 16:16:44.000000 c2-4apr24-0.1.1/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2049 2024-04-04 10:33:55.000000 c2-4apr24-0.1.1/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.478655 c2-4apr24-0.1.2/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 12:34:02.477997 c2-4apr24-0.1.2/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.2/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.475906 c2-4apr24-0.1.2/c2_4apr24.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      384 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       10 2024-04-05 12:34:02.000000 c2-4apr24-0.1.2/c2_4apr24.egg-info/top_level.txt
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.460636 c2-4apr24-0.1.2/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       90 2024-04-04 12:18:52.000000 c2-4apr24-0.1.2/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      780 2024-04-04 10:26:37.000000 c2-4apr24-0.1.2/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     9969 2024-04-05 10:58:22.000000 c2-4apr24-0.1.2/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.467346 c2-4apr24-0.1.2/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      165 2024-04-04 12:18:42.000000 c2-4apr24-0.1.2/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7732 2024-04-05 12:08:02.000000 c2-4apr24-0.1.2/dqc/utils/_generic.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1359 2024-03-20 17:25:30.000000 c2-4apr24-0.1.2/dqc/utils/_sklearn_artifacts.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1218 2024-04-05 12:32:16.000000 c2-4apr24-0.1.2/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-05 12:34:02.478942 c2-4apr24-0.1.2/setup.cfg
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1499 2024-04-04 13:05:07.000000 c2-4apr24-0.1.2/setup.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 12:34:02.474185 c2-4apr24-0.1.2/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.2/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-02 16:16:44.000000 c2-4apr24-0.1.2/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2097 2024-04-05 11:56:12.000000 c2-4apr24-0.1.2/tests/test_crossval.py
```

### Comparing `c2-4apr24-0.1.1/LICENSE` & `c2-4apr24-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.1/PKG-INFO` & `c2-4apr24-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2-4apr24
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Quality Check for Machine Learning
 Home-page: https://github.com/sumanthprabhu/C2
 Author: Sumanth S Prabhu
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
```

### Comparing `c2-4apr24-0.1.1/c2_4apr24.egg-info/PKG-INFO` & `c2-4apr24-0.1.2/c2_4apr24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2-4apr24
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data Quality Check for Machine Learning
 Home-page: https://github.com/sumanthprabhu/C2
 Author: Sumanth S Prabhu
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
```

### Comparing `c2-4apr24-0.1.1/dqc/base.py` & `c2-4apr24-0.1.2/dqc/base.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.1/dqc/crossval.py` & `c2-4apr24-0.1.2/dqc/crossval.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,8 +265,8 @@
         )
 
         logger.info("Identifying the correctly labelled samples..")
         data_with_noisy_labels["is_label_correct"] = (
             data_with_noisy_labels.progress_apply(self._is_confident, axis=1)
         )
 
-        return dp._postprocess(display_cols=[data_columns] + self.result_col_list)
+        return dp._postprocess(display_cols=data_columns + self.result_col_list)
```

### Comparing `c2-4apr24-0.1.1/dqc/utils/_generic.py` & `c2-4apr24-0.1.2/dqc/utils/_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,17 @@
     def _shuffle_data(self) -> pd.DataFrame:
         """_summary_
 
         Returns:
             pd.DataFrame: _description_
         """
         # Shuffle the dataframe
-        self.df = self.df.sample(frac=1.0, random_state=self.random_state)
+        self.df = self.df.sample(frac=1.0, 
+                                 random_state=self.random_state)\
+                         .reset_index(drop=True)
 
         return
 
     def _convert_labels_to_int(self):
         """
         Map string labels to integers for downstream processing and return the updated DataFrame
         along with the mapping dictionary.
@@ -237,12 +239,16 @@
         Args:
             df (pd.DataFrame): _description_
             display_cols (List[str]): _description_
 
         Returns:
             pd.DataFrame: _description_
         """
-
-        self.df = self.df.drop(columns=self.newly_added_cols)
-        return self.df[display_cols]\
-                    .sort_values(by=self.row_id_col)\
-                    .reset_index(drop=True)
+        
+        res = self.df
+        row_id_col = self.row_id_col
+
+        if not row_id_col:
+            return res[display_cols]
+        
+        return res.sort_values(by=[row_id_col])\
+                    .reset_index(drop=True)[display_cols]
```

### Comparing `c2-4apr24-0.1.1/dqc/utils/_sklearn_artifacts.py` & `c2-4apr24-0.1.2/dqc/utils/_sklearn_artifacts.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.1/pyproject.toml` & `c2-4apr24-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c2-4apr24"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `c2-4apr24-0.1.1/setup.py` & `c2-4apr24-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.1/tests/test_crossval.py` & `c2-4apr24-0.1.2/tests/test_crossval.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 @pytest.mark.parametrize("random_state", [None, 1])
 def test_crossvalcurate_success(
     data, curate_representation, curate_model, calibration_method, random_state
 ):
     cvc = CrossValCurate(
         calibration_method=calibration_method, random_state=random_state
     )
-    data = cvc.fit_transform(data)
+    data_curated = cvc.fit_transform(data)
 
     # Check if dataframe is return
-    assert type(data) == pd.DataFrame
+    assert type(data_curated) == pd.DataFrame
 
     # Check column presence
     assert all(
-        col in data.columns
+        col in data_curated.columns
         for col in [
             "prediction_probability",
             "predicted_label",
             "label_correctness_score",
             "is_label_correct",
         ]
     )
 
     # Check data types
     assert all(
-        data[col].dtype == dtype
+        data_curated[col].dtype == dtype
         for col, dtype in [
             ("prediction_probability", float),
             ("label_correctness_score", float),
             ("is_label_correct", bool),
         ]
     )
 
     # Check non-null values
     assert all(
-        data[col].notnull().all()
+        data_curated[col].notnull().all()
         for col in [
             "prediction_probability",
             "predicted_label",
             "label_correctness_score",
             "is_label_correct",
         ]
     )
@@ -64,8 +64,8 @@
 def test_crossvalcurate_failure(
     data, curate_representation, curate_model, calibration_method, random_state
 ):
     with pytest.raises(ValueError):
         cvc = CrossValCurate(
             calibration_method=calibration_method, random_state=random_state
         )
-        data = cvc.fit_transform(data)
+        data_curated = cvc.fit_transform(data)
```

