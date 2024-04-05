# Comparing `tmp/ado_wrapper-0.0.2.tar.gz` & `tmp/ado_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.2.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.3.tar", max compression
```

## Comparing `ado_wrapper-0.0.2.tar` & `ado_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.2/LICENSE
--rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.2/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.2/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-05 14:34:46.569797 ado_wrapper-0.0.2/ado_wrapper/__main__.py
--rw-r--r--   0        0        0      757 2024-03-18 13:18:23.074326 ado_wrapper-0.0.2/ado_wrapper/attribute_types.py
--rw-r--r--   0        0        0     1789 2024-04-05 11:26:50.366793 ado_wrapper-0.0.2/ado_wrapper/client.py
--rw-r--r--   0        0        0    16521 2024-04-05 11:26:35.608888 ado_wrapper-0.0.2/ado_wrapper/dumps.py
--rw-r--r--   0        0        0      933 2024-04-05 11:26:35.608861 ado_wrapper-0.0.2/ado_wrapper/generate_type_hints.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.2/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.2/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     3160 2024-04-05 14:34:38.388460 ado_wrapper-0.0.2/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1173 2024-04-05 11:26:35.675487 ado_wrapper-0.0.2/ado_wrapper/plan_resources/singletons.py
--rw-r--r--   0        0        0      592 2024-04-05 11:26:35.608910 ado_wrapper-0.0.2/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-05 11:26:35.611010 ado_wrapper-0.0.2/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14211 2024-04-05 14:34:16.697054 ado_wrapper-0.0.2/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6680 2024-04-05 11:26:35.611906 ado_wrapper-0.0.2/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3582 2024-04-05 11:26:35.622227 ado_wrapper-0.0.2/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2226 2024-04-05 11:26:35.611094 ado_wrapper-0.0.2/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    10175 2024-04-05 11:26:35.611081 ado_wrapper-0.0.2/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12933 2024-04-05 11:26:35.608871 ado_wrapper-0.0.2/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0     9376 2024-04-05 11:26:35.611060 ado_wrapper-0.0.2/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5133 2024-04-05 14:34:26.887910 ado_wrapper-0.0.2/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8223 2024-04-05 11:26:35.611032 ado_wrapper-0.0.2/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     5384 2024-04-05 11:26:35.622212 ado_wrapper-0.0.2/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     6204 2024-04-05 11:26:50.367079 ado_wrapper-0.0.2/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8367 2024-04-05 14:40:18.511801 ado_wrapper-0.0.2/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     3919 2024-04-05 11:26:35.608850 ado_wrapper-0.0.2/ado_wrapper/utils.py
--rw-r--r--   0        0        0     1947 2024-04-05 14:41:44.987378 ado_wrapper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.3/LICENSE
+-rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.3/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.3/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6471 2024-04-05 14:34:46.569797 ado_wrapper-0.0.3/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0      757 2024-03-18 13:18:23.074326 ado_wrapper-0.0.3/ado_wrapper/attribute_types.py
+-rw-r--r--   0        0        0     1789 2024-04-05 11:26:50.366793 ado_wrapper-0.0.3/ado_wrapper/client.py
+-rw-r--r--   0        0        0    16521 2024-04-05 11:26:35.608888 ado_wrapper-0.0.3/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0      933 2024-04-05 11:26:35.608861 ado_wrapper-0.0.3/ado_wrapper/generate_type_hints.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.3/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.3/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     2999 2024-04-05 15:06:59.436804 ado_wrapper-0.0.3/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1173 2024-04-05 15:06:51.254984 ado_wrapper-0.0.3/ado_wrapper/plan_resources/singletons.py
+-rw-r--r--   0        0        0      592 2024-04-05 11:26:35.608910 ado_wrapper-0.0.3/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-05 11:26:35.611010 ado_wrapper-0.0.3/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14311 2024-04-05 15:08:13.711235 ado_wrapper-0.0.3/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6680 2024-04-05 11:26:35.611906 ado_wrapper-0.0.3/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3582 2024-04-05 11:26:35.622227 ado_wrapper-0.0.3/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0     2226 2024-04-05 11:26:35.611094 ado_wrapper-0.0.3/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    10175 2024-04-05 11:26:35.611081 ado_wrapper-0.0.3/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12933 2024-04-05 11:26:35.608871 ado_wrapper-0.0.3/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0     9370 2024-04-05 15:06:28.103613 ado_wrapper-0.0.3/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5133 2024-04-05 14:34:26.887910 ado_wrapper-0.0.3/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8223 2024-04-05 11:26:35.611032 ado_wrapper-0.0.3/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     5384 2024-04-05 11:26:35.622212 ado_wrapper-0.0.3/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     6204 2024-04-05 14:46:36.791614 ado_wrapper-0.0.3/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8239 2024-04-05 14:54:03.323466 ado_wrapper-0.0.3/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     3919 2024-04-05 11:26:35.608850 ado_wrapper-0.0.3/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     1997 2024-04-05 15:08:55.949910 ado_wrapper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.3/PKG-INFO
```

### Comparing `ado_wrapper-0.0.2/LICENSE` & `ado_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/README.md` & `ado_wrapper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/__main__.py` & `ado_wrapper-0.0.3/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/attribute_types.py` & `ado_wrapper-0.0.3/ado_wrapper/attribute_types.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/client.py` & `ado_wrapper-0.0.3/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/dumps.py` & `ado_wrapper-0.0.3/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/generate_type_hints.py` & `ado_wrapper-0.0.3/ado_wrapper/generate_type_hints.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.3/ado_wrapper/plan_resources/plan_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from typing import Callable, Any
 # import re
+import requests
 # from datetime import datetime
+
 from ado_wrapper.client import AdoClient
 from ado_wrapper.resources.repo import Repo
 
-import requests
-
-# class UnknownUntilApply(str):
-#     def __str__(self) -> str:
-#         return "Unknown until apply"
-# UnknownUntilApply = UnknownUntilApply()  # type: ignore
 UNKNOWN_UNTIL_APPLY = "Unknown until apply"
 
 
 class FakeResponse(requests.Response):
     def __init__(self, _json: dict[str, Any], status_code: int) -> None:
         super().__init__()
         self._json = _json
```

### Comparing `ado_wrapper-0.0.2/ado_wrapper/plan_resources/singletons.py` & `ado_wrapper-0.0.3/ado_wrapper/plan_resources/singletons.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable
 
+import requests
+
 from ado_wrapper.client import AdoClient
 from ado_wrapper.plan_resources.mapping import get_resource_variables_plans
 
-import requests
-
 mapping = get_resource_variables_plans()
 
 # A decorator that will wrap a Resource.get_by_id method and override the requests.get method temporarily
 # to return a custom Fake response
 
 
 def plannable_resource(func: Callable[[Any, AdoClient], Any]) -> Callable[[Any], Any]:  # fmt: skip
```

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/builds.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,17 @@
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_all_by_definition(cls, ado_client: AdoClient, definition_id: str) -> "list[Build]":
-        response = requests.get(
+        return super().get_all(ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds?api-version=7.1&definitions={definition_id}",
-            auth=ado_client.auth,
-        ).json()["value"]
-        return [cls.from_request_payload(build) for build in response]
+        )  # type: ignore[return-value]
 
     def delete(self, ado_client: AdoClient) -> None:
         return self.delete_by_id(ado_client, self.build_id)
 
     @classmethod
     def create_and_wait_until_completion(cls, ado_client: AdoClient, definition_id: str, branch_name: str = "main",
                                          max_timeout_seconds: int = 300) -> "Build":  # fmt: skip
@@ -141,18 +139,22 @@
             if (datetime.now() - start_time).seconds > max_timeout_seconds:
                 raise TimeoutError(f"The build did not complete within {max_timeout_seconds} seconds ({max_timeout_seconds//60} minutes)")
             time.sleep(3)
         return build
 
     @staticmethod
     def delete_all_leases(ado_client: AdoClient, build_id: str) -> None:
-        leases = requests.get(
+        leases_request = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}/leases?api-version=7.1-preview.1",
             auth=ado_client.auth,
-        ).json()["value"]
+        )
+        if leases_request.status_code != 200:
+            print(f"Could not delete leases, {leases_request.status_code}")
+            return
+        leases = leases_request.json()["value"]
         for lease in leases:
             lease_response = requests.delete(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/retention/leases?ids={lease['leaseId']}&api-version=6.1",
                 auth=ado_client.auth,
             )
             assert lease_response.status_code <= 204
```

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         if request.status_code == 404:
             raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
         if request.status_code != 200:
             raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
         return request.text  # This is the file content
 
     def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
-        """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP"""
-        """This function downloads the contents of a repo, and returns a dictionary of the files and their contents
+        """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
+        This function downloads the contents of a repo, and returns a dictionary of the files and their contents
         The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
         try:
             request = requests.get(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
                 auth=ado_client.auth,
             )
         except requests.exceptions.ConnectionError:
```

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.3/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.3/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.3/ado_wrapper/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not adding resource to state")
             return None
         all_states = self.load_state()
         if resource_id in all_states["resources"][resource_type]:
             self.remove_resource_from_state(resource_type, resource_id)
         metadata = {"created_datetime": datetime.now().isoformat(), "run_id": self.run_id}
-        all_data = metadata | {resource_id: {"data": resource_data}}
+        all_data = {resource_id: {"data": resource_data, "metadata": metadata, "lifecycle-status": {}}}
         all_states["resources"][resource_type] |= all_data
         return self.write_state_file(all_states)
 
     def remove_resource_from_state(self, resource_type: ResourceType, resource_id: str) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not removing resource to state")
             return None
@@ -65,16 +65,14 @@
 
     def update_resource_in_state(self, resource_type: ResourceType, resource_id: str, updated_data: dict[str, Any]) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not updating resource in state")
             return None
         all_states = self.load_state()
         all_states["resources"][resource_type][resource_id]["data"] = updated_data
-        if "metadata" not in all_states["resources"][resource_type][resource_id]:
-            all_states["resources"][resource_type][resource_id]["metadata"] = {}
         all_states["resources"][resource_type][resource_id]["metadata"]["updated_datetime"] = datetime.now().isoformat()
         return self.write_state_file(all_states)
 
     # =======================================================================================================
 
     def delete_resource(self, resource_type: ResourceType, resource_id: str) -> None:
         all_resource_classes = get_resource_variables()
```

### Comparing `ado_wrapper-0.0.2/ado_wrapper/utils.py` & `ado_wrapper-0.0.3/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.2/pyproject.toml` & `ado_wrapper-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.2"
+version = "0.0.3"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -43,15 +43,17 @@
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "missing-timeout",
 
     "too-few-public-methods",
     "too-many-instance-attributes",
+    "too-many-arguments",
 
+    "arguments-differ",
     "arguments-renamed",
     "invalid-name",
     "too-many-locals",
     "line-too-long",
     "broad-exception-caught",
     "import-outside-toplevel",
     "attribute-defined-outside-init",
```

### Comparing `ado_wrapper-0.0.2/PKG-INFO` & `ado_wrapper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

