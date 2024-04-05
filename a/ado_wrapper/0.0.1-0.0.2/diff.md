# Comparing `tmp/ado_wrapper-0.0.1.tar.gz` & `tmp/ado_wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.1.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.2.tar", max compression
```

## Comparing `ado_wrapper-0.0.1.tar` & `ado_wrapper-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.1/LICENSE
--rw-r--r--   0        0        0      514 2024-04-05 11:26:35.758555 ado_wrapper-0.0.1/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.1/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     5594 2024-04-05 11:27:30.944640 ado_wrapper-0.0.1/ado_wrapper/__main__.py
--rw-r--r--   0        0        0      757 2024-03-18 13:18:23.074326 ado_wrapper-0.0.1/ado_wrapper/attribute_types.py
--rw-r--r--   0        0        0     1789 2024-04-05 11:26:50.366793 ado_wrapper-0.0.1/ado_wrapper/client.py
--rw-r--r--   0        0        0    16521 2024-04-05 11:26:35.608888 ado_wrapper-0.0.1/ado_wrapper/dumps.py
--rw-r--r--   0        0        0      933 2024-04-05 11:26:35.608861 ado_wrapper-0.0.1/ado_wrapper/generate_type_hints.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.1/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.1/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     3156 2024-04-05 11:26:35.653410 ado_wrapper-0.0.1/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1173 2024-04-05 11:26:35.675487 ado_wrapper-0.0.1/ado_wrapper/plan_resources/singletons.py
--rw-r--r--   0        0        0      592 2024-04-05 11:26:35.608910 ado_wrapper-0.0.1/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-05 11:26:35.611010 ado_wrapper-0.0.1/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14212 2024-04-05 11:26:35.608898 ado_wrapper-0.0.1/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6680 2024-04-05 11:26:35.611906 ado_wrapper-0.0.1/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3582 2024-04-05 11:26:35.622227 ado_wrapper-0.0.1/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2226 2024-04-05 11:26:35.611094 ado_wrapper-0.0.1/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    10175 2024-04-05 11:26:35.611081 ado_wrapper-0.0.1/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12933 2024-04-05 11:26:35.608871 ado_wrapper-0.0.1/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0     9376 2024-04-05 11:26:35.611060 ado_wrapper-0.0.1/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5099 2024-04-05 11:26:35.621976 ado_wrapper-0.0.1/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8223 2024-04-05 11:26:35.611032 ado_wrapper-0.0.1/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     5384 2024-04-05 11:26:35.622212 ado_wrapper-0.0.1/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     6204 2024-04-05 11:26:50.367079 ado_wrapper-0.0.1/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     7865 2024-04-05 11:26:50.367066 ado_wrapper-0.0.1/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     3919 2024-04-05 11:26:35.608850 ado_wrapper-0.0.1/ado_wrapper/utils.py
--rw-r--r--   0        0        0     1947 2024-04-05 11:26:35.607735 ado_wrapper-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 ado_wrapper-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.2/LICENSE
+-rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.2/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.2/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6471 2024-04-05 14:34:46.569797 ado_wrapper-0.0.2/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0      757 2024-03-18 13:18:23.074326 ado_wrapper-0.0.2/ado_wrapper/attribute_types.py
+-rw-r--r--   0        0        0     1789 2024-04-05 11:26:50.366793 ado_wrapper-0.0.2/ado_wrapper/client.py
+-rw-r--r--   0        0        0    16521 2024-04-05 11:26:35.608888 ado_wrapper-0.0.2/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0      933 2024-04-05 11:26:35.608861 ado_wrapper-0.0.2/ado_wrapper/generate_type_hints.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.2/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.2/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     3160 2024-04-05 14:34:38.388460 ado_wrapper-0.0.2/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1173 2024-04-05 11:26:35.675487 ado_wrapper-0.0.2/ado_wrapper/plan_resources/singletons.py
+-rw-r--r--   0        0        0      592 2024-04-05 11:26:35.608910 ado_wrapper-0.0.2/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-05 11:26:35.611010 ado_wrapper-0.0.2/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14211 2024-04-05 14:34:16.697054 ado_wrapper-0.0.2/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6680 2024-04-05 11:26:35.611906 ado_wrapper-0.0.2/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3582 2024-04-05 11:26:35.622227 ado_wrapper-0.0.2/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0     2226 2024-04-05 11:26:35.611094 ado_wrapper-0.0.2/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    10175 2024-04-05 11:26:35.611081 ado_wrapper-0.0.2/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12933 2024-04-05 11:26:35.608871 ado_wrapper-0.0.2/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0     9376 2024-04-05 11:26:35.611060 ado_wrapper-0.0.2/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5133 2024-04-05 14:34:26.887910 ado_wrapper-0.0.2/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8223 2024-04-05 11:26:35.611032 ado_wrapper-0.0.2/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     5384 2024-04-05 11:26:35.622212 ado_wrapper-0.0.2/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     6204 2024-04-05 11:26:50.367079 ado_wrapper-0.0.2/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8367 2024-04-05 14:40:18.511801 ado_wrapper-0.0.2/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     3919 2024-04-05 11:26:35.608850 ado_wrapper-0.0.2/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     1947 2024-04-05 14:41:44.987378 ado_wrapper-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.2/PKG-INFO
```

### Comparing `ado_wrapper-0.0.1/LICENSE` & `ado_wrapper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/README.md` & `ado_wrapper-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# ado_wrapper
+# Ado Wrapper
 
 This is a Python Package which works as an interface to the Azure DevOps API
 
-It is essentially a wrapper for the horrible to work with ADO API, and supports OOP principals.
+It is essentially a wrapper for the (horrible to work with) ADO API, and supports OOP principals.
 
 Any resource can be fetched by calling the `<resource>.get_by_id()` function.
 
 It also includes a solution for managing resources created by this script, which is extremely useful for testing the creation of random resources.
 To delete all resources created by this, run the main module with the "--delete-everything" flag.
```

### Comparing `ado_wrapper-0.0.1/ado_wrapper/attribute_types.py` & `ado_wrapper-0.0.2/ado_wrapper/attribute_types.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/client.py` & `ado_wrapper-0.0.2/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/dumps.py` & `ado_wrapper-0.0.2/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/generate_type_hints.py` & `ado_wrapper-0.0.2/ado_wrapper/generate_type_hints.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.2/ado_wrapper/plan_resources/plan_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Any
-import re
-from datetime import datetime
+# import re
+# from datetime import datetime
 from ado_wrapper.client import AdoClient
 from ado_wrapper.resources.repo import Repo
 
 import requests
 
 # class UnknownUntilApply(str):
 #     def __str__(self) -> str:
```

### Comparing `ado_wrapper-0.0.1/ado_wrapper/plan_resources/singletons.py` & `ado_wrapper-0.0.2/ado_wrapper/plan_resources/singletons.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/builds.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
         description: str, agent_pool_id: str, variable_groups: list[str], branch_name: str = "main",  # fmt: skip
     ) -> "BuildDefinition":
         return super().create(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
-            payload=get_build_definition(name, repo_id, repo_name, path_to_pipeline, description, ado_client.ado_project, 
+            payload=get_build_definition(name, repo_id, repo_name, path_to_pipeline, description, ado_client.ado_project,
                                          agent_pool_id, branch_name)  # fmt: skip
         )  # type: ignore[return-value]
         #  | {"variableGroups": [{"id": x for x in variable_groups}]},
 
     def update(self, ado_client: AdoClient, attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         if self.build_repo is None or self.process is None:
             raise ValueError("This build definition does not have a (repository or process) in its data, it cannot be updated")
```

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,24 +98,24 @@
     # def get_all_teams_recursively(cls, ado_client: AdoClient) -> list["TeamMember | Team"]:
     #     all_teams = [
     #         cls._recursively_extract_teams(ado_client, team)
     #         for team in cls.get_all(ado_client)
     #     ]
     #     return all_teams  # type: ignore[return-value]
 
-    """
-    The output should be as follows:
-    [
-        Team 1 = [
-            TeamMember 1,
-            TeamMember 2,
-            TeamMember 3
-        ],
-        Team 2 = [
-            TeamMember 4,
-            Team 3 = [
-                TeamMember 5,
-                TeamMember 6
-            ]
-        ],
-    ]
-    """
+    # """
+    # The output should be as follows:
+    # [
+    #     Team 1 = [
+    #         TeamMember 1,
+    #         TeamMember 2,
+    #         TeamMember 3
+    #     ],
+    #     Team 2 = [
+    #         TeamMember 4,
+    #         Team 3 = [
+    #             TeamMember 5,
+    #             TeamMember 6
+    #         ]
+    #     ],
+    # ]
+    # """
```

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.2/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.2/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.2/ado_wrapper/state_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
 from pathlib import Path
+from datetime import datetime
+from uuid import uuid4
 from typing import Any, TypedDict, TYPE_CHECKING  # , Generator
 
 from ado_wrapper.attribute_types import ResourceType
 from ado_wrapper.utils import DeletionFailed, get_resource_variables
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
-STATE_FILE_VERSION = "1.3"
+STATE_FILE_VERSION = "1.4"
 
 
 class StateFileType(TypedDict):
     state_file_version: str
     resources: dict[ResourceType, dict[str, Any]]
 
 
 class StateManager:
     def __init__(self, ado_client: "AdoClient", state_file_name: str | None = "main.state") -> None:
         self.ado_client = ado_client
         self.state_file_name = state_file_name
+        self.run_id = str(uuid4())
 
         # If they have a state file name input, but the file doesn't exist:
         if self.state_file_name is not None and not Path(self.state_file_name).exists():
             self.wipe_state()  # Will automatically create the file
 
     def load_state(self) -> StateFileType:
         assert self.state_file_name is not None
@@ -43,15 +46,17 @@
     def add_resource_to_state(self, resource_type: ResourceType, resource_id: str, resource_data: dict[str, Any]) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not adding resource to state")
             return None
         all_states = self.load_state()
         if resource_id in all_states["resources"][resource_type]:
             self.remove_resource_from_state(resource_type, resource_id)
-        all_states["resources"][resource_type] |= {resource_id: {"data": resource_data}}
+        metadata = {"created_datetime": datetime.now().isoformat(), "run_id": self.run_id}
+        all_data = metadata | {resource_id: {"data": resource_data}}
+        all_states["resources"][resource_type] |= all_data
         return self.write_state_file(all_states)
 
     def remove_resource_from_state(self, resource_type: ResourceType, resource_id: str) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not removing resource to state")
             return None
         all_states = self.load_state()
@@ -60,14 +65,17 @@
 
     def update_resource_in_state(self, resource_type: ResourceType, resource_id: str, updated_data: dict[str, Any]) -> None:
         if self.state_file_name is None:
             print("[ADO_WRAPPER] Not storing state, so not updating resource in state")
             return None
         all_states = self.load_state()
         all_states["resources"][resource_type][resource_id]["data"] = updated_data
+        if "metadata" not in all_states["resources"][resource_type][resource_id]:
+            all_states["resources"][resource_type][resource_id]["metadata"] = {}
+        all_states["resources"][resource_type][resource_id]["metadata"]["updated_datetime"] = datetime.now().isoformat()
         return self.write_state_file(all_states)
 
     # =======================================================================================================
 
     def delete_resource(self, resource_type: ResourceType, resource_id: str) -> None:
         all_resource_classes = get_resource_variables()
         class_reference = all_resource_classes[resource_type]
```

### Comparing `ado_wrapper-0.0.1/ado_wrapper/utils.py` & `ado_wrapper-0.0.2/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.1/pyproject.toml` & `ado_wrapper-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.1"
+version = "0.0.2"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-0.0.1/PKG-INFO` & `ado_wrapper-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (==2.31.0)
 Description-Content-Type: text/markdown
 
-# ado_wrapper
+# Ado Wrapper
 
 This is a Python Package which works as an interface to the Azure DevOps API
 
-It is essentially a wrapper for the horrible to work with ADO API, and supports OOP principals.
+It is essentially a wrapper for the (horrible to work with) ADO API, and supports OOP principals.
 
 Any resource can be fetched by calling the `<resource>.get_by_id()` function.
 
 It also includes a solution for managing resources created by this script, which is extremely useful for testing the creation of random resources.
 To delete all resources created by this, run the main module with the "--delete-everything" flag.
```

