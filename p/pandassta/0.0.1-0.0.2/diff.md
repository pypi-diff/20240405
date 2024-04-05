# Comparing `tmp/pandassta-0.0.1.tar.gz` & `tmp/pandassta-0.0.2.tar.gz`

## Comparing `pandassta-0.0.1.tar` & `pandassta-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pandassta-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pandassta-0.0.1/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pandassta-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pandassta-0.0.1/src/pandassta/__init__.py
--rw-r--r--   0        0        0    14439 2020-02-02 00:00:00.000000 pandassta-0.0.1/src/pandassta/df.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pandassta-0.0.1/src/pandassta/logging_constants.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pandassta-0.0.1/src/pandassta/sta.py
--rw-r--r--   0        0        0    21143 2020-02-02 00:00:00.000000 pandassta-0.0.1/src/pandassta/sta_requests.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/test_df.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/test_queries.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/test_sta.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/conf/conf_base.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/data_velocity_acc.csv
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/response_with_nextlink.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/single_datastream_response_missing_resultquality.json
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/test_response.json
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/test_response_noF.json
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/test_response_obs_wF.json
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 pandassta-0.0.1/tests/resources/test_response_wF.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pandassta-0.0.1/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 pandassta-0.0.1/LICENSE
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pandassta-0.0.1/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pandassta-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pandassta-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pandassta-0.0.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pandassta-0.0.2/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pandassta-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/__init__.py
+-rw-r--r--   0        0        0    14888 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/df.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/logging_constants.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/sta.py
+-rw-r--r--   0        0        0    21143 2020-02-02 00:00:00.000000 pandassta-0.0.2/src/pandassta/sta_requests.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_df.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_queries.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/test_sta.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/conf/conf_base.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/data_velocity_acc.csv
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/response_with_nextlink.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/single_datastream_response_missing_resultquality.json
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response.json
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_noF.json
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_obs_wF.json
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 pandassta-0.0.2/tests/resources/test_response_wF.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pandassta-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 pandassta-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pandassta-0.0.2/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pandassta-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pandassta-0.0.2/PKG-INFO
```

### Comparing `pandassta-0.0.1/Makefile` & `pandassta-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/src/pandassta/df.py` & `pandassta-0.0.2/src/pandassta/df.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,14 +102,38 @@
     def __str__(self):
         return f"{self.value}"
 
 
 CAT_TYPE = CategoricalDtype(list(QualityFlags), ordered=True)
 
 
+def process_feature_column(df: pd.DataFrame) -> pd.DataFrame:
+    try:
+        df_features = pd.json_normalize(df.pop(str(Entities.FEATUREOFINTEREST))) # type: ignore
+        try:
+            df_features = df_features.rename( 
+            columns={Df.IOT_ID: Df.FEATURE_ID},
+            errors="raise"
+        )
+        except KeyError as e:
+            df_features[Df.FEATURE_ID] = None
+
+        df_coordinates = pd.DataFrame(
+            df_features.pop("feature.coordinates").values.tolist(),
+            columns=[Df.LONG, Df.LAT],
+        )
+        df_features = df_features.join(df_coordinates)
+        df = df.join(df_features)
+
+    except KeyError as e:
+        df[[Df.FEATURE_ID, Df.LONG, Df.LAT]] = [None, None, None]
+
+    return df
+
+
 def response_single_datastream_to_df(response_datastream: dict) -> pd.DataFrame:
     df = pd.DataFrame()
     observations_list = response_datastream.get(Entities.OBSERVATIONS, [])
     log.debug(f"{observations_list=}")
     if observations_list:
         df_i = pd.DataFrame(observations_list).astype(
             {Properties.IOT_ID: int, Df.RESULT: float}
@@ -135,28 +159,22 @@
         df_i[Df.OBSERVATION_TYPE] = response_datastream.get(
             Entities.OBSERVEDPROPERTY, {}
         ).get(Properties.NAME)
         df_i[Df.OBSERVED_PROPERTY_ID] = response_datastream.get(
             Entities.OBSERVEDPROPERTY, {}
         ).get(Properties.IOT_ID)
         df_i[Df.OBSERVATION_TYPE] = df_i[Df.OBSERVATION_TYPE].astype("category")
-        k1, k2 = Properties.UNITOFMEASUREMENT.split("/", 1)
+        k1, k2 = Properties.UNITOFMEASUREMENT.split(
+            "/", 1
+        )  # could be improved by using df.join(pd.DataFrame(df.pop('COLUMNNAME').values.tolist()))
         df_i[Df.UNITS] = response_datastream.get(k1, {}).get(k2)
         df_i[Df.UNITS] = df_i[Df.UNITS].astype("category")
 
-        df_i[[Df.LONG, Df.LAT]] = pd.DataFrame.from_records(
-            df_i[str(Entities.FEATUREOFINTEREST)].apply(
-                lambda x: x.get("feature").get("coordinates")
-            )
-        )
-        df_i[Df.FEATURE_ID] = df_i[str(Entities.FEATUREOFINTEREST)].apply(
-            lambda x: x.get(str(Properties.IOT_ID))
-        )
-        del df_i[str(Entities.FEATUREOFINTEREST)]
-        # df_i.drop(columns=str(Entities.FEATUREOFINTEREST))
+        df_i = process_feature_column(df_i)
+
         df = pd.concat([df, df_i], ignore_index=True)
 
     return df
 
 
 # def response_datastreams_to_df(response: dict) -> pd.DataFrame:
 #     df_out = pd.DataFrame()
```

### Comparing `pandassta-0.0.1/src/pandassta/sta.py` & `pandassta-0.0.2/src/pandassta/sta.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/src/pandassta/sta_requests.py` & `pandassta-0.0.2/src/pandassta/sta_requests.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/test_df.py` & `pandassta-0.0.2/tests/test_df.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/test_queries.py` & `pandassta-0.0.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/test_sta.py` & `pandassta-0.0.2/tests/test_sta.py`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/data_velocity_acc.csv` & `pandassta-0.0.2/tests/resources/data_velocity_acc.csv`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/response_with_nextlink.json` & `pandassta-0.0.2/tests/resources/response_with_nextlink.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/single_datastream_response_missing_resultquality.json` & `pandassta-0.0.2/tests/resources/single_datastream_response_missing_resultquality.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/test_response.json` & `pandassta-0.0.2/tests/resources/test_response.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/test_response_noF.json` & `pandassta-0.0.2/tests/resources/test_response_noF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/test_response_obs_wF.json` & `pandassta-0.0.2/tests/resources/test_response_obs_wF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/tests/resources/test_response_wF.json` & `pandassta-0.0.2/tests/resources/test_response_wF.json`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/LICENSE` & `pandassta-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandassta-0.0.1/pyproject.toml` & `pandassta-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pandassta"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="nvds" },
 ]
 description = "Package for easy datarequests from sensortings"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

