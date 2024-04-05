# Comparing `tmp/vanna-0.3.2.tar.gz` & `tmp/vanna-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.3.2.tar` & `vanna-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     7922 2024-04-01 21:25:37.491082 vanna-0.3.2/README.md
--rw-r--r--   0        0        0     1205 2024-04-01 21:25:37.507082 vanna-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8906 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    54890 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8372 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      717 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    21212 2024-04-01 21:25:37.507082 vanna-0.3.2/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   180924 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/flask/assets.py
--rw-r--r--   0        0        0      313 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     3852 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0    12803 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     1472 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     5644 2024-04-01 21:25:37.511082 vanna-0.3.2/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0     9961 1970-01-01 00:00:00.000000 vanna-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     7922 2024-04-05 14:52:15.482886 vanna-0.3.3/README.md
+-rw-r--r--   0        0        0     1247 2024-04-05 14:52:15.498886 vanna-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8728 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    54875 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8453 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      717 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    21212 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   180924 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0      313 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0    12803 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     5644 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 vanna-0.3.3/PKG-INFO
```

### Comparing `vanna-0.3.2/README.md` & `vanna-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/pyproject.toml` & `vanna-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -27,15 +27,16 @@
 
 [project.optional-dependencies]
 postgres = ["psycopg2-binary", "db-dtypes"]
 mysql = ["PyMySQL"]
 bigquery = ["google-cloud-bigquery"]
 snowflake = ["snowflake-connector-python"]
 duckdb = ["duckdb"]
-all = ["psycopg2-binary", "db-dtypes", "PyMySQL", "google-cloud-bigquery", "snowflake-connector-python", "duckdb", "openai", "mistralai", "chromadb", "anthropic"]
+all = ["psycopg2-binary", "db-dtypes", "PyMySQL", "google-cloud-bigquery", "snowflake-connector-python", "duckdb", "openai", "mistralai", "chromadb", "anthropic", "zhipuai", "marqo"]
 test = ["tox"]
 chromadb = ["chromadb"]
 openai = ["openai"]
 mistralai = ["mistralai"]
 anthropic = ["anthropic"]
 gemini = ["google-generativeai"]
 marqo = ["marqo"]
+zhipuai = ["zhipuai"]
```

### Comparing `vanna-0.3.2/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,23 +216,18 @@
     ):
         if prompt is None:
             raise Exception("Prompt is None")
 
         if len(prompt) == 0:
             raise Exception("Prompt is empty")
 
-        client = ZhipuAI(api_key=self.api_key)  # 填写您自己的APIKey
+        client = ZhipuAI(api_key=self.api_key)
         response = client.chat.completions.create(
-            model="glm-4",  # 填写需要调用的模型名称
+            model="glm-4",
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             messages=prompt,
         )
-        # print(prompt)
-
-        # print(response)
-
-        # print(f"Cost {response.usage.total_tokens} token")
 
         return response.choices[0].message.content
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `vanna-0.3.2/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/__init__.py` & `vanna-0.3.3/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.3.3/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/base/base.py` & `vanna-0.3.3/src/vanna/base/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,38 +143,40 @@
 
         if "SELECT" in sql.upper():
             return True
         else:
             return False
 
     def generate_followup_questions(
-        self, question: str, sql: str, df: pd.DataFrame, **kwargs
+        self, question: str, sql: str, df: pd.DataFrame, n_questions: int = 5, **kwargs
     ) -> list:
         """
         **Example:**
         ```python
-        vn.generate_followup_questions("What are the top 10 customers by sales?", df)
+        vn.generate_followup_questions("What are the top 10 customers by sales?", sql, df)
         ```
 
         Generate a list of followup questions that you can ask Vanna.AI.
 
         Args:
             question (str): The question that was asked.
+            sql (str): The LLM-generated SQL query.
             df (pd.DataFrame): The results of the SQL query.
+            n_questions (int): Number of follow-up questions to generate.
 
         Returns:
             list: A list of followup questions that you can ask Vanna.AI.
         """
 
         message_log = [
             self.system_message(
                 f"You are a helpful data assistant. The user asked the question: '{question}'\n\nThe SQL query for this question was: {sql}\n\nThe following is a pandas DataFrame with the results of the query: \n{df.to_markdown()}\n\n"
             ),
             self.user_message(
-                "Generate a list of followup questions that the user might ask about this data. Respond with a list of questions, one per line. Do not answer with any explanations -- just the questions. Remember that there should be an unambiguous SQL query that can be generated from the question. Prefer questions that are answerable outside of the context of this conversation. Prefer questions that are slight modifications of the SQL query that was generated that allow digging deeper into the data. Each question will be turned into a button that the user can click to generate a new SQL query so don't use 'example' type questions. Each question must have a one-to-one correspondence with an instantiated SQL query."
+                f"Generate a list of {n_questions} followup questions that the user might ask about this data. Respond with a list of questions, one per line. Do not answer with any explanations -- just the questions. Remember that there should be an unambiguous SQL query that can be generated from the question. Prefer questions that are answerable outside of the context of this conversation. Prefer questions that are slight modifications of the SQL query that was generated that allow digging deeper into the data. Each question will be turned into a button that the user can click to generate a new SQL query so don't use 'example' type questions. Each question must have a one-to-one correspondence with an instantiated SQL query."
             ),
         ]
 
         llm_response = self.submit_prompt(message_log, **kwargs)
 
         numbers_removed = re.sub(r"^\d+\.\s*", "", llm_response, flags=re.MULTILINE)
         return numbers_removed.split("\n")
@@ -1300,20 +1302,22 @@
         ].to_list()[0]
         schema_column = df.columns[
             df.columns.str.lower().str.contains("table_schema")
         ].to_list()[0]
         table_column = df.columns[
             df.columns.str.lower().str.contains("table_name")
         ].to_list()[0]
-        column_column = df.columns[
-            df.columns.str.lower().str.contains("column_name")
-        ].to_list()[0]
-        data_type_column = df.columns[
-            df.columns.str.lower().str.contains("data_type")
-        ].to_list()[0]
+        columns = [database_column,
+                    schema_column,
+                    table_column]
+        candidates = ["column_name",
+                      "data_type",
+                      "comment"]
+        matches = df.columns.str.lower().str.contains("|".join(candidates), regex=True)
+        columns += df.columns[matches].to_list()
 
         plan = TrainingPlan([])
 
         for database in df[database_column].unique().tolist():
             for schema in (
                 df.query(f'{database_column} == "{database}"')[schema_column]
                 .unique()
@@ -1326,23 +1330,15 @@
                     .unique()
                     .tolist()
                 ):
                     df_columns_filtered_to_table = df.query(
                         f'{database_column} == "{database}" and {schema_column} == "{schema}" and {table_column} == "{table}"'
                     )
                     doc = f"The following columns are in the {table} table in the {database} database:\n\n"
-                    doc += df_columns_filtered_to_table[
-                        [
-                            database_column,
-                            schema_column,
-                            table_column,
-                            column_column,
-                            data_type_column,
-                        ]
-                    ].to_markdown()
+                    doc += df_columns_filtered_to_table[columns].to_markdown()
 
                     plan._plan.append(
                         TrainingPlanItem(
                             item_type=TrainingPlanItem.ITEM_TYPE_IS,
                             item_group=f"{database}.{schema}",
                             item_name=table,
                             item_value=doc,
```

### Comparing `vanna-0.3.2/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.3.3/src/vanna/chromadb/chromadb_vector.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import chromadb
 import pandas as pd
 from chromadb.config import Settings
 from chromadb.utils import embedding_functions
 
 from ..base import VannaBase
+from ..utils import deterministic_uuid
 
 default_ef = embedding_functions.DefaultEmbeddingFunction()
 
 
 class ChromaDB_VectorStore(VannaBase):
     def __init__(self, config=None):
         VannaBase.__init__(self, config=config)
@@ -61,34 +62,34 @@
         question_sql_json = json.dumps(
             {
                 "question": question,
                 "sql": sql,
             },
             ensure_ascii=False,
         )
-        id = str(uuid.uuid4()) + "-sql"
+        id = deterministic_uuid(question_sql_json) + "-sql"
         self.sql_collection.add(
             documents=question_sql_json,
             embeddings=self.generate_embedding(question_sql_json),
             ids=id,
         )
 
         return id
 
     def add_ddl(self, ddl: str, **kwargs) -> str:
-        id = str(uuid.uuid4()) + "-ddl"
+        id = deterministic_uuid(ddl) + "-ddl"
         self.ddl_collection.add(
             documents=ddl,
             embeddings=self.generate_embedding(ddl),
             ids=id,
         )
         return id
 
     def add_documentation(self, documentation: str, **kwargs) -> str:
-        id = str(uuid.uuid4()) + "-doc"
+        id = deterministic_uuid(documentation) + "-doc"
         self.documentation_collection.add(
             documents=documentation,
             embeddings=self.generate_embedding(documentation),
             ids=id,
         )
         return id
```

### Comparing `vanna-0.3.2/src/vanna/exceptions/__init__.py` & `vanna-0.3.3/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/flask/__init__.py` & `vanna-0.3.3/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/flask/assets.py` & `vanna-0.3.3/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/marqo/marqo.py` & `vanna-0.3.3/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/mistral/mistral.py` & `vanna-0.3.3/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/ollama/ollama.py` & `vanna-0.3.3/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/openai/openai_chat.py` & `vanna-0.3.3/src/vanna/openai/openai_chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if client is not None:
             self.client = client
             return
 
         if config is None and client is None:
             self.client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
             return
-      
+
         if "api_key" in config:
             self.client = OpenAI(api_key=config["api_key"])
 
     def system_message(self, message: str) -> any:
         return {"role": "system", "content": message}
 
     def user_message(self, message: str) -> any:
@@ -63,15 +63,39 @@
 
         # Count the number of tokens in the message log
         # Use 4 as an approximation for the number of characters per token
         num_tokens = 0
         for message in prompt:
             num_tokens += len(message["content"]) / 4
 
-        if self.config is not None and "engine" in self.config:
+        if kwargs.get("model", None) is not None:
+            model = kwargs.get("model", None)
+            print(
+                f"Using model {model} for {num_tokens} tokens (approx)"
+            )
+            response = self.client.chat.completions.create(
+                model=model,
+                messages=prompt,
+                max_tokens=self.max_tokens,
+                stop=None,
+                temperature=self.temperature,
+            )
+        elif kwargs.get("engine", None) is not None:
+            engine = kwargs.get("engine", None)
+            print(
+                f"Using model {engine} for {num_tokens} tokens (approx)"
+            )
+            response = self.client.chat.completions.create(
+                engine=engine,
+                messages=prompt,
+                max_tokens=self.max_tokens,
+                stop=None,
+                temperature=self.temperature,
+            )
+        elif self.config is not None and "engine" in self.config:
             print(
                 f"Using engine {self.config['engine']} for {num_tokens} tokens (approx)"
             )
             response = self.client.chat.completions.create(
                 engine=self.config["engine"],
                 messages=prompt,
                 max_tokens=self.max_tokens,
```

### Comparing `vanna-0.3.2/src/vanna/openai/openai_embeddings.py` & `vanna-0.3.3/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/remote.py` & `vanna-0.3.3/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/types/__init__.py` & `vanna-0.3.3/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.3.3/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.2/PKG-INFO` & `vanna-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,30 @@
 Requires-Dist: google-cloud-bigquery ; extra == "all"
 Requires-Dist: snowflake-connector-python ; extra == "all"
 Requires-Dist: duckdb ; extra == "all"
 Requires-Dist: openai ; extra == "all"
 Requires-Dist: mistralai ; extra == "all"
 Requires-Dist: chromadb ; extra == "all"
 Requires-Dist: anthropic ; extra == "all"
+Requires-Dist: zhipuai ; extra == "all"
+Requires-Dist: marqo ; extra == "all"
 Requires-Dist: anthropic ; extra == "anthropic"
 Requires-Dist: google-cloud-bigquery ; extra == "bigquery"
 Requires-Dist: chromadb ; extra == "chromadb"
 Requires-Dist: duckdb ; extra == "duckdb"
 Requires-Dist: google-generativeai ; extra == "gemini"
 Requires-Dist: marqo ; extra == "marqo"
 Requires-Dist: mistralai ; extra == "mistralai"
 Requires-Dist: PyMySQL ; extra == "mysql"
 Requires-Dist: openai ; extra == "openai"
 Requires-Dist: psycopg2-binary ; extra == "postgres"
 Requires-Dist: db-dtypes ; extra == "postgres"
 Requires-Dist: snowflake-connector-python ; extra == "snowflake"
 Requires-Dist: tox ; extra == "test"
+Requires-Dist: zhipuai ; extra == "zhipuai"
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna/issues
 Project-URL: Homepage, https://github.com/vanna-ai/vanna
 Provides-Extra: all
 Provides-Extra: anthropic
 Provides-Extra: bigquery
 Provides-Extra: chromadb
 Provides-Extra: duckdb
@@ -50,14 +53,15 @@
 Provides-Extra: marqo
 Provides-Extra: mistralai
 Provides-Extra: mysql
 Provides-Extra: openai
 Provides-Extra: postgres
 Provides-Extra: snowflake
 Provides-Extra: test
+Provides-Extra: zhipuai
 
 
 
 | GitHub | PyPI | Documentation |
 | ------ | ---- | ------------- |
 | [![GitHub](https://img.shields.io/badge/GitHub-vanna-blue?logo=github)](https://github.com/vanna-ai/vanna) | [![PyPI](https://img.shields.io/pypi/v/vanna?logo=pypi)](https://pypi.org/project/vanna/) | [![Documentation](https://img.shields.io/badge/Documentation-vanna-blue?logo=read-the-docs)](https://vanna.ai/docs/) |
```

