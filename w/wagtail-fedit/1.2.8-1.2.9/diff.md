# Comparing `tmp/wagtail_fedit-1.2.8.tar.gz` & `tmp/wagtail_fedit-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.8.tar", last modified: Thu Apr  4 08:37:23 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.9.tar", last modified: Fri Apr  5 12:47:43 2024, max compression
```

## Comparing `wagtail_fedit-1.2.8.tar` & `wagtail_fedit-1.2.9.tar`

### file list

```diff
@@ -1,94 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.8/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-04 08:37:23.149506 wagtail_fedit-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.917972 wagtail_fedit-1.2.8/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1387 2024-04-04 07:56:39.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.2.8/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.965635 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4597 2024-04-04 08:36:46.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.999014 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    12165 2024-04-03 20:03:43.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.016167 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.021161 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.043715 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3414 2024-04-04 08:31:26.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1283 2024-04-03 19:57:11.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1593 2024-04-04 08:07:32.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.060784 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.071859 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.074254 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16924 2024-04-03 19:52:53.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.085223 wagtail_fedit-1.2.8/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.8/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.8/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.8/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.8/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     8857 2024-04-04 08:33:38.000000 wagtail_fedit-1.2.8/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.113138 wagtail_fedit-1.2.8/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8783 2024-04-04 08:12:17.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12186 2024-04-04 08:33:10.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3204 2024-04-04 07:53:17.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.128464 wagtail_fedit-1.2.9/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6742 2024-04-05 12:47:43.128464 wagtail_fedit-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5749 2024-04-05 11:07:38.000000 wagtail_fedit-1.2.9/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-05 12:47:43.138353 wagtail_fedit-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.751185 wagtail_fedit-1.2.9/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.803121 wagtail_fedit-1.2.9/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.2.9/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.2.9/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.808796 wagtail_fedit-1.2.9/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.809795 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3219 2024-04-05 07:50:20.000000 wagtail_fedit-1.2.9/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.650472 wagtail_fedit-1.2.9/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.651665 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.841491 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4852 2024-04-04 16:51:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0      761 2024-04-04 19:41:08.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.867745 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    15212 2024-04-04 19:40:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.651665 wagtail_fedit-1.2.9/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.652983 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.880377 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.889069 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.902233 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     4890 2024-04-04 16:34:08.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      826 2024-04-04 16:21:51.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.936429 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/
+-rw-rw-rw-   0        0        0      656 2024-04-04 19:58:15.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:57:54.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
+-rw-rw-rw-   0        0        0      865 2024-04-04 19:58:20.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1375 2024-04-04 19:33:39.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.964722 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.976285 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.005674 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/
+-rw-rw-rw-   0        0        0      709 2024-04-04 19:41:32.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+-rw-rw-rw-   0        0        0     1140 2024-04-04 19:41:35.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+-rw-rw-rw-   0        0        0      875 2024-04-04 19:41:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
+-rw-rw-rw-   0        0        0     1529 2024-04-04 19:38:34.000000 wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.007672 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.011696 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16924 2024-04-04 19:49:27.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13828 2024-04-04 19:49:26.000000 wagtail_fedit-1.2.9/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.030270 wagtail_fedit-1.2.9/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.054257 wagtail_fedit-1.2.9/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.058248 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3145 2024-04-05 12:28:28.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.085364 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     6932 2024-04-05 12:43:52.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4248 2024-04-05 12:46:12.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3572 2024-04-05 12:46:14.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0      696 2024-04-05 08:39:46.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/manage.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 08:43:15.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.106247 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      644 2024-04-05 08:09:30.000000 wagtail_fedit-1.2.9/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    11047 2024-04-05 11:55:37.000000 wagtail_fedit-1.2.9/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.122929 wagtail_fedit-1.2.9/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9147 2024-04-05 12:45:56.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0    12122 2024-04-05 11:56:25.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    11884 2024-04-05 12:45:59.000000 wagtail_fedit-1.2.9/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:43.127714 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     5451 2024-04-04 19:59:02.000000 wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-05 12:47:42.786106 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     6742 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3550 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 12:47:42.000000 wagtail_fedit-1.2.9/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.8/LICENSE` & `wagtail_fedit-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/PKG-INFO` & `wagtail_fedit-1.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.8
+Version: 1.2.9
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
@@ -103,26 +101,65 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+
+## Permissions
+
+**Note: This is not required for pages.**
+
+**The `Page` model already provides this interface.**
+
+We have the following basic permission requirements:
+
+* You must have `wagtailadmin.access_admin` to edit a block/field.
+* You must have the appropriate `app_label.change_*` permission for the model.
+
+This however only applies to editing.
+
+We use separate permissions for publishing and submitting workflows, etc.
+
+Models which you want to allow the publish view for should also implement a `PermissionTester`- like object.
+
+Example of how you should implement the `Tester` object and all required permissions. (More details in `models.py`)
+
+```python
+
+class MyModel(...):
+    def permissions_for_user(self, user):
+        return MyModelPermissionTester(self, user)
+
+class MyModelPermissionTester(...):
+    def can_unpublish(self):
+        """ Can the user unpublish this object? (Required for un-publishing"""
+  
+    def can_publish(self):
+        """ Can the user publish this object? (Required for publishing)"""  
+  
+    def can_submit_for_moderation(self):
+        """ Can the user submit this object for moderation? (Optional) """
+
+```
 
-4. **But wait?! I go to my template and I do not see a way to edit!**  
-   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
-   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
-   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
-   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
+## Workflows
+
+We include a `WorkFlow` to submit this object for moderation.
+
+More workflow support will be included in the future.
+
 ## Logs
 
 Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.8 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.9 Summary: An
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
@@ -34,28 +33,44 @@
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!** That is
-true! We try to protect any styling on your actual page; we do not want to
-interfere. Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
-your model inherits from a `RevisionMixin`, we will automatically create drafts
-for you. These will not be published (If the model inherits from
-`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
-out of the box. We will automatically update your model's history; including
-possible revisions. This will allow you to backtrack each change made on the
-frontend. This however does mean that a possibly large amount of data will be
-stored in your database. ## Caveats Wagtail does not always make it's `id`
-attribute available. This is only available to instances of `StreamChild` and
+**But wait?! I go to my template and I do not see a way to edit!**That is true!
+We try to protect any styling on your actual page; we do not want to
+interfere.Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
+that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
+**The `Page` model already provides this interface.** We have the following
+basic permission requirements: * You must have `wagtailadmin.access_admin` to
+edit a block/field. * You must have the appropriate `app_label.change_*`
+permission for the model. This however only applies to editing. We use separate
+permissions for publishing and submitting workflows, etc. Models which you want
+to allow the publish view for should also implement a `PermissionTester`- like
+object. Example of how you should implement the `Tester` object and all
+required permissions. (More details in `models.py`) ```python class MyModel
+(...): def permissions_for_user(self, user): return MyModelPermissionTester
+(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
+Can the user unpublish this object? (Required for un-publishing""" def
+can_publish(self): """ Can the user publish this object? (Required for
+publishing)""" def can_submit_for_moderation(self): """ Can the user submit
+this object for moderation? (Optional) """ ``` ## Revisions Revision support is
+included out of the box. If your model inherits from a `RevisionMixin`, we will
+automatically create drafts for you. These will not be published (If the model
+inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
+include a `WorkFlow` to submit this object for moderation. More workflow
+support will be included in the future. ## Logs Logs are also included out of
+the box. We will automatically update your model's history; including possible
+revisions. This will allow you to backtrack each change made on the frontend.
+This however does mean that a possibly large amount of data will be stored in
+your database. ## Caveats Wagtail does not always make it's `id` attribute
+available. This is only available to instances of `StreamChild` and
 `ListChild`. Consider the following regular wagtail list loop where `items` is
 a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
```

### Comparing `wagtail_fedit-1.2.8/README.md` & `wagtail_fedit-1.2.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -76,26 +76,65 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+
+## Permissions
+
+**Note: This is not required for pages.**
+
+**The `Page` model already provides this interface.**
+
+We have the following basic permission requirements:
+
+* You must have `wagtailadmin.access_admin` to edit a block/field.
+* You must have the appropriate `app_label.change_*` permission for the model.
+
+This however only applies to editing.
+
+We use separate permissions for publishing and submitting workflows, etc.
+
+Models which you want to allow the publish view for should also implement a `PermissionTester`- like object.
+
+Example of how you should implement the `Tester` object and all required permissions. (More details in `models.py`)
+
+```python
+
+class MyModel(...):
+    def permissions_for_user(self, user):
+        return MyModelPermissionTester(self, user)
+
+class MyModelPermissionTester(...):
+    def can_unpublish(self):
+        """ Can the user unpublish this object? (Required for un-publishing"""
+  
+    def can_publish(self):
+        """ Can the user publish this object? (Required for publishing)"""  
+  
+    def can_submit_for_moderation(self):
+        """ Can the user submit this object for moderation? (Optional) """
+
+```
 
-4. **But wait?! I go to my template and I do not see a way to edit!**  
-   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
-   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
-   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
-   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
+## Workflows
+
+We include a `WorkFlow` to submit this object for moderation.
+
+More workflow support will be included in the future.
+
 ## Logs
 
 Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
```

#### html2text {}

```diff
@@ -20,28 +20,44 @@
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!** That is
-true! We try to protect any styling on your actual page; we do not want to
-interfere. Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
-your model inherits from a `RevisionMixin`, we will automatically create drafts
-for you. These will not be published (If the model inherits from
-`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
-out of the box. We will automatically update your model's history; including
-possible revisions. This will allow you to backtrack each change made on the
-frontend. This however does mean that a possibly large amount of data will be
-stored in your database. ## Caveats Wagtail does not always make it's `id`
-attribute available. This is only available to instances of `StreamChild` and
+**But wait?! I go to my template and I do not see a way to edit!**That is true!
+We try to protect any styling on your actual page; we do not want to
+interfere.Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
+that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
+**The `Page` model already provides this interface.** We have the following
+basic permission requirements: * You must have `wagtailadmin.access_admin` to
+edit a block/field. * You must have the appropriate `app_label.change_*`
+permission for the model. This however only applies to editing. We use separate
+permissions for publishing and submitting workflows, etc. Models which you want
+to allow the publish view for should also implement a `PermissionTester`- like
+object. Example of how you should implement the `Tester` object and all
+required permissions. (More details in `models.py`) ```python class MyModel
+(...): def permissions_for_user(self, user): return MyModelPermissionTester
+(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
+Can the user unpublish this object? (Required for un-publishing""" def
+can_publish(self): """ Can the user publish this object? (Required for
+publishing)""" def can_submit_for_moderation(self): """ Can the user submit
+this object for moderation? (Optional) """ ``` ## Revisions Revision support is
+included out of the box. If your model inherits from a `RevisionMixin`, we will
+automatically create drafts for you. These will not be published (If the model
+inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
+include a `WorkFlow` to submit this object for moderation. More workflow
+support will be included in the future. ## Logs Logs are also included out of
+the box. We will automatically update your model's history; including possible
+revisions. This will allow you to backtrack each change made on the frontend.
+This however does mean that a possibly large amount of data will be stored in
+your database. ## Caveats Wagtail does not always make it's `id` attribute
+available. This is only available to instances of `StreamChild` and
 `ListChild`. Consider the following regular wagtail list loop where `items` is
 a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
```

### Comparing `wagtail_fedit-1.2.8/setup.cfg` & `wagtail_fedit-1.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
+00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.2.8/tests/testapp/manage.py` & `wagtail_fedit-1.2.9/wagtail_fedit/test/manage.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'testapp.settings')
+    os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'wagtail_fedit.test.settings')
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `wagtail_fedit-1.2.8/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.9/wagtail_fedit/test/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 
 ALLOWED_HOSTS = []
 
 
 # Application definition
 
 INSTALLED_APPS = [
-    'core',
-
     'wagtail_fedit',
+    'wagtail_fedit.test.core',
 
     'wagtail',
     'wagtail.sites',
     'wagtail.users',
     'wagtail.admin',
     'wagtail.documents',
     'wagtail.images',
@@ -86,15 +85,15 @@
 
 # Database
 # https://docs.djangoproject.com/en/5.0/ref/settings/#databases
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': BASE_DIR / 'db.sqlite3',
+        'NAME': BASE_DIR  / 'test' / 'db.sqlite3',
     }
 }
 
 
 # Password validation
 # https://docs.djangoproject.com/en/5.0/ref/settings/#auth-password-validators
```

### Comparing `wagtail_fedit-1.2.8/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.9/wagtail_fedit/test/testapp/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,12 +11,14 @@
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
-from django.urls import path
+from django.urls import path, include
+from wagtail.admin import urls as wagtailadmin_urls
 
 urlpatterns = [
-    path('admin/', admin.site.urls),
+    path('django/', admin.site.urls),
+    path('admin/', include(wagtailadmin_urls)),
 ]
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.9/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.9/wagtail_fedit/forms/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         )
         instance = instance.as_object()
     else:
         instance.save()
 
     return instance
 
-def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[WagtailAdminModelForm]:
+def get_form_class_for_fields(form_model: models.Model, form_fields: list[str]) -> Type[PossiblePreviewForm]:
 
     if hasattr(form_model, "get_fedit_form"):
         return form_model.get_fedit_form(form_fields)
 
     class Form(PossiblePreviewForm):
         class Meta:
             model = form_model
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.9/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 .wagtail-fedit-modal-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
     flex: 1;
 }
-.wagtail-fedit-modal-wrapper .wagtail-fedit-modal .wagtail-fedit-close-button {
+.wagtail-fedit-modal-wrapper .wagtail-fedit-close-button {
     position: absolute;
     right: 0;
     top: 0;
     text-align: center;
     vertical-align: middle;
     padding: 0;
     width: 28px;
@@ -154,11 +154,27 @@
     border: 1px solid rgb(172, 27, 27);
     border-right-width: 0;
     border-top-width: 0;
     background-color: rgb(255, 255, 255);
     color: rgb(172, 27, 27);
     cursor: pointer;
 }
-.wagtail-fedit-modal-wrapper .wagtail-fedit-modal .wagtail-fedit-close-button:hover {
+.wagtail-fedit-modal-wrapper .wagtail-fedit-close-button:hover {
     background-color: rgb(172, 27, 27);
     color: rgb(235, 235, 235);
+}
+
+.wagtail-fedit-banner-modal {
+    position: fixed;
+    bottom: 0;
+    left: 0;
+    width: 100%;
+    background-color: rgba(0, 0, 0, 0.5);
+    display: flex;
+    justify-content: center;
+    align-items: center;
+    z-index: 400;
+    overflow: auto;
+}
+.wagtail-fedit-banner-modal iframe {
+    min-height: 280px;
 }
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 .wagtail-fedit-form-wrapper form input {
     margin-bottom: 0.5em;
 }
 .wagtail-fedit-form-wrapper .wagtail-fedit-form {
     display: flex;
     flex-direction: column;
 }
+.wagtail-fedit-form-wrapper .wagtail-fedit-publish-form {
+    justify-content: center;
+}
 .wagtail-fedit-form-wrapper .buttons {
     display: flex;
     flex-direction: row;
     justify-content: flex-end;
     margin-top: auto;
     margin-bottom: 1em;
 }
@@ -129,14 +132,20 @@
     flex-direction: column;
     border-bottom: unset;
     overflow: hidden;
 }
 #djDebug {
     display: none;
 }
+#modal-header > #modal-title {
+    padding-left: 1.3rem;
+    text-wrap: nowrap;
+    text-overflow: ellipsis;
+    overflow: hidden;
+}
 #modal-header > #modal-title,
 #modal-header {
     background-color: var(--w-color-surface-menus);
     color: var(--w-color-text-label-menus-default);
     margin: 0;
     padding-top: 0.5em;
     padding-bottom: 0.5em;
@@ -146,14 +155,15 @@
     top: 0;
     left: 0;
     right: 0;
     z-index: 100;
 }
 #wagtail-fedit-help-text-section {
     margin-bottom: 0;
+    margin-top: 0.5em;
 }
 #wagtail-fedit-help-text-section .w-panel__anchor,
 #wagtail-fedit-editor-section .w-panel__anchor {
     display: none;
 }
 #wagtail-fedit-help-text-section .w-panel__toggle,
 #wagtail-fedit-editor-section .w-panel__toggle {
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -2,22 +2,24 @@
     constructor(options) {
         const {
             url,
             id,
             className,
             onLoad = () => {},
             onError = () => {},
+            onCancel = () => {},
         } = options;
 
 
         this.url = url;
         this.id = id;
         this.className = className;
         this.onLoad = onLoad;
         this.onError = onError;
+        this.onCancel = onCancel;
         this.render();
     }
 
     get element() {
         if (!this.iframe) {
             this.iframe = this._renderFrame(this.url, this.onLoad);
         }
@@ -67,25 +69,30 @@
 
     _renderFrame(url, onLoad, onError) {
         const iframe = document.createElement('iframe');
         iframe.src = url;
         iframe.id = this.id;
         iframe.className = this.className;
         iframe.onload = () => {
+            const cancelButton = this.document.querySelector(".wagtail-fedit-cancel-button");
+            if (cancelButton) {
+                cancelButton.addEventListener("click", this.onCancel);
+            }
             onLoad({
                 newFrame: iframe
             });
         };
         iframe.onerror = () => {
             onError();
         };
         return iframe;
     }
 }
 
+
 const modalHtml = `
 <div class="wagtail-fedit-modal-wrapper">
     <div class="wagtail-fedit-modal" id="wagtail-fedit-modal-__ID__-modal">
     </div>
 </div>`
 
 
@@ -174,27 +181,33 @@
                             this.iframe.formElement.onsubmit = onSubmit;
 
                             const uninitializedBlock = this.iframe.mainElement.querySelector("#value[data-block]");
                             if (uninitializedBlock) {
                                 this.iframe.window.initBlockWidget(uninitializedBlock.id);
                             }
 
-                            const cancelButton = this.iframe.document.querySelector("button.wagtail-fedit-cancel-button");
+                            const cancelButton = this.iframe.document.querySelector(".wagtail-fedit-cancel-button");
                             cancelButton.addEventListener("click", this.closeModal.bind(this));
                             return;
                         }
                         this.wrapperElement.style.display = "none";
                         this.setWrapperHtml(response.html);
                         this.initNewEditors();
                         this.closeModal();
+
+                        const event = new CustomEvent("wagtail-fedit:change", {
+                            detail: {
+                                element: this.wrapperElement,
+                            }
+                        });
+                        document.dispatchEvent(event);
                     });
                 };
-                const cancelButton = this.iframe.document.querySelector("button.wagtail-fedit-cancel-button");
-                cancelButton.addEventListener("click", this.closeModal.bind(this));
                 this.iframe.formElement.onsubmit = onSubmit;
+                this.iframe.onCancel = this.closeModal.bind(this);
 
                 // Check if we need to apply the fedit-full class to the modal
                 const formHeight = this.iframe.formElement.getBoundingClientRect().height;
                 const formWrapper = this.iframe.formWrapper;
                 if (
                     (formWrapper && (
                         formWrapper.classList.contains("fedit-full") ||
@@ -205,14 +218,20 @@
                     this.modal.classList.add("fedit-full");
                 }
 
                 const url = window.location.href.split("#")[0];
                 window.history.pushState(null, this.iframe.document.title, url + `#${this.wrapperElement.id}`);
                 document.title = this.iframe.document.title;
             },
+            onError: () => {
+                this.closeModal();
+            },
+            onCancel: () => {
+                this.closeModal();
+            },
         });
         this.modal.appendChild(this.iframe.element);
 
         const closeBtn = document.createElement("button");
         closeBtn.innerHTML = "&times;";
         closeBtn.classList.add("wagtail-fedit-close-button");
         closeBtn.addEventListener("click", this.closeModal.bind(this));
@@ -276,14 +295,77 @@
                     type: this.type
                 });
             }
         }
     }
 }
 
+class WagtailFeditPublishMenu {
+    constructor(publishButton) {
+        this.publishButton = publishButton;
+        this.publishForm = publishButton.parentElement.querySelector("form");
+        const buttons = this.publishForm.querySelectorAll("button");
+        let initialIsHidden = false;
+        for (const button of buttons) {
+            if (button.classList.contains("initially-hidden")) {
+                initialIsHidden = true;
+                break;
+            }
+        }
+
+        if (initialIsHidden) {
+            document.addEventListener("wagtail-fedit:change", (e) => {
+                for (const button of buttons) {
+                    if (button.classList.contains("initially-hidden")) {
+                        button.classList.remove("initially-hidden");
+                    }
+                }
+            })
+        }
+
+        this.init();
+    }
+
+    init() {
+        this.publishButton.addEventListener("click", (e) => {
+            if (this.publishForm.classList.contains("open")) {
+                const anim = this.publishForm.animate([{
+                    opacity: 1,
+                    height: `${this.publishForm.scrollHeight}px`
+                }, {
+                    opacity: 0,
+                    height: "0px"
+                }, ], {
+                    duration: 500,
+                    easing: "ease-in-out",
+                });
+                anim.onfinish = () => {
+                    this.publishForm.classList.remove("open");
+                };
+                return;
+            }
+            e.preventDefault();
+            e.stopPropagation();
+            const anim = this.publishForm.animate([{
+                opacity: 0,
+                height: "0px"
+            }, {
+                opacity: 1,
+                height: `${this.publishForm.scrollHeight}px`
+            }], {
+                duration: 500,
+                easing: "ease-in-out",
+            });
+            anim.onfinish = () => {
+                this.publishForm.classList.add("open");
+            };
+        });
+    }
+}
+
 function initFEditors() {
     const wagtailFeditBlockEditors = document.querySelectorAll(".wagtail-fedit-block-wrapper");
     const wagtailFeditFieldEditors = document.querySelectorAll(".wagtail-fedit-field-wrapper");
     for (const editor of wagtailFeditBlockEditors) {
         if (!editor.classList.contains("wagtail-fedit-initialized")) {
             editor.classList.add("wagtail-fedit-initialized");
             new WagtailFeditEditor({
@@ -326,14 +408,15 @@
         window.scrollTo(scrollX, scrollY);
     }
 
     const userbar = document.querySelector("wagtail-userbar");
     if (userbar) {
         const editButton = userbar.shadowRoot.querySelector("#wagtail-fedit-editor-button");
         const liveButton = userbar.shadowRoot.querySelector("#wagtail-fedit-live-button");
+        const publishMenu = userbar.shadowRoot.querySelector("#wagtail-fedit-publish-menu");
 
         function setScrollParams(button) {
             if (!button) {
                 return;
             }
             const url = new URL(button.href);
             if (window.scrollY > 100) {
@@ -342,21 +425,33 @@
             if (window.scrollX > 100) {
                 url.searchParams.set("scrollX", window.scrollX);
             }
             button.href = url.toString();
         }
 
         if (editButton || liveButton) {
-            window.addEventListener("scroll", () => {
-                setScrollParams(editButton);
-                setScrollParams(liveButton);
+            let timer = null;
 
-                const windowURL = new URL(window.location.href);
-                windowURL.searchParams.set("scrollY", window.scrollY);
-                windowURL.searchParams.set("scrollX", window.scrollX);
-                window.history.replaceState(null, "", windowURL.toString());
+            window.addEventListener("scroll", () => {
+                if (timer) {
+                    clearTimeout(timer);
+                }
+                timer = setTimeout(() => {
+                    setScrollParams(editButton);
+                    setScrollParams(liveButton);
+
+                    const windowURL = new URL(window.location.href);
+                    windowURL.searchParams.set("scrollY", window.scrollY);
+                    windowURL.searchParams.set("scrollX", window.scrollX);
+                    window.history.replaceState(null, "", windowURL.toString());
+                }, 50);
             });
         }
+
+
+        if (publishMenu) {
+            const publisher = new WagtailFeditPublishMenu(publishMenu);
+        }
     }
 }
 
 document.addEventListener("DOMContentLoaded", initFEditors);
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 24% similar despite different names*

```diff
@@ -8,60 +8,94 @@
 {{ form.media.css }}
 <link rel="stylesheet" href="{% static 'wagtail_fedit/css/furniture.css' %}">
 <base target="_blank">
 {% endblock %}
 
 {% block extra_js %}
 <script src="{% versioned_static 'wagtailadmin/js/modal-workflow.js' %}"></script>
-{% include "wagtailadmin/pages/_editor_js.html" %}
+{% block page_js %}{% include "wagtailadmin/pages/_editor_js.html" %}{% endblock %}
 {{ block.super }}
 {{ form.media.js }}
 {% endblock %}
 
 {% block furniture %}
+
     <main class="content-wrapper w-overflow-x-hidden" id="main">
         {% block header %}
-            <header class="nice-padding" id="modal-header">
+            <header id="modal-header">
                 <h1 id="modal-title">{{ view.get_header_title }}</h1>
             </header>
         {% endblock %}
+        <div class="messages" role="status">
+            {# Always show messages div so it can be appended to by JS #}
+            {% if messages or form.errors %}
+                <ul>
+                    {% if form.errors %}
+                        {% for error in form.non_field_errors %}
+                            <li class="error">{{ error }}</li>
+                        {% endfor %}
+                    {% endif %}
+                    {% for message in messages %}
+                        <li class="{{ message.tags }}">{{ message }}</li>
+                    {% endfor %}
+                </ul>
+            {% endif %}
+        </div>
+
         <div class="nice-padding">
+    
             {% if help_text %}
                 {% panel id="wagtail-fedit-help-text" icon="help" heading=help_text.heading %}
                     {% help_block status=help_text.status %}
                         <p><strong>{{ help_text.title }}</strong></p>
                         <p>{{ help_text.text }}</p>
                     {% endhelp_block %}
                 {% endpanel %}
             {% endif %}
-            {% block content %}{% endblock %}
-        </div>
-    </main>
-    <aside>
-        <div class="fedit-sidebar-logo">
-            {% block sidebar_logo %}{% endblock %}
-        </div>
-        <div class="fedit-sidebar">
-            {% block sidebar %}
-                {% if admin_edit_url %}
-                    <a href="{{ admin_edit_url }}" class="fedit-menu-item fedit-sidebar-icon" aria-label="{% translate "Edit in Wagtail Admin" %}" target="_blank">
-                        {% icon name="link-external" %}
-                    </a>
-                {% endif %}
-                <button type="submit" form="wagtail-fedit-form" class="fedit-menu-item fedit-sidebar-icon wagtail-fedit-save-button bottom" aria-label="{% translate "Save" %}">
-                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="icon" title="{% translate "Save" %}" viewBox="0 0 16 16">
-                        <!-- The MIT License (MIT) -->
-                        <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
-                        <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0m-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z"/>
-                    </svg>
-                </button>
-                <button type="button" class="fedit-menu-item fedit-sidebar-icon wagtail-fedit-cancel-button" aria-label="{% translate "Close" %}">
-                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="icon" title="{% translate "Close" %}" viewBox="0 0 16 16">
-                        <!-- The MIT License (MIT) -->
-                        <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
-                        <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0M5.354 4.646a.5.5 0 1 0-.708.708L7.293 8l-2.647 2.646a.5.5 0 0 0 .708.708L8 8.707l2.646 2.647a.5.5 0 0 0 .708-.708L8.707 8l2.647-2.646a.5.5 0 0 0-.708-.708L8 7.293z"/>
-                    </svg>
-                </button>
+            {% block content %}
+                {% block errors %}
+                    {% if form.errors or form.non_field_errors %}
+                        <div class="error-message">
+                            <h2>{{ view.get_error_title }}</h2>
+                            <ul>
+                                {% for error in form.non_field_errors %}
+                                    <li>{{ error }}</li>
+                                {% endfor %}
+                                {{ form.errors.as_ul }}
+                            </ul>
+                        </div>
+                    {% endif %}
+                {% endblock %}
             {% endblock %}
         </div>
-    </aside>
+    </main>
+    {% block sidebar_root %}
+        <aside>
+            <div class="fedit-sidebar-logo">
+                {% block sidebar_logo %}{% endblock %}
+            </div>
+            <div class="fedit-sidebar">
+                {% block sidebar %}
+                    {% if admin_edit_url %}
+                        <a href="{{ admin_edit_url }}" class="fedit-menu-item fedit-sidebar-icon" aria-label="{% translate "Edit in Wagtail Admin" %}" target="_blank">
+                            {% icon name="link-external" %}
+                        </a>
+                    {% endif %}
+                    <button type="submit" form="wagtail-fedit-form" class="fedit-menu-item fedit-sidebar-icon wagtail-fedit-save-button bottom" aria-label="{% translate "Save" %}">
+                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="icon" title="{% translate "Save" %}" viewBox="0 0 16 16">
+                            <!-- The MIT License (MIT) -->
+                            <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
+                            <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0m-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z"/>
+                        </svg>
+                    </button>
+                    <button type="button" class="fedit-menu-item fedit-sidebar-icon wagtail-fedit-cancel-button" aria-label="{% translate "Close" %}">
+                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="icon" title="{% translate "Close" %}" viewBox="0 0 16 16">
+                            <!-- The MIT License (MIT) -->
+                            <!-- Copyright (c) 2011-2024 The Bootstrap Authors -->
+                            <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0M5.354 4.646a.5.5 0 1 0-.708.708L7.293 8l-2.647 2.646a.5.5 0 0 0 .708.708L8 8.707l2.646 2.647a.5.5 0 0 0 .708-.708L8.707 8l2.647-2.646a.5.5 0 0 0-.708-.708L8 7.293z"/>
+                        </svg>
+                    </button>
+                {% endblock %}
+            </div>
+        </aside>
+    {% endblock %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,23 +1,38 @@
 {% extends "wagtailadmin/admin_base.html" %} {% load wagtailadmin_tags i18n
 static %} {% block titletag %}{{view.get_header_title}}{% endblock %} {% block
 extra_css %} {{ block.super }} {{ form.media.css }}
 {% endblock %} {% block extra_js %}
-{% include "wagtailadmin/pages/_editor_js.html" %} {{ block.super }} {
-{ form.media.js }} {% endblock %} {% block furniture %} {% block header %}
+{% block page_js %}{% include "wagtailadmin/pages/_editor_js.html" %}{%
+endblock %} {{ block.super }} {{ form.media.js }} {% endblock %} {% block
+furniture %} {% block header %}
 ************ {{{{ vviieeww..ggeett__hheeaaddeerr__ttiittllee }}}} ************
 {% endblock %}
+{# Always show messages div so it can be appended to by JS #} {% if messages or
+form.errors %}
+    * {% if form.errors %} {% for error in form.non_field_errors %}
+    * {{ error }}
+    * {% endfor %} {% endif %} {% for message in messages %}
+    * {{ message }}
+    * {% endfor %}
+{% endif %}
 {% if help_text %} {% panel id="wagtail-fedit-help-text" icon="help"
 heading=help_text.heading %} {% help_block status=help_text.status %}
 {{{{ hheellpp__tteexxtt..ttiittllee }}}}
 {{ help_text.text }}
-{% endhelp_block %} {% endpanel %} {% endif %} {% block content %}{% endblock
-%}
+{% endhelp_block %} {% endpanel %} {% endif %} {% block content %} {% block
+errors %} {% if form.errors or form.non_field_errors %}
+********** {{{{ vviieeww..ggeett__eerrrroorr__ttiittllee }}}} **********
+    * {% for error in form.non_field_errors %}
+    * {{ error }}
+    * {% endfor %} {{ form.errors.as_ul }}
+{% endif %} {% endblock %} {% endblock %}
+{% block sidebar_root %}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
 }" viewBox="0 0 16 16">
 }">
 }" viewBox="0 0 16 16"> {% endblock %}
-{% endblock %}
+{% endblock %} {% endblock %}
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-{% extends "wagtailadmin/base.html" %}
+{% extends "./base_iframe.html" %}
 
-{% load static wagtailadmin_tags wagtailuserbar i18n %}
+{% load static wagtailadmin_tags i18n %}
 
-{% block titletag %}{{view.get_header_title}}{% endblock %}
-
-{% block extra_css %}
-    <link rel="stylesheet" href="{% static 'wagtail_fedit/css/admin.css' %}">
-{% endblock %}
+{% block sidebar_root %}{% endblock %}
 
 {% block content %}
-    {% include "wagtailadmin/shared/header.html" with title=view.get_header_title icon=view.get_header_icon %}
-
-    <div class="nice-padding">
-        <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
-            <form id="wagtail-fedit-form" action="{{ publish_url }}" method="post">
-                {% csrf_token %}
-
-                <div class="wagtail-fedit-form-help">
-                    {% help_block status="warning" %}
-                        <p>{% blocktranslate %}Publishing this object means it will be made visible to all users on the website.{% endblocktranslate %}</p>
-                        <p>{% blocktranslate %}If this is not what you intended; please cancel to go back.{% endblocktranslate %}</p>
-                    {% endhelp_block %}
-                    <h2>{% blocktranslate with model_type=model_verbose_name%}Are you sure you want to publish {{model_type}}?{% endblocktranslate %}</h2>
-                </div>
-                <div class="wagtail-fedit-form-buttons">
-                    <button type="submit" class="button button-primary button-large bicolor button--icon" name="publish" value="1">
-                        <span class="icon-wrapper">
-                            {% icon name="upload" classname="icon" %}
-                        </span>
-                        {% translate "Publish" %}
-                    </button>
-                    <a href="{{ edit_url }}" class="button no button-large">
-                        {% translate "Cancel" %}
-                    </a>
-                </div>
-            </form>
-        </div>
+    <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
+        <form id="wagtail-fedit-form" action="{{ publish_url }}" method="post">
+            {% csrf_token %}
+
+            <div class="wagtail-fedit-form-help">
+                {% help_block status="warning" %}
+                    <p>{% blocktranslate %}Publishing this object means it will be made visible to all users on the website.{% endblocktranslate %}</p>
+                    <p>{% blocktranslate %}If this is not what you intended; please cancel to go back.{% endblocktranslate %}</p>
+                {% endhelp_block %}
+                <h2>{% blocktranslate with model_type=model_verbose_name%}Are you sure you want to publish {{model_type}}?{% endblocktranslate %}</h2>
+            </div>
+
+            <div class="wagtail-fedit-form-buttons">
+                {% for button in buttons %}
+                    {{ button }}
+                {% endfor %}
+                <a href="{{ edit_url }}" class="button no button-large wagtail-fedit-cancel-button" target="_self">
+                    {% translate "Cancel" %}
+                </a>
+            </div>
+        </form>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,13 @@
-{% extends "wagtailadmin/base.html" %} {% load static wagtailadmin_tags
-wagtailuserbar i18n %} {% block titletag %}{{view.get_header_title}}{% endblock
-%} {% block extra_css %}
-{% endblock %} {% block content %} {% include "wagtailadmin/shared/header.html"
-with title=view.get_header_title icon=view.get_header_icon %}
+{% extends "./base_iframe.html" %} {% load static wagtailadmin_tags i18n %} {%
+block sidebar_root %}{% endblock %} {% block content %}
 {% csrf_token %}
 {% help_block status="warning" %}
 {% blocktranslate %}Publishing this object means it will be made visible to all
 users on the website.{% endblocktranslate %}
 {% blocktranslate %}If this is not what you intended; please cancel to go back.
 {% endblocktranslate %}
 {% endhelp_block %}
 ********** {{%% bblloocckkttrraannssllaattee wwiitthh mmooddeell__ttyyppee==mmooddeell__vveerrbboossee__nnaammee%%}}AArree yyoouu ssuurree yyoouu
 wwaanntt ttoo ppuubblliisshh {{{{mmooddeell__ttyyppee}}}}??{{%% eennddbblloocckkttrraannssllaattee %%}} **********
-{% icon name="upload" classname="icon" %} {% translate "Publish" %} _{_%
-_t_r_a_n_s_l_a_t_e_ _"_C_a_n_c_e_l_"_ _%_}
+{% for button in buttons %} {{ button }} {% endfor %} _{_%_ _t_r_a_n_s_l_a_t_e_ _"_C_a_n_c_e_l_"_ _%_}
 {% endblock %}
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-00000000: 7b25 2065 7874 656e 6473 2022 7761 6774  {% extends "wagt
-00000010: 6169 6c61 646d 696e 2f75 7365 7262 6172  ailadmin/userbar
-00000020: 2f69 7465 6d5f 6261 7365 2e68 746d 6c22  /item_base.html"
-00000030: 2025 7d0d 0a7b 2520 6c6f 6164 2069 3138   %}..{% load i18
-00000040: 6e20 7761 6774 6169 6c61 646d 696e 5f74  n wagtailadmin_t
-00000050: 6167 7320 257d 0d0a 0d0a 7b25 2062 6c6f  ags %}....{% blo
-00000060: 636b 2069 7465 6d5f 636f 6e74 656e 7420  ck item_content 
-00000070: 257d 0d0a 2020 2020 3c61 2068 7265 663d  %}..    <a href=
-00000080: 227b 7b20 6564 6974 5f75 726c 7c73 6166  "{{ edit_url|saf
-00000090: 6520 7d7d 2220 7461 7267 6574 3d22 5f73  e }}" target="_s
-000000a0: 656c 6622 2072 6f6c 653d 226d 656e 7569  elf" role="menui
-000000b0: 7465 6d22 3e0d 0a20 2020 2020 2020 203c  tem">..        <
-000000c0: 7376 6720 786d 6c6e 733d 2268 7474 703a  svg xmlns="http:
-000000d0: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
-000000e0: 302f 7376 6722 2066 696c 6c3d 2263 7572  0/svg" fill="cur
-000000f0: 7265 6e74 436f 6c6f 7222 2063 6c61 7373  rentColor" class
-00000100: 3d22 772d 6163 7469 6f6e 2d69 636f 6e22  ="w-action-icon"
-00000110: 2076 6965 7742 6f78 3d22 3020 3020 3136   viewBox="0 0 16
-00000120: 2031 3622 3e0d 0a20 2020 2020 2020 2020   16">..         
-00000130: 2020 203c 212d 2d20 5468 6520 4d49 5420     <!-- The MIT 
-00000140: 4c69 6365 6e73 6520 284d 4954 2920 2d2d  License (MIT) --
-00000150: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00000160: 212d 2d20 436f 7079 7269 6768 7420 2863  !-- Copyright (c
-00000170: 2920 3230 3131 2d32 3032 3420 5468 6520  ) 2011-2024 The 
-00000180: 426f 6f74 7374 7261 7020 4175 7468 6f72  Bootstrap Author
-00000190: 7320 2d2d 3e0d 0a20 2020 2020 2020 2020  s -->..         
-000001a0: 2020 203c 7061 7468 2064 3d22 4d31 3120     <path d="M11 
-000001b0: 3248 3976 3368 327a 222f 3e0d 0a20 2020  2H9v3h2z"/>..   
-000001c0: 2020 2020 2020 2020 203c 7061 7468 2064           <path d
-000001d0: 3d22 4d31 2e35 2030 6831 312e 3538 3661  ="M1.5 0h11.586a
-000001e0: 312e 3520 312e 3520 3020 3020 3120 312e  1.5 1.5 0 0 1 1.
-000001f0: 3036 2e34 346c 312e 3431 3520 312e 3431  06.44l1.415 1.41
-00000200: 3441 312e 3520 312e 3520 3020 3020 3120  4A1.5 1.5 0 0 1 
-00000210: 3136 2032 2e39 3134 5631 342e 3561 312e  16 2.914V14.5a1.
-00000220: 3520 312e 3520 3020 3020 312d 312e 3520  5 1.5 0 0 1-1.5 
-00000230: 312e 3568 2d31 3341 312e 3520 312e 3520  1.5h-13A1.5 1.5 
-00000240: 3020 3020 3120 3020 3134 2e35 762d 3133  0 0 1 0 14.5v-13
-00000250: 4131 2e35 2031 2e35 2030 2030 2031 2031  A1.5 1.5 0 0 1 1
-00000260: 2e35 2030 4d31 2031 2e35 7631 3361 2e35  .5 0M1 1.5v13a.5
-00000270: 2e35 2030 2030 2030 202e 352e 3548 3276  .5 0 0 0 .5.5H2v
-00000280: 2d34 2e35 4131 2e35 2031 2e35 2030 2030  -4.5A1.5 1.5 0 0
-00000290: 2031 2033 2e35 2039 6839 6131 2e35 2031   1 3.5 9h9a1.5 1
-000002a0: 2e35 2030 2030 2031 2031 2e35 2031 2e35  .5 0 0 1 1.5 1.5
-000002b0: 5631 3568 2e35 612e 352e 3520 3020 3020  V15h.5a.5.5 0 0 
-000002c0: 3020 2e35 2d2e 3556 322e 3931 3461 2e35  0 .5-.5V2.914a.5
-000002d0: 2e35 2030 2030 2030 2d2e 3134 362d 2e33  .5 0 0 0-.146-.3
-000002e0: 3533 6c2d 312e 3431 352d 312e 3431 3541  53l-1.415-1.415A
-000002f0: 2e35 2e35 2030 2030 2030 2031 332e 3038  .5.5 0 0 0 13.08
-00000300: 3620 3148 3133 7634 2e35 4131 2e35 2031  6 1H13v4.5A1.5 1
-00000310: 2e35 2030 2030 2031 2031 312e 3520 3768  .5 0 0 1 11.5 7h
-00000320: 2d37 4131 2e35 2031 2e35 2030 2030 2031  -7A1.5 1.5 0 0 1
-00000330: 2033 2035 2e35 5631 4831 2e35 612e 352e   3 5.5V1H1.5a.5.
-00000340: 3520 3020 3020 302d 2e35 2e35 6d33 2034  5 0 0 0-.5.5m3 4
-00000350: 612e 352e 3520 3020 3020 3020 2e35 2e35  a.5.5 0 0 0 .5.5
-00000360: 6837 612e 352e 3520 3020 3020 3020 2e35  h7a.5.5 0 0 0 .5
-00000370: 2d2e 3556 3148 347a 4d33 2031 3568 3130  -.5V1H4zM3 15h10
-00000380: 762d 342e 3561 2e35 2e35 2030 2030 2030  v-4.5a.5.5 0 0 0
-00000390: 2d2e 352d 2e35 682d 3961 2e35 2e35 2030  -.5-.5h-9a.5.5 0
-000003a0: 2030 2030 2d2e 352e 357a 222f 3e0d 0a20   0 0-.5.5z"/>.. 
-000003b0: 2020 2020 2020 203c 2f73 7667 3e0d 0a20         </svg>.. 
-000003c0: 2020 2020 2020 207b 2520 7472 616e 7320         {% trans 
-000003d0: 2750 7562 6c69 7368 2052 6576 6973 696f  'Publish Revisio
-000003e0: 6e27 2025 7d0d 0a20 2020 203c 2f61 3e0d  n' %}..    </a>.
-000003f0: 0a7b 2520 656e 6462 6c6f 636b 2025 7d    .{% endblock %}
+00000000: 7b25 206c 6f61 6420 7761 6774 6169 6c61  {% load wagtaila
+00000010: 646d 696e 5f74 6167 7320 6931 386e 2025  dmin_tags i18n %
+00000020: 7d0d 0a3c 6275 7474 6f6e 2074 7970 653d  }..<button type=
+00000030: 2273 7562 6d69 7422 2063 6c61 7373 3d22  "submit" class="
+00000040: 7761 6774 6169 6c2d 6665 6469 742d 7573  wagtail-fedit-us
+00000050: 6572 6261 722d 6275 7474 6f6e 2062 7574  erbar-button but
+00000060: 746f 6e20 6269 636f 6c6f 7220 6275 7474  ton bicolor butt
+00000070: 6f6e 2d2d 6963 6f6e 7b25 2069 6620 6869  on--icon{% if hi
+00000080: 6464 656e 2025 7d20 696e 6974 6961 6c6c  dden %} initiall
+00000090: 792d 6869 6464 656e 7b25 2065 6e64 6966  y-hidden{% endif
+000000a0: 2025 7d22 206e 616d 653d 2261 6374 696f   %}" name="actio
+000000b0: 6e2d 7375 626d 6974 2220 7661 6c75 653d  n-submit" value=
+000000c0: 2231 223e 0d0a 2020 2020 3c73 7061 6e20  "1">..    <span 
+000000d0: 636c 6173 733d 2269 636f 6e2d 7772 6170  class="icon-wrap
+000000e0: 7065 7222 3e0d 0a20 2020 2020 2020 203c  per">..        <
+000000f0: 7376 6720 786d 6c6e 733d 2268 7474 703a  svg xmlns="http:
+00000100: 2f2f 7777 772e 7733 2e6f 7267 2f32 3030  //www.w3.org/200
+00000110: 302f 7376 6722 2066 696c 6c3d 2263 7572  0/svg" fill="cur
+00000120: 7265 6e74 436f 6c6f 7222 2063 6c61 7373  rentColor" class
+00000130: 3d22 772d 6163 7469 6f6e 2d69 636f 6e22  ="w-action-icon"
+00000140: 2076 6965 7742 6f78 3d22 3020 3020 3136   viewBox="0 0 16
+00000150: 2031 3622 3e0d 0a20 2020 2020 2020 2020   16">..         
+00000160: 2020 203c 212d 2d20 5468 6520 4d49 5420     <!-- The MIT 
+00000170: 4c69 6365 6e73 6520 284d 4954 2920 2d2d  License (MIT) --
+00000180: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000190: 212d 2d20 436f 7079 7269 6768 7420 2863  !-- Copyright (c
+000001a0: 2920 3230 3131 2d32 3032 3420 5468 6520  ) 2011-2024 The 
+000001b0: 426f 6f74 7374 7261 7020 4175 7468 6f72  Bootstrap Author
+000001c0: 7320 2d2d 3e0d 0a20 2020 2020 2020 2020  s -->..         
+000001d0: 2020 203c 7061 7468 2064 3d22 4d31 342e     <path d="M14.
+000001e0: 3520 3361 2e35 2e35 2030 2030 2031 202e  5 3a.5.5 0 0 1 .
+000001f0: 352e 3576 3961 2e35 2e35 2030 2030 2031  5.5v9a.5.5 0 0 1
+00000200: 2d2e 352e 3568 2d31 3361 2e35 2e35 2030  -.5.5h-13a.5.5 0
+00000210: 2030 2031 2d2e 352d 2e35 762d 3961 2e35   0 1-.5-.5v-9a.5
+00000220: 2e35 2030 2030 2031 202e 352d 2e35 7a6d  .5 0 0 1 .5-.5zm
+00000230: 2d31 332d 3141 312e 3520 312e 3520 3020  -13-1A1.5 1.5 0 
+00000240: 3020 3020 3020 332e 3576 3941 312e 3520  0 0 0 3.5v9A1.5 
+00000250: 312e 3520 3020 3020 3020 312e 3520 3134  1.5 0 0 0 1.5 14
+00000260: 6831 3361 312e 3520 312e 3520 3020 3020  h13a1.5 1.5 0 0 
+00000270: 3020 312e 352d 312e 3576 2d39 4131 2e35  0 1.5-1.5v-9A1.5
+00000280: 2031 2e35 2030 2030 2030 2031 342e 3520   1.5 0 0 0 14.5 
+00000290: 327a 222f 3e0d 0a20 2020 2020 2020 2020  2z"/>..         
+000002a0: 2020 203c 7061 7468 2064 3d22 4d37 2035     <path d="M7 5
+000002b0: 2e35 612e 352e 3520 3020 3020 3120 2e35  .5a.5.5 0 0 1 .5
+000002c0: 2d2e 3568 3561 2e35 2e35 2030 2030 2031  -.5h5a.5.5 0 0 1
+000002d0: 2030 2031 682d 3561 2e35 2e35 2030 2030   0 1h-5a.5.5 0 0
+000002e0: 2031 2d2e 352d 2e35 6d2d 312e 3439 362d   1-.5-.5m-1.496-
+000002f0: 2e38 3534 612e 352e 3520 3020 3020 3120  .854a.5.5 0 0 1 
+00000300: 3020 2e37 3038 6c2d 312e 3520 312e 3561  0 .708l-1.5 1.5a
+00000310: 2e35 2e35 2030 2030 2031 2d2e 3730 3820  .5.5 0 0 1-.708 
+00000320: 306c 2d2e 352d 2e35 612e 352e 3520 3020  0l-.5-.5a.5.5 0 
+00000330: 3120 3120 2e37 3038 2d2e 3730 386c 2e31  1 1 .708-.708l.1
+00000340: 3436 2e31 3437 2031 2e31 3436 2d31 2e31  46.147 1.146-1.1
+00000350: 3437 612e 352e 3520 3020 3020 3120 2e37  47a.5.5 0 0 1 .7
+00000360: 3038 2030 4d37 2039 2e35 612e 352e 3520  08 0M7 9.5a.5.5 
+00000370: 3020 3020 3120 2e35 2d2e 3568 3561 2e35  0 0 1 .5-.5h5a.5
+00000380: 2e35 2030 2030 2031 2030 2031 682d 3561  .5 0 0 1 0 1h-5a
+00000390: 2e35 2e35 2030 2030 2031 2d2e 352d 2e35  .5.5 0 0 1-.5-.5
+000003a0: 6d2d 312e 3439 362d 2e38 3534 612e 352e  m-1.496-.854a.5.
+000003b0: 3520 3020 3020 3120 3020 2e37 3038 6c2d  5 0 0 1 0 .708l-
+000003c0: 312e 3520 312e 3561 2e35 2e35 2030 2030  1.5 1.5a.5.5 0 0
+000003d0: 2031 2d2e 3730 3820 306c 2d2e 352d 2e35   1-.708 0l-.5-.5
+000003e0: 612e 352e 3520 3020 3020 3120 2e37 3038  a.5.5 0 0 1 .708
+000003f0: 2d2e 3730 386c 2e31 3436 2e31 3437 2031  -.708l.146.147 1
+00000400: 2e31 3436 2d31 2e31 3437 612e 352e 3520  .146-1.147a.5.5 
+00000410: 3020 3020 3120 2e37 3038 2030 222f 3e0d  0 0 1 .708 0"/>.
+00000420: 0a20 2020 2020 2020 203c 2f73 7667 3e0d  .        </svg>.
+00000430: 0a20 2020 203c 2f73 7061 6e3e 0d0a 2020  .    </span>..  
+00000440: 2020 7b25 2074 7261 6e73 6c61 7465 2022    {% translate "
+00000450: 5375 626d 6974 2066 6f72 204d 6f64 6572  Submit for Moder
+00000460: 6174 696f 6e22 2025 7d0d 0a3c 2f62 7574  ation" %}..</but
+00000470: 746f 6e3e                                ton>
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd0b10d66 (Wed Apr  3 19:45:20 2024 UTC)
+moddate:  0x46040f66 (Thu Apr  4 19:49:26 2024 UTC)
 files sz: 13828
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.9/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.9/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,16 @@
 from django.test import TestCase
-from django import forms
 from wagtail import blocks
-from .. import forms as block_forms
-from .. import utils
-
-TEST_BLOCK_DATA = [
-    {
-        "type": "heading_component",
-        "value": {
-            "heading": "This is pretty cool!!!",
-            "subheading": "RIGHT?! FUCK YES!"
-        },
-        "id": "0bc9f67e-f116-48a6-9ca1-6c11d39b54e8"
-    },
-    {
-        "type": "heading_component",
-        "value": {
-            "heading": "AWESOME!!",
-            "subheading": "RIGHT?!"
-        },
-        "id": "d543a6bf-34dc-4365-a3fa-d302561930ae"
-    },
-    {
-        "type": "heading_component",
-        "value": {
-            "heading": "WORKS NOW!",
-            "subheading": "!!!!!!!!!!!!1"
-        },
-        "id": "c49abcae-3c66-4fc7-979d-35407226b9f5"
-    },
-    {
-        "type": "heading_component",
-        "value": {
-            "heading": "Heading!!!!",
-            "subheading": "Subheading"
-        },
-        "id": "7bd7bc3a-1d2d-4182-8726-b257beace968"
-    },
-    {
-        "type": "heading_component",
-        "value": {
-            "heading": "Hey!",
-            "subheading": "Subheading!"
-        },
-        "id": "74a94baa-acf4-49ab-be5f-9c8a70cbc623"
-    },
-    {
-        "type": "flat_menu_component",
-        "value": {
-            "title": "Test Title123123! HAHA!",
-            "subtitle": "<p data-block-key=\"306j3\">i am so<b><i> happy</i></b></p>",
-            "items": [
-                {
-                    "type": "item",
-                    "value": {
-                        "link": {
-                            "text": "Test Item 1"
-                        }
-                    },
-                    "id": "c757f54d-0df5-4b35-8a06-4174f180ec41"
-                },
-                {
-                    "type": "item",
-                    "value": {
-                        "link": {
-                            "text": "Test Item 2"
-                        }
-                    },
-                    "id": "ec3d73d1-fd01-49ba-840a-d44586ac0025"
-                },
-                {
-                    "type": "item",
-                    "value": {
-                        "link": {
-                            "text": "Test Item 3"
-                        }
-                    },
-                    "id": "a98a19c6-2ead-4e69-9ea2-3158c7e82976"
-                },
-                {
-                    "type": "item",
-                    "value": {
-                        "link": {
-                            "text": "Test Item 4"
-                        }
-                    },
-                    "id": "db7183a2-d9dd-4fbd-9e42-fd2b9ebf0458"
-                }
-            ]
-        },
-        "id": "3e9144fd-5fa5-47f8-917e-8fe87c15da01"
-    }
-]
-
-
-class HeadingComponent(blocks.StructBlock):
-    heading = blocks.CharBlock(max_length=25)
-    subheading = blocks.CharBlock(max_length=40)
-
-class LinkBlock(blocks.StructBlock):
-    text = blocks.CharBlock(max_length=25)
-
-class MenuItemBlock(blocks.StructBlock):
-    link = LinkBlock()
-
-class FlatMenuComponent(blocks.StructBlock):
-    title = blocks.CharBlock(max_length=25)
-    subtitle = blocks.RichTextBlock()
-    items = blocks.ListBlock(
-        MenuItemBlock()
-    )
+from wagtail_fedit import forms as block_forms
+from wagtail_fedit import utils
+from .base import TEST_BLOCK_DATA
+from ..models import (
+    HeadingComponent,
+    FlatMenuComponent
+)
 
 import uuid
 
 _model_map = {}
 
 class FakeModel(object):
     def __init__(self, title="Fake Model"):
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.9/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.9/wagtail_fedit/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 
 app_name = "wagtail_fedit"
 
 urlpatterns = [
     path("editable/<str:object_id>/<str:app_label>/<str:model_name>/", views.FEditableView.as_view(), name="editable"),
     path("publish/<str:object_id>/<str:app_label>/<str:model_name>/", views.FeditablePublishView.as_view(), name="publish"),
     path("field/<str:field_name>/<str:app_label>/<str:model_name>/<str:model_id>/", views.EditFieldView.as_view(), name="edit_field"),
-    path("edit_block/<str:block_id>/<str:field_name>/<str:app_label>/<str:model_name>/<str:model_id>/", views.EditBlockView.as_view(), name="edit_block"),
+    path("block/<str:block_id>/<str:field_name>/<str:app_label>/<str:model_name>/<str:model_id>/", views.EditBlockView.as_view(), name="edit_block"),
 ]
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.9/wagtail_fedit/views/blocks.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,58 +21,64 @@
 from ..templatetags.fedit import BlockEditNode
 from .. import forms as block_forms
 from .. import utils
 
 
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
-class EditBlockView(utils.FeditHelpTextMixin, utils.FeditPermissionCheck, WagtailAdminTemplateMixin, View):
+class EditBlockView(utils.FeditIFrameMixin, utils.FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     template_name = "wagtail_fedit/editor/block_iframe.html"
+    ERROR_TITLE = _("Block Validation Errors")
 
     def dispatch(self, request: HttpRequest, block_id = None, field_name = None, model_id = None, model_name = None, app_label = None) -> None:
 
         self.edit_args = ["block_id", "field_name", "model_id", "model_name", "app_label"]
         if not all([block_id, field_name, model_id, model_name, app_label]):
             return HttpResponseBadRequest("Missing required parameters")
         
         self.block_id = block_id
         self.field_name = field_name
         self.model_id = model_id
         self.model_name = model_name
         self.app_label = app_label
-        self.has_block = BlockEditNode.unpack("has_block", request=request)["has_block"].lower() == "true"
+        if "has_block" in request.GET:
+            self.has_block = BlockEditNode.unpack("has_block", request=request)["has_block"].lower() == "true"
+        else:
+            self.has_block = False
 
 
         self.model = apps.get_model(self.app_label, self.model_name)
         if not self.has_perms(request, self.model):
             return HttpResponseBadRequest("You do not have permission to view this page")
 
 
-        if issubclass(self.model, RevisionMixin):
-            self.model_instance = self.model.objects.get(pk=self.model_id)
+        self.model_instance = self.model._default_manager.get(pk=self.model_id)
+        if issubclass(self.model, RevisionMixin) and self.model_instance.latest_revision_id:
             self.instance = self.model_instance.latest_revision.as_object()
         else:
-            self.instance = self.model._default_manager.get(pk=self.model_id)
-            self.model_instance = self.instance
+            self.instance = self.model_instance
 
 
         self.streamfield: StreamValue = getattr(self.instance, self.field_name)
         result = utils.find_block(self.block_id, self.streamfield)
         if not result:
             # raise ValueError("Block not found; did you provide the correct block ID?")
             return HttpResponseBadRequest("Block not found; did you provide the correct block ID?")
 
 
         self.block, self.contentpath = result
         self.form_class = block_forms.get_block_form_class(self.block.block)
 
-
         if not self.form_class:
             return HttpResponseBadRequest("Invalid block type")
 
+        self.lock, self.locked_for_user = utils.lock_info(
+            self.model_instance, request.user,
+        )
+
         return super().dispatch(request, block_id, field_name, model_id, model_name, app_label)
 
     def get_header_title(self):
 
         model_string = getattr(self.instance, "get_admin_display_title", None)
         if model_string:
             model_string = model_string()
@@ -99,15 +105,14 @@
             "block": self.block,
             "instance": self.instance,
             "streamfield": self.streamfield,
             "has_block": self.has_block,
             "label": self.block.block.label,
             "wagtail_fedit_instance": self.instance,
             "wagtail_fedit_has_block": self.has_block,
-            "help_text": self.get_help_text(),
             "edit_url": BlockEditNode.get_edit_url(
                 self.block_id, self.field_name, self.instance,
             ),
             "form_attrs": {
                 "data-block-id": self.block_id,
                 "data-block-name": self.block.block.name,
             },
@@ -121,14 +126,15 @@
                 "wagtailadmin_pages:edit",
                 args=[self.instance.pk],
             )
             admin_edit_url = f"{admin_edit_url}#block-{self.block_id}-section"
         else:
             admin_edit_url = None
 
+
         must["admin_edit_url"] = admin_edit_url
 
         context.update(must)
         for key, value in can.items():
             context.setdefault(key, value)
 
         return context
@@ -149,38 +155,39 @@
             context,
         )
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(block=self.block, parent_instance=self.instance, request=request)
         # Safe to omit data from context - we are not rendering the content.
         return self.render_to_response(
-            self.get_context_data(form=form),
+            self.get_context_data(form=form, locked=self.locked_for_user),
             success=True,
         )
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, block=self.block, parent_instance=self.instance, request=request)
 
         # Set the preview flag to mark as editable block when re-rendering.
         setattr(request, utils.FEDIT_PREVIEW_VAR, True)
 
         valid = form.is_valid()
-        if valid:
+        if valid and not self.locked_for_user:
             self.block = form.save()
         else:
             # We are not rendering the content, so we can omit data from context.
             return JsonResponse({
                 "success": False,
                 "errors": form.errors,
+                "locked": self.locked_for_user,
                 "html": render_to_string(
                     "wagtail_fedit/editor/block_iframe.html",
-                    context=self.get_context_data(form=form),
+                    context=self.get_context_data(form=form, locked=self.locked_for_user),
                     request=request,
                 )
-            })
+            }, status=423 if self.locked_for_user else 400)
         
         extra_log_kwargs = {}
         if isinstance(self.instance, RevisionMixin):
             extra_log_kwargs["revision"] = self.instance.latest_revision
 
         meta_field = self.model._meta.get_field(self.field_name)
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.9/wagtail_fedit/views/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import View
 from django.http import (
     HttpRequest,
     HttpResponseBadRequest,
+    HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
 )
 from django.apps import apps
 
 from wagtail.log_actions import log
 from wagtail.models import (
-    DraftStateMixin,
     RevisionMixin, 
 )
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 
 import uuid
 
 from ..templatetags.fedit import (
@@ -30,41 +30,45 @@
 )
 from ..forms import (
     blocks as block_forms,
     fields as field_forms,
 )
 from ..utils import (
     FeditPermissionCheck,
-    FeditHelpTextMixin,
+    FeditIFrameMixin,
     use_related_form,
     get_field_content,
     saving_relation,
     is_draft_capable,
     get_model_string,
+    lock_info,
 )
 
 
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
-class EditFieldView(FeditHelpTextMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
+class EditFieldView(FeditIFrameMixin, FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     template_name = "wagtail_fedit/editor/field_iframe.html"
+    ERROR_TITLE = _("Validation Errors")
 
     def dispatch(self, request: HttpRequest, field_name = None, app_label = None, model_name = None, model_id = None) -> None:
         if not all([field_name, model_name, app_label, model_id]):
             return HttpResponseBadRequest("Missing required parameters")
 
         self.model = apps.get_model(app_label, model_name)
         if not self.has_perms(request, self.model):
-            return HttpResponseBadRequest("You do not have permission to view this page")
+            return HttpResponseForbidden("Permission denied")
 
-        if issubclass(self.model, RevisionMixin):
-            model_instance = self.model.objects.get(pk=model_id)
+        # Only fetch latest reivision if it exists
+        # If not; it will be automatically created by the form.
+        model_instance = self.model._default_manager.get(pk=model_id)
+        if isinstance(model_instance, RevisionMixin) and model_instance.latest_revision_id:
             self.instance = model_instance.latest_revision.as_object()
         else:
-            self.instance = self.model._default_manager.get(pk=model_id)
+            self.instance = model_instance
 
         self.field_name = field_name
         self.model_name = model_name
         self.app_label = app_label
         self.model_id = model_id
         self.original_instance = self.instance
         self.field_value = getattr(self.instance, self.field_name)
@@ -89,14 +93,18 @@
             )
         else:
             self.form_class = field_forms.get_form_class_for_fields(
                 self.model,
                 [field_name],
             )
 
+        self.lock, self.locked_for_user = lock_info(
+            self.instance, request.user,
+        )
+
         return super().dispatch(request, field_name, model_name, app_label, model_id)
 
     def get_header_title(self):
         meta_field: models.Field = self.model._meta.get_field(self.field_name)
 
         model_string = get_model_string(self.original_instance)
         if self.original_instance != self.instance:
@@ -130,171 +138,163 @@
         )
     
     def get_help_text(self):
         if is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
-                "status": "info",
-                "heading": _("Publishing required."),
-                "title": _("The objects you are editing support drafts."),
+                "status": "warning",
+                "heading": FeditIFrameMixin.HEADING_SUPPORTS_DRAFTS,
+                "title": FeditIFrameMixin.TITLE_SUPPORTS_DRAFTS,
                 "text": mark_safe(_("You must publish %(model)s and the related object of type %(related_verbose_name)s (%(related_model)s) to make any changes visible.") % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                     "related_verbose_name": self.instance._meta.verbose_name,
                     "related_model": get_model_string(self.instance, publish_url=True, request=self.request),
                 })
             }
 
         elif is_draft_capable(self.original_instance)\
                 and not is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
-                "status": "info",
-                "heading": _("Publishing required."),
-                "title": _("The object you are editing supports drafts."),
-                "text": mark_safe(_("You must publish %(model)s to make any changes visible.") % {
+                "status": "warning",
+                "heading": FeditIFrameMixin.HEADING_SUPPORTS_DRAFTS,
+                "title": FeditIFrameMixin.TITLE_SUPPORTS_DRAFTS,
+                "text": mark_safe(FeditIFrameMixin.TEXT_PUBLISH_DRAFTS % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                 })
             }
         
         elif not is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
-                "status": "info",
+                "status": "warning",
                 "heading": _("Publishing related object required."),
                 "title": _("The object you are editing supports drafts."),
                 "text": mark_safe(_("You must publish the related object of type %(type)s (%(model)s) to make any changes visible.") % {
                     "type": self.original_instance._meta.verbose_name,
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                 })
             }
 
         return super().get_help_text()
-
         
     
     def get_context_data(self, **kwargs):
         return super().get_context_data(**kwargs) | {
             "form_attrs": {
                 "data-original-pk": self.original_instance.pk,
                 "data-original-model": self.model_name,
                 "data-original-app": self.app_label,
                 "data-original-field": self.field_name,
                 "data-is-relation": self.meta_field.is_relation\
                     and isinstance(self.field_value, models.Model),
             },
-            "original_instance": {
-                "is_draft_capable": issubclass(self.model, RevisionMixin)\
-                    and issubclass(self.model, DraftStateMixin),
-                "object": self.original_instance,
-            },
-            "instance": {
-                "is_draft_capable": issubclass(self.model, RevisionMixin)\
-                    and issubclass(self.model, DraftStateMixin),
-                "object": self.instance,
-            },
-            "help_text": self.get_help_text(),
             "meta_field": self.meta_field,
             "field_name": self.field_name,
         }
 
+
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.form_class(request=request, instance=self.instance)
         return self.render_to_response(
-            self.get_context_data(form=form),
+            self.get_context_data(form=form, locked=self.locked_for_user),
             success=True,
         )
 
+
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         form = self.form_class(request.POST, request=request, instance=self.instance)
-        if form.is_valid():
-            self.instance = form.save()
-            
-            # add data to context
-            context = self.get_context_data(form=form, **self.data)
-
-            # Check if we are saving a relation
-            if saving_relation(self.instance, self.original_instance):
-                self.meta_field.save_form_data(self.original_instance, self.instance)
-                field_forms.save_possible_revision(self.original_instance, request)
-
-            extra_log_kwargs = {}
-            if isinstance(self.original_instance, RevisionMixin):
-                extra_log_kwargs["revision"] = self.original_instance.latest_revision
-
-            data = {
-                "verbose_field_name": self.meta_field.verbose_name,
-                "field_name": self.field_name,
-                "model_id": self.model_id,
-                "model_name": self.model_name,
-                "app_label": self.app_label,
-                "model_verbose": str(self.model._meta.verbose_name),
-                "model_string": str(get_model_string(self.original_instance)),
-                "old": str(self.initial_field_value),
-                "new": str(getattr(
-                    self.original_instance,
-                    self.field_name
-                )),
-            }
+        if not form.is_valid() or self.locked_for_user:
+            return JsonResponse({
+                "success": False,
+                "errors": form.errors,
+                "locked": self.locked_for_user,
+                "html": render_to_string(
+                    "wagtail_fedit/editor/field_iframe.html",
+                    context=self.get_context_data(form=form, locked=self.locked_for_user),
+                    request=request,
+                )
+            }, status=423 if self.locked_for_user else 400)
 
-            uid = uuid.uuid4()
-            if self.original_instance.pk != self.instance.pk:
-                data.update({
-                    "edited_model_string": str(get_model_string(self.instance)),
-                    "edited_model_verbose": str(self.instance._meta.verbose_name),
-                    "edited_model_id": self.instance.pk,
-                    "edited_model_name": self.instance._meta.model_name,
-                    "edited_app_label": self.instance._meta.app_label,
-                })
+        
+        self.instance = form.save()
+        
+        # add data to context
+        context = self.get_context_data(form=form, **self.data)
+
+        # Check if we are saving a relation
+        if saving_relation(self.instance, self.original_instance):
+            self.meta_field.save_form_data(self.original_instance, self.instance)
+            field_forms.save_possible_revision(self.original_instance, request)
+
+        extra_log_kwargs = {}
+        if isinstance(self.original_instance, RevisionMixin):
+            extra_log_kwargs["revision"] = self.original_instance.latest_revision
+
+        data = {
+            "verbose_field_name": self.meta_field.verbose_name,
+            "field_name": self.field_name,
+            "model_id": self.model_id,
+            "model_name": self.model_name,
+            "app_label": self.app_label,
+            "model_verbose": str(self.model._meta.verbose_name),
+            "model_string": str(get_model_string(self.original_instance)),
+            "old": str(self.initial_field_value),
+            "new": str(getattr(
+                self.original_instance,
+                self.field_name
+            )),
+        }
+
+        uid = uuid.uuid4()
+        if self.original_instance.pk != self.instance.pk:
+            data.update({
+                "edited_model_string": str(get_model_string(self.instance)),
+                "edited_model_verbose": str(self.instance._meta.verbose_name),
+                "edited_model_id": self.instance.pk,
+                "edited_model_name": self.instance._meta.model_name,
+                "edited_app_label": self.instance._meta.app_label,
+            })
 
-                log(
-                    instance=self.instance,
-                    action="wagtail_fedit.related_changed",
-                    user=request.user,
-                    uuid=uid,
-                    data=data,
-                    content_changed=True,
-                )
-            
             log(
-                instance=self.original_instance,
-                action="wagtail_fedit.edit_field",
+                instance=self.instance,
+                action="wagtail_fedit.related_changed",
                 user=request.user,
-                title=self.get_header_title(),
                 uuid=uid,
                 data=data,
                 content_changed=True,
-                **extra_log_kwargs,
-            )
-
-            content = get_field_content(
-                request,
-                self.original_instance,
-                self.meta_field,
-                context
             )
+        
+        log(
+            instance=self.original_instance,
+            action="wagtail_fedit.edit_field",
+            user=request.user,
+            title=self.get_header_title(),
+            uuid=uid,
+            data=data,
+            content_changed=True,
+            **extra_log_kwargs,
+        )
 
-            # Render the frame HTML
-            html = render_editable_field(
-                self.request, content,
-                self.field_name, self.original_instance,
-                context=context,
-                **self.data,
-            )
+        content = get_field_content(
+            request,
+            self.original_instance,
+            self.meta_field,
+            context
+        )
 
-            return JsonResponse({
-                "success": True,
-                "html": html,
-            })
+        # Render the frame HTML
+        html = render_editable_field(
+            self.request, content,
+            self.field_name, self.original_instance,
+            context=context,
+            **self.data,
+        )
 
         return JsonResponse({
-            "success": False,
-            "errors": form.errors,
-            "html": render_to_string(
-                "wagtail_fedit/editor/field_iframe.html",
-                context=self.get_context_data(form=form),
-                request=request,
-            )
+            "success": True,
+            "html": html,
         })
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.9/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.9/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_fedit
-Version: 1.2.8
+Name: wagtail-fedit
+Version: 1.2.9
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
@@ -103,26 +101,65 @@
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
    Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+
+## Permissions
+
+**Note: This is not required for pages.**
+
+**The `Page` model already provides this interface.**
+
+We have the following basic permission requirements:
+
+* You must have `wagtailadmin.access_admin` to edit a block/field.
+* You must have the appropriate `app_label.change_*` permission for the model.
+
+This however only applies to editing.
+
+We use separate permissions for publishing and submitting workflows, etc.
+
+Models which you want to allow the publish view for should also implement a `PermissionTester`- like object.
+
+Example of how you should implement the `Tester` object and all required permissions. (More details in `models.py`)
+
+```python
+
+class MyModel(...):
+    def permissions_for_user(self, user):
+        return MyModelPermissionTester(self, user)
+
+class MyModelPermissionTester(...):
+    def can_unpublish(self):
+        """ Can the user unpublish this object? (Required for un-publishing"""
+  
+    def can_publish(self):
+        """ Can the user publish this object? (Required for publishing)"""  
+  
+    def can_submit_for_moderation(self):
+        """ Can the user submit this object for moderation? (Optional) """
+
+```
 
-4. **But wait?! I go to my template and I do not see a way to edit!**  
-   That is true! We try to protect any styling on your actual page; we do not want to interfere.  
-   Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar.  
-   Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
-   
 ## Revisions
 
 Revision support is included out of the box.
 If your model inherits from a `RevisionMixin`, we will automatically create drafts for you.
 These will not be published (If the model inherits from `DraftStateMixin`) until you choose to do so.
 
+## Workflows
+
+We include a `WorkFlow` to submit this object for moderation.
+
+More workflow support will be included in the future.
+
 ## Logs
 
 Logs are also included out of the box.
 We will automatically update your model's history; including possible revisions.
 This will allow you to backtrack each change made on the frontend.
 This however does mean that a possibly large amount of data will be stored in your database.
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.8 Summary: An
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.2.9 Summary: An
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
@@ -34,28 +33,44 @@
 fedit %} {% for block in self.content %} {% fedit_block block=block
 block_id=block.id field_name="content" model=self %} {% endfor %} ``` ```python
 from django.template.loader import render_to_string ... class MyPage(...): #
 Can be any type of model. content = StreamField(...) def render_fedit_content
 (self, request): return render_to_string("myapp/render_my_field.html",
 self.get_context(request)) ``` Your content will then automatically be rendered
 with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!** That is
-true! We try to protect any styling on your actual page; we do not want to
-interfere. Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Revisions Revision support is included out of the box. If
-your model inherits from a `RevisionMixin`, we will automatically create drafts
-for you. These will not be published (If the model inherits from
-`DraftStateMixin`) until you choose to do so. ## Logs Logs are also included
-out of the box. We will automatically update your model's history; including
-possible revisions. This will allow you to backtrack each change made on the
-frontend. This however does mean that a possibly large amount of data will be
-stored in your database. ## Caveats Wagtail does not always make it's `id`
-attribute available. This is only available to instances of `StreamChild` and
+**But wait?! I go to my template and I do not see a way to edit!**That is true!
+We try to protect any styling on your actual page; we do not want to
+interfere.Instead; we serve the editing interface on a different URL,
+accessible by clicking `Frontend Editing` in the Wagtail userbar.Keep an eye on
+that userbar! It is also used for publishing if your model inherits from
+`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
+**The `Page` model already provides this interface.** We have the following
+basic permission requirements: * You must have `wagtailadmin.access_admin` to
+edit a block/field. * You must have the appropriate `app_label.change_*`
+permission for the model. This however only applies to editing. We use separate
+permissions for publishing and submitting workflows, etc. Models which you want
+to allow the publish view for should also implement a `PermissionTester`- like
+object. Example of how you should implement the `Tester` object and all
+required permissions. (More details in `models.py`) ```python class MyModel
+(...): def permissions_for_user(self, user): return MyModelPermissionTester
+(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
+Can the user unpublish this object? (Required for un-publishing""" def
+can_publish(self): """ Can the user publish this object? (Required for
+publishing)""" def can_submit_for_moderation(self): """ Can the user submit
+this object for moderation? (Optional) """ ``` ## Revisions Revision support is
+included out of the box. If your model inherits from a `RevisionMixin`, we will
+automatically create drafts for you. These will not be published (If the model
+inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
+include a `WorkFlow` to submit this object for moderation. More workflow
+support will be included in the future. ## Logs Logs are also included out of
+the box. We will automatically update your model's history; including possible
+revisions. This will allow you to backtrack each change made on the frontend.
+This however does mean that a possibly large amount of data will be stored in
+your database. ## Caveats Wagtail does not always make it's `id` attribute
+available. This is only available to instances of `StreamChild` and
 `ListChild`. Consider the following regular wagtail list loop where `items` is
 a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
 item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
 editable block instead; we would slightly change the loop to make the block's
 `id` available. This is done by accessing the `bound_blocks` of that ListBlock
 *(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
 would then be: ```django-html {% for item in self.items.bound_blocks %} {#
```

### Comparing `wagtail_fedit-1.2.8/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.9/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,78 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-tests/__init__.py
-tests/testapp/__init__.py
-tests/testapp/manage.py
-tests/testapp/core/__init__.py
-tests/testapp/core/tests.py
-tests/testapp/core/migrations/__init__.py
-tests/testapp/testapp/__init__.py
-tests/testapp/testapp/asgi.py
-tests/testapp/testapp/settings.py
-tests/testapp/testapp/urls.py
-tests/testapp/testapp/wsgi.py
 wagtail_fedit/__init__.py
 wagtail_fedit/admin.py
 wagtail_fedit/apps.py
 wagtail_fedit/hooks.py
+wagtail_fedit/models.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-wagtail_fedit/static/wagtail_fedit/css/admin.css
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
+wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
-wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+wagtail_fedit/templates/wagtail_fedit/editor/buttons/publish.html
+wagtail_fedit/templates/wagtail_fedit/editor/buttons/submit.html
+wagtail_fedit/templates/wagtail_fedit/editor/buttons/unpublish.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
-wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/publish.html
+wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/submit.html
+wagtail_fedit/templates/wagtail_fedit/userbar/publish/buttons/unpublish.html
 wagtail_fedit/templatetags/__init__.py
 wagtail_fedit/templatetags/fedit.py
 wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
-wagtail_fedit/tests/__init__.py
-wagtail_fedit/tests/test_blocks.py
+wagtail_fedit/test/__init__.py
+wagtail_fedit/test/manage.py
+wagtail_fedit/test/settings.py
+wagtail_fedit/test/core/__init__.py
+wagtail_fedit/test/core/apps.py
+wagtail_fedit/test/core/models.py
+wagtail_fedit/test/core/migrations/0001_initial.py
+wagtail_fedit/test/core/migrations/0002_basicmodel.py
+wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+wagtail_fedit/test/core/migrations/__init__.py
+wagtail_fedit/test/core/tests/__init__.py
+wagtail_fedit/test/core/tests/base.py
+wagtail_fedit/test/core/tests/test_block_edit.py
+wagtail_fedit/test/core/tests/test_blocks.py
+wagtail_fedit/test/core/tests/test_field_edit.py
+wagtail_fedit/test/core/tests/test_revision.py
+wagtail_fedit/test/testapp/__init__.py
+wagtail_fedit/test/testapp/asgi.py
+wagtail_fedit/test/testapp/urls.py
+wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/blocks.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/fields.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/excluded_relations.py
 wagtail_fedit/wagtail_hooks/log_actions.py
```

