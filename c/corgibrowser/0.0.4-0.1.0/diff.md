# Comparing `tmp/corgibrowser-0.0.4.tar.gz` & `tmp/corgibrowser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgibrowser-0.0.4.tar", last modified: Mon Mar 25 08:33:12 2024, max compression
+gzip compressed data, was "corgibrowser-0.1.0.tar", last modified: Fri Apr  5 07:55:37 2024, max compression
```

## Comparing `corgibrowser-0.0.4.tar` & `corgibrowser-0.1.0.tar`

### file list

```diff
@@ -1,102 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.531736 corgibrowser-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-03-24 01:38:53.000000 corgibrowser-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5216 2024-03-25 08:33:12.530732 corgibrowser-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-24 01:38:53.000000 corgibrowser-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.473725 corgibrowser-0.0.4/corgibrowser/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/corgibrowser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.486729 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/
--rw-rw-rw-   0        0        0        0 2024-02-07 08:22:09.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/__init__.py
--rw-rw-rw-   0        0        0    19471 2024-03-24 00:25:31.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/azure_direct_operations.py
--rw-rw-rw-   0        0        0    12568 2024-03-25 04:49:22.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/cloud_integration.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.487725 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/queues_schemas/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/queues_schemas/__init__.py
--rw-rw-rw-   0        0        0     2563 2024-03-23 21:00:54.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/queues_schemas/corgi_web_queue_version_1.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.490729 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/__init__.py
--rw-rw-rw-   0        0        0      598 2024-03-24 00:02:10.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgi_hash_table.py
--rw-rw-rw-   0        0        0     1434 2024-03-23 23:25:40.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgi_web_entity.py
--rw-rw-rw-   0        0        0      745 2024-03-23 23:26:40.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgiweb_queuepreference.py
--rw-rw-rw-   0        0        0      867 2024-03-23 23:26:24.000000 corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgiweb_storage_analytics.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.493725 corgibrowser-0.0.4/corgibrowser/corgi_crawler/
--rw-rw-rw-   0        0        0     3786 2024-03-23 23:02:16.000000 corgibrowser-0.0.4/corgibrowser/corgi_crawler/RobotsCache.py
--rw-rw-rw-   0        0        0        0 2024-02-07 22:18:34.000000 corgibrowser-0.0.4/corgibrowser/corgi_crawler/__init__.py
--rw-rw-rw-   0        0        0     7209 2024-03-25 07:38:47.000000 corgibrowser-0.0.4/corgibrowser/corgi_crawler/crawler.py
--rw-rw-rw-   0        0        0     7431 2024-03-25 07:52:30.000000 corgibrowser-0.0.4/corgibrowser/corgi_crawler/crawler_processor.py
--rw-rw-rw-   0        0        0     4934 2024-03-23 20:41:55.000000 corgibrowser-0.0.4/corgibrowser/corgi_crawler/visited_url_processor.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.494725 corgibrowser-0.0.4/corgibrowser/corgi_data_analytics_and_ai/
--rw-rw-rw-   0        0        0        0 2024-02-09 20:08:34.000000 corgibrowser-0.0.4/corgibrowser/corgi_data_analytics_and_ai/__init__.py
--rw-rw-rw-   0        0        0     4493 2024-03-23 17:41:01.000000 corgibrowser-0.0.4/corgibrowser/corgi_data_analytics_and_ai/data_analytics_and_ai.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.495730 corgibrowser-0.0.4/corgibrowser/corgi_datasets/
--rw-rw-rw-   0        0        0      827 2024-03-25 08:31:28.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/DataSetsManager.py
--rw-rw-rw-   0        0        0        0 2024-03-23 21:54:43.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.496729 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/
--rw-rw-rw-   0        0        0        0 2024-03-25 08:18:43.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.515725 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/
--rw-rw-rw-   0        0        0        0 2024-03-25 07:23:52.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/__init__.py
--rw-rw-rw-   0        0        0     4055 2024-03-25 08:03:12.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/arizona.py
--rw-rw-rw-   0        0        0      924 2024-03-25 08:02:23.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/arkansas.py
--rw-rw-rw-   0        0        0    17536 2024-03-25 08:11:36.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/california.py
--rw-rw-rw-   0        0        0     2662 2024-03-25 08:12:04.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/colorado.py
--rw-rw-rw-   0        0        0     1558 2024-03-25 08:12:32.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/connecticut.py
--rw-rw-rw-   0        0        0      392 2024-03-25 08:03:06.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/delaware.py
--rw-rw-rw-   0        0        0     5508 2024-03-25 08:21:51.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/extra.py
--rw-rw-rw-   0        0        0     1853 2024-03-25 08:22:41.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/georgia.py
--rw-rw-rw-   0        0        0      608 2024-03-25 08:13:26.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/hawaii.py
--rw-rw-rw-   0        0        0     4156 2024-03-25 08:14:06.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/illinois.py
--rw-rw-rw-   0        0        0     1645 2024-03-25 08:03:45.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/indiana.py
--rw-rw-rw-   0        0        0     1624 2024-03-25 08:04:15.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/iowa.py
--rw-rw-rw-   0        0        0      801 2024-03-25 08:04:39.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/kansas.py
--rw-rw-rw-   0        0        0     2535 2024-03-25 08:14:42.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/massachusetts.py
--rw-rw-rw-   0        0        0     2124 2024-03-25 08:05:14.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/mississippi.py
--rw-rw-rw-   0        0        0      810 2024-03-25 08:05:36.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/montana.py
--rw-rw-rw-   0        0        0      839 2024-03-25 08:06:04.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/nevada.py
--rw-rw-rw-   0        0        0      434 2024-03-25 08:06:35.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_hampshire.py
--rw-rw-rw-   0        0        0      434 2024-03-25 08:06:55.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_jersey.py
--rw-rw-rw-   0        0        0      615 2024-03-25 08:15:17.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_mexico.py
--rw-rw-rw-   0        0        0     7998 2024-03-25 08:15:52.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_york.py
--rw-rw-rw-   0        0        0     1558 2024-03-25 08:07:20.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/oregon.py
--rw-rw-rw-   0        0        0     4686 2024-03-25 08:16:25.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/pennsylvania.py
--rw-rw-rw-   0        0        0     1034 2024-03-25 08:08:55.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/rhode_island.py
--rw-rw-rw-   0        0        0      853 2024-03-25 08:09:24.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/south_dakota.py
--rw-rw-rw-   0        0        0     2153 2024-03-25 08:17:04.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/tennessee.py
--rw-rw-rw-   0        0        0     8864 2024-03-25 08:17:43.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/texas.py
--rw-rw-rw-   0        0        0     3190 2024-03-25 08:18:25.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/washington.py
--rw-rw-rw-   0        0        0     1044 2024-03-25 08:10:03.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/west_virginia.py
--rw-rw-rw-   0        0        0     2873 2024-03-25 08:10:42.000000 corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/wisconsin.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.517725 corgibrowser-0.0.4/corgibrowser/corgi_settings/
--rw-rw-rw-   0        0        0     1767 2024-03-25 05:01:45.000000 corgibrowser-0.0.4/corgibrowser/corgi_settings/SettingsManager.py
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/corgibrowser/corgi_settings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.520698 corgibrowser-0.0.4/corgibrowser/corgi_utils/
--rw-rw-rw-   0        0        0      418 2024-03-25 06:40:49.000000 corgibrowser-0.0.4/corgibrowser/corgi_utils/AsyncRequests.py
--rw-rw-rw-   0        0        0      241 2024-03-25 06:40:49.000000 corgibrowser-0.0.4/corgibrowser/corgi_utils/SyncRequests.py
--rw-rw-rw-   0        0        0        0 2024-03-23 01:15:45.000000 corgibrowser-0.0.4/corgibrowser/corgi_utils/__init__.py
--rw-rw-rw-   0        0        0     4071 2024-03-25 04:36:13.000000 corgibrowser-0.0.4/corgibrowser/corgi_utils/names_generator.py
--rw-rw-rw-   0        0        0      670 2024-03-24 00:37:57.000000 corgibrowser-0.0.4/corgibrowser/corgi_utils/url_hash.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.522730 corgibrowser-0.0.4/corgibrowser/corgi_webscraping/
--rw-rw-rw-   0        0        0        0 2024-02-15 01:40:53.000000 corgibrowser-0.0.4/corgibrowser/corgi_webscraping/__init__.py
--rw-rw-rw-   0        0        0    11306 2024-03-25 07:36:11.000000 corgibrowser-0.0.4/corgibrowser/corgi_webscraping/batch_scraper_processor.py
--rw-rw-rw-   0        0        0    14669 2024-03-23 23:53:36.000000 corgibrowser-0.0.4/corgibrowser/corgi_webscraping/default_scrape_template.py
--rw-rw-rw-   0        0        0     2857 2024-03-25 07:33:24.000000 corgibrowser-0.0.4/corgibrowser/corgi_webscraping/scraper.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.529734 corgibrowser-0.0.4/corgibrowser.egg-info/
--rw-rw-rw-   0        0        0     5216 2024-03-25 08:33:12.000000 corgibrowser-0.0.4/corgibrowser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3921 2024-03-25 08:33:12.000000 corgibrowser-0.0.4/corgibrowser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 08:33:12.000000 corgibrowser-0.0.4/corgibrowser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2926 2024-03-25 08:33:12.000000 corgibrowser-0.0.4/corgibrowser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-25 08:33:12.000000 corgibrowser-0.0.4/corgibrowser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 08:33:12.531736 corgibrowser-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-03-25 08:32:41.000000 corgibrowser-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.523735 corgibrowser-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.524734 corgibrowser-0.0.4/tests/test_cloud_integration/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/tests/test_cloud_integration/__init__.py
--rw-rw-rw-   0        0        0     2995 2024-03-25 07:44:34.000000 corgibrowser-0.0.4/tests/test_cloud_integration/test_add_urls_to_queue.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.526734 corgibrowser-0.0.4/tests/test_crawler/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/tests/test_crawler/__init__.py
--rw-rw-rw-   0        0        0     2445 2024-03-25 04:32:17.000000 corgibrowser-0.0.4/tests/test_crawler/test_crawler.py
--rw-rw-rw-   0        0        0     1844 2024-03-24 00:48:31.000000 corgibrowser-0.0.4/tests/test_crawler/test_robots_txt.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.527734 corgibrowser-0.0.4/tests/test_scraper/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/tests/test_scraper/__init__.py
--rw-rw-rw-   0        0        0     1273 2024-03-24 00:42:06.000000 corgibrowser-0.0.4/tests/test_scraper/test_scraper.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:33:12.528734 corgibrowser-0.0.4/tests/test_utils/
--rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.0.4/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0     2872 2024-03-23 23:26:49.000000 corgibrowser-0.0.4/tests/test_utils/test_names_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.646845 corgibrowser-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-03-24 01:38:53.000000 corgibrowser-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    10350 2024-04-05 07:55:37.645843 corgibrowser-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5074 2024-04-05 07:53:27.000000 corgibrowser-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.584533 corgibrowser-0.1.0/corgibrowser/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/corgibrowser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.598004 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/
+-rw-rw-rw-   0        0        0        0 2024-02-07 08:22:09.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/__init__.py
+-rw-rw-rw-   0        0        0    19471 2024-03-24 00:25:31.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/azure_direct_operations.py
+-rw-rw-rw-   0        0        0    12767 2024-04-04 07:16:51.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/cloud_integration.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.599001 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/queues_schemas/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/queues_schemas/__init__.py
+-rw-rw-rw-   0        0        0     2563 2024-03-23 21:00:54.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/queues_schemas/corgi_web_queue_version_1.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.603984 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-03-24 00:02:10.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_hash_table.py
+-rw-rw-rw-   0        0        0     1434 2024-03-23 23:25:40.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_web_entity.py
+-rw-rw-rw-   0        0        0      760 2024-04-04 07:03:06.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_web_request_log.py
+-rw-rw-rw-   0        0        0      759 2024-04-04 07:02:54.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_web_scrape_log.py
+-rw-rw-rw-   0        0        0      823 2024-04-04 07:12:57.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_web_trottling.py
+-rw-rw-rw-   0        0        0      745 2024-03-23 23:26:40.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgiweb_queuepreference.py
+-rw-rw-rw-   0        0        0      867 2024-03-23 23:26:24.000000 corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgiweb_storage_analytics.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.606978 corgibrowser-0.1.0/corgibrowser/corgi_crawler/
+-rw-rw-rw-   0        0        0     3786 2024-03-23 23:02:16.000000 corgibrowser-0.1.0/corgibrowser/corgi_crawler/RobotsCache.py
+-rw-rw-rw-   0        0        0        0 2024-02-07 22:18:34.000000 corgibrowser-0.1.0/corgibrowser/corgi_crawler/__init__.py
+-rw-rw-rw-   0        0        0     7209 2024-03-25 07:38:47.000000 corgibrowser-0.1.0/corgibrowser/corgi_crawler/crawler.py
+-rw-rw-rw-   0        0        0     7431 2024-03-25 07:52:30.000000 corgibrowser-0.1.0/corgibrowser/corgi_crawler/crawler_processor.py
+-rw-rw-rw-   0        0        0     4934 2024-03-23 20:41:55.000000 corgibrowser-0.1.0/corgibrowser/corgi_crawler/visited_url_processor.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.607970 corgibrowser-0.1.0/corgibrowser/corgi_data_analytics_and_ai/
+-rw-rw-rw-   0        0        0        0 2024-02-09 20:08:34.000000 corgibrowser-0.1.0/corgibrowser/corgi_data_analytics_and_ai/__init__.py
+-rw-rw-rw-   0        0        0     4493 2024-03-23 17:41:01.000000 corgibrowser-0.1.0/corgibrowser/corgi_data_analytics_and_ai/data_analytics_and_ai.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.608967 corgibrowser-0.1.0/corgibrowser/corgi_datasets/
+-rw-rw-rw-   0        0        0      827 2024-03-25 08:31:28.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/DataSetsManager.py
+-rw-rw-rw-   0        0        0        0 2024-03-23 21:54:43.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.608967 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/
+-rw-rw-rw-   0        0        0        0 2024-03-25 08:18:43.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.627908 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/
+-rw-rw-rw-   0        0        0        0 2024-03-25 07:23:52.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/__init__.py
+-rw-rw-rw-   0        0        0     4055 2024-03-25 08:03:12.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/arizona.py
+-rw-rw-rw-   0        0        0      924 2024-03-25 08:02:23.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/arkansas.py
+-rw-rw-rw-   0        0        0    17536 2024-03-25 08:11:36.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/california.py
+-rw-rw-rw-   0        0        0     2662 2024-03-25 08:12:04.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/colorado.py
+-rw-rw-rw-   0        0        0     1558 2024-03-25 08:12:32.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/connecticut.py
+-rw-rw-rw-   0        0        0      392 2024-03-25 08:03:06.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/delaware.py
+-rw-rw-rw-   0        0        0     5508 2024-03-25 08:21:51.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/extra.py
+-rw-rw-rw-   0        0        0     1853 2024-03-25 08:22:41.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/georgia.py
+-rw-rw-rw-   0        0        0      608 2024-03-25 08:13:26.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/hawaii.py
+-rw-rw-rw-   0        0        0     4156 2024-03-25 08:14:06.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/illinois.py
+-rw-rw-rw-   0        0        0     1645 2024-03-25 08:03:45.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/indiana.py
+-rw-rw-rw-   0        0        0     1624 2024-03-25 08:04:15.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/iowa.py
+-rw-rw-rw-   0        0        0      801 2024-03-25 08:04:39.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/kansas.py
+-rw-rw-rw-   0        0        0     2535 2024-03-25 08:14:42.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/massachusetts.py
+-rw-rw-rw-   0        0        0     2124 2024-03-25 08:05:14.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/mississippi.py
+-rw-rw-rw-   0        0        0      810 2024-03-25 08:05:36.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/montana.py
+-rw-rw-rw-   0        0        0      839 2024-03-25 08:06:04.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/nevada.py
+-rw-rw-rw-   0        0        0      434 2024-03-25 08:06:35.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_hampshire.py
+-rw-rw-rw-   0        0        0      434 2024-03-25 08:06:55.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_jersey.py
+-rw-rw-rw-   0        0        0      615 2024-03-25 08:15:17.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_mexico.py
+-rw-rw-rw-   0        0        0     7998 2024-03-25 08:15:52.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_york.py
+-rw-rw-rw-   0        0        0     1558 2024-03-25 08:07:20.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/oregon.py
+-rw-rw-rw-   0        0        0     4686 2024-03-25 08:16:25.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/pennsylvania.py
+-rw-rw-rw-   0        0        0     1034 2024-03-25 08:08:55.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/rhode_island.py
+-rw-rw-rw-   0        0        0      853 2024-03-25 08:09:24.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/south_dakota.py
+-rw-rw-rw-   0        0        0     2153 2024-03-25 08:17:04.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/tennessee.py
+-rw-rw-rw-   0        0        0     8864 2024-03-25 08:17:43.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/texas.py
+-rw-rw-rw-   0        0        0     3190 2024-03-25 08:18:25.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/washington.py
+-rw-rw-rw-   0        0        0     1044 2024-03-25 08:10:03.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/west_virginia.py
+-rw-rw-rw-   0        0        0     2873 2024-03-25 08:10:42.000000 corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/wisconsin.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.628900 corgibrowser-0.1.0/corgibrowser/corgi_settings/
+-rw-rw-rw-   0        0        0     1679 2024-04-05 06:58:44.000000 corgibrowser-0.1.0/corgibrowser/corgi_settings/SettingsManager.py
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/corgibrowser/corgi_settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.630894 corgibrowser-0.1.0/corgibrowser/corgi_social_media/
+-rw-rw-rw-   0        0        0      249 2024-03-26 07:15:42.000000 corgibrowser-0.1.0/corgibrowser/corgi_social_media/Meta.py
+-rw-rw-rw-   0        0        0      621 2024-03-26 05:43:43.000000 corgibrowser-0.1.0/corgibrowser/corgi_social_media/Twitter.py
+-rw-rw-rw-   0        0        0        0 2024-03-31 23:44:28.000000 corgibrowser-0.1.0/corgibrowser/corgi_social_media/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.634888 corgibrowser-0.1.0/corgibrowser/corgi_utils/
+-rw-rw-rw-   0        0        0      418 2024-03-25 06:40:49.000000 corgibrowser-0.1.0/corgibrowser/corgi_utils/AsyncRequests.py
+-rw-rw-rw-   0        0        0      241 2024-03-25 06:40:49.000000 corgibrowser-0.1.0/corgibrowser/corgi_utils/SyncRequests.py
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:15:45.000000 corgibrowser-0.1.0/corgibrowser/corgi_utils/__init__.py
+-rw-rw-rw-   0        0        0     4071 2024-03-25 04:36:13.000000 corgibrowser-0.1.0/corgibrowser/corgi_utils/names_generator.py
+-rw-rw-rw-   0        0        0      670 2024-03-24 00:37:57.000000 corgibrowser-0.1.0/corgibrowser/corgi_utils/url_hash.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.636874 corgibrowser-0.1.0/corgibrowser/corgi_webscraping/
+-rw-rw-rw-   0        0        0        0 2024-02-15 01:40:53.000000 corgibrowser-0.1.0/corgibrowser/corgi_webscraping/__init__.py
+-rw-rw-rw-   0        0        0    11306 2024-03-25 07:36:11.000000 corgibrowser-0.1.0/corgibrowser/corgi_webscraping/batch_scraper_processor.py
+-rw-rw-rw-   0        0        0    14669 2024-03-23 23:53:36.000000 corgibrowser-0.1.0/corgibrowser/corgi_webscraping/default_scrape_template.py
+-rw-rw-rw-   0        0        0     2857 2024-03-25 07:33:24.000000 corgibrowser-0.1.0/corgibrowser/corgi_webscraping/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.643850 corgibrowser-0.1.0/corgibrowser.egg-info/
+-rw-rw-rw-   0        0        0    10350 2024-04-05 07:55:37.000000 corgibrowser-0.1.0/corgibrowser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4252 2024-04-05 07:55:37.000000 corgibrowser-0.1.0/corgibrowser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 07:55:37.000000 corgibrowser-0.1.0/corgibrowser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2926 2024-04-05 07:55:37.000000 corgibrowser-0.1.0/corgibrowser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-05 07:55:37.000000 corgibrowser-0.1.0/corgibrowser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 07:55:37.646845 corgibrowser-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-04-05 07:55:24.000000 corgibrowser-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.637870 corgibrowser-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.638871 corgibrowser-0.1.0/tests/test_cloud_integration/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/tests/test_cloud_integration/__init__.py
+-rw-rw-rw-   0        0        0     2995 2024-03-25 07:44:34.000000 corgibrowser-0.1.0/tests/test_cloud_integration/test_add_urls_to_queue.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.640860 corgibrowser-0.1.0/tests/test_crawler/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/tests/test_crawler/__init__.py
+-rw-rw-rw-   0        0        0     2445 2024-03-25 04:32:17.000000 corgibrowser-0.1.0/tests/test_crawler/test_crawler.py
+-rw-rw-rw-   0        0        0     1844 2024-03-24 00:48:31.000000 corgibrowser-0.1.0/tests/test_crawler/test_robots_txt.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.641857 corgibrowser-0.1.0/tests/test_scraper/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/tests/test_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1273 2024-03-24 00:42:06.000000 corgibrowser-0.1.0/tests/test_scraper/test_scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:55:37.643850 corgibrowser-0.1.0/tests/test_utils/
+-rw-rw-rw-   0        0        0        0 2024-03-22 20:39:17.000000 corgibrowser-0.1.0/tests/test_utils/__init__.py
+-rw-rw-rw-   0        0        0     2872 2024-03-23 23:26:49.000000 corgibrowser-0.1.0/tests/test_utils/test_names_generator.py
```

### Comparing `corgibrowser-0.0.4/LICENSE` & `corgibrowser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/azure_direct_operations.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/azure_direct_operations.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/cloud_integration.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/cloud_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from azure.identity import DefaultAzureCredential
 from corgibrowser.corgi_cloud_integration.azure_direct_operations import AzureDirectOperations
 from corgibrowser.corgi_cloud_integration.queues_schemas.corgi_web_queue_version_1 import CorgiWebMessageSchemaVersion1
 from corgibrowser.corgi_cloud_integration.tables.corgi_hash_table import CorgiHashTable
+from corgibrowser.corgi_cloud_integration.tables.corgi_web_request_log import CorgiWebRequestLog
+from corgibrowser.corgi_cloud_integration.tables.corgi_web_scrape_log import CorgiWebScrapeLog
+from corgibrowser.corgi_cloud_integration.tables.corgi_web_trottling import CorgiWebThrottling
 from corgibrowser.corgi_cloud_integration.tables.corgiweb_queuepreference import CorgiWebQueuePreference
 import urllib.parse
 import datetime
 from datetime import timedelta
 from corgibrowser.corgi_utils.names_generator import CorgiNameGenerator
 
 
@@ -95,84 +98,55 @@
                     }
                     self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebsitemaps", row = entity )
 
     def save_robots_txt_blobs(self, data, blob_name):
         self.upload_to_blob(data, "corgirobotscache", CorgiNameGenerator.get_storage_compatible_name(blob_name))
 
     def update_visit_rate(self, domain, rate):
-
         if rate:
-            partition_key = "RateLimit"
-            row_key = domain
-
-            entity = {
-                "PartitionKey": partition_key,
-                "RowKey": row_key,
-                "ThrottlingLimitSeconds": int( rate )
-            }
-
-            self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling", row = entity )
+            throttling_entity = CorgiWebThrottling( domain, rate )
+            print( throttling_entity.to_dict() )
+            self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling",
+                                                          row = throttling_entity.to_dict() )
 
     def can_process_domain(self, domain):
-
         entity = self.cloud_direct_operations.get_entity_from_table( table_name = "corgiwebthrottling",
                                                                      partition_key = "RateLimit", row_key = domain )
         if entity:
-            last_access_time = entity._metadata[ 'timestamp' ].replace( tzinfo = None )
-
-            if (datetime.datetime.utcnow() - last_access_time) < timedelta(
-                    seconds = entity[ 'ThrottlingLimitSeconds' ] ):
+            throttling_info = CorgiWebThrottling.from_entity( entity )
+            if (datetime.datetime.utcnow() - throttling_info.LastAccessTime) < timedelta(
+                    seconds = throttling_info.ThrottlingLimitSeconds ):
                 print( f"Not Allowed to visit {domain}" )
                 return False
         else:
-            entity = {
-                "PartitionKey": "RateLimit",
-                "RowKey": domain,
-                "ThrottlingLimitSeconds": 1
-            }
-            self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling", row = entity )
+            # If no entity is found, create a new one with a default throttling limit of 1 second
+            new_throttling_info = CorgiWebThrottling( domain, 1 )
+            self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling",
+                                                          row = new_throttling_info.to_dict() )
 
         return True
 
     def visit_domain(self, domain):
-        entity = {
-            "PartitionKey": "RateLimit",
-            "RowKey": domain,
-            "ThrottlingLimitSeconds": 1
-        }
-
-        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling", row = entity )
-
-    def log_request(self, domain, url, status_code,instance_id):
-        utc_now = datetime.datetime.utcnow()
-        row_key = utc_now.strftime( '%Y%m%dT%H%M%SZ' )
-
-        entity = {
-            "PartitionKey": domain,
-            "RowKey": row_key,
-            "Url": url,
-            "StatusCode": status_code,
-            "InstanceId" : instance_id
-        }
-        print(entity)
-        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebrequestslog", row = entity )
-
-    def log_request_scrape(self, domain, url, status_code,instance_id):
-        utc_now = datetime.datetime.utcnow()
-        row_key = utc_now.strftime( '%Y%m%dT%H%M%SZ' )
-
-        entity = {
-            "PartitionKey": domain,
-            "RowKey": row_key,
-            "Url": url,
-            "StatusCode": status_code,
-            "InstanceId" : instance_id
-        }
-        print(entity)
-        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebscrapelog", row = entity )
+        # Create a new instance of CorgiWebThrottling with a default throttling limit of 1 second
+        throttling_info = CorgiWebThrottling( domain, 1 )
+
+        # Use the to_dict method to convert the instance to a dictionary suitable for the database operation
+        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebthrottling",
+                                                      row = throttling_info.to_dict() )
+
+    def log_request(self, domain, url, status_code, instance_id):
+        web_request_log = CorgiWebRequestLog( domain, url, status_code, instance_id )
+        print( web_request_log.to_dict() )
+        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebrequestslog",
+                                                      row = web_request_log.to_dict() )
+
+    def log_request_scrape(self, domain, url, status_code, instance_id):
+        web_scrape_log = CorgiWebScrapeLog( domain, url, status_code, instance_id )
+        print( web_scrape_log.to_dict() )
+        self.cloud_direct_operations.upsert_to_table( table_name = "corgiwebscrapelog", row = web_scrape_log.to_dict() )
 
     def upload_to_blob(self, data, container_name, blob_name, metadata=None, container_suffix = ""):
         container_name = CorgiNameGenerator.get_container_compatible_name(CorgiNameGenerator.get_storage_compatible_name( container_name ) + container_suffix)
         blob_name = CorgiNameGenerator.generate_blob_name( blob_name )
         print( f"     CloudIntegration: upload_to_blob container_name {container_name}, blob_name:{blob_name}" )
 
         self.cloud_direct_operations.upload_blob_to_container( container_name = container_name, blob_name = blob_name,
```

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/queues_schemas/corgi_web_queue_version_1.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/queues_schemas/corgi_web_queue_version_1.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgi_hash_table.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_hash_table.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgi_web_entity.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgi_web_entity.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgiweb_queuepreference.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgiweb_queuepreference.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_cloud_integration/tables/corgiweb_storage_analytics.py` & `corgibrowser-0.1.0/corgibrowser/corgi_cloud_integration/tables/corgiweb_storage_analytics.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_crawler/RobotsCache.py` & `corgibrowser-0.1.0/corgibrowser/corgi_crawler/RobotsCache.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_crawler/crawler.py` & `corgibrowser-0.1.0/corgibrowser/corgi_crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_crawler/crawler_processor.py` & `corgibrowser-0.1.0/corgibrowser/corgi_crawler/crawler_processor.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_crawler/visited_url_processor.py` & `corgibrowser-0.1.0/corgibrowser/corgi_crawler/visited_url_processor.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_data_analytics_and_ai/data_analytics_and_ai.py` & `corgibrowser-0.1.0/corgibrowser/corgi_data_analytics_and_ai/data_analytics_and_ai.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/DataSetsManager.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/DataSetsManager.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/arizona.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/arizona.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/arkansas.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/arkansas.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/california.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/california.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/colorado.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/colorado.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/connecticut.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/connecticut.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/extra.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/extra.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/georgia.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/georgia.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/hawaii.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/hawaii.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/illinois.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/illinois.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/indiana.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/indiana.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/iowa.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/iowa.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/kansas.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/kansas.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/massachusetts.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/massachusetts.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/mississippi.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/mississippi.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/montana.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/montana.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/nevada.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/nevada.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_mexico.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_mexico.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/new_york.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/new_york.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/oregon.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/oregon.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/pennsylvania.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/pennsylvania.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/rhode_island.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/rhode_island.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/south_dakota.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/south_dakota.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/tennessee.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/tennessee.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/texas.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/texas.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/washington.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/washington.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/west_virginia.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/west_virginia.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_datasets/newspapers/usa/wisconsin.py` & `corgibrowser-0.1.0/corgibrowser/corgi_datasets/newspapers/usa/wisconsin.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_settings/SettingsManager.py` & `corgibrowser-0.1.0/corgibrowser/corgi_settings/SettingsManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,14 @@
             "USE_AZURE_STORAGE_ACCOUNT_KEY": True,
             "ENABLE_LOGS_azure_integration": False
         }
 
     def load_crawler_settings(self,):
 
         self.settings["CRAWLER"] = {
-            "ADD_NEW_URLS_TO_TABLE": True,
-            "ADD_NEW_URLS_TO_QUEUE": True,
             "PROCESS_VISITED_URL": True,
             "CRAWLER_SLEEP_IN_SECONDS": 20,
             "QUEUE_ONLY_DOMAINS": [],
             "CRAWLER_CYCLES_COUNT" : 1000000,
             "ENABLE_CORGIWEB_QUEUE": True,
             "CORGIWEB_QUEUE_ITEMS_TO_POP": 30,
             "CRAWLER_URLS_TO_VISIT": 1000000,
```

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_utils/names_generator.py` & `corgibrowser-0.1.0/corgibrowser/corgi_utils/names_generator.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_utils/url_hash.py` & `corgibrowser-0.1.0/corgibrowser/corgi_utils/url_hash.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_webscraping/batch_scraper_processor.py` & `corgibrowser-0.1.0/corgibrowser/corgi_webscraping/batch_scraper_processor.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_webscraping/default_scrape_template.py` & `corgibrowser-0.1.0/corgibrowser/corgi_webscraping/default_scrape_template.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser/corgi_webscraping/scraper.py` & `corgibrowser-0.1.0/corgibrowser/corgi_webscraping/scraper.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/corgibrowser.egg-info/SOURCES.txt` & `corgibrowser-0.1.0/corgibrowser.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 corgibrowser/corgi_cloud_integration/azure_direct_operations.py
 corgibrowser/corgi_cloud_integration/cloud_integration.py
 corgibrowser/corgi_cloud_integration/queues_schemas/__init__.py
 corgibrowser/corgi_cloud_integration/queues_schemas/corgi_web_queue_version_1.py
 corgibrowser/corgi_cloud_integration/tables/__init__.py
 corgibrowser/corgi_cloud_integration/tables/corgi_hash_table.py
 corgibrowser/corgi_cloud_integration/tables/corgi_web_entity.py
+corgibrowser/corgi_cloud_integration/tables/corgi_web_request_log.py
+corgibrowser/corgi_cloud_integration/tables/corgi_web_scrape_log.py
+corgibrowser/corgi_cloud_integration/tables/corgi_web_trottling.py
 corgibrowser/corgi_cloud_integration/tables/corgiweb_queuepreference.py
 corgibrowser/corgi_cloud_integration/tables/corgiweb_storage_analytics.py
 corgibrowser/corgi_crawler/RobotsCache.py
 corgibrowser/corgi_crawler/__init__.py
 corgibrowser/corgi_crawler/crawler.py
 corgibrowser/corgi_crawler/crawler_processor.py
 corgibrowser/corgi_crawler/visited_url_processor.py
@@ -56,14 +59,17 @@
 corgibrowser/corgi_datasets/newspapers/usa/tennessee.py
 corgibrowser/corgi_datasets/newspapers/usa/texas.py
 corgibrowser/corgi_datasets/newspapers/usa/washington.py
 corgibrowser/corgi_datasets/newspapers/usa/west_virginia.py
 corgibrowser/corgi_datasets/newspapers/usa/wisconsin.py
 corgibrowser/corgi_settings/SettingsManager.py
 corgibrowser/corgi_settings/__init__.py
+corgibrowser/corgi_social_media/Meta.py
+corgibrowser/corgi_social_media/Twitter.py
+corgibrowser/corgi_social_media/__init__.py
 corgibrowser/corgi_utils/AsyncRequests.py
 corgibrowser/corgi_utils/SyncRequests.py
 corgibrowser/corgi_utils/__init__.py
 corgibrowser/corgi_utils/names_generator.py
 corgibrowser/corgi_utils/url_hash.py
 corgibrowser/corgi_webscraping/__init__.py
 corgibrowser/corgi_webscraping/batch_scraper_processor.py
```

### Comparing `corgibrowser-0.0.4/corgibrowser.egg-info/requires.txt` & `corgibrowser-0.1.0/corgibrowser.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/setup.py` & `corgibrowser-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,25 @@
     long_description = fh.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="corgibrowser",
-    version="0.0.4",
+    version="0.1.0",
     author="Jose Enriquez",
     author_email="joseaenriqueza@hotmail.com",
     description="Corgi Browser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/j-enriquez/corgibrowser",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=requirements,
+    project_urls={
+        'Documentation': 'https://corgibrowser.readthedocs.io/en/latest/',
+    }
 )
```

### Comparing `corgibrowser-0.0.4/tests/test_cloud_integration/test_add_urls_to_queue.py` & `corgibrowser-0.1.0/tests/test_cloud_integration/test_add_urls_to_queue.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/tests/test_crawler/test_crawler.py` & `corgibrowser-0.1.0/tests/test_crawler/test_crawler.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/tests/test_crawler/test_robots_txt.py` & `corgibrowser-0.1.0/tests/test_crawler/test_robots_txt.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/tests/test_scraper/test_scraper.py` & `corgibrowser-0.1.0/tests/test_scraper/test_scraper.py`

 * *Files identical despite different names*

### Comparing `corgibrowser-0.0.4/tests/test_utils/test_names_generator.py` & `corgibrowser-0.1.0/tests/test_utils/test_names_generator.py`

 * *Files identical despite different names*

