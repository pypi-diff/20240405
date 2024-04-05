# Comparing `tmp/djangoldp_notification-3.1.2.tar.gz` & `tmp/djangoldp_notification-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_notification-3.1.2.tar", last modified: Mon Feb  5 09:16:46 2024, max compression
+gzip compressed data, was "djangoldp_notification-3.1.3.tar", last modified: Fri Apr  5 15:37:11 2024, max compression
```

## Comparing `djangoldp_notification-3.1.2.tar` & `djangoldp_notification-3.1.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      341 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5648 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.652213 djangoldp_notification-3.1.2/djangoldp_notification/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-05 09:16:43.000000 djangoldp_notification-3.1.2/djangoldp_notification/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3372 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.648213 djangoldp_notification-3.1.2/djangoldp_notification/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.648213 djangoldp_notification-3.1.2/djangoldp_notification/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.652213 djangoldp_notification-3.1.2/djangoldp_notification/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      872 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.648213 djangoldp_notification-3.1.2/djangoldp_notification/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.652213 djangoldp_notification-3.1.2/djangoldp_notification/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.648213 djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.652213 djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1313 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.648213 djangoldp_notification-3.1.2/djangoldp_notification/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.656214 djangoldp_notification-3.1.2/djangoldp_notification/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/management/commands/create_subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/management/commands/mock_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/management/commands/suppress_old_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/djangoldp_notification/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1832 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0002_auto_20190917_1107.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0003_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0004_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0005_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0006_subscription_parent.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0007_auto_20200604_1055.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0008_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0009_auto_20200619_0802.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0010_notificationsetting.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0011_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0012_auto_20210729_1912.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0013_auto_20211016_1203.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0015_alter_subscription_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/0016_alter_notification_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13638 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/models.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/djangoldp_notification/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/djangoldp_notification/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/djangoldp_notification/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/scripts/generate_inbox_fixture.py
--rw-rw-rw-   0 root         (0) root         (0)     4000 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1911 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/tests/test_subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1962 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/djangoldp_notification/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 09:16:46.652213 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2024-02-05 09:16:46.000000 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2651 2024-02-05 09:16:46.000000 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 09:16:46.000000 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2024-02-05 09:16:46.000000 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-02-05 09:16:46.000000 djangoldp_notification-3.1.2/djangoldp_notification.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-02-05 09:16:46.660214 djangoldp_notification-3.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-05 09:16:24.000000 djangoldp_notification-3.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      341 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.582334 djangoldp_notification-3.1.3/djangoldp_notification/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-05 15:37:09.000000 djangoldp_notification-3.1.3/djangoldp_notification/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.578334 djangoldp_notification-3.1.3/djangoldp_notification/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.574334 djangoldp_notification-3.1.3/djangoldp_notification/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.582334 djangoldp_notification-3.1.3/djangoldp_notification/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.578334 djangoldp_notification-3.1.3/djangoldp_notification/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.582334 djangoldp_notification-3.1.3/djangoldp_notification/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.578334 djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.582334 djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.578334 djangoldp_notification-3.1.3/djangoldp_notification/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.586334 djangoldp_notification-3.1.3/djangoldp_notification/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/management/commands/create_subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/management/commands/mock_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/management/commands/suppress_old_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/djangoldp_notification/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0002_auto_20190917_1107.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0003_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0004_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0005_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0006_subscription_parent.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0007_auto_20200604_1055.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0008_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0009_auto_20200619_0802.py
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0010_notificationsetting.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0011_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0012_auto_20210729_1912.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0013_auto_20211016_1203.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0015_alter_subscription_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/0016_alter_notification_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13638 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/djangoldp_notification/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/djangoldp_notification/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/djangoldp_notification/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/scripts/generate_inbox_fixture.py
+-rw-rw-rw-   0 root         (0) root         (0)     4000 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/tests/test_subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/djangoldp_notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:37:11.582334 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2024-04-05 15:37:11.000000 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-05 15:37:11.000000 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 15:37:11.000000 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-05 15:37:11.000000 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-05 15:37:11.000000 djangoldp_notification-3.1.3/djangoldp_notification.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-05 15:37:11.590334 djangoldp_notification-3.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-05 15:36:53.000000 djangoldp_notification-3.1.3/setup.py
```

### Comparing `djangoldp_notification-3.1.2/README.md` & `djangoldp_notification-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/admin.py` & `djangoldp_notification-3.1.3/djangoldp_notification/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/check_integrity.py` & `djangoldp_notification-3.1.3/djangoldp_notification/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/factories.py` & `djangoldp_notification-3.1.3/djangoldp_notification/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/locale/en/LC_MESSAGES/django.mo` & `djangoldp_notification-3.1.3/djangoldp_notification/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/locale/en/LC_MESSAGES/django.po` & `djangoldp_notification-3.1.3/djangoldp_notification/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/locale/es/LC_MESSAGES/django.po` & `djangoldp_notification-3.1.3/djangoldp_notification/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/locale/fr/LC_MESSAGES/django.po` & `djangoldp_notification-3.1.3/djangoldp_notification/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/management/commands/create_subscriptions.py` & `djangoldp_notification-3.1.3/djangoldp_notification/management/commands/create_subscriptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,20 +31,18 @@
     try:
         sub = Subscription.objects.get(object="{}/project-members/".format(host))
         sub.delete()
     except Subscription.DoesNotExist:
         pass
 
     # Allow us to manage general information about circles and projects like name, jabberIDs, description, etc.
-    Subscription.objects.get_or_create(object=host+"/circles/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_admin", field=None)
-    Subscription.objects.get_or_create(object=host+"/projects/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_muc_admin", field=None)
+    Subscription.objects.get_or_create(object=host+"/circles/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_groups_muc_admin", field=None)
+    Subscription.objects.get_or_create(object=host+"/projects/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_groups_muc_admin", field=None)
 
     # The management of circle and projets members now comes from management of groups
     Subscription.objects.get_or_create(object=host+"/groups/", inbox=xmpp + "/conference." + jabber_host + "/startinblox_groups_muc_members_admin", field=None)
     
     # Allow us to manage general information about users, like their names, jabberID, avatars, etc.
-    Subscription.objects.get_or_create(object=host+"/users/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field=None)
-    Subscription.objects.get_or_create(object=host+"/profiles/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
-    Subscription.objects.get_or_create(object=host+"/chatprofiles/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
-    Subscription.objects.get_or_create(object=host+"/accounts/", inbox=xmpp + "/" + jabber_host + "/happydev_user_admin", field="user")
-
+    Subscription.objects.get_or_create(object=host+"/users/", inbox=xmpp + "/" + jabber_host + "/startinblox_groups_user_admin", field=None)
+    
+    # When we change an information about the user (like avatar and so on) we want to notify prosody
     self.stdout.write(self.style.SUCCESS("Successfully  created subscriptions\nhost: "+host+"\nxmpp server: "+xmpp+"\njabber host: "+jabber_host))
```

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/management/commands/suppress_old_notifications.py` & `djangoldp_notification-3.1.3/djangoldp_notification/management/commands/suppress_old_notifications.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0001_initial.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0002_auto_20190917_1107.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0002_auto_20190917_1107.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0003_auto_20200429_1346.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0003_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0004_auto_20200501_1207.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0004_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0005_auto_20200505_1733.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0005_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0006_subscription_parent.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0006_subscription_parent.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0007_auto_20200604_1055.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0007_auto_20200604_1055.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0008_auto_20200610_1323.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0008_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0009_auto_20200619_0802.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0009_auto_20200619_0802.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0010_notificationsetting.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0010_notificationsetting.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0011_auto_20210218_1145.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0011_auto_20210218_1145.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0013_auto_20211016_1203.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0013_auto_20211016_1203.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0014_subscription_disable_automatic_notifications.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/migrations/0016_alter_notification_options_and_more.py` & `djangoldp_notification-3.1.3/djangoldp_notification/migrations/0016_alter_notification_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/models.py` & `djangoldp_notification-3.1.3/djangoldp_notification/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/templates/email.html` & `djangoldp_notification-3.1.3/djangoldp_notification/templates/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/tests/runner.py` & `djangoldp_notification-3.1.3/djangoldp_notification/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/tests/scripts/generate_inbox_fixture.py` & `djangoldp_notification-3.1.3/djangoldp_notification/tests/scripts/generate_inbox_fixture.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/tests/test_cache.py` & `djangoldp_notification-3.1.3/djangoldp_notification/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/tests/test_models.py` & `djangoldp_notification-3.1.3/djangoldp_notification/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/tests/test_subscriptions.py` & `djangoldp_notification-3.1.3/djangoldp_notification/tests/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification/views.py` & `djangoldp_notification-3.1.3/djangoldp_notification/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/djangoldp_notification.egg-info/SOURCES.txt` & `djangoldp_notification-3.1.3/djangoldp_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_notification-3.1.2/setup.cfg` & `djangoldp_notification-3.1.3/setup.cfg`

 * *Files identical despite different names*

