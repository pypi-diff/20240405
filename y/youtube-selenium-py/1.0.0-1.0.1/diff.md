# Comparing `tmp/youtube_selenium_py-1.0.0.tar.gz` & `tmp/youtube_selenium_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_selenium_py-1.0.0.tar", last modified: Fri Apr  5 07:03:07 2024, max compression
+gzip compressed data, was "youtube_selenium_py-1.0.1.tar", last modified: Fri Apr  5 07:25:32 2024, max compression
```

## Comparing `youtube_selenium_py-1.0.0.tar` & `youtube_selenium_py-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.499516 youtube_selenium_py-1.0.0/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/LICENSE
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1497 2024-04-05 07:03:07.498516 youtube_selenium_py-1.0.0/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/README.md
--rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 07:03:07.499516 youtube_selenium_py-1.0.0/setup.cfg
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1708 2024-04-05 06:52:38.000000 youtube_selenium_py-1.0.0/setup.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.480516 youtube_selenium_py-1.0.0/youtube_selenium_py/
--rw-r--r--   0 adonis    (1000) adonis    (1000)       44 2024-04-05 06:19:36.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)    25329 2024-04-05 06:38:36.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/classes.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.489516 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1453 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1172 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      794 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      880 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      656 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1061 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1146 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_video_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      665 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      725 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_delete_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      579 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      525 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1679 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1757 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_edit_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      478 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      442 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      594 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      561 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      585 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      638 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      420 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      758 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      755 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.491516 youtube_selenium_py-1.0.0/youtube_selenium_py/utils/
--rw-r--r--   0 adonis    (1000) adonis    (1000)      132 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/utils/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/utils/generic_utils.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.497516 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1060 2024-04-05 06:17:35.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2129 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     5521 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2381 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     6619 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2634 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      903 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     7799 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     3925 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      879 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1062 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1856 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2464 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/sign_into_youtube_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1724 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:03:07.498516 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1497 2024-04-05 07:03:07.000000 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2549 2024-04-05 07:03:07.000000 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/SOURCES.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 07:03:07.000000 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/dependency_links.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)       54 2024-04-05 07:03:07.000000 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/requires.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 07:03:07.000000 youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/top_level.txt
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.645425 youtube_selenium_py-1.0.1/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/LICENSE
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 07:25:32.644425 youtube_selenium_py-1.0.1/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/README.md
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 07:25:32.645425 youtube_selenium_py-1.0.1/setup.cfg
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1706 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/setup.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.627423 youtube_selenium_py-1.0.1/youtube_selenium_py/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       40 2024-04-05 07:25:00.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)    25301 2024-04-05 07:25:12.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/classes.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1985 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/test.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.637424 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1453 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1172 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      794 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      880 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      656 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1061 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1146 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      665 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      725 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      579 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      525 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1679 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1757 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      478 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      442 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      594 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      561 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      585 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      638 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      420 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      758 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      755 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.638424 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      132 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/utils/generic_utils.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.643425 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1060 2024-04-05 07:24:19.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2129 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     5521 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2381 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     6619 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2634 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      903 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     7799 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     3925 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      879 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1062 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1856 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2464 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/sign_into_youtube_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1724 2024-04-05 05:58:53.000000 youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 07:25:32.644425 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1495 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2577 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/SOURCES.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/dependency_links.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       54 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/requires.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 07:25:32.000000 youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/top_level.txt
```

### Comparing `youtube_selenium_py-1.0.0/LICENSE` & `youtube_selenium_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/PKG-INFO` & `youtube_selenium_py-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
-Author-email: business@williamferns.com
+Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
 Project-URL: Automa Automations, https://github.com/Automa-Automations
 Keywords: youtube,API,video,channel,upload,statistics,python,development,selenium
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `youtube_selenium_py-1.0.0/setup.py` & `youtube_selenium_py-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'youtube_selenium_py'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = "A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more."
 URL = 'https://github.com/Automa-Automations/youtube_selenium_py'
 AUTHOR = 'William Ferns'
-AUTHOR_EMAIL = 'business@williamferns.com'
+AUTHOR_EMAIL = 'business@agnostica.site'
 LICENSE = 'MIT'
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
```

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/classes.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, List
-import youtube_selenium_py.youtube as youtube
+import youtube 
 from utils import new_driver
 from dataclasses import dataclass
 
 @dataclass
 class Youtube:
     email: Optional[str] = None
     password: Optional[str] = None
@@ -732,12 +732,12 @@
         }
         - example error return object: {
             "status": "error",
             "message": "Error downloading thumbnail.",
             "error": str(e),
         }
         """
-        # Download thumbnail and save to absolute path
+        # # Download thumbnail and save to absolute path
         result = youtube.download_thumbnail(video_id, export_path, thumbnail_name)
         return result
```

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/__init__.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_community_post.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_community_post_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_community_post_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_sub_channels.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_sub_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_video.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_create_video_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_create_video_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_delete_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_delete_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_delete_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_download_thumbnail.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_download_video.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_download_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_edit_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_edit_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_edit_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_channel_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_handle.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_handle.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_id.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_id.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_channel_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_get_my_videos_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_get_my_videos_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_list_all_channels.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_list_all_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/tests/test_switch_to_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/tests/test_switch_to_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/utils/generic_utils.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/__init__.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/all_video_stats_from_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_community_post.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_community_post.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_sub_channels.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_sub_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/create_video.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/create_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/delete_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/delete_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/download_thumbnail.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/download_video.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/download_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/edit_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/edit_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_channel_id.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_id.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_channel_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_my_channel_handle.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_channel_handle.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_my_videos_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_my_videos_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/get_video_stats.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/get_video_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/list_all_channels.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/list_all_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/sign_into_youtube_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/sign_into_youtube_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py/youtube/switch_to_sub_channel.py` & `youtube_selenium_py-1.0.1/youtube_selenium_py/youtube/switch_to_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/PKG-INFO` & `youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
-Author-email: business@williamferns.com
+Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
 Project-URL: Automa Automations, https://github.com/Automa-Automations
 Keywords: youtube,API,video,channel,upload,statistics,python,development,selenium
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `youtube_selenium_py-1.0.0/youtube_selenium_py.egg-info/SOURCES.txt` & `youtube_selenium_py-1.0.1/youtube_selenium_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 youtube_selenium_py/__init__.py
 youtube_selenium_py/classes.py
+youtube_selenium_py/test.py
 youtube_selenium_py.egg-info/PKG-INFO
 youtube_selenium_py.egg-info/SOURCES.txt
 youtube_selenium_py.egg-info/dependency_links.txt
 youtube_selenium_py.egg-info/requires.txt
 youtube_selenium_py.egg-info/top_level.txt
 youtube_selenium_py/tests/__init__.py
 youtube_selenium_py/tests/test_create_channel.py
```

