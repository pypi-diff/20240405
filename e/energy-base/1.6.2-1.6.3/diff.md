# Comparing `tmp/energy_base-1.6.2.tar.gz` & `tmp/energy_base-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energy_base-1.6.2.tar", max compression
+gzip compressed data, was "energy_base-1.6.3.tar", max compression
```

## Comparing `energy_base-1.6.2.tar` & `energy_base-1.6.3.tar`

### file list

```diff
@@ -1,63 +1,69 @@
--rw-r--r--   0        0        0      685 2024-04-01 07:49:29.649035 energy_base-1.6.2/pyproject.toml
--rw-r--r--   0        0        0       19 2024-03-11 05:37:22.917248 energy_base-1.6.2/README.md
--rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/api/__init__.py
--rw-r--r--   0        0        0     2423 2024-04-01 07:42:22.627511 energy_base-1.6.2/src/energy_base/api/base.py
--rw-r--r--   0        0        0      886 2024-03-29 08:55:52.301726 energy_base-1.6.2/src/energy_base/api/pagination.py
--rw-r--r--   0        0        0       65 2024-04-01 07:42:22.611897 energy_base-1.6.2/src/energy_base/api/permissions/__init__.py
--rw-r--r--   0        0        0      334 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/api/permissions/superuser.py
--rw-r--r--   0        0        0      186 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/api/routers.py
--rw-r--r--   0        0        0      483 2024-03-29 08:59:36.574149 energy_base-1.6.2/src/energy_base/api/views.py
--rw-r--r--   0        0        0      245 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/authentications/__init__.py
--rw-r--r--   0        0        0     1031 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/authentications/microservice_authentication.py
--rw-r--r--   0        0        0     2588 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/authentications/models.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.508892 energy_base-1.6.2/src/energy_base/file_upload/__init__.py
--rw-r--r--   0        0        0       66 2024-03-29 10:44:11.508892 energy_base-1.6.2/src/energy_base/file_upload/admin.py
--rw-r--r--   0        0        0      171 2024-03-29 10:58:14.727096 energy_base-1.6.2/src/energy_base/file_upload/apps.py
--rw-r--r--   0        0        0      160 2024-03-29 10:57:55.998201 energy_base-1.6.2/src/energy_base/file_upload/data_processors/__init__.py
--rw-r--r--   0        0        0     1569 2024-03-29 10:48:14.069159 energy_base-1.6.2/src/energy_base/file_upload/data_processors/base_sheet_processor.py
--rw-r--r--   0        0        0      789 2024-03-29 10:44:11.509889 energy_base-1.6.2/src/energy_base/file_upload/data_processors/xls_processor.py
--rw-r--r--   0        0        0       72 2024-03-29 10:57:55.994201 energy_base-1.6.2/src/energy_base/file_upload/filters/__init__.py
--rw-r--r--   0        0        0      338 2024-03-29 10:48:14.051821 energy_base-1.6.2/src/energy_base/file_upload/filters/file.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.509889 energy_base-1.6.2/src/energy_base/file_upload/migrations/__init__.py
--rw-r--r--   0        0        0      138 2024-03-29 10:57:56.002202 energy_base-1.6.2/src/energy_base/file_upload/models/__init__.py
--rw-r--r--   0        0        0     1125 2024-03-29 10:48:14.058943 energy_base-1.6.2/src/energy_base/file_upload/models/import_file.py
--rw-r--r--   0        0        0      748 2024-03-29 10:48:14.063725 energy_base-1.6.2/src/energy_base/file_upload/models/temporary_data.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.509889 energy_base-1.6.2/src/energy_base/file_upload/serializers/__init__.py
--rw-r--r--   0        0        0      737 2024-03-29 10:48:14.046819 energy_base-1.6.2/src/energy_base/file_upload/serializers/file.py
--rw-r--r--   0        0        0       74 2024-03-29 10:51:10.661193 energy_base-1.6.2/src/energy_base/file_upload/services/__init__.py
--rw-r--r--   0        0        0      258 2024-03-29 10:51:10.676832 energy_base-1.6.2/src/energy_base/file_upload/services/minio.py
--rw-r--r--   0        0        0      557 2024-03-29 10:59:23.890704 energy_base-1.6.2/src/energy_base/file_upload/urls.py
--rw-r--r--   0        0        0        0 2024-03-29 10:44:11.509889 energy_base-1.6.2/src/energy_base/file_upload/views/__init__.py
--rw-r--r--   0        0        0     5820 2024-03-29 10:53:38.129538 energy_base-1.6.2/src/energy_base/file_upload/views/file.py
--rw-r--r--   0        0        0       82 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/models/__init__.py
--rw-r--r--   0        0        0      308 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/models/jwt_user.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/__init__.py
--rw-r--r--   0        0        0      159 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/apps.py
--rw-r--r--   0        0        0       97 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/filters/__init__.py
--rw-r--r--   0        0        0      138 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/filters/task.py
--rw-r--r--   0        0        0      201 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/serializers/__init__.py
--rw-r--r--   0        0        0      396 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/serializers/schedule.py
--rw-r--r--   0        0        0      617 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/serializers/task.py
--rw-r--r--   0        0        0      483 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/urls.py
--rw-r--r--   0        0        0      224 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/views/__init__.py
--rw-r--r--   0        0        0      863 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/views/schedule.py
--rw-r--r--   0        0        0      532 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/q_api/views/task.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:16.931816 energy_base-1.6.2/src/energy_base/references_api/__init__.py
--rw-r--r--   0        0        0       66 2024-03-29 05:31:16.911760 energy_base-1.6.2/src/energy_base/references_api/admin.py
--rw-r--r--   0        0        0      177 2024-03-29 08:47:27.971536 energy_base-1.6.2/src/energy_base/references_api/apps.py
--rw-r--r--   0        0        0        0 2024-03-29 05:31:16.932321 energy_base-1.6.2/src/energy_base/references_api/migrations/__init__.py
--rw-r--r--   0        0        0       60 2024-03-29 05:31:16.918805 energy_base-1.6.2/src/energy_base/references_api/models.py
--rw-r--r--   0        0        0       63 2024-03-29 05:31:16.926923 energy_base-1.6.2/src/energy_base/references_api/tests.py
--rw-r--r--   0        0        0      403 2024-03-29 08:29:14.326841 energy_base-1.6.2/src/energy_base/references_api/urls.py
--rw-r--r--   0        0        0     3690 2024-04-01 07:42:22.643147 energy_base-1.6.2/src/energy_base/references_api/utils.py
--rw-r--r--   0        0        0      122 2024-03-29 10:53:38.129538 energy_base-1.6.2/src/energy_base/services/__init__.py
--rw-r--r--   0        0        0     1508 2024-03-11 05:37:22.917248 energy_base-1.6.2/src/energy_base/services/minio.py
--rw-r--r--   0        0        0      527 2024-03-29 10:53:38.129538 energy_base-1.6.2/src/energy_base/services/user.py
--rw-r--r--   0        0        0      208 2024-03-11 05:37:22.932870 energy_base-1.6.2/src/energy_base/translation/__init__.py
--rw-r--r--   0        0        0      358 2024-03-11 05:37:22.932870 energy_base-1.6.2/src/energy_base/translation/utils.py
--rw-r--r--   0        0        0      176 2024-03-11 06:08:58.881930 energy_base-1.6.2/src/energy_base/utils/__init__.py
--rw-r--r--   0        0        0     1402 2024-03-11 10:56:13.497068 energy_base-1.6.2/src/energy_base/utils/data.py
--rw-r--r--   0        0        0     1589 2024-03-29 05:31:12.838377 energy_base-1.6.2/src/energy_base/utils/date.py
--rw-r--r--   0        0        0      778 2024-03-11 05:37:22.932870 energy_base-1.6.2/src/energy_base/utils/dict_util.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 energy_base-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-01-19 05:01:21.446226 energy_base-1.6.3/README.md
+-rw-r--r--   0        0        0      658 2024-04-05 06:45:28.706261 energy_base-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-18 13:04:36.214467 energy_base-1.6.3/src/energy_base/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:00:16.243328 energy_base-1.6.3/src/energy_base/api/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-05 06:38:25.870944 energy_base-1.6.3/src/energy_base/api/base.py
+-rw-r--r--   0        0        0      853 2024-04-05 06:38:25.871491 energy_base-1.6.3/src/energy_base/api/pagination.py
+-rw-r--r--   0        0        0       62 2024-04-05 06:38:25.871627 energy_base-1.6.3/src/energy_base/api/permissions/__init__.py
+-rw-r--r--   0        0        0      323 2024-03-20 12:37:42.669800 energy_base-1.6.3/src/energy_base/api/permissions/superuser.py
+-rw-r--r--   0        0        0      178 2024-01-18 13:05:51.729378 energy_base-1.6.3/src/energy_base/api/routers.py
+-rw-r--r--   0        0        0      466 2024-04-05 06:38:25.871699 energy_base-1.6.3/src/energy_base/api/views.py
+-rw-r--r--   0        0        0      239 2024-02-01 10:01:47.652585 energy_base-1.6.3/src/energy_base/authentications/__init__.py
+-rw-r--r--   0        0        0     1002 2024-02-01 10:01:47.647816 energy_base-1.6.3/src/energy_base/authentications/microservice_authentication.py
+-rw-r--r--   0        0        0     2496 2024-02-01 07:47:27.882905 energy_base-1.6.3/src/energy_base/authentications/models.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:05:27.551510 energy_base-1.6.3/src/energy_base/external_api/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-05 06:45:09.287330 energy_base-1.6.3/src/energy_base/external_api/serializers/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-05 06:45:09.282687 energy_base-1.6.3/src/energy_base/external_api/serializers/api_status.py
+-rw-r--r--   0        0        0       72 2024-04-05 06:45:09.280547 energy_base-1.6.3/src/energy_base/external_api/views/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-05 06:45:09.284881 energy_base-1.6.3/src/energy_base/external_api/views/api_status.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.871770 energy_base-1.6.3/src/energy_base/file_upload/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-05 06:38:25.872022 energy_base-1.6.3/src/energy_base/file_upload/admin.py
+-rw-r--r--   0        0        0      165 2024-04-05 06:38:25.872083 energy_base-1.6.3/src/energy_base/file_upload/apps.py
+-rw-r--r--   0        0        0      153 2024-04-05 06:38:25.872179 energy_base-1.6.3/src/energy_base/file_upload/data_processors/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-05 06:38:25.872248 energy_base-1.6.3/src/energy_base/file_upload/data_processors/base_sheet_processor.py
+-rw-r--r--   0        0        0      762 2024-04-05 06:38:25.872314 energy_base-1.6.3/src/energy_base/file_upload/data_processors/xls_processor.py
+-rw-r--r--   0        0        0       67 2024-04-05 06:38:25.872417 energy_base-1.6.3/src/energy_base/file_upload/filters/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-05 06:38:25.872478 energy_base-1.6.3/src/energy_base/file_upload/filters/file.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872541 energy_base-1.6.3/src/energy_base/file_upload/migrations/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-05 06:38:25.872667 energy_base-1.6.3/src/energy_base/file_upload/models/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-05 06:38:25.872729 energy_base-1.6.3/src/energy_base/file_upload/models/import_file.py
+-rw-r--r--   0        0        0      726 2024-04-05 06:38:25.872792 energy_base-1.6.3/src/energy_base/file_upload/models/temporary_data.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.872856 energy_base-1.6.3/src/energy_base/file_upload/serializers/__init__.py
+-rw-r--r--   0        0        0      710 2024-04-05 06:38:25.872951 energy_base-1.6.3/src/energy_base/file_upload/serializers/file.py
+-rw-r--r--   0        0        0       69 2024-04-05 06:38:25.873054 energy_base-1.6.3/src/energy_base/file_upload/services/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-05 06:38:25.873114 energy_base-1.6.3/src/energy_base/file_upload/services/minio.py
+-rw-r--r--   0        0        0      542 2024-04-05 06:38:25.873191 energy_base-1.6.3/src/energy_base/file_upload/urls.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873294 energy_base-1.6.3/src/energy_base/file_upload/views/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-05 06:38:25.873438 energy_base-1.6.3/src/energy_base/file_upload/views/file.py
+-rw-r--r--   0        0        0       77 2024-01-23 06:30:45.082611 energy_base-1.6.3/src/energy_base/models/__init__.py
+-rw-r--r--   0        0        0      298 2024-03-28 12:32:03.966843 energy_base-1.6.3/src/energy_base/models/jwt_user.py
+-rw-r--r--   0        0        0        0 2024-03-20 10:58:18.698302 energy_base-1.6.3/src/energy_base/q_api/__init__.py
+-rw-r--r--   0        0        0      153 2024-03-27 13:08:53.141117 energy_base-1.6.3/src/energy_base/q_api/apps.py
+-rw-r--r--   0        0        0       92 2024-03-27 13:05:43.703022 energy_base-1.6.3/src/energy_base/q_api/filters/__init__.py
+-rw-r--r--   0        0        0      133 2024-03-20 12:32:09.410169 energy_base-1.6.3/src/energy_base/q_api/filters/task.py
+-rw-r--r--   0        0        0      194 2024-03-27 13:08:53.144544 energy_base-1.6.3/src/energy_base/q_api/serializers/__init__.py
+-rw-r--r--   0        0        0      383 2024-03-27 13:08:53.146756 energy_base-1.6.3/src/energy_base/q_api/serializers/schedule.py
+-rw-r--r--   0        0        0      596 2024-03-29 04:25:10.738382 energy_base-1.6.3/src/energy_base/q_api/serializers/task.py
+-rw-r--r--   0        0        0      468 2024-03-28 06:56:59.203700 energy_base-1.6.3/src/energy_base/q_api/urls.py
+-rw-r--r--   0        0        0      216 2024-03-28 06:56:59.208785 energy_base-1.6.3/src/energy_base/q_api/views/__init__.py
+-rw-r--r--   0        0        0      838 2024-03-29 04:13:01.770648 energy_base-1.6.3/src/energy_base/q_api/views/schedule.py
+-rw-r--r--   0        0        0      516 2024-03-29 04:13:01.763075 energy_base-1.6.3/src/energy_base/q_api/views/task.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873512 energy_base-1.6.3/src/energy_base/references_api/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-05 06:38:25.873608 energy_base-1.6.3/src/energy_base/references_api/admin.py
+-rw-r--r--   0        0        0      171 2024-04-05 06:38:25.873676 energy_base-1.6.3/src/energy_base/references_api/apps.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:38:25.873746 energy_base-1.6.3/src/energy_base/references_api/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-05 06:38:25.873832 energy_base-1.6.3/src/energy_base/references_api/models.py
+-rw-r--r--   0        0        0       60 2024-04-05 06:38:25.873892 energy_base-1.6.3/src/energy_base/references_api/tests.py
+-rw-r--r--   0        0        0      390 2024-04-05 06:38:25.873959 energy_base-1.6.3/src/energy_base/references_api/urls.py
+-rw-r--r--   0        0        0     3575 2024-04-05 06:38:25.874023 energy_base-1.6.3/src/energy_base/references_api/utils.py
+-rw-r--r--   0        0        0      115 2024-04-05 06:38:25.874925 energy_base-1.6.3/src/energy_base/services/__init__.py
+-rw-r--r--   0        0        0     1468 2024-03-05 05:53:43.397963 energy_base-1.6.3/src/energy_base/services/minio.py
+-rw-r--r--   0        0        0      757 2024-04-05 06:45:09.277605 energy_base-1.6.3/src/energy_base/services/telnet.py
+-rw-r--r--   0        0        0      503 2024-04-05 06:38:25.874994 energy_base-1.6.3/src/energy_base/services/user.py
+-rw-r--r--   0        0        0      194 2024-03-05 06:28:37.626781 energy_base-1.6.3/src/energy_base/translation/__init__.py
+-rw-r--r--   0        0        0      344 2024-03-05 06:49:11.397042 energy_base-1.6.3/src/energy_base/translation/utils.py
+-rw-r--r--   0        0        0      167 2024-03-19 09:20:40.790206 energy_base-1.6.3/src/energy_base/utils/__init__.py
+-rw-r--r--   0        0        0     1356 2024-03-19 09:20:40.790318 energy_base-1.6.3/src/energy_base/utils/data.py
+-rw-r--r--   0        0        0     1535 2024-03-20 07:33:11.117325 energy_base-1.6.3/src/energy_base/utils/date.py
+-rw-r--r--   0        0        0      758 2024-02-29 10:58:24.635825 energy_base-1.6.3/src/energy_base/utils/dict_util.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 energy_base-1.6.3/PKG-INFO
```

### Comparing `energy_base-1.6.2/src/energy_base/api/base.py` & `energy_base-1.6.3/src/energy_base/api/base.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from django.utils import timezone
-from django.utils.translation import activate, get_language
-from rest_framework.request import Request
-from rest_framework.views import APIView
-
-from energy_base.models import JWTUser
-
-
-class BaseRequest(Request):
-
-    @property
-    def user(self) -> JWTUser:
-        return super(BaseRequest, self).user()
-
-
-class BaseAPIView(APIView):
-    user_id_assign_fields_on_create = []
-    user_id_assign_fields_on_update = []
-    user_id_assign_fields_on_delete = []
-    deleted_at_field = None
-
-    def __init__(self, **kwargs):
-        # Check user_id_assign_fields_on_create
-        assert isinstance(self.user_id_assign_fields_on_create, list), (
-            'Expected iterable user_id_assign_fields_on_create field'
-        )
-
-        # Check user_id_assign_fields_on_update
-        assert isinstance(self.user_id_assign_fields_on_update, list), (
-            'Expected iterable user_id_assign_fields_on_update field'
-        )
-
-        # Check user_id_assign_fields_on_delete
-        assert isinstance(self.user_id_assign_fields_on_delete, list), (
-            'Expected iterable user_id_assign_fields_on_delete field'
-        )
-
-        # Check deleted_at_field
-        assert isinstance(self.deleted_at_field, (str, type(None))), (
-            'Expected str | None deleted_at_field field'
-        )
-        super().__init__(**kwargs)
-        self.request: BaseRequest | None = None
-
-    def perform_create(self, serializer):
-        kws = {}
-        for attr in getattr(self, 'user_id_assign_fields_on_create', []):
-            kws[attr] = self.request.user.id
-        serializer.save(**kws)
-
-    def perform_update(self, serializer):
-        kws = {}
-        for attr in getattr(self, 'user_id_assign_fields_on_update', []):
-            kws[attr] = self.request.user.id
-        serializer.save(**kws)
-
-    def perform_destroy(self, instance):
-        for attr in getattr(self, 'user_id_assign_fields_on_delete', []):
-            setattr(instance, attr, self.request.user.id)
-        if self.deleted_at_field and hasattr(instance, self.deleted_at_field):
-            setattr(instance, self.deleted_at_field, timezone.now())
-        instance.save()
-
-    def update_lang(self):
-        activate(self.get_language())
-
-    def get_language(self):
-        return self.request.headers.get('accept-language') or get_language()
+from django.utils import timezone
+from django.utils.translation import activate, get_language
+from rest_framework.request import Request
+from rest_framework.views import APIView
+
+from energy_base.models import JWTUser
+
+
+class BaseRequest(Request):
+
+    @property
+    def user(self) -> JWTUser:
+        return super(BaseRequest, self).user()
+
+
+class BaseAPIView(APIView):
+    user_id_assign_fields_on_create = []
+    user_id_assign_fields_on_update = []
+    user_id_assign_fields_on_delete = []
+    deleted_at_field = None
+
+    def __init__(self, **kwargs):
+        # Check user_id_assign_fields_on_create
+        assert isinstance(self.user_id_assign_fields_on_create, list), (
+            'Expected iterable user_id_assign_fields_on_create field'
+        )
+
+        # Check user_id_assign_fields_on_update
+        assert isinstance(self.user_id_assign_fields_on_update, list), (
+            'Expected iterable user_id_assign_fields_on_update field'
+        )
+
+        # Check user_id_assign_fields_on_delete
+        assert isinstance(self.user_id_assign_fields_on_delete, list), (
+            'Expected iterable user_id_assign_fields_on_delete field'
+        )
+
+        # Check deleted_at_field
+        assert isinstance(self.deleted_at_field, (str, type(None))), (
+            'Expected str | None deleted_at_field field'
+        )
+        super().__init__(**kwargs)
+        self.request: BaseRequest | None = None
+
+    def perform_create(self, serializer):
+        kws = {}
+        for attr in getattr(self, 'user_id_assign_fields_on_create', []):
+            kws[attr] = self.request.user.id
+        serializer.save(**kws)
+
+    def perform_update(self, serializer):
+        kws = {}
+        for attr in getattr(self, 'user_id_assign_fields_on_update', []):
+            kws[attr] = self.request.user.id
+        serializer.save(**kws)
+
+    def perform_destroy(self, instance):
+        for attr in getattr(self, 'user_id_assign_fields_on_delete', []):
+            setattr(instance, attr, self.request.user.id)
+        if self.deleted_at_field and hasattr(instance, self.deleted_at_field):
+            setattr(instance, self.deleted_at_field, timezone.now())
+        instance.save()
+
+    def update_lang(self):
+        activate(self.get_language())
+
+    def get_language(self):
+        return self.request.headers.get('accept-language') or get_language()
```

### Comparing `energy_base-1.6.2/src/energy_base/authentications/microservice_authentication.py` & `energy_base-1.6.3/src/energy_base/authentications/microservice_authentication.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ipaddress import ip_address, ip_network
-
-from rest_framework import authentication
-
-from energy_base.authentications import MicroserviceUser
-
-
-class MicroserviceUserAuthentication(authentication.BaseAuthentication):
-    # List of local IP address ranges
-    local_ip_ranges = [
-        '127.0.0.0/8',  # Loopback addresses
-        '10.0.0.0/8',  # Private network addresses
-        '172.16.0.0/12',  # Private network addresses
-        '192.168.0.0/16',  # Private network addresses
-        # Add more local ranges if needed
-    ]
-
-    def authenticate(self, request):
-        client_ip = request.META.get('REMOTE_ADDR', None)
-        server_ip = request.META.get('SERVER_ADDR', None)
-
-        if any(ip_address(client_ip) in ip_network(ip_range, strict=False) for ip_range in self.local_ip_ranges):
-            return self.get_user(), None
-
-        if client_ip == server_ip:
-            return self.get_user(), None
-
-    def get_user(self) -> MicroserviceUser:
-        return MicroserviceUser()
+from ipaddress import ip_address, ip_network
+
+from rest_framework import authentication
+
+from energy_base.authentications import MicroserviceUser
+
+
+class MicroserviceUserAuthentication(authentication.BaseAuthentication):
+    # List of local IP address ranges
+    local_ip_ranges = [
+        '127.0.0.0/8',  # Loopback addresses
+        '10.0.0.0/8',  # Private network addresses
+        '172.16.0.0/12',  # Private network addresses
+        '192.168.0.0/16',  # Private network addresses
+        # Add more local ranges if needed
+    ]
+
+    def authenticate(self, request):
+        client_ip = request.META.get('REMOTE_ADDR', None)
+        server_ip = request.META.get('SERVER_ADDR', None)
+
+        if any(ip_address(client_ip) in ip_network(ip_range, strict=False) for ip_range in self.local_ip_ranges):
+            return self.get_user(), None
+
+        if client_ip == server_ip:
+            return self.get_user(), None
+
+    def get_user(self) -> MicroserviceUser:
+        return MicroserviceUser()
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/data_processors/xls_processor.py` & `energy_base-1.6.3/src/energy_base/file_upload/data_processors/xls_processor.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from io import BytesIO
-
-from openpyxl import load_workbook
-
-from .base_sheet_processor import BaseSheetProcessor
-
-
-class XlsProcessor:
-
-    def __init__(self, file: str | bytes):
-        self.file = file
-        self.wb = load_workbook(BytesIO(self.file))
-
-    def get_data(self, sheet_processor: BaseSheetProcessor):
-        return sheet_processor.get_data(self.wb)
-
-    def validate(self, sheet_processor: BaseSheetProcessor):
-        return sheet_processor.validate(self.wb)
-
-    def validate_many(self, sheet_processors: list[BaseSheetProcessor]):
-        errors = {}
-        for sheet_processor in sheet_processors:
-            error = self.validate(sheet_processor)
-            if error:
-                errors.update(error)
-
-        return errors or None
+from io import BytesIO
+
+from openpyxl import load_workbook
+
+from .base_sheet_processor import BaseSheetProcessor
+
+
+class XlsProcessor:
+
+    def __init__(self, file: str | bytes):
+        self.file = file
+        self.wb = load_workbook(BytesIO(self.file))
+
+    def get_data(self, sheet_processor: BaseSheetProcessor):
+        return sheet_processor.get_data(self.wb)
+
+    def validate(self, sheet_processor: BaseSheetProcessor):
+        return sheet_processor.validate(self.wb)
+
+    def validate_many(self, sheet_processors: list[BaseSheetProcessor]):
+        errors = {}
+        for sheet_processor in sheet_processors:
+            error = self.validate(sheet_processor)
+            if error:
+                errors.update(error)
+
+        return errors or None
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/models/import_file.py` & `energy_base-1.6.3/src/energy_base/file_upload/models/import_file.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import uuid
-
-from django.conf import settings
-from django.db import models
-
-
-class FileStatus(models.TextChoices):
-    DRAFT = 'DRAFT'
-    SUCCESS = 'SUCCESS'
-    ERROR = 'ERROR'
-    PROCESS = 'PROCESS'
-
-
-class ImportFile(models.Model):
-    Status = FileStatus
-
-    id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
-    date = models.DateField()
-    real_name = models.CharField(max_length=500)
-    store_name = models.CharField(max_length=500)
-    size = models.BigIntegerField()
-    status = models.CharField(max_length=20, choices=FileStatus.choices)
-    active = models.BooleanField()
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
-    deleted_at = models.DateTimeField(blank=True, null=True)
-    created_by = models.UUIDField()
-    updated_by = models.UUIDField(blank=True, null=True)
-    deleted_by = models.UUIDField(blank=True, null=True)
-
-    class Meta:
-        app_label = settings.FILE_UPLOAD_APP_LABEL or 'file_upload'
-        db_table = 'import_files'
-        ordering = ('-created_at',)
+import uuid
+
+from django.conf import settings
+from django.db import models
+
+
+class FileStatus(models.TextChoices):
+    DRAFT = 'DRAFT'
+    SUCCESS = 'SUCCESS'
+    ERROR = 'ERROR'
+    PROCESS = 'PROCESS'
+
+
+class ImportFile(models.Model):
+    Status = FileStatus
+
+    id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
+    date = models.DateField()
+    real_name = models.CharField(max_length=500)
+    store_name = models.CharField(max_length=500)
+    size = models.BigIntegerField()
+    status = models.CharField(max_length=20, choices=FileStatus.choices)
+    active = models.BooleanField()
+    created_at = models.DateTimeField(auto_now_add=True)
+    updated_at = models.DateTimeField(auto_now=True)
+    deleted_at = models.DateTimeField(blank=True, null=True)
+    created_by = models.UUIDField()
+    updated_by = models.UUIDField(blank=True, null=True)
+    deleted_by = models.UUIDField(blank=True, null=True)
+
+    class Meta:
+        app_label = settings.FILE_UPLOAD_APP_LABEL or 'file_upload'
+        db_table = 'import_files'
+        ordering = ('-created_at',)
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/models/temporary_data.py` & `energy_base-1.6.3/src/energy_base/file_upload/models/temporary_data.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import uuid
-
-from django.db import models
-
-from ..models import ImportFile
-
-
-class TemporaryData(models.Model):
-    id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
-    file = models.ForeignKey(ImportFile, on_delete=models.CASCADE)
-    data = models.JSONField()
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
-    deleted_at = models.DateTimeField(blank=True, null=True)
-    created_by = models.UUIDField()
-    updated_by = models.UUIDField(blank=True, null=True)
-    deleted_by = models.UUIDField(blank=True, null=True)
-
-    class Meta:
-        app_label = 'main'
-        db_table = 'temporary_data'
-        ordering = ('-created_at',)
+import uuid
+
+from django.db import models
+
+from ..models import ImportFile
+
+
+class TemporaryData(models.Model):
+    id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
+    file = models.ForeignKey(ImportFile, on_delete=models.CASCADE)
+    data = models.JSONField()
+    created_at = models.DateTimeField(auto_now_add=True)
+    updated_at = models.DateTimeField(auto_now=True)
+    deleted_at = models.DateTimeField(blank=True, null=True)
+    created_by = models.UUIDField()
+    updated_by = models.UUIDField(blank=True, null=True)
+    deleted_by = models.UUIDField(blank=True, null=True)
+
+    class Meta:
+        app_label = 'main'
+        db_table = 'temporary_data'
+        ordering = ('-created_at',)
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/serializers/file.py` & `energy_base-1.6.3/src/energy_base/file_upload/serializers/file.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from django.core.validators import FileExtensionValidator
-from rest_framework import serializers
-
-from ..models import ImportFile
-
-
-class ImportFileSerializer(serializers.ModelSerializer):
-    created_by = serializers.DictField()
-
-    class Meta:
-        model = ImportFile
-        fields = '__all__'
-
-
-class FileDownloadSerializer(serializers.Serializer):
-    file = serializers.FileField()
-
-
-class FileUploadSerializer(serializers.Serializer):
-    file = serializers.FileField(validators=[FileExtensionValidator(allowed_extensions=['xls', 'xlsx'])])
-    date = serializers.DateField()
-
-
-class FileConfirmSerializer(serializers.ModelSerializer):
-    class Meta:
-        model = ImportFile
-        fields = []
+from django.core.validators import FileExtensionValidator
+from rest_framework import serializers
+
+from ..models import ImportFile
+
+
+class ImportFileSerializer(serializers.ModelSerializer):
+    created_by = serializers.DictField()
+
+    class Meta:
+        model = ImportFile
+        fields = '__all__'
+
+
+class FileDownloadSerializer(serializers.Serializer):
+    file = serializers.FileField()
+
+
+class FileUploadSerializer(serializers.Serializer):
+    file = serializers.FileField(validators=[FileExtensionValidator(allowed_extensions=['xls', 'xlsx'])])
+    date = serializers.DateField()
+
+
+class FileConfirmSerializer(serializers.ModelSerializer):
+    class Meta:
+        model = ImportFile
+        fields = []
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/urls.py` & `energy_base-1.6.3/src/energy_base/file_upload/urls.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from django.urls import path
-
-from .views.file import ImportFileViewSet, FileDownloadViewSet, FileUploadViewSet, FileConfirmViewSet
-from ..api.routers import OptionalSlashRouter
-
-router = OptionalSlashRouter()
-router.register('files', ImportFileViewSet, 'files')
-
-urlpatterns = [
-    path('files/<pk>/download/', FileDownloadViewSet.as_view(), name='download'),
-    path('files/upload/', FileUploadViewSet.as_view(), name='upload'),
-    path('files/<pk>/confirm/', FileConfirmViewSet.as_view(), name='confirm'),
-]
-
-urlpatterns += router.urls
+from django.urls import path
+
+from .views.file import ImportFileViewSet, FileDownloadViewSet, FileUploadViewSet, FileConfirmViewSet
+from ..api.routers import OptionalSlashRouter
+
+router = OptionalSlashRouter()
+router.register('files', ImportFileViewSet, 'files')
+
+urlpatterns = [
+    path('files/<pk>/download/', FileDownloadViewSet.as_view(), name='download'),
+    path('files/upload/', FileUploadViewSet.as_view(), name='upload'),
+    path('files/<pk>/confirm/', FileConfirmViewSet.as_view(), name='confirm'),
+]
+
+urlpatterns += router.urls
```

### Comparing `energy_base-1.6.2/src/energy_base/file_upload/views/file.py` & `energy_base-1.6.3/src/energy_base/file_upload/views/file.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-import importlib
-import mimetypes
-import os
-import uuid
-
-from django.conf import settings
-from django.core.files.uploadedfile import InMemoryUploadedFile
-from django.http import HttpResponse
-from django_filters.rest_framework.backends import DjangoFilterBackend
-from rest_framework import viewsets, filters, status
-from rest_framework.parsers import MultiPartParser
-from rest_framework.response import Response
-
-from ..data_processors import XlsProcessor
-from ..filters import FileFilterSet
-from ..models import ImportFile, TemporaryData
-from ..serializers.file import (
-    FileDownloadSerializer,
-    ImportFileSerializer,
-    FileUploadSerializer,
-    FileConfirmSerializer
-)
-from ..services import minio_service
-from ...api import pagination
-from ...api.base import BaseAPIView, BaseRequest
-from ...services import UserService
-
-data_processors = []
-for processor_class in settings.DATA_PROCESSORS_CLASSES:
-    module_name, class_name = processor_class.rsplit('.', 1)
-    module = importlib.import_module(module_name)
-    data_processors.append(getattr(module, class_name))
-
-
-class ImportFileViewSet(viewsets.GenericViewSet, viewsets.generics.ListAPIView):
-    queryset = ImportFile.objects.all()
-    serializer_class = ImportFileSerializer
-    filter_backends = (filters.OrderingFilter, DjangoFilterBackend)
-    filterset_class = FileFilterSet
-    pagination_class = pagination.SmallResultsSetPagination
-
-    def list(self, request, *args, **kwargs):
-        queryset = self.filter_queryset(self.get_queryset())
-        queryset = self.paginate_queryset(queryset)
-
-        files = list(queryset)
-
-        created_bys = []
-        for file in files:
-            created_bys.append(str(file.created_by))
-
-        users = UserService.get_users(created_bys)
-        users = {u['id']: u for u in users}
-
-        for file in files:
-            creator = users.get(str(file.created_by), {})
-
-            file.created_by = {
-                'id': creator.get('id'),
-                'username': creator.get('username'),
-                'firstName': creator.get('firstName'),
-                'surName': creator.get('surName'),
-                'midName': creator.get('midName'),
-            }
-
-        serializer = self.get_serializer(files, many=True)
-        return self.get_paginated_response(serializer.data)
-
-
-class FileDownloadViewSet(viewsets.generics.RetrieveAPIView):
-    queryset = ImportFile.objects.all()
-    serializer_class = FileDownloadSerializer
-
-    def retrieve(self, request, *args, **kwargs):
-        obj = self.get_object()
-        file_bytes = minio_service.get_object('liquid-hydrocarbons', obj.store_name)
-        content_type, _ = mimetypes.guess_type(obj.real_name, strict=False)
-        response = HttpResponse(file_bytes, content_type=content_type or 'application/octet-stream')
-        response['Content-Length'] = len(file_bytes)
-        response['Content-Disposition'] = 'attachment; filename="%s"' % obj.real_name
-        return response
-
-
-class FileUploadViewSet(BaseAPIView, viewsets.generics.CreateAPIView):
-    serializer_class = FileUploadSerializer
-    parser_classes = (MultiPartParser,)
-
-    def create(self, request: BaseRequest, *args, **kwargs):
-        serializer = self.get_serializer(data=request.data)
-        serializer.is_valid(raise_exception=True)
-
-        file: InMemoryUploadedFile = serializer.validated_data.get('file')
-        xls_processor = XlsProcessor(file.read())
-        errors = xls_processor.validate_many([data_processor() for data_processor in data_processors])
-
-        if errors:
-            return Response({
-                'sheets': errors
-            }, status=status.HTTP_400_BAD_REQUEST)
-
-        file.seek(0)
-
-        random_str = uuid.uuid4().hex
-        date = serializer.validated_data.get('date').strftime('%Y-%m-%d')
-        file_extension = os.path.splitext(file.name)[1]
-        store_name = f'{date}--{random_str}{file_extension}'
-
-        minio_service.put_object('liquid-hydrocarbons', store_name, file)
-
-        import_file = ImportFile(
-            date=serializer.validated_data.get('date'),
-            real_name=file.name,
-            store_name=store_name,
-            size=file.size,
-            status=ImportFile.Status.DRAFT,
-            active=False,
-            created_by=self.request.user.pk,
-        )
-        import_file.save()
-
-        data = {}
-        for data_processor in data_processors:
-            data[data_processor.sheet_index] = xls_processor.get_data(data_processor())
-
-        temporary_data = TemporaryData(
-            file=import_file,
-            data=data,
-            created_by=self.request.user.pk
-        )
-        temporary_data.save()
-
-        return Response(
-            data={
-                'success': True,
-                'file_id': import_file.pk
-            },
-            status=status.HTTP_201_CREATED
-        )
-
-
-class FileConfirmViewSet(BaseAPIView, viewsets.generics.UpdateAPIView):
-    serializer_class = FileConfirmSerializer
-    http_method_names = ['patch']
-    queryset = ImportFile.objects.filter(status=ImportFile.Status.DRAFT, active=False).all()
-
-    def perform_update(self, serializer):
-        model: ImportFile = self.get_object()
-        temp = TemporaryData.objects.filter(file=model).get()
-        data = temp.data
-        for data_processor in data_processors:
-            data_processor().write_db(
-                data.get(str(data_processor.sheet_index)),
-                model,
-                self.request.user.pk,
-            )
-        temp.delete()
-        ImportFile.objects.filter(active=True, date=model.date).update(active=False)
-        serializer.save(status=ImportFile.Status.SUCCESS, active=True)
+import importlib
+import mimetypes
+import os
+import uuid
+
+from django.conf import settings
+from django.core.files.uploadedfile import InMemoryUploadedFile
+from django.http import HttpResponse
+from django_filters.rest_framework.backends import DjangoFilterBackend
+from rest_framework import viewsets, filters, status
+from rest_framework.parsers import MultiPartParser
+from rest_framework.response import Response
+
+from ..data_processors import XlsProcessor
+from ..filters import FileFilterSet
+from ..models import ImportFile, TemporaryData
+from ..serializers.file import (
+    FileDownloadSerializer,
+    ImportFileSerializer,
+    FileUploadSerializer,
+    FileConfirmSerializer
+)
+from ..services import minio_service
+from ...api import pagination
+from ...api.base import BaseAPIView, BaseRequest
+from ...services import UserService
+
+data_processors = []
+for processor_class in settings.DATA_PROCESSORS_CLASSES:
+    module_name, class_name = processor_class.rsplit('.', 1)
+    module = importlib.import_module(module_name)
+    data_processors.append(getattr(module, class_name))
+
+
+class ImportFileViewSet(viewsets.GenericViewSet, viewsets.generics.ListAPIView):
+    queryset = ImportFile.objects.all()
+    serializer_class = ImportFileSerializer
+    filter_backends = (filters.OrderingFilter, DjangoFilterBackend)
+    filterset_class = FileFilterSet
+    pagination_class = pagination.SmallResultsSetPagination
+
+    def list(self, request, *args, **kwargs):
+        queryset = self.filter_queryset(self.get_queryset())
+        queryset = self.paginate_queryset(queryset)
+
+        files = list(queryset)
+
+        created_bys = []
+        for file in files:
+            created_bys.append(str(file.created_by))
+
+        users = UserService.get_users(created_bys)
+        users = {u['id']: u for u in users}
+
+        for file in files:
+            creator = users.get(str(file.created_by), {})
+
+            file.created_by = {
+                'id': creator.get('id'),
+                'username': creator.get('username'),
+                'firstName': creator.get('firstName'),
+                'surName': creator.get('surName'),
+                'midName': creator.get('midName'),
+            }
+
+        serializer = self.get_serializer(files, many=True)
+        return self.get_paginated_response(serializer.data)
+
+
+class FileDownloadViewSet(viewsets.generics.RetrieveAPIView):
+    queryset = ImportFile.objects.all()
+    serializer_class = FileDownloadSerializer
+
+    def retrieve(self, request, *args, **kwargs):
+        obj = self.get_object()
+        file_bytes = minio_service.get_object('liquid-hydrocarbons', obj.store_name)
+        content_type, _ = mimetypes.guess_type(obj.real_name, strict=False)
+        response = HttpResponse(file_bytes, content_type=content_type or 'application/octet-stream')
+        response['Content-Length'] = len(file_bytes)
+        response['Content-Disposition'] = 'attachment; filename="%s"' % obj.real_name
+        return response
+
+
+class FileUploadViewSet(BaseAPIView, viewsets.generics.CreateAPIView):
+    serializer_class = FileUploadSerializer
+    parser_classes = (MultiPartParser,)
+
+    def create(self, request: BaseRequest, *args, **kwargs):
+        serializer = self.get_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+
+        file: InMemoryUploadedFile = serializer.validated_data.get('file')
+        xls_processor = XlsProcessor(file.read())
+        errors = xls_processor.validate_many([data_processor() for data_processor in data_processors])
+
+        if errors:
+            return Response({
+                'sheets': errors
+            }, status=status.HTTP_400_BAD_REQUEST)
+
+        file.seek(0)
+
+        random_str = uuid.uuid4().hex
+        date = serializer.validated_data.get('date').strftime('%Y-%m-%d')
+        file_extension = os.path.splitext(file.name)[1]
+        store_name = f'{date}--{random_str}{file_extension}'
+
+        minio_service.put_object('liquid-hydrocarbons', store_name, file)
+
+        import_file = ImportFile(
+            date=serializer.validated_data.get('date'),
+            real_name=file.name,
+            store_name=store_name,
+            size=file.size,
+            status=ImportFile.Status.DRAFT,
+            active=False,
+            created_by=self.request.user.pk,
+        )
+        import_file.save()
+
+        data = {}
+        for data_processor in data_processors:
+            data[data_processor.sheet_index] = xls_processor.get_data(data_processor())
+
+        temporary_data = TemporaryData(
+            file=import_file,
+            data=data,
+            created_by=self.request.user.pk
+        )
+        temporary_data.save()
+
+        return Response(
+            data={
+                'success': True,
+                'file_id': import_file.pk
+            },
+            status=status.HTTP_201_CREATED
+        )
+
+
+class FileConfirmViewSet(BaseAPIView, viewsets.generics.UpdateAPIView):
+    serializer_class = FileConfirmSerializer
+    http_method_names = ['patch']
+    queryset = ImportFile.objects.filter(status=ImportFile.Status.DRAFT, active=False).all()
+
+    def perform_update(self, serializer):
+        model: ImportFile = self.get_object()
+        temp = TemporaryData.objects.filter(file=model).get()
+        data = temp.data
+        for data_processor in data_processors:
+            data_processor().write_db(
+                data.get(str(data_processor.sheet_index)),
+                model,
+                self.request.user.pk,
+            )
+        temp.delete()
+        ImportFile.objects.filter(active=True, date=model.date).update(active=False)
+        serializer.save(status=ImportFile.Status.SUCCESS, active=True)
```

### Comparing `energy_base-1.6.2/src/energy_base/q_api/views/schedule.py` & `energy_base-1.6.3/src/energy_base/q_api/views/schedule.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from django.utils import timezone
-from django_q.models import Schedule
-from drf_spectacular.utils import extend_schema
-from rest_framework import viewsets
-
-from energy_base.api.permissions import IsSuperUser
-from energy_base.q_api.serializers import ScheduleSerializer
-
-
-@extend_schema(tags=['admin/schedules'])
-class ScheduleViewSet(viewsets.ModelViewSet):
-    http_method_names = ['get', 'patch']
-    queryset = Schedule.objects.all()
-    serializer_class = ScheduleSerializer
-    permission_classes = [IsSuperUser]
-
-
-@extend_schema(tags=['admin/schedules'], request={})
-class ScheduleRunNowView(viewsets.generics.UpdateAPIView):
-    serializer_class = ScheduleSerializer
-    http_method_names = ['patch']
-    queryset = Schedule.objects.all()
-
-    def perform_update(self, serializer):
-        serializer.save(next_run=timezone.now())
+from django.utils import timezone
+from django_q.models import Schedule
+from drf_spectacular.utils import extend_schema
+from rest_framework import viewsets
+
+from energy_base.api.permissions import IsSuperUser
+from energy_base.q_api.serializers import ScheduleSerializer
+
+
+@extend_schema(tags=['admin/schedules'])
+class ScheduleViewSet(viewsets.ModelViewSet):
+    http_method_names = ['get', 'patch']
+    queryset = Schedule.objects.all()
+    serializer_class = ScheduleSerializer
+    permission_classes = [IsSuperUser]
+
+
+@extend_schema(tags=['admin/schedules'], request={})
+class ScheduleRunNowView(viewsets.generics.UpdateAPIView):
+    serializer_class = ScheduleSerializer
+    http_method_names = ['patch']
+    queryset = Schedule.objects.all()
+
+    def perform_update(self, serializer):
+        serializer.save(next_run=timezone.now())
```

### Comparing `energy_base-1.6.2/src/energy_base/services/minio.py` & `energy_base-1.6.3/src/energy_base/services/minio.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import mimetypes
-from typing import BinaryIO
-
-from django.core.files.uploadedfile import InMemoryUploadedFile
-from minio import Minio
-
-
-class MinioService:
-    def __init__(self, endpoint, access_key, secret_key):
-        self.client = Minio(
-            endpoint=endpoint,
-            access_key=access_key,
-            secret_key=secret_key,
-            secure=False
-        )
-
-    def fput_object(self, bucket_name, object_name, file_path):
-        content_type, *_ = mimetypes.guess_type(file_path)
-        return self.client.fput_object(bucket_name, object_name, file_path, content_type=content_type)
-
-    def put_object(self, bucket_name, object_name, file: BinaryIO | InMemoryUploadedFile):
-        content_type = "application/octet-stream"
-        length = -1
-        if hasattr(file, 'content_type'):
-            content_type = file.content_type
-        if hasattr(file, '__len__'):
-            length = len(file)
-        return self.client.put_object(bucket_name, object_name, file,
-                                      length=length,
-                                      content_type=content_type,
-                                      part_size=10 * 1024 * 1024)
-
-    def get_object(self, bucket_name, object_name):
-        try:
-            response = self.client.get_object(bucket_name, object_name)
-            object_bytes = response.read()
-        finally:
-            response.close()
-            response.release_conn()
-        return object_bytes
+import mimetypes
+from typing import BinaryIO
+
+from django.core.files.uploadedfile import InMemoryUploadedFile
+from minio import Minio
+
+
+class MinioService:
+    def __init__(self, endpoint, access_key, secret_key):
+        self.client = Minio(
+            endpoint=endpoint,
+            access_key=access_key,
+            secret_key=secret_key,
+            secure=False
+        )
+
+    def fput_object(self, bucket_name, object_name, file_path):
+        content_type, *_ = mimetypes.guess_type(file_path)
+        return self.client.fput_object(bucket_name, object_name, file_path, content_type=content_type)
+
+    def put_object(self, bucket_name, object_name, file: BinaryIO | InMemoryUploadedFile):
+        content_type = "application/octet-stream"
+        length = -1
+        if hasattr(file, 'content_type'):
+            content_type = file.content_type
+        if hasattr(file, '__len__'):
+            length = len(file)
+        return self.client.put_object(bucket_name, object_name, file,
+                                      length=length,
+                                      content_type=content_type,
+                                      part_size=10 * 1024 * 1024)
+
+    def get_object(self, bucket_name, object_name):
+        try:
+            response = self.client.get_object(bucket_name, object_name)
+            object_bytes = response.read()
+        finally:
+            response.close()
+            response.release_conn()
+        return object_bytes
```

### Comparing `energy_base-1.6.2/src/energy_base/utils/data.py` & `energy_base-1.6.3/src/energy_base/utils/data.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from copy import deepcopy
-
-
-def deep_map(data: dict | list, func_cond, func_map, in_place=True):
-    if not in_place:
-        data = deepcopy(data)
-
-    if isinstance(data, dict):
-        for key, value in data.items():
-            if isinstance(value, (list, dict)):
-                deep_map(value, func_cond, func_map, True)
-            elif func_cond(value):
-                data[key] = func_map(value)
-    elif isinstance(data, list):
-        for index, value in enumerate(data):
-            if isinstance(value, (list, dict)):
-                deep_map(value, func_cond, func_map, True)
-            elif func_cond(value):
-                data[index] = func_map(value)
-
-    return data
-
-
-def null_to_zero(data: dict | list, in_place=True):
-    return deep_map(data, lambda value: value is None, lambda _: 0, in_place)
-
-
-def deep_round(data: dict | list, ndigits: int, in_place=True):
-    return deep_map(data, lambda value: isinstance(value, float), lambda value: round(value, ndigits), in_place)
-
-
-class EData:
-    def __init__(self, data):
-        self.data = data
-
-    def null_to_zero(self):
-        null_to_zero(self.data)
-        return self
-
-    def round(self, ndigits: int):
-        deep_round(self.data, ndigits)
-        return self
-
-    def map(self, func_cond, func_map):
-        deep_map(self.data, func_cond, func_map)
-        return self
+from copy import deepcopy
+
+
+def deep_map(data: dict | list, func_cond, func_map, in_place=True):
+    if not in_place:
+        data = deepcopy(data)
+
+    if isinstance(data, dict):
+        for key, value in data.items():
+            if isinstance(value, (list, dict)):
+                deep_map(value, func_cond, func_map, True)
+            elif func_cond(value):
+                data[key] = func_map(value)
+    elif isinstance(data, list):
+        for index, value in enumerate(data):
+            if isinstance(value, (list, dict)):
+                deep_map(value, func_cond, func_map, True)
+            elif func_cond(value):
+                data[index] = func_map(value)
+
+    return data
+
+
+def null_to_zero(data: dict | list, in_place=True):
+    return deep_map(data, lambda value: value is None, lambda _: 0, in_place)
+
+
+def deep_round(data: dict | list, ndigits: int, in_place=True):
+    return deep_map(data, lambda value: isinstance(value, float), lambda value: round(value, ndigits), in_place)
+
+
+class EData:
+    def __init__(self, data):
+        self.data = data
+
+    def null_to_zero(self):
+        null_to_zero(self.data)
+        return self
+
+    def round(self, ndigits: int):
+        deep_round(self.data, ndigits)
+        return self
+
+    def map(self, func_cond, func_map):
+        deep_map(self.data, func_cond, func_map)
+        return self
```

### Comparing `energy_base-1.6.2/src/energy_base/utils/date.py` & `energy_base-1.6.3/src/energy_base/utils/date.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from calendar import monthrange
-from datetime import date, datetime, timedelta
-
-DEFAULT_DATE_FORMAT = '%Y-%m-%d'
-
-
-def to_edate(date: date | datetime):
-    return EDate(date.year, date.month, date.day)
-
-
-class EDate(date):
-    def datetime(self):
-        return datetime(self.year, self.month, self.day)
-
-    def tomorrow(self):
-        return to_edate(self.datetime() + timedelta(days=1))
-
-    def yesterday(self):
-        return to_edate(self.datetime() - timedelta(days=1))
-
-    def first_day_of_month(self):
-        return self.replace(day=1)
-
-    def first_day_of_year(self):
-        return self.replace(day=1, month=1)
-
-    def last_day_of_month(self):
-        day1, ndays = monthrange(self.year, self.month)
-        return self.replace(day=ndays)
-
-    def last_day_of_year(self):
-        return self.replace(day=31, month=12)
-
-    def first_day_of_last_month(self):
-        return self.replace(day=1).yesterday().replace(day=1)
-
-    def first_day_of_last_year(self):
-        return self.replace(day=1, month=1, year=self.year - 1)
-
-    def last_day_of_last_month(self):
-        return self.replace(day=1).yesterday()
-
-    def last_day_of_last_year(self):
-        return self.replace(day=31, month=12, year=self.year - 1)
-
-    def strftime(self, __format=DEFAULT_DATE_FORMAT):
-        return super().strftime(__format)
-
-    @staticmethod
-    def strptime(__date_string: str, __format=DEFAULT_DATE_FORMAT):
-        return to_edate(datetime.strptime(__date_string, __format))
-
-    def __str__(self):
-        return self.strftime()
+from calendar import monthrange
+from datetime import date, datetime, timedelta
+
+DEFAULT_DATE_FORMAT = '%Y-%m-%d'
+
+
+def to_edate(date: date | datetime):
+    return EDate(date.year, date.month, date.day)
+
+
+class EDate(date):
+    def datetime(self):
+        return datetime(self.year, self.month, self.day)
+
+    def tomorrow(self):
+        return to_edate(self.datetime() + timedelta(days=1))
+
+    def yesterday(self):
+        return to_edate(self.datetime() - timedelta(days=1))
+
+    def first_day_of_month(self):
+        return self.replace(day=1)
+
+    def first_day_of_year(self):
+        return self.replace(day=1, month=1)
+
+    def last_day_of_month(self):
+        day1, ndays = monthrange(self.year, self.month)
+        return self.replace(day=ndays)
+
+    def last_day_of_year(self):
+        return self.replace(day=31, month=12)
+
+    def first_day_of_last_month(self):
+        return self.replace(day=1).yesterday().replace(day=1)
+
+    def first_day_of_last_year(self):
+        return self.replace(day=1, month=1, year=self.year - 1)
+
+    def last_day_of_last_month(self):
+        return self.replace(day=1).yesterday()
+
+    def last_day_of_last_year(self):
+        return self.replace(day=31, month=12, year=self.year - 1)
+
+    def strftime(self, __format=DEFAULT_DATE_FORMAT):
+        return super().strftime(__format)
+
+    @staticmethod
+    def strptime(__date_string: str, __format=DEFAULT_DATE_FORMAT):
+        return to_edate(datetime.strptime(__date_string, __format))
+
+    def __str__(self):
+        return self.strftime()
```

### Comparing `energy_base-1.6.2/src/energy_base/utils/dict_util.py` & `energy_base-1.6.3/src/energy_base/utils/dict_util.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-def get_by_dotted(dict_obj: dict, dotted_key: str, default=None):
-    """
-    Get a value from a dictionary using a dotted key notation.
-
-    Args:
-        dict_obj (dict): The dictionary to retrieve the value from.
-        dotted_key (str): The dotted key notation to access nested keys.
-        default: The default value to return if the key is not found.
-
-    Returns:
-        The value at the given dotted key, or default if not found.
-    """
-    parts = dotted_key.split('.')
-    for part in parts:
-        # Check if current part is in the dictionary and is a dictionary itself
-        if isinstance(dict_obj, dict) and part in dict_obj:
-            dict_obj = dict_obj.get(part, default)
-        else:
-            return default
-    return dict_obj
+def get_by_dotted(dict_obj: dict, dotted_key: str, default=None):
+    """
+    Get a value from a dictionary using a dotted key notation.
+
+    Args:
+        dict_obj (dict): The dictionary to retrieve the value from.
+        dotted_key (str): The dotted key notation to access nested keys.
+        default: The default value to return if the key is not found.
+
+    Returns:
+        The value at the given dotted key, or default if not found.
+    """
+    parts = dotted_key.split('.')
+    for part in parts:
+        # Check if current part is in the dictionary and is a dictionary itself
+        if isinstance(dict_obj, dict) and part in dict_obj:
+            dict_obj = dict_obj.get(part, default)
+        else:
+            return default
+    return dict_obj
```

### Comparing `energy_base-1.6.2/PKG-INFO` & `energy_base-1.6.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: energy-base
-Version: 1.6.2
+Version: 1.6.3
 Summary: Energy Base Package
 Author: Olimboy
 Author-email: shavkatov.olimboy@mail.ru
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: django (==4.2.9)
 Requires-Dist: django-filter (>=23.5,<24.0)
 Requires-Dist: django-q (>=1.3.9,<2.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: djangorestframework-simplejwt[crypto] (>=5.3.1,<6.0.0)
 Requires-Dist: drf-spectacular[sidecar] (>=0.27.1,<0.28.0)
```

