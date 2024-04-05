# Comparing `tmp/wagtail_fedit-1.3.1.tar.gz` & `tmp/wagtail_fedit-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.1.tar", last modified: Fri Apr  5 13:39:17 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.2.tar", last modified: Fri Apr  5 18:01:52 2024, max compression
```

## Comparing `wagtail_fedit-1.3.1.tar` & `wagtail_fedit-1.3.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.708294 wagtail_fedit-1.3.1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7595 2024-04-05 13:39:17.707295 wagtail_fedit-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 13:39:17.721958 wagtail_fedit-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.249475 wagtail_fedit-1.3.1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.303944 wagtail_fedit-1.3.1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.304943 wagtail_fedit-1.3.1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.305965 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.1/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.200035 wagtail_fedit-1.3.1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.201515 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.340990 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.366936 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15212 2024-04-05 13:21:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.202525 wagtail_fedit-1.3.1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.204977 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.384954 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.408508 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.454459 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.483461 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
--rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
--rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
--rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.507071 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.520068 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.549929 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.551930 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.554317 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.580280 wagtail_fedit-1.3.1/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.610414 wagtail_fedit-1.3.1/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.615378 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.675804 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/manage.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.687632 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.700297 wagtail_fedit-1.3.1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9276 2024-04-05 13:38:18.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12008 2024-04-05 13:08:52.000000 wagtail_fedit-1.3.1/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.706294 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:39:17.707295 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7595 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3550 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 13:39:17.000000 wagtail_fedit-1.3.1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7538 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 18:01:52.440832 wagtail_fedit-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.333047 wagtail_fedit-1.3.2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.363707 wagtail_fedit-1.3.2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.364639 wagtail_fedit-1.3.2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.367684 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.2/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.302994 wagtail_fedit-1.3.2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.304376 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.371779 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.372854 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15212 2024-04-05 13:21:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.305377 wagtail_fedit-1.3.2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.308360 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.374840 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.375963 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.381232 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.386714 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
+-rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
+-rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.388388 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.389387 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.391473 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.393852 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.397168 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.400008 wagtail_fedit-1.3.2/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.402022 wagtail_fedit-1.3.2/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.408783 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.413606 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.420119 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.3.2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.423462 wagtail_fedit-1.3.2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    12202 2024-04-05 14:30:59.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.2/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.428298 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:01:52.360380 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7538 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3558 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 18:01:52.000000 wagtail_fedit-1.3.2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.1/LICENSE` & `wagtail_fedit-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/PKG-INFO` & `wagtail_fedit-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.1
+Version: 1.3.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,16 +18,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 Getting Started
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.2 Summary: An
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
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
-FEdit is a library to allow your Wagtail pages and content-blocks to be edited
-on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
-INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
-] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
-the models you wish to edit inherit from PreviewableMixin. **This is a
-requirement.** 2. Define a template for your model. Example: ```django-html {%
-load fedit static wagtailuserbar %} {# Load the required template tag libraries
-#}
+Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
+============= Wagtail FEdit is a library to allow your Wagtail pages and
+content-blocks to be edited on the frontend. Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
+collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
+inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
 #} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
```

### Comparing `wagtail_fedit-1.3.1/README.md` & `wagtail_fedit-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/setup.cfg` & `wagtail_fedit-1.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
+00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/models.py` & `wagtail_fedit-1.3.2/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.2/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                     model.pk,
                 ),
                 {
                     "content": f"{model.content} test case {i + 1}"
                 }
             )
 
-            self.assertEqual(response.status_code, 403)
+            self.assertEqual(response.status_code, 403, msg=f"Expected 403, got {response.status_code} ({response.content})")
 
             model.refresh_from_db()
 
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 0)
                 chk = model
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                     model.pk,
                 ),
                 {
                     "title": f"{model.title} test case {i + 1}"
                 }
             )
 
-            self.assertEqual(response.status_code, 403)
+            self.assertEqual(response.status_code, 403, msg=f"Expected 403, got {response.status_code} ({response.content})")
 
             model.refresh_from_db()
 
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 0)
                 chk = model
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'wagtail_fedit.test.settings')
+    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'wagtail_fedit.test.testapp.settings')
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/settings.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.2/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.2/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.2/wagtail_fedit/views/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.utils.decorators import method_decorator
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import View
 from django.urls import reverse
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
+    HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
 )
 from django.apps import apps
 
 from wagtail.fields import StreamValue
 from wagtail.models import RevisionMixin, Page
@@ -41,18 +42,20 @@
         self.model_name = model_name
         self.app_label = app_label
         if "has_block" in request.GET:
             self.has_block = BlockEditNode.unpack("has_block", request=request)["has_block"].lower() == "true"
         else:
             self.has_block = False
 
-
-        self.model = apps.get_model(self.app_label, self.model_name)
-        if not self.has_perms(request, self.model):
-            return HttpResponseBadRequest("You do not have permission to view this page")
+        try:
+            self.model = apps.get_model(app_label, model_name)
+            if not self.has_perms(request, self.model):
+                return HttpResponseForbidden("You do not have permission to view this page")
+        except LookupError:
+            return HttpResponseBadRequest("Invalid model")
 
 
         self.model_instance = self.model._default_manager.get(pk=self.model_id)
         if issubclass(self.model, RevisionMixin) and self.model_instance.latest_revision_id:
             self.instance = self.model_instance.latest_revision.as_object()
         else:
             self.instance = self.model_instance
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.2/wagtail_fedit/views/editable.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,18 @@
         return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=self.check_for_changes)
 
 class BaseFeditView(FeditPermissionCheck, TemplateView):
     def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         try:
             self.model = apps.get_model(app_label, model_name)
             self.model_object = self.model._default_manager.get(pk=object_id)
-        except (self.model.DoesNotExist, LookupError):
+        except (LookupError):
             return HttpResponseBadRequest("Invalid model provided")
+        except (self.model.DoesNotExist):
+            return HttpResponseBadRequest("Model not found")
 
         if not self.has_perms(request, self.model):
             return HttpResponseForbidden("You do not have permission to view this page")
 
         if issubclass(self.model, RevisionMixin) and self.model_object.latest_revision_id:
             instance: RevisionMixin  = self.model_object
             revision: RevisionMixin = instance.latest_revision
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.2/wagtail_fedit/views/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,20 @@
     template_name = "wagtail_fedit/editor/field_iframe.html"
     ERROR_TITLE = _("Validation Errors")
 
     def dispatch(self, request: HttpRequest, field_name = None, app_label = None, model_name = None, model_id = None) -> None:
         if not all([field_name, model_name, app_label, model_id]):
             return HttpResponseBadRequest("Missing required parameters")
 
-        self.model = apps.get_model(app_label, model_name)
-        if not self.has_perms(request, self.model):
-            return HttpResponseForbidden("Permission denied")
+        try:
+            self.model = apps.get_model(app_label, model_name)
+            if not self.has_perms(request, self.model):
+                return HttpResponseForbidden("You do not have permission to view this page")
+        except LookupError:
+            return HttpResponseBadRequest("Invalid model")
 
         # Only fetch latest reivision if it exists
         # If not; it will be automatically created by the form.
         model_instance = self.model._default_manager.get(pk=model_id)
         if isinstance(model_instance, RevisionMixin) and model_instance.latest_revision_id:
             self.instance = model_instance.latest_revision.as_object()
         else:
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.3.1
+Name: wagtail-fedit
+Version: 1.3.2
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,16 +18,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=4.2
-Requires-Dist: Wagtail>=4.2
 
 wagtail_fedit
 =============
 
 Wagtail FEdit is a library to allow your Wagtail pages and content-blocks to be edited on the frontend.
 
 Getting Started
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.2 Summary: An
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
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-Django>=4.2 Requires-Dist: Wagtail>=4.2 wagtail_fedit ============= Wagtail
-FEdit is a library to allow your Wagtail pages and content-blocks to be edited
-on the frontend. Getting Started --------------- 1. Add 'wagtail_fedit' to your
-INSTALLED_APPS setting like this: ``` INSTALLED_APPS = [ ..., 'wagtail_fedit',
-] ``` 2. Run `py ./manage.py collectstatic`. ## Getting Editing! 1. Make sure
-the models you wish to edit inherit from PreviewableMixin. **This is a
-requirement.** 2. Define a template for your model. Example: ```django-html {%
-load fedit static wagtailuserbar %} {# Load the required template tag libraries
-#}
+Description-Content-Type: text/markdown License-File: LICENSE wagtail_fedit
+============= Wagtail FEdit is a library to allow your Wagtail pages and
+content-blocks to be edited on the frontend. Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
+collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
+inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Pass in the field_name and the model instance on which that field resides.
 #}
 ************ {{%% ffeeddiitt__ffiieelldd ""ttiittllee"" sseellff %%}} ************
 {# Pass in the field_name and the model instance on which that field resides.
 #} {% fedit_field "content" self %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
```

### Comparing `wagtail_fedit-1.3.1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
 wagtail_fedit/templatetags/__init__.py
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
 wagtail_fedit/test/__init__.py
 wagtail_fedit/test/manage.py
-wagtail_fedit/test/settings.py
 wagtail_fedit/test/core/__init__.py
 wagtail_fedit/test/core/apps.py
 wagtail_fedit/test/core/models.py
 wagtail_fedit/test/core/migrations/0001_initial.py
 wagtail_fedit/test/core/migrations/0002_basicmodel.py
 wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
 wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
@@ -63,14 +62,15 @@
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
 wagtail_fedit/test/core/tests/test_revision.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
+wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/blocks.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/fields.py
 wagtail_fedit/wagtail_hooks/__init__.py
```

