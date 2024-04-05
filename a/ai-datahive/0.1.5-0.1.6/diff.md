# Comparing `tmp/ai-datahive-0.1.5.tar.gz` & `tmp/ai-datahive-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-datahive-0.1.5.tar", last modified: Wed Apr  3 18:08:53 2024, max compression
+gzip compressed data, was "ai-datahive-0.1.6.tar", last modified: Fri Apr  5 19:17:39 2024, max compression
```

## Comparing `ai-datahive-0.1.5.tar` & `ai-datahive-0.1.6.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.621750 ai-datahive-0.1.5/
--rw-rw-rw-   0        0        0     1085 2024-02-28 17:54:56.000000 ai-datahive-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       93 2024-03-19 18:04:54.000000 ai-datahive-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      570 2024-04-03 18:08:53.620750 ai-datahive-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4998 2024-03-09 15:08:20.000000 ai-datahive-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.426169 ai-datahive-0.1.5/ai_datahive/
--rw-rw-rw-   0        0        0        0 2024-03-11 14:33:26.000000 ai-datahive-0.1.5/ai_datahive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.458678 ai-datahive-0.1.5/ai_datahive/collectors/
--rw-rw-rw-   0        0        0      231 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/collectors/__init__.py
--rw-rw-rw-   0        0        0     3618 2024-04-02 16:37:45.000000 ai-datahive-0.1.5/ai_datahive/collectors/arxiv_collector.py
--rw-rw-rw-   0        0        0     1871 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/collectors/base_collector.py
--rw-rw-rw-   0        0        0     5096 2024-04-02 16:37:20.000000 ai-datahive-0.1.5/ai_datahive/collectors/civitai_collector.py
--rw-rw-rw-   0        0        0     3913 2024-04-02 16:36:56.000000 ai-datahive-0.1.5/ai_datahive/collectors/github_collector.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.471674 ai-datahive-0.1.5/ai_datahive/collectors/models/
--rw-rw-rw-   0        0        0      112 2024-03-05 20:56:45.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/__init__.py
--rw-rw-rw-   0        0        0     1023 2024-04-01 16:46:30.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/github_project.py
--rw-rw-rw-   0        0        0     2483 2024-04-01 16:30:52.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/media.py
--rw-rw-rw-   0        0        0      483 2024-04-01 16:12:36.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/research_paper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.494674 ai-datahive-0.1.5/ai_datahive/collectors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-28 13:53:11.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/__init__.py
--rw-rw-rw-   0        0        0    19908 2024-02-20 18:30:47.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/allowed_github_parameter.py
--rw-rw-rw-   0        0        0    25962 2024-03-09 15:05:32.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/arxiv_helper.py
--rw-rw-rw-   0        0        0      483 2024-02-19 18:48:46.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     7633 2024-02-28 13:58:34.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/github_helper.py
--rw-rw-rw-   0        0        0      833 2024-02-25 13:35:06.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/scraping_helper.py
--rw-rw-rw-   0        0        0     4947 2024-02-20 17:00:33.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/zotero_helper.py
--rw-rw-rw-   0        0        0     3784 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/collectors/zotero_collector.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.504673 ai-datahive-0.1.5/ai_datahive/dao/
--rw-rw-rw-   0        0        0       81 2024-04-02 15:51:26.000000 ai-datahive-0.1.5/ai_datahive/dao/__init__.py
--rw-rw-rw-   0        0        0     1245 2024-04-01 16:54:42.000000 ai-datahive-0.1.5/ai_datahive/dao/base_dao.py
--rw-rw-rw-   0        0        0     8183 2024-04-01 16:56:49.000000 ai-datahive-0.1.5/ai_datahive/dao/supabase_dao.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.512674 ai-datahive-0.1.5/ai_datahive/models/
--rw-rw-rw-   0        0        0       93 2024-03-04 19:54:55.000000 ai-datahive-0.1.5/ai_datahive/models/__init__.py
--rw-rw-rw-   0        0        0      395 2024-04-01 16:16:17.000000 ai-datahive-0.1.5/ai_datahive/models/base_model.py
--rw-rw-rw-   0        0        0      543 2024-04-01 15:28:04.000000 ai-datahive-0.1.5/ai_datahive/models/content_base_model.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.517674 ai-datahive-0.1.5/ai_datahive/publishers/
--rw-rw-rw-   0        0        0        0 2024-03-04 15:35:13.000000 ai-datahive-0.1.5/ai_datahive/publishers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.538745 ai-datahive-0.1.5/ai_datahive/publishers/loader/
--rw-rw-rw-   0        0        0       54 2024-03-06 20:28:03.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/__init__.py
--rw-rw-rw-   0        0        0     3282 2024-04-02 16:20:47.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_base_loader.py
--rw-rw-rw-   0        0        0     1377 2024-04-02 15:31:13.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py
--rw-rw-rw-   0        0        0     1464 2024-04-02 15:18:12.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py
--rw-rw-rw-   0        0        0     1391 2024-04-02 15:38:15.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py
--rw-rw-rw-   0        0        0     1322 2024-04-02 15:30:50.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.549745 ai-datahive-0.1.5/ai_datahive/publishers/models/
--rw-rw-rw-   0        0        0      144 2024-03-04 20:28:30.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/__init__.py
--rw-rw-rw-   0        0        0      171 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_group.py
--rw-rw-rw-   0        0        0      211 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_group_topic.py
--rw-rw-rw-   0        0        0      532 2024-04-01 15:40:56.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_message.py
--rw-rw-rw-   0        0        0     7256 2024-04-02 15:53:48.000000 ai-datahive-0.1.5/ai_datahive/publishers/telegram_bot.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.573745 ai-datahive-0.1.5/ai_datahive/services/
--rw-rw-rw-   0        0        0      266 2024-03-09 14:16:03.000000 ai-datahive-0.1.5/ai_datahive/services/__init__.py
--rw-rw-rw-   0        0        0      494 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/ai_backed_translation_service.py
--rw-rw-rw-   0        0        0      523 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/ai_service_factory.py
--rw-rw-rw-   0        0        0      337 2024-03-09 13:52:41.000000 ai-datahive-0.1.5/ai_datahive/services/base_ai_vision_service.py
--rw-rw-rw-   0        0        0      423 2024-03-09 14:14:43.000000 ai-datahive-0.1.5/ai_datahive/services/base_llm_service.py
--rw-rw-rw-   0        0        0      314 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/data_service.py
--rw-rw-rw-   0        0        0     2681 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/openai_service.py
--rw-rw-rw-   0        0        0     1947 2024-03-09 16:04:56.000000 ai-datahive-0.1.5/ai_datahive/services/prompt_service.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.575747 ai-datahive-0.1.5/ai_datahive/services/prompts/
--rw-rw-rw-   0        0        0     2133 2024-03-09 16:06:57.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/js_style_image_critique_prompt.txt
--rw-rw-rw-   0        0        0       50 2024-03-06 19:11:41.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/summarize_prompt.txt
--rw-rw-rw-   0        0        0       49 2024-03-06 19:11:41.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/translate_prompt.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.599747 ai-datahive-0.1.5/ai_datahive/transformers/
--rw-rw-rw-   0        0        0       62 2024-03-09 14:18:22.000000 ai-datahive-0.1.5/ai_datahive/transformers/__init__.py
--rw-rw-rw-   0        0        0     2600 2024-04-02 16:20:28.000000 ai-datahive-0.1.5/ai_datahive/transformers/base_content_transformer.py
--rw-rw-rw-   0        0        0     2710 2024-04-02 16:41:37.000000 ai-datahive-0.1.5/ai_datahive/transformers/daily_arxiv_paper_transformer.py
--rw-rw-rw-   0        0        0     2907 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/transformers/daily_trending_github_project_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.606745 ai-datahive-0.1.5/ai_datahive/transformers/models/
--rw-rw-rw-   0        0        0       30 2024-03-04 16:57:55.000000 ai-datahive-0.1.5/ai_datahive/transformers/models/__init__.py
--rw-rw-rw-   0        0        0      610 2024-03-20 16:46:25.000000 ai-datahive-0.1.5/ai_datahive/transformers/models/content.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.608747 ai-datahive-0.1.5/ai_datahive/transformers/templates/
--rw-rw-rw-   0        0        0       96 2024-03-06 19:41:54.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/daily_arxiv_paper_template.html
--rw-rw-rw-   0        0        0      132 2024-04-02 16:40:23.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/github_loader_trending_template.html
--rw-rw-rw-   0        0        0       88 2024-03-09 16:10:33.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/top_daily_image_critique_template.html
--rw-rw-rw-   0        0        0      136 2024-03-04 21:29:24.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/top_daily_image_template.html
--rw-rw-rw-   0        0        0     2858 2024-04-02 16:41:37.000000 ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_critique_transformer.py
--rw-rw-rw-   0        0        0     2463 2024-04-02 17:15:38.000000 ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.619753 ai-datahive-0.1.5/ai_datahive/utils/
--rw-rw-rw-   0        0        0        0 2024-02-25 13:31:44.000000 ai-datahive-0.1.5/ai_datahive/utils/__init__.py
--rw-rw-rw-   0        0        0      247 2024-04-02 15:55:29.000000 ai-datahive-0.1.5/ai_datahive/utils/dao_factory.py
--rw-rw-rw-   0        0        0     1957 2024-04-02 15:59:25.000000 ai-datahive-0.1.5/ai_datahive/utils/datetime_helper.py
--rw-rw-rw-   0        0        0      842 2024-03-09 14:32:24.000000 ai-datahive-0.1.5/ai_datahive/utils/text_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.620750 ai-datahive-0.1.5/ai_datahive.egg-info/
--rw-rw-rw-   0        0        0      570 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3165 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 18:08:53.621750 ai-datahive-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-04-03 18:08:41.000000 ai-datahive-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.059440 ai-datahive-0.1.6/
+-rw-rw-rw-   0        0        0     1085 2024-02-28 17:54:56.000000 ai-datahive-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       93 2024-03-19 18:04:54.000000 ai-datahive-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2024-04-05 19:17:39.058435 ai-datahive-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2024-03-09 15:08:20.000000 ai-datahive-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.870410 ai-datahive-0.1.6/ai_datahive/
+-rw-rw-rw-   0        0        0        0 2024-03-11 14:33:26.000000 ai-datahive-0.1.6/ai_datahive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.895414 ai-datahive-0.1.6/ai_datahive/collectors/
+-rw-rw-rw-   0        0        0      231 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3618 2024-04-02 16:37:45.000000 ai-datahive-0.1.6/ai_datahive/collectors/arxiv_collector.py
+-rw-rw-rw-   0        0        0     1871 2024-04-02 16:28:44.000000 ai-datahive-0.1.6/ai_datahive/collectors/base_collector.py
+-rw-rw-rw-   0        0        0     5997 2024-04-05 18:56:58.000000 ai-datahive-0.1.6/ai_datahive/collectors/civitai_collector.py
+-rw-rw-rw-   0        0        0     3913 2024-04-02 16:36:56.000000 ai-datahive-0.1.6/ai_datahive/collectors/github_collector.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.908411 ai-datahive-0.1.6/ai_datahive/collectors/models/
+-rw-rw-rw-   0        0        0      112 2024-03-05 20:56:45.000000 ai-datahive-0.1.6/ai_datahive/collectors/models/__init__.py
+-rw-rw-rw-   0        0        0     1023 2024-04-01 16:46:30.000000 ai-datahive-0.1.6/ai_datahive/collectors/models/github_project.py
+-rw-rw-rw-   0        0        0     2483 2024-04-01 16:30:52.000000 ai-datahive-0.1.6/ai_datahive/collectors/models/media.py
+-rw-rw-rw-   0        0        0      483 2024-04-01 16:12:36.000000 ai-datahive-0.1.6/ai_datahive/collectors/models/research_paper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.931409 ai-datahive-0.1.6/ai_datahive/collectors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-28 13:53:11.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/__init__.py
+-rw-rw-rw-   0        0        0    19908 2024-02-20 18:30:47.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/allowed_github_parameter.py
+-rw-rw-rw-   0        0        0    25962 2024-03-09 15:05:32.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/arxiv_helper.py
+-rw-rw-rw-   0        0        0      483 2024-02-19 18:48:46.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     7633 2024-02-28 13:58:34.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/github_helper.py
+-rw-rw-rw-   0        0        0      833 2024-02-25 13:35:06.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/scraping_helper.py
+-rw-rw-rw-   0        0        0     4947 2024-02-20 17:00:33.000000 ai-datahive-0.1.6/ai_datahive/collectors/utils/zotero_helper.py
+-rw-rw-rw-   0        0        0     3784 2024-04-02 16:28:44.000000 ai-datahive-0.1.6/ai_datahive/collectors/zotero_collector.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.940409 ai-datahive-0.1.6/ai_datahive/dao/
+-rw-rw-rw-   0        0        0       81 2024-04-02 15:51:26.000000 ai-datahive-0.1.6/ai_datahive/dao/__init__.py
+-rw-rw-rw-   0        0        0     1245 2024-04-01 16:54:42.000000 ai-datahive-0.1.6/ai_datahive/dao/base_dao.py
+-rw-rw-rw-   0        0        0     8183 2024-04-01 16:56:49.000000 ai-datahive-0.1.6/ai_datahive/dao/supabase_dao.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.948417 ai-datahive-0.1.6/ai_datahive/models/
+-rw-rw-rw-   0        0        0       93 2024-03-04 19:54:55.000000 ai-datahive-0.1.6/ai_datahive/models/__init__.py
+-rw-rw-rw-   0        0        0      395 2024-04-01 16:16:17.000000 ai-datahive-0.1.6/ai_datahive/models/base_model.py
+-rw-rw-rw-   0        0        0      543 2024-04-01 15:28:04.000000 ai-datahive-0.1.6/ai_datahive/models/content_base_model.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.953416 ai-datahive-0.1.6/ai_datahive/publishers/
+-rw-rw-rw-   0        0        0        0 2024-03-04 15:35:13.000000 ai-datahive-0.1.6/ai_datahive/publishers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.964926 ai-datahive-0.1.6/ai_datahive/publishers/loader/
+-rw-rw-rw-   0        0        0      391 2024-04-05 19:02:21.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/__init__.py
+-rw-rw-rw-   0        0        0     3282 2024-04-02 16:20:47.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_base_loader.py
+-rw-rw-rw-   0        0        0     1377 2024-04-02 15:31:13.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py
+-rw-rw-rw-   0        0        0     1470 2024-04-05 19:08:25.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py
+-rw-rw-rw-   0        0        0     1391 2024-04-02 15:38:15.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py
+-rw-rw-rw-   0        0        0     1322 2024-04-02 15:30:50.000000 ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:38.975925 ai-datahive-0.1.6/ai_datahive/publishers/models/
+-rw-rw-rw-   0        0        0      144 2024-03-04 20:28:30.000000 ai-datahive-0.1.6/ai_datahive/publishers/models/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/publishers/models/telegram_group.py
+-rw-rw-rw-   0        0        0      211 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/publishers/models/telegram_group_topic.py
+-rw-rw-rw-   0        0        0      532 2024-04-01 15:40:56.000000 ai-datahive-0.1.6/ai_datahive/publishers/models/telegram_message.py
+-rw-rw-rw-   0        0        0     7256 2024-04-02 15:53:48.000000 ai-datahive-0.1.6/ai_datahive/publishers/telegram_bot.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.002926 ai-datahive-0.1.6/ai_datahive/services/
+-rw-rw-rw-   0        0        0      266 2024-03-09 14:16:03.000000 ai-datahive-0.1.6/ai_datahive/services/__init__.py
+-rw-rw-rw-   0        0        0      494 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/services/ai_backed_translation_service.py
+-rw-rw-rw-   0        0        0      523 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/services/ai_service_factory.py
+-rw-rw-rw-   0        0        0      337 2024-03-09 13:52:41.000000 ai-datahive-0.1.6/ai_datahive/services/base_ai_vision_service.py
+-rw-rw-rw-   0        0        0      423 2024-03-09 14:14:43.000000 ai-datahive-0.1.6/ai_datahive/services/base_llm_service.py
+-rw-rw-rw-   0        0        0      314 2024-03-11 14:22:40.000000 ai-datahive-0.1.6/ai_datahive/services/data_service.py
+-rw-rw-rw-   0        0        0     2681 2024-04-03 19:24:34.000000 ai-datahive-0.1.6/ai_datahive/services/openai_service.py
+-rw-rw-rw-   0        0        0     1947 2024-03-09 16:04:56.000000 ai-datahive-0.1.6/ai_datahive/services/prompt_service.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.008926 ai-datahive-0.1.6/ai_datahive/services/prompts/
+-rw-rw-rw-   0        0        0       44 2024-04-03 19:22:02.000000 ai-datahive-0.1.6/ai_datahive/services/prompts/image_caption_prompt.txt
+-rw-rw-rw-   0        0        0     2133 2024-04-03 19:24:25.000000 ai-datahive-0.1.6/ai_datahive/services/prompts/js_style_image_critique_prompt.txt
+-rw-rw-rw-   0        0        0       50 2024-03-06 19:11:41.000000 ai-datahive-0.1.6/ai_datahive/services/prompts/summarize_prompt.txt
+-rw-rw-rw-   0        0        0       49 2024-03-06 19:11:41.000000 ai-datahive-0.1.6/ai_datahive/services/prompts/translate_prompt.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.031926 ai-datahive-0.1.6/ai_datahive/transformers/
+-rw-rw-rw-   0        0        0      378 2024-04-05 18:09:02.000000 ai-datahive-0.1.6/ai_datahive/transformers/__init__.py
+-rw-rw-rw-   0        0        0     2610 2024-04-03 18:39:20.000000 ai-datahive-0.1.6/ai_datahive/transformers/base_content_transformer.py
+-rw-rw-rw-   0        0        0     2710 2024-04-02 16:41:37.000000 ai-datahive-0.1.6/ai_datahive/transformers/daily_arxiv_paper_transformer.py
+-rw-rw-rw-   0        0        0     2907 2024-04-02 16:28:44.000000 ai-datahive-0.1.6/ai_datahive/transformers/daily_trending_github_project_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.036927 ai-datahive-0.1.6/ai_datahive/transformers/models/
+-rw-rw-rw-   0        0        0       30 2024-03-04 16:57:55.000000 ai-datahive-0.1.6/ai_datahive/transformers/models/__init__.py
+-rw-rw-rw-   0        0        0      610 2024-03-20 16:46:25.000000 ai-datahive-0.1.6/ai_datahive/transformers/models/content.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.043930 ai-datahive-0.1.6/ai_datahive/transformers/templates/
+-rw-rw-rw-   0        0        0       96 2024-03-06 19:41:54.000000 ai-datahive-0.1.6/ai_datahive/transformers/templates/daily_arxiv_paper_template.html
+-rw-rw-rw-   0        0        0      132 2024-04-02 16:40:23.000000 ai-datahive-0.1.6/ai_datahive/transformers/templates/github_loader_trending_template.html
+-rw-rw-rw-   0        0        0       88 2024-03-09 16:10:33.000000 ai-datahive-0.1.6/ai_datahive/transformers/templates/top_daily_image_critique_template.html
+-rw-rw-rw-   0        0        0      136 2024-03-04 21:29:24.000000 ai-datahive-0.1.6/ai_datahive/transformers/templates/top_daily_image_template.html
+-rw-rw-rw-   0        0        0     3403 2024-04-05 18:27:00.000000 ai-datahive-0.1.6/ai_datahive/transformers/top_daily_image_critique_transformer.py
+-rw-rw-rw-   0        0        0     2463 2024-04-02 17:15:38.000000 ai-datahive-0.1.6/ai_datahive/transformers/top_daily_image_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.056930 ai-datahive-0.1.6/ai_datahive/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-25 13:31:44.000000 ai-datahive-0.1.6/ai_datahive/utils/__init__.py
+-rw-rw-rw-   0        0        0      247 2024-04-02 15:55:29.000000 ai-datahive-0.1.6/ai_datahive/utils/dao_factory.py
+-rw-rw-rw-   0        0        0     1957 2024-04-02 15:59:25.000000 ai-datahive-0.1.6/ai_datahive/utils/datetime_helper.py
+-rw-rw-rw-   0        0        0      948 2024-04-03 19:09:34.000000 ai-datahive-0.1.6/ai_datahive/utils/image_helper.py
+-rw-rw-rw-   0        0        0      842 2024-03-09 14:32:24.000000 ai-datahive-0.1.6/ai_datahive/utils/text_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:17:39.058435 ai-datahive-0.1.6/ai_datahive.egg-info/
+-rw-rw-rw-   0        0        0      593 2024-04-05 19:17:38.000000 ai-datahive-0.1.6/ai_datahive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3253 2024-04-05 19:17:38.000000 ai-datahive-0.1.6/ai_datahive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:17:38.000000 ai-datahive-0.1.6/ai_datahive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-05 19:17:38.000000 ai-datahive-0.1.6/ai_datahive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 19:17:38.000000 ai-datahive-0.1.6/ai_datahive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:17:39.059440 ai-datahive-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-04-05 19:17:34.000000 ai-datahive-0.1.6/setup.py
```

### Comparing `ai-datahive-0.1.5/LICENSE` & `ai-datahive-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/PKG-INFO` & `ai-datahive-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ai-datahive
-Version: 0.1.5
+Version: 0.1.6
 Summary: ETL Package for crawling data, transform it with AI and store it in a datastorage.
 Author: Danny Gerst
 Author-email: d.gerst@bizrock.de
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: inflect
+Requires-Dist: pillow
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
 Requires-Dist: apscheduler
 Requires-Dist: sqlalchemy
 Requires-Dist: supabase
 Requires-Dist: feedparser
```

### Comparing `ai-datahive-0.1.5/README.md` & `ai-datahive-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/arxiv_collector.py` & `ai-datahive-0.1.6/ai_datahive/collectors/arxiv_collector.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/base_collector.py` & `ai-datahive-0.1.6/ai_datahive/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/civitai_collector.py` & `ai-datahive-0.1.6/ai_datahive/collectors/civitai_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,38 +8,41 @@
 
 from ai_datahive.collectors.models import Media
 
 
 class CivitaiCollector(BaseCollector):
     VALID_PERIODS = ['AllTime', 'Year', 'Month', 'Week', 'Day']
     VALID_MEDIA_TYPES = ['image', 'video', 'model']
-    VALID_NSFW_LEVELS = [None, 'Soft', 'Mature', 'X']
+    VALID_NSFW_LEVELS = ['None', 'Soft', 'Mature', 'X']
     VALID_SORTS = ['Most Reactions', 'Most Buzz', 'Most Comments', 'Most Collected', 'Oldest']
 
     def __init__(self, creator='CivitaiCollector', media_type='image', period='Day', sort='Most Reactions',
-                 nsfw=None, tags=None, limit=1):
+                 nsfw_level='None', tags=None, limit=10):
         self.creator = creator
+        self.nsfw_level = nsfw_level
         if tags is None:
-            self.tags = self.build_tags(media_type, period, sort, nsfw)
+            self.tags = self.build_tags(media_type, period, sort, self.nsfw_level)
         else:
             self.tags = tags
         self.limit = limit
 
-        self.validate_parameters(media_type, period, nsfw, sort)
+        if self.nsfw_level is None:
+            self.nsfw_level = 'None'
+        self.validate_parameters(media_type, period, self.nsfw_level, sort)
 
         # TODO Right now, there is no way to determine videos directly from Civitai API
         # START - Workaround as long as there is no way to get videos directly from Civitai
         if media_type == 'video':
             self.media_type = 'image'
         else:
             self.media_type = media_type
         # END - Workaround as long as there is no way to get videos directly from Civitai
 
         base_url = os.getenv('CIVITAI_API_URL', '')
-        self.civitai_url = self.build_url(base_url, media_type, sort, nsfw, period, limit)
+        self.civitai_url = self.build_url(base_url, media_type, sort, self.nsfw_level, period)
 
         super().__init__(creator=self.creator, content_type=Media)
 
     def build_tags(self, media_type, period, sort, nsfw):
         tags = 'civitai, '
         tags += media_type.lower() + ', '
         tags += to_periodic_format(period) + ', '
@@ -57,38 +60,55 @@
         if media_type not in self.VALID_MEDIA_TYPES:
             raise ValueError(f"media_type must be one of {self.VALID_MEDIA_TYPES}")
         if nsfw not in self.VALID_NSFW_LEVELS:
             raise ValueError(f"nsfw must be one of {self.VALID_NSFW_LEVELS}")
         if sort not in self.VALID_SORTS:
             raise ValueError(f"sort must be one of {self.VALID_SORTS}")
 
-    def build_url(self, base_url, media_type, sort, nsfw, period, limit):
+    def build_url(self, base_url, media_type, sort, nsfw, period):
+        api_limit = 100  # Maximum limit for Civitai API
         path = f"{media_type}s"  # Append 's' to make it plural (image -> images, video -> videos, model -> models)
         params = {
             'nsfw': nsfw if nsfw is not None else 'None',
-            'limit': limit,
+            'limit': api_limit,
             'period': period,
             'sort': sort
         }
         query_string = urlencode({k: v for k, v in params.items() if v is not None})  # Exclude None values
         return urljoin(base_url, path) + '?' + query_string
 
     def retrieve(self):
-        data = get_request_as_json(self.civitai_url)
-        if isinstance(data, dict):
-            media = self.convert_to_media(data)
-            return media
-        else:
-            # Fehlerbehandlung
-            print(f"Es gab einen Fehler bei der Anfrage: {data}")
+        exit_count = 3
+        current_page = self.civitai_url
+        while exit_count > 0:
+            data = get_request_as_json(current_page)
+            if isinstance(data, dict):
+                item_list = []
+                for item in data['items']:
+                    if item['nsfwLevel'] == self.nsfw_level:
+                        item_list.append(item)
+                if len(item_list) >= self.limit:
+                    print('Iam out')
+                    media = self.convert_to_media(item_list[:self.limit])
+                    return media
+                exit_count -= 1
+                if data.get('metadata') and data.get('metadata').get('nextPage'):
+                    current_page = data['metadata']['nextPage']
+                else:
+                    break
+            else:
+                # Fehlerbehandlung
+                print(f"Es gab einen Fehler bei der Anfrage: {data}")
+                return None
 
     def convert_to_media(self, data):
         result = []
         if data:
-            for item in data['items']:
+            print(data)
+            for item in data:
                 media = Media(
                     creator=self.creator,
                     media_url=item['url'],
                     media_type=self.media_type,
                     likes=item['stats']['likeCount'],
                     hearts=item['stats']['heartCount'],
                     prompt=item['meta'].get('prompt') if item.get('meta') is not None else None,
```

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/github_collector.py` & `ai-datahive-0.1.6/ai_datahive/collectors/github_collector.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/models/github_project.py` & `ai-datahive-0.1.6/ai_datahive/collectors/models/github_project.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/models/media.py` & `ai-datahive-0.1.6/ai_datahive/collectors/models/media.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/utils/allowed_github_parameter.py` & `ai-datahive-0.1.6/ai_datahive/collectors/utils/allowed_github_parameter.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/utils/arxiv_helper.py` & `ai-datahive-0.1.6/ai_datahive/collectors/utils/arxiv_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/utils/github_helper.py` & `ai-datahive-0.1.6/ai_datahive/collectors/utils/github_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/utils/scraping_helper.py` & `ai-datahive-0.1.6/ai_datahive/collectors/utils/scraping_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/utils/zotero_helper.py` & `ai-datahive-0.1.6/ai_datahive/collectors/utils/zotero_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/collectors/zotero_collector.py` & `ai-datahive-0.1.6/ai_datahive/collectors/zotero_collector.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/dao/base_dao.py` & `ai-datahive-0.1.6/ai_datahive/dao/base_dao.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/dao/supabase_dao.py` & `ai-datahive-0.1.6/ai_datahive/dao/supabase_dao.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/models/content_base_model.py` & `ai-datahive-0.1.6/ai_datahive/models/content_base_model.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_base_loader.py` & `ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_base_loader.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py` & `ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py` & `ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 
         return projects
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
-    ARXIV_GROUP_TOPIC_ID = 20
-    loader = TelegramDailyTrendingGithubProjectsLoader('KI & Business', ARXIV_GROUP_TOPIC_ID)
+    PROJECTS_GROUP_TOPIC_ID = 20
+    loader = TelegramDailyTrendingGithubProjectsLoader('KI & Business', PROJECTS_GROUP_TOPIC_ID)
     loader.load()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py` & `ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py` & `ai-datahive-0.1.6/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_message.py` & `ai-datahive-0.1.6/ai_datahive/publishers/models/telegram_message.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/publishers/telegram_bot.py` & `ai-datahive-0.1.6/ai_datahive/publishers/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/services/ai_service_factory.py` & `ai-datahive-0.1.6/ai_datahive/services/ai_service_factory.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/services/openai_service.py` & `ai-datahive-0.1.6/ai_datahive/services/openai_service.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/services/prompt_service.py` & `ai-datahive-0.1.6/ai_datahive/services/prompt_service.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/services/prompts/js_style_image_critique_prompt.txt` & `ai-datahive-0.1.6/ai_datahive/services/prompts/js_style_image_critique_prompt.txt`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/base_content_transformer.py` & `ai-datahive-0.1.6/ai_datahive/transformers/base_content_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     def __init__(self, creator, template_file_name, language, run_interval: timedelta = timedelta(days=1)):
         from ai_datahive.utils.dao_factory import get_dao
         self.dao = get_dao()
         self.language = language
         self.creator = creator
         self.run_interval = run_interval
         caller_file = inspect.getfile(self.__class__)
-        template_file_path = os.path.join(caller_file, 'templates', template_file_name)
+        caller_dir = os.path.dirname(caller_file)
+        template_file_path = os.path.join(caller_dir, 'templates', template_file_name)
         if os.path.exists(template_file_path):
-            self.template_path = os.path.join(caller_file, 'templates', template_file_name)
+            self.template_path = template_file_path
         elif os.path.exists(os.path.join(os.path.dirname(__file__), 'templates', template_file_name)):
             self.template_path = os.path.join(os.path.dirname(__file__), 'templates', template_file_name)
         else:
             self.template_path = os.path.join('templates', template_file_name)
 
     def save(self, content: Union[Content, Collection[Content]]):
         if isinstance(content, Collection):
```

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/daily_arxiv_paper_transformer.py` & `ai-datahive-0.1.6/ai_datahive/transformers/daily_arxiv_paper_transformer.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/daily_trending_github_project_transformer.py` & `ai-datahive-0.1.6/ai_datahive/transformers/daily_trending_github_project_transformer.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/models/content.py` & `ai-datahive-0.1.6/ai_datahive/transformers/models/content.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_critique_transformer.py` & `ai-datahive-0.1.6/ai_datahive/transformers/top_daily_image_critique_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
 
 from ai_datahive.transformers import BaseContentTransformer
 
 from ai_datahive.collectors.models import Media
 from ai_datahive.transformers.models import Content
 
@@ -18,50 +20,58 @@
 
         super().__init__(creator=creator, template_file_name=template_file_name, language=language)
 
     def retrieve(self) -> Media:
         start_date_str, end_date_str = today_as_start_and_enddate_str()
 
         filters = [["creator", "CivitAIDailyTopImage"], ['created_at', 'between', start_date_str, end_date_str]]
-        media = self.dao.read(Media, filters, limit=1, order_by='likes')
-        return media[0] if media else None
+        media = self.dao.read(Media, filters, limit=3, order_by='likes', order_dir='desc')
+        return media
 
-    def transform(self, topdailyimage: Media) -> Content:
+    def transform(self, topdailyimages: List['Media']) -> Content:
 
-        if topdailyimage:
-            image_language = topdailyimage.lang
-            system_prompt = self.ps.create_system_prompt_from_file('js_style_image_critique_prompt.txt')
-
-            user_prompt = f"Prompt: {topdailyimage.prompt}\nartist: {topdailyimage.author}"
-            critique = self.oais.vision_response(system_prompt=system_prompt, user_prompt=user_prompt,
-                                                 image_url=topdailyimage.media_url)
-            if self.language != image_language:
-                critique = self.ts.translate(critique, self.language)
-
-            template_data = {
-                'critique': critique,
-                'author': topdailyimage.author,
-                'created_at': topdailyimage.media_created_at,
-                'media_url': topdailyimage.media_url,
-            }
-            str_content = self.create_content(template_data)
-
-            content = Content(
-                creator=self.creator,
-                tags=topdailyimage.tags+', critique, JS style',
-                title=f'Die Bildkritik mit Saltz',
-                content=str_content,
-                media_url=topdailyimage.media_url,
-                media_type='image',
-                media_created_at=topdailyimage.media_created_at,
-                source_name=topdailyimage.source_name,
-                source_url=topdailyimage.source_url,
-                lang=self.language
-            )
-            return content
+        if topdailyimages:
+            for topdailyimage in topdailyimages:
+                image_language = topdailyimage.lang
+                system_prompt = self.ps.create_system_prompt_from_file('js_style_image_critique_prompt.txt')
+
+                user_prompt = f"Prompt: {topdailyimage.prompt}\nartist: {topdailyimage.author}"
+
+                critique = self.oais.vision_response(system_prompt=system_prompt, user_prompt=user_prompt,
+                                                     image_url=topdailyimage.media_url)
+                print(critique)
+                if "I'm sorry" in critique and "can't" in critique:
+                    print(f'I could not get the GPT-4V critique for the image: Image URL {topdailyimage.media_url}')
+                    continue
+
+                if self.language != image_language:
+                    critique = self.ts.translate(critique, self.language)
+
+                template_data = {
+                    'critique': critique,
+                    'author': topdailyimage.author,
+                    'created_at': topdailyimage.media_created_at,
+                    'media_url': topdailyimage.media_url,
+                }
+                str_content = self.create_content(template_data)
+
+                content = Content(
+                    creator=self.creator,
+                    tags=topdailyimage.tags+', critique, JS style',
+                    title=f'Die Bildkritik mit Saltz',
+                    content=str_content,
+                    media_url=topdailyimage.media_url,
+                    media_type='image',
+                    media_created_at=topdailyimage.media_created_at,
+                    source_name=topdailyimage.source_name,
+                    source_url=topdailyimage.source_url,
+                    lang=self.language
+                )
+                return content
+            print('I could not get the GPT-4V critique for the image. No critique was generated.')
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
 
     transformer = TopDailyImageCritiqueTransformer()
```

### Comparing `ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_transformer.py` & `ai-datahive-0.1.6/ai_datahive/transformers/top_daily_image_transformer.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/utils/datetime_helper.py` & `ai-datahive-0.1.6/ai_datahive/utils/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive/utils/text_helper.py` & `ai-datahive-0.1.6/ai_datahive/utils/text_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.5/ai_datahive.egg-info/PKG-INFO` & `ai-datahive-0.1.6/ai_datahive.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ai-datahive
-Version: 0.1.5
+Version: 0.1.6
 Summary: ETL Package for crawling data, transform it with AI and store it in a datastorage.
 Author: Danny Gerst
 Author-email: d.gerst@bizrock.de
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: inflect
+Requires-Dist: pillow
 Requires-Dist: requests
 Requires-Dist: bs4
 Requires-Dist: lxml
 Requires-Dist: apscheduler
 Requires-Dist: sqlalchemy
 Requires-Dist: supabase
 Requires-Dist: feedparser
```

### Comparing `ai-datahive-0.1.5/ai_datahive.egg-info/SOURCES.txt` & `ai-datahive-0.1.6/ai_datahive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ai_datahive/services/ai_backed_translation_service.py
 ai_datahive/services/ai_service_factory.py
 ai_datahive/services/base_ai_vision_service.py
 ai_datahive/services/base_llm_service.py
 ai_datahive/services/data_service.py
 ai_datahive/services/openai_service.py
 ai_datahive/services/prompt_service.py
+ai_datahive/services/prompts/image_caption_prompt.txt
 ai_datahive/services/prompts/js_style_image_critique_prompt.txt
 ai_datahive/services/prompts/summarize_prompt.txt
 ai_datahive/services/prompts/translate_prompt.txt
 ai_datahive/transformers/__init__.py
 ai_datahive/transformers/base_content_transformer.py
 ai_datahive/transformers/daily_arxiv_paper_transformer.py
 ai_datahive/transformers/daily_trending_github_project_transformer.py
@@ -65,8 +66,9 @@
 ai_datahive/transformers/templates/daily_arxiv_paper_template.html
 ai_datahive/transformers/templates/github_loader_trending_template.html
 ai_datahive/transformers/templates/top_daily_image_critique_template.html
 ai_datahive/transformers/templates/top_daily_image_template.html
 ai_datahive/utils/__init__.py
 ai_datahive/utils/dao_factory.py
 ai_datahive/utils/datetime_helper.py
+ai_datahive/utils/image_helper.py
 ai_datahive/utils/text_helper.py
```

### Comparing `ai-datahive-0.1.5/setup.py` & `ai-datahive-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_requirements():
     with open('requirements.txt') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='ai-datahive',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     package_data={
         'ai_datahive': ['transformers/templates/*.html', 'services/prompts/*.txt'],
     },
     include_package_data=True,
     description='ETL Package for crawling data, transform it with AI and store it in a datastorage.',
     author='Danny Gerst',
```

