# Comparing `tmp/wagtail_fedit-1.2.9.tar.gz` & `tmp/wagtail_fedit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.9.tar", last modified: Fri Apr  5 12:47:43 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.0.tar", last modified: Fri Apr  5 12:55:06 2024, max compression
```

## Comparing `wagtail_fedit-1.2.9.tar` & `wagtail_fedit-1.3.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.128464 wagtail_fedit-1.2.9/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6742 2024-04-05 12:47:43.128464 wagtail_fedit-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5749 2024-04-05 11:07:38.000000 wagtail_fedit-1.2.9/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 12:47:43.138353 wagtail_fedit-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.751185 wagtail_fedit-1.2.9/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.803121 wagtail_fedit-1.2.9/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.2.9/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.808796 wagtail_fedit-1.2.9/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.809795 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.2.9/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.650472 wagtail_fedit-1.2.9/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.651665 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.841491 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.867745 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15212 2024-04-04 19:40:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.651665 wagtail_fedit-1.2.9/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.652983 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.880377 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.889069 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.902233 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     4890 2024-04-04 16:34:08.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.936429 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
--rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
--rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
--rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.964722 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.976285 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.005674 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.007672 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.011696 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16924 2024-04-04 19:49:27.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13828 2024-04-04 19:49:26.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.030270 wagtail_fedit-1.2.9/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.054257 wagtail_fedit-1.2.9/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.058248 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.085364 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/manage.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.106247 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.2.9/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.2.9/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.122929 wagtail_fedit-1.2.9/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9147 2024-04-05 12:45:56.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    11884 2024-04-05 12:45:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.127714 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.786106 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     6742 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3550 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.190174 wagtail_fedit-1.3.0/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7546 2024-04-05 12:55:06.188175 wagtail_fedit-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6496 2024-04-05 12:54:51.000000 wagtail_fedit-1.3.0/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 12:55:06.249926 wagtail_fedit-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.788661 wagtail_fedit-1.3.0/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.829831 wagtail_fedit-1.3.0/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.0/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.0/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.832829 wagtail_fedit-1.3.0/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.836837 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.0/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.735180 wagtail_fedit-1.3.0/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.737189 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.849722 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.855719 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15212 2024-04-04 19:40:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.739190 wagtail_fedit-1.3.0/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.741534 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.862628 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.871240 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.890683 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     4890 2024-04-04 16:34:08.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.900531 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
+-rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
+-rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.909489 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.911348 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.922173 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.933605 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.933605 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16924 2024-04-04 19:49:27.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13828 2024-04-04 19:49:26.000000 wagtail_fedit-1.3.0/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.957259 wagtail_fedit-1.3.0/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.967409 wagtail_fedit-1.3.0/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:05.985962 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.067163 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/manage.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.090072 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.0/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.0/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.108307 wagtail_fedit-1.3.0/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9147 2024-04-05 12:45:56.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    11884 2024-04-05 12:45:59.000000 wagtail_fedit-1.3.0/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.151471 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:55:06.183248 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7546 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3550 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 12:55:05.000000 wagtail_fedit-1.3.0/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.9/LICENSE` & `wagtail_fedit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/PKG-INFO` & `wagtail_fedit-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.9
+Version: 1.3.0
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 Getting Started
@@ -84,14 +86,16 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
+       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
+       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
        {% fedit_block block=block block_id=block.id field_name="content" model=self %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
@@ -101,15 +105,15 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
@@ -186,10 +190,19 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
 {% endfor %}
 ```
 
-## Settings
-
-## Models/Methods
+**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.  
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
+## Implemented
+
+* Revision Support
+* Locked Support
+* Draft Support
+* Preview Support
+* Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -1,51 +1,55 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.9 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.0 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
-============= Wagtail FEdit is a library to allow your Wagtail pages and
-content-blocks to be edited on the frontend. Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
-INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
-inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
-for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
-{# Load the required template tag libraries #}
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
+FEdit is a library to allow your Wagtail pages and content-blocks to be edited
+on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
+INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
+] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
+the models you wish to edit inherit from PreviewableMixin. **This is a
+requirement.** 2. Define a template for your model. Example: ```django-html {%
+load fedit static wagtailuserbar %} {# Load the required template tag libraries
+#}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
 #} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {% fedit_block block=block
-block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
-from django.template.loader import render_to_string ... class MyPage(...): #
-Can be any type of model. content = StreamField(...) def render_fedit_content
-(self, request): return render_to_string("myapp/render_my_field.html",
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
+do not require the field_name or model argument. #} {# This is taken from the
+parent (also wrapped by `fedit_block`); the model and field name are shared
+through context. #} {% fedit_block block=block block_id=block.id
+field_name="content" model=self %} {% endfor %} ``` ```python from
+django.template.loader import render_to_string ... class MyPage(...): # Can be
+any type of model. content = StreamField(...) def render_fedit_content(self,
+request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
 **But wait?! I go to my template and I do not see a way to edit!**That is true!
 We try to protect any styling on your actual page; we do not want to
 interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
-that userbar! It is also used for publishing if your model inherits from
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
 `DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
 **The `Page` model already provides this interface.** We have the following
 basic permission requirements: * You must have `wagtailadmin.access_admin` to
 edit a block/field. * You must have the appropriate `app_label.change_*`
 permission for the model. This however only applies to editing. We use separate
 permissions for publishing and submitting workflows, etc. Models which you want
 to allow the publish view for should also implement a `PermissionTester`- like
@@ -72,8 +76,15 @@
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
 Field name and model are the same arguments as in the first example! #} {%
 fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` ## Settings ## Models/Methods
+model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
+is wrapped with `fedit_block` or `fedit_field` the field_name and model
+argument can be omitted. The parent- blocktag will share these variables
+through context. This makes it possibly to easily use editable sub-blocks
+across multiple different model types. If your model **ISN'T** capable of
+editing; or these variables aren't shared - your block will be rendered as
+normal. ## Implemented * Revision Support * Locked Support * Draft Support *
+Preview Support * Full block capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.2.9/README.md` & `wagtail_fedit-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
+       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
+       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
        {% fedit_block block=block block_id=block.id field_name="content" model=self %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
@@ -76,15 +78,15 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
@@ -161,10 +163,19 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
 {% endfor %}
 ```
 
-## Settings
-
-## Models/Methods
+**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.  
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
+## Implemented
+
+* Revision Support
+* Locked Support
+* Draft Support
+* Preview Support
+* Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -13,26 +13,29 @@
 #} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {% fedit_block block=block
-block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
-from django.template.loader import render_to_string ... class MyPage(...): #
-Can be any type of model. content = StreamField(...) def render_fedit_content
-(self, request): return render_to_string("myapp/render_my_field.html",
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
+do not require the field_name or model argument. #} {# This is taken from the
+parent (also wrapped by `fedit_block`); the model and field name are shared
+through context. #} {% fedit_block block=block block_id=block.id
+field_name="content" model=self %} {% endfor %} ``` ```python from
+django.template.loader import render_to_string ... class MyPage(...): # Can be
+any type of model. content = StreamField(...) def render_fedit_content(self,
+request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
 **But wait?! I go to my template and I do not see a way to edit!**That is true!
 We try to protect any styling on your actual page; we do not want to
 interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
-that userbar! It is also used for publishing if your model inherits from
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
 `DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
 **The `Page` model already provides this interface.** We have the following
 basic permission requirements: * You must have `wagtailadmin.access_admin` to
 edit a block/field. * You must have the appropriate `app_label.change_*`
 permission for the model. This however only applies to editing. We use separate
 permissions for publishing and submitting workflows, etc. Models which you want
 to allow the publish view for should also implement a `PermissionTester`- like
@@ -59,8 +62,15 @@
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
 Field name and model are the same arguments as in the first example! #} {%
 fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` ## Settings ## Models/Methods
+model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
+is wrapped with `fedit_block` or `fedit_field` the field_name and model
+argument can be omitted. The parent- blocktag will share these variables
+through context. This makes it possibly to easily use editable sub-blocks
+across multiple different model types. If your model **ISN'T** capable of
+editing; or these variables aren't shared - your block will be rendered as
+normal. ## Implemented * Revision Support * Locked Support * Draft Support *
+Preview Support * Full block capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.2.9/setup.cfg` & `wagtail_fedit-1.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
+00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.0/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.0/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.0/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/models.py` & `wagtail_fedit-1.3.0/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.0/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.0/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/settings.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.0/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.0/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.0/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.0/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.0/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.0/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.0/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.0/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.0/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-fedit
-Version: 1.2.9
+Name: wagtail_fedit
+Version: 1.3.0
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,14 +18,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 Getting Started
@@ -84,14 +86,16 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
+       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
+       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
        {% fedit_block block=block block_id=block.id field_name="content" model=self %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
@@ -101,15 +105,15 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
@@ -186,10 +190,19 @@
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
 {% endfor %}
 ```
 
-## Settings
-
-## Models/Methods
+**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.  
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
+## Implemented
+
+* Revision Support
+* Locked Support
+* Draft Support
+* Preview Support
+* Full block capabilities on Frontend Editing
```

#### html2text {}

```diff
@@ -1,51 +1,55 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.2.9 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.0 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier:
 Topic :: Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
-============= Wagtail FEdit is a library to allow your Wagtail pages and
-content-blocks to be edited on the frontend. Getting Started --------------- 1.
-Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
-INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
-collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
-inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
-for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
-{# Load the required template tag libraries #}
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
+FEdit is a library to allow your Wagtail pages and content-blocks to be edited
+on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
+INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
+] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
+the models you wish to edit inherit from PreviewableMixin. **This is a
+requirement.** 2. Define a template for your model. Example: ```django-html {%
+load fedit static wagtailuserbar %} {# Load the required template tag libraries
+#}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
 #} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {% fedit_block block=block
-block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
-from django.template.loader import render_to_string ... class MyPage(...): #
-Can be any type of model. content = StreamField(...) def render_fedit_content
-(self, request): return render_to_string("myapp/render_my_field.html",
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
+do not require the field_name or model argument. #} {# This is taken from the
+parent (also wrapped by `fedit_block`); the model and field name are shared
+through context. #} {% fedit_block block=block block_id=block.id
+field_name="content" model=self %} {% endfor %} ``` ```python from
+django.template.loader import render_to_string ... class MyPage(...): # Can be
+any type of model. content = StreamField(...) def render_fedit_content(self,
+request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
 **But wait?! I go to my template and I do not see a way to edit!**That is true!
 We try to protect any styling on your actual page; we do not want to
 interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
-that userbar! It is also used for publishing if your model inherits from
+accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
+on that userbar! It is also used for publishing if your model inherits from
 `DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
 **The `Page` model already provides this interface.** We have the following
 basic permission requirements: * You must have `wagtailadmin.access_admin` to
 edit a block/field. * You must have the appropriate `app_label.change_*`
 permission for the model. This however only applies to editing. We use separate
 permissions for publishing and submitting workflows, etc. Models which you want
 to allow the publish view for should also implement a `PermissionTester`- like
@@ -72,8 +76,15 @@
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
 Field name and model are the same arguments as in the first example! #} {%
 fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` ## Settings ## Models/Methods
+model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
+is wrapped with `fedit_block` or `fedit_field` the field_name and model
+argument can be omitted. The parent- blocktag will share these variables
+through context. This makes it possibly to easily use editable sub-blocks
+across multiple different model types. If your model **ISN'T** capable of
+editing; or these variables aren't shared - your block will be rendered as
+normal. ## Implemented * Revision Support * Locked Support * Draft Support *
+Preview Support * Full block capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.2.9/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.0/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

