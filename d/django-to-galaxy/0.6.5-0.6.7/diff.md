# Comparing `tmp/django_to_galaxy-0.6.5.tar.gz` & `tmp/django_to_galaxy-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_to_galaxy-0.6.5.tar", max compression
+gzip compressed data, was "django_to_galaxy-0.6.7.tar", max compression
```

## Comparing `django_to_galaxy-0.6.5.tar` & `django_to_galaxy-0.6.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    34498 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/LICENSE
--rw-r--r--   0        0        0       41 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/__init__.py
--rw-r--r--   0        0        0      369 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/__init__.py
--rw-r--r--   0        0        0      159 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_element.py
--rw-r--r--   0        0        0      834 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_instance.py
--rw-r--r--   0        0        0     2321 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_output_file.py
--rw-r--r--   0        0        0     7278 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_user.py
--rw-r--r--   0        0        0     2562 2023-11-03 10:07:16.026196 django_to_galaxy-0.6.5/django_to_galaxy/admin/history.py
--rw-r--r--   0        0        0     4821 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/admin/invocation.py
--rw-r--r--   0        0        0      315 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/admin/tag.py
--rw-r--r--   0        0        0     1360 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/admin/workflow.py
--rw-r--r--   0        0        0        0 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/__init__.py
--rw-r--r--   0        0        0     1079 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py
--rw-r--r--   0        0        0      257 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/galaxy_instance.py
--rw-r--r--   0        0        0      428 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/galaxy_output_file.py
--rw-r--r--   0        0        0      674 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/galaxy_user.py
--rw-r--r--   0        0        0      387 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/history.py
--rw-r--r--   0        0        0      396 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/invocation.py
--rw-r--r--   0        0        0      657 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/invoke_workflow.py
--rw-r--r--   0        0        0      883 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/upload_to_history.py
--rw-r--r--   0        0        0      981 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/workflow.py
--rw-r--r--   0        0        0     1661 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/urls.py
--rw-r--r--   0        0        0      748 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/create_history.py
--rw-r--r--   0        0        0      434 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/galaxy_instance.py
--rw-r--r--   0        0        0      439 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/galaxy_output_file.py
--rw-r--r--   0        0        0      420 2023-11-03 10:07:16.027196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/galaxy_user.py
--rw-r--r--   0        0        0      394 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/history.py
--rw-r--r--   0        0        0     1318 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/invocation.py
--rw-r--r--   0        0        0     6530 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/invoke_workflow.py
--rw-r--r--   0        0        0     2972 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/upload_to_history.py
--rw-r--r--   0        0        0      401 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/api/views/workflow.py
--rw-r--r--   0        0        0      143 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/apps.py
--rw-r--r--   0        0        0     5954 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0001_new_initial.py
--rw-r--r--   0        0        0      965 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py
--rw-r--r--   0        0        0      515 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0003_invocation_create_time.py
--rw-r--r--   0        0        0     1506 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py
--rw-r--r--   0        0        0     1052 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py
--rw-r--r--   0        0        0     1180 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py
--rw-r--r--   0        0        0     2000 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py
--rw-r--r--   0        0        0      481 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0008_workflowinput_label.py
--rw-r--r--   0        0        0      500 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/0009_galaxyoutputfile_unique_galaxy_id_per_invocation.py
--rw-r--r--   0        0        0        0 2023-11-03 10:07:16.028196 django_to_galaxy-0.6.5/django_to_galaxy/migrations/__init__.py
--rw-r--r--   0        0        0      370 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/__init__.py
--rw-r--r--   0        0        0      889 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/accepted_input.py
--rw-r--r--   0        0        0     1537 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_element.py
--rw-r--r--   0        0        0      723 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_instance.py
--rw-r--r--   0        0        0     1915 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_output_file.py
--rw-r--r--   0        0        0     3264 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_user.py
--rw-r--r--   0        0        0     2635 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/history.py
--rw-r--r--   0        0        0     6870 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/invocation.py
--rw-r--r--   0        0        0     1891 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/models/workflow.py
--rw-r--r--   0        0        0        0 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/schemas/__init__.py
--rw-r--r--   0        0        0      396 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/schemas/dataset.py
--rw-r--r--   0        0        0      138 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/settings.py
--rw-r--r--   0        0        0     2389 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/templates/admin/import_workflows.html
--rw-r--r--   0        0        0      106 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/urls.py
--rw-r--r--   0        0        0     1625 2023-11-03 10:07:16.029196 django_to_galaxy-0.6.5/django_to_galaxy/utils.py
--rw-r--r--   0        0        0      111 2023-11-03 10:36:50.511839 django_to_galaxy-0.6.5/django_to_galaxy/version.py
--rw-r--r--   0        0        0      771 2023-11-03 10:43:56.712915 django_to_galaxy-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 django_to_galaxy-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    34498 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/LICENSE
+-rw-r--r--   0        0        0       41 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/__init__.py
+-rw-r--r--   0        0        0      369 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/__init__.py
+-rw-r--r--   0        0        0      159 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_element.py
+-rw-r--r--   0        0        0      834 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_instance.py
+-rw-r--r--   0        0        0     2321 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_output_file.py
+-rw-r--r--   0        0        0     7278 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_user.py
+-rw-r--r--   0        0        0     2562 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/history.py
+-rw-r--r--   0        0        0     5121 2024-04-04 15:13:17.375293 django_to_galaxy-0.6.7/django_to_galaxy/admin/invocation.py
+-rw-r--r--   0        0        0      315 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/tag.py
+-rw-r--r--   0        0        0     1360 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/admin/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:03:49.926001 django_to_galaxy-0.6.7/django_to_galaxy/api/__init__.py
+-rw-r--r--   0        0        0     1079 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py
+-rw-r--r--   0        0        0      257 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/galaxy_instance.py
+-rw-r--r--   0        0        0      428 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/galaxy_output_file.py
+-rw-r--r--   0        0        0      674 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/galaxy_user.py
+-rw-r--r--   0        0        0      387 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/history.py
+-rw-r--r--   0        0        0      396 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/invocation.py
+-rw-r--r--   0        0        0      657 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/invoke_workflow.py
+-rw-r--r--   0        0        0      883 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/upload_to_history.py
+-rw-r--r--   0        0        0      981 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/workflow.py
+-rw-r--r--   0        0        0     1661 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/urls.py
+-rw-r--r--   0        0        0      748 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/create_history.py
+-rw-r--r--   0        0        0      434 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/galaxy_instance.py
+-rw-r--r--   0        0        0      439 2023-11-03 10:15:22.426513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/galaxy_output_file.py
+-rw-r--r--   0        0        0      420 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/galaxy_user.py
+-rw-r--r--   0        0        0      394 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/history.py
+-rw-r--r--   0        0        0     1318 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/invocation.py
+-rw-r--r--   0        0        0     6530 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/invoke_workflow.py
+-rw-r--r--   0        0        0     2972 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/upload_to_history.py
+-rw-r--r--   0        0        0      401 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/api/views/workflow.py
+-rw-r--r--   0        0        0      143 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/apps.py
+-rw-r--r--   0        0        0     5954 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0001_new_initial.py
+-rw-r--r--   0        0        0      965 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py
+-rw-r--r--   0        0        0      515 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0003_invocation_create_time.py
+-rw-r--r--   0        0        0     1506 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py
+-rw-r--r--   0        0        0     1052 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py
+-rw-r--r--   0        0        0     1180 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py
+-rw-r--r--   0        0        0     2000 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py
+-rw-r--r--   0        0        0      481 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0008_workflowinput_label.py
+-rw-r--r--   0        0        0      500 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/migrations/0009_galaxyoutputfile_unique_galaxy_id_per_invocation.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:03:49.926001 django_to_galaxy-0.6.7/django_to_galaxy/migrations/__init__.py
+-rw-r--r--   0        0        0      370 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/__init__.py
+-rw-r--r--   0        0        0      889 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/accepted_input.py
+-rw-r--r--   0        0        0     1537 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_element.py
+-rw-r--r--   0        0        0      723 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_instance.py
+-rw-r--r--   0        0        0     1915 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_output_file.py
+-rw-r--r--   0        0        0     3264 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_user.py
+-rw-r--r--   0        0        0     2635 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/history.py
+-rw-r--r--   0        0        0     7620 2024-04-04 15:13:17.375293 django_to_galaxy-0.6.7/django_to_galaxy/models/invocation.py
+-rw-r--r--   0        0        0     1891 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/models/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:03:49.930001 django_to_galaxy-0.6.7/django_to_galaxy/schemas/__init__.py
+-rw-r--r--   0        0        0      396 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/schemas/dataset.py
+-rw-r--r--   0        0        0      138 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/settings.py
+-rw-r--r--   0        0        0     2389 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/templates/admin/import_workflows.html
+-rw-r--r--   0        0        0      106 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/urls.py
+-rw-r--r--   0        0        0     1625 2023-11-03 10:15:22.430513 django_to_galaxy-0.6.7/django_to_galaxy/utils.py
+-rw-r--r--   0        0        0      111 2023-11-03 10:45:30.098487 django_to_galaxy-0.6.7/django_to_galaxy/version.py
+-rw-r--r--   0        0        0      771 2024-04-05 14:03:01.362106 django_to_galaxy-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 django_to_galaxy-0.6.7/PKG-INFO
```

### Comparing `django_to_galaxy-0.6.5/LICENSE` & `django_to_galaxy-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_instance.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_instance.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_output_file.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_output_file.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/galaxy_user.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/history.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/invocation.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/invocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,30 @@
         "history",
         "create_time",
     )
     actions = ["synchronize_invocation", "update_output_files"]
 
     @admin.display(description="Percentage Done")
     def display_percentage_done(self, obj):
-        return format_html(
-            """
-            <progress value="{0}" max="100"></progress>
-            <span style="font-weight:bold">{0}%</span>
-            """,
-            obj.percentage_done,
-        )
+        try:
+            return format_html(
+                """
+                <progress value="{0}" max="100"></progress>
+                <span style="font-weight:bold">{0}%</span>
+                """,
+                obj.percentage_done,
+            )
+        except ZeroDivisionError:
+            return format_html(
+                """
+                <progress value="{0}" max="100"></progress>
+                <span style="font-weight:bold">{0}%</span>
+                """,
+                0,
+            )
 
     def _get_message_invocation(
         self,
         request,
         invocations: List[Invocation],
         message_singular: str,
         message_plural: str,
```

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/admin/workflow.py` & `django_to_galaxy-0.6.7/django_to_galaxy/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/galaxy_user.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/invoke_workflow.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/invoke_workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/upload_to_history.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/upload_to_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/serializers/workflow.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/serializers/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/urls.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/urls.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/views/create_history.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/views/create_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/views/invocation.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/views/invocation.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/views/invoke_workflow.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/views/invoke_workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/api/views/upload_to_history.py` & `django_to_galaxy-0.6.7/django_to_galaxy/api/views/upload_to_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0001_new_initial.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0001_new_initial.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0003_invocation_create_time.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0003_invocation_create_time.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py` & `django_to_galaxy-0.6.7/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/accepted_input.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/accepted_input.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_element.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_element.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_instance.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_instance.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_output_file.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_output_file.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/galaxy_user.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/history.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/invocation.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/invocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,25 +55,43 @@
             self._galaxy_invocation = self._get_galaxy_invocation()
         return self._galaxy_invocation
 
     def _get_galaxy_invocation(self) -> wrappers.Invocation:
         """Get galaxy object using bioblend."""
         return self.workflow.galaxy_owner.obj_gi.invocations.get(self.galaxy_id)
 
+    def complet_jobs_summary(self, step):
+        subinv = self.galaxy_invocation.gi.invocations.get(
+            step.wrapped["subworkflow_invocation_id"]
+        )
+        sub_jobs_summary = subinv.step_jobs_summary()
+        for job in sub_jobs_summary:
+            self.step_jobs_summary.append(job)
+        for sub in subinv.steps:
+            if "subworkflow_invocation_id" in sub.wrapped:
+                if sub.wrapped["subworkflow_invocation_id"]:
+                    self.complet_jobs_summary(sub)
+
     @property
     def percentage_done(self) -> float:
         """Retrieve percentage of jobs done for the invocation."""
         if self.status == DONE:
             return 100.0
-        step_jobs_summary = self.galaxy_invocation.step_jobs_summary()
+        self.step_jobs_summary = self.galaxy_invocation.step_jobs_summary()
+
+        for step in self.galaxy_invocation.steps:
+            if "subworkflow_invocation_id" in step.wrapped:
+                if step.wrapped["subworkflow_invocation_id"]:
+                    self.complet_jobs_summary(step)
+
         count_states = defaultdict(int)
-        for step in step_jobs_summary:
+        for step in self.step_jobs_summary:
             for key in step["states"].keys():
                 count_states[key] += 1
-        percentage_done = count_states.get("ok", 0) / len(step_jobs_summary)
+        percentage_done = count_states.get("ok", 0) / len(self.step_jobs_summary)
         if percentage_done == 1:
             self.status = DONE
             self.save()
         if "error" in count_states.keys():
             self.status = ERROR
             self.save()
         elif "paused" in count_states.keys():
```

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/models/workflow.py` & `django_to_galaxy-0.6.7/django_to_galaxy/models/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/templates/admin/import_workflows.html` & `django_to_galaxy-0.6.7/django_to_galaxy/templates/admin/import_workflows.html`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/django_to_galaxy/utils.py` & `django_to_galaxy-0.6.7/django_to_galaxy/utils.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.5/pyproject.toml` & `django_to_galaxy-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-to-galaxy"
-version = "0.6.5"
+version = "0.6.7"
 description = "Django extension that eases communication with Galaxy instance to execute workflows."
 authors = ["Kenzo-Hugo Hillion <hillion.kenzo@posteo.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Django = "^4.0.3"
 bioblend = "^0.16.0"
```

### Comparing `django_to_galaxy-0.6.5/PKG-INFO` & `django_to_galaxy-0.6.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-to-galaxy
-Version: 0.6.5
+Version: 0.6.7
 Summary: Django extension that eases communication with Galaxy instance to execute workflows.
 Author: Kenzo-Hugo Hillion
 Author-email: hillion.kenzo@posteo.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=4.0.3,<5.0.0)
 Requires-Dist: Markdown (>=3.3.6,<4.0.0)
 Requires-Dist: bioblend (>=0.16.0,<0.17.0)
 Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: requests-cache (>=0.9.5,<0.10.0)
```

