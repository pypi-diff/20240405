# Comparing `tmp/wagtail_fedit-1.3.2.tar.gz` & `tmp/wagtail_fedit-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.2.tar", last modified: Fri Apr  5 18:01:52 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.3.tar", last modified: Fri Apr  5 19:40:34 2024, max compression
```

## Comparing `wagtail_fedit-1.3.2.tar` & `wagtail_fedit-1.3.3.tar`

### file list

```diff
@@ -1,110 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7538 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 18:01:52.440832 wagtail_fedit-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.333047 wagtail_fedit-1.3.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.363707 wagtail_fedit-1.3.2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.364639 wagtail_fedit-1.3.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.367684 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.302994 wagtail_fedit-1.3.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.304376 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.371779 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.372854 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15212 2024-04-05 13:21:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.305377 wagtail_fedit-1.3.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.308360 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.374840 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.375963 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.381232 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.386714 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
--rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
--rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
--rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.388388 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.389387 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.391473 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.393852 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.397168 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.400008 wagtail_fedit-1.3.2/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.402022 wagtail_fedit-1.3.2/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.408783 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.413606 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.420119 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.423462 wagtail_fedit-1.3.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    12202 2024-04-05 14:30:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.360380 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7538 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3558 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.217662 wagtail_fedit-1.3.3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7538 2024-04-05 19:40:34.218706 wagtail_fedit-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 19:40:34.230249 wagtail_fedit-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.963357 wagtail_fedit-1.3.3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.006288 wagtail_fedit-1.3.3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.007286 wagtail_fedit-1.3.3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.009291 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.930411 wagtail_fedit-1.3.3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.931476 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.032239 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.058338 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.933412 wagtail_fedit-1.3.3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.935411 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.067291 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.078599 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.107511 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1715 2024-04-05 19:12:49.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.112507 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.113766 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.117684 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.119653 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.122659 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.124655 wagtail_fedit-1.3.3/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.130687 wagtail_fedit-1.3.3/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.137163 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.156562 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.175677 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.211370 wagtail_fedit-1.3.3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    13978 2024-04-05 19:25:14.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.216668 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.003285 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7538 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3454 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.2/LICENSE` & `wagtail_fedit-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/PKG-INFO` & `wagtail_fedit-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.2
+Version: 1.3.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.2/README.md` & `wagtail_fedit-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/setup.cfg` & `wagtail_fedit-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.3/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/models.py` & `wagtail_fedit-1.3.3/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -298,16 +298,16 @@
         }
     }
 }
 
 class WagtailFeditPublishMenu {
     constructor(publishButton) {
         this.publishButton = publishButton;
-        this.publishForm = publishButton.parentElement.querySelector("form");
-        const buttons = this.publishForm.querySelectorAll("button");
+        this.publishButtonsWrapper = publishButton.parentElement.querySelector(".wagtail-fedit-form-buttons");
+        const buttons = this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button");
         let initialIsHidden = false;
         for (const button of buttons) {
             if (button.classList.contains("initially-hidden")) {
                 initialIsHidden = true;
                 break;
             }
         }
@@ -323,44 +323,44 @@
         }
 
         this.init();
     }
 
     init() {
         this.publishButton.addEventListener("click", (e) => {
-            if (this.publishForm.classList.contains("open")) {
-                const anim = this.publishForm.animate([{
+            if (this.publishButtonsWrapper.classList.contains("open")) {
+                const anim = this.publishButtonsWrapper.animate([{
                     opacity: 1,
-                    height: `${this.publishForm.scrollHeight}px`
+                    height: `${this.publishButtonsWrapper.scrollHeight}px`
                 }, {
                     opacity: 0,
                     height: "0px"
                 }, ], {
                     duration: 500,
                     easing: "ease-in-out",
                 });
                 anim.onfinish = () => {
-                    this.publishForm.classList.remove("open");
+                    this.publishButtonsWrapper.classList.remove("open");
                 };
                 return;
             }
             e.preventDefault();
             e.stopPropagation();
-            const anim = this.publishForm.animate([{
+            const anim = this.publishButtonsWrapper.animate([{
                 opacity: 0,
                 height: "0px"
             }, {
                 opacity: 1,
-                height: `${this.publishForm.scrollHeight}px`
+                height: `${this.publishButtonsWrapper.scrollHeight}px`
             }], {
                 duration: 500,
                 easing: "ease-in-out",
             });
             anim.onfinish = () => {
-                this.publishForm.classList.add("open");
+                this.publishButtonsWrapper.classList.add("open");
             };
         });
     }
 }
 
 function initFEditors() {
     const wagtailFeditBlockEditors = document.querySelectorAll(".wagtail-fedit-block-wrapper");
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 00000000: 7b25 206c 6f61 6420 7761 6774 6169 6c61  {% load wagtaila
 00000010: 646d 696e 5f74 6167 7320 6931 386e 2025  dmin_tags i18n %
-00000020: 7d0d 0a3c 6275 7474 6f6e 2074 7970 653d  }..<button type=
-00000030: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
-00000040: 6275 7474 6f6e 2062 7574 746f 6e2d 7365  button button-se
-00000050: 636f 6e64 6172 7920 6275 7474 6f6e 2d6c  condary button-l
-00000060: 6172 6765 2062 6963 6f6c 6f72 2062 7574  arge bicolor but
-00000070: 746f 6e2d 2d69 636f 6e22 206e 616d 653d  ton--icon" name=
-00000080: 2261 6374 696f 6e2d 7375 626d 6974 2220  "action-submit" 
-00000090: 7661 6c75 653d 2231 223e 0d0a 2020 2020  value="1">..    
-000000a0: 3c73 7061 6e20 636c 6173 733d 2269 636f  <span class="ico
-000000b0: 6e2d 7772 6170 7065 7222 3e0d 0a20 2020  n-wrapper">..   
-000000c0: 2020 2020 203c 7376 6720 786d 6c6e 733d       <svg xmlns=
-000000d0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000000e0: 7267 2f32 3030 302f 7376 6722 2066 696c  rg/2000/svg" fil
-000000f0: 6c3d 2263 7572 7265 6e74 436f 6c6f 7222  l="currentColor"
-00000100: 2063 6c61 7373 3d22 6963 6f6e 2220 7669   class="icon" vi
-00000110: 6577 426f 783d 2230 2030 2031 3620 3136  ewBox="0 0 16 16
-00000120: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
-00000130: 3c21 2d2d 2054 6865 204d 4954 204c 6963  <!-- The MIT Lic
-00000140: 656e 7365 2028 4d49 5429 202d 2d3e 0d0a  ense (MIT) -->..
-00000150: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-00000160: 2043 6f70 7972 6967 6874 2028 6329 2032   Copyright (c) 2
-00000170: 3031 312d 3230 3234 2054 6865 2042 6f6f  011-2024 The Boo
-00000180: 7473 7472 6170 2041 7574 686f 7273 202d  tstrap Authors -
-00000190: 2d3e 0d0a 2020 2020 2020 2020 2020 2020  ->..            
-000001a0: 3c70 6174 6820 643d 224d 3134 2e35 2033  <path d="M14.5 3
-000001b0: 612e 352e 3520 3020 3020 3120 2e35 2e35  a.5.5 0 0 1 .5.5
-000001c0: 7639 612e 352e 3520 3020 3020 312d 2e35  v9a.5.5 0 0 1-.5
-000001d0: 2e35 682d 3133 612e 352e 3520 3020 3020  .5h-13a.5.5 0 0 
-000001e0: 312d 2e35 2d2e 3576 2d39 612e 352e 3520  1-.5-.5v-9a.5.5 
-000001f0: 3020 3020 3120 2e35 2d2e 357a 6d2d 3133  0 0 1 .5-.5zm-13
-00000200: 2d31 4131 2e35 2031 2e35 2030 2030 2030  -1A1.5 1.5 0 0 0
-00000210: 2030 2033 2e35 7639 4131 2e35 2031 2e35   0 3.5v9A1.5 1.5
-00000220: 2030 2030 2030 2031 2e35 2031 3468 3133   0 0 0 1.5 14h13
-00000230: 6131 2e35 2031 2e35 2030 2030 2030 2031  a1.5 1.5 0 0 0 1
-00000240: 2e35 2d31 2e35 762d 3941 312e 3520 312e  .5-1.5v-9A1.5 1.
-00000250: 3520 3020 3020 3020 3134 2e35 2032 7a22  5 0 0 0 14.5 2z"
-00000260: 2f3e 0d0a 2020 2020 2020 2020 2020 2020  />..            
-00000270: 3c70 6174 6820 643d 224d 3720 352e 3561  <path d="M7 5.5a
-00000280: 2e35 2e35 2030 2030 2031 202e 352d 2e35  .5.5 0 0 1 .5-.5
-00000290: 6835 612e 352e 3520 3020 3020 3120 3020  h5a.5.5 0 0 1 0 
-000002a0: 3168 2d35 612e 352e 3520 3020 3020 312d  1h-5a.5.5 0 0 1-
-000002b0: 2e35 2d2e 356d 2d31 2e34 3936 2d2e 3835  .5-.5m-1.496-.85
-000002c0: 3461 2e35 2e35 2030 2030 2031 2030 202e  4a.5.5 0 0 1 0 .
-000002d0: 3730 386c 2d31 2e35 2031 2e35 612e 352e  708l-1.5 1.5a.5.
-000002e0: 3520 3020 3020 312d 2e37 3038 2030 6c2d  5 0 0 1-.708 0l-
-000002f0: 2e35 2d2e 3561 2e35 2e35 2030 2031 2031  .5-.5a.5.5 0 1 1
-00000300: 202e 3730 382d 2e37 3038 6c2e 3134 362e   .708-.708l.146.
-00000310: 3134 3720 312e 3134 362d 312e 3134 3761  147 1.146-1.147a
-00000320: 2e35 2e35 2030 2030 2031 202e 3730 3820  .5.5 0 0 1 .708 
-00000330: 304d 3720 392e 3561 2e35 2e35 2030 2030  0M7 9.5a.5.5 0 0
-00000340: 2031 202e 352d 2e35 6835 612e 352e 3520   1 .5-.5h5a.5.5 
-00000350: 3020 3020 3120 3020 3168 2d35 612e 352e  0 0 1 0 1h-5a.5.
-00000360: 3520 3020 3020 312d 2e35 2d2e 356d 2d31  5 0 0 1-.5-.5m-1
-00000370: 2e34 3936 2d2e 3835 3461 2e35 2e35 2030  .496-.854a.5.5 0
-00000380: 2030 2031 2030 202e 3730 386c 2d31 2e35   0 1 0 .708l-1.5
-00000390: 2031 2e35 612e 352e 3520 3020 3020 312d   1.5a.5.5 0 0 1-
-000003a0: 2e37 3038 2030 6c2d 2e35 2d2e 3561 2e35  .708 0l-.5-.5a.5
-000003b0: 2e35 2030 2030 2031 202e 3730 382d 2e37  .5 0 0 1 .708-.7
-000003c0: 3038 6c2e 3134 362e 3134 3720 312e 3134  08l.146.147 1.14
-000003d0: 362d 312e 3134 3761 2e35 2e35 2030 2030  6-1.147a.5.5 0 0
-000003e0: 2031 202e 3730 3820 3022 2f3e 0d0a 2020   1 .708 0"/>..  
-000003f0: 2020 2020 2020 3c2f 7376 673e 0d0a 2020        </svg>..  
-00000400: 2020 3c2f 7370 616e 3e0d 0a20 2020 207b    </span>..    {
-00000410: 2520 7472 616e 736c 6174 6520 2253 7562  % translate "Sub
-00000420: 6d69 7420 666f 7220 4d6f 6465 7261 7469  mit for Moderati
-00000430: 6f6e 2220 257d 0d0a 3c2f 6275 7474 6f6e  on" %}..</button
-00000440: 3e                                       >
+00000020: 7d0d 0a3c 6120 6872 6566 3d22 7b7b 6163  }..<a href="{{ac
+00000030: 7469 6f6e 5f75 726c 7d7d 2220 636c 6173  tion_url}}" clas
+00000040: 733d 2277 6167 7461 696c 2d66 6564 6974  s="wagtail-fedit
+00000050: 2d75 7365 7262 6172 2d62 7574 746f 6e20  -userbar-button 
+00000060: 6275 7474 6f6e 2062 6963 6f6c 6f72 2062  button bicolor b
+00000070: 7574 746f 6e2d 2d69 636f 6e7b 2520 6966  utton--icon{% if
+00000080: 2068 6964 6465 6e20 257d 2069 6e69 7469   hidden %} initi
+00000090: 616c 6c79 2d68 6964 6465 6e7b 2520 656e  ally-hidden{% en
+000000a0: 6469 6620 257d 2220 6e61 6d65 3d22 6163  dif %}" name="ac
+000000b0: 7469 6f6e 2d73 7562 6d69 7422 2076 616c  tion-submit" val
+000000c0: 7565 3d22 3122 3e0d 0a20 2020 203c 7370  ue="1">..    <sp
+000000d0: 616e 2063 6c61 7373 3d22 6963 6f6e 2d77  an class="icon-w
+000000e0: 7261 7070 6572 223e 0d0a 2020 2020 2020  rapper">..      
+000000f0: 2020 3c73 7667 2078 6d6c 6e73 3d22 6874    <svg xmlns="ht
+00000100: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000110: 3230 3030 2f73 7667 2220 6669 6c6c 3d22  2000/svg" fill="
+00000120: 6375 7272 656e 7443 6f6c 6f72 2220 636c  currentColor" cl
+00000130: 6173 733d 2277 2d61 6374 696f 6e2d 6963  ass="w-action-ic
+00000140: 6f6e 2220 7669 6577 426f 783d 2230 2030  on" viewBox="0 0
+00000150: 2031 3620 3136 223e 0d0a 2020 2020 2020   16 16">..      
+00000160: 2020 2020 2020 3c21 2d2d 2054 6865 204d        <!-- The M
+00000170: 4954 204c 6963 656e 7365 2028 4d49 5429  IT License (MIT)
+00000180: 202d 2d3e 0d0a 2020 2020 2020 2020 2020   -->..          
+00000190: 2020 3c21 2d2d 2043 6f70 7972 6967 6874    <!-- Copyright
+000001a0: 2028 6329 2032 3031 312d 3230 3234 2054   (c) 2011-2024 T
+000001b0: 6865 2042 6f6f 7473 7472 6170 2041 7574  he Bootstrap Aut
+000001c0: 686f 7273 202d 2d3e 0d0a 2020 2020 2020  hors -->..      
+000001d0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000001e0: 3134 2e35 2033 612e 352e 3520 3020 3020  14.5 3a.5.5 0 0 
+000001f0: 3120 2e35 2e35 7639 612e 352e 3520 3020  1 .5.5v9a.5.5 0 
+00000200: 3020 312d 2e35 2e35 682d 3133 612e 352e  0 1-.5.5h-13a.5.
+00000210: 3520 3020 3020 312d 2e35 2d2e 3576 2d39  5 0 0 1-.5-.5v-9
+00000220: 612e 352e 3520 3020 3020 3120 2e35 2d2e  a.5.5 0 0 1 .5-.
+00000230: 357a 6d2d 3133 2d31 4131 2e35 2031 2e35  5zm-13-1A1.5 1.5
+00000240: 2030 2030 2030 2030 2033 2e35 7639 4131   0 0 0 0 3.5v9A1
+00000250: 2e35 2031 2e35 2030 2030 2030 2031 2e35  .5 1.5 0 0 0 1.5
+00000260: 2031 3468 3133 6131 2e35 2031 2e35 2030   14h13a1.5 1.5 0
+00000270: 2030 2030 2031 2e35 2d31 2e35 762d 3941   0 0 1.5-1.5v-9A
+00000280: 312e 3520 312e 3520 3020 3020 3020 3134  1.5 1.5 0 0 0 14
+00000290: 2e35 2032 7a22 2f3e 0d0a 2020 2020 2020  .5 2z"/>..      
+000002a0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
+000002b0: 3720 352e 3561 2e35 2e35 2030 2030 2031  7 5.5a.5.5 0 0 1
+000002c0: 202e 352d 2e35 6835 612e 352e 3520 3020   .5-.5h5a.5.5 0 
+000002d0: 3020 3120 3020 3168 2d35 612e 352e 3520  0 1 0 1h-5a.5.5 
+000002e0: 3020 3020 312d 2e35 2d2e 356d 2d31 2e34  0 0 1-.5-.5m-1.4
+000002f0: 3936 2d2e 3835 3461 2e35 2e35 2030 2030  96-.854a.5.5 0 0
+00000300: 2031 2030 202e 3730 386c 2d31 2e35 2031   1 0 .708l-1.5 1
+00000310: 2e35 612e 352e 3520 3020 3020 312d 2e37  .5a.5.5 0 0 1-.7
+00000320: 3038 2030 6c2d 2e35 2d2e 3561 2e35 2e35  08 0l-.5-.5a.5.5
+00000330: 2030 2031 2031 202e 3730 382d 2e37 3038   0 1 1 .708-.708
+00000340: 6c2e 3134 362e 3134 3720 312e 3134 362d  l.146.147 1.146-
+00000350: 312e 3134 3761 2e35 2e35 2030 2030 2031  1.147a.5.5 0 0 1
+00000360: 202e 3730 3820 304d 3720 392e 3561 2e35   .708 0M7 9.5a.5
+00000370: 2e35 2030 2030 2031 202e 352d 2e35 6835  .5 0 0 1 .5-.5h5
+00000380: 612e 352e 3520 3020 3020 3120 3020 3168  a.5.5 0 0 1 0 1h
+00000390: 2d35 612e 352e 3520 3020 3020 312d 2e35  -5a.5.5 0 0 1-.5
+000003a0: 2d2e 356d 2d31 2e34 3936 2d2e 3835 3461  -.5m-1.496-.854a
+000003b0: 2e35 2e35 2030 2030 2031 2030 202e 3730  .5.5 0 0 1 0 .70
+000003c0: 386c 2d31 2e35 2031 2e35 612e 352e 3520  8l-1.5 1.5a.5.5 
+000003d0: 3020 3020 312d 2e37 3038 2030 6c2d 2e35  0 0 1-.708 0l-.5
+000003e0: 2d2e 3561 2e35 2e35 2030 2030 2031 202e  -.5a.5.5 0 0 1 .
+000003f0: 3730 382d 2e37 3038 6c2e 3134 362e 3134  708-.708l.146.14
+00000400: 3720 312e 3134 362d 312e 3134 3761 2e35  7 1.146-1.147a.5
+00000410: 2e35 2030 2030 2031 202e 3730 3820 3022  .5 0 0 1 .708 0"
+00000420: 2f3e 0d0a 2020 2020 2020 2020 3c2f 7376  />..        </sv
+00000430: 673e 0d0a 2020 2020 3c2f 7370 616e 3e0d  g>..    </span>.
+00000440: 0a20 2020 207b 2520 7472 616e 736c 6174  .    {% translat
+00000450: 6520 2253 7562 6d69 7420 666f 7220 4d6f  e "Submit for Mo
+00000460: 6465 7261 7469 6f6e 2220 257d 0d0a 3c2f  deration" %}..</
+00000470: 613e                                     a>
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 00000000: 7b25 206c 6f61 6420 7761 6774 6169 6c61  {% load wagtaila
 00000010: 646d 696e 5f74 6167 7320 6931 386e 2025  dmin_tags i18n %
-00000020: 7d0d 0a3c 6275 7474 6f6e 2074 7970 653d  }..<button type=
-00000030: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
-00000040: 6275 7474 6f6e 2062 7574 746f 6e2d 7365  button button-se
-00000050: 636f 6e64 6172 7920 6275 7474 6f6e 2d6c  condary button-l
-00000060: 6172 6765 2062 6963 6f6c 6f72 2062 7574  arge bicolor but
-00000070: 746f 6e2d 2d69 636f 6e22 206e 616d 653d  ton--icon" name=
-00000080: 2261 6374 696f 6e2d 7075 626c 6973 6822  "action-publish"
-00000090: 2076 616c 7565 3d22 3122 3e0d 0a20 2020   value="1">..   
-000000a0: 203c 7370 616e 2063 6c61 7373 3d22 6963   <span class="ic
-000000b0: 6f6e 2d77 7261 7070 6572 223e 0d0a 2020  on-wrapper">..  
-000000c0: 2020 2020 2020 3c73 7667 2078 6d6c 6e73        <svg xmlns
-000000d0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-000000e0: 6f72 672f 3230 3030 2f73 7667 2220 6669  org/2000/svg" fi
-000000f0: 6c6c 3d22 6375 7272 656e 7443 6f6c 6f72  ll="currentColor
-00000100: 2220 636c 6173 733d 2269 636f 6e22 2076  " class="icon" v
-00000110: 6965 7742 6f78 3d22 3020 3020 3136 2031  iewBox="0 0 16 1
-00000120: 3622 3e0d 0a20 2020 2020 2020 2020 2020  6">..           
-00000130: 203c 212d 2d20 5468 6520 4d49 5420 4c69   <!-- The MIT Li
-00000140: 6365 6e73 6520 284d 4954 2920 2d2d 3e0d  cense (MIT) -->.
-00000150: 0a20 2020 2020 2020 2020 2020 203c 212d  .            <!-
-00000160: 2d20 436f 7079 7269 6768 7420 2863 2920  - Copyright (c) 
-00000170: 3230 3131 2d32 3032 3420 5468 6520 426f  2011-2024 The Bo
-00000180: 6f74 7374 7261 7020 4175 7468 6f72 7320  otstrap Authors 
-00000190: 2d2d 3e0d 0a20 2020 2020 2020 2020 2020  -->..           
-000001a0: 203c 7061 7468 2064 3d22 6d31 302e 3739   <path d="m10.79
-000001b0: 2031 322e 3931 322d 312e 3631 342d 312e   12.912-1.614-1.
-000001c0: 3631 3561 332e 3520 332e 3520 3020 3020  615a3.5 3.5 0 0 
-000001d0: 312d 342e 3437 342d 342e 3437 346c 2d32  1-4.474-4.474l-2
-000001e0: 2e30 362d 322e 3036 432e 3933 3820 362e  .06-2.06C.938 6.
-000001f0: 3237 3820 3020 3820 3020 3873 3320 352e  278 0 8 0 8s3 5.
-00000200: 3520 3820 352e 3561 3720 3720 3020 3020  5 8 5.5a7 7 0 0 
-00000210: 3020 322e 3739 2d2e 3538 384d 352e 3231  0 2.79-.588M5.21
-00000220: 2033 2e30 3838 4137 2037 2030 2030 2031   3.088A7 7 0 0 1
-00000230: 2038 2032 2e35 6335 2030 2038 2035 2e35   8 2.5c5 0 8 5.5
-00000240: 2038 2035 2e35 732d 2e39 3339 2031 2e37   8 5.5s-.939 1.7
-00000250: 3231 2d32 2e36 3431 2033 2e32 3338 6c2d  21-2.641 3.238l-
-00000260: 322e 3036 322d 322e 3036 3261 332e 3520  2.062-2.062a3.5 
-00000270: 332e 3520 3020 3020 302d 342e 3437 342d  3.5 0 0 0-4.474-
-00000280: 342e 3437 347a 222f 3e0d 0a20 2020 2020  4.474z"/>..     
-00000290: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
-000002a0: 4d35 2e35 3235 2037 2e36 3436 6132 2e35  M5.525 7.646a2.5
-000002b0: 2032 2e35 2030 2030 2030 2032 2e38 3239   2.5 0 0 0 2.829
-000002c0: 2032 2e38 3239 7a6d 342e 3935 2e37 3038   2.829zm4.95.708
-000002d0: 2d32 2e38 3239 2d32 2e38 3361 322e 3520  -2.829-2.83a2.5 
-000002e0: 322e 3520 3020 3020 3120 322e 3832 3920  2.5 0 0 1 2.829 
-000002f0: 322e 3832 397a 6d33 2e31 3731 2036 2d31  2.829zm3.171 6-1
-00000300: 322d 3132 202e 3730 382d 2e37 3038 2031  2-12 .708-.708 1
-00000310: 3220 3132 7a22 2f3e 0d0a 2020 2020 2020  2 12z"/>..      
-00000320: 2020 3c2f 7376 673e 0d0a 2020 2020 3c2f    </svg>..    </
-00000330: 7370 616e 3e0d 0a20 2020 207b 2520 7472  span>..    {% tr
-00000340: 616e 736c 6174 6520 2255 6e70 7562 6c69  anslate "Unpubli
-00000350: 7368 2220 257d 0d0a 3c2f 6275 7474 6f6e  sh" %}..</button
-00000360: 3e                                       >
+00000020: 7d0d 0a3c 6120 6872 6566 3d22 7b7b 6163  }..<a href="{{ac
+00000030: 7469 6f6e 5f75 726c 7d7d 2220 636c 6173  tion_url}}" clas
+00000040: 733d 2277 6167 7461 696c 2d66 6564 6974  s="wagtail-fedit
+00000050: 2d75 7365 7262 6172 2d62 7574 746f 6e20  -userbar-button 
+00000060: 6275 7474 6f6e 2062 6963 6f6c 6f72 2062  button bicolor b
+00000070: 7574 746f 6e2d 2d69 636f 6e22 206e 616d  utton--icon" nam
+00000080: 653d 2261 6374 696f 6e2d 756e 7075 626c  e="action-unpubl
+00000090: 6973 6822 2076 616c 7565 3d22 3122 3e0d  ish" value="1">.
+000000a0: 0a20 2020 203c 7370 616e 2063 6c61 7373  .    <span class
+000000b0: 3d22 6963 6f6e 2d77 7261 7070 6572 223e  ="icon-wrapper">
+000000c0: 0d0a 2020 2020 2020 2020 3c73 7667 2078  ..        <svg x
+000000d0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+000000e0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
+000000f0: 2220 6669 6c6c 3d22 6375 7272 656e 7443  " fill="currentC
+00000100: 6f6c 6f72 2220 636c 6173 733d 2277 2d61  olor" class="w-a
+00000110: 6374 696f 6e2d 6963 6f6e 2220 7669 6577  ction-icon" view
+00000120: 426f 783d 2230 2030 2031 3620 3136 223e  Box="0 0 16 16">
+00000130: 0d0a 2020 2020 2020 2020 2020 2020 3c21  ..            <!
+00000140: 2d2d 2054 6865 204d 4954 204c 6963 656e  -- The MIT Licen
+00000150: 7365 2028 4d49 5429 202d 2d3e 0d0a 2020  se (MIT) -->..  
+00000160: 2020 2020 2020 2020 2020 3c21 2d2d 2043            <!-- C
+00000170: 6f70 7972 6967 6874 2028 6329 2032 3031  opyright (c) 201
+00000180: 312d 3230 3234 2054 6865 2042 6f6f 7473  1-2024 The Boots
+00000190: 7472 6170 2041 7574 686f 7273 202d 2d3e  trap Authors -->
+000001a0: 0d0a 2020 2020 2020 2020 2020 2020 3c70  ..            <p
+000001b0: 6174 6820 643d 226d 3130 2e37 3920 3132  ath d="m10.79 12
+000001c0: 2e39 3132 2d31 2e36 3134 2d31 2e36 3135  .912-1.614-1.615
+000001d0: 6133 2e35 2033 2e35 2030 2030 2031 2d34  a3.5 3.5 0 0 1-4
+000001e0: 2e34 3734 2d34 2e34 3734 6c2d 322e 3036  .474-4.474l-2.06
+000001f0: 2d32 2e30 3643 2e39 3338 2036 2e32 3738  -2.06C.938 6.278
+00000200: 2030 2038 2030 2038 7333 2035 2e35 2038   0 8 0 8s3 5.5 8
+00000210: 2035 2e35 6137 2037 2030 2030 2030 2032   5.5a7 7 0 0 0 2
+00000220: 2e37 392d 2e35 3838 4d35 2e32 3120 332e  .79-.588M5.21 3.
+00000230: 3038 3841 3720 3720 3020 3020 3120 3820  088A7 7 0 0 1 8 
+00000240: 322e 3563 3520 3020 3820 352e 3520 3820  2.5c5 0 8 5.5 8 
+00000250: 352e 3573 2d2e 3933 3920 312e 3732 312d  5.5s-.939 1.721-
+00000260: 322e 3634 3120 332e 3233 386c 2d32 2e30  2.641 3.238l-2.0
+00000270: 3632 2d32 2e30 3632 6133 2e35 2033 2e35  62-2.062a3.5 3.5
+00000280: 2030 2030 2030 2d34 2e34 3734 2d34 2e34   0 0 0-4.474-4.4
+00000290: 3734 7a22 2f3e 0d0a 2020 2020 2020 2020  74z"/>..        
+000002a0: 2020 2020 3c70 6174 6820 643d 224d 352e      <path d="M5.
+000002b0: 3532 3520 372e 3634 3661 322e 3520 322e  525 7.646a2.5 2.
+000002c0: 3520 3020 3020 3020 322e 3832 3920 322e  5 0 0 0 2.829 2.
+000002d0: 3832 397a 6d34 2e39 352e 3730 382d 322e  829zm4.95.708-2.
+000002e0: 3832 392d 322e 3833 6132 2e35 2032 2e35  829-2.83a2.5 2.5
+000002f0: 2030 2030 2031 2032 2e38 3239 2032 2e38   0 0 1 2.829 2.8
+00000300: 3239 7a6d 332e 3137 3120 362d 3132 2d31  29zm3.171 6-12-1
+00000310: 3220 2e37 3038 2d2e 3730 3820 3132 2031  2 .708-.708 12 1
+00000320: 327a 222f 3e0d 0a20 2020 2020 2020 203c  2z"/>..        <
+00000330: 2f73 7667 3e0d 0a20 2020 203c 2f73 7061  /svg>..    </spa
+00000340: 6e3e 0d0a 2020 2020 7b25 2074 7261 6e73  n>..    {% trans
+00000350: 6c61 7465 2022 556e 7075 626c 6973 6822  late "Unpublish"
+00000360: 2025 7d0d 0a3c 2f61 3e                    %}..</a>
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 00000000: 7b25 206c 6f61 6420 7761 6774 6169 6c61  {% load wagtaila
 00000010: 646d 696e 5f74 6167 7320 6931 386e 2025  dmin_tags i18n %
-00000020: 7d0d 0a3c 6275 7474 6f6e 2074 7970 653d  }..<button type=
-00000030: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
-00000040: 7761 6774 6169 6c2d 6665 6469 742d 7573  wagtail-fedit-us
-00000050: 6572 6261 722d 6275 7474 6f6e 2062 7574  erbar-button but
-00000060: 746f 6e20 6269 636f 6c6f 7220 6275 7474  ton bicolor butt
-00000070: 6f6e 2d2d 6963 6f6e 7b25 2069 6620 6869  on--icon{% if hi
-00000080: 6464 656e 2025 7d20 696e 6974 6961 6c6c  dden %} initiall
-00000090: 792d 6869 6464 656e 7b25 2065 6e64 6966  y-hidden{% endif
-000000a0: 2025 7d22 206e 616d 653d 2261 6374 696f   %}" name="actio
-000000b0: 6e2d 7075 626c 6973 6822 2076 616c 7565  n-publish" value
-000000c0: 3d22 3122 3e0d 0a20 2020 203c 7370 616e  ="1">..    <span
-000000d0: 2063 6c61 7373 3d22 6963 6f6e 2d77 7261   class="icon-wra
-000000e0: 7070 6572 223e 0d0a 2020 2020 2020 2020  pper">..        
-000000f0: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
-00000100: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000110: 3030 2f73 7667 2220 6669 6c6c 3d22 6375  00/svg" fill="cu
-00000120: 7272 656e 7443 6f6c 6f72 2220 636c 6173  rrentColor" clas
-00000130: 733d 2277 2d61 6374 696f 6e2d 6963 6f6e  s="w-action-icon
-00000140: 2220 7669 6577 426f 783d 2230 2030 2031  " viewBox="0 0 1
-00000150: 3620 3136 223e 0d0a 2020 2020 2020 2020  6 16">..        
-00000160: 2020 2020 3c21 2d2d 2054 6865 204d 4954      <!-- The MIT
-00000170: 204c 6963 656e 7365 2028 4d49 5429 202d   License (MIT) -
-00000180: 2d3e 0d0a 2020 2020 2020 2020 2020 2020  ->..            
-00000190: 3c21 2d2d 2043 6f70 7972 6967 6874 2028  <!-- Copyright (
-000001a0: 6329 2032 3031 312d 3230 3234 2054 6865  c) 2011-2024 The
-000001b0: 2042 6f6f 7473 7472 6170 2041 7574 686f   Bootstrap Autho
-000001c0: 7273 202d 2d3e 0d0a 2020 2020 2020 2020  rs -->..        
-000001d0: 2020 2020 3c70 6174 6820 643d 224d 3130      <path d="M10
-000001e0: 2e35 2038 6132 2e35 2032 2e35 2030 2031  .5 8a2.5 2.5 0 1
-000001f0: 2031 2d35 2030 2032 2e35 2032 2e35 2030   1-5 0 2.5 2.5 0
-00000200: 2030 2031 2035 2030 222f 3e0d 0a20 2020   0 1 5 0"/>..   
-00000210: 2020 2020 2020 2020 203c 7061 7468 2064           <path d
-00000220: 3d22 4d30 2038 7333 2d35 2e35 2038 2d35  ="M0 8s3-5.5 8-5
-00000230: 2e35 5331 3620 3820 3136 2038 732d 3320  .5S16 8 16 8s-3 
-00000240: 352e 352d 3820 352e 3553 3020 3820 3020  5.5-8 5.5S0 8 0 
-00000250: 386d 3820 332e 3561 332e 3520 332e 3520  8m8 3.5a3.5 3.5 
-00000260: 3020 3120 3020 302d 3720 332e 3520 332e  0 1 0 0-7 3.5 3.
-00000270: 3520 3020 3020 3020 3020 3722 2f3e 0d0a  5 0 0 0 0 7"/>..
-00000280: 2020 2020 2020 2020 3c2f 7376 673e 0d0a          </svg>..
-00000290: 2020 2020 3c2f 7370 616e 3e0d 0a20 2020      </span>..   
-000002a0: 207b 2520 7472 616e 736c 6174 6520 2250   {% translate "P
-000002b0: 7562 6c69 7368 2220 257d 0d0a 3c2f 6275  ublish" %}..</bu
-000002c0: 7474 6f6e 3e                             tton>
+00000020: 7d0d 0a3c 6120 6872 6566 3d22 7b7b 6163  }..<a href="{{ac
+00000030: 7469 6f6e 5f75 726c 7d7d 2220 636c 6173  tion_url}}" clas
+00000040: 733d 2277 6167 7461 696c 2d66 6564 6974  s="wagtail-fedit
+00000050: 2d75 7365 7262 6172 2d62 7574 746f 6e20  -userbar-button 
+00000060: 6275 7474 6f6e 2062 6963 6f6c 6f72 2062  button bicolor b
+00000070: 7574 746f 6e2d 2d69 636f 6e7b 2520 6966  utton--icon{% if
+00000080: 2068 6964 6465 6e20 257d 2069 6e69 7469   hidden %} initi
+00000090: 616c 6c79 2d68 6964 6465 6e7b 2520 656e  ally-hidden{% en
+000000a0: 6469 6620 257d 2220 6e61 6d65 3d22 6163  dif %}" name="ac
+000000b0: 7469 6f6e 2d70 7562 6c69 7368 2220 7661  tion-publish" va
+000000c0: 6c75 653d 2231 223e 0d0a 2020 2020 3c73  lue="1">..    <s
+000000d0: 7061 6e20 636c 6173 733d 2269 636f 6e2d  pan class="icon-
+000000e0: 7772 6170 7065 7222 3e0d 0a20 2020 2020  wrapper">..     
+000000f0: 2020 203c 7376 6720 786d 6c6e 733d 2268     <svg xmlns="h
+00000100: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00000110: 2f32 3030 302f 7376 6722 2066 696c 6c3d  /2000/svg" fill=
+00000120: 2263 7572 7265 6e74 436f 6c6f 7222 2063  "currentColor" c
+00000130: 6c61 7373 3d22 772d 6163 7469 6f6e 2d69  lass="w-action-i
+00000140: 636f 6e22 2076 6965 7742 6f78 3d22 3020  con" viewBox="0 
+00000150: 3020 3136 2031 3622 3e0d 0a20 2020 2020  0 16 16">..     
+00000160: 2020 2020 2020 203c 212d 2d20 5468 6520         <!-- The 
+00000170: 4d49 5420 4c69 6365 6e73 6520 284d 4954  MIT License (MIT
+00000180: 2920 2d2d 3e0d 0a20 2020 2020 2020 2020  ) -->..         
+00000190: 2020 203c 212d 2d20 436f 7079 7269 6768     <!-- Copyrigh
+000001a0: 7420 2863 2920 3230 3131 2d32 3032 3420  t (c) 2011-2024 
+000001b0: 5468 6520 426f 6f74 7374 7261 7020 4175  The Bootstrap Au
+000001c0: 7468 6f72 7320 2d2d 3e0d 0a20 2020 2020  thors -->..     
+000001d0: 2020 2020 2020 203c 7061 7468 2064 3d22         <path d="
+000001e0: 4d31 302e 3520 3861 322e 3520 322e 3520  M10.5 8a2.5 2.5 
+000001f0: 3020 3120 312d 3520 3020 322e 3520 322e  0 1 1-5 0 2.5 2.
+00000200: 3520 3020 3020 3120 3520 3022 2f3e 0d0a  5 0 0 1 5 0"/>..
+00000210: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+00000220: 6820 643d 224d 3020 3873 332d 352e 3520  h d="M0 8s3-5.5 
+00000230: 382d 352e 3553 3136 2038 2031 3620 3873  8-5.5S16 8 16 8s
+00000240: 2d33 2035 2e35 2d38 2035 2e35 5330 2038  -3 5.5-8 5.5S0 8
+00000250: 2030 2038 6d38 2033 2e35 6133 2e35 2033   0 8m8 3.5a3.5 3
+00000260: 2e35 2030 2031 2030 2030 2d37 2033 2e35  .5 0 1 0 0-7 3.5
+00000270: 2033 2e35 2030 2030 2030 2030 2037 222f   3.5 0 0 0 0 7"/
+00000280: 3e0d 0a20 2020 2020 2020 203c 2f73 7667  >..        </svg
+00000290: 3e0d 0a20 2020 203c 2f73 7061 6e3e 0d0a  >..    </span>..
+000002a0: 2020 2020 7b25 2074 7261 6e73 6c61 7465      {% translate
+000002b0: 2022 5075 626c 6973 6822 2025 7d0d 0a3c   "Publish" %}..<
+000002c0: 2f61 3e                                  /a>
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,15 @@
                 <!-- The MIT License (MIT) -->
                 <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
                 <path d="M11 2H9v3h2z"/>
                 <path d="M1.5 0h11.586a1.5 1.5 0 0 1 1.06.44l1.415 1.414A1.5 1.5 0 0 1 16 2.914V14.5a1.5 1.5 0 0 1-1.5 1.5h-13A1.5 1.5 0 0 1 0 14.5v-13A1.5 1.5 0 0 1 1.5 0M1 1.5v13a.5.5 0 0 0 .5.5H2v-4.5A1.5 1.5 0 0 1 3.5 9h9a1.5 1.5 0 0 1 1.5 1.5V15h.5a.5.5 0 0 0 .5-.5V2.914a.5.5 0 0 0-.146-.353l-1.415-1.415A.5.5 0 0 0 13.086 1H13v4.5A1.5 1.5 0 0 1 11.5 7h-7A1.5 1.5 0 0 1 3 5.5V1H1.5a.5.5 0 0 0-.5.5m3 4a.5.5 0 0 0 .5.5h7a.5.5 0 0 0 .5-.5V1H4zM3 15h10v-4.5a.5.5 0 0 0-.5-.5h-9a.5.5 0 0 0-.5.5z"/>
             </svg>
             {% trans "Revision Management" %}
         </button>
-        <form id="wagtail-fedit-form" class="wagtail-fedit-form wagtail-fedit-publish-form" action="{{ publish_url }}" method="post">
-            {% csrf_token %}
-            <div class="wagtail-fedit-form-buttons">
-                {% for button in buttons %}
-                    {{ button }}
-                {% endfor %}
-            </div>
-        </form>
+        <div class="wagtail-fedit-form-buttons">
+            {% for button in buttons %}
+                {{ button }}
+            {% endfor %}
+        </div>
     </div>
 
 {% endblock %}
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.3/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.3/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.3/wagtail_fedit/views/editable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Any, Union, Type
+from typing import Any, Type
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 from django.utils.decorators import method_decorator
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import TemplateView
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.apps import apps
+from django.core.exceptions import PermissionDenied
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
     HttpResponseForbidden,
     HttpResponse,
 )
 from wagtail.admin import messages
@@ -22,122 +23,65 @@
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 from wagtail.models import (
     RevisionMixin,
     PreviewableMixin,
     DraftStateMixin,
     WorkflowMixin,
     WorkflowState,
-    LockableMixin,
     Page,
 )
 from .. import forms as block_forms
 from ..utils import (
     FEDIT_PREVIEW_VAR,
     USERBAR_MODEL_VAR,
     FeditPermissionCheck,
     with_userbar_model,
     user_can_publish,
     user_can_unpublish,
     user_can_submit_for_moderation,
     lock_info,
 )
 
-from ..toolbar import (
-    FeditToolbarComponent,
+from .mixins import (
+    ObjectViewMixin,
+    LockViewMixin,
 )
 
 
-
 def get_unpublish_action(object):
     if isinstance(object, Page):
         return UnpublishPageAction
     return UnpublishAction
 
 
 def get_publish_action(object):
     if isinstance(object, Page):
         return PublishPageRevisionAction
     return PublishRevisionAction
 
 
-class FeditableModelComponent(FeditToolbarComponent):
-    def __init__(self, instance):
-        self.instance = instance
-
-
-class ActionPublishComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/editor/buttons/publish.html"
-    check_for_changes: bool = True
-
-    def get_context_data(self, request):
-        return super().get_context_data(request) | {
-            "hidden": not self.instance.has_unpublished_changes,
-        }
-    
-    def is_shown(self, request):
-        if not super().is_shown(request):
-            return False
-        
-        return user_can_publish(self.instance, request.user, check_for_changes=self.check_for_changes)
-
-class ActionUnpublishComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/editor/buttons/unpublish.html"
-    
-    def is_shown(self, request):
-        if not super().is_shown(request):
-            return False
-        
-        return user_can_unpublish(self.instance, request.user)
-    
-class ActionSubmitComponent(FeditableModelComponent):
-    template_name = "wagtail_fedit/editor/buttons/submit.html"
-    check_for_changes: bool = True
-
-    def get_context_data(self, request):
-        return super().get_context_data(request) | {
-            "hidden": not self.instance.has_unpublished_changes,
-        }
-
-    def is_shown(self, request):
-        if not super().is_shown(request):
-            return False
-        
-        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=self.check_for_changes)
-
-class BaseFeditView(FeditPermissionCheck, TemplateView):
+class BaseFeditView(ObjectViewMixin, FeditPermissionCheck, TemplateView):
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
-        try:
-            self.model = apps.get_model(app_label, model_name)
-            self.model_object = self.model._default_manager.get(pk=object_id)
-        except (LookupError):
-            return HttpResponseBadRequest("Invalid model provided")
-        except (self.model.DoesNotExist):
-            return HttpResponseBadRequest("Model not found")
 
-        if not self.has_perms(request, self.model):
+        if not self.has_perms(request, self.object):
             return HttpResponseForbidden("You do not have permission to view this page")
 
-        if issubclass(self.model, RevisionMixin) and self.model_object.latest_revision_id:
-            instance: RevisionMixin  = self.model_object
+        if issubclass(self.model, RevisionMixin) and self.object.latest_revision_id:
+            instance: RevisionMixin  = self.object
             revision: RevisionMixin = instance.latest_revision
             self.object = revision.as_object()
             self.is_preview = True
         else:
-            self.object = self.model_object
             self.is_preview = False
 
         try:
             self.checks(request, self.object)
         except ValueError as e:
             return HttpResponseForbidden(str(e))
 
-        self.lock, self.locked_for_user = lock_info(
-            self.object, request.user,
-        )
-
         return super().dispatch(request, object_id, app_label, model_name)
     
     def checks(self, request: HttpRequest, object: Any) -> None:
         pass
 
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
         return super().get_context_data(**kwargs) | {
@@ -161,99 +105,152 @@
         object: PreviewableMixin = self.object
         return object.make_preview_request(original_request=self.request, extra_request_attrs={
             FEDIT_PREVIEW_VAR: True,
             USERBAR_MODEL_VAR: self.object,
         })
     
 
-@method_decorator(xframe_options_sameorigin, name="dispatch")
-class FeditablePublishView(WagtailAdminTemplateMixin, BaseFeditView):
-    template_name = "wagtail_fedit/editor/publish_confirm.html"
-    buttons: list[Type[FeditToolbarComponent]] = [
-        ActionPublishComponent,
-        ActionSubmitComponent,
-        ActionUnpublishComponent,
-    ]
-    object: DraftStateMixin
+class BaseActionView(LockViewMixin, BaseFeditView):
+    template_name         = "wagtail_fedit/editor/action_confirm.html"
+    required_superclasses = [DraftStateMixin]
+    action_text            = None
+    title_format           = None
+    action_help_text_title = None
+    action_help_text       = None
 
+    def get_action(self) -> str:
+        return self.action_text
+    
+    def get_action_value(self) -> str:
+        return f"{self.__class__.__name__.lower()}"
 
-    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
-
-        buttons = []
-
-        for button in self.buttons:
-            buttons.append(button(self.object).render(self.request))
+    def get_action_title(self) -> str:
+        return self.title_format.format(self.object)
+    
+    def get_action_help_text_title(self) -> str:
+        return self.action_help_text_title
+    
+    def get_action_help_text(self) -> str:
+        return self.action_help_text
 
-        buttons = list(filter(None, buttons))
+    def redirect_to_success_url(self, request: HttpRequest) -> HttpResponse:
+        if hasattr(self.object, "get_url"):
+            return redirect(self.object.get_url(request))
+        
+        elif hasattr(self.object, "get_absolute_url"):
+            return redirect(self.object.get_absolute_url())
+        
+        return redirect(reverse(
+            "wagtail_fedit:editable",
+            args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
+        ))
+    
+    def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
+        super().setup(request, object_id, app_label, model_name)
+        self.policy = self.object.permissions_for_user(request.user)
+
+        if not isinstance(self.object, tuple(self.required_superclasses)):
+            self.error_response = HttpResponseBadRequest(
+                "Model {} does not inherit from {}".format(
+                    self.model.__name__, ", ".join([cls.__name__ for cls in self.required_superclasses])
+                )
+            )
 
+    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
         return super().get_context_data(**kwargs) | {
-            "buttons": buttons,
-            "object": self.object,
-            "model_verbose_name": self.object._meta.verbose_name,
-            "publish_url": reverse(
-                "wagtail_fedit:publish",
-                args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
-            ),
-            "edit_url": reverse(
+            "action": self.get_action_value(),  # e.g. "publishview"
+            "action_text": self.get_action(),
+            "action_title": self.get_action_title(),
+            "action_help_text_title": self.get_action_help_text_title(),
+            "action_help_text": self.get_action_help_text(),
+            "cancel_url": reverse(
                 "wagtail_fedit:editable",
                 args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
             ),
         }
-    
-    def get_header_title(self):
-        return _("Publishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
 
-    def checks(self, request: HttpRequest, object: Any) -> None:
-        if not isinstance(self.object, DraftStateMixin):
-            raise ValueError("Model {} does not inherit from DraftStateMixin, cannot publish.".format(self.model))
+    def redirect_to_failsafe_url(self, request: HttpRequest) -> HttpResponse:
+        try:
+            finder = AdminURLFinder(request.user)
+            edit_url = finder.get_edit_url(self.object)
+            return redirect(edit_url)
+        except Exception:
+            return redirect(reverse(
+                "wagtail_fedit:editable",
+                args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
+            ))
+        
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        pass
+
+    def action(self, request: HttpRequest) -> HttpResponse:
+        raise NotImplementedError("Subclasses must implement this method")
     
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
-
-        policy = self.object.permissions_for_user(request.user)
-
-        if not isinstance(self.object, DraftStateMixin):
-            raise ValueError("Model {} does not inherit from DraftStateMixin, cannot publish.".format(self.model))
         
         if getattr(settings, "WAGTAIL_WORKFLOW_ENABLED", True) and issubclass(self.model, WorkflowMixin):
             # Retrieve current workflow state if set, default to last workflow state
             self.workflow_state = (
                 self.object.current_workflow_state
                 or self.object.workflow_states.order_by("created_at").last()
             )
         else:
             self.workflow_state = None
 
+        try:
+            self.check_policy(request, self.policy)
+        except ValueError as e:
+            messages.error(request, str(e))
+            return self.get(request, *args, **kwargs)
+
         # Check if lock applies to this user
         if self.locked_for_user:
-            messages.error(request, _("This object is locked. It cannot be published."))
+            messages.error(request, _("This object is locked. It cannot be acted upon."))
             return self.redirect_to_failsafe_url(request)
+        
+        if "action" not in request.POST:
+            messages.error(request, _("No action specified"))
+            return self.get(request, *args, **kwargs)
+        
+        if request.POST["action"] != self.get_action_value():
+            messages.error(request, _("Invalid action specified"))
+            return self.get(request, *args, **kwargs)
+        
+        return self.action(request)
+
+
+class PublishView(BaseActionView):
+    required_superclasses = [DraftStateMixin]
+    action_text = _("Publish")
+
+    def get_action_title(self):
+        return _("Publishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
+
+    def get_action_help_text_title(self):
+        return _("About publishing")
 
-        if request.POST.get("action-publish") == "1"\
-                and policy.can_publish()\
-                and self.object.has_unpublished_changes:
-            return self.publish(request)
-        
-        if request.POST.get("action-unpublish") == "1" and policy.can_unpublish():
-            return self.unpublish(request)
-        
-        if request.POST.get("action-submit") == "1"\
-                and policy.can_submit_for_moderation()\
-                and isinstance(self.object, WorkflowMixin)\
-                and self.object.has_unpublished_changes:
-            return self.submit_for_moderation(request)
-        
-        if request.POST.get("action-cancel") == "1"\
-                and self.workflow_state\
-                and self.workflow_state.user_can_cancel(self.request.user):
-            return self.cancel_workflow(request)
+    def get_action_help_text(self):
+        s = [
+            _("Publishing this object will make it visible to users on the site."),
+            _("That means that any changes you make will be immediately visible to everyone."),
+        ]
+
+        if self.policy.can_unpublish():
+            s.append(_("You can always choose to unpublish it."))
+
+        return s
+
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_publish():
+            raise ValueError("User does not have permission to publish")
         
-        messages.error(request, _("Invalid form submission"))
-        return self.get(request, *args, **kwargs)
-    
-    def publish(self, request: HttpRequest) -> HttpResponse:
+        if not self.object.has_unpublished_changes:
+            raise ValueError("Object has no unpublished changes")
+
+    def action(self, request: HttpRequest) -> HttpResponse:
         latest_revision = None
         if isinstance(self.object, RevisionMixin):
             latest_revision = self.object.latest_revision
 
         action = get_publish_action(self.object)(
             revision=latest_revision,
             user=request.user,
@@ -261,65 +258,105 @@
 
         action.execute()
 
         if latest_revision:
             self.object = latest_revision.as_object()
 
         return self.redirect_to_success_url(request)
-    
-    def unpublish(self, request: HttpRequest) -> HttpResponse:
-        if not self.object.live:
-            messages.error(request, _("This object is not live"))
-            return self.get(request)
-        
-        action = get_unpublish_action(self.object)(
-            self.object,
-            user=request.user,
-        )
 
-        action.execute()
 
-        return self.redirect_to_failsafe_url(request)
+class UnpublishView(BaseActionView):
+    required_superclasses = [DraftStateMixin]
+    action_text = _("Unpublish")
+    action_help_text_title = _("About unpublishing")
+    action_help_text = [
+        _("Unpublishing this object will make it invisible to users on the site."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to publish it again."),
+    ]
+
+    def get_action_title(self):
+        return _("Unpublishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
     
-    def submit_for_moderation(self, request: HttpRequest) -> HttpResponse:
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_unpublish():
+            raise ValueError("User does not have permission to unpublish")
+        
+        if not self.object.live:
+            raise ValueError("Object is not live")
+    
+    def action(self, request: HttpRequest) -> HttpResponse:
         if (
             self.workflow_state
             and self.workflow_state.status == WorkflowState.STATUS_NEEDS_CHANGES
         ):
             # If the workflow was in the needs changes state, resume the existing workflow on submission
             self.workflow_state.resume(self.request.user)
         else:
             # Otherwise start a new workflow
             workflow = self.object.get_workflow()
             workflow.start(self.object, self.request.user)
 
         return self.redirect_to_success_url(request)
 
-    def cancel_workflow(self, request: HttpRequest) -> HttpResponse:
-        if self.workflow_state:
-            self.workflow_state.cancel(user=self.request.user)
-            return self.redirect_to_success_url(request)
+
+class SubmitView(BaseActionView):
+    required_superclasses = [DraftStateMixin, WorkflowMixin]
+    action_text = _("Submit for moderation")
+    action_help_text_title = _("About submitting for moderation")
+    action_help_text = [
+        _("Submitting this object for moderation will make it invisible to users on the site."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to publish it again."),
+    ]
+
+    def get_action_title(self):
+        return _("Submitting {} \"{}\" for moderation").format(self.object._meta.verbose_name, self.object)
+
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_submit_for_moderation():
+            raise ValueError("User does not have permission to submit for moderation")
         
-        return self.get(request)
+        if not self.object.has_unpublished_changes:
+            raise ValueError("Object has no unpublished changes")
 
-    def redirect_to_success_url(self, request: HttpRequest) -> HttpResponse:
-        if hasattr(self.object, "get_url"):
-            return redirect(self.object.get_url(request))
+    def action(self, request: HttpRequest) -> HttpResponse:
+        if not self.object.live:
+            messages.error(request, _("This object is not live"))
+            return self.get(request)
         
-        elif hasattr(self.object, "get_absolute_url"):
-            return redirect(self.object.get_absolute_url())
+        action = get_unpublish_action(self.object)(
+            self.object,
+            user=request.user,
+        )
+
+        action.execute()
+
+        return self.redirect_to_failsafe_url(request)
+
+
+class CancelView(BaseActionView):
+    template_name = "wagtail_fedit/editor/cancel_confirm.html"
+    required_superclasses = [DraftStateMixin, WorkflowMixin]
+    action_text = _("Cancel")
+    action_help_text_title = _("About cancelling")
+    action_help_text = [
+        _("Cancelling this object will make it visible to users on the site."),
+        _("That means that any changes you make will be immediately visible to everyone."),
+    ]
+
+    def get_action_title(self):
+        return _("Cancelling workflow for {} \"{}\"").format(self.object._meta.verbose_name, self.object)
+
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not self.workflow_state:
+            raise ValueError("No workflow state found")
         
-        return redirect(reverse(
-            "wagtail_fedit:editable",
-            args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
-        ))
+        if not self.workflow_state.user_can_cancel(request.user):
+            raise ValueError("User does not have permission to cancel this workflow")
 
-    def redirect_to_failsafe_url(self, request: HttpRequest) -> HttpResponse:
-        try:
-            finder = AdminURLFinder(request.user)
-            edit_url = finder.get_edit_url(self.object)
-            return redirect(edit_url)
-        except Exception:
-            return redirect(reverse(
-                "wagtail_fedit:editable",
-                args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
-            ))
+    def action(self, request: HttpRequest) -> HttpResponse:
+        if self.workflow_state:
+            self.workflow_state.cancel(user=self.request.user)
+            return self.redirect_to_success_url(request)
+        
+        return self.get(request)
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.3/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,47 +4,73 @@
 from django.templatetags.static import static
 from wagtail.admin.userbar import (
     BaseItem,
     AddPageItem,
     ExplorePageItem,
     EditPageItem,
 )
-from wagtail.models import (
-    DraftStateMixin,
-    PreviewableMixin,
-    WorkflowMixin,
-)
 from wagtail import hooks
-from ..views.editable import (
-    ActionPublishComponent,
-    ActionUnpublishComponent,
-    ActionSubmitComponent,
+from ..toolbar import (
+    FeditToolbarComponent,
 )
 from ..utils import (
     is_draft_capable,
     FeditPermissionCheck,
     access_userbar_model,
     FEDIT_PREVIEW_VAR,
     user_can_publish,
     user_can_unpublish,
     user_can_submit_for_moderation,
 )
 
+class FeditableModelComponent(FeditToolbarComponent):
+    def __init__(self, instance):
+        self.instance = instance
+
+    def get_context_data(self, request):
+        return super().get_context_data(request) | {
+            "hidden": not self.instance.has_unpublished_changes,
+            "action_url": reverse(
+                self.action_url,
+                args=[self.instance.pk, self.instance._meta.app_label, self.instance._meta.model_name],
+            ),
+        }
 
-class UserBarActionPublishComponent(ActionPublishComponent):
+class UserBarActionPublishComponent(FeditableModelComponent):
     template_name = "wagtail_fedit/userbar/publish/buttons/publish.html"
+    action_url = "wagtail_fedit:publish"
     check_for_changes = False
     
-class UserBarActionUnpublishComponent(ActionUnpublishComponent):
+    def is_shown(self, request):
+        if not super().is_shown(request):
+            return False
+        
+        return user_can_publish(self.instance, request.user, check_for_changes=self.check_for_changes)
+
+class UserBarActionUnpublishComponent(FeditableModelComponent):
     template_name = "wagtail_fedit/userbar/publish/buttons/unpublish.html"
-    
-class UserBarActionSubmitComponent(ActionSubmitComponent):
+    action_url = "wagtail_fedit:unpublish"
+        
+    def is_shown(self, request):
+        if not super().is_shown(request):
+            return False
+        
+        return user_can_unpublish(self.instance, request.user)
+
+class UserBarActionSubmitComponent(FeditableModelComponent):
     template_name = "wagtail_fedit/userbar/publish/buttons/submit.html"
+    action_url = "wagtail_fedit:submit"
     check_for_changes = False
 
+    def is_shown(self, request):
+        if not super().is_shown(request):
+            return False
+        
+        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=self.check_for_changes)
+
 
 class BaseWagtailFeditItem(BaseItem, FeditPermissionCheck):
     def __init__(self, model):
         self.model = model
 
     def get_context_data(self, request):
         context = super().get_context_data(request)
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.3.2
+Version: 1.3.3
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,20 @@
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
-wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
-wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
 wagtail_fedit/templatetags/__init__.py
@@ -69,13 +67,14 @@
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/blocks.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/fields.py
+wagtail_fedit/views/mixins.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/excluded_relations.py
 wagtail_fedit/wagtail_hooks/log_actions.py
 wagtail_fedit/wagtail_hooks/renderers.py
 wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

