# Comparing `tmp/tidal_per_transformers-0.1.0.tar.gz` & `tmp/tidal_per_transformers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_per_transformers-0.1.0.tar", max compression
+gzip compressed data, was "tidal_per_transformers-0.1.1.tar", max compression
```

## Comparing `tidal_per_transformers-0.1.0.tar` & `tidal_per_transformers-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0    11341 2024-03-01 12:16:53.534932 tidal_per_transformers-0.1.0/LICENSE
--rw-r--r--   0        0        0      736 2024-03-01 12:16:53.534932 tidal_per_transformers-0.1.0/README.md
--rw-r--r--   0        0        0     1080 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/__init__.py
--rw-r--r--   0        0        0     2700 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/__init__.py
--rw-r--r--   0        0        0     1598 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/aggregate_transformer.py
--rw-r--r--   0        0        0     2163 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artifact_id_mapping_by_user_country_transformer.py
--rw-r--r--   0        0        0     2033 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artist_compound_transformer.py
--rw-r--r--   0        0        0     3409 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artist_filter_transformer.py
--rw-r--r--   0        0        0     2917 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
--rw-r--r--   0        0        0      824 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
--rw-r--r--   0        0        0     1031 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
--rw-r--r--   0        0        0     1750 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/clean_text_transformer.py
--rw-r--r--   0        0        0     1171 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
--rw-r--r--   0        0        0     1887 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
--rw-r--r--   0        0        0      912 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
--rw-r--r--   0        0        0     1299 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/distinct_sequence_transformer.py
--rw-r--r--   0        0        0      346 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/distinct_transformer.py
--rw-r--r--   0        0        0     2845 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/diversity_sort_transformer.py
--rw-r--r--   0        0        0      451 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/drop_columns_transformer.py
--rw-r--r--   0        0        0      502 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/drop_duplicates_transformer.py
--rw-r--r--   0        0        0     2637 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_dead_and_inactive_artists_transformer.py
--rw-r--r--   0        0        0      891 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_inactive_users_transformer.py
--rw-r--r--   0        0        0     2323 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
--rw-r--r--   0        0        0      813 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_infrequent_transformer.py
--rw-r--r--   0        0        0     1492 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_matching_text_transformer.py
--rw-r--r--   0        0        0      706 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/flatten_struct_transformer.py
--rw-r--r--   0        0        0      684 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/join_transformer.py
--rw-r--r--   0        0        0      902 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/loggable_transformer.py
--rw-r--r--   0        0        0     1556 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
--rw-r--r--   0        0        0     1420 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/minmax_scaling_transformer.py
--rw-r--r--   0        0        0     1716 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/multiple_compound_mapping.py
--rw-r--r--   0        0        0      365 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/order_by_transformer.py
--rw-r--r--   0        0        0      868 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/participating_artist_transformer.py
--rw-r--r--   0        0        0     1043 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/pivot_transformer.py
--rw-r--r--   0        0        0     1300 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/playlist_coherence_transformer.py
--rw-r--r--   0        0        0      453 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/replace_null_values_transformer.py
--rw-r--r--   0        0        0      344 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/select_transformer.py
--rw-r--r--   0        0        0     4914 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
--rw-r--r--   0        0        0     2532 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/single_artist_filter_transformer.py
--rw-r--r--   0        0        0      705 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/single_dag_pipeline.py
--rw-r--r--   0        0        0     2721 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/stack_transformer.py
--rw-r--r--   0        0        0     1270 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/top_items_dithering_transformer.py
--rw-r--r--   0        0        0     1330 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/top_items_transformer.py
--rw-r--r--   0        0        0     1547 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
--rw-r--r--   0        0        0     1356 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_availability_transformer.py
--rw-r--r--   0        0        0     4458 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_filter_transformer.py
--rw-r--r--   0        0        0      378 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/union_transformer.py
--rw-r--r--   0        0        0     4235 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/user_blacklist_filter_transformer.py
--rw-r--r--   0        0        0        0 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/__init__.py
--rw-r--r--   0        0        0      545 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/class_utils.py
--rw-r--r--   0        0        0     7882 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/constants.py
--rw-r--r--   0        0        0     1917 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/dither_utils.py
--rw-r--r--   0        0        0      917 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/schemas.py
--rw-r--r--   0        0        0     1233 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/spark_utils.py
--rw-r--r--   0        0        0     1671 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/voiceness_filter_transformer.py
--rw-r--r--   0        0        0      803 2024-03-01 12:16:53.538932 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/where_transformer.py
--rw-r--r--   0        0        0      567 2024-03-01 12:16:53.542933 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
--rw-r--r--   0        0        0      539 2024-03-01 12:16:53.542933 tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/with_column_transfomer.py
--rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 tidal_per_transformers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/LICENSE
+-rw-r--r--   0        0        0      736 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/README.md
+-rw-r--r--   0        0        0     1080 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/__init__.py
+-rw-r--r--   0        0        0     2700 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/aggregate_transformer.py
+-rw-r--r--   0        0        0     2163 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artifact_id_mapping_by_user_country_transformer.py
+-rw-r--r--   0        0        0     2033 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artist_compound_transformer.py
+-rw-r--r--   0        0        0     3409 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artist_filter_transformer.py
+-rw-r--r--   0        0        0     2917 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
+-rw-r--r--   0        0        0      824 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
+-rw-r--r--   0        0        0     1031 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
+-rw-r--r--   0        0        0     1750 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/clean_text_transformer.py
+-rw-r--r--   0        0        0     1171 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
+-rw-r--r--   0        0        0     1887 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
+-rw-r--r--   0        0        0      912 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
+-rw-r--r--   0        0        0     1299 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/distinct_sequence_transformer.py
+-rw-r--r--   0        0        0      346 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/distinct_transformer.py
+-rw-r--r--   0        0        0     2845 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/diversity_sort_transformer.py
+-rw-r--r--   0        0        0      451 2024-04-05 08:00:37.721368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/drop_columns_transformer.py
+-rw-r--r--   0        0        0      502 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/drop_duplicates_transformer.py
+-rw-r--r--   0        0        0     2637 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_dead_and_inactive_artists_transformer.py
+-rw-r--r--   0        0        0      891 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_inactive_users_transformer.py
+-rw-r--r--   0        0        0     2323 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
+-rw-r--r--   0        0        0      813 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_infrequent_transformer.py
+-rw-r--r--   0        0        0     1492 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_matching_text_transformer.py
+-rw-r--r--   0        0        0      706 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/flatten_struct_transformer.py
+-rw-r--r--   0        0        0      684 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/join_transformer.py
+-rw-r--r--   0        0        0      902 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/loggable_transformer.py
+-rw-r--r--   0        0        0     1556 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
+-rw-r--r--   0        0        0     4374 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/master_bundle_filter_transformer.py
+-rw-r--r--   0        0        0     1420 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/minmax_scaling_transformer.py
+-rw-r--r--   0        0        0     1716 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/multiple_compound_mapping.py
+-rw-r--r--   0        0        0      365 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/order_by_transformer.py
+-rw-r--r--   0        0        0      868 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/participating_artist_transformer.py
+-rw-r--r--   0        0        0     1043 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/pivot_transformer.py
+-rw-r--r--   0        0        0     1300 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/playlist_coherence_transformer.py
+-rw-r--r--   0        0        0      453 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/replace_null_values_transformer.py
+-rw-r--r--   0        0        0      344 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/select_transformer.py
+-rw-r--r--   0        0        0     4914 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
+-rw-r--r--   0        0        0     2532 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/single_artist_filter_transformer.py
+-rw-r--r--   0        0        0      705 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/single_dag_pipeline.py
+-rw-r--r--   0        0        0     2721 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/stack_transformer.py
+-rw-r--r--   0        0        0     1270 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/top_items_dithering_transformer.py
+-rw-r--r--   0        0        0     1330 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/top_items_transformer.py
+-rw-r--r--   0        0        0     1547 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
+-rw-r--r--   0        0        0     1356 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_availability_transformer.py
+-rw-r--r--   0        0        0     4458 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_filter_transformer.py
+-rw-r--r--   0        0        0      378 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/union_transformer.py
+-rw-r--r--   0        0        0     4235 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/user_blacklist_filter_transformer.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/__init__.py
+-rw-r--r--   0        0        0      545 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/class_utils.py
+-rw-r--r--   0        0        0     7882 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/constants.py
+-rw-r--r--   0        0        0     1917 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/dither_utils.py
+-rw-r--r--   0        0        0      917 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/schemas.py
+-rw-r--r--   0        0        0     1233 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/spark_utils.py
+-rw-r--r--   0        0        0     1671 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/voiceness_filter_transformer.py
+-rw-r--r--   0        0        0      803 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/where_transformer.py
+-rw-r--r--   0        0        0      567 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
+-rw-r--r--   0        0        0      539 2024-04-05 08:00:37.725368 tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/with_column_transfomer.py
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 tidal_per_transformers-0.1.1/PKG-INFO
```

### Comparing `tidal_per_transformers-0.1.0/LICENSE` & `tidal_per_transformers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/README.md` & `tidal_per_transformers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/pyproject.toml` & `tidal_per_transformers-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/tidal-music/per-transformers"
 
 [tool.poetry]
 name = "tidal_per_transformers"
-version = "0.1.0"
+version = "0.1.1"
 description = "common transformers used by the tidal personalization team."
 authors = [
     "Loay <loay@squareup.com>",
     "Tao <tma@squareup.com>",
     "Thomas <talmenningen@squareup.com>",
 ]
```

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/__init__.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/aggregate_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/aggregate_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artifact_id_mapping_by_user_country_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artifact_id_mapping_by_user_country_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artist_compound_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artist_compound_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artist_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/artists_struct_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/artists_struct_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/clean_text_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/clean_text_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/collect_ranked_list_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/collect_ranked_list_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/collect_ranked_map_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/collect_ranked_map_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/distinct_sequence_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/distinct_sequence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/diversity_sort_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/diversity_sort_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_dead_and_inactive_artists_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_dead_and_inactive_artists_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_inactive_users_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_inactive_users_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_infrequent_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_infrequent_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/filter_matching_text_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/filter_matching_text_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/flatten_struct_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/flatten_struct_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/join_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/loggable_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/loggable_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/minmax_scaling_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/minmax_scaling_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/multiple_compound_mapping.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/multiple_compound_mapping.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/participating_artist_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/participating_artist_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/pivot_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/playlist_coherence_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/playlist_coherence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/sequence_content_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/sequence_content_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/single_artist_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/single_artist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/single_dag_pipeline.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/single_dag_pipeline.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/stack_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/stack_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/top_items_dithering_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/top_items_dithering_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/top_items_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/top_items_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_availability_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_availability_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/track_group_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/track_group_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/user_blacklist_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/user_blacklist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/class_utils.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/constants.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/dither_utils.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/dither_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/schemas.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/utils/spark_utils.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/voiceness_filter_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/voiceness_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/where_transformer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/where_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/with_column_renamed_transfomer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/with_column_renamed_transfomer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/tidal_per_transformers/transformers/with_column_transfomer.py` & `tidal_per_transformers-0.1.1/tidal_per_transformers/transformers/with_column_transfomer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.1.0/PKG-INFO` & `tidal_per_transformers-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal_per_transformers
-Version: 0.1.0
+Version: 0.1.1
 Summary: common transformers used by the tidal personalization team.
 License: Apache License V 2.0
 Author: Loay
 Author-email: loay@squareup.com
 Requires-Python: >=3.12.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

