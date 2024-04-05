# Comparing `tmp/wagtail_fedit-1.3.3.tar.gz` & `tmp/wagtail_fedit-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.3.tar", last modified: Fri Apr  5 19:40:34 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.4.tar", last modified: Fri Apr  5 19:47:02 2024, max compression
```

## Comparing `wagtail_fedit-1.3.3.tar` & `wagtail_fedit-1.3.4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.217662 wagtail_fedit-1.3.3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7538 2024-04-05 19:40:34.218706 wagtail_fedit-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 19:40:34.230249 wagtail_fedit-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.963357 wagtail_fedit-1.3.3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.006288 wagtail_fedit-1.3.3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.007286 wagtail_fedit-1.3.3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.009291 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.930411 wagtail_fedit-1.3.3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.931476 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.032239 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.058338 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.933412 wagtail_fedit-1.3.3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:33.935411 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.067291 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.078599 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.107511 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1715 2024-04-05 19:12:49.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.112507 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.113766 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.117684 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.119653 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.122659 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.124655 wagtail_fedit-1.3.3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.130687 wagtail_fedit-1.3.3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.137163 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.156562 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.175677 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.211370 wagtail_fedit-1.3.3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    13978 2024-04-05 19:25:14.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.216668 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:40:34.003285 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7538 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3454 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 19:40:33.000000 wagtail_fedit-1.3.3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.513699 wagtail_fedit-1.3.4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7538 2024-04-05 19:47:02.513756 wagtail_fedit-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 19:47:02.523951 wagtail_fedit-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.345328 wagtail_fedit-1.3.4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.366033 wagtail_fedit-1.3.4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.367262 wagtail_fedit-1.3.4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.368272 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.4/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.322092 wagtail_fedit-1.3.4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.322092 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.374368 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.395823 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.323464 wagtail_fedit-1.3.4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.323464 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.398816 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.403076 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.410734 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.417711 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.418707 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.423670 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.424719 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.426859 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.428119 wagtail_fedit-1.3.4/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.432129 wagtail_fedit-1.3.4/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.436132 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.466637 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.472164 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.506247 wagtail_fedit-1.3.4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14013 2024-04-05 19:46:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.512612 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.363790 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7538 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3454 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.3/LICENSE` & `wagtail_fedit-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/PKG-INFO` & `wagtail_fedit-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.3
+Version: 1.3.4
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.3/README.md` & `wagtail_fedit-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/setup.cfg` & `wagtail_fedit-1.3.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
+00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.4/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.4/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/models.py` & `wagtail_fedit-1.3.4/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                     {% endhelp_block %}
                 {% endpanel %}
 
                 <div class="wagtail-fedit-form-help">
                     <h2>{% translate "Are you sure you want to continue?" %}</h2>
                 </div>
 
-                <input type="hidden" name="action" value="{{ action_value }}" />
+                <input type="hidden" name="action" value="{{ action }}" />
 
                 <div class="wagtail-fedit-form-buttons">
                     <button type="submit" class="button button-primary button-large">
                         {{ action_text }}
                     </button>
                     <a href="{{ cancel_url }}" class="button no button-large">
                         {% translate "Cancel" %}
```

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.4/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.4/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.4/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.4/wagtail_fedit/views/editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             return self.redirect_to_failsafe_url(request)
         
         if "action" not in request.POST:
             messages.error(request, _("No action specified"))
             return self.get(request, *args, **kwargs)
         
         if request.POST["action"] != self.get_action_value():
-            messages.error(request, _("Invalid action specified"))
+            messages.error(request, _("Invalid action specified: {}").format(request.POST["action"]))
             return self.get(request, *args, **kwargs)
         
         return self.action(request)
 
 
 class PublishView(BaseActionView):
     required_superclasses = [DraftStateMixin]
@@ -279,28 +279,28 @@
     
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_unpublish():
             raise ValueError("User does not have permission to unpublish")
         
         if not self.object.live:
             raise ValueError("Object is not live")
-    
+ 
     def action(self, request: HttpRequest) -> HttpResponse:
-        if (
-            self.workflow_state
-            and self.workflow_state.status == WorkflowState.STATUS_NEEDS_CHANGES
-        ):
-            # If the workflow was in the needs changes state, resume the existing workflow on submission
-            self.workflow_state.resume(self.request.user)
-        else:
-            # Otherwise start a new workflow
-            workflow = self.object.get_workflow()
-            workflow.start(self.object, self.request.user)
+        if not self.object.live:
+            messages.error(request, _("This object is not live"))
+            return self.get(request)
+        
+        action = get_unpublish_action(self.object)(
+            self.object,
+            user=request.user,
+        )
 
-        return self.redirect_to_success_url(request)
+        action.execute()
+
+        return self.redirect_to_failsafe_url(request)
 
 
 class SubmitView(BaseActionView):
     required_superclasses = [DraftStateMixin, WorkflowMixin]
     action_text = _("Submit for moderation")
     action_help_text_title = _("About submitting for moderation")
     action_help_text = [
@@ -314,28 +314,28 @@
 
     def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
         if not policy.can_submit_for_moderation():
             raise ValueError("User does not have permission to submit for moderation")
         
         if not self.object.has_unpublished_changes:
             raise ValueError("Object has no unpublished changes")
-
+   
     def action(self, request: HttpRequest) -> HttpResponse:
-        if not self.object.live:
-            messages.error(request, _("This object is not live"))
-            return self.get(request)
-        
-        action = get_unpublish_action(self.object)(
-            self.object,
-            user=request.user,
-        )
-
-        action.execute()
+        if (
+            self.workflow_state
+            and self.workflow_state.status == WorkflowState.STATUS_NEEDS_CHANGES
+        ):
+            # If the workflow was in the needs changes state, resume the existing workflow on submission
+            self.workflow_state.resume(self.request.user)
+        else:
+            # Otherwise start a new workflow
+            workflow = self.object.get_workflow()
+            workflow.start(self.object, self.request.user)
 
-        return self.redirect_to_failsafe_url(request)
+        return self.redirect_to_success_url(request)
 
 
 class CancelView(BaseActionView):
     template_name = "wagtail_fedit/editor/cancel_confirm.html"
     required_superclasses = [DraftStateMixin, WorkflowMixin]
     action_text = _("Cancel")
     action_help_text_title = _("About cancelling")
```

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.4/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.3.4/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.3.3
+Version: 1.3.4
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
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

