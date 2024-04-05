# Comparing `tmp/dvcx-0.72.0.tar.gz` & `tmp/dvcx-0.72.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.72.0.tar", last modified: Tue Apr  2 04:20:17 2024, max compression
+gzip compressed data, was "dvcx-0.72.1.tar", last modified: Fri Apr  5 05:50:53 2024, max compression
```

## Comparing `dvcx-0.72.0.tar` & `dvcx-0.72.1.tar`

### file list

```diff
@@ -1,225 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.378401 dvcx-0.72.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 04:20:12.000000 dvcx-0.72.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 04:20:12.000000 dvcx-0.72.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.338401 dvcx-0.72.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.338401 dvcx-0.72.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 04:20:12.000000 dvcx-0.72.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-02 04:20:12.000000 dvcx-0.72.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 04:20:12.000000 dvcx-0.72.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 04:20:12.000000 dvcx-0.72.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 04:20:12.000000 dvcx-0.72.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-02 04:20:12.000000 dvcx-0.72.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-02 04:20:12.000000 dvcx-0.72.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-02 04:20:12.000000 dvcx-0.72.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-02 04:20:17.378401 dvcx-0.72.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-02 04:20:12.000000 dvcx-0.72.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.342401 dvcx-0.72.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-02 04:20:12.000000 dvcx-0.72.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.346401 dvcx-0.72.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 04:20:12.000000 dvcx-0.72.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-02 04:20:12.000000 dvcx-0.72.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-02 04:20:12.000000 dvcx-0.72.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:20:17.378401 dvcx-0.72.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.334401 dvcx-0.72.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.350401 dvcx-0.72.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.354401 dvcx-0.72.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69026 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    28953 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.354401 dvcx-0.72.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.358401 dvcx-0.72.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33325 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    53799 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.362401 dvcx-0.72.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-02 04:20:12.000000 dvcx-0.72.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 04:20:17.000000 dvcx-0.72.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.366401 dvcx-0.72.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.370401 dvcx-0.72.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34568 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:20:17.374401 dvcx-0.72.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-02 04:20:12.000000 dvcx-0.72.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.426752 dvcx-0.72.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 05:50:46.000000 dvcx-0.72.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 05:50:46.000000 dvcx-0.72.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-05 05:50:46.000000 dvcx-0.72.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-05 05:50:46.000000 dvcx-0.72.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-05 05:50:46.000000 dvcx-0.72.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-05 05:50:46.000000 dvcx-0.72.1/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 05:50:46.000000 dvcx-0.72.1/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-05 05:50:46.000000 dvcx-0.72.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-05 05:50:46.000000 dvcx-0.72.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-05 05:50:46.000000 dvcx-0.72.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-05 05:50:46.000000 dvcx-0.72.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 05:50:46.000000 dvcx-0.72.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-05 05:50:46.000000 dvcx-0.72.1/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-05 05:50:53.426752 dvcx-0.72.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-05 05:50:46.000000 dvcx-0.72.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.386752 dvcx-0.72.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-05 05:50:46.000000 dvcx-0.72.1/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.390752 dvcx-0.72.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.390752 dvcx-0.72.1/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.394752 dvcx-0.72.1/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.394752 dvcx-0.72.1/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 05:50:46.000000 dvcx-0.72.1/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-05 05:50:46.000000 dvcx-0.72.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-05 05:50:46.000000 dvcx-0.72.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 05:50:53.426752 dvcx-0.72.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.378752 dvcx-0.72.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.398752 dvcx-0.72.1/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.398752 dvcx-0.72.1/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70434 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30412 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.402752 dvcx-0.72.1/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.402752 dvcx-0.72.1/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44476 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30540 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33325 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.406752 dvcx-0.72.1/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54623 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.410752 dvcx-0.72.1/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-05 05:50:46.000000 dvcx-0.72.1/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.422752 dvcx-0.72.1/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 05:50:53.000000 dvcx-0.72.1/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.414752 dvcx-0.72.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.414752 dvcx-0.72.1/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.414752 dvcx-0.72.1/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34571 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109607 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.418752 dvcx-0.72.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.422752 dvcx-0.72.1/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.422752 dvcx-0.72.1/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 05:50:53.422752 dvcx-0.72.1/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-05 05:50:46.000000 dvcx-0.72.1/tests/utils.py
```

### Comparing `dvcx-0.72.0/.cruft.json` & `dvcx-0.72.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.72.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.72.1/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.github/workflows/benchmarks.yml` & `dvcx-0.72.1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.github/workflows/release.yml` & `dvcx-0.72.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.github/workflows/tests.yml` & `dvcx-0.72.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.gitignore` & `dvcx-0.72.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/.pre-commit-config.yaml` & `dvcx-0.72.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/CODE_OF_CONDUCT.rst` & `dvcx-0.72.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/CONTRIBUTING.rst` & `dvcx-0.72.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/LICENSE` & `dvcx-0.72.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/LICENSES/Apache-2.0.txt` & `dvcx-0.72.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.72.1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/LICENSES/Python-2.0.txt` & `dvcx-0.72.1/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/PKG-INFO` & `dvcx-0.72.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.72.0
+Version: 0.72.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +14,15 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
 Requires-Dist: tqdm
+Requires-Dist: pandas
 Requires-Dist: python-dateutil>=2
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
@@ -88,15 +89,15 @@
    :alt: Python Version
 .. |License| image:: https://img.shields.io/pypi/l/dvcx
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License
 .. |Tests| image:: https://github.com/iterative/dvcx/workflows/Tests/badge.svg
    :target: https://github.com/iterative/dvcx/actions?workflow=Tests
    :alt: Tests
-.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg?token=VSCP2T9R5X
    :target: https://app.codecov.io/gh/iterative/dvcx
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

### Comparing `dvcx-0.72.0/README.rst` & `dvcx-0.72.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :alt: Python Version
 .. |License| image:: https://img.shields.io/pypi/l/dvcx
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License
 .. |Tests| image:: https://github.com/iterative/dvcx/workflows/Tests/badge.svg
    :target: https://github.com/iterative/dvcx/actions?workflow=Tests
    :alt: Tests
-.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg?token=VSCP2T9R5X
    :target: https://app.codecov.io/gh/iterative/dvcx
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

### Comparing `dvcx-0.72.0/docs/udfs.md` & `dvcx-0.72.1/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/blip2_image_desc_lib.py` & `dvcx-0.72.1/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/common_sql_functions.py` & `dvcx-0.72.1/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/dir_expansion.py` & `dvcx-0.72.1/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/hf_pipeline.py` & `dvcx-0.72.1/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/llava2_image_desc_lib.py` & `dvcx-0.72.1/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/loader.py` & `dvcx-0.72.1/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/neurips/README` & `dvcx-0.72.1/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/neurips/distance_to_query.py` & `dvcx-0.72.1/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/neurips/llm_chat.py` & `dvcx-0.72.1/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/neurips/single_query.py` & `dvcx-0.72.1/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/neurips/text_loaders.py` & `dvcx-0.72.1/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/openai_image_desc_lib.py` & `dvcx-0.72.1/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/openimage-detect.py` & `dvcx-0.72.1/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/pose_detection.py` & `dvcx-0.72.1/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/torch-loader.py` & `dvcx-0.72.1/examples/torch-loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 from torch import nn, optim
 from torch.utils.data import DataLoader
 from torchvision.transforms import v2
 
 from dvcx.lib.param import Image, Label
-from dvcx.lib.pytorch import DvcxDataset
+from dvcx.lib.pytorch import PytorchDataset
 from dvcx.query import C, DatasetQuery, udf
 from dvcx.sql.types import String
 
 STORAGE = "gcs://dvcx-datalakes/dogs-and-cats/"
 
 # Define transformation for data preprocessing
 transform = v2.Compose(
@@ -54,15 +54,15 @@
         DatasetQuery(STORAGE)
         .filter(C.name.glob("*.jpg"))
         .add_signals(extract_label)
         .save("cats-and-dogs")
     )
 
     train_loader = DataLoader(
-        DvcxDataset(
+        PytorchDataset(
             params=[Image(), Label("label", CLASSES)],
             name="cats-and-dogs",
             cache=True,
             transform=transform,
         ),
         batch_size=16,
     )
```

### Comparing `dvcx-0.72.0/examples/udfs/batching.py` & `dvcx-0.72.1/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/udfs/image_transformation.py` & `dvcx-0.72.1/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/udfs/parallel.py` & `dvcx-0.72.1/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/udfs/simple.py` & `dvcx-0.72.1/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/udfs/stateful.py` & `dvcx-0.72.1/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/udfs/stateful_similarity.py` & `dvcx-0.72.1/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/unstructured-text.py` & `dvcx-0.72.1/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/wds.py` & `dvcx-0.72.1/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/wds_filtered.py` & `dvcx-0.72.1/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/wds_meta.py` & `dvcx-0.72.1/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/zalando/zalando_clip.py` & `dvcx-0.72.1/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.72.1/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/noxfile.py` & `dvcx-0.72.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/pyproject.toml` & `dvcx-0.72.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ]
 requires-python = ">=3.9"
 dynamic = ["version"]
 dependencies = [
   "pyyaml",
   "tomlkit",
   "tqdm",
+  "pandas",
   "python-dateutil>=2",
   "attrs>=21.3.0",
   "s3fs>=2024.2.0",
   "gcsfs>=2024.2.0",
   "adlfs>=2024.2.0",
   "dvc-data>=3.10,<4",
   "dvc-objects>=4,<6",
```

### Comparing `dvcx-0.72.0/src/dvcx/asyn.py` & `dvcx-0.72.1/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/cache.py` & `dvcx-0.72.1/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/catalog/catalog.py` & `dvcx-0.72.1/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import ast
 import functools
 import io
+import json
 import logging
 import math
 import os
 import os.path
 import posixpath
 import subprocess
 import sys
 import time
 import traceback
 from ast import Attribute, Call, Expr, Import, Load, Name, alias
 from collections.abc import Iterable, Iterator, Mapping, Sequence
+from copy import copy
 from dataclasses import dataclass
 from pathlib import Path
 from random import shuffle
 from typing import (
     TYPE_CHECKING,
     Any,
+    NamedTuple,
     NoReturn,
     Optional,
     Union,
 )
 from uuid import uuid4
 
 import requests
@@ -106,14 +109,21 @@
 PULL_DATASET_CHECK_STATUS_INTERVAL = 20  # interval to check export status in Studio
 
 
 def _raise_remote_error(error_message: str) -> NoReturn:
     raise DVCXError(f"Error from server: {error_message}")
 
 
+class QueryResult(NamedTuple):
+    dataset: Optional[DatasetRecord]
+    version: Optional[int]
+    output: str
+    preview: Optional[list[dict]]
+
+
 class DatasetRowsFetcher(NodesThreadPool):
     def __init__(
         self,
         metastore: "AbstractMetastore",
         warehouse: "AbstractWarehouse",
         remote_config: dict[str, Any],
         dataset_name: str,
@@ -553,14 +563,22 @@
 
     def get_init_params(self) -> dict[str, Any]:
         return {
             **self._init_params,
             "client_config": self.client_config,
         }
 
+    def copy(self, cache=True, db=True):
+        result = copy(self)
+        if not db:
+            result.id_generator = None
+            result.metastore = None
+            result.warehouse = None
+        return result
+
     @classmethod
     def generate_query_dataset_name(cls) -> str:
         return f"{QUERY_DATASET_NAME_PREFIX}_{uuid4().hex}"
 
     def compile_query_script(self, script: str, save=False) -> str:
         wrapper_function = "query_wrapper_print"
         if save:
@@ -1686,21 +1704,24 @@
             ds = DatasetQuery(path=source, catalog=self)
         udf = import_object(udf_location)
         if params:
             args, kwargs = parse_params_string(params)
             udf = udf(*args, **kwargs)
         ds.add_signals(udf, parallel=parallel).save(target_name)
 
-    def query(
+    def query(  # noqa: PLR0912
         self,
         query_script: str,
         envs: Optional[Mapping[str, str]] = None,
         python_executable: Optional[str] = None,
         save: bool = False,
-    ) -> tuple[Optional[DatasetRecord], Optional[int], str]:
+        preview_limit: Optional[int] = 10,
+        preview_offset: int = 0,
+        preview_columns: Optional[list[str]] = None,
+    ) -> QueryResult:
         """
         Method to run custom user Python script to run a query and, as result,
         creates new dataset from the results of a query.
         Returns tuple of result dataset and script output.
 
         Constraints on query script:
             1. dvcx.query.DatasetQuery should be used in order to create query
@@ -1728,32 +1749,52 @@
             raise QueryScriptCompileError(
                 f"Query script failed to compile, reason: {exc}"
             ) from exc
 
         if not python_executable:
             python_executable = sys.executable
 
+        envs = dict(envs)
+        envs.update(
+            {
+                "DVCX_QUERY_PREVIEW_ARGS": json.dumps(
+                    {
+                        "limit": preview_limit,
+                        "offset": preview_offset,
+                        "columns": preview_columns,
+                    }
+                )
+            }
+        )
         result = subprocess.run(
             [python_executable, "-c", query_script_compiled],  # noqa: S603
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,  # merging stderr to stdout
             env=envs,
             check=False,
         )
 
         script_output = ""  # stdout + stderr from user script itself
 
         # finding returning dataset name and version from script
         dataset_name = None
         dataset_version = None
+        records = None
         if result.stdout:
             for line in result.stdout.decode("utf-8").splitlines():
                 if len(line.split(PYTHON_SCRIPT_WRAPPER_CODE)) == 4:
                     dataset_name = line.split(PYTHON_SCRIPT_WRAPPER_CODE)[1]
                     dataset_version = int(line.split(PYTHON_SCRIPT_WRAPPER_CODE)[2])
+                elif (
+                    not records
+                    and line.startswith("__ds_records__")
+                    and line.endswith("__ds_records__")
+                ):
+                    _, record, _ = line.split("__ds_records__", 2)
+                    records = json.loads(record.strip())
                 else:
                     # collecting script output as well to save it to the database
                     # later on for debugging
                     script_output += line + "\n"
 
         if result.returncode:
             if result.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
@@ -1771,15 +1812,17 @@
             raise QueryScriptRunError(
                 f"Query script exited with error code {result.returncode}",
                 return_code=result.returncode,
                 output=script_output,
             )
 
         if not save:
-            return None, None, script_output
+            return QueryResult(
+                dataset=None, version=None, output=script_output, preview=records
+            )
 
         # finding returning dataset
         returned_dataset = None
         returned_dataset_version = None
         if dataset_name and dataset_version:
             try:
                 returned_dataset = self.get_dataset(dataset_name)
@@ -1795,15 +1838,20 @@
 
         returned_dataset = self.update_dataset(
             returned_dataset,
             script_output=script_output,
             query_script=query_script,
         )
 
-        return returned_dataset, dataset_version, script_output
+        return QueryResult(
+            dataset=returned_dataset,
+            version=dataset_version,
+            output=script_output,
+            preview=records,
+        )
 
     def cp(
         self,
         sources: list[str],
         output: str,
         force: bool = False,
         update: bool = False,
```

### Comparing `dvcx-0.72.0/src/dvcx/catalog/datasource.py` & `dvcx-0.72.1/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/catalog/formats.py` & `dvcx-0.72.1/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/catalog/loader.py` & `dvcx-0.72.1/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/cli.py` & `dvcx-0.72.1/src/dvcx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from itertools import chain
 from multiprocessing import freeze_support
 from typing import TYPE_CHECKING, Optional, Union
 
 import shtab
 
 from dvcx import __version__, utils
-from dvcx.cli_utils import BooleanOptionalAction
+from dvcx.cli_utils import BooleanOptionalAction, CommaSeparatedArgs
+from dvcx.error import QueryScriptRunError
 from dvcx.utils import DVCXDir
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
 
 logger = logging.getLogger("dvcx")
 
@@ -471,14 +472,40 @@
         default=None,
         metavar="N",
         help=(
             "Use multiprocessing to run any query script UDFs with N worker processes. "
             "N defaults to the CPU count."
         ),
     )
+    query_parser.add_argument(
+        "--limit",
+        action="store",
+        default=10,
+        type=int,
+        help="Number of rows to show",
+    )
+    query_parser.add_argument(
+        "--offset",
+        action="store",
+        default=0,
+        type=int,
+        help="Number of rows to offset",
+    )
+    query_parser.add_argument(
+        "--columns",
+        default=[],
+        action=CommaSeparatedArgs,
+        help="Columns to show",
+    )
+    query_parser.add_argument(
+        "--no-collapse",
+        action="store_true",
+        default=False,
+        help="Do not collapse the columns",
+    )
 
     apply_udf_parser = subp.add_parser(
         "apply-udf", parents=[parent_parser], help="Apply UDF"
     )
     apply_udf_parser.add_argument("udf", type=str, help="UDF location")
     apply_udf_parser.add_argument("source", type=str, help="Source storage or dataset")
     apply_udf_parser.add_argument("target", type=str, help="Target dataset name")
@@ -766,22 +793,44 @@
 
 
 def query(
     catalog: "Catalog",
     script: str,
     dataset_name: str,
     parallel: Optional[int] = None,
+    limit: int = 10,
+    offset: int = 0,
+    columns: Optional[list[str]] = None,
+    no_collapse: bool = False,
+    show_error: bool = False,
 ) -> None:
+    from dvcx.utils import show_records
+
     with open(script, encoding="utf-8") as f:
         script_content = f.read()
+
     if parallel is not None:
         # This also sets this environment variable for any subprocesses
         os.environ["DVCX_SETTINGS_PARALLEL"] = str(parallel)
-    _, _, script_output = catalog.query(script_content)
-    print(script_output)
+
+    try:
+        result = catalog.query(
+            script_content,
+            preview_limit=limit,
+            preview_offset=offset,
+            preview_columns=columns,
+        )
+    except QueryScriptRunError as e:
+        if show_error:
+            print(e.output, end="")
+        raise
+
+    if result.output:
+        print(result.output)
+    show_records(result.preview, collapse_columns=not no_collapse)
 
 
 def clear_cache(catalog: "Catalog"):
     catalog.cache.clear()
 
 
 def completion(shell: str) -> str:
@@ -941,15 +990,24 @@
         elif args.command == "add-storage":
             catalog.add_storage(args.uri)
         elif args.command == "completion":
             print(completion(args.shell))
         elif args.command == "find-stale-storages":
             catalog.find_stale_storages()
         elif args.command == "query":
-            query(catalog, args.script, args.parallel)
+            query(
+                catalog,
+                args.script,
+                args.parallel,
+                limit=args.limit,
+                offset=args.offset,
+                columns=args.columns,
+                no_collapse=args.no_collapse,
+                show_error=args.verbose,
+            )
         elif args.command == "apply-udf":
             catalog.apply_udf(
                 args.udf, args.source, args.target, args.parallel, args.udf_params
             )
         elif args.command == "clear-cache":
             clear_cache(catalog)
         else:
```

### Comparing `dvcx-0.72.0/src/dvcx/cli_utils.py` & `dvcx-0.72.1/src/dvcx/cli_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argparse import SUPPRESS, Action
+from argparse import SUPPRESS, Action, _AppendAction
 
 
 class BooleanOptionalAction(Action):
     """
     Creates --[no-]option style bool options.
 
     Defined here since it doesn't exist in argparse in Python 3.8.
@@ -47,7 +47,14 @@
 
     def __call__(self, parser, namespace, values, option_string=None):
         if option_string in self.option_strings:
             setattr(namespace, self.dest, not option_string.startswith("--no-"))
 
     def format_usage(self):
         return " | ".join(self.option_strings)
+
+
+class CommaSeparatedArgs(_AppendAction):  # pylint: disable=protected-access
+    def __call__(self, parser, namespace, values, option_string=None):  # noqa: ARG002
+        items = getattr(namespace, self.dest) or []
+        items.extend(v for value in values.split(",") if (v := value.strip()))
+        setattr(namespace, self.dest, list(dict.fromkeys(items)))
```

### Comparing `dvcx-0.72.0/src/dvcx/client/azure.py` & `dvcx-0.72.1/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/client/fileslice.py` & `dvcx-0.72.1/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/client/fsspec.py` & `dvcx-0.72.1/src/dvcx/client/fsspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         if url.lower().startswith(ClientS3.PREFIX):
             return ClientS3
         elif url.lower().startswith(GCSClient.PREFIX):
             return GCSClient
         elif url.lower().startswith(AzureClient.PREFIX):
             return AzureClient
-        elif url.lower().startswith(FileClient.PREFIX):
+        elif url.lower().startswith(FileClient.PREFIX) or url == "":
             return FileClient
         raise RuntimeError(f"Unsupported data source format '{url}'")
 
     @staticmethod
     def parse_url(
         source: str,
         metastore: "AbstractMetastore",
```

### Comparing `dvcx-0.72.0/src/dvcx/client/gcs.py` & `dvcx-0.72.1/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/client/local.py` & `dvcx-0.72.1/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/client/s3.py` & `dvcx-0.72.1/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/config.py` & `dvcx-0.72.1/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.72.1/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.72.1/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.72.1/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/schema.py` & `dvcx-0.72.1/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.72.1/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.72.1/src/dvcx/data_storage/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import re
 import sqlite3
 from collections.abc import Iterable, Sequence
 from contextlib import contextmanager
 from functools import wraps
 from time import sleep
 from typing import (
     TYPE_CHECKING,
@@ -517,21 +516,14 @@
         db_file: Optional[str] = None,
     ):
         self.schema: "DefaultSchema" = DefaultSchema()
         super().__init__(id_generator, uri, partial_id)
 
         self.db = db or SQLiteDatabaseEngine.from_db_file(db_file)
 
-        self.listing_table_pattern = re.compile(
-            f"^{self.BUCKET_TABLE_NAME_PREFIX}[a-z0-9-._]+_[0-9]+$"
-        )
-        self._reflect_tables(
-            filter_tables=lambda t, _: bool(self.listing_table_pattern.match(t))
-        )
-
     def clone(
         self, uri: StorageURI = StorageURI(""), partial_id: Optional[int] = None
     ) -> "SQLiteWarehouse":
         if not uri:
             if partial_id is not None:
                 raise ValueError("if partial_id is used, uri cannot be empty")
             if self.uri:
```

### Comparing `dvcx-0.72.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.72.1/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/dataset.py` & `dvcx-0.72.1/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/error.py` & `dvcx-0.72.1/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/dataset.py` & `dvcx-0.72.1/src/dvcx/lib/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from collections.abc import Sequence
-from typing import Callable, Optional, Union
+from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import sqlalchemy
 from sqlalchemy.sql.elements import ColumnElement
 
 from dvcx.lib.feature import Feature, FeatureClass
 from dvcx.lib.udf import (
     Aggregator,
@@ -13,14 +13,17 @@
     GroupMapper,
     Mapper,
     UDFBase,
 )
 from dvcx.query.dataset import DatasetQuery, JoinPredicateType, PartitionByType, detach
 from dvcx.query.schema import Column
 
+if TYPE_CHECKING:
+    from typing_extensions import Self
+
 C = Column
 
 
 class Dataset(DatasetQuery):
     """DVCX DataFrame is a 2-dimensional table of rows and columns designed to work
     with AI datasets - datasets of unstructured data such as images, video audio, text,
     etc.
@@ -78,21 +81,20 @@
         Example:
         >>> df.map(lambda name: name[:-4] + ".json", output={"json_file": String}) \
         >>>     .save("new_dataset")
         """
 
         self._validate_args("map()", parallel, workers, min_task_size)
 
-        udf_obj = self._udf_to_obj(udf, Mapper, "map()", params, output)
+        udf_obj = self._udf_to_obj(udf, Mapper, "map()", params, output, cache=cache)
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
-            cache=cache,
         )
 
     def generate(  # type: ignore[override]
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -115,22 +117,23 @@
            columns and newly generated ones, not just the new columns.
 
         The function returns a nested list, where each inner list represents a set of
         column values (the same as `map()`).
         """
         self._validate_args("generate()", parallel, workers, min_task_size)
 
-        udf_obj = self._udf_to_obj(udf, Generator, "generate()", params, output)
+        udf_obj = self._udf_to_obj(
+            udf, Generator, "generate()", params, output, cache=cache
+        )
         return DatasetQuery.generate(
             self,
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
-            cache=cache,
         )
 
     def aggregate(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -152,24 +155,23 @@
            column names that determine the grouping criteria for aggregation.
         2. Group-based UDF function input: Instead of individual rows, the function
            receives a list all rows within each group defined by `partition_by`.
         """
         self._validate_args("aggregate()", parallel, workers, min_task_size)
 
         udf_obj = self._udf_to_obj(
-            udf, Aggregator, "aggregate()", params, output, batch
+            udf, Aggregator, "aggregate()", params, output, batch, cache=cache
         )
         return DatasetQuery.generate(
             self,
             udf_obj.to_udf_wrapper(),
             partition_by=partition_by,
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
-            cache=cache,
         )
 
     def batch_map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -185,22 +187,21 @@
         `batch` (int), which sets the batch size. The default batch size is 1000.
 
         Input-output relationship: N:N
         """
         self._validate_args("map()", parallel, workers, min_task_size)
 
         udf_obj = self._udf_to_obj(
-            udf, BatchMapper, "batch_map()", params, output, batch
+            udf, BatchMapper, "batch_map()", params, output, batch, cache=cache
         )
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
-            cache=cache,
         )
 
     def group_map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -227,32 +228,27 @@
            values, the function returns nested list of the new columns. Each sub-list
            of the columns should correspond to input row in a given order.
         """
         self._validate_args(
             "group_map()", parallel, workers, min_task_size, partition_by
         )
 
-        udf_obj = self._udf_to_obj(udf, GroupMapper, "group_map()", params, output)
+        udf_obj = self._udf_to_obj(
+            udf, GroupMapper, "group_map()", params, output, cache=cache
+        )
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
             partition_by=partition_by,
-            cache=cache,
         )
 
     def _udf_to_obj(
-        self,
-        udf,
-        target_class,
-        name,
-        params=None,
-        output=None,
-        batch=1,
+        self, udf, target_class, name, params=None, output=None, batch=1, cache=False
     ):
         if isinstance(udf, UDFBase):
             if not isinstance(udf, target_class):
                 cls_name = target_class.__name__
                 raise TypeError(
                     f"{name}: expected an instance derived from {cls_name}"
                     f", but received {udf.name}"
@@ -261,14 +257,21 @@
                 raise ValueError(
                     f"params for BaseUDF class {udf.name} cannot be overwritten"
                 )
             if output:
                 raise ValueError(
                     f"output for BaseUDF class {udf.name} cannot be overwritten"
                 )
+
+            if isinstance(udf, UDFBase):
+                udf.set_catalog(self.catalog)
+
+                if cache:
+                    udf.enable_caching()
+
             return udf
 
         if inspect.isfunction(udf):
             return target_class.create_from_func(udf, params, output, batch)
 
         if isinstance(udf, type):
             raise TypeError(
@@ -334,30 +337,30 @@
         super_func = getattr(super(), method_name)
 
         columns = self._args_to_columns(*args)
         res = super_func(self, *columns)
         return res
 
     @detach
-    def select(self, *args) -> "Dataset":
+    def select(self, *args, **kwargs) -> "Self":
         return self._extend_features("select", *args)
 
     @detach
-    def select_except(self, *args) -> "Dataset":
+    def select_except(self, *args) -> "Self":
         return self._extend_features("select_except", *args)
 
     @detach
     def merge(
         self,
         right_ds: "Dataset",
         on: Union[JoinPredicateType, Sequence[JoinPredicateType]],
-        right_on: Union[JoinPredicateType, Sequence[JoinPredicateType]] = None,
+        right_on: Union[JoinPredicateType, Sequence[JoinPredicateType], None] = None,
         inner=False,
         rname="{name}_right",
-    ) -> "Dataset":
+    ) -> "Self":
         if on is None:
             raise ValueError("'on' must be specified in merge()")
 
         on = [on] if not isinstance(on, (list, tuple)) else on
         on_columns = [cols for item in on for cols in self._args_to_columns(item)]
 
         if right_on is not None:
```

### Comparing `dvcx-0.72.0/src/dvcx/lib/feature.py` & `dvcx-0.72.1/src/dvcx/lib/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,21 +244,7 @@
 
     new_prefix_value = cls._delimiter.join([prefix, norm_name])
     return FeatureAttributeWrapper(anno, new_prefix_value)
 
 
 class ShallowFeature(Feature):
     _expand_name: ClassVar[bool] = False
-
-
-class FileFeature(ShallowFeature):
-    _is_file = True
-
-    def __init__(self, **kwarg):
-        super().__init__(**kwarg)
-        self._stream = None
-
-    def set_file(self, stream):
-        self._stream = stream
-
-    def open(self):
-        return self._stream
```

### Comparing `dvcx-0.72.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.72.1/src/dvcx/lib/feature_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import sys
 import traceback
 from collections.abc import Sequence
 from typing import Optional, Union
 
-from dvcx.catalog import get_catalog
 from dvcx.lib.feature import Feature, FeatureClass, FeatureClassSeq
 from dvcx.lib.udf import Aggregator, BatchMapper, Generator, Mapper, UDFBase
 from dvcx.lib.utils import DvcxError
 from dvcx.query import Stream
 
 
 class ValidationError(DvcxError):
@@ -44,15 +43,15 @@
 
     @property
     def has_stream(self):
         return self._has_stream
 
     @property
     def cache(self):
-        return self._cache
+        return self._udf.catalog.cache
 
     def __init__(
         self,
         udf: UDFBase,
         inputs: Union[FeatureClass, FeatureClassSeq] = (),
         outputs: Union[FeatureClass, FeatureClassSeq] = (),
     ):
@@ -64,15 +63,14 @@
         self._validate_schema("params", self._inputs)
         self._validate_schema("output", self._outputs)
 
         self._has_stream = any(
             f._is_file  # type: ignore[attr-defined]
             for f in self._inputs
         )
-        self._cache = get_catalog().cache
 
         udf_params_spec = Feature._features_to_udf_spec(self._inputs)
         stream_prm = [Stream()] if self._has_stream else []
         self._udf_params_list = stream_prm + list(udf_params_spec.keys())
 
         self._udf_output_spec = Feature._features_to_udf_spec(self._outputs)  # type: ignore[attr-defined]
 
@@ -91,16 +89,16 @@
             streams = [arg[0] for arg in args]
             args = [arg[1:] for arg in args]
 
         obj_rows = [self._params_to_objects(params, arg) for arg in args]
         for row, stream in zip(obj_rows, streams):
             for feature in row:
                 if feature._is_file:
-                    feature.set_file(stream)
-                    feature.set_cache(self._cache)
+                    feature.set_catalog(self._udf.catalog)
+                    feature.set_file(stream, self._udf.caching_enabled)
 
         return obj_rows
 
     def _params_to_objects(self, params, args):
         new_params = params if not self._has_stream else params[1:]
         return [cls._unflatten(dict(zip(new_params, args))) for cls in self._inputs]
```

### Comparing `dvcx-0.72.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.72.1/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.72.1/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.72.1/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/image_transform.py` & `dvcx-0.72.1/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.72.1/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/param.py` & `dvcx-0.72.1/src/dvcx/lib/param.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/pytorch.py` & `dvcx-0.72.1/src/dvcx/lib/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,48 +11,48 @@
 if TYPE_CHECKING:
     from dvcx.query.schema import UDFParamSpec
 
 
 logger = logging.getLogger("dvcx")
 
 
-class DvcxDataset(IterableDataset):
+class PytorchDataset(IterableDataset):
     def __init__(
         self,
         params: "UDFParamSpec",
         name: str,
         version: Optional[int] = None,
         transform: Any = None,
-        async_workers: int = ASYNC_WORKERS,
+        workers: int = ASYNC_WORKERS,
         cache: bool = False,
     ):
         """
         Pytorch IterableDataset that streams DVCx datasets.
 
         Args:
             params (UDFParamSpec): Fields from DVCx dataset to stream.
             name (str): Name of DVCx dataset to stream.
             version (int): Version of DVCx dataset to stream.
             transform (Any): Pytorch v2 transforms to apply to the dataset.
-            async_workers (int): Number of async workers per process.
+            workers (int): Number of async workers per process.
             cache (bool): Whether to download and cache objects locally.
         """
         self.params = params
         self.name = name
         self.version = version
         self.transform = transform
-        self.async_workers = async_workers
+        self.workers = workers
         self.cache = cache
 
     def __iter__(self):
         total_rank, total_workers = self.get_rank_and_workers()
         q = DatasetQuery(name=self.name, version=self.version).chunk(
             total_rank, total_workers
         )
-        stream = q.extract(*self.params, workers=self.async_workers, cache=self.cache)
+        stream = q.extract(*self.params, workers=self.workers, cache=self.cache)
         for row in stream:
             # Auto convert types
             row = self.image_to_tensor(row)
             # Apply transforms
             if self.transform:
                 row = self.transform(row)
             yield row
```

### Comparing `dvcx-0.72.0/src/dvcx/lib/udf.py` & `dvcx-0.72.1/src/dvcx/lib/udf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import types
 from abc import ABC
 from typing import Callable
 
+from dvcx.catalog import get_catalog
 from dvcx.query import udf
 from dvcx.query.schema import DatasetRow
 from dvcx.sql.types import Int, String
 
 
 class UDFBase(ABC):
     DEF_OUTPUT_NAME = "result"
@@ -14,14 +15,16 @@
 
     def __init__(self, params=None, output=None, batch=1):
         sign_params, sign_output = self._get_signature(self.process)
 
         self._params = params or sign_params
         self._output = output or sign_output
         self._batch = batch
+        self._caching_enabled = False
+        self._catalog = get_catalog().copy(db=False)
 
     @property
     def params(self):
         return self._params
 
     @property
     def output(self):
@@ -31,14 +34,28 @@
     def batch(self):
         return self._batch
 
     @property
     def name(self):
         return self.__class__.__name__
 
+    @property
+    def caching_enabled(self):
+        return self._caching_enabled
+
+    def enable_caching(self):
+        self._caching_enabled = True
+
+    def set_catalog(self, catalog):
+        self._catalog = catalog.copy(db=False)
+
+    @property
+    def catalog(self):
+        return self._catalog
+
     def to_udf_wrapper(self):
         udf_wrapper = udf(params=self.params, output=self.output, batch=self.batch)
         return udf_wrapper(self)
 
     def setup(self):  # noqa: B027
         """Initialization process executed on each worker before processing begins.
         This is needed for tasks like pre-loading ML models prior to scoring.
```

### Comparing `dvcx-0.72.0/src/dvcx/lib/unstructured.py` & `dvcx-0.72.1/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/utils.py` & `dvcx-0.72.1/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/webdataset.py` & `dvcx-0.72.1/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.72.1/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.72.1/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/listing.py` & `dvcx-0.72.1/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/node.py` & `dvcx-0.72.1/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.72.1/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.72.1/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/progress.py` & `dvcx-0.72.1/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/query/batch.py` & `dvcx-0.72.1/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/query/builtins.py` & `dvcx-0.72.1/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/query/dataset.py` & `dvcx-0.72.1/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,49 +51,57 @@
 from dvcx.utils import chunk, determine_processes
 
 from .schema import C, UDFParamSpec, normalize_param
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
     from sqlalchemy.sql.schema import Table
-    from sqlalchemy.sql.selectable import SelectBase
+    from sqlalchemy.sql.selectable import GenerativeSelect, SelectBase
+    from typing_extensions import Concatenate, ParamSpec, Self
 
     from dvcx.catalog import Catalog
     from dvcx.data_storage import AbstractWarehouse
     from dvcx.dataset import DatasetRecord
 
     from .udf import UDFResult
 
+    P = ParamSpec("P")
+
 
 INSERT_BATCH_SIZE = 10000
 
 PartitionByType = Union[ColumnElement, Sequence[ColumnElement]]
 JoinPredicateType = Union[str, ColumnClause, ColumnElement]
 S = TypeVar("S", bound="SelectBase")
 # dependency can be either dataset_name + dataset_version tuple or just storage uri
 # depending what type of dependency we are adding
 DatasetDependencyType = Union[tuple[str, int], StorageURI]
 
 logger = logging.getLogger("dvcx")
 
 
-def detach(method: Callable):
+T = TypeVar("T", bound="DatasetQuery")
+
+
+def detach(
+    method: "Callable[Concatenate[T, P], T]",
+) -> "Callable[Concatenate[T, P], T]":
     """
     Decorator that needs to be put on a method that modifies existing DatasetQuery
     which was 100% representing one particular dataset and had name and version of
     that dataset set, and which returns new instance of it.
     This kind of DatasetQuery, which represent one whole dataset, we return from
     .save() method.
     Example of modifying method is .filter() as that one filters out part
     of a dataset which means DatasetQuery no longer 100% represents it (in this case
     it can represents only a part of it)
     """
 
     @wraps(method)
-    def _inner(self, *args, **kwargs) -> "DatasetQuery":
+    def _inner(self: T, *args: "P.args", **kwargs: "P.kwargs") -> T:
         cloned = method(self, *args, **kwargs)
         cloned.name = None
         cloned.version = None
         return cloned
 
     return _inner
 
@@ -781,14 +789,22 @@
     n: int
 
     def apply_sql_clause(self, query):
         return query.limit(self.n)
 
 
 @frozen
+class SQLOffset(SQLClause):
+    offset: int
+
+    def apply_sql_clause(self, query: "GenerativeSelect"):
+        return query.offset(self.offset)
+
+
+@frozen
 class SQLCount(SQLClause):
     def apply_sql_clause(self, query):
         return sqlalchemy.select(f.count(1)).select_from(query.subquery())
 
 
 @frozen
 class SQLUnion(Step):
@@ -1168,23 +1184,23 @@
     def show(self, limit=20) -> None:
         df = self.limit(limit).to_pandas()
         no_footer = re.sub(r"\n\[\d+ rows x \d+ columns\]$", "", str(df))
         print(no_footer.rstrip(" \n"))
         if len(df) == limit:
             print(f"[limited by {limit} objects]")
 
-    def clone(self: "DatasetQuery", new_table=True) -> "DatasetQuery":
+    def clone(self, new_table=True) -> "Self":
         obj = copy(self)
         obj.steps = obj.steps.copy()
         if new_table:
             obj.table = self.get_table()
         return obj
 
     @detach
-    def select(self, *args, **kwargs) -> "DatasetQuery":
+    def select(self, *args, **kwargs) -> "Self":
         """
         Select the given columns or expressions using a subquery.
 
         If used with no arguments, this simply creates a subquery and
         select all columns from it.
 
         Note that the `save` function expects default dataset columns to
@@ -1197,15 +1213,15 @@
         """
         named_args = [v.label(k) for k, v in kwargs.items()]
         query = self.clone()
         query.steps.append(SQLSelect((*args, *named_args)))
         return query
 
     @detach
-    def select_except(self, *args) -> "DatasetQuery":
+    def select_except(self, *args) -> "Self":
         """
         Exclude certain columns from this query using a subquery.
 
         Note that the `save` function expects default dataset columns to
         be present. This function is meant to be followed by a call to
         `results` if used to exclude any default columns.
 
@@ -1222,15 +1238,15 @@
             raise TypeError("select_except expected at least 1 argument, got 0")
         query_args = [c if isinstance(c, str) else c.name for c in args]
         query = self.clone()
         query.steps.append(SQLSelectExcept(query_args))  # type: ignore [arg-type]
         return query
 
     @detach
-    def select_default(self) -> "DatasetQuery":
+    def select_default(self) -> "Self":
         """
         Select only the default dataset columns using a subquery.
 
         This assumes that none of the default dataset columns have
         already been excluded from this query. This is useful if you've
         added columns with `mutate` or `select` calls for filtering but
         only want the default columns in the final output.
@@ -1244,15 +1260,15 @@
             ... )
         """
         query = self.clone()
         query.steps.append(SQLSelect((*DATASET_CORE_COLUMN_NAMES,)))
         return query
 
     @detach
-    def mutate(self, *args, **kwargs) -> "DatasetQuery":
+    def mutate(self, *args, **kwargs) -> "Self":
         """
         Add new columns to this query.
 
         This function selects all existing columns from this query and
         adds in the new columns specified.
 
         Example:
@@ -1260,35 +1276,41 @@
         """
         query_args = [v.label(k) for k, v in dict(args, **kwargs).items()]
         query = self.clone()
         query.steps.append(SQLMutate((*query_args,)))
         return query
 
     @detach
-    def filter(self, *args) -> "DatasetQuery":
+    def filter(self, *args) -> "Self":
         query = self.clone(new_table=False)
         steps = query.steps
         if steps and isinstance(steps[-1], SQLFilter):
             steps[-1] = steps[-1] & args
         else:
             steps.append(SQLFilter(args))
         return query
 
     @detach
-    def order_by(self, *args) -> "DatasetQuery":
+    def order_by(self, *args) -> "Self":
         query = self.clone(new_table=False)
         query.steps.append(SQLOrderBy(args))
         return query
 
     @detach
-    def limit(self, n: int) -> "DatasetQuery":
+    def limit(self, n: int) -> "Self":
         query = self.clone(new_table=False)
         query.steps.append(SQLLimit(n))
         return query
 
+    @detach
+    def offset(self, offset: int) -> "Self":
+        query = self.clone(new_table=False)
+        query.steps.append(SQLOffset(offset))
+        return query
+
     def count(self) -> int:
         query = self.clone()
         query.steps.append(SQLCount())
         return query.results()[0][0]
 
     def sum(self, col: ColumnElement):
         query = self.clone()
@@ -1307,35 +1329,35 @@
 
     def max(self, col: ColumnElement):
         query = self.clone()
         query.steps.append(SQLSelect((f.max(col),)))
         return query.results()[0][0]
 
     @detach
-    def group_by(self, *cols: ColumnElement) -> "DatasetQuery":
+    def group_by(self, *cols: ColumnElement) -> "Self":
         query = self.clone()
         query.steps.append(GroupBy(cols))
         return query
 
     @detach
-    def union(self, dataset_query: "DatasetQuery") -> "DatasetQuery":
+    def union(self, dataset_query: "DatasetQuery") -> "Self":
         left = self.clone()
         right = dataset_query.clone()
         new_query = self.clone()
         new_query.steps = [SQLUnion(left, right)]
         return new_query
 
     @detach
     def join(
         self,
         dataset_query: "DatasetQuery",
         predicates: Union[JoinPredicateType, Sequence[JoinPredicateType]],
         inner=False,
         rname="{name}_right",
-    ) -> "DatasetQuery":
+    ) -> "Self":
         left = self.clone(new_table=False)
         if self.table.name == dataset_query.table.name:
             # for use case where we join with itself, e.g dogs.join(dogs, "name")
             right = dataset_query.clone(new_table=True)
         else:
             right = dataset_query.clone(new_table=False)
 
@@ -1345,15 +1367,15 @@
             if isinstance(predicates, (str, ColumnClause, ColumnElement))
             else tuple(predicates)
         )
         new_query.steps = [SQLJoin(left, right, predicates, inner, rname)]
         return new_query
 
     @detach
-    def chunk(self, index: int, total: int) -> "DatasetQuery":
+    def chunk(self, index: int, total: int) -> "Self":
         """Split a query into smaller chunks for e.g. parallelization.
         Example:
             >>> query = DatasetQuery(...)
             >>> chunk_1 = query._chunk(0, 2)
             >>> chunk_2 = query._chunk(1, 2)
         Note:
             Bear in mind that `index` is 0-indexed but `total` isn't.
@@ -1368,15 +1390,15 @@
         self,
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
         cache: bool = False,
-    ) -> "DatasetQuery":
+    ) -> "Self":
         """
         Adds one or more signals based on the results from the provided UDF.
 
         Parallel can optionally be specified as >= 1 for parallel processing with a
         specific number of processes, or set to -1 for the default of
         the number of CPUs (cores) on the current machine.
 
@@ -1398,35 +1420,35 @@
                 min_task_size=min_task_size,
                 cache=cache,
             )
         )
         return query
 
     @detach
-    def subtract(self, dq: "DatasetQuery") -> "DatasetQuery":
+    def subtract(self, dq: "DatasetQuery") -> "Self":
         query = self.clone()
         query.steps.append(Subtract(dq, self.catalog))
         return query
 
     @detach
-    def changed(self, dq: "DatasetQuery") -> "DatasetQuery":
+    def changed(self, dq: "DatasetQuery") -> "Self":
         query = self.clone()
         query.steps.append(Changed(dq, self.catalog))
         return query
 
     @detach
     def generate(
         self,
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
         cache: bool = False,
-    ) -> "DatasetQuery":
+    ) -> "Self":
         query = self.clone()
         steps = query.steps
         steps.append(
             RowGenerator(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
@@ -1568,18 +1590,32 @@
         if isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
         return obj
 
     if not isinstance(dataset_query, DatasetQuery):
         sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
 
-    if isinstance(dataset_query, DatasetQuery):
-        for r in dataset_query.to_records():
-            print(json.dumps(r, default=_json_serialize))
+    try:
+        preview_args: dict[str, Any] = json.loads(
+            os.getenv("DVCX_QUERY_PREVIEW_ARGS", "")
+        )
+    except ValueError:
+        preview_args = {}
 
+    columns = preview_args.get("columns") or []
+    if columns:
+        columns.insert(0, "id")
+
+    preview_query = (
+        dataset_query.select(*columns)
+        .limit(preview_args.get("limit", 10))
+        .offset(preview_args.get("offset", 0))
+    )
+    records = json.dumps(preview_query.to_records(), default=_json_serialize)
+    print("__ds_records__", records, "__ds_records__", sep="")
     return dataset_query
 
 
 def _random_string(length: int) -> str:
     return "".join(
         random.choice(string.ascii_letters + string.digits)  # noqa: S311
         for i in range(length)
```

### Comparing `dvcx-0.72.0/src/dvcx/query/dispatch.py` & `dvcx-0.72.1/src/dvcx/query/dispatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,14 +200,20 @@
         input_rows,
         n_workers: Optional[int] = None,
         cache: bool = False,
         input_queue=None,
     ) -> Iterator[Iterable[UDFResult]]:
         n_workers = get_n_workers_from_arg(n_workers)
 
+        if self.buffer_size < n_workers:
+            raise RuntimeError(
+                f"Parallel run error: buffer size is smaller than "
+                f"number of workers: {self.buffer_size} < {n_workers}"
+            )
+
         if input_queue:
             streaming_mode = True
             self.task_queue = input_queue
         else:
             streaming_mode = False
             self.task_queue = self.ctx.Queue()
         self.done_queue = self.ctx.Queue()
@@ -240,27 +246,28 @@
             while n_workers > 0:
                 result = self.done_queue.get()
                 status = result["status"]
                 if status == FINISHED_STATUS:
                     # Worker finished
                     n_workers -= 1
                 elif status == OK_STATUS:
-                    if not streaming_mode and not input_finished:
-                        try:
-                            self.task_queue.put(next(input_data))
-                        except StopIteration:
-                            input_finished = True
                     yield result["result"]
                 else:  # Failed / error
                     n_workers -= 1
                     exc = result.get("exception")
                     if exc:
                         raise exc
                     raise RuntimeError("Internal error: Parallel UDF execution failed")
 
+                if not streaming_mode and not input_finished:
+                    try:
+                        self.task_queue.put(next(input_data))
+                    except StopIteration:
+                        input_finished = True
+
             # Finished with all tasks normally
             normal_completion = True
         finally:
             if not normal_completion:
                 # Stop all workers if there is an unexpected exception
                 for _ in pool:
                     self.task_queue.put(STOP_SIGNAL)
```

### Comparing `dvcx-0.72.0/src/dvcx/query/schema.py` & `dvcx-0.72.1/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/query/udf.py` & `dvcx-0.72.1/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/remote/studio.py` & `dvcx-0.72.1/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/default/base.py` & `dvcx-0.72.1/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/functions/array.py` & `dvcx-0.72.1/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/functions/path.py` & `dvcx-0.72.1/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/selectable.py` & `dvcx-0.72.1/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.72.1/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.72.1/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/types.py` & `dvcx-0.72.1/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/sql/utils.py` & `dvcx-0.72.1/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/storage.py` & `dvcx-0.72.1/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/src/dvcx/utils.py` & `dvcx-0.72.1/src/dvcx/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 import random
 import stat
 import sys
 import time
 from collections.abc import Iterable, Sequence
 from datetime import datetime, timezone
 from itertools import islice
-from typing import Any, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 
 from dateutil import tz
 from dateutil.parser import isoparse
 
+if TYPE_CHECKING:
+    import pandas as pd
+
 GLOB_CHARS = ["?", "*", "[", "]"]
 NUL = b"\0"
 TIME_ZERO = datetime.fromtimestamp(0, tz=timezone.utc)
 
 T = TypeVar("T", bound="DVCXDir")
 
 
@@ -293,7 +296,60 @@
     key: str, default: Optional[Sequence] = None, sep: str = ","
 ) -> Optional[Sequence[str]]:
     try:
         str_val = os.environ[key]
     except KeyError:
         return default
     return str_val.split(sep=sep)
+
+
+def show_df(
+    df: "pd.DataFrame", collapse_columns: bool = True, system_columns: bool = False
+) -> None:
+    import pandas as pd
+
+    if df.empty:
+        return
+
+    options: list[Any] = ["display.show_dimensions", False, "display.min_rows", 0]
+    if not collapse_columns:
+        options.extend(("display.max_columns", None))  # show all columns
+        options.extend(("display.max_colwidth", None))  # do not truncate cells
+        options.extend(("display.width", None))  #  do not truncate table
+
+    if not system_columns:
+        df.drop(
+            columns=[
+                "anno",
+                "checksum",
+                "dir_type",
+                "etag",
+                "is_latest",
+                "last_modified",
+                "owner_id",
+                "owner_name",
+                "parent_id",
+                "size",
+                "version",
+                "vtype",
+            ],
+            inplace=True,
+            errors="ignore",
+        )
+
+    with pd.option_context("display.max_rows", None, *options):  # show all rows
+        print(df)
+
+
+def show_records(
+    records: Optional[list[dict]],
+    collapse_columns: bool = False,
+    system_columns: bool = False,
+) -> None:
+    import pandas as pd
+
+    if not records:
+        return
+
+    index = [row.pop("id") for row in records]
+    df = pd.DataFrame.from_records(records, index=index)
+    return show_df(df, collapse_columns=collapse_columns, system_columns=system_columns)
```

### Comparing `dvcx-0.72.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.72.1/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.72.0
+Version: 0.72.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +14,15 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
 Requires-Dist: tqdm
+Requires-Dist: pandas
 Requires-Dist: python-dateutil>=2
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
@@ -88,15 +89,15 @@
    :alt: Python Version
 .. |License| image:: https://img.shields.io/pypi/l/dvcx
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License
 .. |Tests| image:: https://github.com/iterative/dvcx/workflows/Tests/badge.svg
    :target: https://github.com/iterative/dvcx/actions?workflow=Tests
    :alt: Tests
-.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/iterative/dvcx/branch/main/graph/badge.svg?token=VSCP2T9R5X
    :target: https://app.codecov.io/gh/iterative/dvcx
    :alt: Codecov
 .. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

### Comparing `dvcx-0.72.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.72.1/src/dvcx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 src/dvcx/data_storage/id_generator.py
 src/dvcx/data_storage/metastore.py
 src/dvcx/data_storage/schema.py
 src/dvcx/data_storage/serializer.py
 src/dvcx/data_storage/sqlite.py
 src/dvcx/data_storage/warehouse.py
 src/dvcx/lib/__init__.py
+src/dvcx/lib/cached_stream.py
 src/dvcx/lib/dataset.py
 src/dvcx/lib/feature.py
 src/dvcx/lib/feature_udf.py
 src/dvcx/lib/file.py
 src/dvcx/lib/gpt4_vision.py
 src/dvcx/lib/hf_image_to_text.py
 src/dvcx/lib/hf_pipeline.py
@@ -175,14 +176,15 @@
 tests/unit/test_listing.py
 tests/unit/test_metastore.py
 tests/unit/test_serializer.py
 tests/unit/test_storage.py
 tests/unit/test_udf.py
 tests/unit/test_utils.py
 tests/unit/test_warehouse.py
+tests/unit/lib/test_cached_stream.py
 tests/unit/lib/test_feature.py
 tests/unit/lib/test_feature_udf.py
 tests/unit/lib/test_file.py
 tests/unit/lib/test_webdataset.py
 tests/unit/lib/test_webdataset_meta.py
 tests/unit/sql/test_array.py
 tests/unit/sql/test_conditional.py
```

### Comparing `dvcx-0.72.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.72.1/src/dvcx.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 pyyaml
 tomlkit
 tqdm
+pandas
 python-dateutil>=2
 attrs>=21.3.0
 s3fs>=2024.2.0
 gcsfs>=2024.2.0
 adlfs>=2024.2.0
 dvc-data<4,>=3.10
 dvc-objects<6,>=4
```

### Comparing `dvcx-0.72.0/tests/benchmarks/conftest.py` & `dvcx-0.72.1/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/conftest.py` & `dvcx-0.72.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/data.py` & `dvcx-0.72.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_catalog.py` & `dvcx-0.72.1/tests/func/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,15 +938,15 @@
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
     DatasetQuery({src_uri!r})
     """
     query_script = dedent(query_script)
 
-    dataset, version, query_output = catalog.query(query_script, save=True)
+    dataset, version, query_output, _ = catalog.query(query_script, save=True)
     assert dataset
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
```

### Comparing `dvcx-0.72.0/tests/func/test_client.py` & `dvcx-0.72.1/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_dataset_query.py` & `dvcx-0.72.1/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_datasets.py` & `dvcx-0.72.1/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_ls.py` & `dvcx-0.72.1/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_pull.py` & `dvcx-0.72.1/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/func/test_pytorch.py` & `dvcx-0.72.1/tests/func/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from torch import Size, Tensor
 from torchvision.datasets import FakeData
 from torchvision.transforms import v2
 
 from dvcx.catalog import get_catalog
 from dvcx.lib.param import Image
-from dvcx.lib.pytorch import DvcxDataset
+from dvcx.lib.pytorch import PytorchDataset
 from dvcx.query import DatasetQuery, udf
 from dvcx.sql.types import Int
 
 
 @pytest.fixture
 def fake_dataset(tmp_path):
     # Create fake images in labeled dirs
@@ -32,15 +32,15 @@
 
     catalog.remove_dataset("fake", version=1)
     catalog.id_generator.cleanup_for_tests()
 
 
 def test_pytorch_dataset(tmp_path, fake_dataset):
     transform = v2.Resize((64, 64))
-    pt_dataset = DvcxDataset(
+    pt_dataset = PytorchDataset(
         params=[Image(), "label"],
         name=fake_dataset.name,
         version=fake_dataset.version,
         transform=transform,
     )
     for img, label in pt_dataset:
         assert isinstance(img, Tensor)
```

### Comparing `dvcx-0.72.0/tests/func/test_query.py` & `dvcx-0.72.1/tests/func/test_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import json
+from itertools import dropwhile
 from textwrap import dedent
 
 import dill
 import pytest
 
 from dvcx.catalog import QUERY_DATASET_NAME_PREFIX
 from dvcx.cli import query
-from dvcx.query import C, DatasetQuery
 
 
 @pytest.fixture
 def catalog_info_filepath(cloud_test_catalog_tmpfile, tmp_path):
     catalog = cloud_test_catalog_tmpfile.catalog
 
     catalog_info = {
@@ -58,14 +57,15 @@
         warehouse=warehouse,
         **catalog_info["catalog_init_params"],
     )
     """
     return dedent(query_catalog_setup + "\n" + query)
 
 
+@pytest.mark.parametrize("cloud_type,version_aware", [("file", False)], indirect=True)
 def test_query_cli(cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath, capsys):
     catalog = cloud_test_catalog_tmpfile.catalog
     src_uri = cloud_test_catalog_tmpfile.src_uri
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
 
@@ -73,102 +73,42 @@
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     filepath = tmp_path / "query_script.py"
     filepath.write_text(query_script)
 
     ds_name = "my-dataset"
-    query(catalog, str(filepath), ds_name)
+    query(catalog, str(filepath), ds_name, columns=["name"])
     captured = capsys.readouterr()
     assert captured.err == ""
-    printed_rows = captured.out.strip().split("\n")[-7:]
-    rows = [json.loads(r) for r in printed_rows]
-    rows = sorted(rows, key=lambda r: r["name"])
-    assert [r["name"] for r in rows] == [
-        "cat1",
-        "cat2",
-        "description",
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    ]
 
-    result = (
-        DatasetQuery(src_uri, catalog=catalog)
-        .select(C.source, C.parent, C.name, C.vtype, C.size)
-        .order_by(C.source, C.parent, C.name)
-        .to_records()
+    # drop lines with progress bars or empty lines, until we get to the table
+    header, *rows = list(
+        dropwhile(
+            lambda line: not line or "Listing" in line,
+            captured.out.splitlines(),
+        )
     )
-
-    assert result == [
-        {
-            "source": src_uri,
-            "parent": "",
-            "name": "description",
-            "vtype": "",
-            "size": 13,
-        },
-        {
-            "source": src_uri,
-            "parent": "cats",
-            "name": "cat1",
-            "vtype": "",
-            "size": 4,
-        },
-        {
-            "source": src_uri,
-            "parent": "cats",
-            "name": "cat2",
-            "vtype": "",
-            "size": 4,
-        },
-        {
-            "source": src_uri,
-            "parent": "dogs",
-            "name": "dog1",
-            "vtype": "",
-            "size": 4,
-        },
-        {
-            "source": src_uri,
-            "parent": "dogs",
-            "name": "dog2",
-            "vtype": "",
-            "size": 3,
-        },
-        {
-            "source": src_uri,
-            "parent": "dogs",
-            "name": "dog3",
-            "vtype": "",
-            "size": 4,
-        },
-        {
-            "source": src_uri,
-            "parent": "dogs/others",
-            "name": "dog4",
-            "vtype": "",
-            "size": 4,
-        },
-    ]
+    assert header.strip() == "name"
+    name_rows = {row.split()[1] for row in rows}
+    assert name_rows == {"cat1", "cat2", "description", "dog1", "dog2", "dog3", "dog4"}
 
 
 def test_query(cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath):
     catalog = cloud_test_catalog_tmpfile.catalog
     src_uri = cloud_test_catalog_tmpfile.src_uri
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
 
     DatasetQuery({src_uri!r}, catalog=catalog)
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
-    dataset, version, output = catalog.query(query_script, save=True)
+    dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name.startswith(QUERY_DATASET_NAME_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "cat1",
         "cat2",
@@ -193,15 +133,15 @@
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
 
     DatasetQuery({src_uri!r}, catalog=catalog).filter(C.name.glob("dog*")).save("dogs")
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
-    dataset, version, output = catalog.query(query_script, save=True)
+    dataset, version, output, _ = catalog.query(query_script, save=True)
     assert not dataset.name.startswith(QUERY_DATASET_NAME_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
@@ -226,15 +166,15 @@
     ds = DatasetQuery(
         {src_uri!r}, catalog=catalog
     ).filter(C.name.glob("dog*")).save("dogs")
     ds
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
-    dataset, version, output = catalog.query(query_script, save=True)
+    dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name == "dogs"
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
@@ -259,15 +199,15 @@
     ds = DatasetQuery(
         {src_uri!r}, catalog=catalog
     ).filter(C.name.glob("dog*")).save("dogs")
     DatasetQuery(name="dogs", version=1)
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
-    dataset, version, output = catalog.query(query_script, save=True)
+    dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name == "dogs"
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
```

### Comparing `dvcx-0.72.0/tests/test_cli_e2e.py` & `dvcx-0.72.1/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/lib/test_feature.py` & `dvcx-0.72.1/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.72.1/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.72.1/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.72.1/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/sql/test_array.py` & `dvcx-0.72.1/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/sql/test_conditional.py` & `dvcx-0.72.1/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/sql/test_path.py` & `dvcx-0.72.1/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/sql/test_selectable.py` & `dvcx-0.72.1/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/sql/test_string.py` & `dvcx-0.72.1/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_asyn.py` & `dvcx-0.72.1/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_cache.py` & `dvcx-0.72.1/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_catalog.py` & `dvcx-0.72.1/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_catalog_formats.py` & `dvcx-0.72.1/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_catalog_loader.py` & `dvcx-0.72.1/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_cli_parsing.py` & `dvcx-0.72.1/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_client.py` & `dvcx-0.72.1/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_client_s3.py` & `dvcx-0.72.1/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_data_storage.py` & `dvcx-0.72.1/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_database_engine.py` & `dvcx-0.72.1/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_dataset.py` & `dvcx-0.72.1/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_fileslice.py` & `dvcx-0.72.1/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_id_generator.py` & `dvcx-0.72.1/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_listing.py` & `dvcx-0.72.1/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_metastore.py` & `dvcx-0.72.1/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_serializer.py` & `dvcx-0.72.1/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_storage.py` & `dvcx-0.72.1/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_udf.py` & `dvcx-0.72.1/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_utils.py` & `dvcx-0.72.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/unit/test_warehouse.py` & `dvcx-0.72.1/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.72.0/tests/utils.py` & `dvcx-0.72.1/tests/utils.py`

 * *Files identical despite different names*

