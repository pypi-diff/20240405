# Comparing `tmp/pixeltable-0.2.1.tar.gz` & `tmp/pixeltable-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.1.tar", max compression
+gzip compressed data, was "pixeltable-0.2.2.tar", max compression
```

## Comparing `pixeltable-0.2.1.tar` & `pixeltable-0.2.2.tar`

### file list

```diff
@@ -1,125 +1,126 @@
--rw-r--r--   0        0        0      746 2024-01-15 22:21:10.025602 pixeltable-0.2.1/LICENSE
--rw-r--r--   0        0        0     4193 2024-04-04 01:37:06.313845 pixeltable-0.2.1/README.md
--rw-r--r--   0        0        0      959 2024-04-04 01:37:07.019405 pixeltable-0.2.1/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-29 02:10:24.349472 pixeltable-0.2.1/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-02 22:13:56.668343 pixeltable-0.2.1/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     8661 2024-04-03 17:26:04.851919 pixeltable-0.2.1/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-29 02:10:24.350840 pixeltable-0.2.1/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-29 02:10:24.351032 pixeltable-0.2.1/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8280 2024-04-03 17:26:04.852785 pixeltable-0.2.1/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-29 02:10:24.351974 pixeltable-0.2.1/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-03 17:26:04.853184 pixeltable-0.2.1/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-03 17:26:04.853564 pixeltable-0.2.1/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-29 02:10:24.352764 pixeltable-0.2.1/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    25499 2024-04-04 00:19:02.760665 pixeltable-0.2.1/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    35680 2024-04-04 01:37:07.020191 pixeltable-0.2.1/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5461 2024-04-03 17:26:04.855707 pixeltable-0.2.1/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-02 22:13:56.672469 pixeltable-0.2.1/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    20548 2024-04-04 01:37:07.040061 pixeltable-0.2.1/pixeltable/client.py
--rw-r--r--   0        0        0    28327 2024-04-04 01:37:07.059370 pixeltable-0.2.1/pixeltable/dataframe.py
--rw-r--r--   0        0        0    16225 2024-04-04 01:37:07.060269 pixeltable-0.2.1/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-01-15 22:21:10.095679 pixeltable-0.2.1/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-01-15 22:21:10.095882 pixeltable-0.2.1/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-02 22:13:56.674688 pixeltable-0.2.1/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5104 2024-03-29 02:10:24.358353 pixeltable-0.2.1/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-29 02:10:24.358711 pixeltable-0.2.1/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-29 02:10:24.359053 pixeltable-0.2.1/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-29 02:10:24.359224 pixeltable-0.2.1/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-01-15 22:21:10.096673 pixeltable-0.2.1/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-02 22:13:56.675099 pixeltable-0.2.1/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     2949 2024-03-29 02:10:24.359831 pixeltable-0.2.1/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-01-15 22:21:10.097303 pixeltable-0.2.1/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-29 02:10:24.360143 pixeltable-0.2.1/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-03 17:26:04.856752 pixeltable-0.2.1/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-29 02:10:24.360769 pixeltable-0.2.1/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-29 02:10:24.361026 pixeltable-0.2.1/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-29 02:10:24.361259 pixeltable-0.2.1/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-29 02:10:24.361503 pixeltable-0.2.1/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     3000 2024-03-29 02:10:24.361847 pixeltable-0.2.1/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-29 02:10:24.362201 pixeltable-0.2.1/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     7535 2024-01-15 22:21:10.098798 pixeltable-0.2.1/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-02 22:13:56.676458 pixeltable-0.2.1/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-01-15 22:21:10.099182 pixeltable-0.2.1/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-03 17:26:04.857185 pixeltable-0.2.1/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-01-15 22:21:10.099445 pixeltable-0.2.1/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-29 02:10:24.364993 pixeltable-0.2.1/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-29 02:10:24.365419 pixeltable-0.2.1/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-29 02:10:24.366065 pixeltable-0.2.1/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-29 02:10:24.366678 pixeltable-0.2.1/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-29 02:10:24.367023 pixeltable-0.2.1/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-29 02:10:24.368455 pixeltable-0.2.1/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-29 02:10:24.368997 pixeltable-0.2.1/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     1885 2024-03-29 02:10:24.369311 pixeltable-0.2.1/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-01-15 22:21:10.100425 pixeltable-0.2.1/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-29 02:10:24.374640 pixeltable-0.2.1/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    16992 2024-04-02 22:13:56.677709 pixeltable-0.2.1/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-29 02:10:24.376127 pixeltable-0.2.1/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-29 02:10:24.376650 pixeltable-0.2.1/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-03 17:26:04.857483 pixeltable-0.2.1/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      457 2024-04-03 17:26:04.858004 pixeltable-0.2.1/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-03 17:26:04.858396 pixeltable-0.2.1/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-03 17:26:04.858718 pixeltable-0.2.1/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-04 01:37:07.078107 pixeltable-0.2.1/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3392 2024-04-03 17:26:04.859226 pixeltable-0.2.1/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-04 01:37:07.098368 pixeltable-0.2.1/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-04 01:37:07.099391 pixeltable-0.2.1/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1220 2024-04-04 01:37:07.119033 pixeltable-0.2.1/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-03 17:26:04.859586 pixeltable-0.2.1/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7107 2024-04-03 17:26:04.859944 pixeltable-0.2.1/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6457 2024-04-04 01:37:07.138326 pixeltable-0.2.1/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3419 2024-04-04 01:37:07.139301 pixeltable-0.2.1/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-02 22:13:56.685253 pixeltable-0.2.1/pixeltable/functions/eval.py
--rw-r--r--   0        0        0     1596 2024-04-04 02:03:58.915636 pixeltable-0.2.1/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     4804 2024-04-03 17:26:04.860757 pixeltable-0.2.1/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-03 17:26:04.861025 pixeltable-0.2.1/pixeltable/functions/image.py
--rw-r--r--   0        0        0     2863 2024-04-04 01:37:07.159142 pixeltable-0.2.1/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-03 17:26:04.861910 pixeltable-0.2.1/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-02 22:13:56.687559 pixeltable-0.2.1/pixeltable/functions/string.py
--rw-r--r--   0        0        0      650 2024-04-04 01:37:07.179442 pixeltable-0.2.1/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1596 2024-04-02 22:13:56.688834 pixeltable-0.2.1/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-02 22:13:56.689676 pixeltable-0.2.1/pixeltable/functions/video.py
--rw-r--r--   0        0        0       70 2024-01-15 22:21:10.104617 pixeltable-0.2.1/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-29 02:10:24.389524 pixeltable-0.2.1/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13088 2024-03-29 02:10:24.390315 pixeltable-0.2.1/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-29 02:10:24.390700 pixeltable-0.2.1/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-03 17:26:04.862244 pixeltable-0.2.1/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-29 02:10:24.391424 pixeltable-0.2.1/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     7761 2024-04-02 22:13:56.690669 pixeltable-0.2.1/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    34710 2024-04-03 17:26:04.862980 pixeltable-0.2.1/pixeltable/plan.py
--rw-r--r--   0        0        0    19230 2024-04-02 22:13:56.691931 pixeltable-0.2.1/pixeltable/store.py
--rw-r--r--   0        0        0     6581 2024-04-03 17:26:04.864000 pixeltable-0.2.1/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     3186 2024-04-03 17:26:04.864518 pixeltable-0.2.1/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-01-15 22:21:10.632434 pixeltable-0.2.1/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-03 17:26:04.864987 pixeltable-0.2.1/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    17704 2024-04-03 17:26:04.865583 pixeltable-0.2.1/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    17686 2024-04-03 17:26:04.866459 pixeltable-0.2.1/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-03 17:26:04.866972 pixeltable-0.2.1/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5657 2024-04-03 17:26:04.867386 pixeltable-0.2.1/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32695 2024-04-03 17:26:04.868024 pixeltable-0.2.1/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12817 2024-04-04 01:37:07.199475 pixeltable-0.2.1/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0    14477 2024-04-03 17:26:04.869252 pixeltable-0.2.1/pixeltable/tests/test_functions.py
--rw-r--r--   0        0        0     1535 2024-04-03 17:26:04.869854 pixeltable-0.2.1/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-03 17:26:04.870509 pixeltable-0.2.1/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0     9297 2024-04-03 17:26:04.871225 pixeltable-0.2.1/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    48202 2024-04-04 01:37:07.200583 pixeltable-0.2.1/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-03 17:26:04.872718 pixeltable-0.2.1/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0      970 2024-04-03 17:26:04.873099 pixeltable-0.2.1/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7676 2024-04-03 17:26:04.873582 pixeltable-0.2.1/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    21859 2024-04-03 17:26:04.874060 pixeltable-0.2.1/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0     9914 2024-04-03 17:26:04.874467 pixeltable-0.2.1/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5148 2024-04-03 17:26:04.875028 pixeltable-0.2.1/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0    31781 2024-04-03 17:26:04.875632 pixeltable-0.2.1/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-01-15 22:21:10.635863 pixeltable-0.2.1/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0      720 2024-01-15 22:21:10.635981 pixeltable-0.2.1/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-29 02:10:24.462374 pixeltable-0.2.1/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-29 02:10:24.462842 pixeltable-0.2.1/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-29 02:10:24.463396 pixeltable-0.2.1/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-01-15 22:21:10.636442 pixeltable-0.2.1/pixeltable/utils/help.py
--rw-r--r--   0        0        0     3116 2024-03-29 02:10:24.463930 pixeltable-0.2.1/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     5775 2024-01-15 22:21:10.636686 pixeltable-0.2.1/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     6515 2024-04-03 17:26:04.876346 pixeltable-0.2.1/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-01-15 22:21:10.636985 pixeltable-0.2.1/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-01-15 22:21:10.637081 pixeltable-0.2.1/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-03 17:26:04.876793 pixeltable-0.2.1/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3280 2024-04-04 05:03:44.713584 pixeltable-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 pixeltable-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-01-15 22:21:10.025602 pixeltable-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4193 2024-04-05 01:34:32.679704 pixeltable-0.2.2/README.md
+-rw-r--r--   0        0        0      959 2024-04-04 15:03:13.491688 pixeltable-0.2.2/pixeltable/__init__.py
+-rw-r--r--   0        0        0      453 2024-03-29 02:10:24.349472 pixeltable-0.2.2/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-02 22:13:56.668343 pixeltable-0.2.2/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     8661 2024-04-04 15:03:13.492105 pixeltable-0.2.2/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-29 02:10:24.350840 pixeltable-0.2.2/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-29 02:10:24.351032 pixeltable-0.2.2/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8280 2024-04-04 15:03:13.492541 pixeltable-0.2.2/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-29 02:10:24.351974 pixeltable-0.2.2/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-04 15:03:13.492968 pixeltable-0.2.2/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-04 15:03:13.493364 pixeltable-0.2.2/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-29 02:10:24.352764 pixeltable-0.2.2/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    25499 2024-04-04 15:03:13.493856 pixeltable-0.2.2/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    35680 2024-04-04 15:03:13.494406 pixeltable-0.2.2/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5461 2024-04-04 15:03:13.495287 pixeltable-0.2.2/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-02 22:13:56.672469 pixeltable-0.2.2/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    20548 2024-04-04 15:03:13.495950 pixeltable-0.2.2/pixeltable/client.py
+-rw-r--r--   0        0        0    28339 2024-04-05 01:34:32.701874 pixeltable-0.2.2/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    16398 2024-04-05 01:34:32.702438 pixeltable-0.2.2/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-01-15 22:21:10.095679 pixeltable-0.2.2/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      412 2024-01-15 22:21:10.095882 pixeltable-0.2.2/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-02 22:13:56.674688 pixeltable-0.2.2/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5104 2024-03-29 02:10:24.358353 pixeltable-0.2.2/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-29 02:10:24.358711 pixeltable-0.2.2/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3505 2024-03-29 02:10:24.359053 pixeltable-0.2.2/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-29 02:10:24.359224 pixeltable-0.2.2/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-01-15 22:21:10.096673 pixeltable-0.2.2/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10810 2024-04-02 22:13:56.675099 pixeltable-0.2.2/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     2949 2024-03-29 02:10:24.359831 pixeltable-0.2.2/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-01-15 22:21:10.097303 pixeltable-0.2.2/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10318 2024-03-29 02:10:24.360143 pixeltable-0.2.2/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      935 2024-04-04 15:03:13.497550 pixeltable-0.2.2/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-29 02:10:24.360769 pixeltable-0.2.2/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-29 02:10:24.361026 pixeltable-0.2.2/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-29 02:10:24.361259 pixeltable-0.2.2/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     4794 2024-03-29 02:10:24.361503 pixeltable-0.2.2/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     3000 2024-03-29 02:10:24.361847 pixeltable-0.2.2/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-29 02:10:24.362201 pixeltable-0.2.2/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     7535 2024-01-15 22:21:10.098798 pixeltable-0.2.2/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    23748 2024-04-02 22:13:56.676458 pixeltable-0.2.2/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-01-15 22:21:10.099182 pixeltable-0.2.2/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    16961 2024-04-04 15:03:13.526393 pixeltable-0.2.2/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-01-15 22:21:10.099445 pixeltable-0.2.2/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     4663 2024-03-29 02:10:24.364993 pixeltable-0.2.2/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     1906 2024-03-29 02:10:24.365419 pixeltable-0.2.2/pixeltable/exprs/image_similarity_predicate.py
+-rw-r--r--   0        0        0     4312 2024-03-29 02:10:24.366065 pixeltable-0.2.2/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3695 2024-03-29 02:10:24.366678 pixeltable-0.2.2/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-29 02:10:24.367023 pixeltable-0.2.2/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-29 02:10:24.368455 pixeltable-0.2.2/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-29 02:10:24.368997 pixeltable-0.2.2/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     1885 2024-03-29 02:10:24.369311 pixeltable-0.2.2/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-01-15 22:21:10.100425 pixeltable-0.2.2/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-29 02:10:24.374640 pixeltable-0.2.2/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    16992 2024-04-02 22:13:56.677709 pixeltable-0.2.2/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-29 02:10:24.376127 pixeltable-0.2.2/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     1793 2024-03-29 02:10:24.376650 pixeltable-0.2.2/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-04 15:03:13.527090 pixeltable-0.2.2/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      457 2024-04-04 15:03:13.584303 pixeltable-0.2.2/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-04 15:03:13.601913 pixeltable-0.2.2/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     2350 2024-04-04 15:03:13.602549 pixeltable-0.2.2/pixeltable/func/batched_function.py
+-rw-r--r--   0        0        0     2357 2024-04-04 15:03:13.602985 pixeltable-0.2.2/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     3392 2024-04-04 15:03:13.603326 pixeltable-0.2.2/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     4023 2024-04-04 15:03:13.603679 pixeltable-0.2.2/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 15:03:13.604235 pixeltable-0.2.2/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1220 2024-04-04 15:03:13.604579 pixeltable-0.2.2/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-04 15:03:13.604966 pixeltable-0.2.2/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     7107 2024-04-04 15:03:13.605389 pixeltable-0.2.2/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6457 2024-04-04 15:03:13.605802 pixeltable-0.2.2/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3419 2024-04-04 15:03:13.606222 pixeltable-0.2.2/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8453 2024-04-02 22:13:56.685253 pixeltable-0.2.2/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0     1596 2024-04-04 15:03:13.606866 pixeltable-0.2.2/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     4804 2024-04-04 15:03:13.607357 pixeltable-0.2.2/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-04 15:03:13.607789 pixeltable-0.2.2/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     2863 2024-04-04 20:32:17.201830 pixeltable-0.2.2/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     6217 2024-04-04 15:03:13.608251 pixeltable-0.2.2/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-02 22:13:56.687559 pixeltable-0.2.2/pixeltable/functions/string.py
+-rw-r--r--   0        0        0      650 2024-04-04 15:03:13.608761 pixeltable-0.2.2/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1596 2024-04-02 22:13:56.688834 pixeltable-0.2.2/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-02 22:13:56.689676 pixeltable-0.2.2/pixeltable/functions/video.py
+-rw-r--r--   0        0        0       70 2024-01-15 22:21:10.104617 pixeltable-0.2.2/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-29 02:10:24.389524 pixeltable-0.2.2/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    13088 2024-03-29 02:10:24.390315 pixeltable-0.2.2/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3444 2024-03-29 02:10:24.390700 pixeltable-0.2.2/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2083 2024-04-04 15:03:13.609220 pixeltable-0.2.2/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-29 02:10:24.391424 pixeltable-0.2.2/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0     7761 2024-04-02 22:13:56.690669 pixeltable-0.2.2/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    34710 2024-04-04 15:03:13.609842 pixeltable-0.2.2/pixeltable/plan.py
+-rw-r--r--   0        0        0    19230 2024-04-02 22:13:56.691931 pixeltable-0.2.2/pixeltable/store.py
+-rw-r--r--   0        0        0     6677 2024-04-04 21:05:30.616015 pixeltable-0.2.2/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0     3186 2024-04-04 15:03:13.610924 pixeltable-0.2.2/pixeltable/tests/test_audio.py
+-rw-r--r--   0        0        0     1189 2024-01-15 22:21:10.632434 pixeltable-0.2.2/pixeltable/tests/test_catalog.py
+-rw-r--r--   0        0        0      531 2024-04-04 15:03:13.611478 pixeltable-0.2.2/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0    17732 2024-04-04 21:05:30.639792 pixeltable-0.2.2/pixeltable/tests/test_component_view.py
+-rw-r--r--   0        0        0    17686 2024-04-04 15:03:13.612660 pixeltable-0.2.2/pixeltable/tests/test_dataframe.py
+-rw-r--r--   0        0        0     3611 2024-04-04 15:03:13.613238 pixeltable-0.2.2/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0     5657 2024-04-04 15:03:13.613735 pixeltable-0.2.2/pixeltable/tests/test_document.py
+-rw-r--r--   0        0        0    32695 2024-04-04 15:03:13.614257 pixeltable-0.2.2/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0    12817 2024-04-04 15:03:13.614623 pixeltable-0.2.2/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0    14394 2024-04-05 01:34:32.702868 pixeltable-0.2.2/pixeltable/tests/test_functions.py
+-rw-r--r--   0        0        0     1535 2024-04-04 15:03:13.615516 pixeltable-0.2.2/pixeltable/tests/test_migration.py
+-rw-r--r--   0        0        0     2649 2024-04-04 15:03:13.615912 pixeltable-0.2.2/pixeltable/tests/test_nos.py
+-rw-r--r--   0        0        0     9297 2024-04-04 15:03:13.616356 pixeltable-0.2.2/pixeltable/tests/test_snapshot.py
+-rw-r--r--   0        0        0    48202 2024-04-04 15:03:13.617029 pixeltable-0.2.2/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     1308 2024-04-04 15:03:13.617428 pixeltable-0.2.2/pixeltable/tests/test_transactional_directory.py
+-rw-r--r--   0        0        0      970 2024-04-04 15:03:13.617805 pixeltable-0.2.2/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     7676 2024-04-04 15:03:13.618199 pixeltable-0.2.2/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0    21859 2024-04-04 15:03:13.618642 pixeltable-0.2.2/pixeltable/tests/test_view.py
+-rw-r--r--   0        0        0    10213 2024-04-04 21:05:30.640283 pixeltable-0.2.2/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     5148 2024-04-04 15:03:13.619429 pixeltable-0.2.2/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0     2899 2024-04-04 21:05:30.640709 pixeltable-0.2.2/pixeltable/tool/create_test_video.py
+-rw-r--r--   0        0        0    31781 2024-04-04 20:32:17.202919 pixeltable-0.2.2/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-01-15 22:21:10.635863 pixeltable-0.2.2/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0      720 2024-01-15 22:21:10.635981 pixeltable-0.2.2/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-29 02:10:24.462374 pixeltable-0.2.2/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     1094 2024-03-29 02:10:24.462842 pixeltable-0.2.2/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-29 02:10:24.463396 pixeltable-0.2.2/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-01-15 22:21:10.636442 pixeltable-0.2.2/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     3116 2024-03-29 02:10:24.463930 pixeltable-0.2.2/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     5775 2024-01-15 22:21:10.636686 pixeltable-0.2.2/pixeltable/utils/parquet.py
+-rw-r--r--   0        0        0     6515 2024-04-04 15:03:13.619950 pixeltable-0.2.2/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-01-15 22:21:10.636985 pixeltable-0.2.2/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-01-15 22:21:10.637081 pixeltable-0.2.2/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-04 15:03:13.620278 pixeltable-0.2.2/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     3284 2024-04-05 01:34:32.726498 pixeltable-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 pixeltable-0.2.2/PKG-INFO
```

### Comparing `pixeltable-0.2.1/LICENSE` & `pixeltable-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/README.md` & `pixeltable-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 exploration, modeling, and app development without having to deal with the customary
 data plumbing.
 
 **Pixeltable redefines data infrastructure and workflow orchestration for AI development.**
 It brings together data storage, versioning, and indexing with orchestration and model
 versioning under a declarative table interface, with transformations, model inference,
 and custom logic represented as computed columns.
-<!--
+
 ## Quick Start
 
 If you just want to play around with Pixeltable to see what it's capable of, the easiest way is to run
 the Pixeltable Basics tutorial in colab:
 
-<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/docs/tutorials/pixeltable-basics.ipynb">
+<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
--->
+
 ## Installation
 
 Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
 
 ```
 pip install pixeltable
 ```
```

### Comparing `pixeltable-0.2.1/pixeltable/__init__.py` & `pixeltable-0.2.2/pixeltable/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/catalog.py` & `pixeltable-0.2.2/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/column.py` & `pixeltable-0.2.2/pixeltable/catalog/column.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/dir.py` & `pixeltable-0.2.2/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/globals.py` & `pixeltable-0.2.2/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.2/pixeltable/catalog/insertable_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/named_function.py` & `pixeltable-0.2.2/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/path.py` & `pixeltable-0.2.2/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.2/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.2/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/table.py` & `pixeltable-0.2.2/pixeltable/catalog/table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/table_version.py` & `pixeltable-0.2.2/pixeltable/catalog/table_version.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.2/pixeltable/catalog/table_version_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/catalog/view.py` & `pixeltable-0.2.2/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/client.py` & `pixeltable-0.2.2/pixeltable/client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/dataframe.py` & `pixeltable-0.2.2/pixeltable/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     Create <img> tag for Image object.
     """
     assert isinstance(img, Image.Image), f'Wrong type: {type(img)}'
     with io.BytesIO() as buffer:
         img.save(buffer, 'jpeg')
         img_base64 = base64.b64encode(buffer.getvalue()).decode()
-        return f'<div style=\'width:200px;\'><img src="data:image/jpeg;base64,{img_base64}"></div>'
+        return f'<div style="width:200px;"><img src="data:image/jpeg;base64,{img_base64}" width="200" /></div>'
 
 def _create_source_tag(file_path: str) -> str:
     abs_path = Path(file_path)
     assert abs_path.is_absolute()
     src_url = f'{Env.get().http_address}/{abs_path}'
     mime = mimetypes.guess_type(src_url)[0]
     # if mime is None, the attribute string would not be valid html.
```

### Comparing `pixeltable-0.2.1/pixeltable/env.py` & `pixeltable-0.2.2/pixeltable/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def config(self):
         return self._config
 
     @property
     def db_url(self) -> str:
         assert self._db_url is not None
         return self._db_url
-    
+
     @property
     def http_address(self) -> str:
         assert self._http_address is not None
         return self._http_address
 
     def print_log_config(self) -> None:
         print(f'logging to {self._logfilename}')
@@ -138,26 +138,25 @@
             return True
         else:
             return False
 
     def set_up(self, echo: bool = False, reinit_db: bool = False) -> None:
         if self._initialized:
             return
-        
+
         self._initialized = True
         home = Path(os.environ.get('PIXELTABLE_HOME', str(Path.home() / '.pixeltable')))
         assert self._home is None or self._home == home
         self._home = home
         self._config_file = Path(os.environ.get('PIXELTABLE_CONFIG', str(self._home / 'config.yaml')))
         self._media_dir = self._home / 'media'
         self._file_cache_dir = self._home / 'file_cache'
         self._dataset_cache_dir = self._home / 'dataset_cache'
         self._log_dir = self._home / 'logs'
         self._tmp_dir = self._home / 'tmp'
-        self._pgdata_dir = Path(os.environ.get('PIXELTABLE_PGDATA', str(self._home / 'pgdata')))
 
         # Read in the config
         if os.path.isfile(self._config_file):
             with open(self._config_file, 'r') as stream:
                 try:
                     self._config = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
@@ -200,16 +199,17 @@
         sql_logger.propagate = False
 
         # empty tmp dir
         for path in glob.glob(f'{self._tmp_dir}/*'):
             os.remove(path)
 
         self._db_name = os.environ.get('PIXELTABLE_DB', 'pixeltable')
+        self._pgdata_dir = Path(os.environ.get('PIXELTABLE_PGDATA', str(self._home / 'pgdata')))
 
-        # cleanup_mode=None will leave db on for debugging purposes
+        # in pgserver.get_server(): cleanup_mode=None will leave db on for debugging purposes
         self._db_server = pgserver.get_server(self._pgdata_dir, cleanup_mode=None)
         self._db_url = self._db_server.get_uri(database=self._db_name)
 
         if reinit_db:
             if database_exists(self.db_url):
                 drop_database(self.db_url)
 
@@ -253,24 +253,25 @@
             return
         except ImportError:
             pass
         from pixeltable.functions.util import create_nos_modules
         _ = create_nos_modules()
 
     def _create_openai_client(self) -> None:
+        if not self.is_installed_package('openai'):
+            raise excs.Error('OpenAI client not initialized (cannot find package `openai`: `pip install openai`?)')
+        import openai
         if 'openai' in self._config and 'api_key' in self._config['openai']:
             api_key = self._config['openai']['api_key']
         else:
             api_key = os.environ.get('OPENAI_API_KEY')
         if api_key is None or api_key == '':
-            self._logger.info("OpenAI client not initialized (no API key configured).")
-            return
-        import openai
-        self._logger.info('Initializing OpenAI client.')
+            raise excs.Error('OpenAI client not initialized (no API key configured).')
         self._openai_client = openai.OpenAI(api_key=api_key)
+        self._logger.info('Initialized OpenAI client.')
 
     def _create_together_client(self) -> None:
         if 'together' in self._config and 'api_key' in self._config['together']:
             api_key = self._config['together']['api_key']
         else:
             api_key = os.environ.get('TOGETHER_API_KEY')
         if api_key is None or api_key == '':
@@ -281,23 +282,23 @@
         together.api_key = api_key
         self._has_together_client = True
 
     def _start_web_server(self) -> None:
         """
         The http server root is the file system root.
         eg: /home/media/foo.mp4 is located at http://127.0.0.1:{port}/home/media/foo.mp4
-        This arrangement enables serving media hosted within _home, 
+        This arrangement enables serving media hosted within _home,
         as well as external media inserted into pixeltable or produced by pixeltable.
         The port is chosen dynamically to prevent conflicts.
-        """        
+        """
         # Port 0 means OS picks one for us.
         address = ("127.0.0.1", 0)
         class FixedRootHandler(http.server.SimpleHTTPRequestHandler):
             def __init__(self, *args, **kwargs):
-                super().__init__(*args, directory='/', **kwargs)        
+                super().__init__(*args, directory='/', **kwargs)
         self._httpd = socketserver.TCPServer(address, FixedRootHandler)
         port = self._httpd.server_address[1]
         self._http_address = f'http://127.0.0.1:{port}'
 
         def run_server():
             logging.log(logging.INFO, f'running web server at {self._http_address}')
             self._httpd.serve_forever()
@@ -326,16 +327,14 @@
         check('pyarrow')
         check('spacy')  # TODO: deal with en-core-web-sm
         if self.is_installed_package('spacy'):
             import spacy
             self._spacy_nlp = spacy.load('en_core_web_sm')
         check('tiktoken')
         check('openai')
-        if self.is_installed_package('openai'):
-            self._create_openai_client()
         check('together')
         if self.is_installed_package('together'):
             self._create_together_client()
         check('fireworks')
         check('nos')
         if self.is_installed_package('nos'):
             self._create_nos_client()
@@ -397,15 +396,18 @@
         return self._sa_engine
 
     @property
     def nos_client(self) -> Any:
         return self._nos_client
 
     @property
-    def openai_client(self) -> Optional['openai.OpenAI']:
+    def openai_client(self) -> 'openai.OpenAI':
+        if self._openai_client is None:
+            self._create_openai_client()
+        assert self._openai_client is not None
         return self._openai_client
 
     @property
     def has_together_client(self) -> bool:
         return self._has_together_client
 
     @property
```

### Comparing `pixeltable-0.2.1/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.2/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.2/pixeltable/exec/cache_prefetch_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.2/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.2/pixeltable/exec/data_row_batch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/exec_context.py` & `pixeltable-0.2.2/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/exec_node.py` & `pixeltable-0.2.2/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.2/pixeltable/exec/expr_eval_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.2/pixeltable/exec/in_memory_data_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.2/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.2/pixeltable/exec/sql_scan_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/__init__.py` & `pixeltable-0.2.2/pixeltable/exprs/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.2/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.2/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.2/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.2/pixeltable/exprs/column_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/comparison.py` & `pixeltable-0.2.2/pixeltable/exprs/comparison.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.2/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/data_row.py` & `pixeltable-0.2.2/pixeltable/exprs/data_row.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/expr.py` & `pixeltable-0.2.2/pixeltable/exprs/expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.2/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/function_call.py` & `pixeltable-0.2.2/pixeltable/exprs/function_call.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/globals.py` & `pixeltable-0.2.2/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.2/pixeltable/exprs/image_member_access.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/image_similarity_predicate.py` & `pixeltable-0.2.2/pixeltable/exprs/image_similarity_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.2/pixeltable/exprs/inline_array.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.2/pixeltable/exprs/inline_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/is_null.py` & `pixeltable-0.2.2/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.2/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/json_path.py` & `pixeltable-0.2.2/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/literal.py` & `pixeltable-0.2.2/pixeltable/exprs/literal.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.2/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/predicate.py` & `pixeltable-0.2.2/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.2/pixeltable/exprs/row_builder.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.2/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.2/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/exprs/variable.py` & `pixeltable-0.2.2/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.2/pixeltable/func/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/batched_function.py` & `pixeltable-0.2.2/pixeltable/func/batched_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/callable_function.py` & `pixeltable-0.2.2/pixeltable/func/callable_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.2/pixeltable/func/expr_template_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/function.py` & `pixeltable-0.2.2/pixeltable/func/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/function_registry.py` & `pixeltable-0.2.2/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/globals.py` & `pixeltable-0.2.2/pixeltable/func/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/nos_function.py` & `pixeltable-0.2.2/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/signature.py` & `pixeltable-0.2.2/pixeltable/func/signature.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/func/udf.py` & `pixeltable-0.2.2/pixeltable/func/udf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/__init__.py` & `pixeltable-0.2.2/pixeltable/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/eval.py` & `pixeltable-0.2.2/pixeltable/functions/eval.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/fireworks.py` & `pixeltable-0.2.2/pixeltable/functions/fireworks.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/huggingface.py` & `pixeltable-0.2.2/pixeltable/functions/huggingface.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/openai.py` & `pixeltable-0.2.2/pixeltable/functions/openai.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/pil/image.py` & `pixeltable-0.2.2/pixeltable/functions/pil/image.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/string.py` & `pixeltable-0.2.2/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/together.py` & `pixeltable-0.2.2/pixeltable/functions/together.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/util.py` & `pixeltable-0.2.2/pixeltable/functions/util.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/functions/video.py` & `pixeltable-0.2.2/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/iterators/base.py` & `pixeltable-0.2.2/pixeltable/iterators/base.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/iterators/document.py` & `pixeltable-0.2.2/pixeltable/iterators/document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/iterators/video.py` & `pixeltable-0.2.2/pixeltable/iterators/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/metadata/__init__.py` & `pixeltable-0.2.2/pixeltable/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.2/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/metadata/schema.py` & `pixeltable-0.2.2/pixeltable/metadata/schema.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/plan.py` & `pixeltable-0.2.2/pixeltable/plan.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/store.py` & `pixeltable-0.2.2/pixeltable/store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/conftest.py` & `pixeltable-0.2.2/pixeltable/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 
 @pytest.fixture(scope='session')
 def init_env(tmp_path_factory) -> None:
     from pixeltable.env import Env
     # set the relevant env vars for Client() to connect to the test db
 
-    shared_home = pathlib.Path(os.environ.get('PIXELTABLE_HOME', '~/.pixeltable')).expanduser()
+    shared_home = pathlib.Path(os.environ.get('PIXELTABLE_HOME', str(pathlib.Path.home() / '.pixeltable')))
     home_dir = str(tmp_path_factory.mktemp('base') / '.pixeltable')
     os.environ['PIXELTABLE_HOME'] = home_dir
     os.environ['PIXELTABLE_CONFIG'] = str(shared_home / 'config.yaml')
     test_db = 'test'
     os.environ['PIXELTABLE_DB'] = test_db
     os.environ['PIXELTABLE_PGDATA'] = str(shared_home / 'pgdata')
 
+    # ensure this home dir exits
+    shared_home.mkdir(parents=True, exist_ok=True)
     # this also runs create_all()
     Env.get().set_up(echo=True)
     yield
     # leave db in place for debugging purposes
 
 @pytest.fixture(scope='function')
 def test_client(init_env) -> pxt.Client:
```

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_audio.py` & `pixeltable-0.2.2/pixeltable/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_catalog.py` & `pixeltable-0.2.2/pixeltable/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_client.py` & `pixeltable-0.2.2/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_component_view.py` & `pixeltable-0.2.2/pixeltable/tests/test_component_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import pandas as pd
 import pytest
 
 import pixeltable as pxt
 from pixeltable import exceptions as excs
 from pixeltable.iterators import ComponentIterator
 from pixeltable.iterators.video import FrameIterator
-from pixeltable.tests.utils import assert_resultset_eq, get_video_files
+from pixeltable.tests.utils import assert_resultset_eq, get_test_video_files
 from pixeltable.type_system import IntType, VideoType, JsonType
 
-
 class ConstantImgIterator(ComponentIterator):
     """Component iterator that generates a fixed number of all-black 1280x720 images."""
     def __init__(self, video: str, num_frames: int = 10):
         self.img = PIL.Image.new('RGB', (1280, 720))
         self.next_frame_idx = 0
         self.num_frames = num_frames
         self.pos_msec = 0.0
@@ -55,22 +54,21 @@
         pass
 
     def set_pos(self, pos: int) -> None:
         if pos == self.next_frame_idx:
             return
         self.next_frame_idx = pos
 
-
 class TestComponentView:
     def test_basic(self, test_client: pxt.Client) -> None:
         cl = test_client
         # create video table
         schema = {'video': VideoType(), 'angle': IntType(), 'other_angle': IntType()}
         video_t = cl.create_table('video_tbl', schema)
-        video_filepaths = get_video_files()
+        video_filepaths = get_test_video_files()
 
         # cannot add 'pos' column
         with pytest.raises(excs.Error) as excinfo:
             video_t.add_column(pos=IntType())
         assert 'reserved' in str(excinfo.value)
 
         # parameter missing
@@ -120,15 +118,15 @@
         assert len(result) > 0
         assert np.all(result['frame_idx'] == pd.Series(range(len(result))))
 
     def test_add_column(self, test_client: pxt.Client) -> None:
         cl = test_client
         # create video table
         video_t = cl.create_table('video_tbl', {'video': VideoType()})
-        video_filepaths = get_video_files()
+        video_filepaths = get_test_video_files()
         # create frame view
         args = {'video': video_t.video, 'fps': 1}
         view_t = cl.create_view('test_view', video_t, iterator_class=FrameIterator, iterator_args=args)
 
         rows = [{'video': p} for p in video_filepaths]
         video_t.insert(rows)
         # adding a non-computed column backfills it with nulls
@@ -149,15 +147,15 @@
         video_t = cl.create_table('video_tbl', {'video': VideoType()})
         # create frame view with manually updated column
         args = {'video': video_t.video, 'fps': 1}
         view_t = cl.create_view(
             'test_view', video_t, schema={'annotation': JsonType(nullable=True)},
             iterator_class=FrameIterator, iterator_args=args)
 
-        video_filepaths = get_video_files()
+        video_filepaths = get_test_video_files()
         rows = [{'video': p} for p in video_filepaths]
         status = video_t.insert(rows)
         assert status.num_excs == 0
         import urllib
         video_url = urllib.parse.urljoin('file:', urllib.request.pathname2url(video_filepaths[0]))
         status = view_t.update({'annotation': {'a': 1}}, where=view_t.video == video_url)
         c1 = view_t.where(view_t.annotation != None).count()
@@ -202,15 +200,15 @@
     def run_snapshot_test(self, cl: pxt.Client, has_column: bool, has_filter: bool, reload_md: bool) -> None:
         base_path = 'video_tbl'
         view_path = 'test_view'
         snap_path = 'test_snap'
 
         # create video table
         video_t = cl.create_table(base_path, {'video': VideoType(), 'margin': IntType()})
-        video_filepaths = get_video_files()
+        video_filepaths = get_test_video_files()
         rows = [{'video': path, 'margin': i * 10} for i, path in enumerate(video_filepaths)]
         status = video_t.insert(rows)
         assert status.num_rows == len(rows)
         assert status.num_excs == 0
 
         # create frame view with a computed column
         args = {'video': video_t.video}
@@ -273,15 +271,15 @@
 
     def test_chained_views(self, test_client: pxt.Client) -> None:
         """Component view followed by a standard view"""
         cl = test_client
         # create video table
         schema = {'video': VideoType(), 'int1': IntType(), 'int2': IntType()}
         video_t = cl.create_table('video_tbl', schema)
-        video_filepaths = get_video_files()
+        video_filepaths = get_test_video_files()
 
         # create first view
         args = {'video': video_t.video}
         v1 = cl.create_view('test_view', video_t, iterator_class=ConstantImgIterator, iterator_args=args)
         # computed column that references stored base column
         v1.add_column(int3=v1.int1 + 1)
         # stored computed column that references an unstored and a stored computed view column
```

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_dataframe.py` & `pixeltable-0.2.2/pixeltable/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_dirs.py` & `pixeltable-0.2.2/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_document.py` & `pixeltable-0.2.2/pixeltable/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_exprs.py` & `pixeltable-0.2.2/pixeltable/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_function.py` & `pixeltable-0.2.2/pixeltable/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_functions.py` & `pixeltable-0.2.2/pixeltable/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, Any
 
 import pytest
 
 import pixeltable as pxt
 from pixeltable import catalog
 from pixeltable.env import Env
+import pixeltable.exceptions as excs
 from pixeltable.functions.pil.image import blend
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import get_video_files, skip_test_if_not_installed, get_sentences, get_image_files
 from pixeltable.type_system import VideoType, StringType, JsonType, ImageType, BoolType, FloatType, ArrayType
 
 
 class TestFunctions:
@@ -63,16 +64,14 @@
         assert status.num_excs == 0
         row = t.head()[0]
         assert row == {'input': 'MNO', 's1': 'ABC MNO', 's2': 'DEF MNO', 's3': 'GHI MNO JKL MNO'}
 
     def test_openai(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('openai')
         TestFunctions.skip_test_if_no_openai_client()
-        if Env.get().openai_client is None:
-            pytest.skip(f'OpenAI client does not exist (missing API key?).')
         cl = test_client
         t = cl.create_table('test_tbl', {'input': StringType()})
         from pixeltable.functions.openai import chat_completions, embeddings, moderations
         msgs = [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": t.input}
         ]
@@ -106,16 +105,18 @@
         t.add_column(response_content=t.response.choices[0].message.content)
         t.insert(prompt="What's in this image?", img=_sample_image_url)
         result = t.collect()['response_content'][0]
         assert len(result) > 0
 
     @staticmethod
     def skip_test_if_no_openai_client() -> None:
-        if Env.get().openai_client is None:
-            pytest.skip(f'OpenAI client does not exist (missing API key?)')
+        try:
+            _ = Env.get().openai_client
+        except excs.Error as exc:
+            pytest.skip(str(exc))
 
     def test_together(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('together')
         if not Env.get().has_together_client:
             pytest.skip(f'Together client does not exist (missing API key?)')
         cl = test_client
         t = cl.create_table('test_tbl', {'input': StringType()})
```

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_migration.py` & `pixeltable-0.2.2/pixeltable/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_nos.py` & `pixeltable-0.2.2/pixeltable/tests/test_nos.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_snapshot.py` & `pixeltable-0.2.2/pixeltable/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_table.py` & `pixeltable-0.2.2/pixeltable/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_transactional_directory.py` & `pixeltable-0.2.2/pixeltable/tests/test_transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_types.py` & `pixeltable-0.2.2/pixeltable/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_video.py` & `pixeltable-0.2.2/pixeltable/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/test_view.py` & `pixeltable-0.2.2/pixeltable/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/tests/utils.py` & `pixeltable-0.2.2/pixeltable/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from pixeltable import catalog
 from pixeltable.dataframe import DataFrameResultSet
 from pixeltable.env import Env
 from pixeltable.type_system import \
     ColumnType, StringType, IntType, FloatType, ArrayType, BoolType, TimestampType, JsonType, ImageType, VideoType
 
 
+
+
 def make_default_type(t: ColumnType.Type) -> ColumnType:
     if t == ColumnType.Type.STRING:
         return StringType()
     if t == ColumnType.Type.INT:
         return IntType()
     if t == ColumnType.Type.FLOAT:
         return FloatType()
@@ -224,14 +226,21 @@
     return df.to_dict(orient='records')
 
 def get_video_files(include_bad_video=False) -> List[str]:
     tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/videos/*', recursive=True)
     if not include_bad_video:
         glob_result = [f for f in glob_result if 'bad_video' not in f]
+
+    half_res = [f for f in glob_result if 'half_res' in f or 'bad_video' in f]
+    return half_res
+
+def get_test_video_files() -> List[str]:
+    tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
+    glob_result = glob.glob(f'{tests_dir}/**/test_videos/*', recursive=True)
     return glob_result
 
 def get_image_files() -> List[str]:
     tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/imagenette2-160/*', recursive=True)
     return glob_result
```

### Comparing `pixeltable-0.2.1/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.2/pixeltable/tool/create_test_db_dump.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/type_system.py` & `pixeltable-0.2.2/pixeltable/type_system.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/clip.py` & `pixeltable-0.2.2/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/coco.py` & `pixeltable-0.2.2/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/documents.py` & `pixeltable-0.2.2/pixeltable/utils/documents.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/filecache.py` & `pixeltable-0.2.2/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/media_store.py` & `pixeltable-0.2.2/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/parquet.py` & `pixeltable-0.2.2/pixeltable/utils/parquet.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/pytorch.py` & `pixeltable-0.2.2/pixeltable/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/sql.py` & `pixeltable-0.2.2/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.2/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.1/pyproject.toml` & `pixeltable-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.1"
+version = "0.2.2"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
     "pixeltable/tests/data"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.24.1"
-pandas = "^1.5.3"
+pandas = ">=2.0,<3.0"
 pillow = "^9.4.0"
 opencv-python-headless = "^4.7.0.68"
 tqdm = "^4.64.1"
 jmespath = "^1.0.1"
 regex = "^2022.10.31"
 cloudpickle = "^2.2.1"
 psycopg2-binary = "^2.9.5"
 psutil = "^5.9.5"
 sqlalchemy = {extras = ["mypy"], version = "^2.0.23"}
 sqlalchemy-utils = "^0.41.1"
 pgvector = "^0.2.1"
 av = ">=10.0.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
-pgserver = "0.0.5"
+pgserver = "0.0.7"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
 pytest = "^7.2.1"
```

### Comparing `pixeltable-0.2.1/PKG-INFO` & `pixeltable-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: av (>=10.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pgserver (==0.0.5)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: pgserver (==0.0.7)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
@@ -41,24 +41,24 @@
 exploration, modeling, and app development without having to deal with the customary
 data plumbing.
 
 **Pixeltable redefines data infrastructure and workflow orchestration for AI development.**
 It brings together data storage, versioning, and indexing with orchestration and model
 versioning under a declarative table interface, with transformations, model inference,
 and custom logic represented as computed columns.
-<!--
+
 ## Quick Start
 
 If you just want to play around with Pixeltable to see what it's capable of, the easiest way is to run
 the Pixeltable Basics tutorial in colab:
 
-<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/docs/tutorials/pixeltable-basics.ipynb">
+<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
--->
+
 ## Installation
 
 Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
 
 ```
 pip install pixeltable
 ```
```

