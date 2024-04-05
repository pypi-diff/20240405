# Comparing `tmp/django-mailinglist-0.1.6.tar.gz` & `tmp/django-mailinglist-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mailinglist-0.1.6.tar", last modified: Tue Mar  5 01:27:44 2024, max compression
+gzip compressed data, was "django-mailinglist-0.1.7.tar", last modified: Fri Apr  5 16:25:54 2024, max compression
```

## Comparing `django-mailinglist-0.1.6.tar` & `django-mailinglist-0.1.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.510891 django-mailinglist-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-03-05 01:27:44.510891 django-mailinglist-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.510891 django-mailinglist-0.1.6/django_mailinglist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-03-05 01:27:44.000000 django-mailinglist-0.1.6/django_mailinglist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-05 01:27:44.000000 django-mailinglist-0.1.6/django_mailinglist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 01:27:44.000000 django-mailinglist-0.1.6/django_mailinglist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-05 01:27:44.000000 django-mailinglist-0.1.6/django_mailinglist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-05 01:27:44.000000 django-mailinglist-0.1.6/django_mailinglist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.502891 django-mailinglist-0.1.6/mailinglist/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.502891 django-mailinglist-0.1.6/mailinglist/addressimport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/addressimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/addressimport/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/admin_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.502891 django-mailinglist-0.1.6/mailinglist/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.502891 django-mailinglist-0.1.6/mailinglist/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/management/commands/process_submissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/migrations/0002_messageattachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/migrations/0003_alter_messagepart_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.498891 django-mailinglist-0.1.6/mailinglist/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.498891 django-mailinglist-0.1.6/mailinglist/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/message/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/message/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/preview.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/submission/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/submission/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/confirm_import_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/import_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.498891 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/global-deny/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/global-deny/subscribe.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/global-deny/subscribe.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/global-deny/subscribe_subject.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/message.html
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/message.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/message_subject.txt
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/subscribe.html
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/subscribe.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/subscribe_subject.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.506891 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/archive/archives.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/archive/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/archive/message.html
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/global_unsubscribe.html
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/global_unsubscribe_success.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/subscribe.html
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/subscribe_confirm.html
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/subscribe_success.html
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/subscriptions.html
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/unsubscribe.html
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/mailinglist/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 01:27:44.510891 django-mailinglist-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 01:27:44.510891 django-mailinglist-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_admin_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-03-05 01:27:39.000000 django-mailinglist-0.1.6/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.921029 django-mailinglist-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-05 16:25:54.921029 django-mailinglist-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.921029 django-mailinglist-0.1.7/django_mailinglist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-05 16:25:54.000000 django-mailinglist-0.1.7/django_mailinglist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-05 16:25:54.000000 django-mailinglist-0.1.7/django_mailinglist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:25:54.000000 django-mailinglist-0.1.7/django_mailinglist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 16:25:54.000000 django-mailinglist-0.1.7/django_mailinglist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 16:25:54.000000 django-mailinglist-0.1.7/django_mailinglist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/addressimport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/addressimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/addressimport/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/admin_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/management/commands/process_submissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/migrations/0002_messageattachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/migrations/0003_alter_messagepart_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15711 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.905029 django-mailinglist-0.1.7/mailinglist/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.905029 django-mailinglist-0.1.7/mailinglist/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/message/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/preview.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/submission/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/submission/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.913029 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/confirm_import_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/import_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.905029 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.917029 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.917029 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/global-deny/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/global-deny/subscribe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/global-deny/subscribe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/global-deny/subscribe_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/message.html
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/message.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/message_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/subscribe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/subscribe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/subscribe_subject.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.917029 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.917029 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/archive/archives.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/archive/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/archive/message.html
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/global_unsubscribe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/global_unsubscribe_success.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/subscribe.html
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/subscribe_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/subscribe_success.html
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/subscriptions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/unsubscribe.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/mailinglist/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:25:54.921029 django-mailinglist-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:25:54.921029 django-mailinglist-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_admin_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-05 16:25:49.000000 django-mailinglist-0.1.7/tests/test_views.py
```

### Comparing `django-mailinglist-0.1.6/CHANGELOG.md` & `django-mailinglist-0.1.7/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 ## [Unreleased]
 ### Added
 ### Changed
 ### Removed
 ### Fixed
 
 ## [0.1.6]
+### Fixed
+- Unsupported operator for MySQL database backend. (#11)
+
+## [0.1.6]
 ### Added
 - Link to manage subscriptions page from the unsubscribe page
 ### Removed
 - Some unnecssary code for dynamically importing modules
 ### Fixed
 - Documentation reference to management command
```

### Comparing `django-mailinglist-0.1.6/LICENSE.txt` & `django-mailinglist-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/PKG-INFO` & `django-mailinglist-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailinglist
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django app for managing multiple mailing lists with both plaintext as well as HTML templates (facilitated by Markdown).
 Home-page: http://github.com/thismatters/django-mailinglist/
 Author: Paul Stiverson
 Author-email: paul@thismatters.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -187,14 +187,18 @@
 ## [Unreleased]
 ### Added
 ### Changed
 ### Removed
 ### Fixed
 
 ## [0.1.6]
+### Fixed
+- Unsupported operator for MySQL database backend. (#11)
+
+## [0.1.6]
 ### Added
 - Link to manage subscriptions page from the unsubscribe page
 ### Removed
 - Some unnecssary code for dynamically importing modules
 ### Fixed
 - Documentation reference to management command
```

### Comparing `django-mailinglist-0.1.6/README.md` & `django-mailinglist-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/django_mailinglist.egg-info/PKG-INFO` & `django-mailinglist-0.1.7/django_mailinglist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mailinglist
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django app for managing multiple mailing lists with both plaintext as well as HTML templates (facilitated by Markdown).
 Home-page: http://github.com/thismatters/django-mailinglist/
 Author: Paul Stiverson
 Author-email: paul@thismatters.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -187,14 +187,18 @@
 ## [Unreleased]
 ### Added
 ### Changed
 ### Removed
 ### Fixed
 
 ## [0.1.6]
+### Fixed
+- Unsupported operator for MySQL database backend. (#11)
+
+## [0.1.6]
 ### Added
 - Link to manage subscriptions page from the unsubscribe page
 ### Removed
 - Some unnecssary code for dynamically importing modules
 ### Fixed
 - Documentation reference to management command
```

### Comparing `django-mailinglist-0.1.6/django_mailinglist.egg-info/SOURCES.txt` & `django-mailinglist-0.1.7/django_mailinglist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/addressimport/parsers.py` & `django-mailinglist-0.1.7/mailinglist/addressimport/parsers.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/admin.py` & `django-mailinglist-0.1.7/mailinglist/admin.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/admin_forms.py` & `django-mailinglist-0.1.7/mailinglist/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/conf.py` & `django-mailinglist-0.1.7/mailinglist/conf.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/forms.py` & `django-mailinglist-0.1.7/mailinglist/forms.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/hooks.py` & `django-mailinglist-0.1.7/mailinglist/hooks.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/migrations/0001_initial.py` & `django-mailinglist-0.1.7/mailinglist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/migrations/0002_messageattachment.py` & `django-mailinglist-0.1.7/mailinglist/migrations/0002_messageattachment.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/models.py` & `django-mailinglist-0.1.7/mailinglist/models.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/services.py` & `django-mailinglist-0.1.7/mailinglist/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         subscriptions = (
             submission.message.mailing_list.subscriptions.filter(
                 status=SubscriptionStatusEnum.SUBSCRIBED
             )
             # remove all global denies
             .filter(user__mailinglist_deny__isnull=True)
             # remove all excludes
-            .difference(submission.exclude.all())
+            .exclude(pk__in=submission.exclude.all().values_list("id", flat=True))
         )
         return subscriptions
 
     def _send_message(self, *, message, subscription, template_set, **kwargs):
         hookset.send_message(
             from_email=subscription.mailing_list.sender_tag,
             **MessageService().prepare_message_kwargs(
```

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/preview.html` & `django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/preview.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/confirm_import_form.html` & `django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/confirm_import_form.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/admin/mailinglist/subscription/import_form.html` & `django-mailinglist-0.1.7/mailinglist/templates/admin/mailinglist/subscription/import_form.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/mailinglist/email/message.html` & `django-mailinglist-0.1.7/mailinglist/templates/mailinglist/email/message.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/archive/message.html` & `django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/archive/message.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/templates/mailinglist/web/unsubscribe.html` & `django-mailinglist-0.1.7/mailinglist/templates/mailinglist/web/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/urls.py` & `django-mailinglist-0.1.7/mailinglist/urls.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/mailinglist/views.py` & `django-mailinglist-0.1.7/mailinglist/views.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/setup.py` & `django-mailinglist-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_admin.py` & `django-mailinglist-0.1.7/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_admin_forms.py` & `django-mailinglist-0.1.7/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_conf.py` & `django-mailinglist-0.1.7/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_forms.py` & `django-mailinglist-0.1.7/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_hooks.py` & `django-mailinglist-0.1.7/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_misc.py` & `django-mailinglist-0.1.7/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_models.py` & `django-mailinglist-0.1.7/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_parsers.py` & `django-mailinglist-0.1.7/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_services.py` & `django-mailinglist-0.1.7/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `django-mailinglist-0.1.6/tests/test_views.py` & `django-mailinglist-0.1.7/tests/test_views.py`

 * *Files identical despite different names*

