# Comparing `tmp/wagtail_fedit-1.3.0.tar.gz` & `tmp/wagtail_fedit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.0.tar", last modified: Fri Apr  5 12:55:06 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.1.tar", last modified: Fri Apr  5 13:39:17 2024, max compression
```

## Comparing `wagtail_fedit-1.3.0.tar` & `wagtail_fedit-1.3.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.190174 wagtail_fedit-1.3.0/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7546 2024-04-05 12:55:06.188175 wagtail_fedit-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6496 2024-04-05 12:54:51.000000 wagtail_fedit-1.3.0/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 12:55:06.249926 wagtail_fedit-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.788661 wagtail_fedit-1.3.0/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.829831 wagtail_fedit-1.3.0/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.0/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.832829 wagtail_fedit-1.3.0/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.836837 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.0/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.735180 wagtail_fedit-1.3.0/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.737189 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.849722 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.855719 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15212 2024-04-04 19:40:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.739190 wagtail_fedit-1.3.0/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.741534 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.862628 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.871240 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.890683 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     4890 2024-04-04 16:34:08.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.900531 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
--rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
--rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
--rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.909489 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.911348 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.922173 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.933605 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.933605 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16924 2024-04-04 19:49:27.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13828 2024-04-04 19:49:26.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.957259 wagtail_fedit-1.3.0/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.967409 wagtail_fedit-1.3.0/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.985962 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.067163 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/manage.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.090072 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.0/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.0/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.108307 wagtail_fedit-1.3.0/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9147 2024-04-05 12:45:56.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    11884 2024-04-05 12:45:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.151471 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.183248 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7546 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3550 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.708294 wagtail_fedit-1.3.1/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7595 2024-04-05 13:39:17.707295 wagtail_fedit-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.1/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 13:39:17.721958 wagtail_fedit-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.249475 wagtail_fedit-1.3.1/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.303944 wagtail_fedit-1.3.1/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.1/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.304943 wagtail_fedit-1.3.1/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.305965 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.1/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.200035 wagtail_fedit-1.3.1/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.201515 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.340990 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.366936 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15212 2024-04-05 13:21:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.202525 wagtail_fedit-1.3.1/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.204977 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.384954 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.408508 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.454459 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.483461 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
+-rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
+-rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.507071 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.520068 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.549929 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.551930 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.554317 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.580280 wagtail_fedit-1.3.1/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.610414 wagtail_fedit-1.3.1/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.615378 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.675804 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/manage.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.687632 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.1/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.1/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.700297 wagtail_fedit-1.3.1/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9276 2024-04-05 13:38:18.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12008 2024-04-05 13:08:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.706294 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.707295 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7595 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3550 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.0/LICENSE` & `wagtail_fedit-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/PKG-INFO` & `wagtail_fedit-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.0
+Version: 1.3.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -201,8 +201,11 @@
 
 ## Implemented
 
 * Revision Support
 * Locked Support
 * Draft Support
 * Preview Support
+* Workflow Support
+* Permissions
+* Audit Logs
 * Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.0 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.1 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -83,8 +83,9 @@
 model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
 is wrapped with `fedit_block` or `fedit_field` the field_name and model
 argument can be omitted. The parent- blocktag will share these variables
 through context. This makes it possibly to easily use editable sub-blocks
 across multiple different model types. If your model **ISN'T** capable of
 editing; or these variables aren't shared - your block will be rendered as
 normal. ## Implemented * Revision Support * Locked Support * Draft Support *
-Preview Support * Full block capabilities on Frontend Editing
+Preview Support * Workflow Support * Permissions * Audit Logs * Full block
+capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.3.0/README.md` & `wagtail_fedit-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -174,8 +174,11 @@
 
 ## Implemented
 
 * Revision Support
 * Locked Support
 * Draft Support
 * Preview Support
+* Workflow Support
+* Permissions
+* Audit Logs
 * Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -69,8 +69,9 @@
 model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
 is wrapped with `fedit_block` or `fedit_field` the field_name and model
 argument can be omitted. The parent- blocktag will share these variables
 through context. This makes it possibly to easily use editable sub-blocks
 across multiple different model types. If your model **ISN'T** capable of
 editing; or these variables aren't shared - your block will be rendered as
 normal. ## Implemented * Revision Support * Locked Support * Draft Support *
-Preview Support * Full block capabilities on Frontend Editing
+Preview Support * Workflow Support * Permissions * Audit Logs * Full block
+capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.3.0/setup.cfg` & `wagtail_fedit-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
+00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.1/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.1/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.1/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/models.py` & `wagtail_fedit-1.3.1/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 22% similar despite different names*

```diff
@@ -47,29 +47,50 @@
                 {% panel id="wagtail-fedit-help-text" icon="help" heading=help_text.heading %}
                     {% help_block status=help_text.status %}
                         <p><strong>{{ help_text.title }}</strong></p>
                         <p>{{ help_text.text }}</p>
                     {% endhelp_block %}
                 {% endpanel %}
             {% endif %}
-            {% block content %}
-                {% block errors %}
-                    {% if form.errors or form.non_field_errors %}
-                        <div class="error-message">
-                            <h2>{{ view.get_error_title }}</h2>
-                            <ul>
-                                {% for error in form.non_field_errors %}
-                                    <li>{{ error }}</li>
-                                {% endfor %}
-                                {{ form.errors.as_ul }}
-                            </ul>
-                        </div>
-                    {% endif %}
+
+            {% translate "Locked" as locked_heading %}
+            {% if locked and not locked_for_user %}
+                {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
+                    {% help_block status=info %}
+                        <p>{% translate "This object is locked" %}</p>
+                        <p>{% translate "You are still able to edit this object." %}</p>
+                    {% endhelp_block %}
+                {% endpanel %}
+            {% endif %}
+
+            {% if locked_for_user %}
+                {% panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %}
+                    {% help_block status=info %}
+                        <p>{% translate "This object is locked and cannot be edited." %}</p>
+                    {% endhelp_block %}
+                {% endpanel %}
+            {% else %}
+            
+                {% block content %}
+                    {% block errors %}
+                        {% if form.errors or form.non_field_errors %}
+                            <div class="error-message">
+                                <h2>{{ view.get_error_title }}</h2>
+                                <ul>
+                                    {% for error in form.non_field_errors %}
+                                        <li>{{ error }}</li>
+                                    {% endfor %}
+                                    {{ form.errors.as_ul }}
+                                </ul>
+                            </div>
+                        {% endif %}
+                    {% endblock %}
                 {% endblock %}
-            {% endblock %}
+                
+            {% endif %}
         </div>
     </main>
     {% block sidebar_root %}
         <aside>
             <div class="fedit-sidebar-logo">
                 {% block sidebar_logo %}{% endblock %}
             </div>
```

#### html2text {}

```diff
@@ -15,21 +15,31 @@
     * {{ message }}
     * {% endfor %}
 {% endif %}
 {% if help_text %} {% panel id="wagtail-fedit-help-text" icon="help"
 heading=help_text.heading %} {% help_block status=help_text.status %}
 {{{{ hheellpp__tteexxtt..ttiittllee }}}}
 {{ help_text.text }}
-{% endhelp_block %} {% endpanel %} {% endif %} {% block content %} {% block
+{% endhelp_block %} {% endpanel %} {% endif %} {% translate "Locked" as
+locked_heading %} {% if locked and not locked_for_user %} {% panel id="wagtail-
+fedit-lock-text" icon="help" heading=locked_heading %} {% help_block
+status=info %}
+{% translate "This object is locked" %}
+{% translate "You are still able to edit this object." %}
+{% endhelp_block %} {% endpanel %} {% endif %} {% if locked_for_user %} {%
+panel id="wagtail-fedit-lock-text" icon="help" heading=locked_heading %} {%
+help_block status=info %}
+{% translate "This object is locked and cannot be edited." %}
+{% endhelp_block %} {% endpanel %} {% else %} {% block content %} {% block
 errors %} {% if form.errors or form.non_field_errors %}
 ********** {{{{ vviieeww..ggeett__eerrrroorr__ttiittllee }}}} **********
     * {% for error in form.non_field_errors %}
     * {{ error }}
     * {% endfor %} {{ form.errors.as_ul }}
-{% endif %} {% endblock %} {% endblock %}
+{% endif %} {% endblock %} {% endblock %} {% endif %}
 {% block sidebar_root %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
 }" viewBox="0 0 16 16">
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x46040f66 (Thu Apr  4 19:49:26 2024 UTC)
-files sz: 13828
+moddate:  0xa1fe0f66 (Fri Apr  5 13:37:37 2024 UTC)
+files sz: 13783
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -161,18 +161,18 @@
     29         248 PUSH_NULL
                250 LOAD_NAME               16 (signing)
                252 LOAD_ATTR               38 (TimestampSigner)
                262 PRECALL                  0
                266 CALL                     0
                276 STORE_NAME              39 (url_value_signer)
    
-    32         278 LOAD_CONST              18 ('Field name is not available in the context for block {block.name}.')
+    32         278 LOAD_CONST              18 ('Field name is not available in the context for field %(field)s.')
                280 STORE_NAME              40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
    
-    33         282 LOAD_CONST              19 ('Model instance is not available in the context for block {block.name}.')
+    33         282 LOAD_CONST              19 ('Model instance is not available in the context for block %(block)s.')
                284 STORE_NAME              41 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
    
     36         286 PUSH_NULL
                288 LOAD_BUILD_CLASS
                290 LOAD_CONST              20 (<code object BlockEditNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 36>)
                292 MAKE_FUNCTION            0
                294 LOAD_CONST              21 ('BlockEditNode')
@@ -262,16 +262,16 @@
       ('hooks',)
       ('urlencode',)
       None
       2
       ('FeditBlockEditButton', 'FeditFieldEditButton')
       ('FEDIT_PREVIEW_VAR', 'get_field_content')
       ('CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR')
-      'Field name is not available in the context for block {block.name}.'
-      'Model instance is not available in the context for block {block.name}.'
+      'Field name is not available in the context for field %(field)s.'
+      'Model instance is not available in the context for block %(block)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a02020047006401840064026503a6030000ab0300
@@ -503,52 +503,50 @@
                   010000ab0100000000000000008a0c7c047c0164013c000000890c7c0164
                   043c0000007c02725809007c01a00b000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007d016e1023007418000000
                   0000000000000024007203010059006e0477007803590077017c01a00d00
                   000000000000000000000000000000000000007c05a6010000ab01000000
                   000000000001007c02a00e00000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d0864057c005f0f0000000000
-                  0000006e4c7c006a10000000000000000072367c006a1000000000000000
+                  0000006e387c006a10000000000000000072227c006a1000000000000000
                   00a01100000000000000000000000000000000000000007c01a6010000ab
-                  0100000000000000007d087c01a00a000000000000000000000000000000
-                  000000000064066407a6020000ab0200000000000000007c005f0f000000
-                  00000000006e0f7413000000000000000000006408a6010000ab01000000
-                  000000000082017c0473207425000000000000000000006a130000000000
-                  00000074280000000000000000000064097c0269017a060000a6010000ab
-                  01000000000000000001007c085300890c73207425000000000000000000
-                  006a130000000000000000742a0000000000000000000064097c0269017a
+                  0100000000000000007d0864067c005f0f00000000000000006e0f741300
+                  0000000000000000006407a6010000ab01000000000000000082017c0473
+                  207425000000000000000000006a13000000000000000074280000000000
+                  000000000064087c0469017a060000a6010000ab01000000000000000001
+                  007c085300890c73257425000000000000000000006a1300000000000000
+                  00742a0000000000000000000064097c026a16000000000000000069017a
                   060000a6010000ab01000000000000000001007c0853007c03730d64027c
                   01760072097c016402190000000000000000007d036e2d7c03731a7c0272
-                  18742d000000000000000000007c02640aa6020000ab0200000000000000
-                  0072087c026a1700000000000000007d036e117c03730f74130000000000
+                  18742f000000000000000000007c02640aa6020000ab0200000000000000
+                  0072087c026a1800000000000000007d036e117c03730f74130000000000
                   00000000006403a6010000ab01000000000000000082017c01a00a000000
                   0000000000000000000000000000000000640ba6010000ab010000000000
-                  0000008a0d890d7271890d6a1800000000000000006a1900000000000000
-                  007263890d6a180000000000000000a01a00000000000000000000000000
-                  00000000000000640ca6010000ab0100000000000000007249890d6a1800
-                  00000000000000a01a000000000000000000000000000000000000000089
-                  0c6a1b00000000000000006a1c00000000000000009b00640d890c6a1b00
-                  000000000000006a1d00000000000000009b009d03a6010000ab01000000
-                  00000000007216743d00000000000000000000890d743e00000000000000
-                  0000006407a6030000ab03000000000000000073027c085300740d000000
-                  00000000000000890c744000000000000000000000a6020000ab02000000
-                  0000000000721d7443000000000000000000007c01640e880c6601640f84
+                  0000008a0d890d7271890d6a1900000000000000006a1a00000000000000
+                  007263890d6a190000000000000000a01b00000000000000000000000000
+                  00000000000000640ca6010000ab0100000000000000007249890d6a1900
+                  00000000000000a01b000000000000000000000000000000000000000089
+                  0c6a1c00000000000000006a1d00000000000000009b00640d890c6a1c00
+                  000000000000006a1e00000000000000009b009d03a6010000ab01000000
+                  00000000007216743f00000000000000000000890d744000000000000000
+                  0000006406a6030000ab03000000000000000073027c085300740d000000
+                  00000000000000890c744200000000000000000000a6020000ab02000000
+                  0000000000721d7445000000000000000000007c01640e880c6601640f84
                   08a6030000ab0300000000000000007d097c099b0064107c039b0064119d
-                  047d096e0264007d097c05a0220000000000000000000000000000000000
-                  00000064127c006a0f0000000000000000a6020000ab0200000000000000
-                  000100744700000000000000000000a6000000ab00000000000000000067
-                  017d0a7449000000000000000000006a250000000000000000744c000000
-                  00000000000000a6010000ab01000000000000000044005d127d0b02007c
-                  0b890d7c0a890c7c037c04ac13a6050000ab05000000000000000001008c
-                  13880d6601641484087c0a4400a6000000ab0000000000000000007d0a74
-                  4f0000000000000000000074510000000000000000000064007c0aa60200
-                  00ab020000000000000000a6010000ab0100000000000000007d0a745300
-                  000000000000000000641502007c006a2a00000000000000007c037c0466
-                  026416890c69017c05a4018e017c097c03890c7c087c047c017c04890c7c
-                  0a64179c0aa6020000ab0200000000000000005300
+                  047d096e0264007d097c006a0f00000000000000007c0564123c00000074
+                  4700000000000000000000a6000000ab00000000000000000067017d0a74
+                  49000000000000000000006a250000000000000000744c00000000000000
+                  000000a6010000ab01000000000000000044005d127d0b02007c0b890d7c
+                  0a890c7c037c04ac13a6050000ab05000000000000000001008c13880d66
+                  01641484087c0a4400a6000000ab0000000000000000007d0a744f000000
+                  0000000000000074510000000000000000000064007c0aa6020000ab0200
+                  00000000000000a6010000ab0100000000000000007d0a74530000000000
+                  0000000000641502007c006a2a00000000000000007c037c046602641689
+                  0c69017c05a4018e017c097c03890c7c087c047c017c04890c7c0a64179c
+                  0aa6020000ab0200000000000000005300
                              0 MAKE_CELL               12 (model)
                              2 MAKE_CELL               13 (request)
                
                 56           4 RESUME                   0
                
                 57           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (block)
@@ -738,324 +736,317 @@
                            842 PRECALL                  1
                            846 CALL                     1
                            856 STORE_FAST               8 (rendered)
                
                 99         858 LOAD_CONST               5 (True)
                            860 LOAD_FAST                0 (self)
                            862 STORE_ATTR              15 (has_block)
-                           872 JUMP_FORWARD            76 (to 1026)
+                           872 JUMP_FORWARD            56 (to 986)
                
                100     >>  874 LOAD_FAST                0 (self)
                            876 LOAD_ATTR               16 (nl)
-                           886 POP_JUMP_FORWARD_IF_FALSE    54 (to 996)
+                           886 POP_JUMP_FORWARD_IF_FALSE    34 (to 956)
                
                101         888 LOAD_FAST                0 (self)
                            890 LOAD_ATTR               16 (nl)
                            900 LOAD_METHOD             17 (render)
                            922 LOAD_FAST                1 (context)
                            924 PRECALL                  1
                            928 CALL                     1
                            938 STORE_FAST               8 (rendered)
                
-               102         940 LOAD_FAST                1 (context)
-                           942 LOAD_METHOD             10 (get)
-                           964 LOAD_CONST               6 ('wagtail_fedit_has_block')
-                           966 LOAD_CONST               7 (False)
-                           968 PRECALL                  2
-                           972 CALL                     2
-                           982 LOAD_FAST                0 (self)
-                           984 STORE_ATTR              15 (has_block)
-                           994 JUMP_FORWARD            15 (to 1026)
-               
-               104     >>  996 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1008 LOAD_CONST               8 ('Block or nodelist is required')
-                          1010 PRECALL                  1
-                          1014 CALL                     1
-                          1024 RAISE_VARARGS            1
-               
-               106     >> 1026 LOAD_FAST                4 (field_name)
-                          1028 POP_JUMP_FORWARD_IF_TRUE    32 (to 1094)
-               
-               107        1030 LOAD_GLOBAL             37 (NULL + warnings)
-                          1042 LOAD_ATTR               19 (warn)
-                          1052 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-                          1064 LOAD_CONST               9 ('block')
-                          1066 LOAD_FAST                2 (block)
-                          1068 BUILD_MAP                1
-                          1070 BINARY_OP                6 (%)
-                          1074 PRECALL                  1
-                          1078 CALL                     1
-                          1088 POP_TOP
-               
-               108        1090 LOAD_FAST                8 (rendered)
-                          1092 RETURN_VALUE
-               
-               110     >> 1094 LOAD_DEREF              12 (model)
-                          1096 POP_JUMP_FORWARD_IF_TRUE    32 (to 1162)
-               
-               111        1098 LOAD_GLOBAL             37 (NULL + warnings)
-                          1110 LOAD_ATTR               19 (warn)
-                          1120 LOAD_GLOBAL             42 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-                          1132 LOAD_CONST               9 ('block')
-                          1134 LOAD_FAST                2 (block)
-                          1136 BUILD_MAP                1
-                          1138 BINARY_OP                6 (%)
-                          1142 PRECALL                  1
-                          1146 CALL                     1
-                          1156 POP_TOP
-               
-               112        1158 LOAD_FAST                8 (rendered)
-                          1160 RETURN_VALUE
-               
-               115     >> 1162 LOAD_FAST                3 (block_id)
-                          1164 POP_JUMP_FORWARD_IF_TRUE    13 (to 1192)
-                          1166 LOAD_CONST               2 ('block_id')
-                          1168 LOAD_FAST                1 (context)
-                          1170 CONTAINS_OP              0
-                          1172 POP_JUMP_FORWARD_IF_FALSE     9 (to 1192)
-               
-               116        1174 LOAD_FAST                1 (context)
-                          1176 LOAD_CONST               2 ('block_id')
-                          1178 BINARY_SUBSCR
-                          1188 STORE_FAST               3 (block_id)
-                          1190 JUMP_FORWARD            45 (to 1282)
-               
-               117     >> 1192 LOAD_FAST                3 (block_id)
-                          1194 POP_JUMP_FORWARD_IF_TRUE    26 (to 1248)
-                          1196 LOAD_FAST                2 (block)
-                          1198 POP_JUMP_FORWARD_IF_FALSE    24 (to 1248)
-                          1200 LOAD_GLOBAL             45 (NULL + hasattr)
-                          1212 LOAD_FAST                2 (block)
-                          1214 LOAD_CONST              10 ('id')
-                          1216 PRECALL                  2
-                          1220 CALL                     2
-                          1230 POP_JUMP_FORWARD_IF_FALSE     8 (to 1248)
-               
-               118        1232 LOAD_FAST                2 (block)
-                          1234 LOAD_ATTR               23 (id)
-                          1244 STORE_FAST               3 (block_id)
-                          1246 JUMP_FORWARD            17 (to 1282)
-               
-               119     >> 1248 LOAD_FAST                3 (block_id)
-                          1250 POP_JUMP_FORWARD_IF_TRUE    15 (to 1282)
-               
-               120        1252 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1264 LOAD_CONST               3 ('Block ID is required')
-                          1266 PRECALL                  1
-                          1270 CALL                     1
-                          1280 RAISE_VARARGS            1
-               
-               123     >> 1282 LOAD_FAST                1 (context)
-                          1284 LOAD_METHOD             10 (get)
-                          1306 LOAD_CONST              11 ('request')
-                          1308 PRECALL                  1
-                          1312 CALL                     1
-                          1322 STORE_DEREF             13 (request)
-               
-               124        1324 LOAD_DEREF              13 (request)
-                          1326 POP_JUMP_FORWARD_IF_FALSE   113 (to 1554)
-               
-               126        1328 LOAD_DEREF              13 (request)
-                          1330 LOAD_ATTR               24 (user)
-                          1340 LOAD_ATTR               25 (is_authenticated)
-               
-               125        1350 POP_JUMP_FORWARD_IF_FALSE    99 (to 1550)
-               
-               127        1352 LOAD_DEREF              13 (request)
-                          1354 LOAD_ATTR               24 (user)
-                          1364 LOAD_METHOD             26 (has_perm)
-                          1386 LOAD_CONST              12 ('wagtailadmin.access_admin')
-                          1388 PRECALL                  1
-                          1392 CALL                     1
-               
-               125        1402 POP_JUMP_FORWARD_IF_FALSE    73 (to 1550)
-               
-               128        1404 LOAD_DEREF              13 (request)
-                          1406 LOAD_ATTR               24 (user)
-                          1416 LOAD_METHOD             26 (has_perm)
-                          1438 LOAD_DEREF              12 (model)
-                          1440 LOAD_ATTR               27 (_meta)
-                          1450 LOAD_ATTR               28 (app_label)
-                          1460 FORMAT_VALUE             0
-                          1462 LOAD_CONST              13 ('.change_')
-                          1464 LOAD_DEREF              12 (model)
-                          1466 LOAD_ATTR               27 (_meta)
-                          1476 LOAD_ATTR               29 (model_name)
-                          1486 FORMAT_VALUE             0
-                          1488 BUILD_STRING             3
-                          1490 PRECALL                  1
-                          1494 CALL                     1
-               
-               125        1504 POP_JUMP_FORWARD_IF_FALSE    22 (to 1550)
-               
-               129        1506 LOAD_GLOBAL             61 (NULL + getattr)
-                          1518 LOAD_DEREF              13 (request)
-                          1520 LOAD_GLOBAL             62 (FEDIT_PREVIEW_VAR)
-                          1532 LOAD_CONST               7 (False)
-                          1534 PRECALL                  3
-                          1538 CALL                     3
-               
-               125        1548 POP_JUMP_FORWARD_IF_TRUE     2 (to 1554)
-               
-               132     >> 1550 LOAD_FAST                8 (rendered)
-                          1552 RETURN_VALUE
-               
-               136     >> 1554 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1566 LOAD_DEREF              12 (model)
-                          1568 LOAD_GLOBAL             64 (Page)
-                          1580 PRECALL                  2
-                          1584 CALL                     2
-                          1594 POP_JUMP_FORWARD_IF_FALSE    29 (to 1654)
-               
-               137        1596 LOAD_GLOBAL             67 (NULL + _get_from_context_or_set)
-               
-               138        1608 LOAD_FAST                1 (context)
-                          1610 LOAD_CONST              14 ('page_base_edit_url')
-               
-               139        1612 LOAD_CLOSURE            12 (model)
-                          1614 BUILD_TUPLE              1
-                          1616 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 139>)
-                          1618 MAKE_FUNCTION            8 (closure)
-               
-               137        1620 PRECALL                  3
-                          1624 CALL                     3
-                          1634 STORE_FAST               9 (admin_edit_url)
-               
-               144        1636 LOAD_FAST                9 (admin_edit_url)
-                          1638 FORMAT_VALUE             0
-                          1640 LOAD_CONST              16 ('#block-')
-                          1642 LOAD_FAST                3 (block_id)
-                          1644 FORMAT_VALUE             0
-                          1646 LOAD_CONST              17 ('-section')
-                          1648 BUILD_STRING             4
-                          1650 STORE_FAST               9 (admin_edit_url)
-                          1652 JUMP_FORWARD             2 (to 1658)
-               
-               146     >> 1654 LOAD_CONST               0 (None)
-                          1656 STORE_FAST               9 (admin_edit_url)
-               
-               148     >> 1658 LOAD_FAST                5 (extra)
-                          1660 LOAD_METHOD             34 (setdefault)
-                          1682 LOAD_CONST              18 ('has_block')
-                          1684 LOAD_FAST                0 (self)
-                          1686 LOAD_ATTR               15 (has_block)
-                          1696 PRECALL                  2
-                          1700 CALL                     2
-                          1710 POP_TOP
-               
-               151        1712 LOAD_GLOBAL             71 (NULL + FeditBlockEditButton)
-                          1724 PRECALL                  0
-                          1728 CALL                     0
-               
-               150        1738 BUILD_LIST               1
-                          1740 STORE_FAST              10 (items)
-               
-               154        1742 LOAD_GLOBAL             73 (NULL + hooks)
-                          1754 LOAD_ATTR               37 (get_hooks)
-                          1764 LOAD_GLOBAL             76 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1776 PRECALL                  1
-                          1780 CALL                     1
-                          1790 GET_ITER
-                       >> 1792 FOR_ITER                18 (to 1830)
-                          1794 STORE_FAST              11 (hook)
-               
-               155        1796 PUSH_NULL
-                          1798 LOAD_FAST               11 (hook)
-                          1800 LOAD_DEREF              13 (request)
-                          1802 LOAD_FAST               10 (items)
-                          1804 LOAD_DEREF              12 (model)
-                          1806 LOAD_FAST                3 (block_id)
-                          1808 LOAD_FAST                4 (field_name)
-                          1810 KW_NAMES                19
-                          1812 PRECALL                  5
-                          1816 CALL                     5
-                          1826 POP_TOP
-                          1828 JUMP_BACKWARD           19 (to 1792)
-               
-               157     >> 1830 LOAD_CLOSURE            13 (request)
-                          1832 BUILD_TUPLE              1
-                          1834 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 157>)
-                          1836 MAKE_FUNCTION            8 (closure)
-                          1838 LOAD_FAST               10 (items)
-                          1840 GET_ITER
-                          1842 PRECALL                  0
-                          1846 CALL                     0
-                          1856 STORE_FAST              10 (items)
-               
-               158        1858 LOAD_GLOBAL             79 (NULL + list)
-                          1870 LOAD_GLOBAL             81 (NULL + filter)
-                          1882 LOAD_CONST               0 (None)
-                          1884 LOAD_FAST               10 (items)
-                          1886 PRECALL                  2
-                          1890 CALL                     2
-                          1900 PRECALL                  1
-                          1904 CALL                     1
-                          1914 STORE_FAST              10 (items)
-               
-               160        1916 LOAD_GLOBAL             83 (NULL + render_to_string)
-               
-               161        1928 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
-               
-               163        1930 PUSH_NULL
-                          1932 LOAD_FAST                0 (self)
-                          1934 LOAD_ATTR               42 (get_edit_url)
-               
-               164        1944 LOAD_FAST                3 (block_id)
-                          1946 LOAD_FAST                4 (field_name)
-               
-               163        1948 BUILD_TUPLE              2
-                          1950 LOAD_CONST              22 ('instance')
-               
-               165        1952 LOAD_DEREF              12 (model)
-               
-               163        1954 BUILD_MAP                1
-               
-               166        1956 LOAD_FAST                5 (extra)
-               
-               163        1958 DICT_MERGE               1
-                          1960 CALL_FUNCTION_EX         1
-               
-               168        1962 LOAD_FAST                9 (admin_edit_url)
-               
-               169        1964 LOAD_FAST                3 (block_id)
-               
-               170        1966 LOAD_DEREF              12 (model)
-               
-               171        1968 LOAD_FAST                8 (rendered)
-               
-               172        1970 LOAD_FAST                4 (field_name)
-               
-               173        1972 LOAD_FAST                1 (context)
-               
-               174        1974 LOAD_FAST                4 (field_name)
-               
-               175        1976 LOAD_DEREF              12 (model)
-               
-               176        1978 LOAD_FAST               10 (items)
-               
-               162        1980 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
-                          1982 BUILD_CONST_KEY_MAP     10
-               
-               160        1984 PRECALL                  2
-                          1988 CALL                     2
-                          1998 RETURN_VALUE
+               102         940 LOAD_CONST               6 (False)
+                           942 LOAD_FAST                0 (self)
+                           944 STORE_ATTR              15 (has_block)
+                           954 JUMP_FORWARD            15 (to 986)
+               
+               104     >>  956 LOAD_GLOBAL             19 (NULL + ValueError)
+                           968 LOAD_CONST               7 ('Block or nodelist is required')
+                           970 PRECALL                  1
+                           974 CALL                     1
+                           984 RAISE_VARARGS            1
+               
+               106     >>  986 LOAD_FAST                4 (field_name)
+                           988 POP_JUMP_FORWARD_IF_TRUE    32 (to 1054)
+               
+               107         990 LOAD_GLOBAL             37 (NULL + warnings)
+                          1002 LOAD_ATTR               19 (warn)
+                          1012 LOAD_GLOBAL             40 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+                          1024 LOAD_CONST               8 ('field')
+                          1026 LOAD_FAST                4 (field_name)
+                          1028 BUILD_MAP                1
+                          1030 BINARY_OP                6 (%)
+                          1034 PRECALL                  1
+                          1038 CALL                     1
+                          1048 POP_TOP
+               
+               108        1050 LOAD_FAST                8 (rendered)
+                          1052 RETURN_VALUE
+               
+               110     >> 1054 LOAD_DEREF              12 (model)
+                          1056 POP_JUMP_FORWARD_IF_TRUE    37 (to 1132)
+               
+               111        1058 LOAD_GLOBAL             37 (NULL + warnings)
+                          1070 LOAD_ATTR               19 (warn)
+                          1080 LOAD_GLOBAL             42 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+                          1092 LOAD_CONST               9 ('block')
+                          1094 LOAD_FAST                2 (block)
+                          1096 LOAD_ATTR               22 (label)
+                          1106 BUILD_MAP                1
+                          1108 BINARY_OP                6 (%)
+                          1112 PRECALL                  1
+                          1116 CALL                     1
+                          1126 POP_TOP
+               
+               112        1128 LOAD_FAST                8 (rendered)
+                          1130 RETURN_VALUE
+               
+               115     >> 1132 LOAD_FAST                3 (block_id)
+                          1134 POP_JUMP_FORWARD_IF_TRUE    13 (to 1162)
+                          1136 LOAD_CONST               2 ('block_id')
+                          1138 LOAD_FAST                1 (context)
+                          1140 CONTAINS_OP              0
+                          1142 POP_JUMP_FORWARD_IF_FALSE     9 (to 1162)
+               
+               116        1144 LOAD_FAST                1 (context)
+                          1146 LOAD_CONST               2 ('block_id')
+                          1148 BINARY_SUBSCR
+                          1158 STORE_FAST               3 (block_id)
+                          1160 JUMP_FORWARD            45 (to 1252)
+               
+               117     >> 1162 LOAD_FAST                3 (block_id)
+                          1164 POP_JUMP_FORWARD_IF_TRUE    26 (to 1218)
+                          1166 LOAD_FAST                2 (block)
+                          1168 POP_JUMP_FORWARD_IF_FALSE    24 (to 1218)
+                          1170 LOAD_GLOBAL             47 (NULL + hasattr)
+                          1182 LOAD_FAST                2 (block)
+                          1184 LOAD_CONST              10 ('id')
+                          1186 PRECALL                  2
+                          1190 CALL                     2
+                          1200 POP_JUMP_FORWARD_IF_FALSE     8 (to 1218)
+               
+               118        1202 LOAD_FAST                2 (block)
+                          1204 LOAD_ATTR               24 (id)
+                          1214 STORE_FAST               3 (block_id)
+                          1216 JUMP_FORWARD            17 (to 1252)
+               
+               119     >> 1218 LOAD_FAST                3 (block_id)
+                          1220 POP_JUMP_FORWARD_IF_TRUE    15 (to 1252)
+               
+               120        1222 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1234 LOAD_CONST               3 ('Block ID is required')
+                          1236 PRECALL                  1
+                          1240 CALL                     1
+                          1250 RAISE_VARARGS            1
+               
+               123     >> 1252 LOAD_FAST                1 (context)
+                          1254 LOAD_METHOD             10 (get)
+                          1276 LOAD_CONST              11 ('request')
+                          1278 PRECALL                  1
+                          1282 CALL                     1
+                          1292 STORE_DEREF             13 (request)
+               
+               124        1294 LOAD_DEREF              13 (request)
+                          1296 POP_JUMP_FORWARD_IF_FALSE   113 (to 1524)
+               
+               126        1298 LOAD_DEREF              13 (request)
+                          1300 LOAD_ATTR               25 (user)
+                          1310 LOAD_ATTR               26 (is_authenticated)
+               
+               125        1320 POP_JUMP_FORWARD_IF_FALSE    99 (to 1520)
+               
+               127        1322 LOAD_DEREF              13 (request)
+                          1324 LOAD_ATTR               25 (user)
+                          1334 LOAD_METHOD             27 (has_perm)
+                          1356 LOAD_CONST              12 ('wagtailadmin.access_admin')
+                          1358 PRECALL                  1
+                          1362 CALL                     1
+               
+               125        1372 POP_JUMP_FORWARD_IF_FALSE    73 (to 1520)
+               
+               128        1374 LOAD_DEREF              13 (request)
+                          1376 LOAD_ATTR               25 (user)
+                          1386 LOAD_METHOD             27 (has_perm)
+                          1408 LOAD_DEREF              12 (model)
+                          1410 LOAD_ATTR               28 (_meta)
+                          1420 LOAD_ATTR               29 (app_label)
+                          1430 FORMAT_VALUE             0
+                          1432 LOAD_CONST              13 ('.change_')
+                          1434 LOAD_DEREF              12 (model)
+                          1436 LOAD_ATTR               28 (_meta)
+                          1446 LOAD_ATTR               30 (model_name)
+                          1456 FORMAT_VALUE             0
+                          1458 BUILD_STRING             3
+                          1460 PRECALL                  1
+                          1464 CALL                     1
+               
+               125        1474 POP_JUMP_FORWARD_IF_FALSE    22 (to 1520)
+               
+               129        1476 LOAD_GLOBAL             63 (NULL + getattr)
+                          1488 LOAD_DEREF              13 (request)
+                          1490 LOAD_GLOBAL             64 (FEDIT_PREVIEW_VAR)
+                          1502 LOAD_CONST               6 (False)
+                          1504 PRECALL                  3
+                          1508 CALL                     3
+               
+               125        1518 POP_JUMP_FORWARD_IF_TRUE     2 (to 1524)
+               
+               132     >> 1520 LOAD_FAST                8 (rendered)
+                          1522 RETURN_VALUE
+               
+               136     >> 1524 LOAD_GLOBAL             13 (NULL + isinstance)
+                          1536 LOAD_DEREF              12 (model)
+                          1538 LOAD_GLOBAL             66 (Page)
+                          1550 PRECALL                  2
+                          1554 CALL                     2
+                          1564 POP_JUMP_FORWARD_IF_FALSE    29 (to 1624)
+               
+               137        1566 LOAD_GLOBAL             69 (NULL + _get_from_context_or_set)
+               
+               138        1578 LOAD_FAST                1 (context)
+                          1580 LOAD_CONST              14 ('page_base_edit_url')
+               
+               139        1582 LOAD_CLOSURE            12 (model)
+                          1584 BUILD_TUPLE              1
+                          1586 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 139>)
+                          1588 MAKE_FUNCTION            8 (closure)
+               
+               137        1590 PRECALL                  3
+                          1594 CALL                     3
+                          1604 STORE_FAST               9 (admin_edit_url)
+               
+               144        1606 LOAD_FAST                9 (admin_edit_url)
+                          1608 FORMAT_VALUE             0
+                          1610 LOAD_CONST              16 ('#block-')
+                          1612 LOAD_FAST                3 (block_id)
+                          1614 FORMAT_VALUE             0
+                          1616 LOAD_CONST              17 ('-section')
+                          1618 BUILD_STRING             4
+                          1620 STORE_FAST               9 (admin_edit_url)
+                          1622 JUMP_FORWARD             2 (to 1628)
+               
+               146     >> 1624 LOAD_CONST               0 (None)
+                          1626 STORE_FAST               9 (admin_edit_url)
+               
+               148     >> 1628 LOAD_FAST                0 (self)
+                          1630 LOAD_ATTR               15 (has_block)
+                          1640 LOAD_FAST                5 (extra)
+                          1642 LOAD_CONST              18 ('has_block')
+                          1644 STORE_SUBSCR
+               
+               151        1648 LOAD_GLOBAL             71 (NULL + FeditBlockEditButton)
+                          1660 PRECALL                  0
+                          1664 CALL                     0
+               
+               150        1674 BUILD_LIST               1
+                          1676 STORE_FAST              10 (items)
+               
+               154        1678 LOAD_GLOBAL             73 (NULL + hooks)
+                          1690 LOAD_ATTR               37 (get_hooks)
+                          1700 LOAD_GLOBAL             76 (CONSTRUCT_BLOCK_TOOLBAR)
+                          1712 PRECALL                  1
+                          1716 CALL                     1
+                          1726 GET_ITER
+                       >> 1728 FOR_ITER                18 (to 1766)
+                          1730 STORE_FAST              11 (hook)
+               
+               155        1732 PUSH_NULL
+                          1734 LOAD_FAST               11 (hook)
+                          1736 LOAD_DEREF              13 (request)
+                          1738 LOAD_FAST               10 (items)
+                          1740 LOAD_DEREF              12 (model)
+                          1742 LOAD_FAST                3 (block_id)
+                          1744 LOAD_FAST                4 (field_name)
+                          1746 KW_NAMES                19
+                          1748 PRECALL                  5
+                          1752 CALL                     5
+                          1762 POP_TOP
+                          1764 JUMP_BACKWARD           19 (to 1728)
+               
+               157     >> 1766 LOAD_CLOSURE            13 (request)
+                          1768 BUILD_TUPLE              1
+                          1770 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 157>)
+                          1772 MAKE_FUNCTION            8 (closure)
+                          1774 LOAD_FAST               10 (items)
+                          1776 GET_ITER
+                          1778 PRECALL                  0
+                          1782 CALL                     0
+                          1792 STORE_FAST              10 (items)
+               
+               158        1794 LOAD_GLOBAL             79 (NULL + list)
+                          1806 LOAD_GLOBAL             81 (NULL + filter)
+                          1818 LOAD_CONST               0 (None)
+                          1820 LOAD_FAST               10 (items)
+                          1822 PRECALL                  2
+                          1826 CALL                     2
+                          1836 PRECALL                  1
+                          1840 CALL                     1
+                          1850 STORE_FAST              10 (items)
+               
+               160        1852 LOAD_GLOBAL             83 (NULL + render_to_string)
+               
+               161        1864 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
+               
+               163        1866 PUSH_NULL
+                          1868 LOAD_FAST                0 (self)
+                          1870 LOAD_ATTR               42 (get_edit_url)
+               
+               164        1880 LOAD_FAST                3 (block_id)
+                          1882 LOAD_FAST                4 (field_name)
+               
+               163        1884 BUILD_TUPLE              2
+                          1886 LOAD_CONST              22 ('instance')
+               
+               165        1888 LOAD_DEREF              12 (model)
+               
+               163        1890 BUILD_MAP                1
+               
+               166        1892 LOAD_FAST                5 (extra)
+               
+               163        1894 DICT_MERGE               1
+                          1896 CALL_FUNCTION_EX         1
+               
+               168        1898 LOAD_FAST                9 (admin_edit_url)
+               
+               169        1900 LOAD_FAST                3 (block_id)
+               
+               170        1902 LOAD_DEREF              12 (model)
+               
+               171        1904 LOAD_FAST                8 (rendered)
+               
+               172        1906 LOAD_FAST                4 (field_name)
+               
+               173        1908 LOAD_FAST                1 (context)
+               
+               174        1910 LOAD_FAST                4 (field_name)
+               
+               175        1912 LOAD_DEREF              12 (model)
+               
+               176        1914 LOAD_FAST               10 (items)
+               
+               162        1916 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
+                          1918 BUILD_CONST_KEY_MAP     10
+               
+               160        1920 PRECALL                  2
+                          1924 CALL                     2
+                          1934 RETURN_VALUE
                ExceptionTable:
                  700 to 738 -> 742 [0]
                  742 to 760 -> 768 [1] lasti
                  766 to 766 -> 768 [1] lasti
                consts
                   None
                   'wagtail_fedit_field_name'
                   'block_id'
                   'Block ID is required'
                   'wagtail_fedit_instance'
                   True
-                  'wagtail_fedit_has_block'
                   False
                   'Block or nodelist is required'
+                  'field'
                   'block'
                   'id'
                   'request'
                   'wagtailadmin.access_admin'
                   '.change_'
                   'page_base_edit_url'
                   code
@@ -1128,27 +1119,27 @@
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
                      firstlineno 157
                      lnotab 0x
                   'wagtail_fedit/content/editable_block.html'
                   'instance'
                   ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
-               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'setdefault', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
+               names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'get', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'warnings', 'warn', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'label', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
                varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'rendered', 'admin_edit_url', 'items', 'hook')
                freevars   ()
                cellvars   ('model', 'request')
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 56
                lnotab
                   0x06010e010e010e010e010e0332012a0132020c0110022a012a012a012a
                   012a012a012a012a0210011e052e010a010a04040102012c01120104ff08
-                  022a012a0110010e01340138021e0204013c01040204013c0104030c0112
+                  022a012a0110010e01340110021e0204013c0104020401460104030c0112
                   012801100104011e032a01040216ff020232fe020364fd02042afc020704
-                  042a010c01040108fe10071202040236031aff0404360122021c013a020c
+                  042a010c01040108fe10071202040214031aff0404360122021c013a020c
                   0102020e0104ff040202fe020302fd040502010201020102010201020102
                   01020102f204fe
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.1/wagtail_fedit/templatetags/fedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 )
 
 
 register = library.Library()
 url_value_signer = signing.TimestampSigner()
 
 
-WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for block {block.name}."
-WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for block {block.name}."
+WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for field %(field)s."
+WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for block %(block)s."
 
 
 class BlockEditNode(Node):
     class UnpackError(Exception):
         pass
 
     def __init__(self,
@@ -95,24 +95,24 @@
             except AttributeError:
                 pass
             context.update(extra)
             rendered = block.render_as_block(context)
             self.has_block = True
         elif self.nl:
             rendered = self.nl.render(context)
-            self.has_block = context.get("wagtail_fedit_has_block", False)
+            self.has_block = False
         else:
             raise ValueError("Block or nodelist is required")
         
         if not field_name:
-            warnings.warn(WARNING_FIELD_NAME_NOT_AVAILABLE % {"block": block})
+            warnings.warn(WARNING_FIELD_NAME_NOT_AVAILABLE % {"field": field_name})
             return rendered
         
         if not model:
-            warnings.warn(WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {"block": block})
+            warnings.warn(WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {"block": block.label})
             return rendered
         
         # Get block id from block if bound or context.
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
@@ -141,15 +141,15 @@
                     args=[model.id],
                 ),
             )
             admin_edit_url = f"{admin_edit_url}#block-{block_id}-section"
         else:
             admin_edit_url = None
 
-        extra.setdefault("has_block", self.has_block)
+        extra["has_block"] = self.has_block
 
         items = [
             FeditBlockEditButton(),
         ]
 
         for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
             hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/settings.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.1/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.1/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.1/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.1/wagtail_fedit/views/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,27 @@
             "model_string": model_string,
         }
     
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         must = {
             "request": self.request,
-            # "wagtail_fedit_instance": instance,
             "contentpath": self.contentpath,
             "block_id": self.block_id,
             "field_name": self.field_name,
             "model_id": self.model_id,
             "model_name": self.model_name,
             "app_label": self.app_label,
             "block": self.block,
             "instance": self.instance,
             "streamfield": self.streamfield,
             "has_block": self.has_block,
             "label": self.block.block.label,
             "wagtail_fedit_instance": self.instance,
+            "wagtail_fedit_field_name": self.field_name,
             "wagtail_fedit_has_block": self.has_block,
             "edit_url": BlockEditNode.get_edit_url(
                 self.block_id, self.field_name, self.instance,
             ),
             "form_attrs": {
                 "data-block-id": self.block_id,
                 "data-block-name": self.block.block.name,
@@ -141,50 +141,57 @@
     
     def render_to_response(self, context: dict[str, Any], success: bool = True, extra: dict = None, **response_kwargs: Any) -> HttpResponse:
         if not extra:
             extra = {}
 
         extra.update({
             "success": success,
+            "locked": self.lock is not None,
+            "locked_for_user": self.locked_for_user,
         })
 
         context.update(extra)
 
         return render(
             self.request,
             self.template_name,
             context,
         )
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(block=self.block, parent_instance=self.instance, request=request)
         # Safe to omit data from context - we are not rendering the content.
         return self.render_to_response(
-            self.get_context_data(form=form, locked=self.locked_for_user),
+            self.get_context_data(
+                form=form,
+            ),
             success=True,
         )
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, block=self.block, parent_instance=self.instance, request=request)
 
         # Set the preview flag to mark as editable block when re-rendering.
         setattr(request, utils.FEDIT_PREVIEW_VAR, True)
 
         valid = form.is_valid()
         if valid and not self.locked_for_user:
             self.block = form.save()
+
         else:
             # We are not rendering the content, so we can omit data from context.
             return JsonResponse({
                 "success": False,
                 "errors": form.errors,
                 "locked": self.locked_for_user,
                 "html": render_to_string(
                     "wagtail_fedit/editor/block_iframe.html",
-                    context=self.get_context_data(form=form, locked=self.locked_for_user),
+                    context=self.get_context_data(
+                        form=form,
+                    ),
                     request=request,
                 )
             }, status=423 if self.locked_for_user else 400)
         
         extra_log_kwargs = {}
         if isinstance(self.instance, RevisionMixin):
             extra_log_kwargs["revision"] = self.instance.latest_revision
@@ -225,16 +232,17 @@
                 model=self.instance,
                 **data,
             )
 
             context = self.get_context_data()
             html = node.render(context)
         else:
+
             keys = request.GET.keys()
             data = BlockEditNode.unpack(*keys, request=request)
-            html = self.block.block.render(self.block.value, self.get_context_data(**dict(data)))
+            html = self.block.block.render(self.block.value, self.get_context_data(**data))
 
         return JsonResponse({
             "success": True,
             "html": html,
         })
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.1/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.1/wagtail_fedit/views/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,36 +188,42 @@
                 "data-original-app": self.app_label,
                 "data-original-field": self.field_name,
                 "data-is-relation": self.meta_field.is_relation\
                     and isinstance(self.field_value, models.Model),
             },
             "meta_field": self.meta_field,
             "field_name": self.field_name,
+            "locked": self.lock is not None,
+            "locked_for_user": self.locked_for_user,
         }
 
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.form_class(request=request, instance=self.instance)
         return self.render_to_response(
-            self.get_context_data(form=form, locked=self.locked_for_user),
+            self.get_context_data(
+                form=form,
+            ),
             success=True,
         )
 
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, request=request, instance=self.instance)
         if not form.is_valid() or self.locked_for_user:
             return JsonResponse({
                 "success": False,
                 "errors": form.errors,
                 "locked": self.locked_for_user,
                 "html": render_to_string(
                     "wagtail_fedit/editor/field_iframe.html",
-                    context=self.get_context_data(form=form, locked=self.locked_for_user),
+                    context=self.get_context_data(
+                        form=form,
+                    ),
                     request=request,
                 )
             }, status=423 if self.locked_for_user else 400)
 
         
         self.instance = form.save()
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.1/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.0
+Version: 1.3.1
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -201,8 +201,11 @@
 
 ## Implemented
 
 * Revision Support
 * Locked Support
 * Draft Support
 * Preview Support
+* Workflow Support
+* Permissions
+* Audit Logs
 * Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.0 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.1 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -83,8 +83,9 @@
 model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
 is wrapped with `fedit_block` or `fedit_field` the field_name and model
 argument can be omitted. The parent- blocktag will share these variables
 through context. This makes it possibly to easily use editable sub-blocks
 across multiple different model types. If your model **ISN'T** capable of
 editing; or these variables aren't shared - your block will be rendered as
 normal. ## Implemented * Revision Support * Locked Support * Draft Support *
-Preview Support * Full block capabilities on Frontend Editing
+Preview Support * Workflow Support * Permissions * Audit Logs * Full block
+capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.3.0/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.1/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

