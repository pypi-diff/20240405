# Comparing `tmp/youtube_selenium_py-1.0.4.tar.gz` & `tmp/youtube_selenium_py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_selenium_py-1.0.4.tar", last modified: Fri Apr  5 10:51:25 2024, max compression
+gzip compressed data, was "youtube_selenium_py-1.0.5.tar", last modified: Fri Apr  5 11:09:53 2024, max compression
```

## Comparing `youtube_selenium_py-1.0.4.tar` & `youtube_selenium_py-1.0.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.399563 youtube_selenium_py-1.0.4/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/LICENSE
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2842 2024-04-05 10:51:25.397564 youtube_selenium_py-1.0.4/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/README.md
--rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 10:51:25.399563 youtube_selenium_py-1.0.4/setup.cfg
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1706 2024-04-05 10:51:19.000000 youtube_selenium_py-1.0.4/setup.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.381563 youtube_selenium_py-1.0.4/youtube_selenium_py/
--rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)    25351 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/classes.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1985 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/test.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.388563 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1893 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1192 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      814 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      900 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      676 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1081 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1166 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_video_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      685 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      745 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_delete_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      599 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      545 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1699 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1777 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_edit_sub_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      498 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      462 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      614 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      601 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      605 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      658 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      440 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      778 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      775 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.389563 youtube_selenium_py-1.0.4/youtube_selenium_py/utils/
--rw-r--r--   0 adonis    (1000) adonis    (1000)      152 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/utils/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/utils/generic_utils.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.394563 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1400 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/__init__.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2149 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     5541 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_community_post.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2401 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_sub_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     6639 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2654 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/delete_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      923 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/download_thumbnail.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/download_video.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     7819 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/edit_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     3945 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_channel_id.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_channel_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      899 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_my_channel_handle.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1102 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_my_videos_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_video_stats.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1876 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/list_all_channels.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2484 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/sign_into_youtube_channel.py
--rw-r--r--   0 adonis    (1000) adonis    (1000)     1744 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/switch_to_sub_channel.py
-drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 10:51:25.395563 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2842 2024-04-05 10:51:25.000000 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/PKG-INFO
--rw-r--r--   0 adonis    (1000) adonis    (1000)     2577 2024-04-05 10:51:25.000000 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/SOURCES.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 10:51:25.000000 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/dependency_links.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)      801 2024-04-05 10:51:25.000000 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/requires.txt
--rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 10:51:25.000000 youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/top_level.txt
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.228659 youtube_selenium_py-1.0.5/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1077 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/LICENSE
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2842 2024-04-05 11:09:53.228659 youtube_selenium_py-1.0.5/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      248 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/README.md
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       38 2024-04-05 11:09:53.229659 youtube_selenium_py-1.0.5/setup.cfg
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1706 2024-04-05 11:09:41.000000 youtube_selenium_py-1.0.5/setup.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.208658 youtube_selenium_py-1.0.5/youtube_selenium_py/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)    25351 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/classes.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1985 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/test.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.218659 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1893 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1192 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      814 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      900 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_community_post_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      676 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1081 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1166 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_video_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      685 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      745 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_delete_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      599 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      545 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1699 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1777 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_edit_sub_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      498 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      462 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      614 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      601 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      581 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      605 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      658 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      440 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      778 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      775 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.219659 youtube_selenium_py-1.0.5/youtube_selenium_py/utils/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      152 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/utils/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1295 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/utils/generic_utils.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.226659 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1400 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/__init__.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     4002 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2149 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     5541 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_community_post.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2401 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_sub_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     6639 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2654 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/delete_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      923 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/download_thumbnail.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1544 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/download_video.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     7819 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/edit_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     3945 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      936 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_channel_id.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      792 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_channel_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      899 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_my_channel_handle.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1102 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_my_videos_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      751 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_video_stats.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1876 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/list_all_channels.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2648 2024-04-05 11:08:49.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/sign_into_youtube_channel.py
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     1744 2024-04-05 10:37:19.000000 youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/switch_to_sub_channel.py
+drwxr-xr-x   0 adonis    (1000) adonis    (1000)        0 2024-04-05 11:09:53.227659 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2842 2024-04-05 11:09:53.000000 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/PKG-INFO
+-rw-r--r--   0 adonis    (1000) adonis    (1000)     2577 2024-04-05 11:09:53.000000 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/SOURCES.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)        1 2024-04-05 11:09:53.000000 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/dependency_links.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)      801 2024-04-05 11:09:53.000000 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/requires.txt
+-rw-r--r--   0 adonis    (1000) adonis    (1000)       20 2024-04-05 11:09:53.000000 youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/top_level.txt
```

### Comparing `youtube_selenium_py-1.0.4/LICENSE` & `youtube_selenium_py-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/PKG-INFO` & `youtube_selenium_py-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
 Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
```

### Comparing `youtube_selenium_py-1.0.4/setup.py` & `youtube_selenium_py-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'youtube_selenium_py'
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = "A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more."
 URL = 'https://github.com/Automa-Automations/youtube_selenium_py'
 AUTHOR = 'William Ferns'
 AUTHOR_EMAIL = 'business@agnostica.site'
 LICENSE = 'MIT'
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
```

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/classes.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/classes.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/test.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/test.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/__init__.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_community_post.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_community_post.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_community_post_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_community_post_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_sub_channels.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_sub_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_video.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_create_video_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_create_video_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_delete_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_delete_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_delete_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_delete_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_download_thumbnail.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_download_thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_download_video.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_download_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_edit_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_edit_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_edit_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_edit_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_channel_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_handle.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_handle.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_id.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_id.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_channel_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_get_my_videos_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_get_my_videos_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_list_all_channels.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_list_all_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/tests/test_switch_to_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/tests/test_switch_to_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/utils/generic_utils.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/__init__.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/all_video_stats_from_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_community_post.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_community_post.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_sub_channels.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_sub_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/create_video.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/create_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/delete_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/delete_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/download_thumbnail.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/download_thumbnail.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/download_video.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/download_video.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/edit_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/edit_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_all_video_stats_from_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_channel_id.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_channel_id.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_channel_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_channel_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_my_channel_handle.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_my_channel_handle.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_my_videos_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_my_videos_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/get_video_stats.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/get_video_stats.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/list_all_channels.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/list_all_channels.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/sign_into_youtube_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/sign_into_youtube_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 
             see_password_checkbox = find_element(driver, By.CSS_SELECTOR, "input[type='checkbox']")
             see_password_checkbox.click()
 
             next_button = find_element(driver, By.XPATH, "//button[contains(span/text(), 'Next')]")
             next_button.click()
 
+            print("Implicitly sleeping for 20 seconds, if your account has two setp authentication, or asking for verification code...")
+            time.sleep(20)
             return driver
         else:
             raise Exception("You must provide either an email and password, chromium driver path, or cookies.")
 
     except Exception as e:
         print("Error signing into youtube channel: ", e)
```

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py/youtube/switch_to_sub_channel.py` & `youtube_selenium_py-1.0.5/youtube_selenium_py/youtube/switch_to_sub_channel.py`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/PKG-INFO` & `youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube_selenium_py
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python package to create youtube channels, sub channels, upload videos, create community posts, edit channel, delete channel, and so much more.
 Home-page: https://github.com/Automa-Automations/youtube_selenium_py
 Author: William Ferns
 Author-email: business@agnostica.site
 License: MIT
 Project-URL: Bug Reports, https://github.com/Automa-Automations/youtube_selenium_py/issues
 Project-URL: Source, https://github.com/Automa-Automations/youtube_selenium_py
```

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/SOURCES.txt` & `youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `youtube_selenium_py-1.0.4/youtube_selenium_py.egg-info/requires.txt` & `youtube_selenium_py-1.0.5/youtube_selenium_py.egg-info/requires.txt`

 * *Files identical despite different names*

