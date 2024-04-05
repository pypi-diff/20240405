# Comparing `tmp/deeplake-3.8.8.tar.gz` & `tmp/deeplake-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.8.8.tar", last modified: Wed Nov 22 17:04:33 2023, max compression
+gzip compressed data, was "deeplake-3.8.9.tar", last modified: Wed Nov 29 19:29:06 2023, max compression
```

## Comparing `deeplake-3.8.8.tar` & `deeplake-3.8.9.tar`

### file list

```diff
@@ -1,412 +1,418 @@
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.901004 deeplake-3.8.8/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2023-11-22 16:55:57.000000 deeplake-3.8.8/LICENSE
--rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2023-11-22 16:55:57.000000 deeplake-3.8.8/MANIFEST.in
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22051 2023-11-22 17:04:33.901236 deeplake-3.8.8/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21361 2023-11-22 16:55:57.000000 deeplake-3.8.8/README.md
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.800247 deeplake-3.8.8/deeplake/
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2773 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.803268 deeplake-3.8.8/deeplake/api/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   104449 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2703 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/read.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.811607 deeplake-3.8.8/deeplake/api/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2192 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    98370 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_api.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3481 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_events.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      279 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_linking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_none.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1766 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10559 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_pop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_reset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_text.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7449 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tests/test_views.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/api/tiled.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.811770 deeplake-3.8.8/deeplake/auto/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.812255 deeplake-3.8.8/deeplake/auto/structured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/structured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/structured/base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7242 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.813140 deeplake-3.8.8/deeplake/auto/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13490 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.813961 deeplake-3.8.8/deeplake/auto/unstructured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.814608 deeplake-3.8.8/deeplake/auto/unstructured/coco/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6693 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.815322 deeplake-3.8.8/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.816044 deeplake-3.8.8/deeplake/cli/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/cli/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5913 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/cli/auth.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      410 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/cli/commands.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      930 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/cli/test_cli.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.818541 deeplake-3.8.8/deeplake/client/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23581 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1372 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/config.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/log.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12175 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/test_client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13788 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/client/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10030 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/constants.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.829319 deeplake-3.8.8/deeplake/core/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.830978 deeplake-3.8.8/deeplake/core/chunk/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24220 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26201 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6467 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   123835 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    39116 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compression.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.832575 deeplake-3.8.8/deeplake/core/compute/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/process.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/ray.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/serial.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/compute/thread.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.835003 deeplake-3.8.8/deeplake/core/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   194383 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13181 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6267 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4769 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/distance_type.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.835548 deeplake-3.8.8/deeplake/core/index/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/index/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    17728 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/index/index.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/index_maintenance.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20539 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/ipc.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/link_creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16506 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/linked_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/lock.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.836767 deeplake-3.8.8/deeplake/core/meta/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3625 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.838739 deeplake-3.8.8/deeplake/core/meta/encode/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13495 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.840152 deeplake-3.8.8/deeplake/core/meta/encode/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14848 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/partial_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/partial_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/polygon.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.841180 deeplake-3.8.8/deeplake/core/query/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/query/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/query/autocomplete.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14773 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/query/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/query/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20658 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23390 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.844203 deeplake-3.8.8/deeplake/core/storage/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14920 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19100 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/gcs.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13053 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/google_drive.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9594 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/local.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20000 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26417 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/storage/s3.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    64877 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tensor.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7485 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tensor_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.846499 deeplake-3.8.8/deeplake/core/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16104 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_locking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1925 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8907 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tests/test_vdb_indexes.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.848047 deeplake-3.8.8/deeplake/core/tiling/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.849959 deeplake-3.8.8/deeplake/core/transform/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/transform/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/transform/test_transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    30321 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/transform/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9153 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4402 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.852999 deeplake-3.8.8/deeplake/core/vectorstore/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23766 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/deep_memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    40379 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1918 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/deepmemory_vectorstore.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    80915 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18624 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/test_deepmemory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3107 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/test_embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1282 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/unsupported_deep_memory.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.853795 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.854243 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18841 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14222 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.855017 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.856106 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4535 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.856669 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1649 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.857380 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.858051 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2375 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1597 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22169 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3891 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vector_search/vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/vectorstore/vectorstore_factory.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.859280 deeplake-3.8.8/deeplake/core/version_control/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3109 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    91901 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.861025 deeplake-3.8.8/deeplake/enterprise/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      257 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7295 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37214 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6063 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4833 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    28046 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3633 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1743 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/enterprise/util.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/hooks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8281 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/htype.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.861202 deeplake-3.8.8/deeplake/integrations/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.861515 deeplake-3.8.8/deeplake/integrations/huggingface/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5487 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.862360 deeplake-3.8.8/deeplake/integrations/mmdet/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    62754 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4739 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19644 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.863365 deeplake-3.8.8/deeplake/integrations/pytorch/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9863 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7151 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.864550 deeplake-3.8.8/deeplake/integrations/tf/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/tf/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2453 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5330 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.864869 deeplake-3.8.8/deeplake/integrations/wandb/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.869326 deeplake-3.8.8/deeplake/requirements/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      479 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/requirements/common.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/requirements/docs.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/requirements/plugins.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      380 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/requirements/tests.txt
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.879206 deeplake-3.8.8/deeplake/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2379 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/client_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21920 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/path_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.889611 deeplake-3.8.8/deeplake/util/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/array_list.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5873 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/bugout_reporter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/bugout_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/cache_chain.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4594 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/casting.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/check_installation.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/check_latest_version.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/class_label.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/delete_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15912 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/empty_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37405 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/exceptions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/exif.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/from_tfds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/generate_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/hash.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2793 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/htype.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/image.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/invalid_view_op.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/iteration_warning.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/join_chunks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/logging.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/modified.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/notebook.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.893650 deeplake-3.8.8/deeplake/util/object_3d/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10213 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7187 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1160 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/path.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/pretty_print.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2763 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/remove_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/scheduling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/spinner.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9530 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/storage.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/testing.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.898811 deeplake-3.8.8/deeplake/util/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_read.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2428 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/threading.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26825 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    41372 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      927 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/util/warnings.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.900581 deeplake-3.8.8/deeplake/visualizer/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/visualizer/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2023-11-22 16:55:57.000000 deeplake-3.8.8/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-22 17:04:33.801306 deeplake-3.8.8/deeplake.egg-info/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22051 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13207 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       57 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1098 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/requires.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2023-11-22 17:04:33.000000 deeplake-3.8.8/deeplake.egg-info/top_level.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2023-11-22 16:55:57.000000 deeplake-3.8.8/pyproject.toml
--rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2023-11-22 17:04:33.902111 deeplake-3.8.8/setup.cfg
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3399 2023-11-22 16:55:57.000000 deeplake-3.8.8/setup.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.330427 deeplake-3.8.9/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2023-11-29 18:49:50.000000 deeplake-3.8.9/LICENSE
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2023-11-29 18:49:50.000000 deeplake-3.8.9/MANIFEST.in
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22051 2023-11-29 19:29:06.330572 deeplake-3.8.9/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21361 2023-11-29 18:49:50.000000 deeplake-3.8.9/README.md
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.252452 deeplake-3.8.9/deeplake/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2773 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.255697 deeplake-3.8.9/deeplake/api/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   104449 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2703 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/read.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.264685 deeplake-3.8.9/deeplake/api/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2192 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    98370 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_api.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3481 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_events.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      279 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_none.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1766 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10559 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_text.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7449 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tests/test_views.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/api/tiled.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.264931 deeplake-3.8.9/deeplake/auto/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.265248 deeplake-3.8.9/deeplake/auto/structured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/structured/base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7242 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.266193 deeplake-3.8.9/deeplake/auto/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13490 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.266952 deeplake-3.8.9/deeplake/auto/unstructured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.267890 deeplake-3.8.9/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6693 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.268509 deeplake-3.8.9/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.269406 deeplake-3.8.9/deeplake/cli/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/cli/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5913 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/cli/auth.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      410 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/cli/commands.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      930 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/cli/test_cli.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.270779 deeplake-3.8.9/deeplake/client/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    23597 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1779 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/config.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/log.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12175 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/test_client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13804 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/client/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10030 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/constants.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.277141 deeplake-3.8.9/deeplake/core/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.279157 deeplake-3.8.9/deeplake/core/chunk/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24220 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26201 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6467 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   123835 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    39116 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compression.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.281626 deeplake-3.8.9/deeplake/core/compute/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/process.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/ray.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/serial.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/compute/thread.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.284334 deeplake-3.8.9/deeplake/core/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   194454 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13181 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6267 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4769 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/distance_type.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.284746 deeplake-3.8.9/deeplake/core/index/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/index/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    17728 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/index/index.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/index_maintenance.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20539 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/ipc.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/link_creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16506 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/linked_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/lock.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.285494 deeplake-3.8.9/deeplake/core/meta/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3625 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.287104 deeplake-3.8.9/deeplake/core/meta/encode/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13495 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.288838 deeplake-3.8.9/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14848 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/partial_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/partial_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/polygon.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.289724 deeplake-3.8.9/deeplake/core/query/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/query/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14773 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/query/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/query/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20674 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    23390 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.292241 deeplake-3.8.9/deeplake/core/storage/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14952 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19100 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/gcs.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13053 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9594 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/local.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20000 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26417 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/storage/s3.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    64877 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tensor.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7485 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tensor_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.294644 deeplake-3.8.9/deeplake/core/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16104 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1925 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8907 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tests/test_vdb_indexes.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.295996 deeplake-3.8.9/deeplake/core/tiling/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.297441 deeplake-3.8.9/deeplake/core/transform/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/transform/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    30321 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/transform/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9153 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4402 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.297976 deeplake-3.8.9/deeplake/core/vectorstore/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.299292 deeplake-3.8.9/deeplake/core/vectorstore/dataset_handlers/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/dataset_handlers/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13340 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6370 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.301059 deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25072 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/deep_memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18777 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    31852 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.301505 deeplake-3.8.9/deeplake/core/vectorstore/embeddings/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/embeddings/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/embeddings/embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/embeddings/test_embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    88671 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.302085 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.302806 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19073 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.303507 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.304495 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4535 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.305000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1649 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.305586 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.306139 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2375 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1597 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22180 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3891 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.307267 deeplake-3.8.9/deeplake/core/version_control/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3109 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    91901 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.309357 deeplake-3.8.9/deeplake/enterprise/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      257 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7295 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37214 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6063 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4833 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    28046 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3633 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1743 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/enterprise/util.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/hooks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8281 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/htype.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.309491 deeplake-3.8.9/deeplake/integrations/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.309808 deeplake-3.8.9/deeplake/integrations/huggingface/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.310576 deeplake-3.8.9/deeplake/integrations/mmdet/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    62754 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4739 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19644 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.311600 deeplake-3.8.9/deeplake/integrations/pytorch/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9863 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7151 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.312241 deeplake-3.8.9/deeplake/integrations/tf/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/tf/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2453 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5330 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.312598 deeplake-3.8.9/deeplake/integrations/wandb/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.313167 deeplake-3.8.9/deeplake/requirements/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      479 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/requirements/common.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/requirements/docs.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/requirements/plugins.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      399 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/requirements/tests.txt
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.314303 deeplake-3.8.9/deeplake/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2379 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22231 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.325580 deeplake-3.8.9/deeplake/util/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/array_list.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5873 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/bugout_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/cache_chain.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4594 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/casting.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/check_installation.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/check_latest_version.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/class_label.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/delete_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15912 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/empty_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37405 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/exceptions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/exif.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/from_tfds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/generate_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/hash.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2793 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/htype.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/image.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/iteration_warning.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/join_chunks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/logging.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/modified.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/notebook.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.327827 deeplake-3.8.9/deeplake/util/object_3d/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10213 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7187 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1160 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/path.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/pretty_print.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2763 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/remove_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/scheduling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/spinner.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9530 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/storage.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/testing.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.329559 deeplake-3.8.9/deeplake/util/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_read.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2428 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/threading.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26825 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    41372 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      927 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/util/warnings.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.330162 deeplake-3.8.9/deeplake/visualizer/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/visualizer/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2023-11-29 18:49:50.000000 deeplake-3.8.9/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2023-11-29 19:29:06.253505 deeplake-3.8.9/deeplake.egg-info/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22051 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13456 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       57 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2023-11-29 19:28:42.000000 deeplake-3.8.9/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1098 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/requires.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2023-11-29 19:29:06.000000 deeplake-3.8.9/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2023-11-29 18:49:50.000000 deeplake-3.8.9/pyproject.toml
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2023-11-29 19:29:06.330862 deeplake-3.8.9/setup.cfg
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3399 2023-11-29 18:49:50.000000 deeplake-3.8.9/setup.py
```

### Comparing `deeplake-3.8.8/LICENSE` & `deeplake-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/PKG-INFO` & `deeplake-3.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.8.8
+Version: 3.8.9
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.8.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.8.9 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.8.8/README.md` & `deeplake-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/__init__.py` & `deeplake-3.8.9/deeplake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     "delete",
     "copy",
     "rename",
     "random",
 ]
 
 
-__version__ = "3.8.8"
+__version__ = "3.8.9"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
```

### Comparing `deeplake-3.8.8/deeplake/api/dataset.py` & `deeplake-3.8.9/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/info.py` & `deeplake-3.8.9/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/link.py` & `deeplake-3.8.9/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/link_tiled.py` & `deeplake-3.8.9/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/read.py` & `deeplake-3.8.9/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_access_method.py` & `deeplake-3.8.9/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_agreement.py` & `deeplake-3.8.9/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_api.py` & `deeplake-3.8.9/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.8.9/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.8.9/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.8.9/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.8.9/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_dataset.py` & `deeplake-3.8.9/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_dicom.py` & `deeplake-3.8.9/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_downsample.py` & `deeplake-3.8.9/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_events.py` & `deeplake-3.8.9/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_grayscale.py` & `deeplake-3.8.9/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_info.py` & `deeplake-3.8.9/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.8.9/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_json.py` & `deeplake-3.8.9/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_link.py` & `deeplake-3.8.9/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.8.9/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_linking.py` & `deeplake-3.8.9/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_mesh.py` & `deeplake-3.8.9/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_meta.py` & `deeplake-3.8.9/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_nifti.py` & `deeplake-3.8.9/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_none.py` & `deeplake-3.8.9/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.8.9/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_pickle.py` & `deeplake-3.8.9/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.8.9/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_polygons.py` & `deeplake-3.8.9/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_pop.py` & `deeplake-3.8.9/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_readonly.py` & `deeplake-3.8.9/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_rechunk.py` & `deeplake-3.8.9/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_reset.py` & `deeplake-3.8.9/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_sample_info.py` & `deeplake-3.8.9/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_text.py` & `deeplake-3.8.9/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_update_samples.py` & `deeplake-3.8.9/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_video.py` & `deeplake-3.8.9/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tests/test_views.py` & `deeplake-3.8.9/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/api/tiled.py` & `deeplake-3.8.9/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/structured/base.py` & `deeplake-3.8.9/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/structured/dataframe.py` & `deeplake-3.8.9/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.8.9/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.8.9/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.8.9/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.8.9/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/base.py` & `deeplake-3.8.9/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.8.9/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.8.9/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.8.9/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.8.9/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.8.9/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.8.9/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/util.py` & `deeplake-3.8.9/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.8.9/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.8.9/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/cli/auth.py` & `deeplake-3.8.9/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/cli/test_cli.py` & `deeplake-3.8.9/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/client/client.py` & `deeplake-3.8.9/deeplake/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import deeplake
-import requests
+import requests  # type: ignore
 import textwrap
 from typing import Any, Optional, Dict, List, Union
 from deeplake.util.exceptions import (
     AgreementNotAcceptedError,
     AuthorizationException,
     LoginException,
     InvalidPasswordException,
```

### Comparing `deeplake-3.8.8/deeplake/client/config.py` & `deeplake-3.8.9/deeplake/client/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,7 +27,16 @@
 CONNECT_DATASET_SUFFIX = "/api/dataset/connect"
 REMOTE_QUERY_SUFFIX = "/api/query/dataset/{}/{}"
 
 DEFAULT_REQUEST_TIMEOUT = 170
 
 DEEPLAKE_AUTH_TOKEN = "ACTIVELOOP_TOKEN"
 ORG_PERMISSION_SUFFIX = "/api/organizations/{}/features/dataset_query"
+
+# ManagedService Endpoints
+INIT_VECTORSTORE_SUFFIX = "/api/dlserver/vectorstore/init"
+GET_VECTORSTORE_SUMMARY_SUFFIX = "/api/dlserver/vectorstore/{}/{}/summary"
+DELETE_VECTORSTORE_SUFFIX = "/api/dlserver/vectorstore"
+
+VECTORSTORE_SEARCH_SUFFIX = "/api/dlserver/vectorstore/search"
+VECTORSTORE_ADD_SUFFIX = "/api/dlserver/vectorstore/add"
+VECTORSTORE_REMOVE_ROWS_SUFFIX = "/api/dlserver/vectorstore/remove"
```

### Comparing `deeplake-3.8.8/deeplake/client/log.py` & `deeplake-3.8.9/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/client/test_client.py` & `deeplake-3.8.9/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/client/utils.py` & `deeplake-3.8.9/deeplake/client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import json
-import requests
+import requests  # type: ignore
 import textwrap
 from pathlib import Path
 from typing import Dict, List, Any, Union, Optional
 
 
 from deeplake.client.config import (
     REPORTING_CONFIG_FILE_PATH,
```

### Comparing `deeplake-3.8.8/deeplake/compression.py` & `deeplake-3.8.9/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/constants.py` & `deeplake-3.8.9/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/base_chunk.py` & `deeplake-3.8.9/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.8.9/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.8.9/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.8.9/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.8.9/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.8.9/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.8.9/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/chunk_engine.py` & `deeplake-3.8.9/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compression.py` & `deeplake-3.8.9/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compute/process.py` & `deeplake-3.8.9/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compute/provider.py` & `deeplake-3.8.9/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compute/ray.py` & `deeplake-3.8.9/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compute/serial.py` & `deeplake-3.8.9/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/compute/thread.py` & `deeplake-3.8.9/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/__init__.py` & `deeplake-3.8.9/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/dataset.py` & `deeplake-3.8.9/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1351,15 +1351,15 @@
                     "Setting tensor attributes directly is not supported. To add a tensor, use the `create_tensor` method."
                     + "To add data to a tensor, use the `append` and `extend` methods."
                 )
         return super().__setattr__(name, value)
 
     def __iter__(self):
         dataset_read(self)
-        for i in range(len(self)):
+        for i in range(self.__len__(warn=False)):
             yield self.__getitem__(
                 i, is_iteration=not isinstance(self.index.values[0], list)
             )
 
     def _get_commit_id_for_address(self, address, version_state):
         if address in version_state["branch_commit_map"]:
             branch = address
@@ -2146,15 +2146,17 @@
             pad_tensors=pad_tensors,
             decode_method=decode_method,
             cache_size=cache_size,
             **kwargs,
         )
 
         if progressbar:
-            dataloader = tqdm(dataloader, desc=self.path, total=len(self) // batch_size)
+            dataloader = tqdm(
+                dataloader, desc=self.path, total=self.__len__(warn=False) // batch_size
+            )
         dataset_read(self)
         return dataloader
 
     def dataloader(self, ignore_errors: bool = False, verbose: bool = False):
         """Returns a :class:`~deeplake.enterprise.DeepLakeDataLoader` object.
 
         Args:
@@ -3050,15 +3052,14 @@
             Tensor(key='data')
             >>> ds.create_tensor('labels')
             Tensor(key='labels')
             >>> ds.append({"data": [1, 2, 3, 4], "labels":[0, 1, 2, 3]})
 
         """
         tensors = self.tensors
-        new_row_ids = list(range(len(self), len(self) + len(sample)))
         if isinstance(sample, Dataset):
             sample = sample.tensors
         if not isinstance(sample, dict):
             raise SampleAppendingError()
 
         skipped_tensors = [k for k in tensors if k not in sample]
         if skipped_tensors and not skip_ok and not append_empty:
@@ -3173,15 +3174,16 @@
         n = len(samples[next(iter(samples.keys()))])
         for v in samples.values():
             if len(v) != n:
                 sizes = {k: len(v) for (k, v) in samples.items()}
                 raise ValueError(
                     f"Incoming samples are not of equal lengths. Incoming sample sizes: {sizes}"
                 )
-        new_row_ids = list(range(len(self), len(self) + n))
+        len_ds = self.__len__(warn=False)
+        new_row_ids = list(range(len_ds, len_ds + n))
         [f() for f in list(self._update_hooks.values())]
         if extend:
             if ignore_errors:
                 warnings.warn(
                     "`ignore_errors` argument will be ignored while extending with numpy arrays or tensors."
                 )
             self._append_or_extend(
@@ -3243,15 +3245,15 @@
             >>> ds.create_tensor('data')
             Tensor(key='data')
             >>> ds.create_tensor('labels')
             Tensor(key='labels')
             >>> ds.append({"data": [1, 2, 3, 4], "labels":[0, 1, 2, 3]})
 
         """
-        new_row_ids = [len(self)]
+        new_row_ids = [self.__len__(warn=False)]
         self._append_or_extend(
             sample,
             extend=False,
             skip_ok=skip_ok,
             append_empty=append_empty,
         )
         index_maintenance.index_operation_dataset(
@@ -3340,15 +3342,15 @@
 
                         saved[k].append(old_sample)
                     self[k] = v
                 # Regenerate Index
                 index_maintenance.index_operation_dataset(
                     self,
                     dml_type=_INDEX_OPERATION_MAPPING["UPDATE"],
-                    rowids=list(self.index.values[0].indices(len(self))),
+                    rowids=list(self.index.values[0].indices(self.__len__(warn=False))),
                 )
             except Exception as e:
                 for k, v in saved.items():
                     # squeeze
                     if len(v) == 1:
                         v = v[0]
                     try:
@@ -3357,15 +3359,15 @@
                         raise Exception(
                             "Error while attempting to rollback updates"
                         ) from e2
                 # in case of error, regenerate index again to avoid index corruption
                 index_maintenance.index_operation_dataset(
                     self,
                     dml_type=_INDEX_OPERATION_MAPPING["UPDATE"],
-                    rowids=list(self.index.values[0].indices(len(self))),
+                    rowids=list(self.index.values[0].indices(self.__len__(warn=False))),
                 )
                 raise e
             finally:
                 # restore update hooks
                 if self._view_base:
                     self._view_base._update_hooks = saved_update_hooks
```

### Comparing `deeplake-3.8.8/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.8.9/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.8.9/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.8.9/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/invalid_view.py` & `deeplake-3.8.9/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/dataset/view_entry.py` & `deeplake-3.8.9/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/fast_forwarding.py` & `deeplake-3.8.9/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/index/index.py` & `deeplake-3.8.9/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/index_maintenance.py` & `deeplake-3.8.9/deeplake/core/index_maintenance.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/io.py` & `deeplake-3.8.9/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/ipc.py` & `deeplake-3.8.9/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/link_creds.py` & `deeplake-3.8.9/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/linked_chunk_engine.py` & `deeplake-3.8.9/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/linked_sample.py` & `deeplake-3.8.9/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/linked_tiled_sample.py` & `deeplake-3.8.9/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/lock.py` & `deeplake-3.8.9/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/dataset_meta.py` & `deeplake-3.8.9/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.8.9/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.8.9/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.8.9/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/creds.py` & `deeplake-3.8.9/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/pad.py` & `deeplake-3.8.9/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/sequence.py` & `deeplake-3.8.9/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/shape.py` & `deeplake-3.8.9/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/encode/tile.py` & `deeplake-3.8.9/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/meta/tensor_meta.py` & `deeplake-3.8.9/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/partial_reader.py` & `deeplake-3.8.9/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/partial_sample.py` & `deeplake-3.8.9/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/polygon.py` & `deeplake-3.8.9/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/query/autocomplete.py` & `deeplake-3.8.9/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/query/filter.py` & `deeplake-3.8.9/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/query/query.py` & `deeplake-3.8.9/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/sample.py` & `deeplake-3.8.9/deeplake/core/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import requests  # type: ignore
 from deeplake.core.compression import (
     compress_array,
     decompress_array,
     verify_compressed_file,
     read_meta_from_compressed_file,
     get_compression,
     _open_video,
```

### Comparing `deeplake-3.8.8/deeplake/core/seed.py` & `deeplake-3.8.9/deeplake/core/seed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/serialize.py` & `deeplake-3.8.9/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/azure.py` & `deeplake-3.8.9/deeplake/core/storage/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from deeplake.util.exceptions import PathNotEmptyException
 from deeplake.client.client import DeepLakeBackendClient
 from concurrent.futures import ThreadPoolExecutor
 from deeplake.util.path import relpath
 from concurrent import futures
 
 try:
-    from azure.identity import DefaultAzureCredential
-    from azure.storage.blob import (
+    from azure.identity import DefaultAzureCredential  # type: ignore
+    from azure.storage.blob import (  # type: ignore
         BlobServiceClient,
         BlobSasPermissions,
         ContainerSasPermissions,
         generate_blob_sas,
         generate_container_sas,
     )
     from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
```

### Comparing `deeplake-3.8.8/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.8.9/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/gcs.py` & `deeplake-3.8.9/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/google_drive.py` & `deeplake-3.8.9/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/local.py` & `deeplake-3.8.9/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/lru_cache.py` & `deeplake-3.8.9/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/memory.py` & `deeplake-3.8.9/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/provider.py` & `deeplake-3.8.9/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/storage/s3.py` & `deeplake-3.8.9/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tensor.py` & `deeplake-3.8.9/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tensor_link.py` & `deeplake-3.8.9/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/test_serialize.py` & `deeplake-3.8.9/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_compression.py` & `deeplake-3.8.9/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_compute.py` & `deeplake-3.8.9/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.8.9/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_io.py` & `deeplake-3.8.9/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_locking.py` & `deeplake-3.8.9/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_readonly.py` & `deeplake-3.8.9/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_serialize.py` & `deeplake-3.8.9/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tests/test_vdb_indexes.py` & `deeplake-3.8.9/deeplake/core/tests/test_vdb_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/deserialize.py` & `deeplake-3.8.9/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/optimizer.py` & `deeplake-3.8.9/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.8.9/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/serialize.py` & `deeplake-3.8.9/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.8.9/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/tiling/test_serialize.py` & `deeplake-3.8.9/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/transform/test_transform.py` & `deeplake-3.8.9/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/transform/transform.py` & `deeplake-3.8.9/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/transform/transform_dataset.py` & `deeplake-3.8.9/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/transform/transform_tensor.py` & `deeplake-3.8.9/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/__init__.py` & `deeplake-3.8.9/deeplake/core/vectorstore/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,12 +7,10 @@
 )
 from deeplake.core.vectorstore.vector_search.python.search_algorithm import (
     search as python_search_algorithm,
 )
 from deeplake.core.vectorstore.vector_search.indra.search_algorithm import (
     search as indra_search_algorithm,
 )
-from deeplake.core.vectorstore.vectorstore_factory import (
-    vectorstore_factory as VectorStore,
-)
+from deeplake.core.vectorstore.deeplake_vectorstore import VectorStore
 
 DeepLakeVectorStore = VectorStore
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/deep_memory.py` & `deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/deep_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,37 +6,59 @@
 from time import time
 
 import numpy as np
 
 import deeplake
 from deeplake.enterprise.dataloader import indra_available
 from deeplake.util.exceptions import (
+    DeepMemoryWaitingListError,
     IncorrectRelevanceTypeError,
     IncorrectQueriesTypeError,
 )
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.constants import (
     DEFAULT_QUERIES_VECTORSTORE_TENSORS,
     DEFAULT_MEMORY_CACHE_SIZE,
     DEFAULT_LOCAL_CACHE_SIZE,
+    DEFAULT_DEEPMEMORY_DISTANCE_METRIC,
 )
 from deeplake.util.storage import get_storage_and_cache_chain
 from deeplake.core.dataset import Dataset
 from deeplake.core.dataset.deeplake_cloud_dataset import DeepLakeCloudDataset
-from deeplake.core.vectorstore.deeplake_vectorstore import VectorStore
 from deeplake.client.client import DeepMemoryBackendClient
 from deeplake.client.utils import JobResponseStatusSchema
 from deeplake.util.bugout_reporter import (
     feature_report_path,
 )
-from deeplake.util.dataset import try_flushing
 from deeplake.util.path import get_path_type
 from deeplake.util.version_control import load_meta
 
 
+def use_deep_memory(func):
+    def wrapper(self, *args, **kwargs):
+        use_deep_memory = kwargs.get("deep_memory")
+        distance_metric = kwargs.get("distance_metric")
+
+        if use_deep_memory and distance_metric is None:
+            kwargs["distance_metric"] = DEFAULT_DEEPMEMORY_DISTANCE_METRIC
+
+        return func(self, *args, **kwargs)
+
+    return wrapper
+
+
+def access_control(func):
+    def wrapper(self, *args, **kwargs):
+        if self.client is None:
+            raise DeepMemoryWaitingListError()
+        return func(self, *args, **kwargs)
+
+    return wrapper
+
+
 class Relevance(BaseModel):
     data: List[List[Tuple[str, int]]]
 
 
 class Queries(BaseModel):
     data: List[str]
 
@@ -52,51 +74,59 @@
     except ValidationError:
         raise IncorrectQueriesTypeError()
 
 
 class DeepMemory:
     def __init__(
         self,
-        dataset: Dataset,
-        client: DeepMemoryBackendClient,
+        dataset_or_path: Union[Dataset, str],
         logger: logging.Logger,
         embedding_function: Optional[Any] = None,
         token: Optional[str] = None,
-        creds: Optional[Dict[str, Any]] = None,
+        creds: Optional[Union[Dict, str]] = None,
     ):
         """Based Deep Memory class to train and evaluate models on DeepMemory managed service.
 
         Args:
-            dataset (Dataset): deeplake dataset object.
-            client (DeepMemoryBackendClient): Client to interact with the DeepMemory managed service. Defaults to None.
+            dataset_or_path (Union[Dataset, str]): deeplake dataset object or path.
             logger (logging.Logger): Logger object.
             embedding_function (Optional[Any], optional): Embedding funtion class used to convert queries/documents to embeddings. Defaults to None.
             token (Optional[str], optional): API token for the DeepMemory managed service. Defaults to None.
             creds (Optional[Dict[str, Any]], optional): Credentials to access the dataset. Defaults to None.
 
         Raises:
             ImportError: if indra is not installed
+            ValueError: if incorrect type is specified for `dataset_or_path`
         """
+        if isinstance(dataset_or_path, Dataset):
+            self.path = dataset_or_path.path
+        elif isinstance(dataset_or_path, str):
+            self.path = dataset_or_path
+        else:
+            raise ValueError(
+                "dataset_or_path should be a Dataset object or a string path"
+            )
+
         feature_report_path(
-            path=dataset.path,
+            path=self.path,
             feature_name="dm.initialize",
             parameters={
                 "embedding_function": True if embedding_function is not None else False,
-                "client": client,
                 "token": token,
             },
             token=token,
         )
-        self.dataset = dataset
+
         self.token = token
         self.embedding_function = embedding_function
-        self.client = client
+        self.client = self._get_dm_client()
         self.creds = creds or {}
         self.logger = logger
 
+    @access_control
     def train(
         self,
         queries: List[str],
         relevance: List[List[Tuple[str, int]]],
         embedding_function: Optional[Callable[[str], np.ndarray]] = None,
         token: Optional[str] = None,
     ) -> str:
@@ -119,30 +149,31 @@
 
         Returns:
             str: job_id of the training job.
 
         Raises:
             ValueError: if embedding_function is not specified either during initialization or during training.
         """
+        from deeplake.core.vectorstore.deeplake_vectorstore import VectorStore
+
         self.logger.info("Starting DeepMemory training job")
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.train",
             parameters={
                 "queries": queries,
                 "relevance": relevance,
                 "embedding_function": embedding_function,
             },
             token=token or self.token,
         )
-
         validate_relevance_and_queries(relevance=relevance, queries=queries)
 
         # TODO: Support for passing query_embeddings directly without embedding function
-        corpus_path = self.dataset.path
+        corpus_path = self.path
         queries_path = corpus_path + "_queries"
 
         if embedding_function is None and self.embedding_function is None:
             raise ValueError(
                 "Embedding function should be specifed either during initialization or during training."
             )
 
@@ -179,58 +210,61 @@
         )
 
         self.logger.info(
             f"DeepMemory training job started. Job ID: {response['job_id']}"
         )
         return response["job_id"]
 
+    @access_control
     def cancel(self, job_id: str):
         """Cancel a training job on DeepMemory managed service.
 
         Examples:
             >>> cancelled: bool = vectorstore.deep_memory.cancel(job_id)
 
         Args:
             job_id (str): job_id of the training job.
 
         Returns:
             bool: True if job was cancelled successfully, False otherwise.
         """
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.cancel",
             parameters={
                 "job_id": job_id,
             },
             token=self.token,
         )
         return self.client.cancel_job(job_id=job_id)
 
+    @access_control
     def delete(self, job_id: str):
         """Delete a training job on DeepMemory managed service.
 
         Examples:
             >>> deleted: bool = vectorstore.deep_memory.delete(job_id)
 
         Args:
             job_id (str): job_id of the training job.
 
         Returns:
             bool: True if job was deleted successfully, False otherwise.
         """
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.delete",
             parameters={
                 "job_id": job_id,
             },
             token=self.token,
         )
         return self.client.delete_job(job_id=job_id)
 
+    @access_control
     def status(self, job_id: str):
         """Get the status of a training job on DeepMemory managed service.
 
         Examples:
             >>> vectorstore.deep_memory.status(job_id)
             --------------------------------------------------------------
             |                  6508464cd80cab681bfcfff3                  |
@@ -242,28 +276,28 @@
             | results                    | not available yet             |
             --------------------------------------------------------------
 
         Args:
             job_id (str): job_id of the training job.
         """
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.status",
             parameters={
                 "job_id": job_id,
             },
             token=self.token,
         )
 
         _, storage = get_storage_and_cache_chain(
-            path=self.dataset.path,
+            path=self.path,
             db_engine={"tensor_db": True},
             read_only=False,
             creds=self.creds,
-            token=self.dataset.token,
+            token=self.token,
             memory_cache_size=DEFAULT_MEMORY_CACHE_SIZE,
             local_cache_size=DEFAULT_LOCAL_CACHE_SIZE,
         )
 
         loaded_dataset = DeepLakeCloudDataset(storage=storage)
 
         try:
@@ -274,37 +308,38 @@
             recall = "{:.2f}".format(100 * recall)
             improvement = "{:.2f}".format(100 * improvement)
         except:
             recall = None
             improvement = None
         self.client.check_status(job_id=job_id, recall=recall, improvement=improvement)
 
+    @access_control
     def list_jobs(self, debug=False):
         """List all training jobs on DeepMemory managed service."""
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.list_jobs",
             parameters={
                 "debug": debug,
             },
             token=self.token,
         )
         _, storage = get_storage_and_cache_chain(
-            path=self.dataset.path,
+            path=self.path,
             db_engine={"tensor_db": True},
             read_only=False,
             creds=self.creds,
-            token=self.dataset.token,
+            token=self.token,
             memory_cache_size=DEFAULT_MEMORY_CACHE_SIZE,
             local_cache_size=DEFAULT_LOCAL_CACHE_SIZE,
         )
         loaded_dataset = DeepLakeCloudDataset(storage=storage)
 
         response = self.client.list_jobs(
-            dataset_path=self.dataset.path,
+            dataset_path=self.path,
         )
 
         response_status_schema = JobResponseStatusSchema(response=response)
 
         jobs = self._get_jobs(response)
         if jobs is None:
             reposnse_str = "No Deep Memory training jobs were found for this dataset"
@@ -334,14 +369,15 @@
             deltas[f"{job}"] = delta
 
         reposnse_str = response_status_schema.print_jobs(
             debug=debug, recalls=recalls, improvements=deltas
         )
         return reposnse_str
 
+    @access_control
     def evaluate(
         self,
         relevance: List[List[Tuple[str, int]]],
         queries: List[str],
         embedding_function: Optional[Callable[..., List[np.ndarray]]] = None,
         embedding: Optional[Union[List[np.ndarray], List[List[float]]]] = None,
         top_k: List[int] = [1, 3, 5, 10, 50, 100],
@@ -403,63 +439,63 @@
         Returns:
             Dict[str, Dict[str, float]]: Recalls for each rank.
 
         Raises:
             ImportError: If `indra` is not installed.
             ValueError: If no embedding_function is provided either during initialization or evaluation.
         """
-
         feature_report_path(
-            path=self.dataset.path,
+            path=self.path,
             feature_name="dm.evaluate",
             parameters={
                 "relevance": relevance,
                 "queries": queries,
                 "embedding_function": embedding_function,
                 "embedding": embedding,
                 "top_k": top_k,
                 "qvs_params": qvs_params,
             },
             token=self.token,
         )
-        try_flushing(self.dataset)
+
         try:
             from indra import api  # type: ignore
 
             INDRA_INSTALLED = True
         except Exception:
             INDRA_INSTALLED = False
 
         if not INDRA_INSTALLED:
             raise ImportError(
-                "The C++ library is not installed. The library should be installed using `pip install deeplake`, but if you want to install it separately, you may run `pip install libdeeplake`"
+                "indra is not installed. Please install indra to use this functionality with: pip install `deeplake[enterprise]`"
             )
 
+        validate_relevance_and_queries(relevance=relevance, queries=queries)
+
         from indra import api  # type: ignore
 
-        indra_dataset = api.dataset(self.dataset.path, token=self.token)
+        indra_dataset = api.dataset(self.path, token=self.token)
         api.tql.prepare_deepmemory_metrics(indra_dataset)
 
         parsed_qvs_params = parse_queries_params(qvs_params)
-        validate_relevance_and_queries(relevance=relevance, queries=queries)
 
         start = time()
         query_embs: Union[List[np.ndarray], List[List[float]]]
 
         if embedding is not None:
             query_embs = embedding
         else:
             if self.embedding_function is not None:
                 embedding_function = (
                     embedding_function or self.embedding_function.embed_documents
                 )
 
             if embedding_function is None:
                 raise ValueError(
-                    "Embedding function should be specified either during initialization or during evaluation."
+                    "Embedding function should be specifed either during initialization or during evaluation."
                 )
             query_embs = embedding_function(queries)
 
         print(f"Embedding queries took {time() - start:.2f} seconds")
 
         recalls: Dict[str, Dict] = {"with model": {}, "without model": {}}
         queries_data = {
@@ -494,15 +530,15 @@
         log_queries = parsed_qvs_params.get("log_queries")
         branch = parsed_qvs_params.get("branch")
 
         if log_queries == False:
             return recalls
 
         self.queries_dataset = deeplake.empty(
-            self.dataset.path + "_eval_queries",
+            self.path + "_eval_queries",
             token=self.token,
             creds=self.creds,
             overwrite=True,
         )
 
         if len(self.queries_dataset) == 0:
             self.queries_dataset.commit(allow_empty=True)
@@ -514,14 +550,33 @@
             if tensor_params["name"] not in self.queries_dataset.tensors:
                 self.queries_dataset.create_tensor(**tensor_params)
 
         self.queries_dataset.extend(queries_data, progressbar=True)
         self.queries_dataset.commit()
         return recalls
 
+    def _get_dm_client(self):
+        path = self.path
+        path_type = get_path_type(path)
+
+        dm_client = DeepMemoryBackendClient(token=self.token)
+        user_profile = dm_client.get_user_profile()
+
+        if path_type == "hub":
+            # TODO: add support for windows
+            dataset_id = path[6:].split("/")[0]
+        else:
+            # TODO: change user_profile to user_id
+            dataset_id = user_profile["name"]
+
+        deepmemory_is_available = dm_client.deepmemory_is_available(dataset_id)
+        if deepmemory_is_available:
+            return dm_client
+        return None
+
     def _get_jobs(self, response):
         jobs = None
         if response is not None and len(response) > 0:
             jobs = [job["id"] for job in response]
         return jobs
 
 
@@ -624,19 +679,16 @@
 
 
 def _get_best_model(embedding: Any, job_id: str, latest_job: bool = False):
     info = embedding.info
     best_recall = 0
     best_delta = 0
     if latest_job:
-        try:
-            best_recall = info["deepmemory/model.npy"]["recall@10"]
-            best_delta = info["deepmemory/model.npy"]["delta"]
-        except KeyError:
-            pass
+        best_recall = info["deepmemory/model.npy"]["recall@10"]
+        best_delta = info["deepmemory/model.npy"]["delta"]
 
     for job, value in info.items():
         if job_id in job:
             recall = value["recall@10"]
             delta = value["delta"]
             if delta > best_delta:
                 best_recall = recall
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.8.9/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 import logging
 import pathlib
 from typing import Optional, Any, List, Dict, Union, Callable
-import jwt
 
 import numpy as np
 
 import deeplake
-from deeplake.core import index_maintenance
-from deeplake.core.distance_type import DistanceType
-from deeplake.util.exceptions import DeepMemoryWaitingListError
-from deeplake.util.path import convert_pathlib_to_string_if_needed
-
-from deeplake.api import dataset
 from deeplake.core.dataset import Dataset
+from deeplake.core.vectorstore.dataset_handlers import get_dataset_handler
+from deeplake.core.vectorstore.deep_memory import DeepMemory
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_TENSORS,
     MAX_BYTES_PER_MINUTE,
     TARGET_BYTE_SIZE,
-    DEFAULT_VECTORSTORE_DISTANCE_METRIC,
-    DEFAULT_DEEPMEMORY_DISTANCE_METRIC,
-    _INDEX_OPERATION_MAPPING,
 )
-from deeplake.client.utils import read_token
-from deeplake.core.vectorstore import utils
-from deeplake.core.vectorstore.vector_search import vector_search
-from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
-from deeplake.core.vectorstore.vector_search import filter as filter_utils
-from deeplake.util.bugout_reporter import (
-    feature_report_path,
-)
-from deeplake.util.path import get_path_type
-from deeplake.core.vectorstore.unsupported_deep_memory import DeepMemory
+from deeplake.util.bugout_reporter import feature_report_path
+from deeplake.util.exceptions import DeepMemoryWaitingListError
 
 
 logger = logging.getLogger(__name__)
 
 
 class VectorStore:
     """Base class for VectorStore"""
 
     def __init__(
         self,
-        path: Union[str, pathlib.Path],
+        path: Optional[Union[str, pathlib.Path]] = None,
+        dataset: Optional[Dataset] = None,
         tensor_params: List[Dict[str, object]] = DEFAULT_VECTORSTORE_TENSORS,
         embedding_function: Optional[Any] = None,
         read_only: Optional[bool] = None,
         ingestion_batch_size: int = 1000,
         index_params: Optional[Dict[str, Union[int, str]]] = None,
         num_workers: int = 0,
         exec_option: str = "auto",
@@ -120,95 +105,43 @@
 
         ..
             # noqa: DAR101
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if the Vector Store exists! Be very careful when setting this parameter.
         """
-        try:
-            from indra import api  # type: ignore
-
-            self.indra_installed = True
-        except Exception:  # pragma: no cover
-            self.indra_installed = False  # pragma: no cover
-
-        self._token = token
-        self.path = convert_pathlib_to_string_if_needed(path)
-        self.logger = logger
-        self.org_id = org_id if get_path_type(self.path) == "local" else None
-
-        feature_report_path(
-            path,
-            "vs.initialize",
-            {
-                "tensor_params": "default"
-                if tensor_params is not None
-                else tensor_params,
-                "embedding_function": True if embedding_function is not None else False,
-                "num_workers": num_workers,
-                "overwrite": overwrite,
-                "read_only": read_only,
-                "ingestion_batch_size": ingestion_batch_size,
-                "index_params": index_params,
-                "exec_option": exec_option,
-                "token": self.token,
-                "verbose": verbose,
-                "runtime": runtime,
-            },
-            token=self.token,
-            username=self.username,
-        )
-
-        self.ingestion_batch_size = ingestion_batch_size
-        self.index_params = utils.parse_index_params(index_params)
-        kwargs["index_params"] = self.index_params
-        self.num_workers = num_workers
-        self.creds = creds or {}
-        self.embedding_function = utils.create_embedding_function(embedding_function)
-
-        self.dataset = dataset_utils.create_or_load_dataset(
-            tensor_params,
-            path,
-            self.token,
-            self.creds,
-            self.logger,
-            read_only,
-            exec_option,
-            embedding_function,
-            overwrite,
-            runtime,
-            self.org_id,
-            branch,
+        self.dataset_handler = get_dataset_handler(
+            path=path,
+            dataset=dataset,
+            tensor_params=tensor_params,
+            embedding_function=embedding_function,
+            read_only=read_only,
+            ingestion_batch_size=ingestion_batch_size,
+            index_params=index_params,
+            num_workers=num_workers,
+            exec_option=exec_option,
+            token=token,
+            overwrite=overwrite,
+            verbose=verbose,
+            runtime=runtime,
+            creds=creds,
+            org_id=org_id,
+            logger=logger,
+            branch=branch,
             **kwargs,
         )
-        self._exec_option = exec_option
-        self.verbose = verbose
-        self.tensor_params = tensor_params
-        self.distance_metric_index = index_maintenance.index_operation_vectorstore(
-            self,
-        )
-        self.deep_memory = DeepMemory()
-
-    @property
-    def token(self):
-        return self._token or read_token(from_env=True)
 
-    @property
-    def exec_option(self) -> str:
-        return utils.parse_exec_option(
-            self.dataset, self._exec_option, self.indra_installed, self.username
+        self.deep_memory = DeepMemory(
+            dataset_or_path=self.dataset_handler.path,
+            token=self.dataset_handler.token,
+            logger=logger,
+            embedding_function=embedding_function,
+            creds=self.dataset_handler.creds,
         )
 
-    @property
-    def username(self) -> str:
-        username = "public"
-        if self.token is not None:
-            username = jwt.decode(self.token, options={"verify_signature": False})["id"]
-        return username
-
     def add(
         self,
         embedding_function: Optional[Union[Callable, List[Callable]]] = None,
         embedding_data: Optional[Union[List, List[List]]] = None,
         embedding_tensor: Optional[Union[str, List[str]]] = None,
         return_ids: bool = False,
         rate_limiter: Dict = {
@@ -280,77 +213,23 @@
             return_ids (bool): Whether to return added ids as an ouput of the method. Defaults to False.
             rate_limiter (Dict): Rate limiter configuration. Defaults to ``{"enabled": False, "bytes_per_minute": MAX_BYTES_PER_MINUTE, "batch_byte_size": TARGET_BYTE_SIZE}``.
             **tensors: Keyword arguments where the key is the tensor name, and the value is a list of samples that should be uploaded to that tensor.
 
         Returns:
             Optional[List[str]]: List of ids if ``return_ids`` is set to True. Otherwise, None.
         """
-
-        feature_report_path(
-            path=self.path,
-            feature_name="vs.add",
-            parameters={
-                "tensors": list(tensors.keys()) if tensors else None,
-                "embedding_tensor": embedding_tensor,
-                "return_ids": return_ids,
-                "embedding_function": True if embedding_function is not None else False,
-                "embedding_data": True if embedding_data is not None else False,
-            },
-            token=self.token,
-            username=self.username,
-        )
-        (
-            embedding_function,
-            embedding_data,
-            embedding_tensor,
-            tensors,
-        ) = utils.parse_tensors_kwargs(
-            tensors,
-            embedding_function,
-            embedding_data,
-            embedding_tensor,
-        )
-
-        (
-            embedding_function,
-            embedding_data,
-            embedding_tensor,
-            tensors,
-        ) = utils.parse_add_arguments(
-            dataset=self.dataset,
-            initial_embedding_function=self.embedding_function,
-            embedding_function=embedding_function,
-            embedding_data=embedding_data,
-            embedding_tensor=embedding_tensor,
-            **tensors,
-        )
-
-        processed_tensors, id_ = dataset_utils.preprocess_tensors(
-            embedding_data, embedding_tensor, self.dataset, **tensors
-        )
-
-        assert id_ is not None
-
-        dataset_utils.extend_or_ingest_dataset(
-            processed_tensors=processed_tensors,
-            dataset=self.dataset,
+        return self.dataset_handler.add(
             embedding_function=embedding_function,
             embedding_data=embedding_data,
             embedding_tensor=embedding_tensor,
+            return_ids=return_ids,
             rate_limiter=rate_limiter,
-            logger=self.logger,
+            **tensors,
         )
 
-        if self.verbose:
-            self.dataset.summary()
-
-        if return_ids:
-            return id_
-        return None
-
     def search(
         self,
         embedding_data: Union[str, List[str], None] = None,
         embedding_function: Optional[Callable] = None,
         embedding: Optional[Union[List[float], np.ndarray]] = None,
         k: int = 4,
         distance_metric: Optional[str] = None,
@@ -419,100 +298,35 @@
             ValueError: When invalid parameters are specified.
             ValueError: when deep_memory is True. Deep Memory is only available for datasets stored in the Deep Lake Managed Database for paid accounts.
             DeepMemoryWaitingListError: if user is not waitlisted to use deep_memory.
 
         Returns:
             Dict: Dictionary where keys are tensor names and values are the results of the search
         """
-
-        feature_report_path(
-            path=self.path,
-            feature_name="vs.search",
-            parameters={
-                "embedding_data": True if embedding_data is not None else False,
-                "embedding_function": True if embedding_function is not None else False,
-                "k": k,
-                "distance_metric": distance_metric,
-                "query": query[0:100] if query is not None else False,
-                "filter": True if filter is not None else False,
-                "exec_option": exec_option,
-                "embedding_tensor": embedding_tensor,
-                "embedding": True if embedding is not None else False,
-                "return_tensors": return_tensors,
-                "return_view": return_view,
-            },
-            token=self.token,
-            username=self.username,
-        )
-
-        if exec_option is None and self.exec_option != "python" and callable(filter):
-            self.logger.warning(
-                'Switching exec_option to "python" (runs on client) because filter is specified as a function. '
-                f'To continue using the original exec_option "{self.exec_option}", please specify the filter as a dictionary or use the "query" parameter to specify a TQL query.'
-            )
-            exec_option = "python"
-
-        exec_option = exec_option or self.exec_option
-
         if deep_memory and not self.deep_memory:
             raise DeepMemoryWaitingListError()
 
-        utils.parse_search_args(
+        return self.dataset_handler.search(
             embedding_data=embedding_data,
             embedding_function=embedding_function,
-            initial_embedding_function=self.embedding_function,
             embedding=embedding,
             k=k,
             distance_metric=distance_metric,
             query=query,
             filter=filter,
             exec_option=exec_option,
             embedding_tensor=embedding_tensor,
             return_tensors=return_tensors,
-        )
-
-        return_tensors = utils.parse_return_tensors(
-            self.dataset, return_tensors, embedding_tensor, return_view
-        )
-        embedding_function = utils.create_embedding_function(embedding_function)
-        query_emb: Optional[Union[List[float], np.ndarray[Any, Any]]] = None
-        if query is None:
-            query_emb = dataset_utils.get_embedding(
-                embedding,
-                embedding_data,
-                embedding_function=embedding_function or self.embedding_function,
-            )
-
-        if self.distance_metric_index:
-            distance_metric = index_maintenance.parse_index_distance_metric_from_params(
-                logger, self.distance_metric_index, distance_metric
-            )
-
-        distance_metric = distance_metric or DEFAULT_VECTORSTORE_DISTANCE_METRIC
-
-        return vector_search.search(
-            query=query,
-            logger=self.logger,
-            filter=filter,
-            query_embedding=query_emb,
-            k=k,
-            distance_metric=distance_metric,
-            exec_option=exec_option,
-            deeplake_dataset=self.dataset,
-            embedding_tensor=embedding_tensor,
-            return_tensors=return_tensors,
             return_view=return_view,
             deep_memory=deep_memory,
-            token=self.token,
-            org_id=self.org_id,
         )
 
     def delete(
         self,
-        row_ids: Optional[List[str]] = None,
+        row_ids: Optional[List[int]] = None,
         ids: Optional[List[str]] = None,
         filter: Optional[Union[Dict, Callable]] = None,
         query: Optional[str] = None,
         exec_option: Optional[str] = None,
         delete_all: Optional[bool] = None,
     ) -> bool:
         """Delete the data in the Vector Store. Does not delete the tensor definitions. To delete the vector store completely, first run :meth:`VectorStore.delete_by_path()`.
@@ -528,15 +342,15 @@
             >>> data = vector_store.delete(
             ...        query = "select * where ..... <add TQL syntax>",
             ...        exec_option = "compute_engine",
             ... )
 
         Args:
             ids (Optional[List[str]]): List of unique ids. Defaults to None.
-            row_ids (Optional[List[str]]): List of absolute row indices from the dataset. Defaults to None.
+            row_ids (Optional[List[int]]): List of absolute row indices from the dataset. Defaults to None.
             filter (Union[Dict, Callable], optional): Filter for finding samples for deletion.
                 - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
                 - ``Function`` - Any function that is compatible with `deeplake.filter`.
             query (Optional[str]):  TQL Query string for direct evaluation for finding samples for deletion, without application of additional filters.
             exec_option (Optional[str]): Method for search execution. It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``None``, which inherits the option from the Vector Store initialization.
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
@@ -549,55 +363,23 @@
         Returns:
             bool: Returns True if deletion was successful, otherwise it raises a ValueError.
 
         Raises:
             ValueError: If neither ``ids``, ``filter``, ``query``, nor ``delete_all`` are specified, or if an invalid ``exec_option`` is provided.
         """
 
-        feature_report_path(
-            path=self.path,
-            feature_name="vs.delete",
-            parameters={
-                "ids": True if ids is not None else False,
-                "row_ids": True if row_ids is not None else False,
-                "query": query[0:100] if query is not None else False,
-                "filter": True if filter is not None else False,
-                "exec_option": exec_option,
-                "delete_all": delete_all,
-            },
-            token=self.token,
-            username=self.username,
-        )
-
-        if not row_ids:
-            row_ids = (
-                dataset_utils.search_row_ids(
-                    dataset=self.dataset,
-                    search_fn=self.search,
-                    ids=ids,
-                    filter=filter,
-                    query=query,
-                    select_all=delete_all,
-                    exec_option=exec_option or self.exec_option,
-                )
-                or []
-            )
-
-        (
-            self.dataset,
-            dataset_deleted,
-        ) = dataset_utils.delete_all_samples_if_specified(
-            self.dataset,
-            delete_all,
+        return self.dataset_handler.delete(
+            row_ids=row_ids,
+            ids=ids,
+            filter=filter,
+            query=query,
+            exec_option=exec_option,
+            delete_all=delete_all,
         )
 
-        self.dataset.pop_multiple(row_ids)
-
-        return True
-
     def update_embedding(
         self,
         row_ids: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         filter: Optional[Union[Dict, Callable]] = None,
         query: Optional[str] = None,
         exec_option: Optional[str] = None,
@@ -646,60 +428,25 @@
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"tensor_db": True} during dataset creation.
             embedding_function (Optional[Union[Callable, List[Callable]]], optional): function for converting `embedding_source_tensor` into embedding. Only valid if `embedding_source_tensor` is specified. Defaults to None.
             embedding_source_tensor (Union[str, List[str]], optional): Name of tensor with data that needs to be converted to embeddings. Defaults to `text`.
             embedding_tensor (Optional[Union[str, List[str]]], optional): Name of the tensor with embeddings. Defaults to None.
         """
-        feature_report_path(
-            path=self.path,
-            feature_name="vs.delete",
-            parameters={
-                "ids": True if ids is not None else False,
-                "row_ids": True if row_ids is not None else False,
-                "query": query[0:100] if query is not None else False,
-                "filter": True if filter is not None else False,
-                "exec_option": exec_option,
-            },
-            token=self.token,
-            username=self.username,
-        )
-
-        (
-            embedding_function,
-            embedding_source_tensor,
-            embedding_tensor,
-        ) = utils.parse_update_arguments(
-            dataset=self.dataset,
+        self.dataset_handler.update_embedding(
+            row_ids=row_ids,
+            ids=ids,
+            filter=filter,
+            query=query,
+            exec_option=exec_option,
             embedding_function=embedding_function,
-            initial_embedding_function=self.embedding_function,
-            embedding_source_tensor=embedding_source_tensor,
-            embedding_tensor=embedding_tensor,
-        )
-
-        if not row_ids:
-            row_ids = dataset_utils.search_row_ids(
-                dataset=self.dataset,
-                search_fn=self.search,
-                ids=ids,
-                filter=filter,
-                query=query,
-                exec_option=exec_option or self.exec_option,
-            )
-
-        embedding_tensor_data = utils.convert_embedding_source_tensor_to_embeddings(
-            dataset=self.dataset,
             embedding_source_tensor=embedding_source_tensor,
             embedding_tensor=embedding_tensor,
-            embedding_function=embedding_function,
-            row_ids=row_ids,
         )
 
-        self.dataset[row_ids].update(embedding_tensor_data)
-
     @staticmethod
     def delete_by_path(
         path: Union[str, pathlib.Path],
         token: Optional[str] = None,
         force: bool = False,
         creds: Optional[Union[Dict, str]] = None,
     ) -> None:
@@ -713,16 +460,14 @@
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             force (bool): delete the path in a forced manner without rising an exception. Defaults to ``True``.
 
         Danger:
             This method permanently deletes all of your data if the Vector Store exists! Be very careful when using this method.
         """
-        token = token or read_token(from_env=True)
-
         feature_report_path(
             path,
             "vs.delete_by_path",
             parameters={
                 "path": path,
                 "token": token,
                 "force": force,
@@ -734,31 +479,42 @@
 
     def commit(self, allow_empty: bool = True) -> None:
         """Commits the Vector Store.
 
         Args:
             allow_empty (bool): Whether to allow empty commits. Defaults to True.
         """
-        self.dataset.commit(allow_empty=allow_empty)
+        self.dataset_handler.commit(allow_empty=allow_empty)
 
-    def checkout(self, branch: str = "main") -> None:
+    def checkout(self, branch: str = "main", create=False) -> None:
         """Checkout the Vector Store to a specific branch.
 
         Args:
             branch (str): Branch name to checkout. Defaults to "main".
+            create (bool): Whether to create the branch if it doesn't exist. Defaults to False.
         """
-        self.dataset.checkout(branch)
+        self.dataset_handler.checkout(branch, create=create)
 
     def tensors(self):
         """Returns the list of tensors present in the dataset"""
-        return self.dataset.tensors
+        return self.dataset_handler.tensors()
 
     def summary(self):
         """Prints a summary of the dataset"""
-        return self.dataset.summary()
+        return self.dataset_handler.summary()
+
+    @property
+    def dataset(self):
+        """Returns the dataset"""
+        try:
+            return self.dataset_handler.dataset
+        except AttributeError:
+            raise AttributeError(
+                "Acessing the dataset is not available for managed Vector Store."
+            )
 
     def __len__(self):
         """Length of the dataset"""
-        return len(self.dataset)
+        return len(self.dataset_handler)
 
 
 DeepLakeVectorStore = VectorStore
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/deepmemory_vectorstore.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Dict, Union, Callable
 
-import numpy as np
-
-from deeplake.core.dataset import Dataset
-from deeplake.core.vectorstore.deeplake_vectorstore import VectorStore
-from deeplake.core.vectorstore.deep_memory import DeepMemory
-from deeplake.constants import DEFAULT_DEEPMEMORY_DISTANCE_METRIC
-
-
-class DeepMemoryVectorStore(VectorStore):
-    def __init__(self, client, *arg, **kwargs):
-        super().__init__(*arg, **kwargs)
-        self.deep_memory = DeepMemory(
-            self.dataset,
-            token=self.token,
-            embedding_function=self.embedding_function,
-            client=client,
-            creds=self.creds,
-            logger=self.logger,
+from deeplake.core.dataset import Dataset as DeepLakeDataset
+from deeplake.core.vectorstore.vector_search import utils
+from deeplake.core.vectorstore.vector_search import filter as filter_utils
+from deeplake.core import vectorstore
+
+
+def vector_search(
+    query,
+    query_emb,
+    exec_option,
+    dataset,
+    logger,
+    filter,
+    embedding_tensor,
+    distance_metric,
+    k,
+    return_tensors,
+    return_view,
+    deep_memory,
+    token,
+    org_id,
+) -> Union[Dict, DeepLakeDataset]:
+    try:
+        from indra import api  # type: ignore
+
+        _INDRA_INSTALLED = True  # pragma: no cover
+    except ImportError:  # pragma: no cover
+        _INDRA_INSTALLED = False  # pragma: no cover
+
+    runtime = utils.get_runtime_from_exec_option(exec_option)
+
+    if callable(filter):
+        raise ValueError(
+            f"UDF filter functions are not supported with the current `exec_option`={exec_option}. "
         )
 
-    def search(
-        self,
-        embedding_data: Union[str, List[str], None] = None,
-        embedding_function: Optional[Callable] = None,
-        embedding: Optional[Union[List[float], np.ndarray]] = None,
-        k: int = 4,
-        distance_metric: Optional[str] = None,
-        query: Optional[str] = None,
-        filter: Optional[Union[Dict, Callable]] = None,
-        exec_option: Optional[str] = None,
-        embedding_tensor: str = "embedding",
-        return_tensors: Optional[List[str]] = None,
-        return_view: bool = False,
-        deep_memory: bool = False,
-    ) -> Union[Dict, Dataset]:
-        if deep_memory and not distance_metric:
-            distance_metric = DEFAULT_DEEPMEMORY_DISTANCE_METRIC
-
-        return super().search(
-            embedding_data=embedding_data,
-            embedding_function=embedding_function,
-            embedding=embedding,
-            k=k,
-            distance_metric=distance_metric,
-            query=query,
-            filter=filter,
-            exec_option=exec_option,
-            embedding_tensor=embedding_tensor,
-            return_tensors=return_tensors,
-            return_view=return_view,
-            deep_memory=deep_memory,
-        )
+    utils.check_indra_installation(exec_option, indra_installed=_INDRA_INSTALLED)
+
+    view, tql_filter = filter_utils.attribute_based_filtering_tql(
+        view=dataset,
+        filter=filter,
+        logger=logger,
+    )
+
+    return vectorstore.indra_search_algorithm(
+        query_embedding=query_emb,
+        distance_metric=distance_metric.lower(),
+        deeplake_dataset=view,
+        k=k,
+        tql_string=query,
+        tql_filter=tql_filter,
+        embedding_tensor=embedding_tensor,
+        runtime=runtime,
+        return_tensors=return_tensors,
+        return_view=return_view,
+        deep_memory=deep_memory,
+        token=token,
+        org_id=org_id,
+    )
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/embedder.py` & `deeplake-3.8.9/deeplake/core/vectorstore/embeddings/embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.8.9/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import uuid
 import os
 import sys
 from math import isclose
 from functools import partial
 from typing import List
+from unittest.mock import patch
 
 import numpy as np
 import pytest
 
 import deeplake
 from deeplake.core.vectorstore.deeplake_vectorstore import (
     DeepLakeVectorStore,
     VectorStore,
 )
-from deeplake.core.vectorstore.deepmemory_vectorstore import DeepMemoryVectorStore
-from deeplake.core.vectorstore.embedder import DeepLakeEmbedder
-from deeplake.core.vectorstore.vectorstore_factory import vectorstore_factory
+from deeplake.core.vectorstore.embeddings.embedder import DeepLakeEmbedder
 from deeplake.core.vectorstore import utils
 from deeplake.tests.common import requires_libdeeplake
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_TENSORS,
     DEFAULT_VECTORSTORE_DISTANCE_METRIC,
 )
 from deeplake.constants import MB
@@ -82,15 +81,15 @@
 
 
 def embedding_function(embedding_value, text):
     """Embedding function with custom embedding values"""
     return [np.ones(EMBEDDING_DIM) * embedding_value for _ in range(len(text))]
 
 
-def get_embedding_function(embedding_value):
+def get_embedding_function(embedding_value=100):
     """Function for creation embedding function with given embedding value"""
     return partial(embedding_function, embedding_value)
 
 
 def get_multiple_embedding_function(embedding_value, num_of_funcs=2):
     return [
         partial(embedding_function, embedding_value[i]) for i in range(num_of_funcs)
@@ -257,15 +256,15 @@
     # Initialize vector store object and add data
     vector_store = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
         token=hub_cloud_dev_token,
     )
 
-    assert vector_store.exec_option == "compute_engine"
+    assert vector_store.dataset_handler.exec_option == "compute_engine"
 
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
 
     with pytest.raises(IncorrectEmbeddingShapeError):
         vector_store.add(
             embedding_function=embedding_fn2,
             embedding_data=texts,
@@ -283,105 +282,133 @@
         k=2,
         return_tensors=["id", "text"],
         filter={"metadata": {"abc": 1}},
     )
 
     assert len(data_p["text"]) == 1
     assert (
-        sum([tensor in data_p.keys() for tensor in vector_store.dataset.tensors]) == 2
+        sum(
+            [
+                tensor in data_p.keys()
+                for tensor in vector_store.dataset_handler.dataset.tensors
+            ]
+        )
+        == 2
     )  # One for each return_tensors
     assert len(data_p.keys()) == 3  # One for each return_tensors + score
 
     # Load a vector store object from the cloud for indra testing
     vector_store_cloud = DeepLakeVectorStore(
         path="hub://testingacc2/vectorstore_test",
         read_only=True,
         token=hub_cloud_dev_token,
     )
-    assert vector_store_cloud.exec_option == "compute_engine"
+    assert vector_store_cloud.dataset_handler.exec_option == "compute_engine"
 
     # Use indra implementation to search the data
     data_ce = vector_store_cloud.search(
         embedding=query_embedding,
         k=2,
         return_tensors=["id", "text"],
     )
     assert len(data_ce["text"]) == 2
     assert (
-        sum([tensor in data_ce.keys() for tensor in vector_store_cloud.dataset.tensors])
+        sum(
+            [
+                tensor in data_ce.keys()
+                for tensor in vector_store_cloud.dataset_handler.dataset.tensors
+            ]
+        )
         == 2
     )  # One for each return_tensors
     assert len(data_ce.keys()) == 3  # One for each return_tensors + score
 
     with pytest.raises(ValueError):
         vector_store_cloud.search(
-            query=f"SELECT * WHERE id=='{vector_store_cloud.dataset.id[0].numpy()[0]}'",
+            query=f"SELECT * WHERE id=='{vector_store_cloud.dataset_handler.dataset.id[0].numpy()[0]}'",
             embedding=query_embedding,
             k=2,
             return_tensors=["id", "text"],
         )
 
     # Run a full custom query
-    test_text = vector_store_cloud.dataset.text[0].data()["value"]
+    test_text = vector_store_cloud.dataset_handler.dataset.text[0].data()["value"]
     data_q = vector_store_cloud.search(
         query=f"select * where text == '{test_text}'",
     )
 
     assert len(data_q["text"]) == 1
     assert data_q["text"][0] == test_text
     assert sum(
-        [tensor in data_q.keys() for tensor in vector_store_cloud.dataset.tensors]
+        [
+            tensor in data_q.keys()
+            for tensor in vector_store_cloud.dataset_handler.dataset.tensors
+        ]
     ) == len(
-        vector_store_cloud.dataset.tensors
+        vector_store_cloud.dataset_handler.dataset.tensors
     )  # One for each tensor - embedding + score
 
     # Run a filter query using a json
     data_e_j = vector_store.search(
         k=2,
         return_tensors=["id", "text"],
         filter={"metadata": metadatas[2], "text": texts[2]},
     )
     assert len(data_e_j["text"]) == 1
     assert (
-        sum([tensor in data_e_j.keys() for tensor in vector_store.dataset.tensors]) == 2
+        sum(
+            [
+                tensor in data_e_j.keys()
+                for tensor in vector_store.dataset_handler.dataset.tensors
+            ]
+        )
+        == 2
     )  # One for each return_tensors
     assert len(data_e_j.keys()) == 2
 
     # Run the same filter as above using a function
     def filter_fn(x):
         return x["metadata"].data()["value"]["abc"] == 1
 
     data_e_f = vector_store.search(
         k=2,
         return_tensors=["id", "text"],
         filter=filter_fn,
     )
     assert len(data_e_f["text"]) == 1
     assert (
-        sum([tensor in data_e_f.keys() for tensor in vector_store.dataset.tensors]) == 2
+        sum(
+            [
+                tensor in data_e_f.keys()
+                for tensor in vector_store.dataset_handler.dataset.tensors
+            ]
+        )
+        == 2
     )  # One for each return_tensors
     assert len(data_e_f.keys()) == 2
 
     # Run a filter query using a json with indra
     data_ce_f = vector_store_cloud.search(
         embedding=query_embedding,
         exec_option="compute_engine",
         k=2,
         return_tensors=["id", "text"],
         filter={
-            "metadata": vector_store_cloud.dataset.metadata[0].data()["value"],
-            "text": vector_store_cloud.dataset.text[0].data()["value"],
+            "metadata": vector_store_cloud.dataset_handler.dataset.metadata[0].data()[
+                "value"
+            ],
+            "text": vector_store_cloud.dataset_handler.dataset.text[0].data()["value"],
         },
     )
     assert len(data_ce_f["text"]) == 1
     assert (
         sum(
             [
                 tensor in data_ce_f.keys()
-                for tensor in vector_store_cloud.dataset.tensors
+                for tensor in vector_store_cloud.dataset_handler.dataset.tensors
             ]
         )
         == 2
     )  # One for each return_tensors
     assert len(data_ce_f.keys()) == 3  # One for each return_tensors + score
 
     # Check returning views
@@ -413,15 +440,15 @@
     assert data_ce_v.embedding[0].numpy().size > 0
 
     # Check that None option works
     vector_store_none_exec = DeepLakeVectorStore(
         path=local_path, overwrite=True, token=hub_cloud_dev_token, exec_option=None
     )
 
-    assert vector_store_none_exec.exec_option == "compute_engine"
+    assert vector_store_none_exec.dataset_handler.exec_option == "compute_engine"
 
     # Check that filter_fn with cloud dataset (and therefore "compute_engine" exec option) switches to "python" automatically.
     with pytest.warns(None):
         _ = vector_store_cloud.search(
             filter=filter_fn,
         )
 
@@ -466,15 +493,15 @@
             embedding=query_embedding,
             k=2,
             filter={"metadata": {"abc": 1}},
             return_view=True,
         )
 
     vector_store = DeepLakeVectorStore(path="mem://xyz")
-    assert vector_store.exec_option == "python"
+    assert vector_store.dataset_handler.exec_option == "python"
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
 
     data = vector_store.search(
         embedding_function=openai_embeddings.embed_query,
         embedding_data=["dummy"],
         return_view=True,
         k=2,
@@ -520,15 +547,15 @@
     assert len(data["text"]) == 0
     assert len(data["score"]) == 0
 
     # Test that the embedding function during initalization works
     vector_store = DeepLakeVectorStore(
         path="mem://xyz", embedding_function=openai_embeddings
     )
-    assert vector_store.exec_option == "python"
+    assert vector_store.dataset_handler.exec_option == "python"
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
     result = vector_store.search(embedding_data=["dummy"])
     assert len(result) == 4
 
 
 @pytest.mark.slow
 @requires_libdeeplake
@@ -536,49 +563,68 @@
     # Start by testing behavior without an index
     vector_store = VectorStore(
         path=local_path,
         overwrite=True,
         token=hub_cloud_dev_token,
     )
 
-    assert vector_store.distance_metric_index is None
+    assert vector_store.dataset_handler.distance_metric_index is None
 
     # Then test behavior when index is added
     vector_store = VectorStore(
         path=local_path, token=hub_cloud_dev_token, index_params={"threshold": 1}
     )
 
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
-    es = vector_store.dataset.embedding.get_vdb_indexes()
+    es = vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()
 
     assert (
         es[0]["distance"] == METRIC_TO_INDEX_METRIC[DEFAULT_VECTORSTORE_DISTANCE_METRIC]
     )
 
     # Then test behavior when index is added previously and the dataset is reloaded
     vector_store = VectorStore(path=local_path, token=hub_cloud_dev_token)
-    es = vector_store.dataset.embedding.get_vdb_indexes()
+    es = vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()
 
     assert (
         es[0]["distance"] == METRIC_TO_INDEX_METRIC[DEFAULT_VECTORSTORE_DISTANCE_METRIC]
     )
 
     # Test index with sample updates
-    pre_update_index = vector_store.dataset.embedding.get_vdb_indexes()[0]
+    pre_update_index = vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[
+        0
+    ]
     vector_store.add(
         embedding=[embeddings[0]], text=[texts[0]], metadata=[metadatas[0]]
     )
-    post_update_index = vector_store.dataset.embedding.get_vdb_indexes()[0]
+    post_update_index = (
+        vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[0]
+    )
 
     assert pre_update_index == post_update_index
 
+    # Test index with sample deletion
+    pre_delete_index = vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[
+        0
+    ]
+    vector_store.delete(row_ids=[len(vector_store) - 1])
+    post_delete_index = (
+        vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[0]
+    )
+
+    assert pre_delete_index == post_delete_index
+
     # Test index with sample updating
-    pre_update_index = vector_store.dataset.embedding.get_vdb_indexes()[0]
+    pre_update_index = vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[
+        0
+    ]
     vector_store.update_embedding(row_ids=[0], embedding_function=embedding_fn)
-    post_update_index = vector_store.dataset.embedding.get_vdb_indexes()[0]
+    post_update_index = (
+        vector_store.dataset_handler.dataset.embedding.get_vdb_indexes()[0]
+    )
 
     assert pre_update_index == post_update_index
 
     # Check that distance metric throws a warning when there is an index
     with pytest.warns(None):
         vector_store.search(embedding=query_embedding, distance_metric="l1")
 
@@ -640,15 +686,15 @@
         vector_store.search(
             query="select * where metadata == {'abcdefg': 28}",
             exec_option="compute_engine",
             distance_metric=distance_metric,
             filter={"metadata": {"abcdefg": 28}},
         )
 
-    test_id = vector_store.dataset.id[0].data()["value"]
+    test_id = vector_store.dataset_handler.dataset.id[0].data()["value"]
 
     data_ce_q = vector_store.search(
         query=f"select * where id == '{test_id}'",
         exec_option="compute_engine",
     )
     assert data_ce_q["id"][0] == test_id
 
@@ -671,15 +717,15 @@
     )
 
     data_db = vector_store.search(
         embedding=query_embedding,
         exec_option="tensor_db",
     )
 
-    assert "vectordb/" in vector_store.dataset.base_storage.path
+    assert "vectordb/" in vector_store.dataset_handler.dataset.base_storage.path
 
     assert len(data_ce["score"]) == len(data_db["score"])
     assert all(
         [
             isclose(
                 data_ce["score"][i],
                 data_db["score"][i],
@@ -704,31 +750,34 @@
     )
 
     # add data to the dataset:
     vector_store.add(id=ids, embedding=embeddings, text=texts, metadata=metadatas)
     assert_vectorstore_structure(vector_store, 10)
 
     # delete the data in the dataset by id:
-    print(len(vector_store.dataset))
+    print(len(vector_store.dataset_handler.dataset))
     vector_store.delete(row_ids=[4, 8, 9])
-    assert len(vector_store.dataset) == NUMBER_OF_DATA - 3
+    assert len(vector_store.dataset_handler.dataset) == NUMBER_OF_DATA - 3
 
     vector_store.delete(filter={"metadata": {"abc": 1}})
-    assert len(vector_store.dataset) == NUMBER_OF_DATA - 4
+    assert len(vector_store.dataset_handler.dataset) == NUMBER_OF_DATA - 4
 
     vector_store.delete(ids=["7"])
-    assert len(vector_store.dataset) == NUMBER_OF_DATA - 5
+    assert len(vector_store.dataset_handler.dataset) == NUMBER_OF_DATA - 5
 
     with pytest.raises(ValueError):
         vector_store.delete()
 
-    tensors_before_delete = vector_store.dataset.tensors
+    tensors_before_delete = vector_store.dataset_handler.dataset.tensors
     vector_store.delete(delete_all=True)
-    assert len(vector_store.dataset) == 0
-    assert vector_store.dataset.tensors.keys() == tensors_before_delete.keys()
+    assert len(vector_store.dataset_handler.dataset) == 0
+    assert (
+        vector_store.dataset_handler.dataset.tensors.keys()
+        == tensors_before_delete.keys()
+    )
 
     vector_store.delete_by_path(local_path)
     dirs = os.listdir("./")
     assert local_path not in dirs
 
     # backwards compatibility test:
     vector_store_b = DeepLakeVectorStore(
@@ -748,15 +797,15 @@
         token=hub_cloud_dev_token,
     )
     # add data to the dataset:
     vector_store_b.add(ids=ids, docs=texts)
 
     # delete the data in the dataset by id:
     vector_store_b.delete(row_ids=[0])
-    assert len(vector_store_b.dataset) == NUMBER_OF_DATA - 1
+    assert len(vector_store_b.dataset_handler.dataset) == NUMBER_OF_DATA - 1
 
     ds = deeplake.empty(local_path, overwrite=True)
     ds.create_tensor("id", htype="text")
     ds.create_tensor("embedding", htype="embedding")
     ds.extend(
         {
             "id": ids,
@@ -806,72 +855,125 @@
             filter=filters,
             query=query,
             exec_option=exec_option,
         )
 
     if callable(embedding_function) and isinstance(embedding_tensor, str):
         np.testing.assert_array_equal(
-            vector_store.dataset[embedding_tensor][row_ids].numpy(),
+            vector_store.dataset_handler.dataset[embedding_tensor][row_ids].numpy(),
             new_embeddings,
         )
 
     if callable(embedding_function) and isinstance(embedding_tensor, list):
         for i in range(len(embedding_tensor)):
             np.testing.assert_array_equal(
-                vector_store.dataset[embedding_tensor[i]][row_ids].numpy(),
+                vector_store.dataset_handler.dataset[embedding_tensor[i]][
+                    row_ids
+                ].numpy(),
                 new_embeddings[i],
             )
 
     if isinstance(embedding_function, list) and isinstance(embedding_tensor, list):
         for i in range(len(embedding_tensor)):
             np.testing.assert_array_equal(
-                vector_store.dataset[embedding_tensor[i]][row_ids].numpy(),
+                vector_store.dataset_handler.dataset[embedding_tensor[i]][
+                    row_ids
+                ].numpy(),
                 new_embeddings[i],
             )
 
 
+# TODO: refactor this method:
+# 1. Split this method into multiple methods (1 test per 1 behavior)
+# 2. use create_and_populate_vs to make these tests more readable
+# 3. create one fixture for these nested fixtures
 @requires_libdeeplake
 @pytest.mark.parametrize(
-    "ds, vector_store_hash_ids, vector_store_row_ids, vector_store_filters, vector_store_query",
+    "ds, vector_store_hash_ids, vector_store_row_ids, vector_store_filters, vector_store_filter_udf, vector_store_query, hub_cloud_dev_token",
     [
-        ("local_auth_ds", "vector_store_hash_ids", None, None, None),
-        ("local_auth_ds", None, "vector_store_row_ids", None, None),
-        ("local_auth_ds", None, None, "vector_store_filter_udf", None),
-        ("local_auth_ds", None, None, "vector_store_filters", None),
-        ("hub_cloud_ds", None, None, None, "vector_store_query"),
+        (
+            "local_auth_ds",
+            "vector_store_hash_ids",
+            None,
+            None,
+            None,
+            None,
+            "hub_cloud_dev_token",
+        ),
+        (
+            "local_auth_ds",
+            None,
+            "vector_store_row_ids",
+            None,
+            None,
+            None,
+            "hub_cloud_dev_token",
+        ),
+        (
+            "local_auth_ds",
+            None,
+            None,
+            None,
+            "vector_store_filter_udf",
+            None,
+            "hub_cloud_dev_token",
+        ),
+        (
+            "local_auth_ds",
+            None,
+            None,
+            "vector_store_filters",
+            None,
+            None,
+            "hub_cloud_dev_token",
+        ),
+        (
+            "hub_cloud_ds",
+            None,
+            None,
+            None,
+            None,
+            "vector_store_query",
+            "hub_cloud_dev_token",
+        ),
     ],
     indirect=True,
 )
 @pytest.mark.parametrize("init_embedding_function", [embedding_fn3, None])
 @pytest.mark.slow
 @requires_libdeeplake
 def test_update_embedding(
     ds,
     vector_store_hash_ids,
     vector_store_row_ids,
     vector_store_filters,
+    vector_store_filter_udf,
     vector_store_query,
     init_embedding_function,
+    hub_cloud_dev_token,
 ):
-    if vector_store_filters == "filter_udf":
-        vector_store_filters = filter_udf
+    vector_store_filters = vector_store_filters or vector_store_filter_udf
+
+    exec_option = "compute_engine"
+    if vector_store_filter_udf:
+        exec_option = "python"
 
     embedding_tensor = "embedding"
     embedding_source_tensor = "text"
     # dataset has a single embedding_tensor:
 
     path = ds.path
     vector_store = DeepLakeVectorStore(
         path=path,
         overwrite=True,
         verbose=False,
-        exec_option="compute_engine",
+        exec_option=exec_option,
         embedding_function=init_embedding_function,
         index_params={"threshold": 10},
-        token=ds.token,
+        token=hub_cloud_dev_token,
     )
 
     # add data to the dataset:
     metadatas[1:6] = [{"a": 1} for _ in range(5)]
     vector_store.add(id=ids, embedding=embeddings, text=texts, metadata=metadatas)
 
     # case 1: single embedding_source_tensor, single embedding_tensor, single embedding_function
@@ -892,15 +994,15 @@
         vector_store_hash_ids,
         vector_store_row_ids,
         vector_store_filters,
         vector_store_query,
         embedding_fn,
         embedding_source_tensor,
         embedding_tensor,
-        "compute_engine",
+        exec_option,
         num_changed_samples=5,
     )
 
     # case 2: single embedding_source_tensor, single embedding_tensor not specified, single embedding_function
     new_embedding_value = 100
     embedding_fn = get_embedding_function(embedding_value=new_embedding_value)
     vector_store.update_embedding(
@@ -917,15 +1019,15 @@
         vector_store_hash_ids,
         vector_store_row_ids,
         vector_store_filters,
         vector_store_query,
         embedding_fn,
         embedding_source_tensor,
         embedding_tensor,
-        "compute_engine",
+        exec_option,
         num_changed_samples=5,
     )
 
     # case 3-4: single embedding_source_tensor, single embedding_tensor, single init_embedding_function
     if init_embedding_function is None:
         # case 3: errors out when init_embedding_function is not specified
         with pytest.raises(ValueError):
@@ -951,15 +1053,15 @@
             vector_store_hash_ids,
             vector_store_row_ids,
             vector_store_filters,
             vector_store_query,
             init_embedding_function,
             embedding_source_tensor,
             embedding_tensor,
-            "compute_engine",
+            exec_option,
             num_changed_samples=5,
         )
 
     vector_store.delete_by_path(path, token=ds.token)
 
     # dataset has a multiple embedding_tensor:
     tensors = [
@@ -1008,14 +1110,15 @@
     vector_store = DeepLakeVectorStore(
         path=path + "_multi",
         overwrite=True,
         verbose=False,
         embedding_function=init_embedding_function,
         tensor_params=tensors,
         token=ds.token,
+        exec_option=exec_option,
     )
 
     vector_store.add(
         id=ids,
         text=texts,
         embedding=embeddings,
         embedding_md=embeddings,
@@ -1079,15 +1182,15 @@
         vector_store_hash_ids,
         vector_store_row_ids,
         vector_store_filters,
         vector_store_query,
         embedding_fn,
         multiple_embedding_source_tensor,
         multiple_embedding_tensor,
-        "compute_engine",
+        exec_option,
         num_changed_samples=5,
     )
 
     # case 5-6: multiple embedding_source_tensor, multiple embedding_tensor, single init_embedding_function
     new_embedding_value = [0, 0]
 
     if init_embedding_function is None:
@@ -1117,15 +1220,15 @@
             vector_store_hash_ids,
             vector_store_row_ids,
             vector_store_filters,
             vector_store_query,
             embedding_fn3,
             multiple_embedding_source_tensor,
             multiple_embedding_tensor,
-            "compute_engine",
+            exec_option,
             num_changed_samples=5,
         )
 
     # case 7: multiple embedding_source_tensor, not specified embedding_tensor, multiple embedding_function -> error out?
     with pytest.raises(ValueError):
         vector_store.update_embedding(
             ids=vector_store_hash_ids,
@@ -1180,20 +1283,116 @@
         vector_store_hash_ids,
         vector_store_row_ids,
         vector_store_filters,
         vector_store_query,
         embedding_function,
         embedding_source_tensor,
         embedding_tensor,
-        "compute_engine",
+        exec_option,
         num_changed_samples=5,
     )
     vector_store.delete_by_path(path + "_multi", token=ds.token)
 
 
+def create_and_populate_vs(
+    path,
+    token=None,
+    overwrite=True,
+    verbose=False,
+    exec_option="compute_engine",
+    index_params={"threshold": 10},
+    number_of_data=NUMBER_OF_DATA,
+):
+    # TODO: cache the vectostore object and reuse it in other tests (maybe with deepcopy)
+    vector_store = DeepLakeVectorStore(
+        path=path,
+        overwrite=overwrite,
+        verbose=verbose,
+        exec_option=exec_option,
+        index_params=index_params,
+        token=token,
+    )
+
+    utils.create_data(number_of_data=number_of_data, embedding_dim=EMBEDDING_DIM)
+
+    # add data to the dataset:
+    metadatas[1:6] = [{"a": 1} for _ in range(5)]
+    vector_store.add(id=ids, embedding=embeddings, text=texts, metadata=metadatas)
+    return vector_store
+
+
+def test_update_embedding_row_ids_and_ids_specified_should_throw_exception(
+    local_path,
+    vector_store_hash_ids,
+    vector_store_row_ids,
+    hub_cloud_dev_token,
+):
+    # specifying both row_ids and ids during update embedding should throw an exception
+    # initializing vectorstore and populating it:
+    vector_store = create_and_populate_vs(
+        local_path,
+        token=hub_cloud_dev_token,
+    )
+    embedding_fn = get_embedding_function()
+
+    # calling update_embedding with both ids and row_ids being specified
+    with pytest.raises(ValueError):
+        vector_store.update_embedding(
+            ids=vector_store_hash_ids,
+            row_ids=vector_store_row_ids,
+            embedding_function=embedding_fn,
+        )
+
+
+def test_update_embedding_row_ids_and_filter_specified_should_throw_exception(
+    local_path,
+    vector_store_filters,
+    vector_store_row_ids,
+    hub_cloud_dev_token,
+):
+    # specifying both row_ids and filter during update embedding should throw an exception
+    # initializing vectorstore and populating it:
+    vector_store = create_and_populate_vs(
+        local_path,
+        token=hub_cloud_dev_token,
+    )
+    embedding_fn = get_embedding_function()
+
+    # calling update_embedding with both ids and filter being specified
+    with pytest.raises(ValueError):
+        vector_store.update_embedding(
+            row_ids=vector_store_row_ids,
+            filter=vector_store_filters,
+            embedding_function=embedding_fn,
+        )
+
+
+@requires_libdeeplake
+def test_update_embedding_query_and_filter_specified_should_throw_exception(
+    local_path,
+    vector_store_filters,
+    vector_store_query,
+    hub_cloud_dev_token,
+):
+    # initializing vectorstore and populating it:
+    vector_store = create_and_populate_vs(
+        local_path,
+        token=hub_cloud_dev_token,
+    )
+    embedding_fn = get_embedding_function()
+
+    # calling update_embedding with both query and filter being specified
+    with pytest.raises(ValueError):
+        vector_store.update_embedding(
+            filter=vector_store_filters,
+            query=vector_store_query,
+            embedding_function=embedding_fn,
+        )
+
+
 @requires_libdeeplake
 def test_vdb_index_creation(local_path, capsys, hub_cloud_dev_token):
     number_of_data = 1000
     texts, embeddings, ids, metadatas, _ = utils.create_data(
         number_of_data=number_of_data, embedding_dim=EMBEDDING_DIM
     )
 
@@ -1206,15 +1405,15 @@
         index_params={"threshold": 200, "distance_metric": "L2"},
         token=hub_cloud_dev_token,
     )
 
     vector_store.add(embedding=embeddings, text=texts, id=ids, metadata=metadatas)
 
     assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1224,15 +1423,15 @@
             "id",
             "metadata",
             "text",
         ]
     )
 
     # Check if the index is recreated properly.
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     es = ds.embedding.get_vdb_indexes()
     assert len(es) == 1
     assert es[0]["id"] == "hnsw_1"
     assert es[0]["distance"] == "l2_norm"
     assert es[0]["type"] == "hnsw"
 
     vector_store.delete_by_path(local_path, token=ds.token)
@@ -1277,15 +1476,15 @@
 
     vector_store.add(embedding=emb1, text=txt1, id=ids1, metadata=md1)
     vector_store.add(embedding=emb2, text=txt2, id=ids2, metadata=md2)
     vector_store.add(embedding=emb3, text=txt3, id=ids3, metadata=md3)
     vector_store.add(embedding=emb4, text=txt4, id=ids4, metadata=md4)
 
     assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1295,15 +1494,15 @@
             "id",
             "metadata",
             "text",
         ]
     )
 
     # Check if the index is recreated properly.
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     es = ds.embedding.get_vdb_indexes()
     assert len(es) == 1
     assert es[0]["id"] == "hnsw_1"
     assert es[0]["distance"] == "l2_norm"
     assert es[0]["type"] == "hnsw"
 
     # search the embeddings.
@@ -1369,21 +1568,21 @@
         verbose=True,
         exec_option="compute_engine",
         index_params={"threshold": 50, "distance_metric": "L2"},
         token=hub_cloud_dev_token,
     )
 
     vector_store.add(embedding=emb1, text=txt1, id=ids1, metadata=md1)
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     ds.extend({"embedding": emb2, "text": txt2, "id": ids2, "metadata": md2})
     ds.extend({"embedding": emb3, "text": txt3, "id": ids3, "metadata": md3})
     ds.extend({"embedding": emb4, "text": txt4, "id": ids4, "metadata": md4})
 
     assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1393,15 +1592,15 @@
             "id",
             "metadata",
             "text",
         ]
     )
 
     # Check if the index is recreated properly.
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     es = ds.embedding.get_vdb_indexes()
     assert len(es) == 1
     assert es[0]["id"] == "hnsw_1"
     assert es[0]["distance"] == "l2_norm"
     assert es[0]["type"] == "hnsw"
 
     # search the embeddings.
@@ -1470,22 +1669,22 @@
         overwrite=True,
         verbose=True,
         exec_option="compute_engine",
         index_params={"threshold": 2, "distance_metric": "L2"},
         token=hub_cloud_dev_token,
     )
 
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     ds.append({"embedding": emb1, "text": txt1, "id": ids1, "metadata": md1})
     ds.append({"embedding": emb2, "text": txt2, "id": ids2, "metadata": md2})
     ds.append({"embedding": emb3, "text": txt3, "id": ids3, "metadata": md3})
     ds.append({"embedding": emb4, "text": txt4, "id": ids4, "metadata": md4})
 
     # assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1579,21 +1778,21 @@
         verbose=True,
         exec_option="compute_engine",
         index_params={"threshold": 2, "distance_metric": "L2"},
         token=hub_cloud_dev_token,
     )
 
     vector_store.add(embedding=emb1, text=txt1, id=ids1, metadata=md1)
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
     ds.append({"embedding": emb2, "text": txt2, "id": ids2, "metadata": md2})
     ds.append({"embedding": emb3, "text": txt3, "id": ids3, "metadata": md3})
     ds.append({"embedding": emb4, "text": txt4, "id": ids4, "metadata": md4})
 
     # assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1696,23 +1895,23 @@
         verbose=True,
         exec_option="compute_engine",
         index_params={"threshold": 2, "distance_metric": "L2"},
         token=hub_cloud_dev_token,
     )
 
     vector_store.add(embedding=emb1, text=txt1, id=ids1, metadata=md1)
-    ds = vector_store.dataset
+    ds = vector_store.dataset_handler.dataset
 
     ds.embedding.append(emb2)
     ds.embedding.append(emb3)
     ds.embedding.append(emb4)
     # ds.embedding[104] = emb5
 
     # assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == set(
+    assert set(vector_store.dataset_handler.dataset.tensors) == set(
         [
             "embedding",
             "id",
             "metadata",
             "text",
         ]
     )
@@ -1815,34 +2014,34 @@
         ds2[tensor].extend(ds[tensor].data()["value"])
 
     vector_store.delete_by_path(local_path, token=hub_cloud_dev_token)
 
 
 def assert_vectorstore_structure(vector_store, number_of_data):
     assert len(vector_store) == number_of_data
-    assert set(vector_store.dataset.tensors) == {
+    assert set(vector_store.dataset_handler.dataset.tensors) == {
         "embedding",
         "id",
         "metadata",
         "text",
     }
     assert set(vector_store.tensors()) == {
         "embedding",
         "id",
         "metadata",
         "text",
     }
-    assert vector_store.dataset.embedding.htype == "embedding"
-    assert vector_store.dataset.id.htype == "text"
-    assert vector_store.dataset.metadata.htype == "json"
-    assert vector_store.dataset.text.htype == "text"
-    assert vector_store.dataset.embedding.dtype == "float32"
-    assert vector_store.dataset.id.dtype == "str"
-    assert vector_store.dataset.metadata.dtype == "str"
-    assert vector_store.dataset.text.dtype == "str"
+    assert vector_store.dataset_handler.dataset.embedding.htype == "embedding"
+    assert vector_store.dataset_handler.dataset.id.htype == "text"
+    assert vector_store.dataset_handler.dataset.metadata.htype == "json"
+    assert vector_store.dataset_handler.dataset.text.htype == "text"
+    assert vector_store.dataset_handler.dataset.embedding.dtype == "float32"
+    assert vector_store.dataset_handler.dataset.id.dtype == "str"
+    assert vector_store.dataset_handler.dataset.metadata.dtype == "str"
+    assert vector_store.dataset_handler.dataset.text.dtype == "str"
 
 
 @pytest.mark.slow
 def test_ingestion(local_path):
     # create data
     number_of_data = 1000
     texts, embeddings, ids, metadatas, _ = utils.create_data(
@@ -1914,18 +2113,18 @@
         tensor_params=tensor_params,
         overwrite=True,
         verbose=True,
     )
 
     ids = vector_store.add(image=images, embedding=embeddings, return_ids=True)
 
-    assert "image" in vector_store.dataset.tensors
-    assert "embedding" in vector_store.dataset.tensors
-    assert len(vector_store.dataset.image[0].numpy().shape) == 3
-    assert len(vector_store.dataset.image[1].numpy().shape) == 3
+    assert "image" in vector_store.dataset_handler.dataset.tensors
+    assert "embedding" in vector_store.dataset_handler.dataset.tensors
+    assert len(vector_store.dataset_handler.dataset.image[0].numpy().shape) == 3
+    assert len(vector_store.dataset_handler.dataset.image[1].numpy().shape) == 3
     assert len(ids) == 10
 
 
 def test_parse_add_arguments(local_path):
     deeplake_vector_store = DeepLakeVectorStore(
         path="mem://dummy",
         overwrite=True,
@@ -1933,67 +2132,67 @@
     )
     embedding_fn_dp = DeepLakeEmbedder(embedding_function=embedding_fn)
     embedding_fn2_dp = DeepLakeEmbedder(embedding_function=embedding_fn2)
 
     with pytest.raises(ValueError):
         # Throw error because embedding_function requires embed_data_from
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             initial_embedding_function=embedding_fn,
             embedding_function=embedding_fn,
             embeding_tensor="embedding",
             text=texts,
             id=ids,
             metadata=metadatas,
         )
 
     with pytest.raises(ValueError):
         # Throw error because embedding function is not specified anywhere
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             embedding_data=texts,
             embeding_tensor="embedding",
             text=texts,
             id=ids,
             metadata=metadatas,
         )
 
     with pytest.raises(ValueError):
         # Throw error because data is not specified for all tensors
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             text=texts,
             id=ids,
             metadata=metadatas,
         )
 
     with pytest.raises(ValueError):
         # initial embedding function specified and embeding_tensor is specified
         (
             embedding_function,
             embeding_tensor,
             embed_data_from,
             tensors,
         ) = utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             initial_embedding_function=embedding_fn,
             embedding_tensor="embedding",
             text=texts,
             id=ids,
             metadata=metadatas,
         )
 
     # initial embedding function is specified and embeding_tensor, embed_data_from are not specified
     (
         embedding_function,
         embeding_tensor,
         embed_data_from,
         tensors,
     ) = utils.parse_add_arguments(
-        dataset=deeplake_vector_store.dataset,
+        dataset=deeplake_vector_store.dataset_handler.dataset,
         initial_embedding_function=embedding_fn_dp,
         text=texts,
         id=ids,
         embedding=embeddings,
         metadata=metadatas,
     )
     assert embedding_function is None
@@ -2005,65 +2204,65 @@
         "metadata": metadatas,
         "embedding": embeddings,
     }
 
     with pytest.raises(ValueError):
         # initial embedding function specified and embeding_tensor is not specified
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             initial_embedding_function=embedding_fn_dp,
             embedding_data=texts,
             text=texts,
             id=ids,
             embedding=embeddings,
             metadata=metadatas,
         )  # 2
 
     with pytest.raises(ValueError):
         # Throw error because embedding_function and embedding are specified
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             initial_embedding_function=embedding_fn_dp,
             embedding_function=embedding_fn_dp,
             embedding_data=texts,
             embedding_tensor="embedding",
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding=embeddings,
         )
 
     with pytest.raises(ValueError):
         # initial_embedding_function is specified and embeding_tensor, embed_data_from and embedding is specified.
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             initial_embedding_function=embedding_fn_dp,
             embedding_tensor="embedding",
             embedding_data=texts,
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding=embeddings,
         )
 
     with pytest.raises(ValueError):
         # initial_embedding_function is not specified and embeding_tensor, embed_data_from and embedding is specified.
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             embeding_tensor="embedding",
             embedding_data=texts,
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding=embeddings,
         )
 
     with pytest.raises(ValueError):
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             embedding_function=embedding_fn_dp,
             initial_embedding_function=embedding_fn_dp,
             embedding_data=texts,
             embedding_tensor="embedding",
             text=texts,
             id=ids,
             embedding=embeddings,
@@ -2072,15 +2271,15 @@
 
     (
         embedding_function,
         embedding_data,
         embedding_tensors,
         tensors,
     ) = utils.parse_add_arguments(
-        dataset=deeplake_vector_store.dataset,
+        dataset=deeplake_vector_store.dataset_handler.dataset,
         embedding_function=embedding_fn2_dp,
         embedding_data=texts,
         embedding_tensor="embedding",
         text=texts,
         id=ids,
         metadata=metadatas,
     )
@@ -2093,15 +2292,15 @@
 
     (
         embedding_function,
         embedding_data,
         embedding_tensors,
         tensors,
     ) = utils.parse_add_arguments(
-        dataset=deeplake_vector_store.dataset,
+        dataset=deeplake_vector_store.dataset_handler.dataset,
         embedding_function=embedding_fn2_dp,
         embedding_data="text",
         embedding_tensor="embedding",
         text=texts,
         metadata=metadatas,
     )
     assert embedding_tensors == ["embedding"]
@@ -2127,15 +2326,15 @@
             },
         ],
     )
 
     # There are two embedding but an embedding_tensor is not specified, so it's not clear where to add the embedding data
     with pytest.raises(ValueError):
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             embedding_function=embedding_fn2_dp,
             embedding_data="text",
             text=texts,
             metadata=metadatas,
         )
 
     # Creating a vector store without embedding htype or tensor name
@@ -2150,15 +2349,15 @@
             },
         ],
     )
 
     # There is no embedding tensor, so it's not clear where to add the embedding data
     with pytest.raises(ValueError):
         utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             embedding_function=embedding_fn2_dp,
             embedding_data=texts,
             text=texts,
         )
 
     # Creating a vector store with embedding tensor with a custom name
     deeplake_vector_store = DeepLakeVectorStore(
@@ -2179,15 +2378,15 @@
 
     (
         embedding_function,
         embedding_data,
         embedding_tensors,
         tensors,
     ) = utils.parse_add_arguments(
-        dataset=deeplake_vector_store.dataset,
+        dataset=deeplake_vector_store.dataset_handler.dataset,
         embedding_function=embedding_fn2_dp,
         embedding_data=texts,
         text=texts,
     )
 
     assert embedding_tensors == ["embedding_1"]
     assert len(tensors) == 1
@@ -2200,15 +2399,15 @@
 
     (
         embedding_function,
         embedding_data,
         embedding_tensor,
         tensors,
     ) = utils.parse_add_arguments(
-        dataset=deeplake_vector_store.dataset,
+        dataset=deeplake_vector_store.dataset_handler.dataset,
         initial_embedding_function=embedding_fn_dp,
         text=texts,
         id=ids,
         metadata=metadatas,
         embedding_data=texts,
         embedding_tensor="embedding",
     )
@@ -2223,43 +2422,43 @@
     with pytest.raises(ValueError):
         (
             embedding_function,
             embedding_data,
             embedding_tensor,
             tensors,
         ) = utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding_tensor="embedding",
         )
 
     with pytest.raises(ValueError):
         (
             embedding_function,
             embedding_data,
             embedding_tensor,
             tensors,
         ) = utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding_data=texts,
         )
 
     with pytest.raises(ValueError):
         (
             embedding_function,
             embedding_data,
             embedding_tensor,
             tensors,
         ) = utils.parse_add_arguments(
-            dataset=deeplake_vector_store.dataset,
+            dataset=deeplake_vector_store.dataset_handler.dataset,
             text=texts,
             id=ids,
             metadata=metadatas,
             embedding=embeddings,
             new_tensor=texts,
         )
 
@@ -2384,15 +2583,17 @@
         text=texts,
         embedding_function=embedding_fn,
         embedding_data=[texts, texts],
         embedding_tensor=["embedding_1", "embedding_2"],
     )
 
     # test with initial embedding function
-    vector_store.embedding_function = DeepLakeEmbedder(embedding_function=embedding_fn)
+    vector_store.dataset_handler.embedding_function = DeepLakeEmbedder(
+        embedding_function=embedding_fn
+    )
     vector_store.add(
         text=texts,
         embedding_data=[texts, texts],
         embedding_tensor=["embedding_1", "embedding_2"],
     )
 
     number_of_data = 1000
@@ -2407,19 +2608,19 @@
     )
     vector_store.add(
         text=25 * _texts,
         embedding_1=(embedding_fn3, 25 * _texts),
         embedding_2=(embedding_fn3, 25 * _texts),
     )
 
-    assert len(vector_store.dataset) == 50040
-    assert len(vector_store.dataset.embedding_1) == 50040
-    assert len(vector_store.dataset.embedding_2) == 50040
-    assert len(vector_store.dataset.id) == 50040
-    assert len(vector_store.dataset.text) == 50040
+    assert len(vector_store.dataset_handler.dataset) == 50040
+    assert len(vector_store.dataset_handler.dataset.embedding_1) == 50040
+    assert len(vector_store.dataset_handler.dataset.embedding_2) == 50040
+    assert len(vector_store.dataset_handler.dataset.id) == 50040
+    assert len(vector_store.dataset_handler.dataset.text) == 50040
 
 
 def test_extend_none(local_path):
     vector_store = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
         tensor_params=[
@@ -2430,19 +2631,19 @@
                 "htype": "text",
             },
             {"name": "metadata", "htype": "json"},
         ],
     )
 
     vector_store.add(text=texts, embedding=None, id=ids, metadata=None)
-    assert len(vector_store.dataset) == 10
-    assert len(vector_store.dataset.text) == 10
-    assert len(vector_store.dataset.embedding) == 10
-    assert len(vector_store.dataset.id) == 10
-    assert len(vector_store.dataset.metadata) == 10
+    assert len(vector_store.dataset_handler.dataset) == 10
+    assert len(vector_store.dataset_handler.dataset.text) == 10
+    assert len(vector_store.dataset_handler.dataset.embedding) == 10
+    assert len(vector_store.dataset_handler.dataset.id) == 10
+    assert len(vector_store.dataset_handler.dataset.metadata) == 10
 
 
 def test_query_dim(local_path):
     vector_store = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
         tensor_params=[
@@ -2468,62 +2669,64 @@
         ],
     )
 
     vector_store.add(
         embedding_1=(embedding_fn, texts), embedding_2=(embedding_fn3, texts)
     )
 
-    assert len(vector_store.dataset) == 10
-    assert len(vector_store.dataset.embedding_1) == 10
-    assert len(vector_store.dataset.embedding_2) == 10
+    assert len(vector_store.dataset_handler.dataset) == 10
+    assert len(vector_store.dataset_handler.dataset.embedding_1) == 10
+    assert len(vector_store.dataset_handler.dataset.embedding_2) == 10
 
 
 def test_uuid_fix(local_path):
     vector_store = VectorStore(local_path, overwrite=True)
 
     ids = [uuid.uuid4() for _ in range(NUMBER_OF_DATA)]
 
     vector_store.add(text=texts, id=ids, embedding=embeddings, metadata=metadatas)
 
-    assert vector_store.dataset.id.data()["value"] == list(map(str, ids))
+    assert vector_store.dataset_handler.dataset.id.data()["value"] == list(
+        map(str, ids)
+    )
 
 
 def test_read_only():
     db = VectorStore("hub://davitbun/twitter-algorithm")
-    assert db.dataset.read_only == True
+    assert db.dataset_handler.dataset.read_only == True
 
 
 def test_delete_by_path_wrong_path():
     with pytest.raises(DatasetHandlerError):
         VectorStore.delete_by_path("some_path")
 
 
 @requires_libdeeplake
 def test_exec_option_with_auth(local_path, hub_cloud_path, hub_cloud_dev_token):
     db = VectorStore(path=local_path)
-    assert db.exec_option == "python"
+    assert db.dataset_handler.exec_option == "python"
 
     db = VectorStore(
         path=local_path,
         token=hub_cloud_dev_token,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
 
     db = VectorStore(
         path=hub_cloud_path,
         token=hub_cloud_dev_token,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
 
     db = VectorStore(
         path=hub_cloud_path + "_tensor_db",
         token=hub_cloud_dev_token,
         runtime={"tensor_db": True},
     )
-    assert db.exec_option == "tensor_db"
+    assert db.dataset_handler.exec_option == "tensor_db"
 
 
 @requires_libdeeplake
 def test_exec_option_cli(
     local_path,
     hub_cloud_path,
     hub_cloud_dev_token,
@@ -2534,59 +2737,59 @@
     # Testing exec_option with cli login and logout commands are executed
     runner.invoke(login, f"-u {username} -p {password}")
 
     # local dataset and logged in with cli
     db = VectorStore(
         path=local_path,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
 
     # hub cloud dataset and logged in with cli
     db = VectorStore(
         path=hub_cloud_path,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
 
     # hub cloud dataset and logged in with cli
     db = VectorStore(
         path="mem://abc",
     )
-    assert db.exec_option == "python"
+    assert db.dataset_handler.exec_option == "python"
 
     # logging out with cli
     runner.invoke(logout)
 
     # local dataset and logged out with cli
     db = VectorStore(
         path=local_path,
     )
-    assert db.exec_option == "python"
+    assert db.dataset_handler.exec_option == "python"
 
     # Check whether after logging out exec_option changes to python
     # logging in with cli token
     runner.invoke(login, f"-t {hub_cloud_dev_token}")
     db = VectorStore(
         path=local_path,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
     # logging out with cli
     runner.invoke(logout)
-    assert db.exec_option == "python"
+    assert db.dataset_handler.exec_option == "python"
 
     # Check whether after logging out when token specified exec_option doesn't change
     # logging in with cli token
     runner.invoke(login, f"-t {hub_cloud_dev_token}")
     db = VectorStore(
         path=local_path,
         token=hub_cloud_dev_token,
     )
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
     # logging out with cli
     runner.invoke(logout)
-    assert db.exec_option == "compute_engine"
+    assert db.dataset_handler.exec_option == "compute_engine"
 
 
 @requires_libdeeplake
 @pytest.mark.parametrize(
     "path",
     [
         "s3_path",
@@ -2605,34 +2808,75 @@
 
     db = VectorStore(path, overwrite=True)
     assert db.exec_option == "python"
 
     runner.invoke(login, f"-t {hub_cloud_dev_token}")
     assert db.exec_option == "python"
 
-    db.dataset.connect(
+    db.dataset_handler.dataset.connect(
         creds_key=hub_cloud_dev_managed_creds_key,
         dest_path=hub_cloud_path,
         token=hub_cloud_dev_token,
     )
-    db.dataset.add_creds_key(hub_cloud_dev_managed_creds_key, managed=True)
+    db.dataset_handler.dataset.add_creds_key(
+        hub_cloud_dev_managed_creds_key, managed=True
+    )
     assert db.exec_option == "compute_engine"
 
 
-@pytest.mark.slow
-@pytest.mark.parametrize(
-    "runtime",
-    ["runtime", None],
-    indirect=True,
-)
-@pytest.mark.skipif(sys.platform == "win32", reason="Does not run on Windows")
-def test_vectorstore_factory(hub_cloud_dev_token, hub_cloud_path, runtime):
-    db = vectorstore_factory(
-        path=hub_cloud_path,
-        runtime=runtime,
-        token=hub_cloud_dev_token,
+def test_dataset_init_param(local_ds):
+    local_ds.create_tensor("text", htype="text")
+    local_ds.create_tensor("embedding", htype="embedding")
+    local_ds.create_tensor("id", htype="text")
+    local_ds.create_tensor("metadata", htype="json")
+
+    db = VectorStore(
+        dataset=local_ds,
     )
 
-    if runtime is not None:
-        assert isinstance(db, DeepMemoryVectorStore)
-    else:
-        assert isinstance(db, DeepLakeVectorStore)
+    db.add(text=texts, embedding=embeddings, id=ids, metadata=metadatas)
+    assert len(db) == 10
+
+
+def test_vs_commit(local_path):
+    # TODO: add index params, when index will support commit
+    db = create_and_populate_vs(
+        local_path, number_of_data=NUMBER_OF_DATA, index_params=None
+    )
+    db.checkout("branch_1", create=True)
+    db.commit("commit_1")
+    db.add(text=texts, embedding=embeddings, id=ids, metadata=metadatas)
+    assert len(db) == 2 * NUMBER_OF_DATA
+
+    db.checkout("main")
+    assert len(db) == NUMBER_OF_DATA
+
+
+def test_vs_init_when_both_dataset_and_path_is_specified_should_throw_exception(
+    local_path,
+):
+    with pytest.raises(ValueError):
+        VectorStore(
+            path=local_path,
+            dataset=deeplake.empty(local_path, overwrite=True),
+        )
+
+
+def test_specifying_row_ids_and_filter_should_throw_excrption(local_path):
+    db = VectorStore(
+        path=local_path,
+    )
+    db.add(text=texts, embedding=embeddings, id=ids, metadata=metadatas)
+
+
+def test_vs_init_when_both_dataset_and_path_are_not_specified_should_throw_exception():
+    with pytest.raises(ValueError):
+        VectorStore()
+
+
+def test_vs_init_with_emptyt_token_should_not_throw_exception(local_path):
+    with patch("deeplake.client.config.DEEPLAKE_AUTH_TOKEN", ""):
+        db = VectorStore(
+            path=local_path,
+        )
+
+    assert db.dataset_handler.username == "public"
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/test_deepmemory.py` & `deeplake-3.8.9/deeplake/core/vectorstore/deep_memory/test_deepmemory.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import numpy as np
 import pytest
 import sys
 from time import sleep
 
 import deeplake
 from deeplake import VectorStore
+from deeplake.core.vectorstore.deep_memory.deep_memory import DeepMemory
 from deeplake.tests.common import requires_libdeeplake
-from deeplake.core.vectorstore.unsupported_deep_memory import (
-    DeepMemory as UnsupportedDeepMemory,
-)
 from deeplake.util.exceptions import (
     DeepMemoryWaitingListError,
     IncorrectQueriesTypeError,
     IncorrectRelevanceTypeError,
 )
+from deeplake.util.exceptions import DeepMemoryWaitingListError
+
+
+logger = logging.getLogger(__name__)
 
 
 class DummyEmbedder:
     @staticmethod
     def embed_documents(texts):
         return [
             np.random.uniform(low=-10, high=10, size=(1536)).astype(np.float32)
@@ -576,16 +578,18 @@
     assert relevance not in output["id"]
     assert "score" in output
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Does not run on Windows")
 @pytest.mark.slow
 @requires_libdeeplake
-def test_unsupported_deepmemory_users():
-    dm = UnsupportedDeepMemory()
+def test_unsupported_deepmemory_users(local_ds):
+    dm = DeepMemory(
+        dataset_or_path=local_ds, logger=logger, embedding_function=DummyEmbedder
+    )
     with pytest.raises(DeepMemoryWaitingListError):
         dm.train(
             queries=[],
             relevance=[],
         )
 
     with pytest.raises(DeepMemoryWaitingListError):
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/test_embedder.py` & `deeplake-3.8.9/deeplake/core/vectorstore/embeddings/test_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import pytest
 import sys
 from time import time
 
 import numpy as np
 
 from deeplake.constants import MAX_BYTES_PER_MINUTE, TARGET_BYTE_SIZE
-from deeplake.core.vectorstore.embedder import DeepLakeEmbedder, chunk_by_bytes
+from deeplake.core.vectorstore.embeddings.embedder import (
+    DeepLakeEmbedder,
+    chunk_by_bytes,
+)
 
 
 EMBEDDING_DIM = 15
 
 
 def test_chunk_by_bytes():
     data = ["a" * 10000] * 10  # 10 chunks of 10000 bytes
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,19 +551,26 @@
         logger=logger,
     )
 
 
 def convert_id_to_row_id(ids, dataset, search_fn, query, exec_option, filter):
     if ids is None:
         delete_view = search_fn(
+            embedding_data=None,
+            embedding_function=None,
+            embedding=None,
+            distance_metric=None,
+            embedding_tensor=None,
             filter=filter,
             query=query,
             exec_option=exec_option,
+            return_tensors=False,
             return_view=True,
             k=int(1e9),
+            deep_memory=False,
         )
 
     else:
         # backwards compatibility
         tensors = dataset.tensors
         id_tensor = "id"
         if "ids" in tensors:
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 
 import deeplake
 from deeplake.core.vectorstore import utils
 from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
 from deeplake.core.vectorstore import DeepLakeVectorStore
-from deeplake.core.vectorstore.embedder import DeepLakeEmbedder
+from deeplake.core.vectorstore.embeddings.embedder import DeepLakeEmbedder
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_DEEPLAKE_PATH,
     DEFAULT_VECTORSTORE_TENSORS,
     TARGET_BYTE_SIZE,
 )
 from deeplake.tests.common import requires_libdeeplake
 from deeplake.constants import MAX_BYTES_PER_MINUTE
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Dict, Union, Callable
-
-from deeplake.core.dataset import Dataset as DeepLakeDataset
-from deeplake.core.vectorstore.vector_search import utils
-from deeplake.core.vectorstore.vector_search import filter as filter_utils
 from deeplake.core import vectorstore
+from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
+from deeplake.core.vectorstore.vector_search import filter as filter_utils
+from deeplake.core.vectorstore.vector_search import utils
+from deeplake.core.dataset import Dataset as DeepLakeDataset
+from typing import Union, Dict
 
 
 def vector_search(
     query,
     query_emb,
     exec_option,
     dataset,
@@ -18,44 +18,39 @@
     k,
     return_tensors,
     return_view,
     deep_memory,
     token,
     org_id,
 ) -> Union[Dict, DeepLakeDataset]:
-    try:
-        from indra import api  # type: ignore
+    if query is not None:
+        raise NotImplementedError(
+            f"User-specified TQL queries are not supported for exec_option={exec_option} "
+        )
+
+    view = filter_utils.attribute_based_filtering_python(dataset, filter)
+
+    return_data = {}
+
+    # Only fetch embeddings and run the search algorithm if an embedding query is specified
+    if query_emb is not None:
+        embeddings = dataset_utils.fetch_embeddings(
+            view=view,
+            embedding_tensor=embedding_tensor,
+        )
 
-        _INDRA_INSTALLED = True  # pragma: no cover
-    except ImportError:  # pragma: no cover
-        _INDRA_INSTALLED = False  # pragma: no cover
-
-    runtime = utils.get_runtime_from_exec_option(exec_option)
-
-    if callable(filter):
-        raise ValueError(
-            f"UDF filter functions are not supported with the current `exec_option`={exec_option}. "
+        view, scores = vectorstore.python_search_algorithm(
+            deeplake_dataset=view,
+            query_embedding=query_emb,
+            embeddings=embeddings,
+            distance_metric=distance_metric.lower(),
+            k=k,
         )
 
-    utils.check_indra_installation(exec_option, indra_installed=_INDRA_INSTALLED)
+        return_data["score"] = scores
 
-    view, tql_filter = filter_utils.attribute_based_filtering_tql(
-        view=dataset,
-        filter=filter,
-        logger=logger,
-    )
-
-    return vectorstore.indra_search_algorithm(
-        query_embedding=query_emb,
-        distance_metric=distance_metric.lower(),
-        deeplake_dataset=view,
-        k=k,
-        tql_string=query,
-        tql_filter=tql_filter,
-        embedding_tensor=embedding_tensor,
-        runtime=runtime,
-        return_tensors=return_tensors,
-        return_view=return_view,
-        deep_memory=deep_memory,
-        token=token,
-        org_id=org_id,
-    )
+    if return_view:
+        return view
+    else:
+        for tensor in return_tensors:
+            return_data[tensor] = utils.parse_tensor_return(view[tensor])
+        return return_data
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import functools
-import time
 import types
+import random
+import string
 from abc import ABC, abstractmethod
+from typing import Optional, List, Dict, Tuple
 
+import deeplake
 from deeplake.constants import MB, DEFAULT_VECTORSTORE_INDEX_PARAMS, TARGET_BYTE_SIZE
 from deeplake.enterprise.util import raise_indra_installation_error
 from deeplake.util.exceptions import TensorDoesNotExistError
 from deeplake.util.warnings import always_warn
 from deeplake.client.utils import read_token
 from deeplake.core.dataset import DeepLakeCloudDataset, Dataset
-from deeplake.core.vectorstore.embedder import DeepLakeEmbedder
+from deeplake.core.vectorstore.embeddings.embedder import DeepLakeEmbedder
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.util.path import get_path_type
 
 import numpy as np
 
-import jwt
-import random
-import string
-from typing import Optional, List, Dict
 
 EXEC_OPTION_TO_RUNTIME: Dict[str, Optional[Dict]] = {
     "compute_engine": None,
     "python": None,
     "tensor_db": {"db_engine": True},
 }
```

### Comparing `deeplake-3.8.8/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.8.9/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.8.9/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/commit_diff.py` & `deeplake-3.8.9/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/commit_node.py` & `deeplake-3.8.9/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.8.9/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/test_merge.py` & `deeplake-3.8.9/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/core/version_control/test_version_control.py` & `deeplake-3.8.9/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.8.9/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/dataloader.py` & `deeplake-3.8.9/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.8.9/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.8.9/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/test_pytorch.py` & `deeplake-3.8.9/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/test_query.py` & `deeplake-3.8.9/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.8.9/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/enterprise/util.py` & `deeplake-3.8.9/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/hooks.py` & `deeplake-3.8.9/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/htype.py` & `deeplake-3.8.9/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.8.9/deeplake/integrations/huggingface/huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import deeplake
 from typing import Optional
 from tqdm import tqdm
 from deeplake.util.bugout_reporter import feature_report_path, deeplake_reporter
 
 
 def _is_seq_convertible(seq):
-    from datasets import Sequence
+    from datasets import Sequence  # type: ignore
 
     if isinstance(seq, Sequence):
         feature = seq.feature
     else:
         feature = seq[0]
     if isinstance(feature, dict):
         return False
```

### Comparing `deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.8.9/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/pytorch/common.py` & `deeplake-3.8.9/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.8.9/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.8.9/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.8.9/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/tf/common.py` & `deeplake-3.8.9/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.8.9/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.8.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/integrations/wandb/wandb.py` & `deeplake-3.8.9/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/tests/cache_fixtures.py` & `deeplake-3.8.9/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/tests/client_fixtures.py` & `deeplake-3.8.9/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/tests/common.py` & `deeplake-3.8.9/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/tests/dataset_fixtures.py` & `deeplake-3.8.9/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/tests/path_fixtures.py` & `deeplake-3.8.9/deeplake/tests/path_fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,35 +712,43 @@
 @pytest.fixture(scope="session")
 def dataframe_ingestion_data():
     return _download_hub_test_dataframe_data()
 
 
 @pytest.fixture
 def vector_store_hash_ids(request):
-    return [f"{i}" for i in range(5)]
+    if getattr(request, "param", True):
+        return [f"{i}" for i in range(5)]
 
 
 @pytest.fixture
 def vector_store_row_ids(request):
-    return [i for i in range(5)]
+    if getattr(request, "param", True):
+        return [i for i in range(5)]
 
 
 @pytest.fixture
 def vector_store_filter_udf(request):
-    return "filter_udf"
+    def filter_udf(x):
+        return x["metadata"].data()["value"] == {"a": 1}
+
+    if getattr(request, "param", True):
+        return filter_udf
 
 
 @pytest.fixture
 def vector_store_filters(request):
-    return {"a": 1}
+    if getattr(request, "param", True):
+        return {"metadata": {"a": 1}}
 
 
 @pytest.fixture
 def vector_store_query(request):
-    return "select * where metadata=={'a': 1}"
+    if getattr(request, "param", True):
+        return "select * where metadata['a']==1"
 
 
 @pytest.fixture
 def jobs_list():
     parent = get_dummy_data_path("deep_memory")
 
     with open(os.path.join(parent, "jobs_list.txt"), "r") as f:
```

### Comparing `deeplake-3.8.8/deeplake/tests/storage_fixtures.py` & `deeplake-3.8.9/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/access_method.py` & `deeplake-3.8.9/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/agreement.py` & `deeplake-3.8.9/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/array_list.py` & `deeplake-3.8.9/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/assert_byte_indexes.py` & `deeplake-3.8.9/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/auto.py` & `deeplake-3.8.9/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/bugout_reporter.py` & `deeplake-3.8.9/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/cache_chain.py` & `deeplake-3.8.9/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/casting.py` & `deeplake-3.8.9/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/check_latest_version.py` & `deeplake-3.8.9/deeplake/util/check_latest_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import warnings
-import requests
+import requests  # type: ignore
 from deeplake.client.config import HUB_PYPI_VERSION_PATH
 from deeplake.core.fast_forwarding import version_compare
 import time
 
 
 def get_latest_version():
     if os.path.exists(HUB_PYPI_VERSION_PATH):
```

### Comparing `deeplake-3.8.8/deeplake/util/chunk_engine.py` & `deeplake-3.8.9/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/class_label.py` & `deeplake-3.8.9/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/compute.py` & `deeplake-3.8.9/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/connect_dataset.py` & `deeplake-3.8.9/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/dataset.py` & `deeplake-3.8.9/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/diff.py` & `deeplake-3.8.9/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/downsample.py` & `deeplake-3.8.9/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/encoder.py` & `deeplake-3.8.9/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/exceptions.py` & `deeplake-3.8.9/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/exif.py` & `deeplake-3.8.9/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/from_tfds.py` & `deeplake-3.8.9/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/htype.py` & `deeplake-3.8.9/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/image.py` & `deeplake-3.8.9/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/invalid_view_op.py` & `deeplake-3.8.9/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/iteration_warning.py` & `deeplake-3.8.9/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/json.py` & `deeplake-3.8.9/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/keys.py` & `deeplake-3.8.9/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/link.py` & `deeplake-3.8.9/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/logging.py` & `deeplake-3.8.9/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/merge.py` & `deeplake-3.8.9/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/modified.py` & `deeplake-3.8.9/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/notebook.py` & `deeplake-3.8.9/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/mesh.py` & `deeplake-3.8.9/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.8.9/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.8.9/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.8.9/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.8.9/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/path.py` & `deeplake-3.8.9/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/pretty_print.py` & `deeplake-3.8.9/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/remove_cache.py` & `deeplake-3.8.9/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/scheduling.py` & `deeplake-3.8.9/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/shape_interval.py` & `deeplake-3.8.9/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/spinner.py` & `deeplake-3.8.9/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/split.py` & `deeplake-3.8.9/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/storage.py` & `deeplake-3.8.9/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tag.py` & `deeplake-3.8.9/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tensor_db.py` & `deeplake-3.8.9/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/testing.py` & `deeplake-3.8.9/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_auto.py` & `deeplake-3.8.9/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.8.9/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.8.9/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_keys.py` & `deeplake-3.8.9/deeplake/util/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_read.py` & `deeplake-3.8.9/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.8.9/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_split.py` & `deeplake-3.8.9/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.8.9/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/tests/test_version_control.py` & `deeplake-3.8.9/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/transform.py` & `deeplake-3.8.9/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/version_control.py` & `deeplake-3.8.9/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/util/video.py` & `deeplake-3.8.9/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/visualizer/video_streaming.py` & `deeplake-3.8.9/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake/visualizer/visualizer.py` & `deeplake-3.8.9/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.8.8/deeplake.egg-info/PKG-INFO` & `deeplake-3.8.9/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.8.8
+Version: 3.8.9
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.8.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.8.9 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.8.8/deeplake.egg-info/SOURCES.txt` & `deeplake-3.8.9/deeplake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -191,23 +191,26 @@
 deeplake/core/tiling/test_serialize.py
 deeplake/core/transform/__init__.py
 deeplake/core/transform/test_transform.py
 deeplake/core/transform/transform.py
 deeplake/core/transform/transform_dataset.py
 deeplake/core/transform/transform_tensor.py
 deeplake/core/vectorstore/__init__.py
-deeplake/core/vectorstore/deep_memory.py
 deeplake/core/vectorstore/deeplake_vectorstore.py
-deeplake/core/vectorstore/deepmemory_vectorstore.py
-deeplake/core/vectorstore/embedder.py
 deeplake/core/vectorstore/test_deeplake_vectorstore.py
-deeplake/core/vectorstore/test_deepmemory.py
-deeplake/core/vectorstore/test_embedder.py
-deeplake/core/vectorstore/unsupported_deep_memory.py
-deeplake/core/vectorstore/vectorstore_factory.py
+deeplake/core/vectorstore/dataset_handlers/__init__.py
+deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
+deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
+deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
+deeplake/core/vectorstore/deep_memory/__init__.py
+deeplake/core/vectorstore/deep_memory/deep_memory.py
+deeplake/core/vectorstore/deep_memory/test_deepmemory.py
+deeplake/core/vectorstore/embeddings/__init__.py
+deeplake/core/vectorstore/embeddings/embedder.py
+deeplake/core/vectorstore/embeddings/test_embedder.py
 deeplake/core/vectorstore/vector_search/__init__.py
 deeplake/core/vectorstore/vector_search/utils.py
 deeplake/core/vectorstore/vector_search/vector_search.py
 deeplake/core/vectorstore/vector_search/dataset/__init__.py
 deeplake/core/vectorstore/vector_search/dataset/dataset.py
 deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
 deeplake/core/vectorstore/vector_search/filter/__init__.py
```

### Comparing `deeplake-3.8.8/deeplake.egg-info/requires.txt` & `deeplake-3.8.9/deeplake.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 libdeeplake==0.0.90
 
 [:python_version >= "3.7" and sys_platform != "win32"]
 aioboto3>=10.4.0
 nest_asyncio
 
 [all]
-azure-identity
-nibabel
-google-api-python-client~=2.31.0
 azure-storage-blob
+google-api-python-client~=2.31.0
 oauth2client~=4.1.3
+laspy
+flask
+nibabel
+google-auth~=2.0.1
+azure-identity
 pydicom
 IPython
-google-auth~=2.0.1
-google-cloud-storage~=1.42.0
-google-auth-oauthlib~=0.4.5
 azure-cli
-laspy
-flask
+google-auth-oauthlib~=0.4.5
+google-cloud-storage~=1.42.0
 libdeeplake==0.0.90
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
```

### Comparing `deeplake-3.8.8/setup.py` & `deeplake-3.8.9/setup.py`

 * *Files identical despite different names*

