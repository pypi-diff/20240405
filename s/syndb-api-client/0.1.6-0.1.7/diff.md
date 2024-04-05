# Comparing `tmp/syndb-api-client-0.1.6.tar.gz` & `tmp/syndb-api-client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndb-api-client-0.1.6.tar", last modified: Mon Mar 25 12:35:09 2024, max compression
+gzip compressed data, was "syndb-api-client-0.1.7.tar", last modified: Fri Apr  5 14:37:32 2024, max compression
```

## Comparing `syndb-api-client-0.1.6.tar` & `syndb-api-client-0.1.7.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.242818 syndb-api-client-0.1.6/
--rw-r--r--   0 can       (1000) can       (1000)      545 2024-03-25 12:35:09.242818 syndb-api-client-0.1.6/PKG-INFO
--rw-r--r--   0 can       (1000) can       (1000)    20289 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/README.md
--rw-r--r--   0 can       (1000) can       (1000)     1946 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/pyproject.toml
--rw-r--r--   0 can       (1000) can       (1000)       69 2024-03-25 12:35:09.242818 syndb-api-client-0.1.6/setup.cfg
--rw-r--r--   0 can       (1000) can       (1000)     1374 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/setup.py
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.228818 syndb-api-client-0.1.6/syndb_api_client/
--rw-r--r--   0 can       (1000) can       (1000)     4080 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/__init__.py
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.230818 syndb-api-client-0.1.6/syndb_api_client/api/
--rw-r--r--   0 can       (1000) can       (1000)      530 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/__init__.py
--rw-r--r--   0 can       (1000) can       (1000)    45509 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/auth_api.py
--rw-r--r--   0 can       (1000) can       (1000)    73828 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/dataset_api.py
--rw-r--r--   0 can       (1000) can       (1000)     9900 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/default_api.py
--rw-r--r--   0 can       (1000) can       (1000)    31853 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/external_api.py
--rw-r--r--   0 can       (1000) can       (1000)    43664 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/io_api.py
--rw-r--r--   0 can       (1000) can       (1000)   138780 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/metadata_api.py
--rw-r--r--   0 can       (1000) can       (1000)   181378 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/neurodata_api.py
--rw-r--r--   0 can       (1000) can       (1000)    55103 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/tag_api.py
--rw-r--r--   0 can       (1000) can       (1000)   139779 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api/user_api.py
--rw-r--r--   0 can       (1000) can       (1000)    25806 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api_client.py
--rw-r--r--   0 can       (1000) can       (1000)      652 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/api_response.py
--rw-r--r--   0 can       (1000) can       (1000)    14745 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/configuration.py
--rw-r--r--   0 can       (1000) can       (1000)     5975 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/exceptions.py
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.235818 syndb-api-client-0.1.6/syndb_api_client/models/
--rw-r--r--   0 can       (1000) can       (1000)     3036 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/models/__init__.py
--rw-r--r--   0 can       (1000) can       (1000)     5920 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/all_metadata_response.py
--rw-r--r--   0 can       (1000) can       (1000)     2871 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/animal_model_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     3098 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/animal_model_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     2596 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/bearer_response.py
--rw-r--r--   0 can       (1000) can       (1000)     2615 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/body_verify_request_token_user_request_verify_token_post.py
--rw-r--r--   0 can       (1000) can       (1000)     2543 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/body_verify_verify_user_verify_post.py
--rw-r--r--   0 can       (1000) can       (1000)     2890 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/brain_region_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     3279 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/brain_region_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)    15372 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/brain_structure.py
--rw-r--r--   0 can       (1000) can       (1000)     6735 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/create_dataset.py
--rw-r--r--   0 can       (1000) can       (1000)     3620 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/create_read_dataset_collection_model.py
--rw-r--r--   0 can       (1000) can       (1000)     3340 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/dataset_search_model.py
--rw-r--r--   0 can       (1000) can       (1000)     4907 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/detail.py
--rw-r--r--   0 can       (1000) can       (1000)     2721 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/error_model.py
--rw-r--r--   0 can       (1000) can       (1000)     8143 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/filter_dataset.py
--rw-r--r--   0 can       (1000) can       (1000)      898 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/gene_expression.py
--rw-r--r--   0 can       (1000) can       (1000)     2988 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/http_validation_error.py
--rw-r--r--   0 can       (1000) can       (1000)     2530 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/id2_label_response.py
--rw-r--r--   0 can       (1000) can       (1000)     2451 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/id_response.py
--rw-r--r--   0 can       (1000) can       (1000)     4844 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/location_inner.py
--rw-r--r--   0 can       (1000) can       (1000)     2499 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/microscopy_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     2491 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/microscopy_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     2756 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/mutation_model_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     3116 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/mutation_model_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1862 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/neuroanatomical_direction.py
--rw-r--r--   0 can       (1000) can       (1000)     2563 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/o_auth2_authorize_response.py
--rw-r--r--   0 can       (1000) can       (1000)     2589 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/pre_signed_s3_schema.py
--rw-r--r--   0 can       (1000) can       (1000)     2499 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/publication_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)      736 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/s3_instance.py
--rw-r--r--   0 can       (1000) can       (1000)     2729 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/s3_pre_signed_download_request.py
--rw-r--r--   0 can       (1000) can       (1000)      874 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/syndb_table.py
--rw-r--r--   0 can       (1000) can       (1000)     3572 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/user_create.py
--rw-r--r--   0 can       (1000) can       (1000)     3026 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/user_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     3085 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/user_profile.py
--rw-r--r--   0 can       (1000) can       (1000)     3047 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/syndb_api_client/models/validation_error.py
--rw-r--r--   0 can       (1000) can       (1000)        0 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/py.typed
--rw-r--r--   0 can       (1000) can       (1000)     9237 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/syndb_api_client/rest.py
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.242818 syndb-api-client-0.1.6/syndb_api_client.egg-info/
--rw-r--r--   0 can       (1000) can       (1000)      545 2024-03-25 12:35:09.000000 syndb-api-client-0.1.6/syndb_api_client.egg-info/PKG-INFO
--rw-r--r--   0 can       (1000) can       (1000)     3927 2024-03-25 12:35:09.000000 syndb-api-client-0.1.6/syndb_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 can       (1000) can       (1000)        1 2024-03-25 12:35:09.000000 syndb-api-client-0.1.6/syndb_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 can       (1000) can       (1000)       76 2024-03-25 12:35:09.000000 syndb-api-client-0.1.6/syndb_api_client.egg-info/requires.txt
--rw-r--r--   0 can       (1000) can       (1000)       17 2024-03-25 12:35:09.000000 syndb-api-client-0.1.6/syndb_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-03-25 12:35:09.241818 syndb-api-client-0.1.6/test/
--rw-r--r--   0 can       (1000) can       (1000)     2644 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_all_metadata_response.py
--rw-r--r--   0 can       (1000) can       (1000)     1575 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_animal_model_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1485 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_animal_model_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1520 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_auth_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1493 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_bearer_response.py
--rw-r--r--   0 can       (1000) can       (1000)     1828 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_body_verify_request_token_user_request_verify_token_post.py
--rw-r--r--   0 can       (1000) can       (1000)     1609 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_body_verify_verify_user_verify_post.py
--rw-r--r--   0 can       (1000) can       (1000)     1660 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_brain_region_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1611 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_brain_region_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)      716 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_brain_structure.py
--rw-r--r--   0 can       (1000) can       (1000)     3162 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_create_dataset.py
--rw-r--r--   0 can       (1000) can       (1000)     1825 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_create_read_dataset_collection_model.py
--rw-r--r--   0 can       (1000) can       (1000)     2445 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_dataset_api.py
--rw-r--r--   0 can       (1000) can       (1000)     6158 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_dataset_search_model.py
--rw-r--r--   0 can       (1000) can       (1000)      754 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_default_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1261 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_detail.py
--rw-r--r--   0 can       (1000) can       (1000)     1371 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_error_model.py
--rw-r--r--   0 can       (1000) can       (1000)     1225 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_external_api.py
--rw-r--r--   0 can       (1000) can       (1000)     2684 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_filter_dataset.py
--rw-r--r--   0 can       (1000) can       (1000)      716 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_gene_expression.py
--rw-r--r--   0 can       (1000) can       (1000)     1715 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_http_validation_error.py
--rw-r--r--   0 can       (1000) can       (1000)     1558 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_id2_label_response.py
--rw-r--r--   0 can       (1000) can       (1000)     1359 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_id_response.py
--rw-r--r--   0 can       (1000) can       (1000)     1424 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_io_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1346 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_location_inner.py
--rw-r--r--   0 can       (1000) can       (1000)     3839 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_metadata_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1484 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_microscopy_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1460 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_microscopy_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1630 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_mutation_model_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1581 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_mutation_model_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)      786 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_neuroanatomical_direction.py
--rw-r--r--   0 can       (1000) can       (1000)     4662 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_neurodata_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1547 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_o_auth2_authorize_response.py
--rw-r--r--   0 can       (1000) can       (1000)     1593 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_pre_signed_s3_schema.py
--rw-r--r--   0 can       (1000) can       (1000)     1494 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_publication_create_read.py
--rw-r--r--   0 can       (1000) can       (1000)      688 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_s3_instance.py
--rw-r--r--   0 can       (1000) can       (1000)     1850 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_s3_pre_signed_download_request.py
--rw-r--r--   0 can       (1000) can       (1000)      688 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_syndb_table.py
--rw-r--r--   0 can       (1000) can       (1000)     1766 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_tag_api.py
--rw-r--r--   0 can       (1000) can       (1000)     3422 2024-03-25 12:35:06.000000 syndb-api-client-0.1.6/test/test_user_api.py
--rw-r--r--   0 can       (1000) can       (1000)     1534 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_user_create.py
--rw-r--r--   0 can       (1000) can       (1000)     1547 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_user_just_read.py
--rw-r--r--   0 can       (1000) can       (1000)     1560 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_user_profile.py
--rw-r--r--   0 can       (1000) can       (1000)     1619 2024-03-25 12:35:05.000000 syndb-api-client-0.1.6/test/test_validation_error.py
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.566480 syndb-api-client-0.1.7/
+-rw-r--r--   0 can       (1000) can       (1000)      545 2024-04-05 14:37:32.566480 syndb-api-client-0.1.7/PKG-INFO
+-rw-r--r--   0 can       (1000) can       (1000)    19395 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/README.md
+-rw-r--r--   0 can       (1000) can       (1000)     1946 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/pyproject.toml
+-rw-r--r--   0 can       (1000) can       (1000)       69 2024-04-05 14:37:32.566480 syndb-api-client-0.1.7/setup.cfg
+-rw-r--r--   0 can       (1000) can       (1000)     1374 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/setup.py
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.558480 syndb-api-client-0.1.7/syndb_api_client/
+-rw-r--r--   0 can       (1000) can       (1000)     4080 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/__init__.py
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.560480 syndb-api-client-0.1.7/syndb_api_client/api/
+-rw-r--r--   0 can       (1000) can       (1000)      530 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/api/__init__.py
+-rw-r--r--   0 can       (1000) can       (1000)    45509 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/auth_api.py
+-rw-r--r--   0 can       (1000) can       (1000)    63104 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/dataset_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     9900 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/default_api.py
+-rw-r--r--   0 can       (1000) can       (1000)    34628 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/external_api.py
+-rw-r--r--   0 can       (1000) can       (1000)    47888 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/io_api.py
+-rw-r--r--   0 can       (1000) can       (1000)   128056 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/metadata_api.py
+-rw-r--r--   0 can       (1000) can       (1000)   174878 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/api/neurodata_api.py
+-rw-r--r--   0 can       (1000) can       (1000)    55103 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/api/tag_api.py
+-rw-r--r--   0 can       (1000) can       (1000)   139779 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/api/user_api.py
+-rw-r--r--   0 can       (1000) can       (1000)    25806 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/api_client.py
+-rw-r--r--   0 can       (1000) can       (1000)      652 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/api_response.py
+-rw-r--r--   0 can       (1000) can       (1000)    14745 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/configuration.py
+-rw-r--r--   0 can       (1000) can       (1000)     5975 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/exceptions.py
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.563480 syndb-api-client-0.1.7/syndb_api_client/models/
+-rw-r--r--   0 can       (1000) can       (1000)     3036 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/models/__init__.py
+-rw-r--r--   0 can       (1000) can       (1000)     5920 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/all_metadata_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     2871 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/animal_model_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     3098 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/animal_model_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     2596 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/bearer_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     2615 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/body_verify_request_token_user_request_verify_token_post.py
+-rw-r--r--   0 can       (1000) can       (1000)     2543 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/body_verify_verify_user_verify_post.py
+-rw-r--r--   0 can       (1000) can       (1000)     2890 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/brain_region_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     3279 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/brain_region_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)    15372 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/brain_structure.py
+-rw-r--r--   0 can       (1000) can       (1000)     6504 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/create_dataset.py
+-rw-r--r--   0 can       (1000) can       (1000)     3620 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/create_read_dataset_collection_model.py
+-rw-r--r--   0 can       (1000) can       (1000)     3340 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/dataset_search_model.py
+-rw-r--r--   0 can       (1000) can       (1000)     4907 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/detail.py
+-rw-r--r--   0 can       (1000) can       (1000)     2721 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/error_model.py
+-rw-r--r--   0 can       (1000) can       (1000)     8143 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/filter_dataset.py
+-rw-r--r--   0 can       (1000) can       (1000)      898 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/gene_expression.py
+-rw-r--r--   0 can       (1000) can       (1000)     2988 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/http_validation_error.py
+-rw-r--r--   0 can       (1000) can       (1000)     2530 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/id2_label_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     2451 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/id_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     4844 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/location_inner.py
+-rw-r--r--   0 can       (1000) can       (1000)     2499 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/microscopy_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     2491 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/microscopy_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     2756 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/mutation_model_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     3116 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/mutation_model_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1862 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/neuroanatomical_direction.py
+-rw-r--r--   0 can       (1000) can       (1000)     2563 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/o_auth2_authorize_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     2589 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/pre_signed_s3_schema.py
+-rw-r--r--   0 can       (1000) can       (1000)     2499 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/publication_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)      736 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/s3_instance.py
+-rw-r--r--   0 can       (1000) can       (1000)     2729 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/s3_pre_signed_download_request.py
+-rw-r--r--   0 can       (1000) can       (1000)      874 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/syndb_table.py
+-rw-r--r--   0 can       (1000) can       (1000)     3572 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/user_create.py
+-rw-r--r--   0 can       (1000) can       (1000)     3026 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/user_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     3085 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/user_profile.py
+-rw-r--r--   0 can       (1000) can       (1000)     3047 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/syndb_api_client/models/validation_error.py
+-rw-r--r--   0 can       (1000) can       (1000)        0 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/py.typed
+-rw-r--r--   0 can       (1000) can       (1000)     9237 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/syndb_api_client/rest.py
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.566480 syndb-api-client-0.1.7/syndb_api_client.egg-info/
+-rw-r--r--   0 can       (1000) can       (1000)      545 2024-04-05 14:37:32.000000 syndb-api-client-0.1.7/syndb_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 can       (1000) can       (1000)     3927 2024-04-05 14:37:32.000000 syndb-api-client-0.1.7/syndb_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 can       (1000) can       (1000)        1 2024-04-05 14:37:32.000000 syndb-api-client-0.1.7/syndb_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 can       (1000) can       (1000)       76 2024-04-05 14:37:32.000000 syndb-api-client-0.1.7/syndb_api_client.egg-info/requires.txt
+-rw-r--r--   0 can       (1000) can       (1000)       17 2024-04-05 14:37:32.000000 syndb-api-client-0.1.7/syndb_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 can       (1000) can       (1000)        0 2024-04-05 14:37:32.566480 syndb-api-client-0.1.7/test/
+-rw-r--r--   0 can       (1000) can       (1000)     2644 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_all_metadata_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     1575 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_animal_model_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1485 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_animal_model_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1520 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_auth_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1493 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_bearer_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     1828 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_body_verify_request_token_user_request_verify_token_post.py
+-rw-r--r--   0 can       (1000) can       (1000)     1609 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_body_verify_verify_user_verify_post.py
+-rw-r--r--   0 can       (1000) can       (1000)     1660 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_brain_region_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1611 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_brain_region_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)      716 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_brain_structure.py
+-rw-r--r--   0 can       (1000) can       (1000)     3162 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_create_dataset.py
+-rw-r--r--   0 can       (1000) can       (1000)     1825 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_create_read_dataset_collection_model.py
+-rw-r--r--   0 can       (1000) can       (1000)     2158 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_dataset_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     6158 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_dataset_search_model.py
+-rw-r--r--   0 can       (1000) can       (1000)      754 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_default_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1261 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_detail.py
+-rw-r--r--   0 can       (1000) can       (1000)     1371 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_error_model.py
+-rw-r--r--   0 can       (1000) can       (1000)     1225 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_external_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     2684 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_filter_dataset.py
+-rw-r--r--   0 can       (1000) can       (1000)      716 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_gene_expression.py
+-rw-r--r--   0 can       (1000) can       (1000)     1715 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_http_validation_error.py
+-rw-r--r--   0 can       (1000) can       (1000)     1558 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_id2_label_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     1359 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_id_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     1424 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_io_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1346 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_location_inner.py
+-rw-r--r--   0 can       (1000) can       (1000)     3552 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_metadata_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1484 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_microscopy_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1460 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_microscopy_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1630 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_mutation_model_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1581 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_mutation_model_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)      786 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_neuroanatomical_direction.py
+-rw-r--r--   0 can       (1000) can       (1000)     4375 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/test/test_neurodata_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1547 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_o_auth2_authorize_response.py
+-rw-r--r--   0 can       (1000) can       (1000)     1593 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_pre_signed_s3_schema.py
+-rw-r--r--   0 can       (1000) can       (1000)     1494 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_publication_create_read.py
+-rw-r--r--   0 can       (1000) can       (1000)      688 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_s3_instance.py
+-rw-r--r--   0 can       (1000) can       (1000)     1850 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_s3_pre_signed_download_request.py
+-rw-r--r--   0 can       (1000) can       (1000)      688 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_syndb_table.py
+-rw-r--r--   0 can       (1000) can       (1000)     1766 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/test/test_tag_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     3422 2024-04-05 14:37:31.000000 syndb-api-client-0.1.7/test/test_user_api.py
+-rw-r--r--   0 can       (1000) can       (1000)     1534 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_user_create.py
+-rw-r--r--   0 can       (1000) can       (1000)     1547 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_user_just_read.py
+-rw-r--r--   0 can       (1000) can       (1000)     1560 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_user_profile.py
+-rw-r--r--   0 can       (1000) can       (1000)     1619 2024-04-05 14:37:30.000000 syndb-api-client-0.1.7/test/test_validation_error.py
```

### Comparing `syndb-api-client-0.1.6/PKG-INFO` & `syndb-api-client-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndb-api-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Synapse DB
 Home-page: https://pypi.org/project/syndb-api-client
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Synapse DB
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `syndb-api-client-0.1.6/README.md` & `syndb-api-client-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # syndb-api-client
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.5
-- Package version: 0.1.6
+- Package version: 0.1.7
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -94,15 +94,14 @@
 *AuthApi* | [**auth_database_logout_user_auth_database_logout_post**](docs/AuthApi.md#auth_database_logout_user_auth_database_logout_post) | **POST** /user/auth/database/logout | Auth:Database.Logout
 *AuthApi* | [**oauth_oauth2_database_authorize_user_auth_orcid_authorize_get**](docs/AuthApi.md#oauth_oauth2_database_authorize_user_auth_orcid_authorize_get) | **GET** /user/auth/orcid/authorize | Oauth:Oauth2.Database.Authorize
 *AuthApi* | [**oauth_oauth2_database_callback_user_auth_orcid_callback_get**](docs/AuthApi.md#oauth_oauth2_database_callback_user_auth_orcid_callback_get) | **GET** /user/auth/orcid/callback | Oauth:Oauth2.Database.Callback
 *DatasetApi* | [**dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post**](docs/DatasetApi.md#dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post) | **POST** /neurodata/metadata/dataset/dataset_tag_search | Dataset Tag Search Endpoint
 *DatasetApi* | [**fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get**](docs/DatasetApi.md#fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get) | **GET** /neurodata/metadata/dataset/get_all | Fetch All Datasets Id2Label
 *DatasetApi* | [**fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get**](docs/DatasetApi.md#fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get) | **GET** /neurodata/metadata/dataset/modifiable | Fetch Modifiable Datasets
 *DatasetApi* | [**new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post**](docs/DatasetApi.md#new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post) | **POST** /neurodata/metadata/dataset/new_dataset_collection | New Dataset Collection
-*DatasetApi* | [**register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put**](docs/DatasetApi.md#register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put) | **PUT** /neurodata/metadata/dataset/upload_complete | Register Dataset Upload Completion
 *DatasetApi* | [**register_new_dataset_neurodata_metadata_dataset_new_dataset_post**](docs/DatasetApi.md#register_new_dataset_neurodata_metadata_dataset_new_dataset_post) | **POST** /neurodata/metadata/dataset/new_dataset | Register New Dataset
 *DatasetApi* | [**scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get**](docs/DatasetApi.md#scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get) | **GET** /neurodata/metadata/dataset/{scientist_tag} | Scientist Tag Datasets
 *DefaultApi* | [**redirect_get**](docs/DefaultApi.md#redirect_get) | **GET** / | Redirect
 *ExternalApi* | [**download_data_neurodata_io_download_get**](docs/ExternalApi.md#download_data_neurodata_io_download_get) | **GET** /neurodata/io/download | Download Data
 *ExternalApi* | [**upload_dataset_mesh_neurodata_io_upload_mesh_get**](docs/ExternalApi.md#upload_dataset_mesh_neurodata_io_upload_mesh_get) | **GET** /neurodata/io/upload/mesh | Upload Dataset Mesh
 *ExternalApi* | [**upload_dataset_swb_neurodata_io_upload_swb_get**](docs/ExternalApi.md#upload_dataset_swb_neurodata_io_upload_swb_get) | **GET** /neurodata/io/upload/swb | Upload Dataset Swb
 *IoApi* | [**download_data_neurodata_io_download_get**](docs/IoApi.md#download_data_neurodata_io_download_get) | **GET** /neurodata/io/download | Download Data
@@ -115,29 +114,27 @@
 *MetadataApi* | [**create_mutation_neurodata_metadata_tag_mutation_create_post**](docs/MetadataApi.md#create_mutation_neurodata_metadata_tag_mutation_create_post) | **POST** /neurodata/metadata/tag/mutation/create | Create Mutation
 *MetadataApi* | [**create_publication_neurodata_metadata_tag_publication_create_post**](docs/MetadataApi.md#create_publication_neurodata_metadata_tag_publication_create_post) | **POST** /neurodata/metadata/tag/publication/create | Create Publication
 *MetadataApi* | [**dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post**](docs/MetadataApi.md#dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post) | **POST** /neurodata/metadata/dataset/dataset_tag_search | Dataset Tag Search Endpoint
 *MetadataApi* | [**fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get**](docs/MetadataApi.md#fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get) | **GET** /neurodata/metadata/dataset/get_all | Fetch All Datasets Id2Label
 *MetadataApi* | [**fetch_all_metadata_endpoint_neurodata_metadata_get_all_get**](docs/MetadataApi.md#fetch_all_metadata_endpoint_neurodata_metadata_get_all_get) | **GET** /neurodata/metadata/get_all | Fetch All Metadata Endpoint
 *MetadataApi* | [**fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get**](docs/MetadataApi.md#fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get) | **GET** /neurodata/metadata/dataset/modifiable | Fetch Modifiable Datasets
 *MetadataApi* | [**new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post**](docs/MetadataApi.md#new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post) | **POST** /neurodata/metadata/dataset/new_dataset_collection | New Dataset Collection
-*MetadataApi* | [**register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put**](docs/MetadataApi.md#register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put) | **PUT** /neurodata/metadata/dataset/upload_complete | Register Dataset Upload Completion
 *MetadataApi* | [**register_new_dataset_neurodata_metadata_dataset_new_dataset_post**](docs/MetadataApi.md#register_new_dataset_neurodata_metadata_dataset_new_dataset_post) | **POST** /neurodata/metadata/dataset/new_dataset | Register New Dataset
 *MetadataApi* | [**scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get**](docs/MetadataApi.md#scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get) | **GET** /neurodata/metadata/dataset/{scientist_tag} | Scientist Tag Datasets
 *NeurodataApi* | [**create_animal_neurodata_metadata_tag_animal_create_post**](docs/NeurodataApi.md#create_animal_neurodata_metadata_tag_animal_create_post) | **POST** /neurodata/metadata/tag/animal/create | Create Animal
 *NeurodataApi* | [**create_brain_region_neurodata_metadata_tag_brain_region_create_post**](docs/NeurodataApi.md#create_brain_region_neurodata_metadata_tag_brain_region_create_post) | **POST** /neurodata/metadata/tag/brain_region/create | Create Brain Region
 *NeurodataApi* | [**create_microscopy_neurodata_metadata_tag_microscopy_create_post**](docs/NeurodataApi.md#create_microscopy_neurodata_metadata_tag_microscopy_create_post) | **POST** /neurodata/metadata/tag/microscopy/create | Create Microscopy
 *NeurodataApi* | [**create_mutation_neurodata_metadata_tag_mutation_create_post**](docs/NeurodataApi.md#create_mutation_neurodata_metadata_tag_mutation_create_post) | **POST** /neurodata/metadata/tag/mutation/create | Create Mutation
 *NeurodataApi* | [**create_publication_neurodata_metadata_tag_publication_create_post**](docs/NeurodataApi.md#create_publication_neurodata_metadata_tag_publication_create_post) | **POST** /neurodata/metadata/tag/publication/create | Create Publication
 *NeurodataApi* | [**dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post**](docs/NeurodataApi.md#dataset_tag_search_endpoint_neurodata_metadata_dataset_dataset_tag_search_post) | **POST** /neurodata/metadata/dataset/dataset_tag_search | Dataset Tag Search Endpoint
 *NeurodataApi* | [**download_data_neurodata_io_download_get**](docs/NeurodataApi.md#download_data_neurodata_io_download_get) | **GET** /neurodata/io/download | Download Data
 *NeurodataApi* | [**fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get**](docs/NeurodataApi.md#fetch_all_datasets_id2label_neurodata_metadata_dataset_get_all_get) | **GET** /neurodata/metadata/dataset/get_all | Fetch All Datasets Id2Label
 *NeurodataApi* | [**fetch_all_metadata_endpoint_neurodata_metadata_get_all_get**](docs/NeurodataApi.md#fetch_all_metadata_endpoint_neurodata_metadata_get_all_get) | **GET** /neurodata/metadata/get_all | Fetch All Metadata Endpoint
 *NeurodataApi* | [**fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get**](docs/NeurodataApi.md#fetch_modifiable_datasets_neurodata_metadata_dataset_modifiable_get) | **GET** /neurodata/metadata/dataset/modifiable | Fetch Modifiable Datasets
 *NeurodataApi* | [**new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post**](docs/NeurodataApi.md#new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post) | **POST** /neurodata/metadata/dataset/new_dataset_collection | New Dataset Collection
-*NeurodataApi* | [**register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put**](docs/NeurodataApi.md#register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put) | **PUT** /neurodata/metadata/dataset/upload_complete | Register Dataset Upload Completion
 *NeurodataApi* | [**register_new_dataset_neurodata_metadata_dataset_new_dataset_post**](docs/NeurodataApi.md#register_new_dataset_neurodata_metadata_dataset_new_dataset_post) | **POST** /neurodata/metadata/dataset/new_dataset | Register New Dataset
 *NeurodataApi* | [**scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get**](docs/NeurodataApi.md#scientist_tag_datasets_neurodata_metadata_dataset_scientist_tag_get) | **GET** /neurodata/metadata/dataset/{scientist_tag} | Scientist Tag Datasets
 *NeurodataApi* | [**upload_dataset_files_neurodata_io_upload_dataset_files_post**](docs/NeurodataApi.md#upload_dataset_files_neurodata_io_upload_dataset_files_post) | **POST** /neurodata/io/upload_dataset_files | Upload Dataset Files
 *NeurodataApi* | [**upload_dataset_mesh_neurodata_io_upload_mesh_get**](docs/NeurodataApi.md#upload_dataset_mesh_neurodata_io_upload_mesh_get) | **GET** /neurodata/io/upload/mesh | Upload Dataset Mesh
 *NeurodataApi* | [**upload_dataset_swb_neurodata_io_upload_swb_get**](docs/NeurodataApi.md#upload_dataset_swb_neurodata_io_upload_swb_get) | **GET** /neurodata/io/upload/swb | Upload Dataset Swb
 *TagApi* | [**create_animal_neurodata_metadata_tag_animal_create_post**](docs/TagApi.md#create_animal_neurodata_metadata_tag_animal_create_post) | **POST** /neurodata/metadata/tag/animal/create | Create Animal
 *TagApi* | [**create_brain_region_neurodata_metadata_tag_brain_region_create_post**](docs/TagApi.md#create_brain_region_neurodata_metadata_tag_brain_region_create_post) | **POST** /neurodata/metadata/tag/brain_region/create | Create Brain Region
```

### Comparing `syndb-api-client-0.1.6/pyproject.toml` & `syndb-api-client-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syndb-api-client"
-version = "0.1.6"
+version = "0.1.7"
 description = "Synapse DB"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Synapse DB"]
 include = ["syndb_api_client/py.typed"]
```

### Comparing `syndb-api-client-0.1.6/setup.py` & `syndb-api-client-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "syndb-api-client"
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/__init__.py` & `syndb-api-client-0.1.7/syndb_api_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.5
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 # import apis into sdk package
 from syndb_api_client.api.auth_api import AuthApi
 from syndb_api_client.api.dataset_api import DatasetApi
 from syndb_api_client.api.default_api import DefaultApi
 from syndb_api_client.api.external_api import ExternalApi
 from syndb_api_client.api.io_api import IoApi
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/__init__.py` & `syndb-api-client-0.1.7/syndb_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/auth_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/dataset_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/dataset_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictStr
 from syndb_api_client.models.create_dataset import CreateDataset
 from syndb_api_client.models.create_read_dataset_collection_model import CreateReadDatasetCollectionModel
 from syndb_api_client.models.dataset_search_model import DatasetSearchModel
 from syndb_api_client.models.id2_label_response import Id2LabelResponse
 from syndb_api_client.models.id_response import IdResponse
 
 from syndb_api_client.api_client import ApiClient, RequestSerialized
@@ -1049,290 +1049,14 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_with_http_info(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_without_preload_content(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-        self,
-        dataset_id,
-        upload_size,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
-        if upload_size is not None:
-            
-            _query_params.append(('upload_size', upload_size))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/neurodata/metadata/dataset/upload_complete',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/default_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/external_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/external_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import Field, StrictBool, StrictStr
+from typing_extensions import Annotated
 from syndb_api_client.models.pre_signed_s3_schema import PreSignedS3Schema
 from syndb_api_client.models.s3_pre_signed_download_request import S3PreSignedDownloadRequest
 
 from syndb_api_client.api_client import ApiClient, RequestSerialized
 from syndb_api_client.api_response import ApiResponse
 from syndb_api_client.rest import RESTResponseType
 
@@ -307,15 +308,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -324,16 +326,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -350,22 +354,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -374,15 +379,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -391,16 +397,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -417,22 +425,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -441,15 +450,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -458,16 +468,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -484,34 +496,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -523,19 +537,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -567,15 +581,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -584,16 +599,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -610,22 +627,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -634,15 +652,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -651,16 +670,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -677,22 +698,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -701,15 +723,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -718,16 +741,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -744,34 +769,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -783,19 +810,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/io_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/io_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBytes, StrictStr
-from typing import List, Union
+from pydantic import Field, StrictBool, StrictBytes, StrictStr
+from typing import Union
 from typing_extensions import Annotated
 from syndb_api_client.models.pre_signed_s3_schema import PreSignedS3Schema
 from syndb_api_client.models.s3_pre_signed_download_request import S3PreSignedDownloadRequest
 
 from syndb_api_client.api_client import ApiClient, RequestSerialized
 from syndb_api_client.api_response import ApiResponse
 from syndb_api_client.rest import RESTResponseType
@@ -309,16 +309,17 @@
 
 
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -326,20 +327,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> object:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -356,23 +359,27 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -381,16 +388,17 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post_with_http_info(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -398,20 +406,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[object]:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -428,23 +438,27 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -453,16 +467,17 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post_without_preload_content(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -470,20 +485,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -500,65 +517,69 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
         self,
         dataset_id,
-        neurodata_files,
+        append,
+        dataset_tar,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'neurodata_files': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
-        if neurodata_files is not None:
-            _files['neurodata_files'] = neurodata_files
+        if dataset_tar is not None:
+            _files['dataset_tar'] = dataset_tar
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
@@ -601,15 +622,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -618,16 +640,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -644,22 +668,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -668,15 +693,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -685,16 +711,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -711,22 +739,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -735,15 +764,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -752,16 +782,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -778,34 +810,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -817,19 +851,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -861,15 +895,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -878,16 +913,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -904,22 +941,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -928,15 +966,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -945,16 +984,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -971,22 +1012,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -995,15 +1037,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1012,16 +1055,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1038,34 +1083,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1077,19 +1124,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/metadata_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictStr
 from typing import Optional
 from syndb_api_client.models.all_metadata_response import AllMetadataResponse
 from syndb_api_client.models.animal_model_create_read import AnimalModelCreateRead
 from syndb_api_client.models.brain_region_create_read import BrainRegionCreateRead
 from syndb_api_client.models.create_dataset import CreateDataset
 from syndb_api_client.models.create_read_dataset_collection_model import CreateReadDatasetCollectionModel
 from syndb_api_client.models.dataset_search_model import DatasetSearchModel
@@ -2676,290 +2676,14 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_with_http_info(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_without_preload_content(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-        self,
-        dataset_id,
-        upload_size,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
-        if upload_size is not None:
-            
-            _query_params.append(('upload_size', upload_size))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/neurodata/metadata/dataset/upload_complete',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/neurodata_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/neurodata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from datetime import datetime
-from pydantic import Field, StrictBytes, StrictInt, StrictStr
-from typing import List, Optional, Union
+from pydantic import Field, StrictBool, StrictBytes, StrictStr
+from typing import Optional, Union
 from typing_extensions import Annotated
 from syndb_api_client.models.all_metadata_response import AllMetadataResponse
 from syndb_api_client.models.animal_model_create_read import AnimalModelCreateRead
 from syndb_api_client.models.brain_region_create_read import BrainRegionCreateRead
 from syndb_api_client.models.create_dataset import CreateDataset
 from syndb_api_client.models.create_read_dataset_collection_model import CreateReadDatasetCollectionModel
 from syndb_api_client.models.dataset_search_model import DatasetSearchModel
@@ -2958,290 +2958,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_with_http_info(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_without_preload_content(
-        self,
-        dataset_id: StrictStr,
-        upload_size: StrictInt,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Register Dataset Upload Completion
-
-
-        :param dataset_id: (required)
-        :type dataset_id: str
-        :param upload_size: (required)
-        :type upload_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-            dataset_id=dataset_id,
-            upload_size=upload_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
-            '422': "HTTPValidationError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put_serialize(
-        self,
-        dataset_id,
-        upload_size,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
-        if upload_size is not None:
-            
-            _query_params.append(('upload_size', upload_size))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-        ]
-
-        return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/neurodata/metadata/dataset/upload_complete',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def register_new_dataset_neurodata_metadata_dataset_new_dataset_post(
         self,
         create_dataset: CreateDataset,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -3767,16 +3491,17 @@
 
 
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3784,20 +3509,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> object:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3814,23 +3541,27 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -3839,16 +3570,17 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post_with_http_info(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3856,20 +3588,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[object]:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3886,23 +3620,27 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -3911,16 +3649,17 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_files_neurodata_io_upload_dataset_files_post_without_preload_content(
         self,
-        dataset_id: StrictStr,
-        neurodata_files: Annotated[List[Union[StrictBytes, StrictStr]], Field(description="Parquet files storing SynDB neurodata")],
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
+        dataset_tar: Annotated[Union[StrictBytes, StrictStr], Field(description="Tar archive storing dataset parquet files by SyndbTable")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -3928,20 +3667,22 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Files
 
-        SynDB neurodata imaging metrics data upload endpoint
+        Imaging metrics dataset upload endpoint
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
-        :param neurodata_files: Parquet files storing SynDB neurodata (required)
-        :type neurodata_files: List[bytearray]
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
+        :param dataset_tar: Tar archive storing dataset parquet files by SyndbTable (required)
+        :type dataset_tar: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3958,65 +3699,69 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
             dataset_id=dataset_id,
-            neurodata_files=neurodata_files,
+            append=append,
+            dataset_tar=dataset_tar,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '201': "object",
+            '406': None,
+            '415': None,
+            '500': None,
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_files_neurodata_io_upload_dataset_files_post_serialize(
         self,
         dataset_id,
-        neurodata_files,
+        append,
+        dataset_tar,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'neurodata_files': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
-        if neurodata_files is not None:
-            _files['neurodata_files'] = neurodata_files
+        if dataset_tar is not None:
+            _files['dataset_tar'] = dataset_tar
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
@@ -4059,15 +3804,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4076,16 +3822,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4102,22 +3850,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4126,15 +3875,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4143,16 +3893,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4169,22 +3921,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4193,15 +3946,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_mesh_neurodata_io_upload_mesh_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4210,16 +3964,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Mesh
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4236,34 +3992,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_mesh_neurodata_io_upload_mesh_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4275,19 +4033,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -4319,15 +4077,16 @@
 
 
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4336,16 +4095,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PreSignedS3Schema:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4362,22 +4123,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4386,15 +4148,16 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_with_http_info(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4403,16 +4166,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PreSignedS3Schema]:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4429,22 +4194,23 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -4453,15 +4219,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def upload_dataset_swb_neurodata_io_upload_swb_get_without_preload_content(
         self,
-        dataset_id: StrictStr,
+        dataset_id: Annotated[StrictStr, Field(description="The dataset id to upload the files to")],
+        append: Annotated[StrictBool, Field(description="Defines if the Dataset is being appended to or if it is expected to be the first upload")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -4470,16 +4237,18 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Upload Dataset Swb
 
 
-        :param dataset_id: (required)
+        :param dataset_id: The dataset id to upload the files to (required)
         :type dataset_id: str
+        :param append: Defines if the Dataset is being appended to or if it is expected to be the first upload (required)
+        :type append: bool
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4496,34 +4265,36 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
             dataset_id=dataset_id,
+            append=append,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "PreSignedS3Schema",
+            '200': "PreSignedS3Schema",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _upload_dataset_swb_neurodata_io_upload_swb_get_serialize(
         self,
         dataset_id,
+        append,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -4535,19 +4306,19 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if dataset_id is not None:
-            
-            _query_params.append(('dataset_id', dataset_id))
-            
+            _path_params['dataset_id'] = dataset_id
+        if append is not None:
+            _path_params['append'] = append
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/tag_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api/user_api.py` & `syndb-api-client-0.1.7/syndb_api_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api_client.py` & `syndb-api-client-0.1.7/syndb_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.6/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/api_response.py` & `syndb-api-client-0.1.7/syndb_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/configuration.py` & `syndb-api-client-0.1.7/syndb_api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.5\n"\
-               "SDK Package Version: 0.1.6".\
+               "SDK Package Version: 0.1.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/exceptions.py` & `syndb-api-client-0.1.7/syndb_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/__init__.py` & `syndb-api-client-0.1.7/syndb_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/all_metadata_response.py` & `syndb-api-client-0.1.7/syndb_api_client/models/all_metadata_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/animal_model_create_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/animal_model_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/animal_model_just_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/animal_model_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/bearer_response.py` & `syndb-api-client-0.1.7/syndb_api_client/models/bearer_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/body_verify_request_token_user_request_verify_token_post.py` & `syndb-api-client-0.1.7/syndb_api_client/models/body_verify_request_token_user_request_verify_token_post.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/body_verify_verify_user_verify_post.py` & `syndb-api-client-0.1.7/syndb_api_client/models/body_verify_verify_user_verify_post.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/brain_region_create_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/brain_region_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/brain_region_just_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/brain_region_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/brain_structure.py` & `syndb-api-client-0.1.7/syndb_api_client/models/brain_structure.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/create_dataset.py` & `syndb-api-client-0.1.7/syndb_api_client/models/create_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 class CreateDataset(BaseModel):
     """
     CreateDataset
     """ # noqa: E501
     authorized_group_names: Optional[List[StrictStr]] = None
     dataset_collection_names: Optional[List[StrictStr]] = None
-    syndb_tables: Optional[List[SyndbTable]] = None
     publication_dois: Optional[List[StrictStr]] = None
     id: Optional[StrictStr] = None
     label: Annotated[str, Field(strict=True, max_length=120)]
-    notes: Optional[StrictStr] = None
+    syndb_tables: Optional[List[SyndbTable]] = None
     animal: AnimalModelCreateRead
     mutations: Optional[List[MutationModelCreateRead]] = None
     brain_region: BrainRegionCreateRead
     microscopy: MicroscopyCreateRead
-    __properties: ClassVar[List[str]] = ["authorized_group_names", "dataset_collection_names", "syndb_tables", "publication_dois", "id", "label", "notes", "animal", "mutations", "brain_region", "microscopy"]
+    notes: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["authorized_group_names", "dataset_collection_names", "publication_dois", "id", "label", "syndb_tables", "animal", "mutations", "brain_region", "microscopy", "notes"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -106,54 +106,49 @@
             _dict['authorized_group_names'] = None
 
         # set to None if dataset_collection_names (nullable) is None
         # and model_fields_set contains the field
         if self.dataset_collection_names is None and "dataset_collection_names" in self.model_fields_set:
             _dict['dataset_collection_names'] = None
 
-        # set to None if syndb_tables (nullable) is None
-        # and model_fields_set contains the field
-        if self.syndb_tables is None and "syndb_tables" in self.model_fields_set:
-            _dict['syndb_tables'] = None
-
         # set to None if publication_dois (nullable) is None
         # and model_fields_set contains the field
         if self.publication_dois is None and "publication_dois" in self.model_fields_set:
             _dict['publication_dois'] = None
 
-        # set to None if notes (nullable) is None
-        # and model_fields_set contains the field
-        if self.notes is None and "notes" in self.model_fields_set:
-            _dict['notes'] = None
-
         # set to None if mutations (nullable) is None
         # and model_fields_set contains the field
         if self.mutations is None and "mutations" in self.model_fields_set:
             _dict['mutations'] = None
 
+        # set to None if notes (nullable) is None
+        # and model_fields_set contains the field
+        if self.notes is None and "notes" in self.model_fields_set:
+            _dict['notes'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateDataset from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "authorized_group_names": obj.get("authorized_group_names"),
             "dataset_collection_names": obj.get("dataset_collection_names"),
-            "syndb_tables": obj.get("syndb_tables"),
             "publication_dois": obj.get("publication_dois"),
             "id": obj.get("id"),
             "label": obj.get("label"),
-            "notes": obj.get("notes"),
+            "syndb_tables": obj.get("syndb_tables"),
             "animal": AnimalModelCreateRead.from_dict(obj["animal"]) if obj.get("animal") is not None else None,
             "mutations": [MutationModelCreateRead.from_dict(_item) for _item in obj["mutations"]] if obj.get("mutations") is not None else None,
             "brain_region": BrainRegionCreateRead.from_dict(obj["brain_region"]) if obj.get("brain_region") is not None else None,
-            "microscopy": MicroscopyCreateRead.from_dict(obj["microscopy"]) if obj.get("microscopy") is not None else None
+            "microscopy": MicroscopyCreateRead.from_dict(obj["microscopy"]) if obj.get("microscopy") is not None else None,
+            "notes": obj.get("notes")
         })
         return _obj
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/create_read_dataset_collection_model.py` & `syndb-api-client-0.1.7/syndb_api_client/models/create_read_dataset_collection_model.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/dataset_search_model.py` & `syndb-api-client-0.1.7/syndb_api_client/models/dataset_search_model.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/detail.py` & `syndb-api-client-0.1.7/syndb_api_client/models/detail.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/error_model.py` & `syndb-api-client-0.1.7/syndb_api_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/filter_dataset.py` & `syndb-api-client-0.1.7/syndb_api_client/models/filter_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 class FilterDataset(BaseModel):
     """
     FilterDataset
     """ # noqa: E501
     authorized_group_names: Optional[List[StrictStr]] = None
     dataset_collection_names: Optional[List[StrictStr]] = None
-    syndb_tables: Optional[List[SyndbTable]] = None
     publication_dois: Optional[List[StrictStr]] = None
     owner_id: Optional[List[StrictStr]] = None
+    syndb_tables: Optional[List[SyndbTable]] = None
     animal_species: Optional[List[StrictStr]] = None
     animal_cultural_names: Optional[List[StrictStr]] = None
     microscopy_names: Optional[List[StrictStr]] = None
     mutations: Optional[List[MutationModelJustRead]] = None
     brain_regions: Optional[List[BrainRegionJustRead]] = None
     microscopies: Optional[List[MicroscopyJustRead]] = None
-    __properties: ClassVar[List[str]] = ["authorized_group_names", "dataset_collection_names", "syndb_tables", "publication_dois", "owner_id", "animal_species", "animal_cultural_names", "microscopy_names", "mutations", "brain_regions", "microscopies"]
+    __properties: ClassVar[List[str]] = ["authorized_group_names", "dataset_collection_names", "publication_dois", "owner_id", "syndb_tables", "animal_species", "animal_cultural_names", "microscopy_names", "mutations", "brain_regions", "microscopies"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -109,29 +109,29 @@
             _dict['authorized_group_names'] = None
 
         # set to None if dataset_collection_names (nullable) is None
         # and model_fields_set contains the field
         if self.dataset_collection_names is None and "dataset_collection_names" in self.model_fields_set:
             _dict['dataset_collection_names'] = None
 
-        # set to None if syndb_tables (nullable) is None
-        # and model_fields_set contains the field
-        if self.syndb_tables is None and "syndb_tables" in self.model_fields_set:
-            _dict['syndb_tables'] = None
-
         # set to None if publication_dois (nullable) is None
         # and model_fields_set contains the field
         if self.publication_dois is None and "publication_dois" in self.model_fields_set:
             _dict['publication_dois'] = None
 
         # set to None if owner_id (nullable) is None
         # and model_fields_set contains the field
         if self.owner_id is None and "owner_id" in self.model_fields_set:
             _dict['owner_id'] = None
 
+        # set to None if syndb_tables (nullable) is None
+        # and model_fields_set contains the field
+        if self.syndb_tables is None and "syndb_tables" in self.model_fields_set:
+            _dict['syndb_tables'] = None
+
         # set to None if animal_species (nullable) is None
         # and model_fields_set contains the field
         if self.animal_species is None and "animal_species" in self.model_fields_set:
             _dict['animal_species'] = None
 
         # set to None if animal_cultural_names (nullable) is None
         # and model_fields_set contains the field
@@ -168,17 +168,17 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "authorized_group_names": obj.get("authorized_group_names"),
             "dataset_collection_names": obj.get("dataset_collection_names"),
-            "syndb_tables": obj.get("syndb_tables"),
             "publication_dois": obj.get("publication_dois"),
             "owner_id": obj.get("owner_id"),
+            "syndb_tables": obj.get("syndb_tables"),
             "animal_species": obj.get("animal_species"),
             "animal_cultural_names": obj.get("animal_cultural_names"),
             "microscopy_names": obj.get("microscopy_names"),
             "mutations": [MutationModelJustRead.from_dict(_item) for _item in obj["mutations"]] if obj.get("mutations") is not None else None,
             "brain_regions": [BrainRegionJustRead.from_dict(_item) for _item in obj["brain_regions"]] if obj.get("brain_regions") is not None else None,
             "microscopies": [MicroscopyJustRead.from_dict(_item) for _item in obj["microscopies"]] if obj.get("microscopies") is not None else None
         })
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/gene_expression.py` & `syndb-api-client-0.1.7/syndb_api_client/models/gene_expression.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/http_validation_error.py` & `syndb-api-client-0.1.7/syndb_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/id2_label_response.py` & `syndb-api-client-0.1.7/syndb_api_client/models/id2_label_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/id_response.py` & `syndb-api-client-0.1.7/syndb_api_client/models/id_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/location_inner.py` & `syndb-api-client-0.1.7/syndb_api_client/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/microscopy_create_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/microscopy_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/microscopy_just_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/microscopy_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/mutation_model_create_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/mutation_model_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/mutation_model_just_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/mutation_model_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/neuroanatomical_direction.py` & `syndb-api-client-0.1.7/syndb_api_client/models/neuroanatomical_direction.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/o_auth2_authorize_response.py` & `syndb-api-client-0.1.7/syndb_api_client/models/o_auth2_authorize_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/pre_signed_s3_schema.py` & `syndb-api-client-0.1.7/syndb_api_client/models/pre_signed_s3_schema.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/publication_create_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/publication_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/s3_instance.py` & `syndb-api-client-0.1.7/syndb_api_client/models/s3_instance.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/s3_pre_signed_download_request.py` & `syndb-api-client-0.1.7/syndb_api_client/models/s3_pre_signed_download_request.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/syndb_table.py` & `syndb-api-client-0.1.7/syndb_api_client/models/syndb_table.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/user_create.py` & `syndb-api-client-0.1.7/syndb_api_client/models/user_create.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/user_just_read.py` & `syndb-api-client-0.1.7/syndb_api_client/models/user_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/user_profile.py` & `syndb-api-client-0.1.7/syndb_api_client/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/models/validation_error.py` & `syndb-api-client-0.1.7/syndb_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client/rest.py` & `syndb-api-client-0.1.7/syndb_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/syndb_api_client.egg-info/PKG-INFO` & `syndb-api-client-0.1.7/syndb_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndb-api-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Synapse DB
 Home-page: https://pypi.org/project/syndb-api-client
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,Synapse DB
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `syndb-api-client-0.1.6/syndb_api_client.egg-info/SOURCES.txt` & `syndb-api-client-0.1.7/syndb_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_all_metadata_response.py` & `syndb-api-client-0.1.7/test/test_all_metadata_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_animal_model_create_read.py` & `syndb-api-client-0.1.7/test/test_animal_model_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_animal_model_just_read.py` & `syndb-api-client-0.1.7/test/test_animal_model_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_auth_api.py` & `syndb-api-client-0.1.7/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_bearer_response.py` & `syndb-api-client-0.1.7/test/test_bearer_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_body_verify_request_token_user_request_verify_token_post.py` & `syndb-api-client-0.1.7/test/test_body_verify_request_token_user_request_verify_token_post.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_body_verify_verify_user_verify_post.py` & `syndb-api-client-0.1.7/test/test_body_verify_verify_user_verify_post.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_brain_region_create_read.py` & `syndb-api-client-0.1.7/test/test_brain_region_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_brain_region_just_read.py` & `syndb-api-client-0.1.7/test/test_brain_region_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_brain_structure.py` & `syndb-api-client-0.1.7/test/test_brain_structure.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_create_dataset.py` & `syndb-api-client-0.1.7/test/test_create_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,38 +37,38 @@
             return CreateDataset(
                 authorized_group_names = [
                     ''
                     ],
                 dataset_collection_names = [
                     ''
                     ],
-                syndb_tables = [
-                    1
-                    ],
                 publication_dois = [
                     ''
                     ],
                 id = '',
                 label = '',
-                notes = '',
+                syndb_tables = [
+                    1
+                    ],
                 animal = syndb_api_client.models.animal_model_create_read.AnimalModelCreateRead(
                     species = '', 
                     cultural_name = '', ),
                 mutations = [
                     syndb_api_client.models.mutation_model_create_read.MutationModelCreateRead(
                         id = '', 
                         gene = '', 
                         expression = 'knock-out', )
                     ],
                 brain_region = syndb_api_client.models.brain_region_create_read.BrainRegionCreateRead(
                     id = '', 
                     brain_structure = 'amygdaloid complex', 
                     direction = 'anterior', ),
                 microscopy = syndb_api_client.models.microscopy_create_read.MicroscopyCreateRead(
-                    name = '', )
+                    name = '', ),
+                notes = ''
             )
         else:
             return CreateDataset(
                 label = '',
                 animal = syndb_api_client.models.animal_model_create_read.AnimalModelCreateRead(
                     species = '', 
                     cultural_name = '', ),
```

### Comparing `syndb-api-client-0.1.6/test/test_create_read_dataset_collection_model.py` & `syndb-api-client-0.1.7/test/test_create_read_dataset_collection_model.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_dataset_api.py` & `syndb-api-client-0.1.7/test/test_dataset_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,21 +50,14 @@
     def test_new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post(self) -> None:
         """Test case for new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post
 
         New Dataset Collection
         """
         pass
 
-    def test_register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(self) -> None:
-        """Test case for register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put
-
-        Register Dataset Upload Completion
-        """
-        pass
-
     def test_register_new_dataset_neurodata_metadata_dataset_new_dataset_post(self) -> None:
         """Test case for register_new_dataset_neurodata_metadata_dataset_new_dataset_post
 
         Register New Dataset
         """
         pass
```

### Comparing `syndb-api-client-0.1.6/test/test_dataset_search_model.py` & `syndb-api-client-0.1.7/test/test_dataset_search_model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,23 +38,23 @@
                 include = syndb_api_client.models.filter_dataset.FilterDataset(
                     authorized_group_names = [
                         ''
                         ], 
                     dataset_collection_names = [
                         ''
                         ], 
-                    syndb_tables = [
-                        1
-                        ], 
                     publication_dois = [
                         ''
                         ], 
                     owner_id = [
                         ''
                         ], 
+                    syndb_tables = [
+                        1
+                        ], 
                     animal_species = [
                         ''
                         ], 
                     animal_cultural_names = [
                         ''
                         ], 
                     microscopy_names = [
@@ -77,23 +77,23 @@
                 exclude = syndb_api_client.models.filter_dataset.FilterDataset(
                     authorized_group_names = [
                         ''
                         ], 
                     dataset_collection_names = [
                         ''
                         ], 
-                    syndb_tables = [
-                        1
-                        ], 
                     publication_dois = [
                         ''
                         ], 
                     owner_id = [
                         ''
                         ], 
+                    syndb_tables = [
+                        1
+                        ], 
                     animal_species = [
                         ''
                         ], 
                     animal_cultural_names = [
                         ''
                         ], 
                     microscopy_names = [
@@ -119,23 +119,23 @@
                 include = syndb_api_client.models.filter_dataset.FilterDataset(
                     authorized_group_names = [
                         ''
                         ], 
                     dataset_collection_names = [
                         ''
                         ], 
-                    syndb_tables = [
-                        1
-                        ], 
                     publication_dois = [
                         ''
                         ], 
                     owner_id = [
                         ''
                         ], 
+                    syndb_tables = [
+                        1
+                        ], 
                     animal_species = [
                         ''
                         ], 
                     animal_cultural_names = [
                         ''
                         ], 
                     microscopy_names = [
```

### Comparing `syndb-api-client-0.1.6/test/test_default_api.py` & `syndb-api-client-0.1.7/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_detail.py` & `syndb-api-client-0.1.7/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_error_model.py` & `syndb-api-client-0.1.7/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_external_api.py` & `syndb-api-client-0.1.7/test/test_external_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_filter_dataset.py` & `syndb-api-client-0.1.7/test/test_filter_dataset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,23 +37,23 @@
             return FilterDataset(
                 authorized_group_names = [
                     ''
                     ],
                 dataset_collection_names = [
                     ''
                     ],
-                syndb_tables = [
-                    1
-                    ],
                 publication_dois = [
                     ''
                     ],
                 owner_id = [
                     ''
                     ],
+                syndb_tables = [
+                    1
+                    ],
                 animal_species = [
                     ''
                     ],
                 animal_cultural_names = [
                     ''
                     ],
                 microscopy_names = [
```

### Comparing `syndb-api-client-0.1.6/test/test_gene_expression.py` & `syndb-api-client-0.1.7/test/test_gene_expression.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_http_validation_error.py` & `syndb-api-client-0.1.7/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_id2_label_response.py` & `syndb-api-client-0.1.7/test/test_id2_label_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_id_response.py` & `syndb-api-client-0.1.7/test/test_id_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_io_api.py` & `syndb-api-client-0.1.7/test/test_io_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_location_inner.py` & `syndb-api-client-0.1.7/test/test_location_inner.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_metadata_api.py` & `syndb-api-client-0.1.7/test/test_metadata_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,21 +92,14 @@
     def test_new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post(self) -> None:
         """Test case for new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post
 
         New Dataset Collection
         """
         pass
 
-    def test_register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(self) -> None:
-        """Test case for register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put
-
-        Register Dataset Upload Completion
-        """
-        pass
-
     def test_register_new_dataset_neurodata_metadata_dataset_new_dataset_post(self) -> None:
         """Test case for register_new_dataset_neurodata_metadata_dataset_new_dataset_post
 
         Register New Dataset
         """
         pass
```

### Comparing `syndb-api-client-0.1.6/test/test_microscopy_create_read.py` & `syndb-api-client-0.1.7/test/test_microscopy_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_microscopy_just_read.py` & `syndb-api-client-0.1.7/test/test_microscopy_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_mutation_model_create_read.py` & `syndb-api-client-0.1.7/test/test_mutation_model_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_mutation_model_just_read.py` & `syndb-api-client-0.1.7/test/test_mutation_model_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_neuroanatomical_direction.py` & `syndb-api-client-0.1.7/test/test_neuroanatomical_direction.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_neurodata_api.py` & `syndb-api-client-0.1.7/test/test_neurodata_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,21 +99,14 @@
     def test_new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post(self) -> None:
         """Test case for new_dataset_collection_neurodata_metadata_dataset_new_dataset_collection_post
 
         New Dataset Collection
         """
         pass
 
-    def test_register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put(self) -> None:
-        """Test case for register_dataset_upload_completion_neurodata_metadata_dataset_upload_complete_put
-
-        Register Dataset Upload Completion
-        """
-        pass
-
     def test_register_new_dataset_neurodata_metadata_dataset_new_dataset_post(self) -> None:
         """Test case for register_new_dataset_neurodata_metadata_dataset_new_dataset_post
 
         Register New Dataset
         """
         pass
```

### Comparing `syndb-api-client-0.1.6/test/test_o_auth2_authorize_response.py` & `syndb-api-client-0.1.7/test/test_o_auth2_authorize_response.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_pre_signed_s3_schema.py` & `syndb-api-client-0.1.7/test/test_pre_signed_s3_schema.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_publication_create_read.py` & `syndb-api-client-0.1.7/test/test_publication_create_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_s3_instance.py` & `syndb-api-client-0.1.7/test/test_s3_instance.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_s3_pre_signed_download_request.py` & `syndb-api-client-0.1.7/test/test_s3_pre_signed_download_request.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_syndb_table.py` & `syndb-api-client-0.1.7/test/test_syndb_table.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_tag_api.py` & `syndb-api-client-0.1.7/test/test_tag_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_user_api.py` & `syndb-api-client-0.1.7/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_user_create.py` & `syndb-api-client-0.1.7/test/test_user_create.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_user_just_read.py` & `syndb-api-client-0.1.7/test/test_user_just_read.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_user_profile.py` & `syndb-api-client-0.1.7/test/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `syndb-api-client-0.1.6/test/test_validation_error.py` & `syndb-api-client-0.1.7/test/test_validation_error.py`

 * *Files identical despite different names*

