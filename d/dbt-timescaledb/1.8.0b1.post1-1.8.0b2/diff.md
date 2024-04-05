# Comparing `tmp/dbt_timescaledb-1.8.0b1.post1.tar.gz` & `tmp/dbt_timescaledb-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_timescaledb-1.8.0b1.post1.tar", last modified: Tue Apr  2 21:47:36 2024, max compression
+gzip compressed data, was "dbt_timescaledb-1.8.0b2.tar", last modified: Fri Apr  5 20:42:54 2024, max compression
```

## Comparing `dbt_timescaledb-1.8.0b1.post1.tar` & `dbt_timescaledb-1.8.0b2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1068 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/LICENSE
--rw-r--r--   0        0        0     3128 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/README.md
--rw-r--r--   0        0        0       76 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/__init__.py
--rw-r--r--   0        0        0      413 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/__init__.py
--rw-r--r--   0        0        0       25 2024-04-02 21:47:36.705935 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/__version__.py
--rw-r--r--   0        0        0      814 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_adapter.py
--rw-r--r--   0        0        0      515 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_change_collection.py
--rw-r--r--   0        0        0     1684 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_connection_manager.py
--rw-r--r--   0        0        0      224 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_credentials.py
--rw-r--r--   0        0        0      791 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_index_config.py
--rw-r--r--   0        0        0     1965 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_relation.py
--rw-r--r--   0        0        0       52 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/__init__.py
--rw-r--r--   0        0        0       55 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/dbt_project.yml
--rw-r--r--   0        0        0     2585 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/adapters.sql
--rw-r--r--   0        0        0     3143 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
--rw-r--r--   0        0        0     4088 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
--rw-r--r--   0        0        0     2150 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
--rw-r--r--   0        0        0     1784 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/compression.sql
--rw-r--r--   0        0        0     1551 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
--rw-r--r--   0        0        0     1724 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/dimensions.sql
--rw-r--r--   0        0        0     1653 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/hypertable.sql
--rw-r--r--   0        0        0      459 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/integer_now_func.sql
--rw-r--r--   0        0        0      846 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/reorder_policy.sql
--rw-r--r--   0        0        0      706 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/retention_policy.sql
--rw-r--r--   0        0        0      307 2024-04-02 21:47:21.618006 dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/profile_template.yml
--rw-r--r--   0        0        0     2046 2024-04-02 21:47:36.709935 dbt_timescaledb-1.8.0b1.post1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/__init__.py
--rw-r--r--   0        0        0      714 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/conftest.py
--rw-r--r--   0        0        0     2425 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
--rw-r--r--   0        0        0     2573 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
--rw-r--r--   0        0        0     1351 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
--rw-r--r--   0        0        0     2109 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
--rw-r--r--   0        0        0     2407 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py
--rw-r--r--   0        0        0     1821 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable.py
--rw-r--r--   0        0        0     4858 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_compression.py
--rw-r--r--   0        0        0     3071 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_dimension.py
--rw-r--r--   0        0        0     1277 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_index.py
--rw-r--r--   0        0        0     1933 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
--rw-r--r--   0        0        0     1859 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_reorder_policy.py
--rw-r--r--   0        0        0     1429 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     3510 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/test_retention_policy.py
--rw-r--r--   0        0        0     3174 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
--rw-r--r--   0        0        0     1855 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py
--rw-r--r--   0        0        0     2116 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_index_updates.py
--rw-r--r--   0        0        0     2074 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
--rw-r--r--   0        0        0     2324 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py
--rw-r--r--   0        0        0     2254 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py
--rw-r--r--   0        0        0      177 2024-04-02 21:47:21.622007 dbt_timescaledb-1.8.0b1.post1/tests/utils.py
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0b1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/LICENSE
+-rw-r--r--   0        0        0     3128 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/README.md
+-rw-r--r--   0        0        0       76 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-05 20:42:54.022934 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/__version__.py
+-rw-r--r--   0        0        0      814 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_adapter.py
+-rw-r--r--   0        0        0      515 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_change_collection.py
+-rw-r--r--   0        0        0     1684 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_connection_manager.py
+-rw-r--r--   0        0        0      224 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_credentials.py
+-rw-r--r--   0        0        0      791 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_index_config.py
+-rw-r--r--   0        0        0     1965 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_relation.py
+-rw-r--r--   0        0        0       52 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/dbt_project.yml
+-rw-r--r--   0        0        0     2585 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/adapters.sql
+-rw-r--r--   0        0        0     3143 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
+-rw-r--r--   0        0        0     4248 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
+-rw-r--r--   0        0        0     2314 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
+-rw-r--r--   0        0        0     1784 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/compression.sql
+-rw-r--r--   0        0        0     1551 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
+-rw-r--r--   0        0        0     1724 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/dimensions.sql
+-rw-r--r--   0        0        0     1936 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/hypertable.sql
+-rw-r--r--   0        0        0      459 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/integer_now_func.sql
+-rw-r--r--   0        0        0      846 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/reorder_policy.sql
+-rw-r--r--   0        0        0      706 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/retention_policy.sql
+-rw-r--r--   0        0        0      307 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/profile_template.yml
+-rw-r--r--   0        0        0     2040 2024-04-05 20:42:54.026934 dbt_timescaledb-1.8.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/tests/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/tests/conftest.py
+-rw-r--r--   0        0        0     2425 2024-04-05 20:42:38.394983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
+-rw-r--r--   0        0        0     2573 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
+-rw-r--r--   0        0        0     1351 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
+-rw-r--r--   0        0        0     2109 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
+-rw-r--r--   0        0        0     2407 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py
+-rw-r--r--   0        0        0     1821 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable.py
+-rw-r--r--   0        0        0     4858 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_compression.py
+-rw-r--r--   0        0        0     3071 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_dimension.py
+-rw-r--r--   0        0        0     1277 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_index.py
+-rw-r--r--   0        0        0     1933 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     1859 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_reorder_policy.py
+-rw-r--r--   0        0        0     1429 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     3510 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/test_retention_policy.py
+-rw-r--r--   0        0        0     3174 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
+-rw-r--r--   0        0        0     1498 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_chunk_time_interval.py
+-rw-r--r--   0        0        0     1855 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py
+-rw-r--r--   0        0        0     2116 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_index_updates.py
+-rw-r--r--   0        0        0     2074 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     2324 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py
+-rw-r--r--   0        0        0     2254 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py
+-rw-r--r--   0        0        0      177 2024-04-05 20:42:38.398983 dbt_timescaledb-1.8.0b2/tests/utils.py
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0b2/PKG-INFO
```

### Comparing `dbt_timescaledb-1.8.0b1.post1/LICENSE` & `dbt_timescaledb-1.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/README.md` & `dbt_timescaledb-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_adapter.py` & `dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_change_collection.py` & `dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_change_collection.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_connection_manager.py` & `dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_index_config.py` & `dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_index_config.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/adapters/timescaledb/timescaledb_relation.py` & `dbt_timescaledb-1.8.0b2/dbt/adapters/timescaledb/timescaledb_relation.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/adapters.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/hypertable.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/hypertable.sql`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,18 @@
       {{ add_compression_policy(intermediate_relation, config.get("compression")) }}
     {% endif -%}
 
     {%- if config.get("integer_now_func") %}
       {{ set_integer_now_func(intermediate_relation, config.get("integer_now_func"), config.get("integer_now_func_sql")) }}
     {% endif -%}
 
+    {%- if config.get("chunk_time_interval") %}
+      {{ set_chunk_time_interval(intermediate_relation, config.get("chunk_time_interval")) }}
+    {% endif -%}
+
   {%- endcall %}
 
   -- cleanup
   {% if existing_relation is not none %}
      /* Do the equivalent of rename_if_exists. 'existing_relation' could have been dropped
         since the variable was first set. */
     {% set existing_relation = load_cached_relation(existing_relation) %}
```

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql`

 * *Files 5% similar despite different names*

```diff
@@ -19,21 +19,25 @@
             {{ add_compression_policy(target_relation, config.get("compression")) }}
         {% endif -%}
 
         {%- if config.get("integer_now_func") %}
             {{ set_integer_now_func(target_relation, config.get("integer_now_func"), config.get("integer_now_func_sql")) }}
         {% endif -%}
 
+        {%- if config.get("chunk_time_interval") %}
+            {{ set_chunk_time_interval(target_relation, config.get("chunk_time_interval")) }}
+        {% endif -%}
+
         {%- if change_collection %}
             {{ timescaledb__update_indexes_on_virtual_hypertable(target_relation, change_collection.indexes) }}
         {%- endif %}
 
         {{ clear_reorder_policy(target_relation) }}
         {%- if config.get("reorder_policy") %}
-                {{ add_reorder_policy(target_relation, config.get("reorder_policy")) }}
+            {{ add_reorder_policy(target_relation, config.get("reorder_policy")) }}
         {% endif -%}
 
         {{ clear_retention_policy(target_relation) }}
         {%- if config.get("retention_policy") %}
             {{ add_retention_policy(target_relation, config.get("retention_policy")) }}
         {% endif -%}
```

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/compression.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/compression.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/dimensions.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/dimensions.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/hypertable.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/hypertable.sql`

 * *Files 12% similar despite different names*

```diff
@@ -38,7 +38,15 @@
 {% endmacro %}
 
 {% macro get_virtual_hypertable_change_collection(existing_relation, new_config) %}
     {% set _existing_hypertable = describe_hypertable(existing_relation) %}
     {% set _change_collection = existing_relation.get_hypertable_config_change_collection(_existing_hypertable, new_config.model) %}
     {% do return(_change_collection) %}
 {% endmacro %}
+
+{% macro set_chunk_time_interval(relation, chunk_time_interval, dimension_name = none) %}
+  select set_chunk_time_interval('{{ relation }}', {{ chunk_time_interval }}
+    {%- if dimension_name %}
+      , dimension_name => '{{ dimension_name }}'
+    {%- endif %}
+  );
+{% endmacro %}
```

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/reorder_policy.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/reorder_policy.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/dbt/include/timescaledb/macros/relations/retention_policy.sql` & `dbt_timescaledb-1.8.0b2/dbt/include/timescaledb/macros/relations/retention_policy.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/pyproject.toml` & `dbt_timescaledb-1.8.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.11",
 ]
-version = "1.8.0b1.post1"
+version = "1.8.0b2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://dbt-timescaledb.debruyn.dev"
 Repository = "https://github.com/sdebruyn/dbt-timescaledb"
```

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/conftest.py` & `dbt_timescaledb-1.8.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_compression.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_dimension.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_index.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_index.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/hypertable/test_reorder_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/hypertable/test_reorder_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/test_basic.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/test_retention_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/test_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_index_updates.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_index_updates.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py` & `dbt_timescaledb-1.8.0b2/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0b1.post1/PKG-INFO` & `dbt_timescaledb-1.8.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-timescaledb
-Version: 1.8.0b1.post1
+Version: 1.8.0b2
 Summary: The TimescaleDB adapter plugin for dbt
 Keywords: dbt timescaledb
 Author-Email: Sam Debruyn <dbt.sam@debruyn.dev>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

