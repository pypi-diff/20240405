# Comparing `tmp/c2-4apr24-0.1.0.tar.gz` & `tmp/c2-4apr24-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2-4apr24-0.1.0.tar", last modified: Thu Apr  4 13:11:49 2024, max compression
+gzip compressed data, was "c2-4apr24-0.1.1.tar", last modified: Fri Apr  5 10:34:54 2024, max compression
```

## Comparing `c2-4apr24-0.1.0.tar` & `c2-4apr24-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-04 13:11:49.009714 c2-4apr24-0.1.0/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.0/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1199 2024-04-04 13:11:49.008774 c2-4apr24-0.1.0/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.0/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-04 13:11:48.988983 c2-4apr24-0.1.0/c2_4apr24.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1199 2024-04-04 13:11:48.000000 c2-4apr24-0.1.0/c2_4apr24.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      369 2024-04-04 13:11:48.000000 c2-4apr24-0.1.0/c2_4apr24.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-04 13:11:48.000000 c2-4apr24-0.1.0/c2_4apr24.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-04 13:11:48.000000 c2-4apr24-0.1.0/c2_4apr24.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       10 2024-04-04 13:11:48.000000 c2-4apr24-0.1.0/c2_4apr24.egg-info/top_level.txt
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-04 13:11:48.993985 c2-4apr24-0.1.0/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       90 2024-04-04 12:18:52.000000 c2-4apr24-0.1.0/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      780 2024-04-04 10:26:37.000000 c2-4apr24-0.1.0/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     9995 2024-04-04 10:26:33.000000 c2-4apr24-0.1.0/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-04 13:11:49.000717 c2-4apr24-0.1.0/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      165 2024-04-04 12:18:42.000000 c2-4apr24-0.1.0/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7422 2024-04-04 10:33:55.000000 c2-4apr24-0.1.0/dqc/utils/_generic.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1359 2024-03-20 17:25:30.000000 c2-4apr24-0.1.0/dqc/utils/_sklearn_artifacts.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-04 13:11:49.009916 c2-4apr24-0.1.0/setup.cfg
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1499 2024-04-04 13:05:07.000000 c2-4apr24-0.1.0/setup.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-04 13:11:49.005603 c2-4apr24-0.1.0/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.0/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-02 16:16:44.000000 c2-4apr24-0.1.0/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2049 2024-04-04 10:33:55.000000 c2-4apr24-0.1.0/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.542894 c2-4apr24-0.1.1/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 c2-4apr24-0.1.1/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 10:34:54.542180 c2-4apr24-0.1.1/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 c2-4apr24-0.1.1/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.540517 c2-4apr24-0.1.1/c2_4apr24.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2514 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      384 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       88 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       10 2024-04-05 10:34:54.000000 c2-4apr24-0.1.1/c2_4apr24.egg-info/top_level.txt
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.528809 c2-4apr24-0.1.1/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       90 2024-04-04 12:18:52.000000 c2-4apr24-0.1.1/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      780 2024-04-04 10:26:37.000000 c2-4apr24-0.1.1/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     9971 2024-04-04 15:19:30.000000 c2-4apr24-0.1.1/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.533154 c2-4apr24-0.1.1/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      165 2024-04-04 12:18:42.000000 c2-4apr24-0.1.1/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7598 2024-04-04 15:16:35.000000 c2-4apr24-0.1.1/dqc/utils/_generic.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1359 2024-03-20 17:25:30.000000 c2-4apr24-0.1.1/dqc/utils/_sklearn_artifacts.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1218 2024-04-05 10:34:22.000000 c2-4apr24-0.1.1/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-05 10:34:54.543022 c2-4apr24-0.1.1/setup.cfg
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1499 2024-04-04 13:05:07.000000 c2-4apr24-0.1.1/setup.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-05 10:34:54.537585 c2-4apr24-0.1.1/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 c2-4apr24-0.1.1/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-02 16:16:44.000000 c2-4apr24-0.1.1/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2049 2024-04-04 10:33:55.000000 c2-4apr24-0.1.1/tests/test_crossval.py
```

### Comparing `c2-4apr24-0.1.0/LICENSE` & `c2-4apr24-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.0/dqc/base.py` & `c2-4apr24-0.1.1/dqc/base.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.0/dqc/crossval.py` & `c2-4apr24-0.1.1/dqc/crossval.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,14 @@
         """
         super().__init__(**options)
         self.n_splits = n_splits
         self.curate_pipeline = None
         self.scaler = None
         self.y_col_name_int = None
         self.result_col_list = [
-            "text",
-            "label",
             "label_correctness_score",
             "is_label_correct",
             "predicted_label",
             "prediction_probability",
         ]
 
     def __str__(self):
@@ -267,8 +265,8 @@
         )
 
         logger.info("Identifying the correctly labelled samples..")
         data_with_noisy_labels["is_label_correct"] = (
             data_with_noisy_labels.progress_apply(self._is_confident, axis=1)
         )
 
-        return dp._postprocess(display_cols=self.result_col_list)
+        return dp._postprocess(display_cols=[data_columns] + self.result_col_list)
```

### Comparing `c2-4apr24-0.1.0/dqc/utils/_generic.py` & `c2-4apr24-0.1.1/dqc/utils/_generic.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,17 @@
         y_col_name: str = "label",
         y_col_name_int: str = "label_int",
     ):
         self.df = df
         self.random_state = random_state
         self.y_col_name = y_col_name
         self.y_col_name_int = y_col_name_int
+        
         self.newly_added_cols = set([])
+        self.row_id_col = None
 
     def _generate_random_suffix(self, length=3):
         """
         Generates and returns a unique string with letters and/or digits.
 
         Parameters:
             length (int): Length of the string (default is 3)
@@ -219,14 +221,15 @@
 
         self._convert_labels_to_int()
 
         if not self.random_state:
             return self.df, None, self.y_col_name_int
 
         row_id_col = self._add_row_id()
+        self.row_id_col = row_id_col
         self._shuffle_data()
 
         return self.df, row_id_col, self.y_col_name_int
 
     def _postprocess(self, display_cols: List[str]) -> pd.DataFrame:
         """Removes redundant columns and returns dataframe
         with selected columns to display
@@ -236,8 +239,10 @@
             display_cols (List[str]): _description_
 
         Returns:
             pd.DataFrame: _description_
         """
 
         self.df = self.df.drop(columns=self.newly_added_cols)
-        return self.df[display_cols]
+        return self.df[display_cols]\
+                    .sort_values(by=self.row_id_col)\
+                    .reset_index(drop=True)
```

### Comparing `c2-4apr24-0.1.0/dqc/utils/_sklearn_artifacts.py` & `c2-4apr24-0.1.1/dqc/utils/_sklearn_artifacts.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.0/setup.py` & `c2-4apr24-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `c2-4apr24-0.1.0/tests/test_crossval.py` & `c2-4apr24-0.1.1/tests/test_crossval.py`

 * *Files identical despite different names*

