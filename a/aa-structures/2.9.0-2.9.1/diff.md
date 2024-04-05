# Comparing `tmp/aa_structures-2.9.0.tar.gz` & `tmp/aa_structures-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_structures-2.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_structures-2.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_structures-2.9.0.tar` & `aa_structures-2.9.1.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0     1070 2020-10-22 17:29:44.465193 aa_structures-2.9.0/LICENSE
--rw-r--r--   0        0        0     4380 2023-12-15 20:30:58.098830 aa_structures-2.9.0/README.md
--rw-r--r--   0        0        0     2385 2023-11-28 20:06:52.952934 aa_structures-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      203 2024-03-21 17:07:26.809358 aa_structures-2.9.0/structures/__init__.py
--rw-r--r--   0        0        0    38662 2024-02-28 15:39:22.070321 aa_structures-2.9.0/structures/admin.py
--rw-r--r--   0        0        0     6526 2023-12-15 20:30:58.102830 aa_structures-2.9.0/structures/app_settings.py
--rw-r--r--   0        0        0      195 2023-07-27 19:27:24.171062 aa_structures-2.9.0/structures/apps.py
--rw-r--r--   0        0        0      915 2022-03-01 14:58:19.767220 aa_structures-2.9.0/structures/auth_hooks.py
--rw-r--r--   0        0        0      967 2023-11-08 17:26:27.194851 aa_structures-2.9.0/structures/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.063868 aa_structures-2.9.0/structures/core/__init__.py
--rw-r--r--   0        0        0      131 2023-07-28 01:22:06.039331 aa_structures-2.9.0/structures/core/notification_embeds/__init__.py
--rw-r--r--   0        0        0     5164 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/billing_embeds.py
--rw-r--r--   0        0        0     6098 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/corporate_embeds.py
--rw-r--r--   0        0        0     2974 2023-08-01 13:22:15.295910 aa_structures-2.9.0/structures/core/notification_embeds/helpers.py
--rw-r--r--   0        0        0    15233 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/main.py
--rw-r--r--   0        0        0     7130 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/moonmining_embeds.py
--rw-r--r--   0        0        0     2864 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/orbital_embeds.py
--rw-r--r--   0        0        0     8901 2024-03-01 16:31:33.199958 aa_structures-2.9.0/structures/core/notification_embeds/sov_embeds.py
--rw-r--r--   0        0        0    13236 2024-03-01 16:31:33.203958 aa_structures-2.9.0/structures/core/notification_embeds/structures_embeds.py
--rw-r--r--   0        0        0     5848 2024-03-01 16:31:33.203958 aa_structures-2.9.0/structures/core/notification_embeds/tower_embeds.py
--rw-r--r--   0        0        0    18333 2024-03-01 16:31:33.203958 aa_structures-2.9.0/structures/core/notification_embeds/war_embeds.py
--rw-r--r--   0        0        0    14977 2023-10-29 21:57:09.516747 aa_structures-2.9.0/structures/core/notification_timers.py
--rw-r--r--   0        0        0    12279 2024-02-28 15:39:22.074321 aa_structures-2.9.0/structures/core/notification_types.py
--rw-r--r--   0        0        0    20965 2023-11-11 19:07:33.644666 aa_structures-2.9.0/structures/core/serializers.py
--rw-r--r--   0        0        0      730 2023-07-28 01:22:06.043331 aa_structures-2.9.0/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1757 2023-07-28 01:22:06.043331 aa_structures-2.9.0/structures/core/starbases.py
--rw-r--r--   0        0        0      391 2024-03-21 13:54:34.393674 aa_structures-2.9.0/structures/forms.py
--rw-r--r--   0        0        0     2344 2024-03-01 16:31:33.203958 aa_structures-2.9.0/structures/helpers.py
--rw-r--r--   0        0        0     3997 2023-11-22 16:33:02.505646 aa_structures-2.9.0/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    69625 2024-03-01 16:31:33.203958 aa_structures-2.9.0/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.207958 aa_structures-2.9.0/structures/locale/django.pot
--rw-r--r--   0        0        0      380 2020-10-22 17:29:44.473193 aa_structures-2.9.0/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68415 2024-03-01 16:31:33.207958 aa_structures-2.9.0/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      871 2023-10-29 21:57:09.520747 aa_structures-2.9.0/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68633 2024-03-01 16:31:33.207958 aa_structures-2.9.0/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-10-29 21:57:09.520747 aa_structures-2.9.0/structures/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.207958 aa_structures-2.9.0/structures/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-10-29 21:57:09.524747 aa_structures-2.9.0/structures/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.211958 aa_structures-2.9.0/structures/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-10-29 21:57:09.528747 aa_structures-2.9.0/structures/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68408 2024-03-01 16:31:33.211958 aa_structures-2.9.0/structures/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-10-29 21:57:09.532747 aa_structures-2.9.0/structures/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68365 2024-03-01 16:31:33.211958 aa_structures-2.9.0/structures/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    71503 2024-03-01 16:31:33.215958 aa_structures-2.9.0/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   105690 2024-03-01 16:31:33.215958 aa_structures-2.9.0/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-10-29 21:57:09.540747 aa_structures-2.9.0/structures/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    68583 2024-03-01 16:31:33.215958 aa_structures-2.9.0/structures/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2869 2023-11-22 16:33:02.517646 aa_structures-2.9.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    69175 2024-03-01 16:31:33.215958 aa_structures-2.9.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.067868 aa_structures-2.9.0/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1507 2023-07-28 01:22:06.047331 aa_structures-2.9.0/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2489 2023-07-28 01:22:06.047331 aa_structures-2.9.0/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0     1306 2023-10-06 22:12:34.657204 aa_structures-2.9.0/structures/management/commands/structures_update_poco_planets.py
--rw-r--r--   0        0        0    19225 2023-11-10 19:24:15.537817 aa_structures-2.9.0/structures/managers.py
--rw-r--r--   0        0        0    59315 2023-04-17 14:02:22.882798 aa_structures-2.9.0/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2023-04-16 22:10:32.169268 aa_structures-2.9.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2023-04-17 00:48:58.414803 aa_structures-2.9.0/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0    14014 2023-10-30 19:14:39.710888 aa_structures-2.9.0/structures/migrations/0004_improve_localization.py
--rw-r--r--   0        0        0     7087 2024-03-21 13:54:34.393674 aa_structures-2.9.0/structures/migrations/0005_add_notification_types.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.067868 aa_structures-2.9.0/structures/migrations/__init__.py
--rw-r--r--   0        0        0      916 2023-07-28 16:06:53.294037 aa_structures-2.9.0/structures/models/__init__.py
--rw-r--r--   0        0        0     2213 2024-03-21 13:54:34.397674 aa_structures-2.9.0/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    35146 2024-02-28 15:39:22.078321 aa_structures-2.9.0/structures/models/notifications.py
--rw-r--r--   0        0        0    53885 2023-11-08 01:50:09.357360 aa_structures-2.9.0/structures/models/owners.py
--rw-r--r--   0        0        0    29778 2023-11-10 22:55:33.220343 aa_structures-2.9.0/structures/models/structures_1.py
--rw-r--r--   0        0        0    10371 2023-11-08 17:26:27.198851 aa_structures-2.9.0/structures/models/structures_2.py
--rw-r--r--   0        0        0      317 2023-07-28 01:22:06.051331 aa_structures-2.9.0/structures/providers.py
--rw-r--r--   0        0        0     1165 2022-05-30 21:05:57.989637 aa_structures-2.9.0/structures/static/structures/css/global.css
--rw-r--r--   0        0        0      303 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/css/main.css
--rw-r--r--   0        0        0      220 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/css/public.css
--rw-r--r--   0        0        0     1646 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/css/statistics.css
--rw-r--r--   0        0        0     1657 2023-11-07 03:14:21.126079 aa_structures-2.9.0/structures/static/structures/css/structures.css
--rw-r--r--   0        0        0     1151 2023-11-04 23:59:12.684284 aa_structures-2.9.0/structures/static/structures/img/bars-rotate-fade-black-36.svg
--rw-r--r--   0        0        0     1163 2023-11-04 23:59:12.684284 aa_structures-2.9.0/structures/static/structures/img/bars-rotate-fade-white-36.svg
--rw-r--r--   0        0        0      908 2021-04-29 22:23:58.269246 aa_structures-2.9.0/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2023-04-16 23:43:18.808312 aa_structures-2.9.0/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2023-04-16 23:43:18.812312 aa_structures-2.9.0/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2023-04-16 23:43:18.816312 aa_structures-2.9.0/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2023-04-16 23:43:18.820312 aa_structures-2.9.0/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      496 2021-04-29 22:23:58.277247 aa_structures-2.9.0/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0     1842 2023-11-07 13:45:35.438148 aa_structures-2.9.0/structures/static/structures/js/global.js
--rw-r--r--   0        0        0     3746 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/static/structures/js/public.js
--rw-r--r--   0        0        0     2857 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/static/structures/js/statistics.js
--rw-r--r--   0        0        0    15089 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/static/structures/js/structures.js
--rw-r--r--   0        0        0     5573 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2023-11-05 23:04:11.662712 aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2023-11-05 23:04:11.666712 aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0     9083 2023-11-10 05:57:15.194459 aa_structures-2.9.0/structures/tasks.py
--rw-r--r--   0        0        0      337 2023-11-05 21:34:20.161309 aa_structures-2.9.0/structures/templates/structures/base.html
--rw-r--r--   0        0        0      264 2022-06-01 20:12:19.043382 aa_structures-2.9.0/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2023-04-16 23:43:18.824312 aa_structures-2.9.0/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2022-06-01 20:12:19.043382 aa_structures-2.9.0/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2022-06-01 20:12:19.047382 aa_structures-2.9.0/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4102 2023-11-05 01:27:47.245854 aa_structures-2.9.0/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0     2324 2023-11-05 04:28:31.217677 aa_structures-2.9.0/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0      596 2023-11-05 01:27:47.245854 aa_structures-2.9.0/structures/templates/structures/modals/tab_services_detail.html
--rw-r--r--   0        0        0     2329 2023-11-06 16:53:40.678662 aa_structures-2.9.0/structures/templates/structures/partials/menu.html
--rw-r--r--   0        0        0     1222 2023-11-06 16:53:40.682662 aa_structures-2.9.0/structures/templates/structures/partials/public/poco_list.html
--rw-r--r--   0        0        0     1133 2023-11-06 16:53:40.682662 aa_structures-2.9.0/structures/templates/structures/partials/statistics/structure_summary.html
--rw-r--r--   0        0        0      106 2023-11-06 16:53:40.682662 aa_structures-2.9.0/structures/templates/structures/partials/structures/active_tags.html
--rw-r--r--   0        0        0     1470 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/partials/structures/jump_gates_list.html
--rw-r--r--   0        0        0     1077 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/partials/structures/poco_list.html
--rw-r--r--   0        0        0     1417 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/partials/structures/starbase_list.html
--rw-r--r--   0        0        0     1421 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/partials/structures/structure_list.html
--rw-r--r--   0        0        0     3233 2023-11-07 13:45:35.438148 aa_structures-2.9.0/structures/templates/structures/public.html
--rw-r--r--   0        0        0     1736 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/statistics.html
--rw-r--r--   0        0        0     8322 2023-11-07 03:14:21.130079 aa_structures-2.9.0/structures/templates/structures/structures.html
--rw-r--r--   0        0        0      117 2022-05-31 14:09:14.519367 aa_structures-2.9.0/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2022-06-01 20:12:19.047382 aa_structures-2.9.0/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2022-06-01 15:59:29.634387 aa_structures-2.9.0/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2023-04-16 22:10:32.185268 aa_structures-2.9.0/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2022-05-30 21:05:57.993637 aa_structures-2.9.0/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.071868 aa_structures-2.9.0/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1637 2023-07-28 01:22:06.051331 aa_structures-2.9.0/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2020-10-22 17:29:44.485193 aa_structures-2.9.0/structures/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/core/notification_embeds/__init__.py
--rw-r--r--   0        0        0     1776 2023-11-10 05:57:15.194459 aa_structures-2.9.0/structures/tests/core/notification_embeds/test_helpers.py
--rw-r--r--   0        0        0    13808 2024-02-29 22:16:28.663517 aa_structures-2.9.0/structures/tests/core/notification_embeds/test_main.py
--rw-r--r--   0        0        0    10857 2023-11-30 15:47:14.138045 aa_structures-2.9.0/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     9881 2023-07-28 16:06:53.302038 aa_structures-2.9.0/structures/tests/core/test_notification_types.py
--rw-r--r--   0        0        0     5583 2023-11-30 15:47:14.138045 aa_structures-2.9.0/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     7056 2023-11-30 15:47:14.138045 aa_structures-2.9.0/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      821 2023-07-28 01:22:06.051331 aa_structures-2.9.0/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3186 2023-11-30 15:47:14.138045 aa_structures-2.9.0/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/integration/__init__.py
--rw-r--r--   0        0        0    23588 2023-11-30 15:47:14.138045 aa_structures-2.9.0/structures/tests/integration/test_tasks.py
--rw-r--r--   0        0        0     4331 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/integration/test_views.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1623 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    30300 2024-02-29 22:16:28.667517 aa_structures-2.9.0/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31989 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     7257 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5551 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    21796 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    21911 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    16947 2023-11-30 15:47:14.142045 aa_structures-2.9.0/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    18831 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/models/test_owners_4.py
--rw-r--r--   0        0        0    31607 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/models/test_owners_5.py
--rw-r--r--   0        0        0    41469 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0    24333 2023-11-28 20:06:52.956934 aa_structures-2.9.0/structures/tests/test_admin.py
--rw-r--r--   0        0        0     4893 2024-03-01 16:31:33.219958 aa_structures-2.9.0/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    34539 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     2942 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/test_managers_2.py
--rw-r--r--   0        0        0    17269 2023-11-30 15:47:14.146045 aa_structures-2.9.0/structures/tests/test_tasks.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2129 2023-10-06 22:12:34.661204 aa_structures-2.9.0/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    32147 2024-02-29 22:16:28.667517 aa_structures-2.9.0/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2022-08-10 19:36:18.186258 aa_structures-2.9.0/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   993284 2023-10-06 22:12:34.665204 aa_structures-2.9.0/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    24718 2023-11-16 00:12:49.124741 aa_structures-2.9.0/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0     5746 2022-09-10 17:58:40.522747 aa_structures-2.9.0/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1413 2023-11-10 05:57:15.214459 aa_structures-2.9.0/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     9134 2023-11-16 00:12:49.128741 aa_structures-2.9.0/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0     6183 2024-03-21 13:54:34.397674 aa_structures-2.9.0/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2022-08-10 15:32:14.940423 aa_structures-2.9.0/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2021-03-24 18:47:30.630666 aa_structures-2.9.0/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2020-10-22 17:29:44.489193 aa_structures-2.9.0/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/tests/views/__init__.py
--rw-r--r--   0        0        0     1372 2023-11-30 15:47:14.150045 aa_structures-2.9.0/structures/tests/views/test_public.py
--rw-r--r--   0        0        0     2626 2023-11-30 15:47:14.150045 aa_structures-2.9.0/structures/tests/views/test_statistics.py
--rw-r--r--   0        0        0    29004 2023-11-30 15:47:14.150045 aa_structures-2.9.0/structures/tests/views/test_structures.py
--rw-r--r--   0        0        0      247 2023-11-07 13:45:35.442148 aa_structures-2.9.0/structures/tests/views/utils.py
--rw-r--r--   0        0        0     1396 2023-11-07 13:45:35.442148 aa_structures-2.9.0/structures/urls.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.075868 aa_structures-2.9.0/structures/views/__init__.py
--rw-r--r--   0        0        0      818 2023-11-11 19:07:33.648666 aa_structures-2.9.0/structures/views/common.py
--rw-r--r--   0        0        0     3035 2023-11-11 19:07:33.648666 aa_structures-2.9.0/structures/views/public.py
--rw-r--r--   0        0        0     4709 2023-11-11 19:07:33.648666 aa_structures-2.9.0/structures/views/statistics.py
--rw-r--r--   0        0        0    23167 2023-11-11 19:07:33.648666 aa_structures-2.9.0/structures/views/structures.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.079868 aa_structures-2.9.0/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6573 2023-08-01 12:33:06.799354 aa_structures-2.9.0/structures/webhooks/core.py
--rw-r--r--   0        0        0     1117 2023-07-28 22:31:18.481156 aa_structures-2.9.0/structures/webhooks/managers.py
--rw-r--r--   0        0        0     2067 2023-11-28 20:06:52.972934 aa_structures-2.9.0/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2024-03-21 17:23:53.079868 aa_structures-2.9.0/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6762 2023-11-28 20:06:52.972934 aa_structures-2.9.0/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2021-02-14 22:48:19.121024 aa_structures-2.9.0/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 aa_structures-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-10-22 17:29:44.465193 aa_structures-2.9.1/LICENSE
+-rw-r--r--   0        0        0     4380 2023-12-15 20:30:58.098830 aa_structures-2.9.1/README.md
+-rw-r--r--   0        0        0     2385 2023-11-28 20:06:52.952934 aa_structures-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-03-29 16:15:34.305984 aa_structures-2.9.1/structures/__init__.py
+-rw-r--r--   0        0        0    38662 2024-02-28 15:39:22.070321 aa_structures-2.9.1/structures/admin.py
+-rw-r--r--   0        0        0     6526 2023-12-15 20:30:58.102830 aa_structures-2.9.1/structures/app_settings.py
+-rw-r--r--   0        0        0      195 2023-07-27 19:27:24.171062 aa_structures-2.9.1/structures/apps.py
+-rw-r--r--   0        0        0      915 2022-03-01 14:58:19.767220 aa_structures-2.9.1/structures/auth_hooks.py
+-rw-r--r--   0        0        0      967 2023-11-08 17:26:27.194851 aa_structures-2.9.1/structures/constants.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:00.976997 aa_structures-2.9.1/structures/core/__init__.py
+-rw-r--r--   0        0        0      131 2023-07-28 01:22:06.039331 aa_structures-2.9.1/structures/core/notification_embeds/__init__.py
+-rw-r--r--   0        0        0     5164 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/billing_embeds.py
+-rw-r--r--   0        0        0     6098 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/corporate_embeds.py
+-rw-r--r--   0        0        0     2974 2023-08-01 13:22:15.295910 aa_structures-2.9.1/structures/core/notification_embeds/helpers.py
+-rw-r--r--   0        0        0    15233 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/main.py
+-rw-r--r--   0        0        0     7130 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/moonmining_embeds.py
+-rw-r--r--   0        0        0     2864 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/orbital_embeds.py
+-rw-r--r--   0        0        0     8901 2024-03-01 16:31:33.199958 aa_structures-2.9.1/structures/core/notification_embeds/sov_embeds.py
+-rw-r--r--   0        0        0    13236 2024-03-01 16:31:33.203958 aa_structures-2.9.1/structures/core/notification_embeds/structures_embeds.py
+-rw-r--r--   0        0        0     5848 2024-03-01 16:31:33.203958 aa_structures-2.9.1/structures/core/notification_embeds/tower_embeds.py
+-rw-r--r--   0        0        0    18333 2024-03-01 16:31:33.203958 aa_structures-2.9.1/structures/core/notification_embeds/war_embeds.py
+-rw-r--r--   0        0        0    14977 2023-10-29 21:57:09.516747 aa_structures-2.9.1/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    12279 2024-02-28 15:39:22.074321 aa_structures-2.9.1/structures/core/notification_types.py
+-rw-r--r--   0        0        0    20965 2023-11-11 19:07:33.644666 aa_structures-2.9.1/structures/core/serializers.py
+-rw-r--r--   0        0        0      730 2023-07-28 01:22:06.043331 aa_structures-2.9.1/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1757 2023-07-28 01:22:06.043331 aa_structures-2.9.1/structures/core/starbases.py
+-rw-r--r--   0        0        0      391 2024-03-21 13:54:34.393674 aa_structures-2.9.1/structures/forms.py
+-rw-r--r--   0        0        0     2344 2024-03-01 16:31:33.203958 aa_structures-2.9.1/structures/helpers.py
+-rw-r--r--   0        0        0     3997 2023-11-22 16:33:02.505646 aa_structures-2.9.1/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    69625 2024-03-01 16:31:33.203958 aa_structures-2.9.1/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.207958 aa_structures-2.9.1/structures/locale/django.pot
+-rw-r--r--   0        0        0      380 2020-10-22 17:29:44.473193 aa_structures-2.9.1/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68415 2024-03-01 16:31:33.207958 aa_structures-2.9.1/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      871 2023-10-29 21:57:09.520747 aa_structures-2.9.1/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68633 2024-03-01 16:31:33.207958 aa_structures-2.9.1/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-10-29 21:57:09.520747 aa_structures-2.9.1/structures/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.207958 aa_structures-2.9.1/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-10-29 21:57:09.524747 aa_structures-2.9.1/structures/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68368 2024-03-01 16:31:33.211958 aa_structures-2.9.1/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-10-29 21:57:09.528747 aa_structures-2.9.1/structures/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68408 2024-03-01 16:31:33.211958 aa_structures-2.9.1/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-10-29 21:57:09.532747 aa_structures-2.9.1/structures/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68365 2024-03-01 16:31:33.211958 aa_structures-2.9.1/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    71503 2024-03-01 16:31:33.215958 aa_structures-2.9.1/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   105690 2024-03-01 16:31:33.215958 aa_structures-2.9.1/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2023-10-29 21:57:09.540747 aa_structures-2.9.1/structures/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    68583 2024-03-01 16:31:33.215958 aa_structures-2.9.1/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2869 2023-11-22 16:33:02.517646 aa_structures-2.9.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    69175 2024-03-01 16:31:33.215958 aa_structures-2.9.1/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:00.988997 aa_structures-2.9.1/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1507 2023-07-28 01:22:06.047331 aa_structures-2.9.1/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2489 2023-07-28 01:22:06.047331 aa_structures-2.9.1/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0     1306 2023-10-06 22:12:34.657204 aa_structures-2.9.1/structures/management/commands/structures_update_poco_planets.py
+-rw-r--r--   0        0        0    19225 2023-11-10 19:24:15.537817 aa_structures-2.9.1/structures/managers.py
+-rw-r--r--   0        0        0    59315 2023-04-17 14:02:22.882798 aa_structures-2.9.1/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2023-04-16 22:10:32.169268 aa_structures-2.9.1/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2023-04-17 00:48:58.414803 aa_structures-2.9.1/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0    14014 2023-10-30 19:14:39.710888 aa_structures-2.9.1/structures/migrations/0004_improve_localization.py
+-rw-r--r--   0        0        0     7087 2024-03-21 13:54:34.393674 aa_structures-2.9.1/structures/migrations/0005_add_notification_types.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:00.992997 aa_structures-2.9.1/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-28 16:06:53.294037 aa_structures-2.9.1/structures/models/__init__.py
+-rw-r--r--   0        0        0     2213 2024-03-21 13:54:34.397674 aa_structures-2.9.1/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    35146 2024-02-28 15:39:22.078321 aa_structures-2.9.1/structures/models/notifications.py
+-rw-r--r--   0        0        0    53953 2024-03-29 16:15:34.309984 aa_structures-2.9.1/structures/models/owners.py
+-rw-r--r--   0        0        0    29778 2023-11-10 22:55:33.220343 aa_structures-2.9.1/structures/models/structures_1.py
+-rw-r--r--   0        0        0    10371 2023-11-08 17:26:27.198851 aa_structures-2.9.1/structures/models/structures_2.py
+-rw-r--r--   0        0        0      317 2023-07-28 01:22:06.051331 aa_structures-2.9.1/structures/providers.py
+-rw-r--r--   0        0        0     1165 2022-05-30 21:05:57.989637 aa_structures-2.9.1/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0      303 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0      220 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/css/public.css
+-rw-r--r--   0        0        0     1646 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/css/statistics.css
+-rw-r--r--   0        0        0     1657 2023-11-07 03:14:21.126079 aa_structures-2.9.1/structures/static/structures/css/structures.css
+-rw-r--r--   0        0        0     1151 2023-11-04 23:59:12.684284 aa_structures-2.9.1/structures/static/structures/img/bars-rotate-fade-black-36.svg
+-rw-r--r--   0        0        0     1163 2023-11-04 23:59:12.684284 aa_structures-2.9.1/structures/static/structures/img/bars-rotate-fade-white-36.svg
+-rw-r--r--   0        0        0      908 2021-04-29 22:23:58.269246 aa_structures-2.9.1/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2023-04-16 23:43:18.808312 aa_structures-2.9.1/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2023-04-16 23:43:18.812312 aa_structures-2.9.1/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2023-04-16 23:43:18.816312 aa_structures-2.9.1/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2023-04-16 23:43:18.820312 aa_structures-2.9.1/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      496 2021-04-29 22:23:58.277247 aa_structures-2.9.1/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0     1842 2023-11-07 13:45:35.438148 aa_structures-2.9.1/structures/static/structures/js/global.js
+-rw-r--r--   0        0        0     3746 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/static/structures/js/public.js
+-rw-r--r--   0        0        0     2857 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/static/structures/js/statistics.js
+-rw-r--r--   0        0        0    15089 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/static/structures/js/structures.js
+-rw-r--r--   0        0        0     5573 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2023-11-05 23:04:11.662712 aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2023-11-05 23:04:11.666712 aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0     9083 2023-11-10 05:57:15.194459 aa_structures-2.9.1/structures/tasks.py
+-rw-r--r--   0        0        0      337 2023-11-05 21:34:20.161309 aa_structures-2.9.1/structures/templates/structures/base.html
+-rw-r--r--   0        0        0      264 2022-06-01 20:12:19.043382 aa_structures-2.9.1/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2023-04-16 23:43:18.824312 aa_structures-2.9.1/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2022-06-01 20:12:19.043382 aa_structures-2.9.1/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2022-06-01 20:12:19.047382 aa_structures-2.9.1/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4102 2023-11-05 01:27:47.245854 aa_structures-2.9.1/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0     2324 2023-11-05 04:28:31.217677 aa_structures-2.9.1/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0      596 2023-11-05 01:27:47.245854 aa_structures-2.9.1/structures/templates/structures/modals/tab_services_detail.html
+-rw-r--r--   0        0        0     2329 2023-11-06 16:53:40.678662 aa_structures-2.9.1/structures/templates/structures/partials/menu.html
+-rw-r--r--   0        0        0     1222 2023-11-06 16:53:40.682662 aa_structures-2.9.1/structures/templates/structures/partials/public/poco_list.html
+-rw-r--r--   0        0        0     1133 2023-11-06 16:53:40.682662 aa_structures-2.9.1/structures/templates/structures/partials/statistics/structure_summary.html
+-rw-r--r--   0        0        0      106 2023-11-06 16:53:40.682662 aa_structures-2.9.1/structures/templates/structures/partials/structures/active_tags.html
+-rw-r--r--   0        0        0     1470 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/partials/structures/jump_gates_list.html
+-rw-r--r--   0        0        0     1077 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/partials/structures/poco_list.html
+-rw-r--r--   0        0        0     1417 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/partials/structures/starbase_list.html
+-rw-r--r--   0        0        0     1421 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/partials/structures/structure_list.html
+-rw-r--r--   0        0        0     3233 2023-11-07 13:45:35.438148 aa_structures-2.9.1/structures/templates/structures/public.html
+-rw-r--r--   0        0        0     1736 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/statistics.html
+-rw-r--r--   0        0        0     8322 2023-11-07 03:14:21.130079 aa_structures-2.9.1/structures/templates/structures/structures.html
+-rw-r--r--   0        0        0      117 2022-05-31 14:09:14.519367 aa_structures-2.9.1/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2022-06-01 20:12:19.047382 aa_structures-2.9.1/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2022-06-01 15:59:29.634387 aa_structures-2.9.1/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2023-04-16 22:10:32.185268 aa_structures-2.9.1/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2022-05-30 21:05:57.993637 aa_structures-2.9.1/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.000997 aa_structures-2.9.1/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1637 2023-07-28 01:22:06.051331 aa_structures-2.9.1/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2020-10-22 17:29:44.485193 aa_structures-2.9.1/structures/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.000997 aa_structures-2.9.1/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/tests/core/notification_embeds/__init__.py
+-rw-r--r--   0        0        0     1776 2023-11-10 05:57:15.194459 aa_structures-2.9.1/structures/tests/core/notification_embeds/test_helpers.py
+-rw-r--r--   0        0        0    13808 2024-02-29 22:16:28.663517 aa_structures-2.9.1/structures/tests/core/notification_embeds/test_main.py
+-rw-r--r--   0        0        0    10857 2023-11-30 15:47:14.138045 aa_structures-2.9.1/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     9881 2023-07-28 16:06:53.302038 aa_structures-2.9.1/structures/tests/core/test_notification_types.py
+-rw-r--r--   0        0        0     5583 2023-11-30 15:47:14.138045 aa_structures-2.9.1/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     7056 2023-11-30 15:47:14.138045 aa_structures-2.9.1/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      821 2023-07-28 01:22:06.051331 aa_structures-2.9.1/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3186 2023-11-30 15:47:14.138045 aa_structures-2.9.1/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/tests/integration/__init__.py
+-rw-r--r--   0        0        0    23588 2023-11-30 15:47:14.138045 aa_structures-2.9.1/structures/tests/integration/test_tasks.py
+-rw-r--r--   0        0        0     4331 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/integration/test_views.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1623 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    30300 2024-02-29 22:16:28.667517 aa_structures-2.9.1/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31989 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     7257 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5551 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    22600 2024-03-29 16:15:34.309984 aa_structures-2.9.1/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    21911 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    16947 2023-11-30 15:47:14.142045 aa_structures-2.9.1/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    18831 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/models/test_owners_4.py
+-rw-r--r--   0        0        0    31607 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/models/test_owners_5.py
+-rw-r--r--   0        0        0    41469 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0    24333 2023-11-28 20:06:52.956934 aa_structures-2.9.1/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     4893 2024-03-01 16:31:33.219958 aa_structures-2.9.1/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    34539 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     2942 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/test_managers_2.py
+-rw-r--r--   0        0        0    17269 2023-11-30 15:47:14.146045 aa_structures-2.9.1/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2129 2023-10-06 22:12:34.661204 aa_structures-2.9.1/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    32147 2024-02-29 22:16:28.667517 aa_structures-2.9.1/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2022-08-10 19:36:18.186258 aa_structures-2.9.1/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   993284 2023-10-06 22:12:34.665204 aa_structures-2.9.1/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    24718 2023-11-16 00:12:49.124741 aa_structures-2.9.1/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0     5746 2022-09-10 17:58:40.522747 aa_structures-2.9.1/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1413 2023-11-10 05:57:15.214459 aa_structures-2.9.1/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     9134 2023-11-16 00:12:49.128741 aa_structures-2.9.1/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0     6183 2024-03-21 13:54:34.397674 aa_structures-2.9.1/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2022-08-10 15:32:14.940423 aa_structures-2.9.1/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2021-03-24 18:47:30.630666 aa_structures-2.9.1/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2020-10-22 17:29:44.489193 aa_structures-2.9.1/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/tests/views/__init__.py
+-rw-r--r--   0        0        0     1372 2023-11-30 15:47:14.150045 aa_structures-2.9.1/structures/tests/views/test_public.py
+-rw-r--r--   0        0        0     2626 2023-11-30 15:47:14.150045 aa_structures-2.9.1/structures/tests/views/test_statistics.py
+-rw-r--r--   0        0        0    29004 2023-11-30 15:47:14.150045 aa_structures-2.9.1/structures/tests/views/test_structures.py
+-rw-r--r--   0        0        0      247 2023-11-07 13:45:35.442148 aa_structures-2.9.1/structures/tests/views/utils.py
+-rw-r--r--   0        0        0     1396 2023-11-07 13:45:35.442148 aa_structures-2.9.1/structures/urls.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.004997 aa_structures-2.9.1/structures/views/__init__.py
+-rw-r--r--   0        0        0      818 2023-11-11 19:07:33.648666 aa_structures-2.9.1/structures/views/common.py
+-rw-r--r--   0        0        0     3035 2023-11-11 19:07:33.648666 aa_structures-2.9.1/structures/views/public.py
+-rw-r--r--   0        0        0     4709 2023-11-11 19:07:33.648666 aa_structures-2.9.1/structures/views/statistics.py
+-rw-r--r--   0        0        0    23167 2023-11-11 19:07:33.648666 aa_structures-2.9.1/structures/views/structures.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.008997 aa_structures-2.9.1/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6573 2023-08-01 12:33:06.799354 aa_structures-2.9.1/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1117 2023-07-28 22:31:18.481156 aa_structures-2.9.1/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     2067 2023-11-28 20:06:52.972934 aa_structures-2.9.1/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2024-03-29 17:56:01.008997 aa_structures-2.9.1/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6762 2023-11-28 20:06:52.972934 aa_structures-2.9.1/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2021-02-14 22:48:19.121024 aa_structures-2.9.1/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 aa_structures-2.9.1/PKG-INFO
```

### Comparing `aa_structures-2.9.0/LICENSE` & `aa_structures-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/README.md` & `aa_structures-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/pyproject.toml` & `aa_structures-2.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/admin.py` & `aa_structures-2.9.1/structures/admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/app_settings.py` & `aa_structures-2.9.1/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/auth_hooks.py` & `aa_structures-2.9.1/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/constants.py` & `aa_structures-2.9.1/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/billing_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/billing_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/corporate_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/corporate_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/helpers.py` & `aa_structures-2.9.1/structures/core/notification_embeds/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/main.py` & `aa_structures-2.9.1/structures/core/notification_embeds/main.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/moonmining_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/moonmining_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/orbital_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/orbital_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/sov_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/sov_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/structures_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/structures_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/tower_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/tower_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_embeds/war_embeds.py` & `aa_structures-2.9.1/structures/core/notification_embeds/war_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_timers.py` & `aa_structures-2.9.1/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/notification_types.py` & `aa_structures-2.9.1/structures/core/notification_types.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/serializers.py` & `aa_structures-2.9.1/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/sovereignty.py` & `aa_structures-2.9.1/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/core/starbases.py` & `aa_structures-2.9.1/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/helpers.py` & `aa_structures-2.9.1/structures/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.9.1/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/django.pot` & `aa_structures-2.9.1/structures/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.9.1/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/it_IT/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/ja/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.9.1/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/uk/LC_MESSAGES/django.mo` & `aa_structures-2.9.1/structures/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/uk/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.9.1/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.9.1/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/management/commands/structures_load_eve.py` & `aa_structures-2.9.1/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.9.1/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/management/commands/structures_update_poco_planets.py` & `aa_structures-2.9.1/structures/management/commands/structures_update_poco_planets.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/managers.py` & `aa_structures-2.9.1/structures/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/migrations/0001_initial_new.py` & `aa_structures-2.9.1/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.9.1/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.9.1/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/migrations/0004_improve_localization.py` & `aa_structures-2.9.1/structures/migrations/0004_improve_localization.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/migrations/0005_add_notification_types.py` & `aa_structures-2.9.1/structures/migrations/0005_add_notification_types.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/models/__init__.py` & `aa_structures-2.9.1/structures/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/models/eveuniverse.py` & `aa_structures-2.9.1/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/models/notifications.py` & `aa_structures-2.9.1/structures/models/notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/models/owners.py` & `aa_structures-2.9.1/structures/models/owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,17 @@
         if self.is_alliance_main:
             Owner.objects.filter(
                 corporation__alliance_id=self.corporation.alliance_id
             ).exclude(corporation__alliance_id__isnull=True).update(
                 is_alliance_main=False
             )
             if "update_fields" in kwargs:
-                kwargs["update_fields"].append("is_alliance_main")
+                u = set(kwargs["update_fields"])
+                u.add("is_alliance_main")
+                kwargs["update_fields"] = u
         super().save(*args, **kwargs)
 
     @property
     def is_structure_sync_fresh(self) -> bool:
         """True if last sync happened with grace time, else False."""
         return bool(
             self.structures_last_update_at
```

### Comparing `aa_structures-2.9.0/structures/models/structures_1.py` & `aa_structures-2.9.1/structures/models/structures_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/models/structures_2.py` & `aa_structures-2.9.1/structures/models/structures_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/css/global.css` & `aa_structures-2.9.1/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/css/statistics.css` & `aa_structures-2.9.1/structures/static/structures/css/statistics.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/css/structures.css` & `aa_structures-2.9.1/structures/static/structures/css/structures.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/bars-rotate-fade-black-36.svg` & `aa_structures-2.9.1/structures/static/structures/img/bars-rotate-fade-black-36.svg`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/bars-rotate-fade-white-36.svg` & `aa_structures-2.9.1/structures/static/structures/img/bars-rotate-fade-white-36.svg`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.9.1/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/0h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/0l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/0m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/0r.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/0s.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/1h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/1l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/1m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/1r.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/2h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/2l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/2m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/2r.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/3h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/3l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/3m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/3r.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/4h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/4l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/4m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/4s.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/5h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/5l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/5m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/5s.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/6h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/6l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/6m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/7h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/7l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/7m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/8h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/8l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/8m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/circle.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/h.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/l.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/m.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/noship.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/r.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.9.1/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/js/global.js` & `aa_structures-2.9.1/structures/static/structures/js/global.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/js/public.js` & `aa_structures-2.9.1/structures/static/structures/js/public.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/js/statistics.js` & `aa_structures-2.9.1/structures/static/structures/js/statistics.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/js/structures.js` & `aa_structures-2.9.1/structures/static/structures/js/structures.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/datetime.js` & `aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/static/structures/vendor/datatables/plugins/filterDropDown.min.js` & `aa_structures-2.9.1/structures/static/structures/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tasks.py` & `aa_structures-2.9.1/structures/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.9.1/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.9.1/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.9.1/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.9.1/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.9.1/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/modals/tab_services_detail.html` & `aa_structures-2.9.1/structures/templates/structures/modals/tab_services_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/menu.html` & `aa_structures-2.9.1/structures/templates/structures/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/public/poco_list.html` & `aa_structures-2.9.1/structures/templates/structures/partials/public/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/statistics/structure_summary.html` & `aa_structures-2.9.1/structures/templates/structures/partials/statistics/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/structures/jump_gates_list.html` & `aa_structures-2.9.1/structures/templates/structures/partials/structures/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/structures/poco_list.html` & `aa_structures-2.9.1/structures/templates/structures/partials/structures/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/structures/starbase_list.html` & `aa_structures-2.9.1/structures/templates/structures/partials/structures/starbase_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/partials/structures/structure_list.html` & `aa_structures-2.9.1/structures/templates/structures/partials/structures/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/public.html` & `aa_structures-2.9.1/structures/templates/structures/public.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/statistics.html` & `aa_structures-2.9.1/structures/templates/structures/statistics.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/structures.html` & `aa_structures-2.9.1/structures/templates/structures/structures.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.9.1/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/templatetags/structures.py` & `aa_structures-2.9.1/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/notification_embeds/test_helpers.py` & `aa_structures-2.9.1/structures/tests/core/notification_embeds/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/notification_embeds/test_main.py` & `aa_structures-2.9.1/structures/tests/core/notification_embeds/test_main.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.9.1/structures/tests/core/test_notification_structuretimers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_notification_types.py` & `aa_structures-2.9.1/structures/tests/core/test_notification_types.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.9.1/structures/tests/core/test_notifications_timerboard.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_serializers.py` & `aa_structures-2.9.1/structures/tests/core/test_serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_sovereignty.py` & `aa_structures-2.9.1/structures/tests/core/test_sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/core/test_starbases.py` & `aa_structures-2.9.1/structures/tests/core/test_starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/integration/test_tasks.py` & `aa_structures-2.9.1/structures/tests/integration/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/integration/test_views.py` & `aa_structures-2.9.1/structures/tests/integration/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.9.1/structures/tests/models/test_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_notifications_1.py` & `aa_structures-2.9.1/structures/tests/models/test_notifications_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_notifications_2.py` & `aa_structures-2.9.1/structures/tests/models/test_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_notifications_3.py` & `aa_structures-2.9.1/structures/tests/models/test_notifications_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.9.1/structures/tests/models/test_notifications_discord.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_owners_1.py` & `aa_structures-2.9.1/structures/tests/models/test_owners_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,34 @@
         owner.save()
         # then
         owner.refresh_from_db()
         self.assertTrue(owner.is_alliance_main)
         self.owner.refresh_from_db()
         self.assertFalse(self.owner.is_alliance_main)
 
+    def test_should_ensure_is_alliance_main_is_set_for_update_fields_1(self):
+        # given
+        corporation = EveCorporationInfoFactory(alliance=self.alliance)
+        owner = OwnerFactory(corporation=corporation, is_alliance_main=True)
+        # when
+        owner.save(update_fields={"is_active"})
+        # then
+        owner.refresh_from_db()
+        self.assertTrue(owner.is_alliance_main)
+
+    def test_should_ensure_is_alliance_main_is_set_for_update_fields_2(self):
+        # given
+        corporation = EveCorporationInfoFactory(alliance=self.alliance)
+        owner = OwnerFactory(corporation=corporation, is_alliance_main=True)
+        # when
+        owner.save(update_fields=["is_active"])
+        # then
+        owner.refresh_from_db()
+        self.assertTrue(owner.is_alliance_main)
+
     def test_should_allow_mains_from_other_alliances(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
         owner = OwnerFactory()
         # when
         owner.is_alliance_main = True
```

### Comparing `aa_structures-2.9.0/structures/tests/models/test_owners_2.py` & `aa_structures-2.9.1/structures/tests/models/test_owners_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_owners_3.py` & `aa_structures-2.9.1/structures/tests/models/test_owners_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_owners_4.py` & `aa_structures-2.9.1/structures/tests/models/test_owners_4.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_owners_5.py` & `aa_structures-2.9.1/structures/tests/models/test_owners_5.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/models/test_structures.py` & `aa_structures-2.9.1/structures/tests/models/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/test_admin.py` & `aa_structures-2.9.1/structures/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/test_helpers.py` & `aa_structures-2.9.1/structures/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/test_managers_1.py` & `aa_structures-2.9.1/structures/tests/test_managers_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/test_managers_2.py` & `aa_structures-2.9.1/structures/tests/test_managers_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/test_tasks.py` & `aa_structures-2.9.1/structures/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.9.1/structures/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/entities.json` & `aa_structures-2.9.1/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/esi_data.json` & `aa_structures-2.9.1/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.9.1/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/factories.py` & `aa_structures-2.9.1/structures/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.9.1/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.9.1/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/generate_structures.py` & `aa_structures-2.9.1/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/helpers.py` & `aa_structures-2.9.1/structures/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.9.1/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/views/test_public.py` & `aa_structures-2.9.1/structures/tests/views/test_public.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/views/test_statistics.py` & `aa_structures-2.9.1/structures/tests/views/test_statistics.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/tests/views/test_structures.py` & `aa_structures-2.9.1/structures/tests/views/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/urls.py` & `aa_structures-2.9.1/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/views/common.py` & `aa_structures-2.9.1/structures/views/common.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/views/public.py` & `aa_structures-2.9.1/structures/views/public.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/views/statistics.py` & `aa_structures-2.9.1/structures/views/statistics.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/views/structures.py` & `aa_structures-2.9.1/structures/views/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/webhooks/core.py` & `aa_structures-2.9.1/structures/webhooks/core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/webhooks/managers.py` & `aa_structures-2.9.1/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/webhooks/models.py` & `aa_structures-2.9.1/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/structures/webhooks/tests/test_core.py` & `aa_structures-2.9.1/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.9.0/PKG-INFO` & `aa_structures-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.9.0
+Version: 2.9.1
 Summary: App for managing Eve Online structures with Alliance Auth.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

