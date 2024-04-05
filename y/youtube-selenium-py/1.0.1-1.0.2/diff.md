# Comparing `tmp/youtube_selenium_py-1.0.1.tar.gz` & `tmp/youtube_selenium_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_selenium_py-1.0.1.tar", last modified: Fri Apr  5 07:25:32 2024, max compression
+gzip compressed data, was "youtube_selenium_py-1.0.2.tar", last modified: Fri Apr  5 10:32:35 2024, max compression
```

## Comparing `youtube_selenium_py-1.0.1.tar` & `youtube_selenium_py-1.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.645425 youtube_selenium_py-1.0.1/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/LICENSE
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 07:25:32.644425 youtube_selenium_py-1.0.1/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/README.md
--rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 07:25:32.645425 youtube_selenium_py-1.0.1/setup.cfg
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1706 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/setup.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.627423 youtube_selenium_py-1.0.1/youtube_selenium_py/
--rw-r--r--   0 adonis    (1000) adonis    (1000)       40 2024-04-05 07:25:00.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)    25301 2024-04-05 07:25:12.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/classes.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1985 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/test.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.637424 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1453 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1172 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      794 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      880 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      656 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1061 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1146 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      665 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      725 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      579 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      525 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1679 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1757 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      478 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      442 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      594 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      561 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      585 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      638 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      420 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      758 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      755 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.638424 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/
--rw-r--r--   0 adonis    (1000) adonis    (1000)      132 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/generic_utils.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.643425 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1060 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2129 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     5521 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2381 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     6619 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2634 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      903 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     7799 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     3925 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      879 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1062 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1856 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2464 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/sign_into_youtube_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1724 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.644425 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2577 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/SOURCES.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/dependency_links.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)       54 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/requires.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/top_level.txt
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.831250 youtube_selenium_py-1.0.2/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/LICENSE
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 10:32:35.831250 youtube_selenium_py-1.0.2/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/README.md
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 10:32:35.831250 youtube_selenium_py-1.0.2/setup.cfg
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1706 2024-04-05 10:30:40.000000 youtube_selenium_py-1.0.2/setup.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.814250 youtube_selenium_py-1.0.2/youtube_selenium_py/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 09:50:23.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)    25351 2024-04-05 10:12:16.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/classes.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1985 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/test.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.825250 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1893 2024-04-05 10:05:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1192 2024-04-05 10:05:48.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      814 2024-04-05 10:05:57.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      900 2024-04-05 10:06:04.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      676 2024-04-05 10:12:23.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1081 2024-04-05 10:06:26.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1166 2024-04-05 10:06:41.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_video_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      685 2024-04-05 10:06:48.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      745 2024-04-05 10:06:57.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_delete_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      599 2024-04-05 10:07:06.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      545 2024-04-05 10:07:16.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1699 2024-04-05 10:07:24.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1777 2024-04-05 10:07:31.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_edit_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      498 2024-04-05 10:07:40.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      462 2024-04-05 10:07:50.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      614 2024-04-05 10:08:20.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      601 2024-04-05 10:08:26.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 10:08:31.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      605 2024-04-05 10:08:39.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      658 2024-04-05 10:08:50.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      440 2024-04-05 10:09:05.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      778 2024-04-05 10:09:13.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      775 2024-04-05 10:09:19.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.825250 youtube_selenium_py-1.0.2/youtube_selenium_py/utils/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      152 2024-04-05 10:09:28.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/utils/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/utils/generic_utils.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.830250 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1400 2024-04-05 09:53:56.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2149 2024-04-05 10:09:55.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     5541 2024-04-05 10:10:05.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2401 2024-04-05 10:10:12.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     6639 2024-04-05 10:10:18.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2654 2024-04-05 10:10:27.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      923 2024-04-05 10:10:34.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     7819 2024-04-05 10:10:50.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     3945 2024-04-05 10:10:57.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      899 2024-04-05 10:11:25.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1102 2024-04-05 10:11:36.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1876 2024-04-05 10:11:47.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2484 2024-04-05 10:11:55.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/sign_into_youtube_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1744 2024-04-05 10:12:03.000000 youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:32:35.830250 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 10:32:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2577 2024-04-05 10:32:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/SOURCES.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 10:32:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/dependency_links.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       54 2024-04-05 10:32:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/requires.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 10:32:35.000000 youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/top_level.txt
```

### Comparing `youtube_selenium_py-1.0.1/LICENSE` & `youtube_selenium_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/PKG-INFO` & `youtube_selenium_py-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
 Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
```

### Comparing `youtube_selenium_py-1.0.1/setup.py` & `youtube_selenium_py-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'youtube_selenium_py'
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = "A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more."
 URL = 'https://github.com/Automa-Automations/youtube_selenium_py'
 AUTHOR = 'William Ferns'
 AUTHOR_EMAIL = 'business@agnostica.site'
 LICENSE = 'MIT'
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/classes.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, List
-import youtube 
-from utils import new_driver
+import youtube_selenium_py.youtube as youtube
+from youtube_selenium_py.utils import new_driver
 from dataclasses import dataclass
 
 @dataclass
 class Youtube:
     email: Optional[str] = None
     password: Optional[str] = None
     absolute_chromium_profile_path: Optional[str] = None
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/test.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/test.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import time
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_community_post.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube 
+from youtube_selenium_py.classes import Youtube 
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_community_post_sub_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube 
+from youtube_selenium_py.classes import Youtube 
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_sub_channels.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_sub_channels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_video.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_create_video_sub_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_delete_channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 test_email = os.getenv("TEST_EMAIL") or ""
 test_password = os.getenv("TEST_PASSWORD") or ""
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_delete_sub_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL") or ""
 test_password = os.getenv("TEST_PASSWORD") or ""
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_thumbnail.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_download_thumbnail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import YoutubeData
+from youtube_selenium_py.classes import YoutubeData
 import os
 
 class TestDownloadThumbnail(unittest.TestCase):
 
     def test_download_thumbnail_success(self):
         youtube_data = YoutubeData()
         path = "./tests/assets"
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_video.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_download_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import YoutubeData
+from youtube_selenium_py.classes import YoutubeData
 import os
 
 class TestDownloadVideo(unittest.TestCase):
 
     def test_download_video_success(self):
         youtube_data = YoutubeData()
         path = "./tests/assets"
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_edit_channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import time
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_edit_sub_channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import time
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_channel_stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import YoutubeData
+from youtube_selenium_py.classes import YoutubeData
 
 class TestGetChannelStats(unittest.TestCase):
     def test_get_channel_stats_success(self):
         youtube_data = YoutubeData()
         print("in get_channel_stats_success")
         channel_id_result = youtube_data.get_channel_id("@Hamza97")
         if channel_id_result['status'] == 'success':
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_handle.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_handle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_id.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
 
-class TestGetMyChannelID(unittest.TestCase):
+class TestGetMyChannelStats(unittest.TestCase):
 
-    def test_get_my_channel_id(self):
+    def test_get_my_channel_stats(self):
         youtube = Youtube(email=test_email, password=test_password)
-        result = youtube.get_my_channel_id()
+        result = youtube.get_my_channel_stats()
         if result:
             self.assertEqual(result["status"], "success")
         else:
-            raise Exception("Getting channel ID, result is None")
+            raise Exception("Problem getting my channel stats, result is None")
 
         youtube.close()
+
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_channel_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
 
-class TestGetMyChannelStats(unittest.TestCase):
+class TestGetMyChannelID(unittest.TestCase):
 
-    def test_get_my_channel_stats(self):
+    def test_get_my_channel_id(self):
         youtube = Youtube(email=test_email, password=test_password)
-        result = youtube.get_my_channel_stats()
+        result = youtube.get_my_channel_id()
         if result:
             self.assertEqual(result["status"], "success")
         else:
-            raise Exception("Problem getting my channel stats, result is None")
+            raise Exception("Getting channel ID, result is None")
 
         youtube.close()
-
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_videos_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_get_my_videos_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 from dotenv import load_dotenv
 import os
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_list_all_channels.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_list_all_channels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import time
 from dotenv import load_dotenv
 
 load_dotenv()
 
 test_email = os.getenv("TEST_EMAIL")
 test_password = os.getenv("TEST_PASSWORD")
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_switch_to_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/tests/test_switch_to_sub_channel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from classes import Youtube
+from youtube_selenium_py.classes import Youtube
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 test_email = os.getenv("TEST_EMAIL") or ""
 test_password = os.getenv("TEST_PASSWORD") or ""
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/utils/generic_utils.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/all_video_stats_from_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.common.by import By
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 import time
 
 def create_channel(
     driver,
 ):
 
     try:
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_community_post.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_community_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 from typing import Optional
 import time
 
 def create_community_post(
     driver,
     community_post_title: str,
     schedule: Optional[dict] = None,
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_sub_channels.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_sub_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 import time
 from selenium.webdriver.common.by import By
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 
 def create_sub_channels(
     driver,
     sub_channels_names: List[str],
 ):
     try:
         time.sleep(5)
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_video.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/create_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 import time
 
 def create_video(
     driver,
     absolute_video_path: str,
     video_title: str,
     video_description: str,
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/delete_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/delete_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.common.by import By
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 import time
 
 def delete_channel(
     driver,
     email: str,
 ):
     try:
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_thumbnail.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/download_thumbnail.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from youtube import get_video_stats
+from youtube_selenium_py.youtube import get_video_stats
 
 def download_thumbnail(video_id, export_path, thumbnail_name):
     try:
         result = get_video_stats(video_id)
         if result["status"] == "success":
             video_data = result["video_stats"]
         else:
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_video.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/download_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/edit_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/edit_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.by import By
-from utils import find_element, scroll_to_bottom, set_element_innertext, gen_random_string
+from youtube_selenium_py.utils import find_element, scroll_to_bottom, set_element_innertext, gen_random_string
 import time
 
 def edit_channel(
     driver,
     channel_name: str,
     channel_handle: str,
     channel_description: str,
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import math
 import threading
-from youtube.get_channel_id import get_channel_id
+from youtube_selenium_py.youtube.get_channel_id import get_channel_id
 
 def all_videos_from_channel(channel_id):
 
     print("Fetching all videos from channel...")
     get_channel_info = f"https://yt.lemnoslife.com/noKey/channels?id={channel_id}&part=contentDetails" 
     response = requests.get(get_channel_info)
     uploads_id = response.json()['items'][0]['contentDetails']['relatedPlaylists']['uploads']
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_id.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_channel_id.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_channel_handle.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_my_channel_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from youtube.list_all_channels import list_all_channels
+from youtube_selenium_py.youtube.list_all_channels import list_all_channels
 
 def get_my_channel_handle(driver):
     try:
         result = list_all_channels(driver)
         if result["status"] == "success":
             channel_handle = result["channels_list"][0]['channel_handle']
         else:
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_videos_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_my_videos_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from youtube.get_all_video_stats_from_channel import get_all_video_stats_from_channel
-from youtube.get_my_channel_handle import get_my_channel_handle
+from youtube_selenium_py.youtube.get_all_video_stats_from_channel import get_all_video_stats_from_channel
+from youtube_selenium_py.youtube.get_my_channel_handle import get_my_channel_handle
 
 def get_my_videos_stats(driver):
     try:
         result = get_my_channel_handle(driver)
         if result['status'] == "success":
             channel_handle = result['channel_handle']
             driver = result['driver']
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_video_stats.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/get_video_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/list_all_channels.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/list_all_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver.common.by import By
-from utils import find_element, find_elements 
+from youtube_selenium_py.utils import find_element, find_elements 
 import time
 
 def list_all_channels(
     driver
 ):
     try:
         time.sleep(3)
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/sign_into_youtube_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/sign_into_youtube_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 import undetected_chromedriver as uc
-from utils import find_element
+from youtube_selenium_py.utils import find_element
 import time
 from selenium.webdriver.common.by import By
 
 def sign_into_youtube_channel(
     driver,
     email: Optional[str] = None,
     password: Optional[str] = None,
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/switch_to_sub_channel.py` & `youtube_selenium_py-1.0.2/youtube_selenium_py/youtube/switch_to_sub_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from selenium.webdriver.common.by import By
-from utils import find_element, find_elements
+from youtube_selenium_py.utils import find_element, find_elements
 
 def switch_to_sub_channel(
     driver,
     channel_name: str,
 ):
     try:
         time.sleep(5)
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/PKG-INFO` & `youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
 Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
```

### Comparing `youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/SOURCES.txt` & `youtube_selenium_py-1.0.2/youtube_selenium_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

