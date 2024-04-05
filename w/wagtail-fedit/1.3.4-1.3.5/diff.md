# Comparing `tmp/wagtail_fedit-1.3.4.tar.gz` & `tmp/wagtail_fedit-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.3.4.tar", last modified: Fri Apr  5 19:47:02 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.3.5.tar", last modified: Fri Apr  5 20:33:32 2024, max compression
```

## Comparing `wagtail_fedit-1.3.4.tar` & `wagtail_fedit-1.3.5.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.513699 wagtail_fedit-1.3.4/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7538 2024-04-05 19:47:02.513756 wagtail_fedit-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.4/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-05 19:47:02.523951 wagtail_fedit-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.345328 wagtail_fedit-1.3.4/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.366033 wagtail_fedit-1.3.4/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.4/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.4/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.367262 wagtail_fedit-1.3.4/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.368272 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.3.4/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.322092 wagtail_fedit-1.3.4/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.322092 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.374368 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.395823 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.323464 wagtail_fedit-1.3.4/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.323464 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.398816 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.403076 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.410734 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.417711 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.418707 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.423670 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
--rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
--rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
--rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
--rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.424719 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.426859 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.4/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.428119 wagtail_fedit-1.3.4/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.432129 wagtail_fedit-1.3.4/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.436132 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.466637 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.472164 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.4/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.4/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.4/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.506247 wagtail_fedit-1.3.4/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    14013 2024-04-05 19:46:41.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.4/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.512612 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:47:02.363790 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     7538 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3454 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 19:47:02.000000 wagtail_fedit-1.3.4/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.311415 wagtail_fedit-1.3.5/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7538 2024-04-05 20:33:32.311737 wagtail_fedit-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6545 2024-04-05 12:55:52.000000 wagtail_fedit-1.3.5/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 20:33:32.324478 wagtail_fedit-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.175448 wagtail_fedit-1.3.5/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.5/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.5/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.5/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.226810 wagtail_fedit-1.3.5/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.3.5/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.3.5/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.3.5/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.3.5/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.228062 wagtail_fedit-1.3.5/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.3.5/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.229800 wagtail_fedit-1.3.5/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.5/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.3.5/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.144749 wagtail_fedit-1.3.5/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.146177 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.233805 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.235806 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15348 2024-04-05 19:37:06.000000 wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.148248 wagtail_fedit-1.3.5/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.150422 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.238806 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.241614 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.248336 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     1709 2024-04-05 19:42:54.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     5895 2024-04-05 13:08:07.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.251336 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.252335 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.256028 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      707 2024-04-05 19:29:33.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1138 2024-04-05 19:27:36.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      873 2024-04-05 19:27:43.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1327 2024-04-05 19:27:54.000000 wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.259004 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.262200 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16806 2024-04-05 13:37:38.000000 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13783 2024-04-05 13:37:37.000000 wagtail_fedit-1.3.5/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.264896 wagtail_fedit-1.3.5/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.268048 wagtail_fedit-1.3.5/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.274971 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.282535 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6996 2024-04-05 20:03:30.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4318 2024-04-05 17:59:43.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     2680 2024-04-05 20:32:06.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.287693 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.3.5/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1051 2024-04-05 18:53:10.000000 wagtail_fedit-1.3.5/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.3.5/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.302516 wagtail_fedit-1.3.5/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.3.5/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9406 2024-04-05 18:01:17.000000 wagtail_fedit-1.3.5/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    14326 2024-04-05 20:33:13.000000 wagtail_fedit-1.3.5/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12150 2024-04-05 18:01:07.000000 wagtail_fedit-1.3.5/wagtail_fedit/views/fields.py
+-rw-rw-rw-   0        0        0     1456 2024-04-05 18:16:06.000000 wagtail_fedit-1.3.5/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.310434 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     6540 2024-04-05 18:52:00.000000 wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 20:33:32.223100 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     7538 2024-04-05 20:33:32.000000 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3499 2024-04-05 20:33:32.000000 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:33:32.000000 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 20:33:32.000000 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 20:33:32.000000 wagtail_fedit-1.3.5/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.3.4/LICENSE` & `wagtail_fedit-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/PKG-INFO` & `wagtail_fedit-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.3.4
+Version: 1.3.5
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.4 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.3.5 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.4/README.md` & `wagtail_fedit-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/setup.cfg` & `wagtail_fedit-1.3.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
-00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.3.5/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.3.5/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/hooks.py` & `wagtail_fedit-1.3.5/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/models.py` & `wagtail_fedit-1.3.5/wagtail_fedit/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,27 @@
         raise NotImplementedError("get_url must be implemented by subclasses; it should return the URL of the object on the frontend site.")
     
     def get_permissions_policy(self):
         return ModelPermissionPolicy(self.__class__)
     
     def permissions_for_user(self, user):
         return FeditPermissionTester(
-            model=self,
+            self,
             user=user,
             policy=self.get_permissions_policy()
         )
 
 
 class FeditPermissionTester:
     model: Type[FEditableMixin]
     
     def __init__(self, model_instance, user, policy = Type[ModelPermissionPolicy]):
         self.user = user
         self.model = model_instance.__class__
-        self.policy: ModelPermissionPolicy = policy(model=self.model)
+        self.policy: ModelPermissionPolicy = policy
         self.model_instance: FEditableMixin = model_instance
 
         # From wagtail.models.PagePermissionTester.__init__
         if self.user.is_active and not self.user.is_superuser:
             self.permissions = {
                 # Get the 'action' part of the permission codename, e.g.
                 # 'add' instead of 'add_page'
@@ -82,18 +82,17 @@
 
         if self.is_root():
             return False
 
         return self.user.is_superuser or ("publish" in self.permissions)
     
     def can_submit_for_moderation(self):
-        if not isinstance(self.model_instance, LockableMixin):
-            return False
-        
-        if not isinstance(self.model_instance, WorkflowMixin):
+        if not isinstance(self.model_instance, WorkflowMixin)\
+            and not isinstance(self.model_instance, LockableMixin):
             return False
 
         return (
             not self.is_locked()
             and self.model_instance.has_workflow
             and not self.model_instance.workflow_in_progress
         )
+
```

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.3.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.3.5/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.3.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.3.5/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.test import TestCase
 from django.db import models
 from django.urls import reverse
+from django.test import RequestFactory
 from django.contrib.auth.models import (
     User,
     Permission,
 )
 from ..models import (
     BasicModel,
     EditableFullModel,
@@ -108,14 +109,16 @@
 class BaseFEditTest(TestCase):
     # Block ID for a sub-block present in test data.
     BLOCK_ID = "c757f54d-0df5-4b35-8a06-4174f180ec41"
     
     def setUp(self):
         super().setUp()
 
+        self.request_factory = RequestFactory()
+
         self.full_model = EditableFullModel.objects.create(
             title="Full Model",
             body="Full Model Body",
             content=TEST_BLOCK_DATA,
         )
         self.draft_model = EditableDraftModel.objects.create(
             title="Draft Model",
@@ -183,26 +186,24 @@
             kwargs={
                 "object_id": object_id,
                 "app_label": app_label,
                 "model_name": model_name
             }
         )
 
-    def get_publish_url(self, object_id, app_label, model_name):
-        url_name = "publish"
+    def get_url_for(self, url_name, app_label, model_name, model_id):
         return reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
-                "object_id": object_id,
+                "object_id": model_id,
                 "app_label": app_label,
-                "model_name": model_name
+                "model_name": model_name,
             }
         )
 
-
     def get_field_url(self, field_name, app_label, model_name, model_id):
         url_name = "edit_field"
         return reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
                 "field_name": field_name,
                 "app_label": app_label,
```

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.3.5/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.3.5/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/urls.py` & `wagtail_fedit-1.3.5/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/utils.py` & `wagtail_fedit-1.3.5/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.3.5/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.3.5/wagtail_fedit/views/editable.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,26 +127,14 @@
         return self.title_format.format(self.object)
     
     def get_action_help_text_title(self) -> str:
         return self.action_help_text_title
     
     def get_action_help_text(self) -> str:
         return self.action_help_text
-
-    def redirect_to_success_url(self, request: HttpRequest) -> HttpResponse:
-        if hasattr(self.object, "get_url"):
-            return redirect(self.object.get_url(request))
-        
-        elif hasattr(self.object, "get_absolute_url"):
-            return redirect(self.object.get_absolute_url())
-        
-        return redirect(reverse(
-            "wagtail_fedit:editable",
-            args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
-        ))
     
     def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
         super().setup(request, object_id, app_label, model_name)
         self.policy = self.object.permissions_for_user(request.user)
 
         if not isinstance(self.object, tuple(self.required_superclasses)):
             self.error_response = HttpResponseBadRequest(
@@ -164,14 +152,26 @@
             "action_help_text": self.get_action_help_text(),
             "cancel_url": reverse(
                 "wagtail_fedit:editable",
                 args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
             ),
         }
 
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
     def redirect_to_failsafe_url(self, request: HttpRequest) -> HttpResponse:
         try:
             finder = AdminURLFinder(request.user)
             edit_url = finder.get_edit_url(self.object)
             return redirect(edit_url)
         except Exception:
             return redirect(reverse(
@@ -215,15 +215,15 @@
             messages.error(request, _("Invalid action specified: {}").format(request.POST["action"]))
             return self.get(request, *args, **kwargs)
         
         return self.action(request)
 
 
 class PublishView(BaseActionView):
-    required_superclasses = [DraftStateMixin]
+    required_superclasses = [DraftStateMixin, RevisionMixin]
     action_text = _("Publish")
 
     def get_action_title(self):
         return _("Publishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
 
     def get_action_help_text_title(self):
         return _("About publishing")
@@ -243,17 +243,20 @@
         if not policy.can_publish():
             raise ValueError("User does not have permission to publish")
         
         if not self.object.has_unpublished_changes:
             raise ValueError("Object has no unpublished changes")
 
     def action(self, request: HttpRequest) -> HttpResponse:
-        latest_revision = None
-        if isinstance(self.object, RevisionMixin):
-            latest_revision = self.object.latest_revision
+        latest_revision = self.object.latest_revision
+
+        if not latest_revision:
+            latest_revision = self.object.save_revision(
+                user=request.user,
+            )
 
         action = get_publish_action(self.object)(
             revision=latest_revision,
             user=request.user,
         )
 
         action.execute()
@@ -296,15 +299,15 @@
 
         action.execute()
 
         return self.redirect_to_failsafe_url(request)
 
 
 class SubmitView(BaseActionView):
-    required_superclasses = [DraftStateMixin, WorkflowMixin]
+    required_superclasses = [DraftStateMixin, WorkflowMixin, RevisionMixin]
     action_text = _("Submit for moderation")
     action_help_text_title = _("About submitting for moderation")
     action_help_text = [
         _("Submitting this object for moderation will make it invisible to users on the site."),
         _("That means that it will no longer be visible to anyone."),
         _("You can always choose to publish it again."),
     ]
@@ -316,14 +319,21 @@
         if not policy.can_submit_for_moderation():
             raise ValueError("User does not have permission to submit for moderation")
         
         if not self.object.has_unpublished_changes:
             raise ValueError("Object has no unpublished changes")
    
     def action(self, request: HttpRequest) -> HttpResponse:
+        
+        latest_revision = getattr(self.object, "latest_revision", None)
+        if not latest_revision:
+            latest_revision = self.object.save_revision(
+                user=request.user,
+            )
+
         if (
             self.workflow_state
             and self.workflow_state.status == WorkflowState.STATUS_NEEDS_CHANGES
         ):
             # If the workflow was in the needs changes state, resume the existing workflow on submission
             self.workflow_state.resume(self.request.user)
         else:
```

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.3.5/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.3.5/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.3.5/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.3.5/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.3.4
+Version: 1.3.5
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
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.4 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.3.5 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.3.4/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.3.5/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
 wagtail_fedit/test/core/tests/test_block_edit.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
 wagtail_fedit/test/core/tests/test_revision.py
+wagtail_fedit/test/core/tests/test_submit.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/blocks.py
```

