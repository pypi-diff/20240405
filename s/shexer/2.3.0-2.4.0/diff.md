# Comparing `tmp/shexer-2.3.0.tar.gz` & `tmp/shexer-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.3.0.tar", last modified: Wed Apr  3 11:55:15 2024, max compression
+gzip compressed data, was "shexer-2.4.0.tar", last modified: Fri Apr  5 16:49:50 2024, max compression
```

## Comparing `shexer-2.3.0.tar` & `shexer-2.4.0.tar`

### file list

```diff
@@ -1,252 +1,256 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.414820 shexer-2.3.0/
--rw-rw-rw-   0        0        0    11558 2023-06-27 16:13:11.000000 shexer-2.3.0/LICENSE
--rw-rw-rw-   0        0        0    27235 2024-04-03 11:55:15.415005 shexer-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    26360 2023-06-27 16:13:11.000000 shexer-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.837550 shexer-2.3.0/local_code/
--rw-rw-rw-   0        0        0        0 2023-07-20 16:50:30.000000 shexer-2.3.0/local_code/__init__.py
--rw-rw-rw-   0        0        0     1278 2023-11-10 20:18:22.000000 shexer-2.3.0/local_code/beyza_test.py
--rw-rw-rw-   0        0        0     1411 2023-11-30 17:16:03.000000 shexer-2.3.0/local_code/img_example.py
--rw-rw-rw-   0        0        0     2756 2023-09-04 15:19:36.000000 shexer-2.3.0/local_code/split_non_split_thats_the_question.py
--rw-rw-rw-   0        0        0     9733 2023-11-08 19:45:06.000000 shexer-2.3.0/local_code/tictactoe.py
--rw-rw-rw-   0        0        0       88 2023-11-13 10:50:47.000000 shexer-2.3.0/local_code/whatever.py
--rw-rw-rw-   0        0        0     1428 2023-10-02 17:19:16.000000 shexer-2.3.0/local_code/yasunori_Test.py
--rw-rw-rw-   0        0        0       86 2024-04-03 11:55:15.419841 shexer-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1370 2024-04-03 11:54:32.000000 shexer-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.860170 shexer-2.3.0/shexer/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/__init__.py
--rw-rw-rw-   0        0        0      644 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.917785 shexer-2.3.0/shexer/core/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.965382 shexer-2.3.0/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.016640 shexer-2.3.0/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3895 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.100211 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      665 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      760 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     2675 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
--rw-rw-rw-   0        0        0       86 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
--rw-rw-rw-   0        0        0     1793 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      815 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4553 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.114576 shexer-2.3.0/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.135524 shexer-2.3.0/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.163451 shexer-2.3.0/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8613 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.217765 shexer-2.3.0/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.243220 shexer-2.3.0/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.307048 shexer-2.3.0/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    17141 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.352536 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.382225 shexer-2.3.0/shexer/io/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.383898 shexer-2.3.0/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.571397 shexer-2.3.0/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16304 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.583685 shexer-2.3.0/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1483 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py
--rw-rw-rw-   0        0        0     2670 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.604438 shexer-2.3.0/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.621320 shexer-2.3.0/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.682312 shexer-2.3.0/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.684308 shexer-2.3.0/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.701263 shexer-2.3.0/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.704254 shexer-2.3.0/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.722207 shexer-2.3.0/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    16449 2023-11-10 20:24:47.000000 shexer-2.3.0/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.737436 shexer-2.3.0/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.755124 shexer-2.3.0/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.781071 shexer-2.3.0/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.784119 shexer-2.3.0/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.818977 shexer-2.3.0/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.879812 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.952657 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.969615 shexer-2.3.0/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/sparql/query.py
--rw-rw-rw-   0        0        0      469 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.148009 shexer-2.3.0/shexer/model/
--rw-rw-rw-   0        0        0      552 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.185555 shexer-2.3.0/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/statement.py
--rw-rw-rw-   0        0        0    24783 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.299050 shexer-2.3.0/shexer/utils/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.457634 shexer-2.3.0/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2322 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12338 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     1723 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    21108 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/log.py
--rw-rw-rw-   0        0        0      761 2023-11-20 19:07:29.000000 shexer-2.3.0/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.479570 shexer-2.3.0/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5708 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.914793 shexer-2.3.0/shexer.egg-info/
--rw-rw-rw-   0        0        0    27235 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8267 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.251578 shexer-2.3.0/test/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-06-27 16:13:11.000000 shexer-2.3.0/test/const.py
--rw-rw-rw-   0        0        0     8963 2023-06-27 16:13:11.000000 shexer-2.3.0/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_allow_opt_cardinality.py
--rw-rw-rw-   0        0        0     3541 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_allow_redundant_or.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.282495 shexer-2.3.0/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-rw-rw-   0        0        0    11274 2024-04-03 11:54:32.000000 shexer-2.3.0/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2557 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_input_format.py
--rw-rw-rw-   0        0        0     4648 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_cap.py
--rw-rw-rw-   0        0        0     3367 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2932 2023-10-20 16:00:26.000000 shexer-2.3.0/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.368573 shexer-2.3.0/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      875 2023-11-10 20:24:47.000000 shexer-2.3.0/test/test_shacl/test_https.py
--rw-rw-rw-   0        0        0     1534 2023-11-10 20:24:47.000000 shexer-2.3.0/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2023-10-20 15:05:20.000000 shexer-2.3.0/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_threshold.py
--rw-rw-rw-   0        0        0     2578 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1900 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.411863 shexer-2.3.0/ws/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.232527 shexer-2.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-27 16:13:11.000000 shexer-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0    27740 2024-04-05 16:49:50.233523 shexer-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26865 2024-04-05 16:49:28.000000 shexer-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.504761 shexer-2.4.0/local_code/
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:50:30.000000 shexer-2.4.0/local_code/__init__.py
+-rw-rw-rw-   0        0        0     1278 2023-11-10 20:18:22.000000 shexer-2.4.0/local_code/beyza_test.py
+-rw-rw-rw-   0        0        0     1411 2023-11-30 17:16:03.000000 shexer-2.4.0/local_code/img_example.py
+-rw-rw-rw-   0        0        0     2756 2023-09-04 15:19:36.000000 shexer-2.4.0/local_code/split_non_split_thats_the_question.py
+-rw-rw-rw-   0        0        0     9733 2023-11-08 19:45:06.000000 shexer-2.4.0/local_code/tictactoe.py
+-rw-rw-rw-   0        0        0       88 2023-11-13 10:50:47.000000 shexer-2.4.0/local_code/whatever.py
+-rw-rw-rw-   0        0        0     1428 2023-10-02 17:19:16.000000 shexer-2.4.0/local_code/yasunori_Test.py
+-rw-rw-rw-   0        0        0       86 2024-04-05 16:49:50.236516 shexer-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2024-04-05 16:49:28.000000 shexer-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.511716 shexer-2.4.0/shexer/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.554611 shexer-2.4.0/shexer/core/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.577540 shexer-2.4.0/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.610452 shexer-2.4.0/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3895 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.689272 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      665 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      760 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     2675 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+-rw-rw-rw-   0        0        0       86 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
+-rw-rw-rw-   0        0        0     1793 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      815 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4553 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.700220 shexer-2.4.0/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.712226 shexer-2.4.0/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.737144 shexer-2.4.0/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8613 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.774024 shexer-2.4.0/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.786988 shexer-2.4.0/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.822929 shexer-2.4.0/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    17141 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.855806 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.875752 shexer-2.4.0/shexer/io/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.877745 shexer-2.4.0/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.996509 shexer-2.4.0/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    16304 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.008477 shexer-2.4.0/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1483 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py
+-rw-rw-rw-   0        0        0     2670 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.023474 shexer-2.4.0/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.034444 shexer-2.4.0/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.070349 shexer-2.4.0/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.072322 shexer-2.4.0/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.077299 shexer-2.4.0/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.079288 shexer-2.4.0/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.091256 shexer-2.4.0/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    16449 2023-11-10 20:24:47.000000 shexer-2.4.0/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.105256 shexer-2.4.0/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.117186 shexer-2.4.0/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.135177 shexer-2.4.0/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.139156 shexer-2.4.0/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.160118 shexer-2.4.0/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.211973 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.262874 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.268820 shexer-2.4.0/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/sparql/query.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.273807 shexer-2.4.0/shexer/io/uml/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/io/uml/__init__.py
+-rw-rw-rw-   0        0        0     6256 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/io/uml/uml_serializer.py
+-rw-rw-rw-   0        0        0      469 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.383542 shexer-2.4.0/shexer/model/
+-rw-rw-rw-   0        0        0      552 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.403500 shexer-2.4.0/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    25844 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.486249 shexer-2.4.0/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.588078 shexer-2.4.0/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2322 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12338 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     2109 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    21108 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      761 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.601024 shexer-2.4.0/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5749 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.551609 shexer-2.4.0/shexer.egg-info/
+-rw-rw-rw-   0        0        0    27740 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8346 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.130805 shexer-2.4.0/test/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-06-27 16:13:11.000000 shexer-2.4.0/test/const.py
+-rw-rw-rw-   0        0        0     9389 2024-04-05 16:49:28.000000 shexer-2.4.0/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_allow_opt_cardinality.py
+-rw-rw-rw-   0        0        0     3541 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_allow_redundant_or.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.158753 shexer-2.4.0/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0    11274 2024-04-03 12:10:04.000000 shexer-2.4.0/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2557 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     7818 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_input_format.py
+-rw-rw-rw-   0        0        0     4648 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_cap.py
+-rw-rw-rw-   0        0        0     3367 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2932 2023-10-20 16:00:26.000000 shexer-2.4.0/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.209586 shexer-2.4.0/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      875 2023-11-10 20:24:47.000000 shexer-2.4.0/test/test_shacl/test_https.py
+-rw-rw-rw-   0        0        0     1534 2023-11-10 20:24:47.000000 shexer-2.4.0/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2023-10-20 15:05:20.000000 shexer-2.4.0/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2729 2024-04-05 16:49:28.000000 shexer-2.4.0/test/test_uml_gen.py
+-rw-rw-rw-   0        0        0     2578 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1931 2024-04-05 16:49:28.000000 shexer-2.4.0/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.230531 shexer-2.4.0/ws/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/wsgi.py
```

### Comparing `shexer-2.3.0/LICENSE` & `shexer-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/PKG-INFO` & `shexer-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.3.0
+Version: 2.4.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -52,14 +52,16 @@
 
 * **Several ways to provide input data**, consisting of a target graph and some target shapes. Tha graph can be provided via raw string content, local/remote file(s), or tracking on the fly some triples from a SPARQL endpoint. There are defined interfaces in case you want to implement some other way to provide input information. 
 
 * **Several ways to select your target shapes**. You may want to generate shapes for each class in the graph or maybe just for some of them. You may want to generate a shape for some custom node agrupations. Or maybe you are extracting some shapes from a big grpah and you just want to explore the neighborhood of some seed nodes.  For custom node aggrupations sheXer supports ShEx's shape maps syntax, and it provides configuration params to target different classes or graph depths. 
 
 * **Valid ShEx and SHACL**. The produced shapes are compilant with the current specification of ShEx2 and SHACL.
 
+* **UML**. Ypu can also generate UML-like views of the extracted schemas.
+
 * **Threshold of tolerance**. The constraints inferred for each shape may not be compatible with every node associated to the shapes. With this threshold you can indicate the minimun percentage of nodes that should conform with a constraint c. If c does not reach the indicated ratio, its associated information will not appear in the final shape.
 
 * **Informative comments** (just for ShEx, by now). Each constraint inferred is associated to one or more comments. Those comments include different types of information, such as the ratio of nodes that actually conform with a given constraint. You can keep this informative comments or exclude them from the results.
 
 * **Sorted constraints** (just for ShEx, by now). For a given constraint, sheXer keeps the ratio of nodes that conform with it. This is used as a score of trustworthiness. The constraints in a shape are sorted w.r.t. this score.
 
 * **Literals recognition**. All kinds of typed literals are recognized and treated separately when inferring the constraints. In case a literal is not explicitly associated with a type in the original KG, xsd:string is used by default. By default, when sheXer finds an untyped literal it tries to infer its type when it is a number. Support to some other untyped literals, such as geolocated points, may be included in future releases.
@@ -83,15 +85,15 @@
 
 ## Experimental results
 
 In the folder [experiments](https://github.com/DaniFdezAlvarez/shexer/tree/develop/experiments), you can see some results of applying this tool over different graphs with different configurations.
 
 ## Example code
 
-The following code is takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
+The following code takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
 
 ```python
 from shexer.shaper import Shaper
 from shexer.consts import NT, SHEXC, SHACL_TURTLE
 
 target_classes = [
     "http://example.org/Person",
@@ -242,9 +244,11 @@
 
 The method __shex\_graph__  of shexer triggers all the inference process and gives back a result. It receives several parameters, being optional some of them:
 
 * string_output (default False): when it is set to True, the method returns a string representation of the inferred shapes. It must be set to True iff output_file is None.
 * output_file (default None): it specifies the path of the file in which the inferred shapes will be written. It must have a value different to None iff string_output is False.
 * output_format (default "ShExC"): format in which the inferred shapes will be serialized. The values currently supported are const.SHEXC and const.SHACLE_TURTLE.
 * aceptance_threshold (default 0): Given a certain inferred constraint __c__ for a shape __s__, the ammount of instances which conform to this constraint (ignoring constraints with '\*' cardinality) should be at least __aceptance\_threshold__. If this does not happen, then __c__ will not be included in __s__.
+* verbose (dafault False): when it is set to True, the extraction process will print log messages through the standard output.
+* to_uml_path (default None). This parameter expects to receive a disk path. If you provide a value here, sheXer will generate a UML diagram containing the extracted scheme and will save it in the path indicated as a PNG image. WARNING: you should be connected to Internet in  order to make this work.
```

### Comparing `shexer-2.3.0/README.md` & `shexer-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 * **Several ways to provide input data**, consisting of a target graph and some target shapes. Tha graph can be provided via raw string content, local/remote file(s), or tracking on the fly some triples from a SPARQL endpoint. There are defined interfaces in case you want to implement some other way to provide input information. 
 
 * **Several ways to select your target shapes**. You may want to generate shapes for each class in the graph or maybe just for some of them. You may want to generate a shape for some custom node agrupations. Or maybe you are extracting some shapes from a big grpah and you just want to explore the neighborhood of some seed nodes.  For custom node aggrupations sheXer supports ShEx's shape maps syntax, and it provides configuration params to target different classes or graph depths. 
 
 * **Valid ShEx and SHACL**. The produced shapes are compilant with the current specification of ShEx2 and SHACL.
 
+* **UML**. Ypu can also generate UML-like views of the extracted schemas.
+
 * **Threshold of tolerance**. The constraints inferred for each shape may not be compatible with every node associated to the shapes. With this threshold you can indicate the minimun percentage of nodes that should conform with a constraint c. If c does not reach the indicated ratio, its associated information will not appear in the final shape.
 
 * **Informative comments** (just for ShEx, by now). Each constraint inferred is associated to one or more comments. Those comments include different types of information, such as the ratio of nodes that actually conform with a given constraint. You can keep this informative comments or exclude them from the results.
 
 * **Sorted constraints** (just for ShEx, by now). For a given constraint, sheXer keeps the ratio of nodes that conform with it. This is used as a score of trustworthiness. The constraints in a shape are sorted w.r.t. this score.
 
 * **Literals recognition**. All kinds of typed literals are recognized and treated separately when inferring the constraints. In case a literal is not explicitly associated with a type in the original KG, xsd:string is used by default. By default, when sheXer finds an untyped literal it tries to infer its type when it is a number. Support to some other untyped literals, such as geolocated points, may be included in future releases.
@@ -63,15 +65,15 @@
 
 ## Experimental results
 
 In the folder [experiments](https://github.com/DaniFdezAlvarez/shexer/tree/develop/experiments), you can see some results of applying this tool over different graphs with different configurations.
 
 ## Example code
 
-The following code is takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
+The following code takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
 
 ```python
 from shexer.shaper import Shaper
 from shexer.consts import NT, SHEXC, SHACL_TURTLE
 
 target_classes = [
     "http://example.org/Person",
@@ -222,9 +224,11 @@
 
 The method __shex\_graph__  of shexer triggers all the inference process and gives back a result. It receives several parameters, being optional some of them:
 
 * string_output (default False): when it is set to True, the method returns a string representation of the inferred shapes. It must be set to True iff output_file is None.
 * output_file (default None): it specifies the path of the file in which the inferred shapes will be written. It must have a value different to None iff string_output is False.
 * output_format (default "ShExC"): format in which the inferred shapes will be serialized. The values currently supported are const.SHEXC and const.SHACLE_TURTLE.
 * aceptance_threshold (default 0): Given a certain inferred constraint __c__ for a shape __s__, the ammount of instances which conform to this constraint (ignoring constraints with '\*' cardinality) should be at least __aceptance\_threshold__. If this does not happen, then __c__ will not be included in __s__.
+* verbose (dafault False): when it is set to True, the extraction process will print log messages through the standard output.
+* to_uml_path (default None). This parameter expects to receive a disk path. If you provide a value here, sheXer will generate a UML diagram containing the extracted scheme and will save it in the path indicated as a PNG image. WARNING: you should be connected to Internet in  order to make this work.
```

### Comparing `shexer-2.3.0/local_code/beyza_test.py` & `shexer-2.4.0/local_code/beyza_test.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/local_code/img_example.py` & `shexer-2.4.0/local_code/img_example.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/local_code/split_non_split_thats_the_question.py` & `shexer-2.4.0/local_code/split_non_split_thats_the_question.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/local_code/tictactoe.py` & `shexer-2.4.0/local_code/tictactoe.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/local_code/yasunori_Test.py` & `shexer-2.4.0/local_code/yasunori_Test.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/setup.py` & `shexer-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.3.0',
+  version = '2.4.0',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.3.0/shexer/consts.py` & `shexer-2.4.0/shexer/consts.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,10 @@
 GZ = "gz"
 
 # FREQUENCY MODES
 
 RATIO_INSTANCES = "ratio"
 ABSOLUTE_INSTANCES = "abs"
 MIXED_INSTANCES = "mixed"
+
+# UML
+UML_PLANT_SERVER = "http://www.plantuml.com/plantuml/img/"
```

### Comparing `shexer-2.3.0/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.4.0/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.4.0/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.4.0/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/instance_tracker.py` & `shexer-2.4.0/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.4.0/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.4.0/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/profiling/class_profiler.py` & `shexer-2.4.0/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.4.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.4.0/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.4.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/shexing/class_shexer.py` & `shexer-2.4.0/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.4.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.4.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.4.0/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.4.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.4.0/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.4.0/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.4.0/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.4.0/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.4.0/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/io/sparql/query.py` & `shexer-2.4.0/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/IRI.py` & `shexer-2.4.0/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/Macro.py` & `shexer-2.4.0/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.4.0/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/graph/abstract_sgraph.py` & `shexer-2.4.0/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.4.0/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.4.0/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/hierarchy_tree.py` & `shexer-2.4.0/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/node_selector.py` & `shexer-2.4.0/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/shape.py` & `shexer-2.4.0/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/shape_map.py` & `shexer-2.4.0/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/model/statement.py` & `shexer-2.4.0/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/shaper.py` & `shexer-2.4.0/shexer/shaper.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     RDF_XML, FIXED_SHAPE_MAP, JSON_LD, RDF_TYPE, SHAPES_DEFAULT_NAMESPACE, ZIP, GZ
 from shexer.utils.factories.class_profiler_factory import get_class_profiler
 from shexer.utils.factories.instance_tracker_factory import get_instance_tracker
 from shexer.utils.factories.class_shexer_factory import get_class_shexer
 from shexer.utils.factories.remote_graph_factory import get_remote_graph_if_needed
 from shexer.utils.factories.shape_map_factory import get_shape_map_if_needed
 from shexer.io.profile.formater.abstract_profile_serializer import AbstractProfileSerializer
-from shexer.utils.factories.shape_serializer_factory import get_shape_serializer
+from shexer.utils.factories.shape_serializer_factory import get_shape_serializer, get_uml_serializer
 from shexer.utils.namespaces import find_adequate_prefix_for_shapes_namespaces
 from shexer.utils.log import log_msg
 from shexer.consts import RATIO_INSTANCES
 
 
 class Shaper(object):
 
@@ -226,40 +226,66 @@
             return AbstractProfileSerializer(self._profile).get_string_representation()
         return AbstractProfileSerializer(self._profile).write_profile_to_file(target_file=output_file)
 
     def shex_graph(self, string_output=False,
                    output_file=None,
                    output_format=SHEXC,
                    acceptance_threshold=0,
-                   verbose=False):
+                   verbose=False,
+                   to_uml_path=None):
         """
         :param string_output:
         :param output_file:
         :param output_format:
         :param acceptance_threshold:
         :param verbose:
+        :param to_uml_path:
         :return:
         """
-        self._check_correct_output_params(string_output, output_file)
+        self._check_correct_output_params(string_output, output_file, to_uml_path)
         self._check_output_format(output_format)
         self._check_aceptance_threshold(acceptance_threshold)
         if self._target_classes_dict is None:
             self._launch_instance_tracker(verbose=verbose)
         if self._profile is None:
             self._launch_class_profiler(verbose=verbose)
         if self._shape_list is None:
             self._launch_class_shexer(acceptance_threshold=acceptance_threshold,
                                       verbose=verbose)
         log_msg(verbose=verbose,
                 msg="Building_output...")
-        serializer = self._build_shapes_serializer(target_file=output_file,
-                                                   string_return=string_output,
-                                                   output_format=output_format)
-        return serializer.serialize_shapes()  # If string return is active, returns string.
-        # Otherwise, it writes to file and returns None
+
+        if to_uml_path is not None:
+            log_msg(verbose=verbose,
+                    msg="Trying to generat UML diagram...")
+            try:
+                self._generate_uml_diagram(to_uml_path)
+                log_msg(verbose=verbose,
+                        msg="UML diagram generated...")
+            except ResourceWarning as e:  # I think this is related to UMLPlant and I can't close the connection from here
+                pass
+
+        if string_output or output_file is not None:
+            log_msg(verbose=verbose,
+                    msg="Generating text serialization...")
+            serializer = self._build_shapes_serializer(target_file=output_file,
+                                                       string_return=string_output,
+                                                       output_format=output_format)
+
+            return serializer.serialize_shapes()  # If string return is active, returns string.
+
+
+    def _generate_uml_diagram(self, to_uml_path):
+        serializer = get_uml_serializer(shapes_list=self._shape_list,
+                                        image_path=to_uml_path,
+                                        namespaces_dict=self._namespaces_dict)
+        serializer.serialize_shapes()
+
+
+
 
     def _add_shapes_namespaces_to_namespaces_dict(self):
         self._namespaces_dict[self._shapes_namespace] = \
             find_adequate_prefix_for_shapes_namespaces(self._namespaces_dict)
 
     def _launch_class_profiler(self, verbose=False):
         if self._class_profiler is None:
@@ -377,17 +403,17 @@
                                     inverse_paths=self._inverse_paths,
                                     compression_mode=self._compression_mode,
                                     disable_endpoint_cache=self._disable_endpoint_cache,
                                     instances_cap=self._instances_cap)
 
 
     @staticmethod
-    def _check_correct_output_params(string_output, target_file):
-        if not string_output and target_file is None:
-            raise ValueError("You must provide a target path or set string output to True")
+    def _check_correct_output_params(string_output, target_file, to_uml_path):
+        if not string_output and target_file is None and to_uml_path is None:
+            raise ValueError("You must provide a target path , set string output to True and/or give a value to to_uml_path")
 
     @staticmethod
     def _check_input_format(input_format):
         if input_format not in [NT, TSV_SPO, N3, TURTLE, RDF_XML, JSON_LD, TURTLE_ITER]:
             raise ValueError("Currently unsupported input format: " + input_format)
 
     @staticmethod
```

### Comparing `shexer-2.3.0/shexer/utils/compression.py` & `shexer-2.4.0/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.4.0/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.4.0/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/h_tree.py` & `shexer-2.4.0/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.4.0/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/shape_map_factory.py` & `shexer-2.4.0/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.4.0/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.4.0/shexer/utils/factories/shape_serializer_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from shexer.consts import SHEXC, SHACL_TURTLE
 from shexer.io.shex.formater.shex_serializer import ShexSerializer
 from shexer.io.shacl.formater.shacl_serializer import ShaclSerializer
-from shexer.consts import RATIO_INSTANCES
+from shexer.io.uml.uml_serializer import UMLSerializer
+from shexer.consts import RATIO_INSTANCES, UML_PLANT_SERVER
 
 
 def get_shape_serializer(output_format, shapes_list, target_file=None, string_return=False, namespaces_dict=None,
                          instantiation_property=None, disable_comments=False, wikidata_annotation=False,
                          instances_report_mode=RATIO_INSTANCES, detect_minimal_iri=False):
     if output_format == SHEXC:
         return ShexSerializer(target_file=target_file,
@@ -22,7 +23,14 @@
                                shapes_list=shapes_list,
                                namespaces_dict=namespaces_dict,
                                string_return=string_return,
                                instantiation_property_str=instantiation_property,
                                wikidata_annotation=wikidata_annotation)
     else:
         raise ValueError("Currently unsupported format in 'output_format': " + output_format)
+
+
+def get_uml_serializer(shapes_list, image_path, url_server=UML_PLANT_SERVER, namespaces_dict=None,):
+    return UMLSerializer(shapes_list=shapes_list,
+                         url_server=url_server,
+                         image_path=image_path,
+                         namespaces_dict=namespaces_dict)
```

### Comparing `shexer-2.3.0/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.4.0/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/namespaces.py` & `shexer-2.4.0/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/obj_references.py` & `shexer-2.4.0/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/shapes.py` & `shexer-2.4.0/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/target_elements.py` & `shexer-2.4.0/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.4.0/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/triple_yielders.py` & `shexer-2.4.0/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/shexer/utils/uri.py` & `shexer-2.4.0/shexer/utils/uri.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,17 @@
             result = target_uri.replace(a_prefix+":", prefix_namespaces_dict[a_prefix])
             if include_corners:
                 result = add_corners(result)
             return result
     raise ValueError("Unrecognized prefix in the following element" + target_uri)
 
 
-def prefixize_uri_if_possible(target_uri, namespaces_prefix_dict):
+def prefixize_uri_if_possible(target_uri, namespaces_prefix_dict, corners=True):
     best_match = None
-    candidate_uri = remove_corners(target_uri)
+    candidate_uri = remove_corners(target_uri) if corners else target_uri
     for a_namespace in namespaces_prefix_dict:  # Prefixed element (all literals are prefixed elements)
         if candidate_uri.startswith(a_namespace):
             if "/" not in candidate_uri[len(a_namespace):] and \
                 "#" not in candidate_uri[len(a_namespace):]:
                 best_match = a_namespace
                 break
             # if best_match is None or len(best_match) < len(a_namespace):
```

### Comparing `shexer-2.3.0/shexer.egg-info/PKG-INFO` & `shexer-2.4.0/shexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.3.0
+Version: 2.4.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -52,14 +52,16 @@
 
 * **Several ways to provide input data**, consisting of a target graph and some target shapes. Tha graph can be provided via raw string content, local/remote file(s), or tracking on the fly some triples from a SPARQL endpoint. There are defined interfaces in case you want to implement some other way to provide input information. 
 
 * **Several ways to select your target shapes**. You may want to generate shapes for each class in the graph or maybe just for some of them. You may want to generate a shape for some custom node agrupations. Or maybe you are extracting some shapes from a big grpah and you just want to explore the neighborhood of some seed nodes.  For custom node aggrupations sheXer supports ShEx's shape maps syntax, and it provides configuration params to target different classes or graph depths. 
 
 * **Valid ShEx and SHACL**. The produced shapes are compilant with the current specification of ShEx2 and SHACL.
 
+* **UML**. Ypu can also generate UML-like views of the extracted schemas.
+
 * **Threshold of tolerance**. The constraints inferred for each shape may not be compatible with every node associated to the shapes. With this threshold you can indicate the minimun percentage of nodes that should conform with a constraint c. If c does not reach the indicated ratio, its associated information will not appear in the final shape.
 
 * **Informative comments** (just for ShEx, by now). Each constraint inferred is associated to one or more comments. Those comments include different types of information, such as the ratio of nodes that actually conform with a given constraint. You can keep this informative comments or exclude them from the results.
 
 * **Sorted constraints** (just for ShEx, by now). For a given constraint, sheXer keeps the ratio of nodes that conform with it. This is used as a score of trustworthiness. The constraints in a shape are sorted w.r.t. this score.
 
 * **Literals recognition**. All kinds of typed literals are recognized and treated separately when inferring the constraints. In case a literal is not explicitly associated with a type in the original KG, xsd:string is used by default. By default, when sheXer finds an untyped literal it tries to infer its type when it is a number. Support to some other untyped literals, such as geolocated points, may be included in future releases.
@@ -83,15 +85,15 @@
 
 ## Experimental results
 
 In the folder [experiments](https://github.com/DaniFdezAlvarez/shexer/tree/develop/experiments), you can see some results of applying this tool over different graphs with different configurations.
 
 ## Example code
 
-The following code is takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
+The following code takes the graph in _raw\_graph_ and extracts shapes for instances of the classes <http://example.org/Person> and <http://example.org/Gender>. The input file format in n-triples and the results are serialized in ShExC to the file shaper_example.shex.
 
 ```python
 from shexer.shaper import Shaper
 from shexer.consts import NT, SHEXC, SHACL_TURTLE
 
 target_classes = [
     "http://example.org/Person",
@@ -242,9 +244,11 @@
 
 The method __shex\_graph__  of shexer triggers all the inference process and gives back a result. It receives several parameters, being optional some of them:
 
 * string_output (default False): when it is set to True, the method returns a string representation of the inferred shapes. It must be set to True iff output_file is None.
 * output_file (default None): it specifies the path of the file in which the inferred shapes will be written. It must have a value different to None iff string_output is False.
 * output_format (default "ShExC"): format in which the inferred shapes will be serialized. The values currently supported are const.SHEXC and const.SHACLE_TURTLE.
 * aceptance_threshold (default 0): Given a certain inferred constraint __c__ for a shape __s__, the ammount of instances which conform to this constraint (ignoring constraints with '\*' cardinality) should be at least __aceptance\_threshold__. If this does not happen, then __c__ will not be included in __s__.
+* verbose (dafault False): when it is set to True, the extraction process will print log messages through the standard output.
+* to_uml_path (default None). This parameter expects to receive a disk path. If you provide a value here, sheXer will generate a UML diagram containing the extracted scheme and will save it in the path indicated as a PNG image. WARNING: you should be connected to Internet in  order to make this work.
```

### Comparing `shexer-2.3.0/shexer.egg-info/SOURCES.txt` & `shexer-2.4.0/shexer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,16 @@
 shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
 shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
 shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
 shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
 shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
 shexer/io/sparql/__init__.py
 shexer/io/sparql/query.py
+shexer/io/uml/__init__.py
+shexer/io/uml/uml_serializer.py
 shexer/model/IRI.py
 shexer/model/Literal.py
 shexer/model/Macro.py
 shexer/model/__init__.py
 shexer/model/bnode.py
 shexer/model/const_elem_types.py
 shexer/model/fixed_prop_choice_statement.py
@@ -187,14 +189,15 @@
 test/test_shape_map_file.py
 test/test_shape_map_format.py
 test/test_shape_qualifiers_mode.py
 test/test_shapes_namespaces.py
 test/test_sort.py
 test/test_target_classes.py
 test/test_threshold.py
+test/test_uml_gen.py
 test/test_url_endpoint.py
 test/test_url_graph.py
 test/test_wikidata_annotation.py
 test/test_bugs/__init__.py
 test/test_bugs/test_no_sharp_in_auto_shape_names.py
 test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
 test/test_shacl/__init__.py
```

### Comparing `shexer-2.3.0/test/const.py` & `shexer-2.4.0/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/t_utils.py` & `shexer-2.4.0/test/t_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from rdflib import Graph
 from rdflib.compare import to_isomorphic, graph_diff
 import re
+from os.path import isfile, exists as file_exists
+from os import remove
 
 _BLANKS = re.compile("[ \t]+")
 _LINE_JUMPS = re.compile("\n+")
 
 _PREFIX = "PREFIX"
 _BEG_SHAPE = "{"
 _END_SHAPE = "}"
@@ -26,20 +28,22 @@
             namespaces.append(a_line)
         elif a_line.startswith(_BEG_SHAPE):
             current_shape = last_line
             shapes[last_line] = []
         elif a_line.startswith(_END_SHAPE):
             current_shape = None
         elif current_shape is not None:
-            shapes[current_shape].append(a_line.replace(";", "").strip())  # Avoid trailing ";", that can be there or not
+            shapes[current_shape].append(
+                a_line.replace(";", "").strip())  # Avoid trailing ";", that can be there or not
 
         last_line = a_line  # Always execute
 
     return namespaces, shapes
 
+
 def get_namespaces_and_shapes_from_str_with_or(str_target):
     namespaces = []
     shapes = {}
     last_line = ""
     current_shape = None
 
     or_mode = False
@@ -83,24 +87,26 @@
 
 def unordered_sets_match(sets1, sets2):
     for a_set1 in sets1:
         if a_set1 not in sets2:
             return False
     return True
 
+
 def ordered_sets_match(sets1, sets2):
     if len(sets1) != len(sets2):
         return False
-    for i in range (len(sets1)):
+    for i in range(len(sets1)):
         if sets1[i] != sets2[i]:
             return False
     return True
 
 
-def simple_and_or_str_constraints(str_constraints):  # TODO Fix here. Receive a dict, not a list. check call to this method
+def simple_and_or_str_constraints(
+        str_constraints):  # TODO Fix here. Receive a dict, not a list. check call to this method
     simple_c = []
     or_c = []
     for a_c in str_constraints:
         if _OR in a_c:
             or_c.append(a_c)
         else:
             simple_c.append(a_c)
@@ -111,14 +117,15 @@
     if len(or_list_1) != len(or_list_2):
         return False
     for i in range(len(or_list_1)):
         or_list_1[i] = set(or_list_1[i].split(_OR))
         or_list_2[i] = set(or_list_2[i].split(_OR))
     return ordered_sets_match(or_list_1, or_list_2)
 
+
 def unordered_or_constraints_match(or_list_1, or_list_2):
     if len(or_list_1) != len(or_list_2):
         return False
 
     for i in range(len(or_list_1)):
         or_list_1[i] = set(or_list_1[i].split("  "))
         or_list_2[i] = set(or_list_2[i].split("  "))
@@ -152,28 +159,31 @@
     for a_key_label in shapes1:
         if a_key_label not in shapes2:
             return False
         if not unordered_lists_match(shapes1[a_key_label], shapes2[a_key_label]):
             return False
     return True
 
+
 def sorted_constraints_comparison(shapes1, shapes2):
     for a_key_label in shapes1:
         if a_key_label not in shapes2:
             return False
         if not ordered_lists_match(shapes1[a_key_label], shapes2[a_key_label]):
             return False
     return True
 
+
 def simple_constraints_comparison(shapes1, shapes2, check_order=False):
     if not check_order:
         return unsorted_constraints_comparison(shapes1, shapes2)
     else:
         return sorted_constraints_comparison(shapes1, shapes2)
 
+
 def shapes_match(shapes1, shapes2, or_shapes=False, check_order=False):
     if len(shapes1) != len(shapes2):
         return False
     if or_shapes:
         return or_shapes_comparison(shapes1, shapes2, check_order)
     return simple_constraints_comparison(shapes1, shapes2, check_order)
 
@@ -190,55 +200,58 @@
 def normalize_str(str_target):
     result = str_target.strip()
     result = _BLANKS.sub(result, " ")
     return _LINE_JUMPS.sub(result, "\n")
 
 
 def tunned_str_comparison(str1, str2, or_shapes=False, check_order=False):
-
     if normalize_str(str1) == normalize_str(str2):
         return True
     else:
         return complex_shape_comparison(str1, str2, or_shapes, check_order)
 
 
 def file_vs_str_tunned_comparison(file_path, str_target, or_shapes=False, check_order=False):
     with open(file_path, "r") as in_stream:
         content = in_stream.read()
     return tunned_str_comparison(content, str_target, or_shapes, check_order)
 
+
 def file_vs_str_exact_comparison(file_path, target_str):
     with open(file_path, "r") as in_stream:
         return in_stream.read().strip() == target_str.strip()
 
+
 def file_vs_file_tunned_comparison(file_path1, file_path2, or_shapes=False):
     with open(file_path1, "r") as in_stream:
         content1 = in_stream.read()
     with open(file_path2, "r") as in_stream:
         content2 = in_stream.read()
     return tunned_str_comparison(content1, content2, or_shapes)
 
+
 def number_of_shapes(target_str):
     counter = 0
     for a_line in target_str.split("\n"):
         if a_line.startswith(_BEG_SHAPE):
             counter += 1
     return counter
 
+
 def shape_contains_constraint(target_str, shape, constraint):
-    constraint = constraint.replace(";","").strip()
+    constraint = constraint.replace(";", "").strip()
     lines = target_str.split("\n")
     seeking_mode = False
     for i in range(len(lines)):
         if seeking_mode:
             if lines[i].replace(";", "").strip() == constraint:
                 return True
             if lines[i].startswith(_END_SHAPE):
                 return False
-        if lines[i].startswith(_BEG_SHAPE) and shape == lines[i-1].strip():
+        if lines[i].startswith(_BEG_SHAPE) and shape == lines[i - 1].strip():
             seeking_mode = True
     return False
 
 
 def graph_comparison_rdflib(g1, g2):
     iso1 = to_isomorphic(g1)
     iso2 = to_isomorphic(g2)
@@ -251,14 +264,15 @@
     g1.parse(data=str_target, format=format)
 
     g2 = Graph()
     g2.parse(source=file_path, format=format)
 
     return graph_comparison_rdflib(g1, g2)
 
+
 def text_contains_lines(text, list_lines):
     text = _BLANKS.sub(" ", text)
     for a_line in list_lines:
         a_line = _BLANKS.sub(" ", a_line)
         if a_line not in text:
             return False
         return True
@@ -266,7 +280,20 @@
 
 def no_sharp_in_shepe_names(str_shapes):
     _, shapes = get_namespaces_and_shapes_from_str(str_shapes, or_shapes=False)
     for a_key_label in shapes:
         if '#' in a_key_label:
             return False
     return True
+
+
+def check_file_exist(file_path):
+    if not isfile(file_path):
+        raise FileExistsError(f"The expected file was not found in disk: {file_path}")
+
+
+def delete_file(file_path):
+    if file_exists(file_path):
+        try:
+            remove(file_path)
+        except:
+            pass
```

### Comparing `shexer-2.3.0/test/test_all_classes_mode.py` & `shexer-2.4.0/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_allow_opt_cardinality.py` & `shexer-2.4.0/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_allow_redundant_or.py` & `shexer-2.4.0/test/test_allow_redundant_or.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.4.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.4.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_compression_mode.py` & `shexer-2.4.0/test/test_compression_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_decimals.py` & `shexer-2.4.0/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_depth_for_building_subgraph.py` & `shexer-2.4.0/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_detect_minimal_iri.py` & `shexer-2.4.0/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_disable_comments.py` & `shexer-2.4.0/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_disable_endpoint_cache.py` & `shexer-2.4.0/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_disable_exact_cardinality.py` & `shexer-2.4.0/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_disable_or_statements.py` & `shexer-2.4.0/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_discard_and_compliant.py` & `shexer-2.4.0/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_file_target_classes.py` & `shexer-2.4.0/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_graph_file_input.py` & `shexer-2.4.0/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_graph_list_of_file_inputs.py` & `shexer-2.4.0/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.4.0/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_input_format.py` & `shexer-2.4.0/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_instances_cap.py` & `shexer-2.4.0/test/test_instances_cap.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_instances_file_input.py` & `shexer-2.4.0/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_instances_report.py` & `shexer-2.4.0/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_instantiation_property.py` & `shexer-2.4.0/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_inverse_paths.py` & `shexer-2.4.0/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_keep_less_specific.py` & `shexer-2.4.0/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_list_of_url_input.py` & `shexer-2.4.0/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_namespaces_dict.py` & `shexer-2.4.0/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_namespaces_to_ignore.py` & `shexer-2.4.0/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_raw_graph.py` & `shexer-2.4.0/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_raw_shape_map.py` & `shexer-2.4.0/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_rdflib_graph.py` & `shexer-2.4.0/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_remove_empty_sahpes.py` & `shexer-2.4.0/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shacl/test_annotation.py` & `shexer-2.4.0/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shacl/test_class_selection.py` & `shexer-2.4.0/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.4.0/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shacl/test_https.py` & `shexer-2.4.0/test/test_shacl/test_https.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shacl/test_literal_types.py` & `shexer-2.4.0/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shape_map_file.py` & `shexer-2.4.0/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shape_map_format.py` & `shexer-2.4.0/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shape_qualifiers_mode.py` & `shexer-2.4.0/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_shapes_namespaces.py` & `shexer-2.4.0/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_sort.py` & `shexer-2.4.0/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_target_classes.py` & `shexer-2.4.0/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_threshold.py` & `shexer-2.4.0/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_url_endpoint.py` & `shexer-2.4.0/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_url_graph.py` & `shexer-2.4.0/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.3.0/test/test_wikidata_annotation.py` & `shexer-2.4.0/test/test_wikidata_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from shexer.shaper import Shaper
 from test.const import BASE_FILES
 from test.t_utils import file_vs_str_tunned_comparison, text_contains_lines
+import os.path as pth
 
-_BASE_DIR = BASE_FILES + "wikidata_annotation\\"
+_BASE_DIR = BASE_FILES + "wikidata_annotation" + pth.sep
 
 class TestWikidataAnnotation(unittest.TestCase):
 
     def test_no_annotation(self):
         shaper = Shaper(all_classes_mode=True,
                         graph_file_input=_BASE_DIR + "wiki_example.ttl",
                         instantiation_property="http://www.wikidata.org/prop/direct/P31",
```

### Comparing `shexer-2.3.0/ws/shexer_rest.py` & `shexer-2.4.0/ws/shexer_rest.py`

 * *Files identical despite different names*

