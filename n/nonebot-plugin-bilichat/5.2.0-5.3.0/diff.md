# Comparing `tmp/nonebot_plugin_bilichat-5.2.0.tar.gz` & `tmp/nonebot_plugin_bilichat-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.2.0.tar", last modified: Thu Feb 22 07:51:06 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.3.0.tar", last modified: Fri Apr  5 09:09:49 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.2.0.tar` & `nonebot_plugin_bilichat-5.3.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0    34523 2024-02-22 07:50:59.642093 nonebot_plugin_bilichat-5.2.0/LICENSE
--rw-r--r--   0        0        0    17818 2024-02-22 07:50:59.642093 nonebot_plugin_bilichat-5.2.0/README.md
--rw-r--r--   0        0        0     2758 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0      575 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/__init__.py
--rw-r--r--   0        0        0     4455 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/base_content_parsing.py
--rw-r--r--   0        0        0     5843 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/mirai2.py
--rw-r--r--   0        0        0     5080 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/onebot_v11.py
--rw-r--r--   0        0        0     5148 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/onebot_v12.py
--rw-r--r--   0        0        0     4258 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/qq.py
--rw-r--r--   0        0        0     1120 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1647 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0       60 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1288 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0      996 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      892 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3845 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9295 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3197 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3975 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2653 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      444 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      870 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3189 2024-02-22 07:50:59.662093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5103 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     2950 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3803 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      546 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3263 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      824 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      341 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      806 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      277 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     2685 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7232 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4022 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    14446 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      650 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4935 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2467 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1691 2024-02-22 07:50:59.666093 nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1704 2024-02-22 07:51:06.318089 nonebot_plugin_bilichat-5.2.0/pyproject.toml
--rw-r--r--   0        0        0    19472 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-05 09:09:45.742194 nonebot_plugin_bilichat-5.3.0/LICENSE
+-rw-r--r--   0        0        0    17818 2024-04-05 09:09:45.742194 nonebot_plugin_bilichat-5.3.0/README.md
+-rw-r--r--   0        0        0     2770 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2232 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1647 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2686 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0      575 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/__init__.py
+-rw-r--r--   0        0        0     4461 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/base_content_parsing.py
+-rw-r--r--   0        0        0     5849 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/mirai2.py
+-rw-r--r--   0        0        0     5086 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     5154 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     4265 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/qq.py
+-rw-r--r--   0        0        0     7880 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1288 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0      996 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      892 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3845 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5230 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9295 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3197 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4233 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3975 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      518 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6192 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2653 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      444 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      870 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 09:09:45.762194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1160 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7333 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     2950 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3794 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      546 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3115 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3263 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1732 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1788 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     4033 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      568 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      824 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      341 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3019 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1040 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      806 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      277 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     2685 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7223 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4022 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    14446 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      650 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4935 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2467 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1691 2024-04-05 09:09:45.766194 nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1742 2024-04-05 09:09:49.078194 nonebot_plugin_bilichat-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0    19518 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.2.0/LICENSE` & `nonebot_plugin_bilichat-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/README.md` & `nonebot_plugin_bilichat-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,8 +66,8 @@
                 "brief_des": "无",
                 "detail_des": "无",
             },
         ],
     },
 )
 
-from . import adapters, api, commands  # noqa: F401, E402
+from . import api, base_content_parsing, commands  # noqa: F401, E402
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/base_content_parsing.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/base_content_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import time
 from typing import Any, Dict, Union
 
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.typing import T_State
 
-from ..config import plugin_config
-from ..content import Column, Dynamic, Video
-from ..lib.text_to_image import t2i
-from ..model.exception import AbortError
+from ...config import plugin_config
+from ...content import Column, Dynamic, Video
+from ...lib.text_to_image import t2i
+from ...model.exception import AbortError
 
 if plugin_config.bilichat_openai_token:
     ENABLE_SUMMARY = True
-    from ..summary import summarization
+    from ...summary import summarization
 else:
     ENABLE_SUMMARY = False
 
 if plugin_config.bilichat_word_cloud:
-    from ..wordcloud.wordcloud import wordcloud
+    from ...wordcloud.wordcloud import wordcloud
 
 FUTUER_FUCTIONS = ENABLE_SUMMARY or plugin_config.bilichat_word_cloud or plugin_config.bilichat_official_summary
 
 
 cd: Dict[str, int] = {}
 cd_size_limit = plugin_config.bilichat_cd_time // 2
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/mirai2.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/mirai2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from nonebot.adapters.mirai2.event import FriendMessage, FriendSyncMessage, GroupMessage, GroupSyncMessage, MessageEvent
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
-from ..config import plugin_config
-from ..content import Column, Dynamic, Video
-from ..lib.b23_extract import b23_extract
-from ..model.arguments import Options, parser
-from ..model.exception import AbortError
-from ..optional import capture_exception
+from ...config import plugin_config
+from ...content import Column, Dynamic, Video
+from ...lib.b23_extract import b23_extract
+from ...model.arguments import Options, parser
+from ...model.exception import AbortError
+from ...optional import capture_exception
 from .base_content_parsing import get_content_info_from_state, get_futuer_fuctions
 
 
 async def _bili_check(bot: Bot, event: MessageEvent, state: T_State):
     # 检查并提取 raw_bililink
     if plugin_config.bilichat_enable_self and str(event.get_user_id()) == str(bot.self_id) and event.quote:
         # 是自身消息的情况下，检查是否是回复，是的话则取被回复的消息
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/onebot_v11.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/onebot_v11.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 )
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
-from ..config import plugin_config
-from ..content import Column, Dynamic, Video
-from ..lib.b23_extract import b23_extract
-from ..model.arguments import Options, parser
-from ..model.exception import AbortError
-from ..optional import capture_exception
+from ...config import plugin_config
+from ...content import Column, Dynamic, Video
+from ...lib.b23_extract import b23_extract
+from ...model.arguments import Options, parser
+from ...model.exception import AbortError
+from ...optional import capture_exception
 from .base_content_parsing import get_content_info_from_state, get_futuer_fuctions
 
 
 async def _bili_check(bot: Bot, event: MessageEvent, state: T_State):
     # 检查并提取 raw_bililink
     try:
         if plugin_config.bilichat_enable_self and str(event.get_user_id()) == str(bot.self_id) and event.reply:
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/onebot_v12.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/onebot_v12.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 )
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
-from ..config import plugin_config
-from ..content import Column, Dynamic, Video
-from ..lib.b23_extract import b23_extract
-from ..model.arguments import Options, parser
-from ..model.exception import AbortError
-from ..optional import capture_exception
+from ...config import plugin_config
+from ...content import Column, Dynamic, Video
+from ...lib.b23_extract import b23_extract
+from ...model.arguments import Options, parser
+from ...model.exception import AbortError
+from ...optional import capture_exception
 from .base_content_parsing import get_content_info_from_state, get_futuer_fuctions
 
 
 async def _bili_check(event: MessageEvent, state: T_State):
     _msgs = event.get_message()
 
     for _msg in _msgs:
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/adapters/qq.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/archive/adapters/qq.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 )
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
-from ..config import plugin_config
-from ..content import Column, Dynamic, Video
-from ..lib.b23_extract import b23_extract
-from ..lib.tools import obfuscate_urls_in_text
-from ..model.arguments import Options, parser
-from ..model.exception import AbortError
-from ..optional import capture_exception
+from ...config import plugin_config
+from ...content import Column, Dynamic, Video
+from ...lib.b23_extract import b23_extract
+from ...lib.tools import obfuscate_urls_in_text
+from ...model.arguments import Options, parser
+from ...model.exception import AbortError
+from ...optional import capture_exception
 from .base_content_parsing import get_content_info_from_state, get_futuer_fuctions
 
 
 async def _bili_check(event: GuildMessageEvent, state: T_State):
     _msgs = event.get_message()
 
     for _msg in _msgs:
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     DynamicType,
 )
 from google.protobuf.json_format import MessageToDict
 from grpc.aio import AioRpcError
 from httpx import TimeoutException
 from nonebot.log import logger
 
-from ..adapters.base_content_parsing import check_cd
+from ..base_content_parsing import check_cd
 from ..content.dynamic import Dynamic
 from ..lib.bilibili_request import get_b23_url, get_user_dynamics
 from ..lib.bilibili_request.auth import AuthManager
 from ..lib.uid_extract import SearchUp
 from ..model.exception import AbortError
 from ..optional import capture_exception
 from ..subscribe.manager import SubscriptionSystem
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     DynModuleType,
 )
 from google.protobuf.json_format import MessageToDict
 from grpc.aio import AioRpcError
 from httpx import TimeoutException
 from nonebot.log import logger
 
-from ..adapters.base_content_parsing import check_cd
+from ..base_content_parsing import check_cd
 from ..config import plugin_config
 from ..content.dynamic import Dynamic
 from ..lib.bilibili_request import get_b23_url, get_user_dynamics
 from ..lib.bilibili_request.auth import AuthManager
 from ..lib.fetch_dynamic import DYNAMIC_TYPE_IGNORE, DYNAMIC_TYPE_MAP
 from ..model.exception import AbortError
 from ..optional import capture_exception
```

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-5.3.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.2.0/pyproject.toml` & `nonebot_plugin_bilichat-5.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.2.0"
+version = "5.3.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
@@ -15,14 +15,15 @@
     "nonebot2[fastapi,websockets]>=2.0.0",
     "httpx>=0.24.1",
     "dynrender-skia-opt>=0.3.8",
     "nonebot-plugin-apscheduler>=0.3.0",
     "nonebot-plugin-send-anything-anywhere>=0.4.0",
     "packaging>=23.2",
     "python-multipart>=0.0.6",
+    "nonebot-plugin-alconna>=0.41.1",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
```

### Comparing `nonebot_plugin_bilichat-5.2.0/PKG-INFO` & `nonebot_plugin_bilichat-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.2.0
+Version: 5.3.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -13,14 +13,15 @@
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: python-multipart>=0.0.6
+Requires-Dist: nonebot-plugin-alconna>=0.41.1
 Requires-Dist: numpy<1.25.0,>=1.20.1; extra == "extra"
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra"
 Requires-Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken>=0.6.0; extra == "summary"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.3.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8 Requires-Dist: nonebot-plugin-
 apscheduler>=0.3.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
 Requires-Dist: packaging>=23.2 Requires-Dist: python-multipart>=0.0.6 Requires-
-Dist: numpy<1.25.0,>=1.20.1; extra == "extra" Requires-Dist: nonebot-plugin-
-sentry>=0.2.2; extra == "extra" Requires-Dist: nonebot-plugin-
-htmlrender>=0.2.0.3; extra == "extra" Requires-Dist: nonebot-plugin-
-mongodb>=0.1.0; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
-"wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
-Dist: tiktoken>=0.6.0; extra == "summary" Requires-Dist: numpy<1.25.0,>=1.20.1;
-extra == "all" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
-wordcloud>=1.8.2.2; extra == "all" Requires-Dist: nonebot-plugin-
-htmlrender>=0.2.0.3; extra == "all" Requires-Dist: nonebot-plugin-
+Dist: nonebot-plugin-alconna>=0.41.1 Requires-Dist: numpy<1.25.0,>=1.20.1;
+extra == "extra" Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra" Requires-
+Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra" Requires-Dist:
+jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
+"wordcloud" Requires-Dist: tiktoken>=0.6.0; extra == "summary" Requires-Dist:
+numpy<1.25.0,>=1.20.1; extra == "all" Requires-Dist: jieba>=0.42.1; extra ==
+"all" Requires-Dist: wordcloud>=1.8.2.2; extra == "all" Requires-Dist: nonebot-
+plugin-htmlrender>=0.2.0.3; extra == "all" Requires-Dist: nonebot-plugin-
 mongodb>=0.1.0; extra == "all" Requires-Dist: nonebot-plugin-sentry>=0.4.1;
 extra == "all" Requires-Dist: tiktoken>=0.6.0; extra == "all" Provides-Extra:
 extra Provides-Extra: wordcloud Provides-Extra: summary Provides-Extra: all
 Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # nonebot-plugin-bilichat _â¨ å¤åè½ç B ç«è§é¢è§£æå·¥å· â¨_
```

