# Comparing `tmp/khoj_assistant-1.8.1.dev56.tar.gz` & `tmp/khoj_assistant-1.8.1.dev58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr  4 05:01:13 2024, max compression
+gzip compressed data, last modified: Fri Apr  5 06:40:03 2024, max compression
```

## Comparing `khoj_assistant-1.8.1.dev56.tar` & `khoj_assistant-1.8.1.dev58.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/__init__.py
--rw-r--r--   0        0        0    14822 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/configure.py
--rw-r--r--   0        0        0     5330 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/main.py
--rwxr-xr-x   0        0        0      664 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/manage.py
--rw-r--r--   0        0        0     2832 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/app/README.md
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/app/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/app/settings.py
--rw-r--r--   0        0        0      869 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/app/urls.py
--rw-r--r--   0        0        0      388 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/__init__.py
--rw-r--r--   0        0        0     5419 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/admin.py
--rw-r--r--   0        0        0      153 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/apps.py
--rw-r--r--   0        0        0       60 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/tests.py
--rw-r--r--   0        0        0    33510 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/adapters/__init__.py
--rw-r--r--   0        0        0     4077 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0001_khojuser.py
--rw-r--r--   0        0        0     1195 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0002_googleuser.py
--rw-r--r--   0        0        0      224 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0003_vector_extension.py
--rw-r--r--   0        0        0     8202 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0004_content_types_and_more.py
--rw-r--r--   0        0        0      429 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0005_embeddings_corpus_id.py
--rw-r--r--   0        0        0     1131 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0006_embeddingsdates.py
--rw-r--r--   0        0        0      917 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0007_add_conversation.py
--rw-r--r--   0        0        0      399 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
--rw-r--r--   0        0        0      876 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0009_khojapiuser.py
--rw-r--r--   0        0        0     3347 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
--rw-r--r--   0        0        0      773 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
--rw-r--r--   0        0        0      331 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0011_merge_20231102_0138.py
--rw-r--r--   0        0        0      552 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0012_entry_file_source.py
--rw-r--r--   0        0        0     1311 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0013_subscription.py
--rw-r--r--   0        0        0      411 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0014_alter_googleuser_picture.py
--rw-r--r--   0        0        0      584 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0015_alter_subscription_user.py
--rw-r--r--   0        0        0      429 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
--rw-r--r--   0        0        0     1219 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0017_searchmodel.py
--rw-r--r--   0        0        0     1152 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
--rw-r--r--   0        0        0      843 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
--rw-r--r--   0        0        0     1190 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0020_reflectivequestion.py
--rw-r--r--   0        0        0     1504 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
--rw-r--r--   0        0        0      904 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
--rw-r--r--   0        0        0     1122 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0023_usersearchmodelconfig.py
--rw-r--r--   0        0        0      405 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0024_alter_entry_embeddings.py
--rw-r--r--   0        0        0     1573 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
--rw-r--r--   0        0        0      691 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      731 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      375 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0027_merge_20240118_1324.py
--rw-r--r--   0        0        0      405 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
--rw-r--r--   0        0        0      934 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0029_userrequests.py
--rw-r--r--   0        0        0     1252 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0030_conversation_slug_and_title.py
--rw-r--r--   0        0        0     2033 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0031_agent_conversation_agent.py
--rw-r--r--   0        0        0      812 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0031_alter_googleuser_locale.py
--rw-r--r--   0        0        0      317 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0032_merge_20240322_0427.py
--rw-r--r--   0        0        0      369 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
--rw-r--r--   0        0        0     1251 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/__init__.py
--rw-r--r--   0        0        0    11129 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/database/models/__init__.py
--rw-r--r--   0        0        0     1651 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     8953 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/agent.html
--rw-r--r--   0        0        0     6672 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/agents.html
--rw-r--r--   0        0        0    11089 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0   112026 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    37581 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     5367 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_computer_input.html
--rw-r--r--   0        0        0     7225 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_github_input.html
--rw-r--r--   0        0        0     3655 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_notion_input.html
--rw-r--r--   0        0        0     1628 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0     4218 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/login.html
--rw-r--r--   0        0        0     2910 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0    18326 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/search.html
--rw-r--r--   0        0        0     2168 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/utils.html
--rw-r--r--   0        0        0     5160 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73396 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0     1222 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/utils.js
--rw-r--r--   0        0        0    51584 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0    10517 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/computer.png
--rw-r--r--   0        0        0      549 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0      503 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/copy-solid.svg
--rw-r--r--   0        0        0      746 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/copy_button.svg
--rw-r--r--   0        0        0    19662 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/credit-card.png
--rw-r--r--   0        0        0   205167 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    30234 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-256x256.png
--rw-r--r--   0        0        0    31531 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0     1100 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/key.svg
--rw-r--r--   0        0        0    13011 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0    29856 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
--rw-r--r--   0        0        0  1301428 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0      616 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/microphone-solid.svg
--rw-r--r--   0        0        0     1578 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     1736 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/openai-logomark.svg
--rw-r--r--   0        0        0     7946 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     2945 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/plaintext.svg
--rw-r--r--   0        0        0     1877 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0     1319 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/stop-solid.svg
--rw-r--r--   0        0        0      503 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/trash-solid.svg
--rw-r--r--   0        0        0     2233 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/user-silhouette.svg
--rw-r--r--   0        0        0      951 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/web.svg
--rw-r--r--   0        0        0     2417 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/whatsapp.svg
--rw-r--r--   0        0        0   591182 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
--rw-r--r--   0        0        0   197173 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
--rw-r--r--   0        0        0   268309 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
--rw-r--r--   0        0        0   406179 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
--rw-r--r--   0        0        0    82985 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
--rw-r--r--   0        0        0   236285 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_default_model.py
--rw-r--r--   0        0        0     2034 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_default_model_2.py
--rw-r--r--   0        0        0     2510 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_schema.py
--rw-r--r--   0        0        0      975 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_model.py
--rw-r--r--   0        0        0     2025 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_processor_config_openai.py
--rw-r--r--   0        0        0     5132 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_server_pg.py
--rw-r--r--   0        0        0      569 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_version.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4715 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/__init__.py
--rw-r--r--   0        0        0    12604 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/text_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/github/__init__.py
--rw-r--r--   0        0        0    13829 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/github/github_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/markdown/__init__.py
--rw-r--r--   0        0        0     5690 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/markdown/markdown_to_entries.py
--rw-r--r--   0        0        0     9871 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/notion/notion_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/org_mode/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/org_mode/org_to_entries.py
--rw-r--r--   0        0        0    18246 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/pdf/__init__.py
--rw-r--r--   0        0        0     4660 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/pdf/pdf_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/plaintext/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/content/plaintext/plaintext_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0    21189 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0    10226 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/__init__.py
--rw-r--r--   0        0        0     8615 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/chat_model.py
--rw-r--r--   0        0        0     1793 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/utils.py
--rw-r--r--   0        0        0      470 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/whisper.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/__init__.py
--rw-r--r--   0        0        0     6896 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/gpt.py
--rw-r--r--   0        0        0     3284 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/utils.py
--rw-r--r--   0        0        0      432 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/whisper.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/tools/__init__.py
--rw-r--r--   0        0        0     5929 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/processor/tools/online_search.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    15036 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1443 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/api_agents.py
--rw-r--r--   0        0        0    24398 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/api_chat.py
--rw-r--r--   0        0        0    10614 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/api_config.py
--rw-r--r--   0        0        0     2208 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/api_phone.py
--rw-r--r--   0        0        0     4569 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/auth.py
--rw-r--r--   0        0        0    28306 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0    12706 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/indexer.py
--rw-r--r--   0        0        0     1151 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/storage.py
--rw-r--r--   0        0        0     4285 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/subscription.py
--rw-r--r--   0        0        0     1081 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/twilio.py
--rw-r--r--   0        0        0    13166 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      358 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0    10101 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0      939 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     1005 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11451 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0     8916 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     3466 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     1866 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/config.py
--rw-r--r--   0        0        0      791 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     9519 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/fs_syncer.py
--rw-r--r--   0        0        0    12034 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     7245 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/initialization.py
--rw-r--r--   0        0        0     1192 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2009 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4028 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1354 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1430 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      565 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/.gitignore
--rw-r--r--   0        0        0    34523 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/LICENSE
--rw-r--r--   0        0        0     2007 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/README.md
--rw-r--r--   0        0        0     3456 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/pyproject.toml
--rw-r--r--   0        0        0     5259 2024-04-04 05:01:13.000000 khoj_assistant-1.8.1.dev56/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/__init__.py
+-rw-r--r--   0        0        0    14395 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/configure.py
+-rw-r--r--   0        0        0     5330 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/main.py
+-rwxr-xr-x   0        0        0      664 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/manage.py
+-rw-r--r--   0        0        0     2832 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/app/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/app/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/app/settings.py
+-rw-r--r--   0        0        0      869 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/app/urls.py
+-rw-r--r--   0        0        0      388 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/__init__.py
+-rw-r--r--   0        0        0     5523 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/admin.py
+-rw-r--r--   0        0        0      153 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/apps.py
+-rw-r--r--   0        0        0       60 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/tests.py
+-rw-r--r--   0        0        0    33625 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/adapters/__init__.py
+-rw-r--r--   0        0        0     4077 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0001_khojuser.py
+-rw-r--r--   0        0        0     1195 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0002_googleuser.py
+-rw-r--r--   0        0        0      224 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0003_vector_extension.py
+-rw-r--r--   0        0        0     8202 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0004_content_types_and_more.py
+-rw-r--r--   0        0        0      429 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0005_embeddings_corpus_id.py
+-rw-r--r--   0        0        0     1131 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0006_embeddingsdates.py
+-rw-r--r--   0        0        0      917 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0007_add_conversation.py
+-rw-r--r--   0        0        0      399 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
+-rw-r--r--   0        0        0      876 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0009_khojapiuser.py
+-rw-r--r--   0        0        0     3347 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
+-rw-r--r--   0        0        0      773 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
+-rw-r--r--   0        0        0      331 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0011_merge_20231102_0138.py
+-rw-r--r--   0        0        0      552 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0012_entry_file_source.py
+-rw-r--r--   0        0        0     1311 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0013_subscription.py
+-rw-r--r--   0        0        0      411 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0014_alter_googleuser_picture.py
+-rw-r--r--   0        0        0      584 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0015_alter_subscription_user.py
+-rw-r--r--   0        0        0      429 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
+-rw-r--r--   0        0        0     1219 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0017_searchmodel.py
+-rw-r--r--   0        0        0     1152 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
+-rw-r--r--   0        0        0      843 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
+-rw-r--r--   0        0        0     1190 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0020_reflectivequestion.py
+-rw-r--r--   0        0        0     1504 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
+-rw-r--r--   0        0        0      904 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
+-rw-r--r--   0        0        0     1122 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0023_usersearchmodelconfig.py
+-rw-r--r--   0        0        0      405 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0024_alter_entry_embeddings.py
+-rw-r--r--   0        0        0     1573 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
+-rw-r--r--   0        0        0      691 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      731 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      375 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0027_merge_20240118_1324.py
+-rw-r--r--   0        0        0      405 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
+-rw-r--r--   0        0        0      934 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0029_userrequests.py
+-rw-r--r--   0        0        0     1252 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0030_conversation_slug_and_title.py
+-rw-r--r--   0        0        0     2033 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0031_agent_conversation_agent.py
+-rw-r--r--   0        0        0      812 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0031_alter_googleuser_locale.py
+-rw-r--r--   0        0        0      317 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0032_merge_20240322_0427.py
+-rw-r--r--   0        0        0      369 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
+-rw-r--r--   0        0        0     1251 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/__init__.py
+-rw-r--r--   0        0        0    11129 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/database/models/__init__.py
+-rw-r--r--   0        0        0     1651 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     8953 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/agent.html
+-rw-r--r--   0        0        0     6672 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/agents.html
+-rw-r--r--   0        0        0    11089 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0   112026 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    38365 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     5367 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_computer_input.html
+-rw-r--r--   0        0        0     7225 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_github_input.html
+-rw-r--r--   0        0        0     3497 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_notion_input.html
+-rw-r--r--   0        0        0     1628 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0     4218 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/login.html
+-rw-r--r--   0        0        0     2910 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0    18326 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/search.html
+-rw-r--r--   0        0        0     2168 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/utils.html
+-rw-r--r--   0        0        0     5160 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73396 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0     1222 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/utils.js
+-rw-r--r--   0        0        0    51584 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0    10517 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/computer.png
+-rw-r--r--   0        0        0      549 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0      503 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/copy-solid.svg
+-rw-r--r--   0        0        0      746 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/copy_button.svg
+-rw-r--r--   0        0        0    19662 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/credit-card.png
+-rw-r--r--   0        0        0   205167 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    30234 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-256x256.png
+-rw-r--r--   0        0        0    31531 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0     1100 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/key.svg
+-rw-r--r--   0        0        0    13011 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0    29856 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
+-rw-r--r--   0        0        0  1301428 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0      616 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/microphone-solid.svg
+-rw-r--r--   0        0        0     1578 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     1736 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/openai-logomark.svg
+-rw-r--r--   0        0        0     7946 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     2945 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/plaintext.svg
+-rw-r--r--   0        0        0     1877 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0     1319 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/stop-solid.svg
+-rw-r--r--   0        0        0      503 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/trash-solid.svg
+-rw-r--r--   0        0        0     2233 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/user-silhouette.svg
+-rw-r--r--   0        0        0      951 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/web.svg
+-rw-r--r--   0        0        0     2417 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/whatsapp.svg
+-rw-r--r--   0        0        0   591182 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
+-rw-r--r--   0        0        0   197173 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
+-rw-r--r--   0        0        0   268309 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
+-rw-r--r--   0        0        0   406179 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
+-rw-r--r--   0        0        0    82985 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
+-rw-r--r--   0        0        0   236285 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_default_model.py
+-rw-r--r--   0        0        0     2034 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_default_model_2.py
+-rw-r--r--   0        0        0     2510 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_schema.py
+-rw-r--r--   0        0        0      975 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_model.py
+-rw-r--r--   0        0        0     2025 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_processor_config_openai.py
+-rw-r--r--   0        0        0     5132 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_server_pg.py
+-rw-r--r--   0        0        0      569 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_version.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/__init__.py
+-rw-r--r--   0        0        0    12604 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/text_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/github/__init__.py
+-rw-r--r--   0        0        0    13829 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/github/github_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/markdown/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/markdown/markdown_to_entries.py
+-rw-r--r--   0        0        0     9871 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/notion/notion_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/org_mode/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/org_mode/org_to_entries.py
+-rw-r--r--   0        0        0    18246 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/pdf/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/pdf/pdf_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/plaintext/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/content/plaintext/plaintext_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0    21189 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0    10226 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/__init__.py
+-rw-r--r--   0        0        0     8615 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/chat_model.py
+-rw-r--r--   0        0        0     1793 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/utils.py
+-rw-r--r--   0        0        0      470 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/__init__.py
+-rw-r--r--   0        0        0     6896 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/gpt.py
+-rw-r--r--   0        0        0     3284 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/utils.py
+-rw-r--r--   0        0        0      432 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/tools/__init__.py
+-rw-r--r--   0        0        0     5929 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/processor/tools/online_search.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13865 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1443 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/api_agents.py
+-rw-r--r--   0        0        0    24398 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/api_chat.py
+-rw-r--r--   0        0        0    10614 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/api_config.py
+-rw-r--r--   0        0        0     2208 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/api_phone.py
+-rw-r--r--   0        0        0     4569 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/auth.py
+-rw-r--r--   0        0        0    28306 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0    10974 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/indexer.py
+-rw-r--r--   0        0        0     3056 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/notion.py
+-rw-r--r--   0        0        0     1151 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/storage.py
+-rw-r--r--   0        0        0     4285 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/subscription.py
+-rw-r--r--   0        0        0     1081 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/twilio.py
+-rw-r--r--   0        0        0    13329 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0    10101 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0      939 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     1005 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0     8916 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     1740 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/config.py
+-rw-r--r--   0        0        0      791 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     9519 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/fs_syncer.py
+-rw-r--r--   0        0        0    12034 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     7245 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/initialization.py
+-rw-r--r--   0        0        0     1192 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2009 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4028 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1309 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1430 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      565 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/LICENSE
+-rw-r--r--   0        0        0     2378 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/README.md
+-rw-r--r--   0        0        0     3456 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/pyproject.toml
+-rw-r--r--   0        0        0     5630 2024-04-05 06:40:03.000000 khoj_assistant-1.8.1.dev58/PKG-INFO
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/configure.py` & `khoj_assistant-1.8.1.dev58/src/khoj/configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     aget_user_subscription_state,
     delete_user_requests,
     get_all_users,
     get_or_create_search_models,
 )
 from khoj.database.models import ClientApplication, KhojUser, Subscription
 from khoj.processor.embeddings import CrossEncoderModel, EmbeddingsModel
-from khoj.routers.indexer import configure_content, configure_search, load_content
+from khoj.routers.indexer import configure_content, configure_search
 from khoj.routers.twilio import is_twilio_enabled
 from khoj.utils import constants, state
 from khoj.utils.config import SearchType
 from khoj.utils.fs_syncer import collect_files
 from khoj.utils.helpers import is_none_or_empty
 from khoj.utils.rawconfig import FullConfig
 
@@ -241,24 +241,20 @@
 
 
 def initialize_content(regenerate: bool, search_type: Optional[SearchType] = None, init=False, user: KhojUser = None):
     # Initialize Content from Config
     if state.search_models:
         try:
             if init:
-                logger.info("📬 Initializing content index...")
-                state.content_index = load_content(state.config.content_type, state.content_index, state.search_models)
+                logger.info("📬 No-op...")
             else:
                 logger.info("📬 Updating content index...")
                 all_files = collect_files(user=user)
-                state.content_index, status = configure_content(
-                    state.content_index,
-                    state.config.content_type,
+                status = configure_content(
                     all_files,
-                    state.search_models,
                     regenerate,
                     search_type,
                     user=user,
                 )
                 if not status:
                     raise RuntimeError("Failed to update content index")
         except Exception as e:
@@ -268,21 +264,23 @@
 def configure_routes(app):
     # Import APIs here to setup search types before while configuring server
     from khoj.routers.api import api
     from khoj.routers.api_agents import api_agents
     from khoj.routers.api_chat import api_chat
     from khoj.routers.api_config import api_config
     from khoj.routers.indexer import indexer
+    from khoj.routers.notion import notion_router
     from khoj.routers.web_client import web_client
 
     app.include_router(api, prefix="/api")
     app.include_router(api_chat, prefix="/api/chat")
     app.include_router(api_agents, prefix="/api/agents")
     app.include_router(api_config, prefix="/api/config")
     app.include_router(indexer, prefix="/api/v1/index")
+    app.include_router(notion_router, prefix="/api/notion")
     app.include_router(web_client)
 
     if not state.anonymous_mode:
         from khoj.routers.auth import auth_router
 
         app.include_router(auth_router, prefix="/auth")
         logger.info("🔑 Enabled Authentication")
@@ -307,21 +305,17 @@
 
 @schedule.repeat(schedule.every(22).to(26).hours)
 def update_search_index():
     try:
         logger.info("📬 Updating content index via Scheduler")
         for user in get_all_users():
             all_files = collect_files(user=user)
-            state.content_index, success = configure_content(
-                state.content_index, state.config.content_type, all_files, state.search_models, user=user
-            )
+            success = configure_content(all_files, user=user)
         all_files = collect_files(user=None)
-        state.content_index, success = configure_content(
-            state.content_index, state.config.content_type, all_files, state.search_models, user=None
-        )
+        success = configure_content(all_files, user=None)
         if not success:
             raise RuntimeError("Failed to update content index")
         logger.info("📪 Content index updated via Scheduler")
     except Exception as e:
         logger.error(f"🚨 Error updating content index via Scheduler: {e}", exc_info=True)
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/main.py` & `khoj_assistant-1.8.1.dev58/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/manage.py` & `khoj_assistant-1.8.1.dev58/src/khoj/manage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/app/README.md` & `khoj_assistant-1.8.1.dev58/src/khoj/app/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/app/settings.py` & `khoj_assistant-1.8.1.dev58/src/khoj/app/settings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/app/urls.py` & `khoj_assistant-1.8.1.dev58/src/khoj/app/urls.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/admin.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 from khoj.database.models import (
     Agent,
     ChatModelOptions,
     ClientApplication,
     Conversation,
     Entry,
+    GithubConfig,
     KhojUser,
+    NotionConfig,
     OfflineChatProcessorConversationConfig,
     OpenAIProcessorConversationConfig,
     ReflectiveQuestion,
     SearchModelConfig,
     SpeechToTextModelOptions,
     Subscription,
     TextToImageModelConfig,
@@ -48,14 +50,16 @@
 admin.site.register(SearchModelConfig)
 admin.site.register(Subscription)
 admin.site.register(ReflectiveQuestion)
 admin.site.register(UserSearchModelConfig)
 admin.site.register(TextToImageModelConfig)
 admin.site.register(ClientApplication)
 admin.site.register(Agent)
+admin.site.register(GithubConfig)
+admin.site.register(NotionConfig)
 
 
 @admin.register(Entry)
 class EntryAdmin(admin.ModelAdmin):
     list_display = (
         "id",
         "created_at",
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/adapters/__init__.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,18 @@
     return subscription_to_state(user_subscription)
 
 
 async def get_user_by_email(email: str) -> KhojUser:
     return await KhojUser.objects.filter(email=email).afirst()
 
 
+async def aget_user_by_uuid(uuid: str) -> KhojUser:
+    return await KhojUser.objects.filter(uuid=uuid).afirst()
+
+
 async def get_user_by_token(token: dict) -> KhojUser:
     google_user = await GoogleUser.objects.filter(sub=token.get("sub")).select_related("user").afirst()
     if not google_user:
         return None
     return google_user.user
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0001_khojuser.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0001_khojuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0002_googleuser.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0002_googleuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0004_content_types_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0004_content_types_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0006_embeddingsdates.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0006_embeddingsdates.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0007_add_conversation.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0007_add_conversation.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0009_khojapiuser.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0009_khojapiuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0012_entry_file_source.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0012_entry_file_source.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0013_subscription.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0013_subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0015_alter_subscription_user.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0015_alter_subscription_user.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0017_searchmodel.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0017_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0020_reflectivequestion.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0020_reflectivequestion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0022_texttoimagemodelconfig.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0022_texttoimagemodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0023_usersearchmodelconfig.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0023_usersearchmodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0029_userrequests.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0029_userrequests.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0030_conversation_slug_and_title.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0030_conversation_slug_and_title.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0031_agent_conversation_agent.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0031_agent_conversation_agent.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0031_alter_googleuser_locale.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0031_alter_googleuser_locale.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/database/models/__init__.py` & `khoj_assistant-1.8.1.dev58/src/khoj/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/404.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/agent.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/agent.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/agents.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/agents.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/base_config.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/chat.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/config.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/config.html`

 * *Files 1% similar despite different names*

```diff
@@ -105,22 +105,31 @@
                             style="display: {% if not current_model_state.notion %}none{% endif %}">
                     </h3>
                 </div>
                 <div class="card-description-row">
                     <p class="card-description">Sync your Notion pages</p>
                 </div>
                 <div class="card-action-row">
+                    {% if current_model_state.notion %}
                     <a class="card-button" href="/config/content-source/notion">
-                        {% if current_model_state.notion %}
                             Update
-                        {% else %}
+                        <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"></path></svg>
+                    </a>
+                    {% elif notion_oauth_url %}
+                    <a class="card-button" href="{{ notion_oauth_url }}">
+                            Connect
+                        <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"></path></svg>
+                    </a>
+                    {% else %}
+                    <a class="card-button" href="/config/content-source/notion">
                             Setup
-                        {% endif %}
                         <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"></path></svg>
                     </a>
+                    {% endif %}
+
                     <div id="clear-notion"
                         class="card-action-row"
                         style="display: {% if not current_model_state.notion %}none{% endif %}">
                         <button class="card-button" onclick="clearContentType('notion')">
                             Disable
                         </button>
                     </div>
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_computer_input.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_computer_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_github_input.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/content_source_notion_input.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/content_source_notion_input.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 {% extends "base_config.html" %}
 {% block content %}
 <div class="page">
     <div class="section">
         <h2 class="section-title">
             <img class="card-icon" src="/static/assets/icons/notion.svg?v={{ khoj_version }}" alt="Notion">
             <span class="card-title-text">Notion</span>
-            <div class="instructions">
-                <a href="https://docs.khoj.dev/#/notion_integration">ⓘ Help</a>
-            </div>
-        </h2>
-        <form>
             <table>
                 <tr>
                     <td>
                         <label for="token">Token</label>
                     </td>
                     <td>
                         <input type="text" id="token" name="pat" value="{{ current_config['token'] }}">
                     </td>
                 </tr>
             </table>
             <div class="section">
                 <div id="success" style="display: none;"></div>
-                <button id="submit" type="submit">Save</button>
+                <button id="submit" type="submit">Sync to Update</button>
             </div>
         </form>
     </div>
 </div>
 <script>
     const submit = document.getElementById("submit");
 
@@ -39,15 +34,15 @@
             document.getElementById("success").innerHTML = "❌ Please enter a Notion Token.";
             document.getElementById("success").style.display = "block";
             return;
         }
 
         const submitButton = document.getElementById("submit");
         submitButton.disabled = true;
-        submitButton.innerHTML = "Saving...";
+        submitButton.innerHTML = "Syncing...";
 
         // Save Notion config on server
         const csrfToken = document.cookie.split('; ').find(row => row.startsWith('csrftoken'))?.split('=')[1];
         fetch('/api/config/data/content-source/notion', {
             method: 'POST',
             headers: {
                 'Content-Type': 'application/json',
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/khoj.webmanifest` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/khoj.webmanifest`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/login.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/login.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/search.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/search.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/utils.html` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/utils.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/utils.js` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/utils.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/computer.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/computer.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/copy_button.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/copy_button.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/credit-card.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/credit-card.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon-256x256.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/key.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/key.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/microphone-solid.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/microphone-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/openai-logomark.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/openai-logomark.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/plaintext.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/plaintext.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/stop-solid.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/stop-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/user-silhouette.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/user-silhouette.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/web.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/web.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/icons/whatsapp.svg` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev58/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_default_model.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_default_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_default_model_2.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_default_model_2.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_chat_schema.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_chat_schema.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_offline_model.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_offline_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_processor_config_openai.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_processor_config_openai.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_server_pg.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_server_pg.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/migrations/migrate_version.py` & `khoj_assistant-1.8.1.dev58/src/khoj/migrations/migrate_version.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/embeddings.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/embeddings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/text_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/text_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/github/github_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/github/github_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/markdown/markdown_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/markdown/markdown_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/notion/notion_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/notion/notion_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/org_mode/org_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/org_mode/org_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/org_mode/orgnode.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/pdf/pdf_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/pdf/pdf_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/content/plaintext/plaintext_to_entries.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/content/plaintext/plaintext_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/utils.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/chat_model.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/offline/utils.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/offline/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/gpt.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/conversation/openai/utils.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/conversation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/processor/tools/online_search.py` & `khoj_assistant-1.8.1.dev58/src/khoj/processor/tools/online_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/api.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     CommonQueryParams,
     ConversationCommandRateLimiter,
     update_telemetry_state,
 )
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
-from khoj.search_type import image_search, text_search
+from khoj.search_type import text_search
 from khoj.utils import constants, state
 from khoj.utils.config import OfflineChatProcessorModel
 from khoj.utils.helpers import ConversationCommand, timer
 from khoj.utils.rawconfig import LocationData, SearchResponse
 from khoj.utils.state import SearchType
 
 # Initialize Router
@@ -141,49 +141,25 @@
                     user_query,
                     t,
                     question_embedding=encoded_asymmetric_query,
                     max_distance=max_distance,
                 )
             ]
 
-        elif (t == SearchType.Image) and state.content_index.image and state.search_models.image_search:
-            # query images
-            search_futures += [
-                executor.submit(
-                    image_search.query,
-                    user_query,
-                    results_count,
-                    state.search_models.image_search,
-                    state.content_index.image,
-                )
-            ]
-
         # Query across each requested content types in parallel
         with timer("Query took", logger):
             for search_future in concurrent.futures.as_completed(search_futures):
-                if t == SearchType.Image and state.content_index.image:
-                    hits = await search_future.result()
-                    output_directory = constants.web_directory / "images"
-                    # Collate results
-                    results += image_search.collate_results(
-                        hits,
-                        image_names=state.content_index.image.image_names,
-                        output_directory=output_directory,
-                        image_files_url="/static/images",
-                        count=results_count,
-                    )
-                else:
-                    hits = await search_future.result()
-                    # Collate results
-                    results += text_search.collate_results(hits, dedupe=dedupe)
-
-                    # Sort results across all content types and take top results
-                    results = text_search.rerank_and_sort_results(
-                        results, query=defiltered_query, rank_results=r, search_model_name=search_model.name
-                    )[:results_count]
+                hits = await search_future.result()
+                # Collate results
+                results += text_search.collate_results(hits, dedupe=dedupe)
+
+                # Sort results across all content types and take top results
+                results = text_search.rerank_and_sort_results(
+                    results, query=defiltered_query, rank_results=r, search_model_name=search_model.name
+                )[:results_count]
 
     # Cache results
     if user:
         state.query_cache[user.uuid][query_cache_key] = results
 
     end_time = time.time()
     logger.debug(f"🔍 Search took: {end_time - start_time:.3f} seconds")
@@ -210,16 +186,14 @@
         error_msg = f"🚨 Failed to update server via API: {e}"
         logger.error(error_msg, exc_info=True)
         raise HTTPException(status_code=500, detail=error_msg)
     else:
         components = []
         if state.search_models:
             components.append("Search models")
-        if state.content_index:
-            components.append("Content index")
         components_msg = ", ".join(components)
         logger.info(f"📪 {components_msg} updated via API")
 
     update_telemetry_state(
         request=request,
         telemetry_type="api",
         api="update",
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/api_agents.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/api_agents.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/api_chat.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/api_chat.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/api_config.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/api_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 api_config = APIRouter()
 logger = logging.getLogger(__name__)
 
 
 def map_config_to_object(content_source: str):
     if content_source == DbEntry.EntrySource.GITHUB:
         return GithubConfig
-    if content_source == DbEntry.EntrySource.GITHUB:
+    if content_source == DbEntry.EntrySource.NOTION:
         return NotionConfig
     if content_source == DbEntry.EntrySource.COMPUTER:
         return "Computer"
 
 
 async def map_config_to_db(config: FullConfig, user: KhojUser):
     if config.content_type:
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/api_phone.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/api_phone.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/auth.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/auth.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/helpers.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/indexer.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/indexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from khoj.processor.content.github.github_to_entries import GithubToEntries
 from khoj.processor.content.markdown.markdown_to_entries import MarkdownToEntries
 from khoj.processor.content.notion.notion_to_entries import NotionToEntries
 from khoj.processor.content.org_mode.org_to_entries import OrgToEntries
 from khoj.processor.content.pdf.pdf_to_entries import PdfToEntries
 from khoj.processor.content.plaintext.plaintext_to_entries import PlaintextToEntries
 from khoj.routers.helpers import ApiIndexedDataLimiter, update_telemetry_state
-from khoj.search_type import image_search, text_search
+from khoj.search_type import text_search
 from khoj.utils import constants, state
-from khoj.utils.config import ContentIndex, SearchModels
+from khoj.utils.config import SearchModels
 from khoj.utils.helpers import LRU, get_file_type
 from khoj.utils.rawconfig import ContentConfig, FullConfig, SearchConfig
 from khoj.utils.yaml import save_config_to_file_updated_state
 
 logger = logging.getLogger(__name__)
 
 indexer = APIRouter()
@@ -101,21 +101,18 @@
             )
             state.config.content_type = default_content_config
             save_config_to_file_updated_state()
             configure_search(state.search_models, state.config.search_type)
 
         # Extract required fields from config
         loop = asyncio.get_event_loop()
-        state.content_index, success = await loop.run_in_executor(
+        success = await loop.run_in_executor(
             None,
             configure_content,
-            state.content_index,
-            state.config.content_type,
             indexer_input.model_dump(),
-            state.search_models,
             force,
             t,
             False,
             user,
         )
         if not success:
             raise RuntimeError("Failed to update content index")
@@ -155,49 +152,43 @@
 def configure_search(search_models: SearchModels, search_config: Optional[SearchConfig]) -> Optional[SearchModels]:
     # Run Validation Checks
     if search_models is None:
         search_models = SearchModels()
 
     if search_config and search_config.image:
         logger.info("🔍 🌄 Setting up image search model")
-        search_models.image_search = image_search.initialize_model(search_config.image)
 
     return search_models
 
 
 def configure_content(
-    content_index: Optional[ContentIndex],
-    content_config: Optional[ContentConfig],
     files: Optional[dict[str, dict[str, str]]],
-    search_models: SearchModels,
     regenerate: bool = False,
     t: Optional[state.SearchType] = state.SearchType.All,
     full_corpus: bool = True,
     user: KhojUser = None,
-) -> tuple[Optional[ContentIndex], bool]:
-    content_index = ContentIndex()
-
+) -> bool:
     success = True
     if t == None:
         t = state.SearchType.All
 
     if t is not None and t in [type.value for type in state.SearchType]:
         t = state.SearchType(t)
 
     if t is not None and not t.value in [type.value for type in state.SearchType]:
         logger.warning(f"🚨 Invalid search type: {t}")
-        return None, False
+        return False
 
     search_type = t.value if t else None
 
     no_documents = all([not files.get(file_type) for file_type in files])
 
     if files is None:
         logger.warning(f"🚨 No files to process for {search_type} search.")
-        return None, True
+        return True
 
     try:
         # Initialize Org Notes Search
         if (search_type == state.SearchType.All.value or search_type == state.SearchType.Org.value) and files["org"]:
             logger.info("🦄 Setting up search for orgmode notes")
             # Extract Entries, Generate Notes Embeddings
             text_search.setup(
@@ -263,32 +254,14 @@
             )
 
     except Exception as e:
         logger.error(f"🚨 Failed to setup plaintext: {e}", exc_info=True)
         success = False
 
     try:
-        # Initialize Image Search
-        if (
-            (search_type == state.SearchType.All.value or search_type == state.SearchType.Image.value)
-            and content_config
-            and content_config.image
-            and search_models.image_search
-        ):
-            logger.info("🌄 Setting up search for images")
-            # Extract Entries, Generate Image Embeddings
-            content_index.image = image_search.setup(
-                content_config.image, search_models.image_search.image_encoder, regenerate=regenerate
-            )
-
-    except Exception as e:
-        logger.error(f"🚨 Failed to setup images: {e}", exc_info=True)
-        success = False
-
-    try:
         if no_documents:
             github_config = GithubConfig.objects.filter(user=user).prefetch_related("githubrepoconfig").first()
             if (
                 search_type == state.SearchType.All.value or search_type == state.SearchType.Github.value
             ) and github_config is not None:
                 logger.info("🐙 Setting up search for github")
                 # Extract Entries, Generate Github Embeddings
@@ -326,27 +299,8 @@
         logger.error(f"🚨 Failed to setup Notion: {e}", exc_info=True)
         success = False
 
     # Invalidate Query Cache
     if user:
         state.query_cache[user.uuid] = LRU()
 
-    return content_index, success
-
-
-def load_content(
-    content_config: Optional[ContentConfig],
-    content_index: Optional[ContentIndex],
-    search_models: SearchModels,
-):
-    if content_config is None:
-        logger.debug("🚨 No Content configuration available.")
-        return None
-    if content_index is None:
-        content_index = ContentIndex()
-
-    if content_config.image:
-        logger.info("🌄 Loading images")
-        content_index.image = image_search.setup(
-            content_config.image, search_models.image_search.image_encoder, regenerate=False
-        )
-    return content_index
+    return success
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/storage.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/storage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/subscription.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/twilio.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/twilio.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/routers/web_client.py` & `khoj_assistant-1.8.1.dev58/src/khoj/routers/web_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     EntryAdapters,
     get_user_github_config,
     get_user_name,
     get_user_notion_config,
     get_user_subscription_state,
 )
 from khoj.database.models import KhojUser
+from khoj.routers.notion import get_notion_auth_url
 from khoj.routers.twilio import is_twilio_enabled
 from khoj.utils import constants, state
 from khoj.utils.rawconfig import (
     GithubContentConfig,
     GithubRepoConfig,
     NotionContentConfig,
 )
@@ -240,14 +241,16 @@
     search_model_options = adapters.get_or_create_search_models().all()
     all_search_model_options = list()
     for search_model_option in search_model_options:
         all_search_model_options.append({"name": search_model_option.name, "id": search_model_option.id})
 
     current_search_model_option = adapters.get_user_search_model_or_default(user)
 
+    notion_oauth_url = get_notion_auth_url(user)
+
     return templates.TemplateResponse(
         "config.html",
         context={
             "request": request,
             "current_model_state": successfully_configured,
             "anonymous_mode": state.anonymous_mode,
             "username": user.username,
@@ -263,14 +266,15 @@
             "khoj_cloud_subscription_url": os.getenv("KHOJ_CLOUD_SUBSCRIPTION_URL"),
             "is_active": has_required_scope(request, ["premium"]),
             "has_documents": has_documents,
             "is_twilio_enabled": is_twilio_enabled(),
             "phone_number": user.phone_number,
             "is_phone_number_verified": user.verified_phone_number,
             "khoj_version": state.khoj_version,
+            "notion_oauth_url": notion_oauth_url,
         },
     )
 
 
 @web_client.get("/config/content-source/github", response_class=HTMLResponse)
 @requires(["authenticated"], redirect="login_page")
 def github_config_page(request: Request):
@@ -320,15 +324,15 @@
     has_documents = EntryAdapters.user_has_entries(user=user)
     current_notion_config = get_user_notion_config(user)
 
     current_config = NotionContentConfig(
         token=current_notion_config.token if current_notion_config else "",
     )
 
-    current_config = json.loads(current_config.json())
+    current_config = json.loads(current_config.model_dump_json())
 
     return templates.TemplateResponse(
         "content_source_notion_input.html",
         context={
             "request": request,
             "current_config": current_config,
             "username": user.username,
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/search_filter/date_filter.py` & `khoj_assistant-1.8.1.dev58/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/search_filter/file_filter.py` & `khoj_assistant-1.8.1.dev58/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/search_filter/word_filter.py` & `khoj_assistant-1.8.1.dev58/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/search_type/text_search.py` & `khoj_assistant-1.8.1.dev58/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/cli.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/config.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,22 +55,16 @@
 
 @dataclass
 class ImageSearchModel:
     image_encoder: BaseEncoder
 
 
 @dataclass
-class ContentIndex:
-    image: Optional[ImageContent] = None
-
-
-@dataclass
 class SearchModels:
     text_search: Optional[TextSearchModel] = None
-    image_search: Optional[ImageSearchModel] = None
 
 
 @dataclass
 class OfflineChatProcessorConfig:
     loaded_model: Union[Any, None] = None
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/constants.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/fs_syncer.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/fs_syncer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/helpers.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/initialization.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/initialization.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/jsonl.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/models.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/rawconfig.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/state.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 from typing import Dict, List
 
 from openai import OpenAI
 from whisper import Whisper
 
 from khoj.processor.embeddings import CrossEncoderModel, EmbeddingsModel
 from khoj.utils import config as utils_config
-from khoj.utils.config import ContentIndex, OfflineChatProcessorModel, SearchModels
+from khoj.utils.config import OfflineChatProcessorModel, SearchModels
 from khoj.utils.helpers import LRU, get_device
 from khoj.utils.rawconfig import FullConfig
 
 # Application Global State
 config = FullConfig()
 search_models = SearchModels()
 embeddings_model: Dict[str, EmbeddingsModel] = None
 cross_encoder_model: Dict[str, CrossEncoderModel] = None
-content_index = ContentIndex()
 openai_client: OpenAI = None
 offline_chat_processor_config: OfflineChatProcessorModel = None
 whisper_model: Whisper = None
 config_file: Path = None
 verbose: int = 0
 host: str = None
 port: int = None
```

### Comparing `khoj_assistant-1.8.1.dev56/src/khoj/utils/yaml.py` & `khoj_assistant-1.8.1.dev58/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/.gitignore` & `khoj_assistant-1.8.1.dev58/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/LICENSE` & `khoj_assistant-1.8.1.dev58/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/README.md` & `khoj_assistant-1.8.1.dev58/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,47 +6,60 @@
 [![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 ![Discord](https://img.shields.io/discord/1112065956647284756?style=plastic&label=discord)
 
 </div>
 
 <div align="center">
-<b>An AI personal assistant for your digital brain</b>
+<b>The open-source, personal AI for your digital brain</b>
 </div>
 
 <br />
 
 <div align="center">
 
-[📜 Read Docs](https://docs.khoj.dev)
+[🤖 Read Docs](https://docs.khoj.dev)
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-[🌍 Try Khoj Cloud](https://khoj.dev)
+[🏮 Khoj Cloud](https://khoj.dev)
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 [💬 Get Involved](https://discord.gg/BDgyabRM6e)
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+[📚 Read Blog](https://blog.khoj.dev)
 
 </div>
 
-<div align="center">
+<div align="left">
 
 ***
 
-Khoj is an AI application to search and chat with your notes and documents.<br />
-It is open-source, self-hostable and accessible on Desktop, Emacs, Obsidian, Web and Whatsapp.<br />
-It works with pdf, markdown, org-mode, notion files and github repositories.<br />
-It can paint, search the internet and understand speech.<br />
+Khoj is an application that creates always-available, personal AI agents for you to extend your capabilities.
+- You can share your notes and documents to extend your digital brain.
+- Your AI agents have access to the internet, allowing you to incorporate realtime information.
+- Khoj is accessible on Desktop, Emacs, Obsidian, Web and Whatsapp.
+- You can share pdf, markdown, org-mode, notion files and github repositories.
+- You'll get fast, accurate semantic search on top of your docs.
+- Your agents can create deeply personal images and understand your speech.
+- Khoj is open-source, self-hostable. Always.
 
 ***
 
 </div>
 
-| 🔎 Search | 💬 Chat |
-|:---------:|:-------:|
-| Quickly retrieve relevant documents using natural language | Get answers and create content from your existing knowledge base |
-| Does not need internet | Can be configured to work without internet |
-| <img src="https://docs.khoj.dev/img/khoj_search_on_web.png" width="400px"> | <img src="https://docs.khoj.dev/img/khoj_chat_on_web.png" width="400px"> |
+## See it in action
+
+<img src="https://github.com/khoj-ai/khoj/blob/master/documentation/assets/img/using_khoj_for_studying.gif?raw=true" alt="Khoj Demo">
+
+Go to https://app.khoj.dev to see Khoj live.
+
+## Full feature list
+You can see the full feature list [here](https://docs.khoj.dev/category/features).
+
+## Self-Host
+
+To get started with self-hosting Khoj, [read the docs](https://docs.khoj.dev/get-started/setup).
 
 ## Contributors
 Cheers to our awesome contributors! 🎉
 
 <a href="https://github.com/khoj-ai/khoj/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=khoj-ai/khoj" />
 </a>
```

#### html2text {}

```diff
@@ -2,24 +2,27 @@
 [![test](https://github.com/khoj-ai/khoj/actions/workflows/test.yml/badge.svg)]
   (https://github.com/khoj-ai/khoj/actions/workflows/test.yml) [![dockerize]
  (https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)]
     (https://github.com/khoj-ai/khoj/pkgs/container/khoj) [![pypi](https://
     github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://
  pypi.org/project/khoj-assistant/) ![Discord](https://img.shields.io/discord/
                1112065956647284756?style=plastic&label=discord)
-                AAnn AAII ppeerrssoonnaall aassssiissttaanntt ffoorr yyoouurr ddiiggiittaall bbrraaiinn
+              TThhee ooppeenn--ssoouurrccee,, ppeerrssoonnaall AAII ffoorr yyoouurr ddiiggiittaall bbrraaiinn
 
-[ð Read Docs](https://docs.khoj.dev)   â¢   [ð Try Khoj Cloud](https://
-     khoj.dev)   â¢   [ð¬ Get Involved](https://discord.gg/BDgyabRM6e)
-*** Khoj is an AI application to search and chat with your notes and documents.
- It is open-source, self-hostable and accessible on Desktop, Emacs, Obsidian,
-                               Web and Whatsapp.
- It works with pdf, markdown, org-mode, notion files and github repositories.
-           It can paint, search the internet and understand speech.
-                                      ***
-| ð Search | ð¬ Chat | |:---------:|:-------:| | Quickly retrieve relevant
-documents using natural language | Get answers and create content from your
-existing knowledge base | | Does not need internet | Can be configured to work
-without internet | | [https://docs.khoj.dev/img/khoj_search_on_web.png]|
-[https://docs.khoj.dev/img/khoj_chat_on_web.png]| ## Contributors Cheers to our
-awesome contributors! ð _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_k_h_o_j_-_a_i_/_k_h_o_j_]Made
-with [contrib.rocks](https://contrib.rocks).
+  [ð¤ Read Docs](https://docs.khoj.dev)   â¢   [ð® Khoj Cloud](https://
+ khoj.dev)   â¢   [ð¬ Get Involved](https://discord.gg/BDgyabRM6e)   â¢  
+                    [ð Read Blog](https://blog.khoj.dev)
+*** Khoj is an application that creates always-available, personal AI agents
+for you to extend your capabilities. - You can share your notes and documents
+to extend your digital brain. - Your AI agents have access to the internet,
+allowing you to incorporate realtime information. - Khoj is accessible on
+Desktop, Emacs, Obsidian, Web and Whatsapp. - You can share pdf, markdown, org-
+mode, notion files and github repositories. - You'll get fast, accurate
+semantic search on top of your docs. - Your agents can create deeply personal
+images and understand your speech. - Khoj is open-source, self-hostable.
+Always. ***
+## See it in action [Khoj Demo]Go to https://app.khoj.dev to see Khoj live. ##
+Full feature list You can see the full feature list [here](https://
+docs.khoj.dev/category/features). ## Self-Host To get started with self-hosting
+Khoj, [read the docs](https://docs.khoj.dev/get-started/setup). ## Contributors
+Cheers to our awesome contributors! ð _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_k_h_o_j_-_a_i_/_k_h_o_j_]Made with [contrib.rocks](https://contrib.rocks).
```

### Comparing `khoj_assistant-1.8.1.dev56/pyproject.toml` & `khoj_assistant-1.8.1.dev58/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev56/PKG-INFO` & `khoj_assistant-1.8.1.dev58/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: khoj-assistant
-Version: 1.8.1.dev56
+Version: 1.8.1.dev58
 Summary: An AI copilot for your Second Brain
 Project-URL: Homepage, https://khoj.dev
 Project-URL: Documentation, https://docs.khoj.dev
 Project-URL: Code, https://github.com/khoj-ai/khoj
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -88,47 +88,60 @@
 [![dockerize](https://github.com/khoj-ai/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/khoj-ai/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/khoj-ai/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 ![Discord](https://img.shields.io/discord/1112065956647284756?style=plastic&label=discord)
 
 </div>
 
 <div align="center">
-<b>An AI personal assistant for your digital brain</b>
+<b>The open-source, personal AI for your digital brain</b>
 </div>
 
 <br />
 
 <div align="center">
 
-[📜 Read Docs](https://docs.khoj.dev)
+[🤖 Read Docs](https://docs.khoj.dev)
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-[🌍 Try Khoj Cloud](https://khoj.dev)
+[🏮 Khoj Cloud](https://khoj.dev)
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 [💬 Get Involved](https://discord.gg/BDgyabRM6e)
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
+[📚 Read Blog](https://blog.khoj.dev)
 
 </div>
 
-<div align="center">
+<div align="left">
 
 ***
 
-Khoj is an AI application to search and chat with your notes and documents.<br />
-It is open-source, self-hostable and accessible on Desktop, Emacs, Obsidian, Web and Whatsapp.<br />
-It works with pdf, markdown, org-mode, notion files and github repositories.<br />
-It can paint, search the internet and understand speech.<br />
+Khoj is an application that creates always-available, personal AI agents for you to extend your capabilities.
+- You can share your notes and documents to extend your digital brain.
+- Your AI agents have access to the internet, allowing you to incorporate realtime information.
+- Khoj is accessible on Desktop, Emacs, Obsidian, Web and Whatsapp.
+- You can share pdf, markdown, org-mode, notion files and github repositories.
+- You'll get fast, accurate semantic search on top of your docs.
+- Your agents can create deeply personal images and understand your speech.
+- Khoj is open-source, self-hostable. Always.
 
 ***
 
 </div>
 
-| 🔎 Search | 💬 Chat |
-|:---------:|:-------:|
-| Quickly retrieve relevant documents using natural language | Get answers and create content from your existing knowledge base |
-| Does not need internet | Can be configured to work without internet |
-| <img src="https://docs.khoj.dev/img/khoj_search_on_web.png" width="400px"> | <img src="https://docs.khoj.dev/img/khoj_chat_on_web.png" width="400px"> |
+## See it in action
+
+<img src="https://github.com/khoj-ai/khoj/blob/master/documentation/assets/img/using_khoj_for_studying.gif?raw=true" alt="Khoj Demo">
+
+Go to https://app.khoj.dev to see Khoj live.
+
+## Full feature list
+You can see the full feature list [here](https://docs.khoj.dev/category/features).
+
+## Self-Host
+
+To get started with self-hosting Khoj, [read the docs](https://docs.khoj.dev/get-started/setup).
 
 ## Contributors
 Cheers to our awesome contributors! 🎉
 
 <a href="https://github.com/khoj-ai/khoj/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=khoj-ai/khoj" />
 </a>
```

