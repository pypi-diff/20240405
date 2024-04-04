# Comparing `tmp/pysparkpipe-0.1.3.tar.gz` & `tmp/pysparkpipe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkpipe-0.1.3.tar", max compression
+gzip compressed data, was "pysparkpipe-0.1.4.tar", max compression
```

## Comparing `pysparkpipe-0.1.3.tar` & `pysparkpipe-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      818 2023-09-12 16:07:27.630863 pysparkpipe-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      163 2023-09-12 16:07:27.630863 pysparkpipe-0.1.3/pysparkpipe/__init__.py
--rw-r--r--   0        0        0     2274 2023-09-12 16:07:27.630863 pysparkpipe-0.1.3/pysparkpipe/exc.py
--rw-r--r--   0        0        0       75 2023-09-12 16:07:27.630863 pysparkpipe-0.1.3/pysparkpipe/pipeline/__init__.py
--rw-r--r--   0        0        0     4385 2023-09-12 16:07:27.630863 pysparkpipe-0.1.3/pysparkpipe/pipeline/layers.py
--rw-r--r--   0        0        0     9541 2023-09-12 16:07:27.634863 pysparkpipe-0.1.3/pysparkpipe/pipeline/pipeline.py
--rw-r--r--   0        0        0     4017 2023-09-12 16:07:27.634863 pysparkpipe-0.1.3/pysparkpipe/pipeline/utils.py
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 pysparkpipe-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      818 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/__init__.py
+-rw-r--r--   0        0        0     2274 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/exc.py
+-rw-r--r--   0        0        0       75 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/pipeline/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/pipeline/layers.py
+-rw-r--r--   0        0        0    10771 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4225 2024-04-04 22:50:19.753810 pysparkpipe-0.1.4/pysparkpipe/pipeline/utils.py
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 pysparkpipe-0.1.4/PKG-INFO
```

### Comparing `pysparkpipe-0.1.3/pyproject.toml` & `pysparkpipe-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name ="pysparkpipe"
-version = "0.1.3"
+version = "0.1.4"
 description = "Flow orchestrator for data transformations within the context of pyspark.sql.GroupedData.applyInPandas"
 authors = ["Santiago Armstrong <santiagoarmstrong@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pyspark = ">=3.2.1"
 pandas = ">=1.4.3,<2.0.0"
```

### Comparing `pysparkpipe-0.1.3/pysparkpipe/exc.py` & `pysparkpipe-0.1.4/pysparkpipe/exc.py`

 * *Files identical despite different names*

### Comparing `pysparkpipe-0.1.3/pysparkpipe/pipeline/layers.py` & `pysparkpipe-0.1.4/pysparkpipe/pipeline/layers.py`

 * *Files identical despite different names*

### Comparing `pysparkpipe-0.1.3/pysparkpipe/pipeline/pipeline.py` & `pysparkpipe-0.1.4/pysparkpipe/pipeline/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 """Spark applyInPandas Pipeline class"""
 
+import concurrent.futures
+import logging
 from typing import List, Optional, Union
 
 from pandas import DataFrame as PandasDataFrame
 from pandera import DataFrameSchema
 from pyspark.sql import DataFrame as SparkDataFrame
 from typeguard import typechecked
 
@@ -15,48 +17,53 @@
 )
 from pysparkpipe.pipeline.layers import Layer
 from pysparkpipe.pipeline.utils import (
     pandera_model_to_spark_structype,
     parse_dataframe_using_pandera_model,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class Pipeline:
     """Pipeline class. A pipeline is a sequence of layers that are applied to the data grouped by the grouping columns."""
 
     @typechecked
     def __init__(
         self,
         grouping_cols: List[str],
         validate_inputs: bool = True,
         validate_outputs: bool = True,
         exception_handler: Optional[callable] = None,
+        timeout: Optional[int] = None,
     ) -> None:
         """Pipeline constructor.
 
         Args:
             grouping_cols (List[str]): List of grouping columns.
             validate_inputs (bool, optional): If True, by default the inner Layers will validate the input dataframes. Defaults to True.
             validate_outputs (bool, optional): If True, by defualt the inner Layers will validate the output dataframes. Defaults to True.
             exception_handler (callable, optional): Exception handler to be used by the pipeline. Defaults to None. If passed, the pipeline
                 will call the exception_handler with the dataframe and the exception as arguments. The exception_handler should return a dataframe.
                 with the same schema as the output schema of the pipeline. If the exception_handler is not passed, the pipeline will raise the exception.
                 NOTE: exception_handler(e: Exception, df: PandasDataFrame) -> PandasDataFrame will not be typechecked.
+            timeout (int, optional): Timeout in seconds for the pipeline to run. Defaults to None.
 
         Raises:
             ValueError: If grouping_cols is not a list of strings.
             ValueError: If validate_inputs is not a boolean.
             ValueError: If validate_outputs is not a boolean.
         """
 
         self.grouping_cols = grouping_cols  # type: List[str]
         self.layers = []  # type: List[Layer]
         self.validate_inputs = validate_inputs  # type: bool
         self.validate_outputs = validate_outputs  # type: bool
         self._exception_handler = exception_handler  # type: Optional[callable]
+        self.timeout = timeout  # type: Optional[int]
 
     def add_layer(
         self,
         new_layer: Layer,
     ):
         # assert new_layer is consistent with previous layers
         if len(self.layers) > 0:
@@ -174,25 +181,36 @@
             df_exc = parse_dataframe_using_pandera_model(
                 self.output_schema, df_exc
             )
             return df_exc
         else:
             raise e
 
-    def fit(
+    def _apply_layers(
         self, df: Union[PandasDataFrame, List[PandasDataFrame]]
     ) -> PandasDataFrame:
-        """Fit the pipeline to the data. Apply all layers to the data to a single group."""
+        """Apply all layers to the data to a single group."""
         _df = df.copy()
+        for layer in self.layers:
+            _df = layer.transform(_df)
+        return _df
+
+    def fit(
+        self, df: Union[PandasDataFrame, List[PandasDataFrame]]
+    ) -> PandasDataFrame:
+        """Fit the pipeline to the data. Apply all layers to the data to a single group with an optional timeout."""
         try:
-            for layer in self.layers:
-                _df = layer.transform(_df)
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                future = executor.submit(self._apply_layers, df)
+                result = future.result(
+                    timeout=self.timeout
+                )  # Set the timeout here (in seconds)
+            return result
         except Exception as e:
-            return self.exception_handler(e, df)  # type: PandasDataFrame
-        return _df
+            return self.exception_handler(e, df)
 
     @typechecked
     def apply_in_pandas(self, df: PandasDataFrame) -> PandasDataFrame:
         """Apply the pipeline to the data using pandas 'groupby'. Apply all layers to the data grouped by the grouping columns.
 
         Args:
             df (DataFrame): DataFrame to apply the pipeline to.
@@ -240,7 +258,20 @@
             def to_apply(key, df):
                 return self.fit(df)
 
         return grouped_df.applyInPandas(
             to_apply,
             schema=pandera_model_to_spark_structype(self.output_schema),
         )
+
+    def __repr__(self) -> str:
+        rep = "PySparkPipe Pipeline\n"
+        for layer in self.layers:
+            rep += f"Layer: {layer.name}\n"
+            rep += f"Input Schema: {layer.input_schema}\n"
+            rep += f"Output Schema: {layer.output_schema}\n"
+            rep += f"Transform: {layer.transform}\n"
+            rep += f"Validate Input: {layer.validate_input}\n"
+            rep += f"Validate Output: {layer.validate_output}\n"
+            rep += "\n"
+
+        return rep
```

### Comparing `pysparkpipe-0.1.3/pysparkpipe/pipeline/utils.py` & `pysparkpipe-0.1.4/pysparkpipe/pipeline/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     cls: DataFrameSchema,
     spark: SparkSession,
     df: Union[pd.DataFrame, Dict, List[Dict]],
 ) -> pyspark.sql.DataFrame:
     """It converts the input into a spark dataframe following the class schema. Accept dictionaries, lists or dataframes as input.
 
     Args:
+        cls (DataFrameSchema): Pandera class schema
         spark (SparkSession): SparkSession
         df (Union[pd.DataFrame,Dict, List[Dict]]): Input data
 
     Returns:
         pyspark.sql.DataFrame: Spark dataframe with the class schema
     """
     # parse and validate the input
@@ -65,14 +66,15 @@
     Initializes dataframe from dict. Wrapper for pd.DataFrame() that adds the
     dtype=object argument to avoid unasked type-castings.
 
     After creating the dataframe, it is parsed (with the parse method), according
     to the schema.
 
     Args:
+        cls (DataFrameSchema): Pandera class schema
         data (Union[List[Dict], Dict]): Dict, List of Dicts, or actually whatever
         input pd.DataFrame wouldn't sneeze at. In extra kwargs are required for
         compatibility, bring on the extra arguments, not gonna cry about that.
 
     Returns:
         pd.DataFrame: DataFrame post parsing.
     """
@@ -85,14 +87,15 @@
     cls: DataFrameSchema, df: pd.DataFrame
 ) -> pd.DataFrame:
     """
     Parses DataFrame, adding required columns and doing valid type conversions
     according to schema typing. Includes a validation
 
     Args:
+        cls (DataFrameSchema): Pandera class schema
         df (pd.DataFrame): pandas DataFrame
 
     Returns:
         pd.DataFrame: pandas DataFrame with correct types according to schema.
     """
     # Add missing columns to dataframe as empty columns
     df_cols = df.columns
@@ -108,14 +111,15 @@
 def pandera_model_to_spark_structype(
     cls: DataFrameSchema, df_cols: List[str] = None
 ) -> StructType:
     """
     Returns spark StructType with schema or corresponding Pandera schema.
 
     Args:
+        cls (DataFrameSchema): Pandera class schema
         df_cols (Optional[List[str]], optional): List of DataFrame col names of corresponding schema,
         useful for returning StructType with a particular column order.
         Defaults to None. If None, uses default schema column ordering.
 
     Returns:
         StructType: schema for pyspark DataFrame
     """
```

### Comparing `pysparkpipe-0.1.3/PKG-INFO` & `pysparkpipe-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pysparkpipe
-Version: 0.1.3
+Version: 0.1.4
 Summary: Flow orchestrator for data transformations within the context of pyspark.sql.GroupedData.applyInPandas
 Author: Santiago Armstrong
 Author-email: santiagoarmstrong@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pandera (>=0.16.1,<0.17.0)
 Requires-Dist: pyarrow (>=7.0.0)
 Requires-Dist: pyspark (>=3.2.1)
 Requires-Dist: typeguard (>=4.1.1,<5.0.0)
```

