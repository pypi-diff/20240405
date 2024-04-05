# Comparing `tmp/energy_base-1.6.5.tar.gz` & `tmp/energy_base-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energy_base-1.6.5.tar", max compression
+gzip compressed data, was "energy_base-1.6.6.tar", max compression
```

## Comparing `energy_base-1.6.5.tar` & `energy_base-1.6.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       19 2024-01-19 05:01:21.446226 energy_base-1.6.5/README.md
--rw-r--r--   0        0        0      658 2024-04-05 11:22:44.052504 energy_base-1.6.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-18 13:04:36.214467 energy_base-1.6.5/src/energy_base/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 13:00:16.243328 energy_base-1.6.5/src/energy_base/api/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-05 06:38:25.870944 energy_base-1.6.5/src/energy_base/api/base.py
--rw-r--r--   0        0        0      853 2024-04-05 06:38:25.871491 energy_base-1.6.5/src/energy_base/api/pagination.py
--rw-r--r--   0        0        0       62 2024-04-05 06:38:25.871627 energy_base-1.6.5/src/energy_base/api/permissions/__init__.py
--rw-r--r--   0        0        0      323 2024-03-20 12:37:42.669800 energy_base-1.6.5/src/energy_base/api/permissions/superuser.py
--rw-r--r--   0        0        0      178 2024-01-18 13:05:51.729378 energy_base-1.6.5/src/energy_base/api/routers.py
--rw-r--r--   0        0        0      466 2024-04-05 06:38:25.871699 energy_base-1.6.5/src/energy_base/api/views.py
--rw-r--r--   0        0        0      239 2024-02-01 10:01:47.652585 energy_base-1.6.5/src/energy_base/authentications/__init__.py
--rw-r--r--   0        0        0     1002 2024-02-01 10:01:47.647816 energy_base-1.6.5/src/energy_base/authentications/microservice_authentication.py
--rw-r--r--   0        0        0     2496 2024-02-01 07:47:27.882905 energy_base-1.6.5/src/energy_base/authentications/models.py
--rw-r--r--   0        0        0        0 2024-04-03 10:05:27.551510 energy_base-1.6.5/src/energy_base/external_api/__init__.py
--rw-r--r--   0        0        0       80 2024-04-05 06:45:09.287330 energy_base-1.6.5/src/energy_base/external_api/serializers/__init__.py
--rw-r--r--   0        0        0      403 2024-04-05 06:45:09.282687 energy_base-1.6.5/src/energy_base/external_api/serializers/api_status.py
--rw-r--r--   0        0        0       72 2024-04-05 06:45:09.280547 energy_base-1.6.5/src/energy_base/external_api/views/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-05 06:45:09.284881 energy_base-1.6.5/src/energy_base/external_api/views/api_status.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.871770 energy_base-1.6.5/src/energy_base/file_upload/__init__.py
--rw-r--r--   0        0        0       63 2024-04-05 06:38:25.872022 energy_base-1.6.5/src/energy_base/file_upload/admin.py
--rw-r--r--   0        0        0      165 2024-04-05 06:38:25.872083 energy_base-1.6.5/src/energy_base/file_upload/apps.py
--rw-r--r--   0        0        0      153 2024-04-05 06:38:25.872179 energy_base-1.6.5/src/energy_base/file_upload/data_processors/__init__.py
--rw-r--r--   0        0        0     1529 2024-04-05 06:38:25.872248 energy_base-1.6.5/src/energy_base/file_upload/data_processors/base_sheet_processor.py
--rw-r--r--   0        0        0      762 2024-04-05 06:38:25.872314 energy_base-1.6.5/src/energy_base/file_upload/data_processors/xls_processor.py
--rw-r--r--   0        0        0       67 2024-04-05 06:38:25.872417 energy_base-1.6.5/src/energy_base/file_upload/filters/__init__.py
--rw-r--r--   0        0        0      326 2024-04-05 06:38:25.872478 energy_base-1.6.5/src/energy_base/file_upload/filters/file.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872541 energy_base-1.6.5/src/energy_base/file_upload/migrations/__init__.py
--rw-r--r--   0        0        0      131 2024-04-05 06:38:25.872667 energy_base-1.6.5/src/energy_base/file_upload/models/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-05 06:38:25.872729 energy_base-1.6.5/src/energy_base/file_upload/models/import_file.py
--rw-r--r--   0        0        0      726 2024-04-05 06:38:25.872792 energy_base-1.6.5/src/energy_base/file_upload/models/temporary_data.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872856 energy_base-1.6.5/src/energy_base/file_upload/serializers/__init__.py
--rw-r--r--   0        0        0      710 2024-04-05 06:38:25.872951 energy_base-1.6.5/src/energy_base/file_upload/serializers/file.py
--rw-r--r--   0        0        0       69 2024-04-05 06:38:25.873054 energy_base-1.6.5/src/energy_base/file_upload/services/__init__.py
--rw-r--r--   0        0        0      248 2024-04-05 06:38:25.873114 energy_base-1.6.5/src/energy_base/file_upload/services/minio.py
--rw-r--r--   0        0        0      542 2024-04-05 06:38:25.873191 energy_base-1.6.5/src/energy_base/file_upload/urls.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873294 energy_base-1.6.5/src/energy_base/file_upload/views/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-05 06:38:25.873438 energy_base-1.6.5/src/energy_base/file_upload/views/file.py
--rw-r--r--   0        0        0       77 2024-01-23 06:30:45.082611 energy_base-1.6.5/src/energy_base/models/__init__.py
--rw-r--r--   0        0        0      298 2024-03-28 12:32:03.966843 energy_base-1.6.5/src/energy_base/models/jwt_user.py
--rw-r--r--   0        0        0        0 2024-03-20 10:58:18.698302 energy_base-1.6.5/src/energy_base/q_api/__init__.py
--rw-r--r--   0        0        0      153 2024-03-27 13:08:53.141117 energy_base-1.6.5/src/energy_base/q_api/apps.py
--rw-r--r--   0        0        0       92 2024-03-27 13:05:43.703022 energy_base-1.6.5/src/energy_base/q_api/filters/__init__.py
--rw-r--r--   0        0        0      133 2024-03-20 12:32:09.410169 energy_base-1.6.5/src/energy_base/q_api/filters/task.py
--rw-r--r--   0        0        0      194 2024-03-27 13:08:53.144544 energy_base-1.6.5/src/energy_base/q_api/serializers/__init__.py
--rw-r--r--   0        0        0      383 2024-03-27 13:08:53.146756 energy_base-1.6.5/src/energy_base/q_api/serializers/schedule.py
--rw-r--r--   0        0        0      596 2024-03-29 04:25:10.738382 energy_base-1.6.5/src/energy_base/q_api/serializers/task.py
--rw-r--r--   0        0        0      468 2024-03-28 06:56:59.203700 energy_base-1.6.5/src/energy_base/q_api/urls.py
--rw-r--r--   0        0        0      216 2024-03-28 06:56:59.208785 energy_base-1.6.5/src/energy_base/q_api/views/__init__.py
--rw-r--r--   0        0        0      838 2024-03-29 04:13:01.770648 energy_base-1.6.5/src/energy_base/q_api/views/schedule.py
--rw-r--r--   0        0        0      516 2024-03-29 04:13:01.763075 energy_base-1.6.5/src/energy_base/q_api/views/task.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873512 energy_base-1.6.5/src/energy_base/references_api/__init__.py
--rw-r--r--   0        0        0       63 2024-04-05 06:38:25.873608 energy_base-1.6.5/src/energy_base/references_api/admin.py
--rw-r--r--   0        0        0      171 2024-04-05 06:38:25.873676 energy_base-1.6.5/src/energy_base/references_api/apps.py
--rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873746 energy_base-1.6.5/src/energy_base/references_api/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-04-05 06:38:25.873832 energy_base-1.6.5/src/energy_base/references_api/models.py
--rw-r--r--   0        0        0       60 2024-04-05 06:38:25.873892 energy_base-1.6.5/src/energy_base/references_api/tests.py
--rw-r--r--   0        0        0      390 2024-04-05 06:38:25.873959 energy_base-1.6.5/src/energy_base/references_api/urls.py
--rw-r--r--   0        0        0     3575 2024-04-05 06:38:25.874023 energy_base-1.6.5/src/energy_base/references_api/utils.py
--rw-r--r--   0        0        0      174 2024-04-05 11:22:44.049722 energy_base-1.6.5/src/energy_base/services/__init__.py
--rw-r--r--   0        0        0     4266 2024-04-05 10:56:22.978028 energy_base-1.6.5/src/energy_base/services/base_api.py
--rw-r--r--   0        0        0     1468 2024-03-05 05:53:43.397963 energy_base-1.6.5/src/energy_base/services/minio.py
--rw-r--r--   0        0        0      757 2024-04-05 06:45:09.277605 energy_base-1.6.5/src/energy_base/services/telnet.py
--rw-r--r--   0        0        0      503 2024-04-05 06:38:25.874994 energy_base-1.6.5/src/energy_base/services/user.py
--rw-r--r--   0        0        0      194 2024-03-05 06:28:37.626781 energy_base-1.6.5/src/energy_base/translation/__init__.py
--rw-r--r--   0        0        0      344 2024-03-05 06:49:11.397042 energy_base-1.6.5/src/energy_base/translation/utils.py
--rw-r--r--   0        0        0      167 2024-03-19 09:20:40.790206 energy_base-1.6.5/src/energy_base/utils/__init__.py
--rw-r--r--   0        0        0     1356 2024-03-19 09:20:40.790318 energy_base-1.6.5/src/energy_base/utils/data.py
--rw-r--r--   0        0        0     1535 2024-03-20 07:33:11.117325 energy_base-1.6.5/src/energy_base/utils/date.py
--rw-r--r--   0        0        0      758 2024-02-29 10:58:24.635825 energy_base-1.6.5/src/energy_base/utils/dict_util.py
--rw-r--r--   0        0        0      605 2024-04-05 09:29:58.495591 energy_base-1.6.5/src/energy_base/utils/response_processors.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 energy_base-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-01-19 05:01:21.446226 energy_base-1.6.6/README.md
+-rw-r--r--   0        0        0      658 2024-04-05 12:36:20.659227 energy_base-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-18 13:04:36.214467 energy_base-1.6.6/src/energy_base/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:00:16.243328 energy_base-1.6.6/src/energy_base/api/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-05 06:38:25.870944 energy_base-1.6.6/src/energy_base/api/base.py
+-rw-r--r--   0        0        0      853 2024-04-05 06:38:25.871491 energy_base-1.6.6/src/energy_base/api/pagination.py
+-rw-r--r--   0        0        0       62 2024-04-05 06:38:25.871627 energy_base-1.6.6/src/energy_base/api/permissions/__init__.py
+-rw-r--r--   0        0        0      323 2024-03-20 12:37:42.669800 energy_base-1.6.6/src/energy_base/api/permissions/superuser.py
+-rw-r--r--   0        0        0      178 2024-01-18 13:05:51.729378 energy_base-1.6.6/src/energy_base/api/routers.py
+-rw-r--r--   0        0        0      466 2024-04-05 06:38:25.871699 energy_base-1.6.6/src/energy_base/api/views.py
+-rw-r--r--   0        0        0      239 2024-02-01 10:01:47.652585 energy_base-1.6.6/src/energy_base/authentications/__init__.py
+-rw-r--r--   0        0        0     1002 2024-02-01 10:01:47.647816 energy_base-1.6.6/src/energy_base/authentications/microservice_authentication.py
+-rw-r--r--   0        0        0     2496 2024-02-01 07:47:27.882905 energy_base-1.6.6/src/energy_base/authentications/models.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:05:27.551510 energy_base-1.6.6/src/energy_base/external_api/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 06:45:09.287330 energy_base-1.6.6/src/energy_base/external_api/serializers/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-05 06:45:09.282687 energy_base-1.6.6/src/energy_base/external_api/serializers/api_status.py
+-rw-r--r--   0        0        0       72 2024-04-05 06:45:09.280547 energy_base-1.6.6/src/energy_base/external_api/views/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-05 06:45:09.284881 energy_base-1.6.6/src/energy_base/external_api/views/api_status.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.871770 energy_base-1.6.6/src/energy_base/file_upload/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-05 06:38:25.872022 energy_base-1.6.6/src/energy_base/file_upload/admin.py
+-rw-r--r--   0        0        0      165 2024-04-05 06:38:25.872083 energy_base-1.6.6/src/energy_base/file_upload/apps.py
+-rw-r--r--   0        0        0      153 2024-04-05 06:38:25.872179 energy_base-1.6.6/src/energy_base/file_upload/data_processors/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-05 06:38:25.872248 energy_base-1.6.6/src/energy_base/file_upload/data_processors/base_sheet_processor.py
+-rw-r--r--   0        0        0      762 2024-04-05 06:38:25.872314 energy_base-1.6.6/src/energy_base/file_upload/data_processors/xls_processor.py
+-rw-r--r--   0        0        0       67 2024-04-05 06:38:25.872417 energy_base-1.6.6/src/energy_base/file_upload/filters/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-05 06:38:25.872478 energy_base-1.6.6/src/energy_base/file_upload/filters/file.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872541 energy_base-1.6.6/src/energy_base/file_upload/migrations/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-05 06:38:25.872667 energy_base-1.6.6/src/energy_base/file_upload/models/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-05 06:38:25.872729 energy_base-1.6.6/src/energy_base/file_upload/models/import_file.py
+-rw-r--r--   0        0        0      726 2024-04-05 06:38:25.872792 energy_base-1.6.6/src/energy_base/file_upload/models/temporary_data.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872856 energy_base-1.6.6/src/energy_base/file_upload/serializers/__init__.py
+-rw-r--r--   0        0        0      710 2024-04-05 06:38:25.872951 energy_base-1.6.6/src/energy_base/file_upload/serializers/file.py
+-rw-r--r--   0        0        0       69 2024-04-05 06:38:25.873054 energy_base-1.6.6/src/energy_base/file_upload/services/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-05 06:38:25.873114 energy_base-1.6.6/src/energy_base/file_upload/services/minio.py
+-rw-r--r--   0        0        0      542 2024-04-05 06:38:25.873191 energy_base-1.6.6/src/energy_base/file_upload/urls.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873294 energy_base-1.6.6/src/energy_base/file_upload/views/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-05 06:38:25.873438 energy_base-1.6.6/src/energy_base/file_upload/views/file.py
+-rw-r--r--   0        0        0       77 2024-01-23 06:30:45.082611 energy_base-1.6.6/src/energy_base/models/__init__.py
+-rw-r--r--   0        0        0      298 2024-03-28 12:32:03.966843 energy_base-1.6.6/src/energy_base/models/jwt_user.py
+-rw-r--r--   0        0        0        0 2024-03-20 10:58:18.698302 energy_base-1.6.6/src/energy_base/q_api/__init__.py
+-rw-r--r--   0        0        0      153 2024-03-27 13:08:53.141117 energy_base-1.6.6/src/energy_base/q_api/apps.py
+-rw-r--r--   0        0        0       92 2024-03-27 13:05:43.703022 energy_base-1.6.6/src/energy_base/q_api/filters/__init__.py
+-rw-r--r--   0        0        0      133 2024-03-20 12:32:09.410169 energy_base-1.6.6/src/energy_base/q_api/filters/task.py
+-rw-r--r--   0        0        0      194 2024-03-27 13:08:53.144544 energy_base-1.6.6/src/energy_base/q_api/serializers/__init__.py
+-rw-r--r--   0        0        0      383 2024-03-27 13:08:53.146756 energy_base-1.6.6/src/energy_base/q_api/serializers/schedule.py
+-rw-r--r--   0        0        0      596 2024-03-29 04:25:10.738382 energy_base-1.6.6/src/energy_base/q_api/serializers/task.py
+-rw-r--r--   0        0        0      468 2024-03-28 06:56:59.203700 energy_base-1.6.6/src/energy_base/q_api/urls.py
+-rw-r--r--   0        0        0      216 2024-03-28 06:56:59.208785 energy_base-1.6.6/src/energy_base/q_api/views/__init__.py
+-rw-r--r--   0        0        0      838 2024-03-29 04:13:01.770648 energy_base-1.6.6/src/energy_base/q_api/views/schedule.py
+-rw-r--r--   0        0        0      516 2024-03-29 04:13:01.763075 energy_base-1.6.6/src/energy_base/q_api/views/task.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873512 energy_base-1.6.6/src/energy_base/references_api/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-05 06:38:25.873608 energy_base-1.6.6/src/energy_base/references_api/admin.py
+-rw-r--r--   0        0        0      171 2024-04-05 06:38:25.873676 energy_base-1.6.6/src/energy_base/references_api/apps.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873746 energy_base-1.6.6/src/energy_base/references_api/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-05 06:38:25.873832 energy_base-1.6.6/src/energy_base/references_api/models.py
+-rw-r--r--   0        0        0       60 2024-04-05 06:38:25.873892 energy_base-1.6.6/src/energy_base/references_api/tests.py
+-rw-r--r--   0        0        0      390 2024-04-05 06:38:25.873959 energy_base-1.6.6/src/energy_base/references_api/urls.py
+-rw-r--r--   0        0        0     3575 2024-04-05 06:38:25.874023 energy_base-1.6.6/src/energy_base/references_api/utils.py
+-rw-r--r--   0        0        0      174 2024-04-05 11:22:44.049722 energy_base-1.6.6/src/energy_base/services/__init__.py
+-rw-r--r--   0        0        0     4291 2024-04-05 12:36:03.275954 energy_base-1.6.6/src/energy_base/services/base_api.py
+-rw-r--r--   0        0        0     1468 2024-03-05 05:53:43.397963 energy_base-1.6.6/src/energy_base/services/minio.py
+-rw-r--r--   0        0        0      757 2024-04-05 06:45:09.277605 energy_base-1.6.6/src/energy_base/services/telnet.py
+-rw-r--r--   0        0        0      503 2024-04-05 06:38:25.874994 energy_base-1.6.6/src/energy_base/services/user.py
+-rw-r--r--   0        0        0      194 2024-03-05 06:28:37.626781 energy_base-1.6.6/src/energy_base/translation/__init__.py
+-rw-r--r--   0        0        0      344 2024-03-05 06:49:11.397042 energy_base-1.6.6/src/energy_base/translation/utils.py
+-rw-r--r--   0        0        0      167 2024-03-19 09:20:40.790206 energy_base-1.6.6/src/energy_base/utils/__init__.py
+-rw-r--r--   0        0        0     1356 2024-03-19 09:20:40.790318 energy_base-1.6.6/src/energy_base/utils/data.py
+-rw-r--r--   0        0        0     1535 2024-03-20 07:33:11.117325 energy_base-1.6.6/src/energy_base/utils/date.py
+-rw-r--r--   0        0        0      758 2024-02-29 10:58:24.635825 energy_base-1.6.6/src/energy_base/utils/dict_util.py
+-rw-r--r--   0        0        0      605 2024-04-05 09:29:58.495591 energy_base-1.6.6/src/energy_base/utils/response_processors.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 energy_base-1.6.6/PKG-INFO
```

### Comparing `energy_base-1.6.5/pyproject.toml` & `energy_base-1.6.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "energy-base"
-version = "1.6.5"
+version = "1.6.6"
 description = "Energy Base Package"
 authors = ["Olimboy <shavkatov.olimboy@mail.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 djangorestframework = "^3.14.0"
```

### Comparing `energy_base-1.6.5/src/energy_base/api/base.py` & `energy_base-1.6.6/src/energy_base/api/base.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/api/pagination.py` & `energy_base-1.6.6/src/energy_base/api/pagination.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/authentications/microservice_authentication.py` & `energy_base-1.6.6/src/energy_base/authentications/microservice_authentication.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/authentications/models.py` & `energy_base-1.6.6/src/energy_base/authentications/models.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/external_api/views/api_status.py` & `energy_base-1.6.6/src/energy_base/external_api/views/api_status.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/data_processors/base_sheet_processor.py` & `energy_base-1.6.6/src/energy_base/file_upload/data_processors/base_sheet_processor.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/data_processors/xls_processor.py` & `energy_base-1.6.6/src/energy_base/file_upload/data_processors/xls_processor.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/models/import_file.py` & `energy_base-1.6.6/src/energy_base/file_upload/models/import_file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/models/temporary_data.py` & `energy_base-1.6.6/src/energy_base/file_upload/models/temporary_data.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/serializers/file.py` & `energy_base-1.6.6/src/energy_base/file_upload/serializers/file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/urls.py` & `energy_base-1.6.6/src/energy_base/file_upload/urls.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/file_upload/views/file.py` & `energy_base-1.6.6/src/energy_base/file_upload/views/file.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/q_api/serializers/task.py` & `energy_base-1.6.6/src/energy_base/q_api/serializers/task.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/q_api/views/schedule.py` & `energy_base-1.6.6/src/energy_base/q_api/views/schedule.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/q_api/views/task.py` & `energy_base-1.6.6/src/energy_base/q_api/views/task.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/references_api/utils.py` & `energy_base-1.6.6/src/energy_base/references_api/utils.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/services/base_api.py` & `energy_base-1.6.6/src/energy_base/services/base_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         response = requests.request(
             method=method,
             url=self.base_url + path,
             data=data,
             json=json,
             params=params,
             headers=headers,
+            verify=False
         )
 
         if response_processor == 'default':
             if self.__class__.default_response_processor is not None:
                 return self.__class__.default_response_processor(response)
             return response
```

### Comparing `energy_base-1.6.5/src/energy_base/services/minio.py` & `energy_base-1.6.6/src/energy_base/services/minio.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/services/telnet.py` & `energy_base-1.6.6/src/energy_base/services/telnet.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/utils/data.py` & `energy_base-1.6.6/src/energy_base/utils/data.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/utils/date.py` & `energy_base-1.6.6/src/energy_base/utils/date.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/utils/dict_util.py` & `energy_base-1.6.6/src/energy_base/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/src/energy_base/utils/response_processors.py` & `energy_base-1.6.6/src/energy_base/utils/response_processors.py`

 * *Files identical despite different names*

### Comparing `energy_base-1.6.5/PKG-INFO` & `energy_base-1.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energy-base
-Version: 1.6.5
+Version: 1.6.6
 Summary: Energy Base Package
 Author: Olimboy
 Author-email: shavkatov.olimboy@mail.ru
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
```

