# Comparing `tmp/gidgetlab_kit-0.7.1.tar.gz` & `tmp/gidgetlab_kit-0.7.2.tar.gz`

## Comparing `gidgetlab_kit-0.7.1.tar` & `gidgetlab_kit-0.7.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/.flake8
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/MANIFEST.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/__init__.py
--rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/api.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/clone.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/command.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/commits.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/exceptions.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/get.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/models.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/pipelines.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/producers.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/tasks.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/gidgetlab_kit/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_api.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_clone.py
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_command.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_commits.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_models.py
--rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_pipelines.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/test_util.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/utils.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/groups_id.json
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/groups_id_subgroup.json
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/project_from_pipeline_event.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/project_from_tag_push_event.json
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/project_null_description.json
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/project_tags.json
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/projects_empty.json
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/projects_id_auth.json
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/projects_id_no_auth.json
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/projects_id_subgroup.json
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/tests/samples/subgroup.json
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/LICENSE
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/MANIFEST.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/__init__.py
+-rw-r--r--   0        0        0    15239 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/api.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/clone.py
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/command.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/commits.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/exceptions.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/get.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/models.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/pipelines.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/producers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/tasks.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/gidgetlab_kit/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_api.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_clone.py
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_command.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_commits.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_models.py
+-rw-r--r--   0        0        0    11382 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_pipelines.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/test_util.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/utils.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/groups_id.json
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/groups_id_subgroup.json
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/project_from_pipeline_event.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/project_from_tag_push_event.json
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/project_null_description.json
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/project_tags.json
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/projects_empty.json
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/projects_id_auth.json
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/projects_id_no_auth.json
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/projects_id_subgroup.json
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/tests/samples/subgroup.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 gidgetlab_kit-0.7.2/PKG-INFO
```

### Comparing `gidgetlab_kit-0.7.1/.gitlab-ci.yml` & `gidgetlab_kit-0.7.2/.gitlab-ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ---
 variables:
   TWINE_USERNAME: __token__
   TWINE_PASSWORD: secret
 
 default:
-  image: python:3.8
+  image: python:3.11
 
 stages:
   - check
   - build
   - test
   - release
 
 run-pre-commit:
   stage: check
+  image: python:3.9
   before_script:
     - pip install pre-commit
   script:
     - pre-commit run --all-files
 
 build-pypi-package:
   stage: build
@@ -35,15 +36,15 @@
   image: python:$PYTHON_VERSION
   before_script:
     - pip install .[tests]
   script:
     - pytest -v --junitxml=report.xml --cov=gidgetlab_kit tests
   parallel:
     matrix:
-      - PYTHON_VERSION: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+      - PYTHON_VERSION: ["3.9", "3.10", "3.11", "3.12"]
   artifacts:
     when: always
     reports:
       junit: report.xml
 
 release-pypi-package:
   stage: release
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/api.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import base64
 import http
 import urllib.parse
 import logging
-from typing import Optional, Any, AsyncIterator, List, Dict
+from typing import Optional, Any, AsyncIterator, Union
 from gidgetlab import GitLabException, HTTPException
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 from .models import Project, Group, GitLabId, Tag, TreeObject
 from .exceptions import PipelineFailure
 from .util import divide_chunks
 
 
 logger = logging.getLogger(__name__)
 
@@ -205,16 +205,16 @@
 
 async def list_repository_tree(
     gl: GitLabAPI,
     project_id: GitLabId,
     ref: str,
     recursive: bool = True,
     path: Optional[str] = None,
-) -> List[TreeObject]:
-    params = {"ref": ref, "recursive": recursive}
+) -> list[TreeObject]:
+    params: dict[str, Union[str, bool]] = {"ref": ref, "recursive": recursive}
     if path:
         params["path"] = path
     return [
         TreeObject(**repo_file)
         async for repo_file in gl.getiter(
             f"/projects/{project_id}/repository/tree",
             params=params,
@@ -304,15 +304,15 @@
         else:
             logger.warning(
                 "wait_on_merge can only be set to True when merge_on_success is"
             )
 
 
 async def get_projects(
-    gl: GitLabAPI, project_ids: List[GitLabId]
+    gl: GitLabAPI, project_ids: list[GitLabId]
 ) -> AsyncIterator[Project]:
     """Return projects based on their id"""
     for project_id in project_ids:
         project = await gl.getitem(f"/projects/{encode_gitlab_id(project_id)}")
         yield Project(**project)
 
 
@@ -336,16 +336,16 @@
     async for subgroup in gl.getiter(f"/groups/{encode_gitlab_id(group_id)}/subgroups"):
         yield Group(**subgroup)
         async for sub in get_subgroups(gl, subgroup["id"]):
             yield sub
 
 
 async def find_projects(
-    gl: GitLabAPI, names: List[str], group_id: GitLabId
-) -> List[Project]:
+    gl: GitLabAPI, names: list[str], group_id: GitLabId
+) -> list[Project]:
     """Find the projects based on their name under `group_id`
 
     The group's subgroups are also searched
     Return the list of projects found
     """
     names_set = {name.lower() for name in names}
     all_projects = [project async for project in get_all_projects(gl, group_id)]
@@ -360,15 +360,15 @@
         f"/projects/{project_id}/triggers", data={"description": description}
     )
     return result["token"]
 
 
 async def get_project_triggers(
     gl: GitLabAPI, project_id: GitLabId
-) -> List[Dict[str, str]]:
+) -> list[dict[str, str]]:
     """Return the project triggers"""
     return [trigger async for trigger in gl.getiter(f"/projects/{project_id}/triggers")]
 
 
 async def get_or_create_project_trigger_token(
     gl: GitLabAPI, project_id: GitLabId, description: str
 ) -> str:
@@ -394,23 +394,23 @@
     await gl.post(
         f"/projects/{project_id}/trigger/pipeline",
         params={"token": token, "ref": git_ref},
         data={},
     )
 
 
-async def list_branches(gl: GitLabAPI, project_id: GitLabId) -> List[str]:
+async def list_branches(gl: GitLabAPI, project_id: GitLabId) -> list[str]:
     """Return the list of branches name"""
     return [
         branch["name"]
         async for branch in gl.getiter(f"/projects/{project_id}/repository/branches")
     ]
 
 
-async def list_tags(gl: GitLabAPI, project_id: GitLabId) -> List[Tag]:
+async def list_tags(gl: GitLabAPI, project_id: GitLabId) -> list[Tag]:
     """Return the list of tags sorted by updated field"""
     return [
         Tag(**data)
         async for data in gl.getiter(
             f"/projects/{project_id}/repository/tags",
             params={"order_by": "updated", "sort": "desc"},
         )
@@ -432,17 +432,17 @@
             if ref["type"] == "branch" and ref["name"] == branch:
                 return tag
     return None
 
 
 async def trigger_pipelines(
     gl: GitLabAPI,
-    projects: List[Project],
+    projects: list[Project],
     description: str,
-    git_refs: Optional[List[str]] = None,
+    git_refs: Optional[list[str]] = None,
     delay: float = 0,
     chunk: int = 1,
 ) -> None:
     """Trigger the pipeline for all projects
 
     If no git ref is given, the pipeline is triggered for the default branch only
     """
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/clone.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import asyncio
 import shutil
 import typer
-from typing import List
 from pathlib import Path
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 from .models import GitLabId, Project
 from .util import run_subprocess
 from . import producers
 
 
 async def run_clone(
     gl: GitLabAPI,
     group: GitLabId,
     path: Path,
     archived: bool = False,
     delete_extra_repos: bool = False,
     force: bool = False,
     nb_consumers: int = 5,
-) -> List[Project]:
+) -> list[Project]:
     """Start producer and consumers to clone all projects from group
 
     Return the list of projects
     """
     queue: asyncio.Queue[Project] = asyncio.Queue(maxsize=0)
     consumers = [
         asyncio.create_task(clone_projects(queue, path, force))
@@ -34,15 +33,15 @@
     await gl._client.aclose()
     if delete_extra_repos:
         loop = asyncio.get_event_loop()
         await loop.run_in_executor(None, delete_extra_repositories, projects, path)
     return projects
 
 
-def delete_extra_repositories(projects: List[Project], path: Path) -> List[Path]:
+def delete_extra_repositories(projects: list[Project], path: Path) -> list[Path]:
     """Delete local git repositories not part of the list of projects
 
     WARNING! All projects are expected to be part of the same base namespace
 
     Return the list of deleted path
     """
     if not projects:
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/command.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/command.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import asyncio
 import logging
 import typer
 import httpx
 from importlib.metadata import version, PackageNotFoundError  # type: ignore
 from pathlib import Path
-from typing import Optional, List
+from typing import Optional
+from typing_extensions import Annotated
 from gidgetlab.httpx import GitLabAPI
 from . import util, api
 from .models import GitLabId
 from .clone import run_clone
 from .get import run_get
 from .pipelines import run_trigger_group_pipelines, PipelineExecution
 from .commits import run_commit_file
 
 try:
     __version__ = version("gidgetlab-kit")
 except PackageNotFoundError:
     __version__ = "unknown"
 
 app = typer.Typer()
-state = {"gl": None}
+state = {}
 
 
 def version_callback(value: bool):
     if value:
         typer.echo(f"gidgetlab-kit version: {__version__}")
         raise typer.Exit()
 
@@ -36,144 +37,173 @@
             fg=typer.colors.GREEN,
         )
     await gl._client.aclose()
 
 
 @app.callback()
 def main(
-    version: Optional[bool] = typer.Option(
-        None,
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-        help="Show the current version and exit.",
-    ),
-    url: str = typer.Option("https://gitlab.com", envvar="GL_URL", help="GitLab URL"),
-    access_token: str = typer.Option(
-        "", envvar="GL_ACCESS_TOKEN", help="GitLab access token"
-    ),
-    verify: bool = typer.Option(
-        True, help="Verify SSL cerificate or disable verification"
-    ),
+    version: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--version",
+            callback=version_callback,
+            is_eager=True,
+            help="Show the current version and exit.",
+        ),
+    ] = None,
+    url: Annotated[
+        str, typer.Option(envvar="GL_URL", help="GitLab URL")
+    ] = "https://gitlab.com",
+    access_token: Annotated[
+        str, typer.Option(envvar="GL_ACCESS_TOKEN", help="GitLab access token")
+    ] = "",
+    verify: Annotated[
+        bool, typer.Option(help="Verify SSL cerificate or disable verification")
+    ] = True,
 ):
     logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
         level=logging.INFO,
     )
     client = httpx.AsyncClient(verify=verify)
     state["gl"] = GitLabAPI(client, "gidgetlab", url=url, access_token=access_token)
 
 
 @app.command()
 def clone(
-    group: str = typer.Argument(..., help="Name of the group to clone"),
-    path: Path = typer.Option(
-        Path("."),
-        "--path",
-        "-p",
-        exists=True,
-        resolve_path=True,
-        help="Path where to clone the group",
-    ),
-    archived: bool = typer.Option(False, help="Clone archived projects"),
-    delete_extra_repos: bool = typer.Option(
-        False, help="Delete extra local repositories"
-    ),
-    force: bool = typer.Option(
-        False,
-        help="Force repository update when it exists (git reset --hard origin/default_branch instead of rebase)",
-    ),
-    nb_consumers: int = typer.Option(
-        5,
-        "--nb-consumers",
-        "-n",
-        help="Number of consumers to start to clone in parallel",
-    ),
+    group: Annotated[str, typer.Argument(..., help="Name of the group to clone")],
+    path: Annotated[
+        Path,
+        typer.Option(
+            "--path",
+            "-p",
+            exists=True,
+            resolve_path=True,
+            help="Path where to clone the group",
+        ),
+    ] = Path("."),
+    archived: Annotated[bool, typer.Option(help="Clone archived projects")] = False,
+    delete_extra_repos: Annotated[
+        bool, typer.Option(help="Delete extra local repositories")
+    ] = False,
+    force: Annotated[
+        bool,
+        typer.Option(
+            help="Force repository update when it exists (git reset --hard origin/default_branch instead of rebase)",
+        ),
+    ] = False,
+    nb_consumers: Annotated[
+        int,
+        typer.Option(
+            "--nb-consumers",
+            "-n",
+            help="Number of consumers to start to clone in parallel",
+        ),
+    ] = 5,
 ):
     """Clone or pull all projects from group (including subgroups)
 
     Projects are cloned/updated in parallel
     """
     asyncio.run(
         run_clone(
             state["gl"], group, path, archived, delete_extra_repos, force, nb_consumers
         )
     )
 
 
 @app.command()
 def get(
-    endpoint: str = typer.Argument(..., help="Endpoint to get"),
-    parameters: List[str] = typer.Argument(
-        None, help="Optional key-value pairs to pass as json parameters"
-    ),
-    nb_items: int = typer.Option(
-        0,
-        "--nb-items",
-        "-n",
-        help="Number of items to retrieve. Only valid when a list is returned. Set to 0 to return all.",
-    ),
+    endpoint: Annotated[str, typer.Argument(help="Endpoint to get")],
+    parameters: Annotated[
+        Optional[list[str]],
+        typer.Argument(help="Optional key-value pairs to pass as json parameters"),
+    ] = None,
+    nb_items: Annotated[
+        int,
+        typer.Option(
+            "--nb-items",
+            "-n",
+            help="Number of items to retrieve. Only valid when a list is returned. Set to 0 to return all.",
+        ),
+    ] = 0,
 ):
     """Get one or several items from the given endpoint"""
+    if parameters is None:
+        parameters = []
     try:
         params = util.convert_params_to_dict(parameters)
     except ValueError:
         typer.echo(
             f"Invalid parameters: '{' '.join(parameters)}' should be a list of key-value pairs separated by '='."
         )
-        raise typer.Exit(code=1)
+        raise typer.Exit(code=1) from None
     asyncio.run(run_get(state["gl"], endpoint, params, nb_items))
 
 
 @app.command()
 def list_projects(
-    group: str = typer.Argument(..., help="Name of the group"),
-    archived: bool = typer.Option(False, help="List archived projects"),
+    group: Annotated[str, typer.Argument(help="Name of the group")],
+    archived: Annotated[bool, typer.Option(help="list archived projects")] = False,
 ):
-    """List all projects from group (including subgroups)"""
+    """list all projects from group (including subgroups)"""
     asyncio.run(run_list_projects(state["gl"], group, archived))
 
 
 @app.command()
 def trigger_pipelines(
-    group: str = typer.Argument(..., help="Name of the group"),
-    nb_projects: int = typer.Option(
-        0,
-        "--nb-projects",
-        "-n",
-        help="Number of projects to trigger. Set to 0 to trigger all projects from the group.",
-    ),
-    sort: PipelineExecution = typer.Option(
-        PipelineExecution.oldest,
-        help="How to sort the projects based on the latest pipeline execution date.",
-    ),
-    exclude: List[str] = typer.Option(
-        None,
-        help=(
-            "Project to exclude (path with basename). "
-            "This is to exclude very specific project(s). To use regex, use include instead."
-        ),
-    ),
-    include: Optional[str] = typer.Option(
-        None,
-        help="regex that should match the name of projects to include (using re.search).",
-    ),
-    description: str = typer.Option(
-        "gidgetlab",
-        help="Pipeline trigger description",
-    ),
-    delay: float = typer.Option(
-        0,
-        help="Delay to apply between pipeline triggering. No delay if set to 0.",
-    ),
-    chunk: int = typer.Option(
-        1,
-        min=1,
-        help="Number of projects to trigger without delay (list will be processed chunk by chunk if greater than 1).",
-    ),
+    group: Annotated[str, typer.Argument(help="Name of the group")],
+    nb_projects: Annotated[
+        int,
+        typer.Option(
+            "--nb-projects",
+            "-n",
+            help="Number of projects to trigger. Set to 0 to trigger all projects from the group.",
+        ),
+    ] = 0,
+    sort: Annotated[
+        PipelineExecution,
+        typer.Option(
+            help="How to sort the projects based on the latest pipeline execution date.",
+        ),
+    ] = PipelineExecution.oldest,
+    exclude: Annotated[
+        Optional[list[str]],
+        typer.Option(
+            help=(
+                "Project to exclude (path with basename). "
+                "This is to exclude very specific project(s). To use regex, use include instead."
+            ),
+        ),
+    ] = None,
+    include: Annotated[
+        Optional[str],
+        typer.Option(
+            help="regex that should match the name of projects to include (using re.search).",
+        ),
+    ] = None,
+    description: Annotated[
+        str,
+        typer.Option(
+            help="Pipeline trigger description",
+        ),
+    ] = "gidgetlab",
+    delay: Annotated[
+        float,
+        typer.Option(
+            help="Delay to apply between pipeline triggering. No delay if set to 0.",
+        ),
+    ] = 0,
+    chunk: Annotated[
+        int,
+        typer.Option(
+            min=1,
+            help="Number of projects to trigger without delay (list will be processed chunk by chunk if greater than 1).",
+        ),
+    ] = 1,
 ):
     """Trigger the pipeline for all or a subset of projects from group"""
     asyncio.run(
         run_trigger_group_pipelines(
             state["gl"],
             group,
             nb_projects,
@@ -185,37 +215,45 @@
             chunk=chunk,
         )
     )
 
 
 @app.command()
 def commit_file(
-    filepath: Path = typer.Argument(..., help="Local file to add or update"),
-    group: str = typer.Option(..., help="Name of the group"),
-    repo_path: Path = typer.Option(
-        Path("."),
-        "--repo-path",
-        "-p",
-        resolve_path=False,
-        help="Path of the file in the repository",
-    ),
-    message: str = typer.Option(
-        "",
-        "--message",
-        "-m",
-        show_default=False,
-        help="Commit message [default: Add/Update <filename>]",
-    ),
-    branch: str = typer.Option("master", "--branch", "-b", help="Branch to commit to"),
-    nb_consumers: int = typer.Option(
-        5,
-        "--nb-consumers",
-        "-n",
-        help="Number of consumers to start to update in parallel",
-    ),
+    filepath: Annotated[Path, typer.Argument(help="Local file to add or update")],
+    group: Annotated[str, typer.Option(help="Name of the group")],
+    repo_path: Annotated[
+        Path,
+        typer.Option(
+            "--repo-path",
+            "-p",
+            resolve_path=False,
+            help="Path of the file in the repository",
+        ),
+    ] = Path("."),
+    message: Annotated[
+        str,
+        typer.Option(
+            "--message",
+            "-m",
+            show_default=False,
+            help="Commit message [default: Add/Update <filename>]",
+        ),
+    ] = "",
+    branch: Annotated[
+        str, typer.Option("--branch", "-b", help="Branch to commit to")
+    ] = "master",
+    nb_consumers: Annotated[
+        int,
+        typer.Option(
+            "--nb-consumers",
+            "-n",
+            help="Number of consumers to start to update in parallel",
+        ),
+    ] = 5,
 ):
     """Add or update a file to a list of projects
 
     Example:
 
       The following will add the local .gitlab-ci.yml file to all projects under the my-group group
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/commits.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/commits.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import asyncio
 import logging
 import typer
-from typing import List
 from pathlib import Path
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 from .models import GitLabId, Project
 from . import api, producers
 
 logger = logging.getLogger(__name__)
 
 
 async def run_commit_file(
     gl: GitLabAPI,
     group: GitLabId,
     local_file_path: Path,
     repo_file_path: str,
     branch: str,
     commit_message: str,
     nb_consumers: int = 5,
-) -> List[Project]:
+) -> list[Project]:
     """Start producer and consumers to commit the file to all projects from group
 
     Return the list of projects
     """
     content = local_file_path.read_text()
     queue: asyncio.Queue[Project] = asyncio.Queue(maxsize=0)
     consumers = [
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/get.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pprint import pprint
-from typing import Dict
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 
 
-async def run_get(gl: GitLabAPI, endpoint: str, params: Dict, nb_items: int) -> None:
+async def run_get(gl: GitLabAPI, endpoint: str, params: dict, nb_items: int) -> None:
     """Get one or several items"""
     result = await gl.getitem(endpoint, params=params)
     if not isinstance(result, list):
         pprint(result, sort_dicts=False)
     else:
         if nb_items > 0 and len(result) >= nb_items:
             for counter, item in enumerate(result, start=1):
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/models.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/models.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/pipelines.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import random
 import re
 import typer
 from operator import itemgetter
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
 from dateutil.parser import parse
 from dateutil.tz import UTC
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 from gidgetlab import BadRequest
 from .models import GitLabId, Project
 from . import api
 
 
 class PipelineExecution(str, Enum):
     oldest = "oldest"
@@ -38,16 +38,16 @@
         latest_pipeline = pipelines[0]
     except IndexError:
         return datetime.datetime(datetime.MINYEAR, 1, 1, tzinfo=UTC)
     return parse(latest_pipeline["updated_at"])
 
 
 async def sort_projects_by_pipeline_date(
-    gl: GitLabAPI, projects: List[Project], reverse=False
-) -> List[Project]:
+    gl: GitLabAPI, projects: list[Project], reverse=False
+) -> list[Project]:
     """Return the projects sorted by latest pipeline execution date"""
     # Build a list of tuple with each project and the latest pipeline date
     project_pipelines = [
         (project, await get_project_latest_pipeline_date(gl, project.id))
         for project in projects
     ]
     sorted_project_pipelines = sorted(
@@ -58,28 +58,30 @@
 
 async def run_trigger_group_pipelines(
     gl: GitLabAPI,
     group: GitLabId,
     nb_projects: int,
     sort: PipelineExecution = PipelineExecution.oldest,
     description: str = "gidgetlab",
-    exclude: List[str] = [],
+    exclude: Optional[list[str]] = None,
     include: Optional[str] = None,
     delay: float = 0,
     chunk: int = 1,
 ) -> None:
     """Trigger the pipeline for the group projects
 
     When greater than 0, nb_projects allows to select a subset of the projects.
     By default, the projects selected are the ones with the oldest pipeline execution date.
     It can be set to "newest" or "random".
     Some projects can be excluded based on the path with namespace.
     You can also filter the projects based on the name using the include regex.
     """
     # Filter out empty project (default_branch is None) and excluded one
+    if exclude is None:
+        exclude = []
     projects = [
         project
         async for project in api.get_all_projects(gl, group)
         if project.default_branch is not None
         and project.path_with_namespace not in exclude
     ]
     if include is not None:
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/producers.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/producers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import asyncio
-from typing import List
-from gidgetlab.abc import GitLabAPI
+from gidgetlab.httpx import GitLabAPI
 from .models import GitLabId, Project
 from . import api
 
 
 async def produce_projects(
     gl: GitLabAPI, queue: asyncio.Queue, group_id: GitLabId, archived: bool
-) -> List[Project]:
+) -> list[Project]:
     """Send to the queue all projects from the group, including subgroups
 
     Return the full list of projects when done
     """
     projects = []
     async for project in api.get_all_projects(gl, group_id, archived):
         projects.append(project)
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/tasks.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import httpx
 import logging
-from typing import Optional, Callable, Awaitable, List, Any
+from typing import Optional, Callable, Awaitable, Any
 from gidgetlab.httpx import GitLabAPI
 from .models import Project, GitLabId
 from .api import get_projects, get_all_projects
 
 logger = logging.getLogger(__name__)
 
 
@@ -32,15 +32,15 @@
 async def run_on_projects(
     func: Callable[[GitLabAPI, Project, Any], Awaitable[Any]],
     *,
     url: str = "https://gitlab.com",
     requester: str = "gidgetlab-kit",
     access_token: Optional[str] = None,
     group: Optional[GitLabId],
-    project_ids: List[GitLabId],
+    project_ids: list[GitLabId],
     nb_consumers: int = 5,
     **kwargs,
 ):
     """Run func on projects from group or list of ids
 
     project_ids has priority over group.
     A number of consumers are started to run the function in parallel on different projects.
```

### Comparing `gidgetlab_kit-0.7.1/gidgetlab_kit/util.py` & `gidgetlab_kit-0.7.2/gidgetlab_kit/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict, List
 import asyncio
 import shlex
 import typer
 
 
 async def run_subprocess(cmd: str, cwd=None) -> str:
     """Run the command as subprocess"""
@@ -11,15 +10,15 @@
     process = await asyncio.create_subprocess_exec(
         *args, stdout=asyncio.subprocess.PIPE, cwd=cwd
     )
     stdout, stderr = await process.communicate()
     return stdout.decode().strip()
 
 
-def convert_params_to_dict(params: List[str]) -> Dict:
+def convert_params_to_dict(params: list[str]) -> dict:
     """Convert a list of key-value pairs to a dict"""
     d = {}
     for kv in params:
         if "=" not in kv:
             raise ValueError(f"Key value pair '{kv}' shall be separated by '='")
         key, _, value = kv.partition("=")
         d[key] = value
```

### Comparing `gidgetlab_kit-0.7.1/tests/test_api.py` & `gidgetlab_kit-0.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/test_clone.py` & `gidgetlab_kit-0.7.2/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/test_command.py` & `gidgetlab_kit-0.7.2/tests/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,27 @@
     [
         (
             ["trigger-pipelines", "group"],
             ["group", 0],
             {
                 "sort": PipelineExecution.oldest,
                 "description": "gidgetlab",
-                "exclude": [],
+                "exclude": None,
                 "include": None,
                 "delay": 0,
                 "chunk": 1,
             },
         ),
         (
             ["trigger-pipelines", "group", "-n", "5"],
             ["group", 5],
             {
                 "sort": PipelineExecution.oldest,
                 "description": "gidgetlab",
-                "exclude": [],
+                "exclude": None,
                 "include": None,
                 "delay": 0,
                 "chunk": 1,
             },
         ),
         (
             [
@@ -129,39 +129,39 @@
         ),
         (
             ["trigger-pipelines", "group", "--sort", "random"],
             ["group", 0],
             {
                 "sort": PipelineExecution.random,
                 "description": "gidgetlab",
-                "exclude": [],
+                "exclude": None,
                 "include": None,
                 "delay": 0,
                 "chunk": 1,
             },
         ),
         (
             ["trigger-pipelines", "group", "--delay", "3", "--chunk", "5"],
             ["group", 0],
             {
                 "sort": PipelineExecution.oldest,
                 "description": "gidgetlab",
-                "exclude": [],
+                "exclude": None,
                 "include": None,
                 "delay": 3.0,
                 "chunk": 5,
             },
         ),
         (
             ["trigger-pipelines", "group", "--description", "my-test"],
             ["group", 0],
             {
                 "sort": PipelineExecution.oldest,
                 "description": "my-test",
-                "exclude": [],
+                "exclude": None,
                 "include": None,
                 "delay": 0,
                 "chunk": 1,
             },
         ),
         (
             [
@@ -170,15 +170,15 @@
                 "--include",
                 "^dev-|^lib-",
             ],
             ["group", 0],
             {
                 "sort": PipelineExecution.oldest,
                 "description": "gidgetlab",
-                "exclude": [],
+                "exclude": None,
                 "include": "^dev-|^lib-",
                 "delay": 0,
                 "chunk": 1,
             },
         ),
     ],
 )
```

### Comparing `gidgetlab_kit-0.7.1/tests/test_commits.py` & `gidgetlab_kit-0.7.2/tests/test_commits.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/test_models.py` & `gidgetlab_kit-0.7.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/test_pipelines.py` & `gidgetlab_kit-0.7.2/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/test_util.py` & `gidgetlab_kit-0.7.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/utils.py` & `gidgetlab_kit-0.7.2/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for tests"""
+
 import json
 import urllib
 import pathlib
 
 SAMPLES_PATH = pathlib.Path(__file__).parent / "samples"
 
 
@@ -47,26 +48,30 @@
     async def getitem(self, url, params=None):
         self.getitem_calls += 1
         self._getitem_url.append(url)
         if params:
             self._getitem_url[-1] += f"?{urllib.parse.urlencode(params)}"
         return self._getitem_return[self.getitem_calls - 1]
 
-    async def getiter(self, url, params={}):
+    async def getiter(self, url, params=None):
+        if params is None:
+            params = {}
         self.params = params
         self.getiter_url.append(url)
         if self._getiter_return and isinstance(self._getiter_return[0], (list, tuple)):
             items = self._getiter_return[self.getiter_calls]
         else:
             items = self._getiter_return
         self.getiter_calls += 1
         for item in items:
             yield item
 
-    async def post(self, url, *, data, params={}):
+    async def post(self, url, *, data, params=None):
+        if params is None:
+            params = {}
         self.post_url.append(url)
         self.post_data.append(data)
         self.post_params.append(params)
         return self._post_return
 
     async def put(self, url, *, data):
         self.put_url.append(url)
```

### Comparing `gidgetlab_kit-0.7.1/tests/samples/groups_id.json` & `gidgetlab_kit-0.7.2/tests/samples/groups_id.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/groups_id_subgroup.json` & `gidgetlab_kit-0.7.2/tests/samples/groups_id_subgroup.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/project_from_tag_push_event.json` & `gidgetlab_kit-0.7.2/tests/samples/project_from_tag_push_event.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/project_null_description.json` & `gidgetlab_kit-0.7.2/tests/samples/project_null_description.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/project_tags.json` & `gidgetlab_kit-0.7.2/tests/samples/project_tags.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/projects_empty.json` & `gidgetlab_kit-0.7.2/tests/samples/projects_empty.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/projects_id_auth.json` & `gidgetlab_kit-0.7.2/tests/samples/projects_id_auth.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/projects_id_no_auth.json` & `gidgetlab_kit-0.7.2/tests/samples/projects_id_no_auth.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/projects_id_subgroup.json` & `gidgetlab_kit-0.7.2/tests/samples/projects_id_subgroup.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/tests/samples/subgroup.json` & `gidgetlab_kit-0.7.2/tests/samples/subgroup.json`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/LICENSE` & `gidgetlab_kit-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gidgetlab_kit-0.7.1/README.md` & `gidgetlab_kit-0.7.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   get                Get one or several items from the given endpoint
   list-projects      List all projects from group (including subgroups)
   trigger-pipelines  Trigger the pipeline for all or a subset of projects...
 ```
 
 ## Installation
 
-Only Python 3.8 and above is tested. Create a virtualenv and run:
+Only Python 3.9 and above is supported. Create a virtualenv and run:
 
 ```bash
 pip3 install gidgetlab-kit
 ```
 
 To use the cli tool, [pipx](https://pipxproject.github.io/pipx/) is recommended.
```

### Comparing `gidgetlab_kit-0.7.1/pyproject.toml` & `gidgetlab_kit-0.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 source = "vcs"
 
 [project]
 name = "gidgetlab-kit"
 dynamic = ["version"]
 description = "Python package to interact with GitLab"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "MIT"
 license-files = { paths = ["LICENSE"] }
 authors = [{ name = "Benjamin Bertrand", email = "beenje@gmail.com" }]
 keywords = ["gitlab", "async"]
-dependencies = ["gidgetlab", "httpx", "typer", "pydantic", "python-dateutil"]
+dependencies = ["gidgetlab", "httpx", "typer>=0.9.0", "pydantic", "python-dateutil"]
 
 [project.urls]
 Source = "https://gitlab.com/beenje/gidgetlab-kit"
 
 [project.scripts]
 gidgetlab = "gidgetlab_kit.command:app"
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov", "pytest-asyncio", "pytest-mock"]
 
 [tool.black]
-target_version = ["py38"]
+target_version = ["py39"]
+
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "B"]
```

### Comparing `gidgetlab_kit-0.7.1/PKG-INFO` & `gidgetlab_kit-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gidgetlab-kit
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python package to interact with GitLab
 Project-URL: Source, https://gitlab.com/beenje/gidgetlab-kit
 Author-email: Benjamin Bertrand <beenje@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: async,gitlab
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: gidgetlab
 Requires-Dist: httpx
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
-Requires-Dist: typer
+Requires-Dist: typer>=0.9.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-asyncio; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-mock; extra == 'tests'
 Description-Content-Type: text/markdown
 
@@ -64,15 +64,15 @@
   get                Get one or several items from the given endpoint
   list-projects      List all projects from group (including subgroups)
   trigger-pipelines  Trigger the pipeline for all or a subset of projects...
 ```
 
 ## Installation
 
-Only Python 3.8 and above is tested. Create a virtualenv and run:
+Only Python 3.9 and above is supported. Create a virtualenv and run:
 
 ```bash
 pip3 install gidgetlab-kit
 ```
 
 To use the cli tool, [pipx](https://pipxproject.github.io/pipx/) is recommended.
```

