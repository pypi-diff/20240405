# Comparing `tmp/geoseeq-0.5.6a7.tar.gz` & `tmp/geoseeq-0.5.6a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.5.6a7.tar", last modified: Tue Apr  2 20:05:16 2024, max compression
+gzip compressed data, was "geoseeq-0.5.6a8.tar", last modified: Fri Apr  5 16:51:54 2024, max compression
```

## Comparing `geoseeq-0.5.6a7.tar` & `geoseeq-0.5.6a8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.495727 geoseeq-0.5.6a7/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a7/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-02 20:05:16.495451 geoseeq-0.5.6a7/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a7/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.476668 geoseeq-0.5.6a7/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a7/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a7/geoseeq/app.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a7/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a7/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.481531 geoseeq-0.5.6a7/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/detail.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a7/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a7/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/get_eula.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3259 2024-04-02 20:05:10.000000 geoseeq-0.5.6a7/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/manage.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a7/geoseeq/cli/progress_bar.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/run.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/search.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.483485 geoseeq-0.5.6a7/geoseeq/cli/shared_params/
--rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/common_state.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/config.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/id_handlers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/obj_getters.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a7/geoseeq/cli/shared_params/opts_and_args.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.484640 geoseeq-0.5.6a7/geoseeq/cli/upload/
--rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a7/geoseeq/cli/upload/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8963 2024-03-18 23:39:08.000000 geoseeq-0.5.6a7/geoseeq/cli/upload/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a7/geoseeq/cli/upload/upload_advanced.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7264 2024-03-19 00:09:27.000000 geoseeq-0.5.6a7/geoseeq/cli/upload/upload_reads.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a7/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a7/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a7/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a7/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.484923 geoseeq-0.5.6a7/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.486046 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4101 2024-03-21 02:53:18.000000 geoseeq-0.5.6a7/geoseeq/file_system_cache.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.488084 geoseeq-0.5.6a7/geoseeq/id_constructors/
--rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/from_blobs.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/from_ids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/from_names.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/from_uuids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/resolvers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a7/geoseeq/id_constructors/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a7/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a7/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a7/geoseeq/pipeline.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.489118 geoseeq-0.5.6a7/geoseeq/plotting/
--rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a7/geoseeq/plotting/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a7/geoseeq/plotting/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a7/geoseeq/plotting/highcharts.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.490297 geoseeq-0.5.6a7/geoseeq/plotting/map/
--rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a7/geoseeq/plotting/map/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a7/geoseeq/plotting/map/base_layer.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a7/geoseeq/plotting/map/map.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a7/geoseeq/plotting/map/overlay.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a7/geoseeq/plotting/selectable.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a7/geoseeq/project.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7131 2024-04-02 19:52:31.000000 geoseeq-0.5.6a7/geoseeq/remote_object.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.492171 geoseeq-0.5.6a7/geoseeq/result/
--rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a7/geoseeq/result/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a7/geoseeq/result/bioinfo.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5568 2024-04-02 20:04:55.000000 geoseeq-0.5.6a7/geoseeq/result/file_download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7390 2024-03-18 21:44:44.000000 geoseeq-0.5.6a7/geoseeq/result/file_upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a7/geoseeq/result/result_file.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a7/geoseeq/result/result_folder.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a7/geoseeq/result/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a7/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a7/geoseeq/search.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7090 2024-03-19 13:53:30.000000 geoseeq-0.5.6a7/geoseeq/upload_download_manager.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a7/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.494067 geoseeq-0.5.6a7/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a7/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a7/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a7/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a7/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a7/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a7/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a7/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.495074 geoseeq-0.5.6a7/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-02 20:05:16.000000 geoseeq-0.5.6a7/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-02 20:05:16.000000 geoseeq-0.5.6a7/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-02 20:05:16.000000 geoseeq-0.5.6a7/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-02 20:05:16.000000 geoseeq-0.5.6a7/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-02 20:05:16.000000 geoseeq-0.5.6a7/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-02 20:05:06.000000 geoseeq-0.5.6a7/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-02 20:05:16.495781 geoseeq-0.5.6a7/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-02 20:05:00.000000 geoseeq-0.5.6a7/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-02 20:05:16.494715 geoseeq-0.5.6a7/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a7/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a7/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a7/tests/test_plotting.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.583830 geoseeq-0.5.6a8/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/LICENSE
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 16:51:54.583407 geoseeq-0.5.6a8/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a8/README.md
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.552427 geoseeq-0.5.6a8/geoseeq/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a8/geoseeq/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a8/geoseeq/app.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a8/geoseeq/blob_constructors.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/bulk_creators.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.560518 geoseeq-0.5.6a8/geoseeq/cli/
+-rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/cli/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/cli/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/copy.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/detail.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a8/geoseeq/cli/download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a8/geoseeq/cli/fastq_utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/get_eula.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3259 2024-04-05 16:51:46.000000 geoseeq-0.5.6a8/geoseeq/cli/main.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/manage.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a8/geoseeq/cli/progress_bar.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/run.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/search.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.563403 geoseeq-0.5.6a8/geoseeq/cli/shared_params/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/common_state.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/config.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/id_handlers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/obj_getters.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/opts_and_args.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.565222 geoseeq-0.5.6a8/geoseeq/cli/upload/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9035 2024-04-05 16:48:06.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload_advanced.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7303 2024-04-05 16:48:16.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload_reads.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a8/geoseeq/cli/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/cli/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/view.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a8/geoseeq/constants.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.565802 geoseeq-0.5.6a8/geoseeq/contrib/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/__init__.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.567462 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/api.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/bioproject.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/setup_logging.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4138 2024-04-05 15:21:33.000000 geoseeq-0.5.6a8/geoseeq/file_system_cache.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.571229 geoseeq-0.5.6a8/geoseeq/id_constructors/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_blobs.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_ids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_names.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_uuids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/resolvers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a8/geoseeq/knex.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/organization.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a8/geoseeq/pipeline.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.573017 geoseeq-0.5.6a8/geoseeq/plotting/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a8/geoseeq/plotting/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a8/geoseeq/plotting/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a8/geoseeq/plotting/highcharts.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.574543 geoseeq-0.5.6a8/geoseeq/plotting/map/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/base_layer.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/map.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/overlay.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a8/geoseeq/plotting/selectable.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a8/geoseeq/project.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7131 2024-04-02 19:52:31.000000 geoseeq-0.5.6a8/geoseeq/remote_object.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.577933 geoseeq-0.5.6a8/geoseeq/result/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/result/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/result/bioinfo.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5568 2024-04-02 20:04:55.000000 geoseeq-0.5.6a8/geoseeq/result/file_download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11496 2024-04-05 16:47:18.000000 geoseeq-0.5.6a8/geoseeq/result/file_upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a8/geoseeq/result/result_file.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a8/geoseeq/result/result_folder.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a8/geoseeq/result/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a8/geoseeq/sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a8/geoseeq/search.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7206 2024-04-05 16:46:50.000000 geoseeq-0.5.6a8/geoseeq/upload_download_manager.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a8/geoseeq/utils.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.581246 geoseeq-0.5.6a8/geoseeq/vc/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a8/geoseeq/vc/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a8/geoseeq/vc/checksum.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a8/geoseeq/vc/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/clone.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_dir.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_stub.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.582995 geoseeq-0.5.6a8/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/SOURCES.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/dependency_links.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/entry_points.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/top_level.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-05 16:51:38.000000 geoseeq-0.5.6a8/pyproject.toml
+-rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-05 16:51:54.583901 geoseeq-0.5.6a8/setup.cfg
+-rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-02 20:05:00.000000 geoseeq-0.5.6a8/setup.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.582338 geoseeq-0.5.6a8/tests/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a8/tests/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a8/tests/test_api_client.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a8/tests/test_plotting.py
```

### Comparing `geoseeq-0.5.6a7/LICENSE` & `geoseeq-0.5.6a8/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/PKG-INFO` & `geoseeq-0.5.6a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a7
+Version: 0.5.6a8
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a7/README.md` & `geoseeq-0.5.6a8/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/__init__.py` & `geoseeq-0.5.6a8/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/app.py` & `geoseeq-0.5.6a8/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/bulk_creators.py` & `geoseeq-0.5.6a8/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/copy.py` & `geoseeq-0.5.6a8/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/detail.py` & `geoseeq-0.5.6a8/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/download.py` & `geoseeq-0.5.6a8/geoseeq/cli/download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/fastq_utils.py` & `geoseeq-0.5.6a8/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/get_eula.py` & `geoseeq-0.5.6a8/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/main.py` & `geoseeq-0.5.6a8/geoseeq/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.5.6a7')  # remember to update setup
+    click.echo('0.5.6a8')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
```

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/manage.py` & `geoseeq-0.5.6a8/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/progress_bar.py` & `geoseeq-0.5.6a8/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/run.py` & `geoseeq-0.5.6a8/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/search.py` & `geoseeq-0.5.6a8/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.5.6a8/geoseeq/cli/shared_params/common_state.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/shared_params/config.py` & `geoseeq-0.5.6a8/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.5.6a8/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.5.6a8/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.5.6a8/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/upload/__init__.py` & `geoseeq-0.5.6a8/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/upload/upload.py` & `geoseeq-0.5.6a8/geoseeq/cli/upload/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         name_pairs = zip([basename(fp) for fp in file_paths], file_paths)
     
     upload_manager = GeoSeeqUploadManager(
         n_parallel_uploads=cores,
         link_type=link_type,
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=state.log_level,
-        overwrite=True
+        overwrite=True,
+        use_cache=state.use_cache,
     )
     for geoseeq_file_name, file_path in name_pairs:
         if isfile(file_path):
             upload_manager.add_local_file_to_result_folder(result_folder, file_path)
         elif isdir(file_path) and recursive:
             upload_manager.add_local_folder_to_result_folder(result_folder, file_path, recursive=recursive, hidden_files=hidden, prefix=file_path)
         elif isdir(file_path) and not recursive:
@@ -136,15 +137,16 @@
     knex = state.get_knex()
     root_obj = handle_project_or_sample_id(knex, project_or_sample_id, yes=yes, private=private)
     upload_manager = GeoSeeqUploadManager(
         n_parallel_uploads=cores,
         link_type='upload',
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=logging.INFO,
-        overwrite=True
+        overwrite=True,
+        use_cache=state.use_cache,
     )
     for folder_name in folder_names:
         result_folder = root_obj.result_folder(folder_name).idem()
         upload_manager.add_local_folder_to_result_folder(result_folder, folder_name, recursive=recursive, hidden_files=hidden)
     click.echo(upload_manager.get_preview_string(), err=True)
     if not yes:
         click.confirm('Continue?', abort=True)
```

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.5.6a8/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.5.6a8/geoseeq/cli/upload/upload_reads.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         upload_manager = GeoSeeqUploadManager(
             n_parallel_uploads=cores,
             session=session,
             link_type=link_type,
             log_level=state.log_level,
             overwrite=overwrite,
             progress_tracker_factory=PBarManager().get_new_bar,
+            use_cache=state.use_cache,
         )
         for group in groups:
             sample = lib.sample(group['sample_name']).idem()
             read_folder = sample.result_folder(module_name).idem()
             for field_name, path in group['fields'].items():
                 result_file = read_folder.read_file(field_name)
                 upload_manager.add_result_file(result_file, filepaths[path])
```

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/user.py` & `geoseeq-0.5.6a8/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/utils.py` & `geoseeq-0.5.6a8/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/cli/view.py` & `geoseeq-0.5.6a8/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/file_system_cache.py` & `geoseeq-0.5.6a8/geoseeq/file_system_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger.addHandler(logging.NullHandler())  # No output unless configured by calling program
 CACHED_BLOB_TIME = 5 * 60 # 5 minutes in seconds
 CACHE_DIR = join(
     os.environ.get('XDG_CACHE_HOME', join(os.environ["HOME"], ".cache")),
     "geoseeq"
 )
 USE_GEOSEEQ_CACHE = None
-
+GEOSEEQ_CACHE_DIR = abspath(f'{CACHE_DIR}/geoseeq_api_cache/v1/')
 
 def hash_obj(obj):
     val = obj
     if not isinstance(obj, str):
         val = obj.pre_hash()
     result = sha256(val.encode())
     result = result.hexdigest()
@@ -37,15 +37,15 @@
     def __init__(self, timeout=CACHED_BLOB_TIME):
         self.timeout = timeout
         self._no_cache = False
         self.setup()
 
     @property
     def cache_dir_path(self):
-        return abspath(f'{CACHE_DIR}/geoseeq_api_cache/v1/')
+        return GEOSEEQ_CACHE_DIR
 
     def setup(self):
         if self.no_cache:
             return
         try:
             os.makedirs(self.cache_dir_path, exist_ok=True)
             open(join(self.cache_dir_path, 'flag'), 'w').close()
```

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/from_blobs.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/from_ids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/from_names.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/id_constructors/utils.py` & `geoseeq-0.5.6a8/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/knex.py` & `geoseeq-0.5.6a8/geoseeq/knex.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/organization.py` & `geoseeq-0.5.6a8/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/pipeline.py` & `geoseeq-0.5.6a8/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/plotting/highcharts.py` & `geoseeq-0.5.6a8/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.5.6a8/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/plotting/map/map.py` & `geoseeq-0.5.6a8/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/plotting/map/overlay.py` & `geoseeq-0.5.6a8/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/plotting/selectable.py` & `geoseeq-0.5.6a8/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/project.py` & `geoseeq-0.5.6a8/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/remote_object.py` & `geoseeq-0.5.6a8/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/result/bioinfo.py` & `geoseeq-0.5.6a8/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/result/file_download.py` & `geoseeq-0.5.6a8/geoseeq/result/file_download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/result/file_upload.py` & `geoseeq-0.5.6a8/geoseeq/upload_download_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,177 +1,176 @@
-
-import time
-import json
-from os.path import basename, getsize
-from pathlib import Path
-
-import requests
-
-from geoseeq.knex import GeoseeqGeneralError
-from geoseeq.constants import FIVE_MB
-from geoseeq.utils import md5_checksum
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from .utils import *
-
-
-class FileChunker:
-
-    def __init__(self, filepath, chunk_size):
-        self.filepath = filepath
-        self.chunk_size = chunk_size
-        self.file_size = getsize(filepath)
-        self.n_parts = int(self.file_size / self.chunk_size) + 1
-        self.loaded_parts = []
-
-    def load_all_chunks(self):
-        if len(self.loaded_parts) != self.n_parts:
-            with open(self.filepath, "rb") as f:
-                f.seek(0)
-                for i in range(self.n_parts):
-                    chunk = f.read(self.chunk_size)
-                    self.loaded_parts.append(chunk)
-        return self  # convenience for chaining
-
-    def get_chunk(self, num):
-        self.load_all_chunks()
-        return self.loaded_parts[num]
-    
-    def get_chunk_size(self, num):
-        self.load_all_chunks()
-        return len(self.loaded_parts[num])
-
-
-class ResultFileUpload:
-    """Abstract class that handles upload methods for result files."""
-
-    def _create_multipart_upload(self, filepath, file_size, optional_fields):
-        optional_fields = optional_fields if optional_fields else {}
-        optional_fields.update(
-            {
-                "md5_checksum": md5_checksum(filepath),
-                "file_size_bytes": file_size,
-            }
-        )
-        data = {
-            "filename": basename(filepath),
-            "optional_fields": optional_fields,
-            "result_type": "sample" if self.is_sample_result else "group",
-        }
-        response = self.knex.post(f"/ar_fields/{self.uuid}/create_upload", json=data)
-        return response
+import logging
+from multiprocessing import Pool, current_process
+from os.path import basename, join, dirname
+from geoseeq.result import ResultFile
+from geoseeq.result.file_download import download_url
+from os import makedirs
+
+logger = logging.getLogger('geoseeq_api')
+logger.addHandler(logging.NullHandler())  # No output unless configured by calling program
+
+
+def _make_in_process_logger(log_level):
+    logger = logging.getLogger('geoseeq_api')
+    logger.setLevel(log_level)
+    handler = logging.StreamHandler()
+    handler.setFormatter(logging.Formatter('[%(levelname)s] %(name)s :: ' + current_process().name + ' :: %(message)s'))
+    logger.addHandler(handler)
+    return logger
+
+
+def _upload_one_file(args):
+    result_file, filepath, session, progress_tracker, link_type, overwrite, log_level, parallel_uploads, use_cache = args
+    if parallel_uploads:
+        _make_in_process_logger(log_level)
+    if link_type == 'upload':
+        # TODO: check checksums to see if the file is the same
+        result_file.upload_file(filepath, session=session, overwrite=overwrite, progress_tracker=progress_tracker, threads=4, use_cache=use_cache)
+    else:
+        result_file.link_file(link_type, filepath)
+    return result_file
+
+
+class GeoSeeqUploadManager:
+
+    def __init__(self,
+                 n_parallel_uploads=1,
+                 session=None,
+                 link_type='upload',
+                 progress_tracker_factory=None,
+                 log_level=logging.WARNING,
+                 overwrite=True,
+                 use_cache=True):
+        self.session = session
+        self.n_parallel_uploads = n_parallel_uploads
+        self.progress_tracker_factory = progress_tracker_factory if progress_tracker_factory else lambda x: None
+        self.log_level = log_level
+        self.link_type = link_type
+        self.overwrite = overwrite
+        self._result_files = []
+        self.use_cache = use_cache
+
+    def add_result_file(self, result_file, local_path):
+        self._result_files.append((result_file, local_path))
+
+    def add_local_file_to_result_folder(self, result_folder, local_path, geoseeq_file_name=None):
+        geoseeq_file_name = geoseeq_file_name if geoseeq_file_name else local_path
+        result_file = result_folder.result_file(geoseeq_file_name)
+        self.add_result_file(result_file, local_path)
+
+    def add_local_folder_to_result_folder(self, result_folder, local_path, recursive=False, hidden_files=False, prefix=""):
+        for result_file, local_path in result_folder._prepare_folder_upload(local_path, recursive, hidden_files, prefix):
+            self.add_result_file(result_file, local_path)
+
+    def get_preview_string(self):
+        out = ["Upload Preview:"]
+        for result_file, local_path in self._result_files:
+            out.append(f"{local_path} -> {result_file}")
+        return "\n".join(out)
+
+    def upload_files(self):
+        upload_args = [(
+                result_file, local_path,
+                self.session, self.progress_tracker_factory(local_path),
+                self.link_type, self.overwrite, self.log_level,
+                self.n_parallel_uploads > 1, self.use_cache
+            ) for result_file, local_path in self._result_files
+        ]
+        out = []
+        if self.n_parallel_uploads == 1:
+            logger.info(f"Uploading files in series.")
+            for upload_arg in upload_args:
+                out.append(_upload_one_file(upload_arg))
+        else:
+            logger.info(f"Uploading files in parallel with {self.n_parallel_uploads} threads.")
+            with Pool(self.n_parallel_uploads) as p:
+                for uploaded_result_file in p.imap_unordered(_upload_one_file, upload_args):
+                    out.append(uploaded_result_file)
+        return out
     
-    def _prep_multipart_upload(self, filepath, file_size, chunk_size, optional_fields):
-        n_parts = int(file_size / chunk_size) + 1
-        response = self._create_multipart_upload(filepath, file_size, optional_fields)
-        upload_id = response["upload_id"]
-        parts = list(range(1, n_parts + 1))
-        data = {
-            "parts": parts,
-            "stance": "upload-multipart",
-            "upload_id": upload_id,
-            "result_type": "sample" if self.is_sample_result else "group",
-        }
-        response = self.knex.post(f"/ar_fields/{self.uuid}/create_upload_urls", json=data)
-        urls = response
-        return upload_id, urls
+    def __len__(self):
+        return len(self._result_files)
+
+
+def _download_one_file(args):
+    url, file_path, pbar, ignore_errors, head, log_level, parallel_downloads = args
+    if parallel_downloads:
+        _make_in_process_logger(log_level)
+    if isinstance(url, ResultFile):
+        url = url.get_download_url()
+    try:
+        if dirname(file_path):
+            makedirs(dirname(file_path), exist_ok=True)
+        return download_url(url, filename=file_path, progress_tracker=pbar, head=head)
+    except Exception as e:
+        if ignore_errors:
+            logger.error(f"Error downloading {url}: {e}")
+        else:
+            raise e
+        
+
+class GeoSeeqDownloadManager:
+
+    def __init__(self, n_parallel_downloads=1, ignore_errors=False, head=False, progress_tracker_factory=None, log_level=logging.WARNING):
+        self.n_parallel_downloads = n_parallel_downloads
+        self.ignore_errors = ignore_errors
+        self.head = head
+        self.progress_tracker_factory = progress_tracker_factory if progress_tracker_factory else lambda x: None
+        self.log_level = log_level
+        self._result_files = []
+
+    def add_download(self, url, file_path=None, progress_tracker=None):
+        if not file_path:
+            if isinstance(url, ResultFile):
+                file_path = url.get_local_filename()
+            else:
+                raise ValueError("file_path must be provided if url is not a ResultFile object.")
+        self._result_files.append((url, file_path))
+
+
+    def add_result_folder_download(self, result_folder, local_folder_path, hidden_files=True):
+        for result_file in result_folder.get_result_files():
+            if not hidden_files and result_file.name.startswith("."):
+                continue
+            self.add_download(result_file, join(local_folder_path, result_file.get_local_filename()))
+
+    def get_preview_string(self):
+        out = ["Download Preview:"]
+        for url, file_path in self._result_files:
+            out.append(f"{url} -> {file_path}")
+        return "\n".join(out)
     
-    def _upload_one_part(self, file_chunker, url, num, max_retries, session=None):
-        file_chunk = file_chunker.get_chunk(num)
-        attempts = 0
-        while attempts < max_retries:
-            try:
-                if session:
-                    http_response = session.put(url, data=file_chunk)
-                else:
-                    http_response = requests.put(url, data=file_chunk)
-                http_response.raise_for_status()
-                logger.debug(f"Upload for part {num + 1} succeeded.")
-                break
-            except requests.exceptions.HTTPError:
-                logger.warn(
-                    f"Upload for part {num + 1} failed. Attempt {attempts + 1} of {max_retries}."
-                )
-                attempts += 1
-                if attempts == max_retries:
-                    raise
-                time.sleep(10**attempts)  # exponential backoff, (10 ** 2)s default max
-        return {"ETag": http_response.headers["ETag"], "PartNumber": num + 1}
+    def get_url_string(self):
+        self._convert_result_files_to_urls()
+        out = []
+        for url, _ in self._result_files:
+            out.append(url)
+        return "\n".join(out)
     
-    def _finish_multipart_upload(self, upload_id, complete_parts):
-        response = self.knex.post(
-            f"/ar_fields/{self.uuid}/complete_upload",
-            json={
-                "parts": complete_parts,
-                "upload_id": upload_id,
-                "result_type": "sample" if self.is_sample_result else "group",
-            },
-            json_response=False,
-        )
-        response.raise_for_status()
-
-    def _upload_parts(self, file_chunker, urls, max_retries, session, progress_tracker, threads):
-        if threads == 1:
-            logger.info(f"Uploading parts in series for {file_chunker.filepath}")
-            complete_parts = []
-            for num, url in enumerate(list(urls.values())):
-                response_part = self._upload_one_part(file_chunker, url, num, max_retries, session)
-                complete_parts.append(response_part)
-                if progress_tracker: progress_tracker.update(file_chunker.get_chunk_size(num))
-                logger.info(f'Uploaded part {num + 1} of {len(urls)} for "{file_chunker.filepath}"')
-            return complete_parts
-        
-        with ThreadPoolExecutor(max_workers=threads) as executor:
-            logger.info(f"Uploading parts in parallel for {file_chunker.filepath} with {threads} threads.")
-            futures = []
-            for num, url in enumerate(list(urls.values())):
-                future = executor.submit(
-                    self._upload_one_part, file_chunker, url, num, max_retries, session
-                )
-                futures.append(future)
-            complete_parts = []
-            for future in as_completed(futures):
-                response_part = future.result()
-                complete_parts.append(response_part)
-                if progress_tracker: progress_tracker.update(file_chunker.get_chunk_size(response_part["PartNumber"] - 1))
-                logger.info(
-                    f'Uploaded part {response_part["PartNumber"]} of {len(urls)} for "{file_chunker.filepath}"'
-                )
-        complete_parts = sorted(complete_parts, key=lambda x: x["PartNumber"])
-        return complete_parts
-
-    def multipart_upload_file(
-        self,
-        filepath,
-        file_size,
-        optional_fields=None,
-        chunk_size=FIVE_MB,
-        max_retries=3,
-        session=None,
-        progress_tracker=None,
-        threads=1,
-    ):
-        """Upload a file to S3 using the multipart upload process."""
-        logger.info(f"Uploading {filepath} to S3 using multipart upload.")
-        upload_id, urls = self._prep_multipart_upload(filepath, file_size, chunk_size, optional_fields)
-        logger.info(f'Starting upload for "{filepath}"')
-        complete_parts = []
-        file_chunker = FileChunker(filepath, chunk_size).load_all_chunks()
-        if progress_tracker: progress_tracker.set_num_chunks(file_chunker.file_size)
-        complete_parts = self._upload_parts(file_chunker, urls, max_retries, session, progress_tracker, threads)
-        self._finish_multipart_upload(upload_id, complete_parts)
-        logger.info(f'Finished Upload for "{filepath}"')
-        return self
-
-    def upload_file(self, filepath, multipart_thresh=FIVE_MB, overwrite=True, **kwargs):
-        if self.exists() and not overwrite:  
-            raise GeoseeqGeneralError(f"Overwrite is set to False and file {self.uuid} already exists.")
-        self.idem()
-        resolved_path = Path(filepath).resolve()
-        file_size = getsize(resolved_path)
-        return self.multipart_upload_file(filepath, file_size, **kwargs)
+    def __len__(self):
+        return len(self._result_files)
     
-    def upload_json(self, data, **kwargs):
-        """Upload a file with the given data as JSON."""
-        with NamedTemporaryFile("w", suffix='.json') as f:
-            json.dump(data, f)
-            f.flush()
-            return self.upload_file(f.name, **kwargs)
+    def _convert_result_files_to_urls(self):
+        self._result_files = [(
+            url.get_download_url() if isinstance(url, ResultFile) else url,
+            file_path,
+        ) for url, file_path in self._result_files]
+
+    def download_files(self):
+        self._convert_result_files_to_urls()
+        download_args = [(
+            url, file_path,
+            self.progress_tracker_factory(url),
+            self.ignore_errors, self.head, self.log_level,
+            self.n_parallel_downloads > 1
+        ) for url, file_path in self._result_files]
+        out = []
+        if self.n_parallel_downloads == 1:
+            logger.info(f"Downloading files in series.")
+            for download_arg in download_args:
+                out.append(_download_one_file(download_arg))
+        else:
+            logger.info(f"Downloading files in parallel with {self.n_parallel_downloads} threads.")
+            with Pool(self.n_parallel_downloads) as p:
+                for downloaded_file in p.imap_unordered(_download_one_file, download_args):
+                    out.append(downloaded_file)
+        return out
```

### Comparing `geoseeq-0.5.6a7/geoseeq/result/result_file.py` & `geoseeq-0.5.6a8/geoseeq/result/result_file.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/result/result_folder.py` & `geoseeq-0.5.6a8/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/result/utils.py` & `geoseeq-0.5.6a8/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/sample.py` & `geoseeq-0.5.6a8/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/search.py` & `geoseeq-0.5.6a8/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/user.py` & `geoseeq-0.5.6a8/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/utils.py` & `geoseeq-0.5.6a8/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/checksum.py` & `geoseeq-0.5.6a8/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/cli.py` & `geoseeq-0.5.6a8/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/clone.py` & `geoseeq-0.5.6a8/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/vc_cache.py` & `geoseeq-0.5.6a8/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/vc_sample.py` & `geoseeq-0.5.6a8/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/vc/vc_stub.py` & `geoseeq-0.5.6a8/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq/work_orders.py` & `geoseeq-0.5.6a8/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.5.6a8/geoseeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a7
+Version: 0.5.6a8
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a7/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.5.6a8/geoseeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/pyproject.toml` & `geoseeq-0.5.6a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.5.6a7"
+version = "0.5.6a8"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.5.6a7/setup.py` & `geoseeq-0.5.6a8/setup.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/tests/test_api_client.py` & `geoseeq-0.5.6a8/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a7/tests/test_plotting.py` & `geoseeq-0.5.6a8/tests/test_plotting.py`

 * *Files identical despite different names*

