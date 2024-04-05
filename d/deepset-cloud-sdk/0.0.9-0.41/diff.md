# Comparing `tmp/deepset_cloud_sdk-0.0.9.tar.gz` & `tmp/deepset_cloud_sdk-0.41.tar.gz`

## Comparing `deepset_cloud_sdk-0.0.9.tar` & `deepset_cloud_sdk-0.41.tar`

### file list

```diff
@@ -1,31 +1,51 @@
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/CONTRIBUTING.md
--rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/assets/logo.png
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/README.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/__init__.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/cli.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/models.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/config.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/deepset_cloud_api.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/files.py
--rw-r--r--   0        0        0     9323 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/upload_sessions.py
--rw-r--r--   0        0        0    10237 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/s3/upload.py
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/service/files_service.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/utils/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/utils/progress_bar.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/async_client/__init__.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/async_client/files.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/sync_client/__init__.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/workflows/sync_client/files.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/cli/README.md
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.pdf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/data/example.txt.meta.json
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/sdk/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/examples/sdk/upload.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/.gitignore
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/README.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/mkdocs.yml
+-rw-r--r--   0        0        0   475761 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/assets/cli.gif
+-rw-r--r--   0        0        0    48074 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/assets/logo.png
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/README.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/__init__.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/cli.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/config.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/deepset_cloud_api.py
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/files.py
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/upload_sessions.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_s3/__init__.py
+-rw-r--r--   0        0        0    11656 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_s3/upload.py
+-rw-r--r--   0        0        0    28822 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_service/files_service.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_utils/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/_utils/datetime.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/__init__.py
+-rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/files.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/__init__.py
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/files.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/sync_client/utils.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/index.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/upload_files.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_images/favicon.svg
+-rw-r--r--   0        0        0    15589 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_images/white-logo.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/renderers.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/requirements.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/async_client.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/cli.yml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_pydoc/config/sync_client.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/_stylesheets/extra.css
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/cli/README.md
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.pdf
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/data/example.txt.meta.json
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/sdk/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/docs/examples/sdk/upload.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example.txt.meta.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example2.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/test-upload/example2.txt.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/.gitignore
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/LICENSE
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/README.md
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/pyproject.toml
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 deepset_cloud_sdk-0.41/PKG-INFO
```

### Comparing `deepset_cloud_sdk-0.0.9/.pre-commit-config.yaml` & `deepset_cloud_sdk-0.41/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,43 @@
     rev: v4.4.0
     hooks:
       - id: check-json # checks JSON files for parseable syntax.
       - id: check-yaml # checks yaml files for parseable syntax.
       - id: end-of-file-fixer # ensures that a file is either empty, or ends with one newline.
       - id: trailing-whitespace # trims trailing whitespace
 
+  - repo: https://github.com/PyCQA/autoflake
+    rev: v2.1.1
+    hooks:
+      - id: autoflake
+        args:
+          - "--in-place"
+          - "--expand-star-imports"
+          - "--remove-duplicate-keys"
+          - "--remove-unused-variables"
+          - "-v"
+
   - repo: https://github.com/psf/black
     # Please keep these aligned with the versions defined in the pyproject.toml [tool.hatch.envs.code-quality]
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     # Please keep these aligned with the versions defined in the pyproject.toml [tool.hatch.envs.code-quality]
     rev: "v1.1.1"
     hooks:
       - id: mypy
         args:
           - "--ignore-missing-imports"
         additional_dependencies:
+          - types-aiofiles==23.1.0.2
           - "types-tabulate~=0.9.0"
+          - "types-requests~=2.28.11"
         #   - "types-Markdown~=3.4.2"
-        #   - "types-requests~=2.28.11"
         #   - "types-PyYAML~=6.0.12"
         #   - "types-python-dateutil~=2.8.19"
         #   - "types-redis~=4.5.1"
 
   - repo: https://github.com/pycqa/isort
     # Please keep these aligned with the versions defined in the pyproject.toml [tool.hatch.envs.code-quality]
     rev: 5.12.0
```

### Comparing `deepset_cloud_sdk-0.0.9/assets/logo.png` & `deepset_cloud_sdk-0.41/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/README.md` & `deepset_cloud_sdk-0.41/deepset_cloud_sdk/README.md`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/config.py` & `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from dataclasses import dataclass
 
 import structlog
 from dotenv import load_dotenv
 
 logger = structlog.get_logger(__name__)
 
-ENV_FILE_PATH = os.path.expanduser("~/.deepset-cloud-cli/.env")
+ENV_FILE_PATH = os.path.expanduser("~/.deepset-cloud/.env")
 
 
 def load_environment() -> bool:
-    """Load environment variables from .env file.
+    """Load environment variables from the .env file.
 
-    If an .env file is present in the current directory, load the environment variables from there.
-    Otherwise, load the environment variables from the .env file in the home directory that can be created using the CLI.
-    To create the .env file in the home directory, run `deepset-cloud-cli login` in the terminal.
+    If an .env file exists in the current directory, load the environment variables from there.
+    Otherwise, load the environment variables from the .env file in the home directory. You can create this file using the CLI
+    by running `deepset-cloud login` in the terminal.
 
     :return: True if the environment variables were loaded successfully, False otherwise.
     """
     successfully_loded_env: bool = False
     current_path_env = os.path.join(os.getcwd(), ".env")
     if os.path.isfile(current_path_env):
         # Load the environment variables from the .env file in the current directory
@@ -30,18 +30,18 @@
         # Load the environment variables from the .env file in the home directory
         successfully_loded_env = load_dotenv(ENV_FILE_PATH)
         return successfully_loded_env
 
 
 loaded_env_vars = load_environment()
 if loaded_env_vars:
-    logger.info("Environment variables loaded successfully")
+    logger.info("Environment variables loaded successfully.")
 else:
     logger.warning(
-        "No environment variables were loaded from the .env file. Set API_KEY and API_URL manually. If you dont wan't to set them manually, run `deepset-cloud-cli login` in the terminal."
+        "No environment variables were loaded from the .env file. Create the .env file and add API_KEY and API_URL there, or run `deepset-cloud login` in the terminal to let SDK create the file for you."
     )
 
 # connection to deepset Cloud
 API_URL: str = os.getenv("API_URL", "https://api.cloud.deepset.ai/api/v1")
 
 API_KEY: str = os.getenv("API_KEY", "")
 
@@ -57,11 +57,11 @@
     api_url: str = API_URL
 
     def __post_init__(self) -> None:
         """Validate config."""
         assert (
             self.api_key != ""
         ), "You must set the API_KEY environment variable. Go to [Connections](https://cloud.deepset.ai/settings/connections) in deepset Cloud to get an API key."
-        assert self.api_url != "", "API_URL environment variable must be set"
+        assert self.api_url != "", "API_URL environment variable must be set."
 
         if self.api_url.endswith("/"):
             self.api_url = self.api_url[:-1]
```

### Comparing `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/deepset_cloud_api.py` & `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/deepset_cloud_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 from contextlib import asynccontextmanager
 from typing import Any, AsyncGenerator, Callable, Dict, Optional
 
 import httpx
 import structlog
 from httpx import Response
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
-from deepset_cloud_sdk.api.config import CommonConfig
+from deepset_cloud_sdk._api.config import CommonConfig
 
 logger = structlog.get_logger(__name__)
 
 
 class WorkspaceNotDefinedError(Exception):
     """The workspace_name is not defined. Set an environment variable or pass the `workspace_name` argument."""
 
@@ -22,37 +23,40 @@
 
     This class takes care of all API calls to deepset Cloud and handles authentication and errors.
     """
 
     def __init__(self, config: CommonConfig, client: httpx.AsyncClient) -> None:
         """Create a deepset Cloud API client.
 
-        Add a config for authencation and a HTTPX client for
+        Add a config for authentication and a HTTPX client for
         sending requests.
 
         :param config: Config for authentication.
         :param client: HTTPX client for sending requests.
         """
         self.headers = {
             "Accept": "application/json",
             "Authorization": f"Bearer {config.api_key}",
+            "X-Client-Source": "deepset-cloud-sdk",
         }
         self.base_url = lambda workspace_name: self._get_base_url(config.api_url)(workspace_name)
         self.client = client
 
     @staticmethod
     def _get_base_url(api_url: str) -> Callable:
         def func(workspace_name: str) -> str:
             """Get the base URL for the API.
 
             :param workspace_name: Name of the workspace to use.
             :return: Base URL.
             """
             if not workspace_name or workspace_name == "":
-                raise WorkspaceNotDefinedError(f"Workspace name is not defined. Got '{workspace_name}'")
+                raise WorkspaceNotDefinedError(
+                    f"Workspace name is not defined. Got '{workspace_name}'. Enter the name of the workspace in `workspace_name`."
+                )
 
             return f"{api_url}/workspaces/{workspace_name}"
 
         return func
 
     @classmethod
     @asynccontextmanager
@@ -60,14 +64,20 @@
         """Create a new instance of the API client.
 
         :param config: CommonConfig object.
         """
         async with httpx.AsyncClient() as client:
             yield cls(config, client)
 
+    @retry(
+        retry=retry_if_exception_type(httpx.RequestError),
+        stop=stop_after_attempt(3),
+        wait=wait_fixed(1),
+        reraise=True,
+    )
     async def get(
         self, workspace_name: str, endpoint: str, params: Optional[Dict[str, Any]] = None, timeout_s: int = 20
     ) -> Response:
         """Make a GET request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
@@ -78,30 +88,31 @@
         response = await self.client.get(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
             headers=self.headers,
             timeout=timeout_s,
         )
         logger.debug(
-            "Called deepset Cloud API",
+            "Called deepset Cloud API.",
             method="GET",
             workspace=workspace_name,
             endpoint=endpoint,
             params=params,
             status=response.status_code,
         )
         return response
 
     async def post(
         self,
         workspace_name: str,
         endpoint: str,
         params: Optional[Dict[str, Any]] = None,
-        data: Optional[Dict[str, Any]] = None,
+        json: Optional[Dict[str, Any]] = None,
         files: Optional[Dict[str, Any]] = None,
+        data: Optional[Dict[str, Any]] = None,
         timeout_s: int = 20,
     ) -> Response:
         """Make a POST request to the deepset Cloud API.
 
         :param workspace_name: Name of the workspace to use.
         :param endpoint: Endpoint to call.
         :param params: Query parameters to pass.
@@ -109,15 +120,16 @@
         :param files: Files to pass.
         :param timeout_s: Timeout in seconds.
         :return: Response object.
         """
         response = await self.client.post(
             f"{self.base_url(workspace_name)}/{endpoint}",
             params=params or {},
-            json=data or {},
+            json=json or {},
+            data=data or {},
             files=files,
             headers=self.headers,
             timeout=timeout_s,
         )
         logger.debug(
             "Called deepset Cloud API",
             method="POST",
@@ -188,15 +200,15 @@
             endpoint=endpoint,
             data=data or {},
             status=response.status_code,
         )
         return response
 
 
-def get_deepset_cloud_api(config: CommonConfig, client: httpx.AsyncClient) -> DeepsetCloudAPI:
-    """Deepset Cloud API factory. Return an instance of DeepsetCloudAPI.
+def get_deepset_cloud_api(config: CommonConfig, client: httpx.AsyncClient) -> DeepsetCloudAPI:  # noqa
+    """deepset Cloud API factory. Return an instance of DeepsetCloudAPI.
 
     :param config: CommonConfig object.
     :param client: httpx.AsyncClient object.
     :return: DeepsetCloudAPI object.
     """
     return DeepsetCloudAPI(config=config, client=client)
```

### Comparing `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/api/upload_sessions.py` & `deepset_cloud_sdk-0.41/deepset_cloud_sdk/_api/upload_sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Upload sessions API for deepset Cloud."""
 
 import datetime
 import enum
 from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import Dict, List, Optional
 from uuid import UUID
 
 import structlog
 from httpx import codes
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
-from deepset_cloud_sdk.api.deepset_cloud_api import DeepsetCloudAPI
+from deepset_cloud_sdk._api.deepset_cloud_api import DeepsetCloudAPI
+from deepset_cloud_sdk._utils.datetime import from_isoformat
 from deepset_cloud_sdk.models import UserInfo
 
 logger = structlog.get_logger(__name__)
 
 
 @dataclass
-class AWSPrefixedRequesetConfig:
+class AWSPrefixedRequestConfig:
     """AWS prefixed request config.
 
     This prefixed request config can be used to send authenticated requests to AWS S3.
     """
 
     fields: Dict[str, str]
     url: str
@@ -29,15 +31,15 @@
 @dataclass
 class UploadSession:
     """Upload session object."""
 
     session_id: UUID
     documentation_url: str
     expires_at: datetime.datetime
-    aws_prefixed_request_config: AWSPrefixedRequesetConfig
+    aws_prefixed_request_config: AWSPrefixedRequestConfig
 
 
 class UploadSessionWriteModeEnum(str, enum.Enum):
     """Write mode for upload session."""
 
     KEEP = "KEEP"  # to keep duplicate files
     OVERWRITE = "OVERWRITE"  # to overwrite files
@@ -114,73 +116,85 @@
         Create FileAPI object.
 
         :param deepset_cloud_api: Instance of the DeepsetCloudAPI.
         """
         self._deepset_cloud_api = deepset_cloud_api
 
     async def create(self, workspace_name: str, write_mode: WriteMode = WriteMode.KEEP) -> UploadSession:
-        """Create upload session.
+        """Create and upload session.
 
-        This method creates an upload session for a given workspace. The upload session
-        is valid for 24 hours. After that, you need to create a new upload session.
+        This method creates an upload session for a given workspace. Use this session to upload files to deepset Cloud.
 
-        You must close a session to start the ingestion.
+        You must close the session to start the file upload. If you don't close a session, it remains open for 24 hours.
+        After that it's automatically closed and you must open a new session to upload more files.
 
         :param workspace_name: Name of the workspace.
+        :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+        Possible options are:
+        KEEP - uploads the file with the same name and keeps both files in the workspace.
+        OVERWRITE - overwrites the file that is in the workspace.
+        FAIL - fails to upload the file with the same name.
         :raises FailedToSendUploadSessionRequest: If the session could not be created.
         :return: UploadSession object.
         """
         response = await self._deepset_cloud_api.post(
-            workspace_name=workspace_name, endpoint="upload_sessions", data={"write_mode": write_mode.value}
+            workspace_name=workspace_name, endpoint="upload_sessions", json={"write_mode": write_mode.value}
         )
         if response.status_code != codes.CREATED:
             logger.error(
-                "Failed to create upload session.",
+                "Failed to create the upload session.",
                 status_code=response.status_code,
                 response_body=response.text,
             )
             raise FailedToSendUploadSessionRequest(
-                f"Failed to create upload session. Status code: {response.status_code}."
+                f"Failed to create the upload session. Status code: {response.status_code}."
             )
         response_body = response.json()
         return UploadSession(
             session_id=UUID(response_body["session_id"]),
             documentation_url=response_body["documentation_url"],
-            expires_at=datetime.datetime.fromisoformat(response_body["expires_at"]),
-            aws_prefixed_request_config=AWSPrefixedRequesetConfig(
+            expires_at=from_isoformat(response_body["expires_at"]),
+            aws_prefixed_request_config=AWSPrefixedRequestConfig(
                 fields=response_body["aws_prefixed_request_config"]["fields"],
                 url=response_body["aws_prefixed_request_config"]["url"],
             ),
         )
 
     async def close(self, workspace_name: str, session_id: UUID) -> None:
-        """Close upload session.
+        """Close an upload session.
 
-        This method closes an upload session for a given workspace. Once the session is closed, you can't upload
-        more files to this session and the ingestion is automatically started.
+        This method closes an upload session for a given workspace. Once the session is closed, the file ingestion starts automatically.
         This means that your files will appear in the workspace after a short while.
 
+        You can't upload files to a closed session.
+
         :param workspace_name: Name of the workspace.
         :param session_id: ID of the session.
         :raises FailedToSendUploadSessionRequest: If the session could not be closed.
         :raises FailedToSendUploadSessionRequest: If the status could not be fetched.
         """
         response = await self._deepset_cloud_api.put(
             workspace_name=workspace_name, endpoint=f"upload_sessions/{session_id}", data={"status": "CLOSED"}
         )
         if response.status_code != codes.NO_CONTENT:
             logger.error(
-                "Failed to close upload session.",
+                "Failed to close the upload session.",
                 status_code=response.status_code,
                 response_body=response.text,
             )
             raise FailedToSendUploadSessionRequest(
-                f"Failed to close upload session. Status code: {response.status_code}."
+                f"Failed to close the upload session. Status code: {response.status_code}."
             )
 
+    @retry(
+        retry=retry_if_exception_type(FailedToSendUploadSessionRequest),
+        stop=stop_after_attempt(3),
+        wait=wait_fixed(1),
+        reraise=True,
+    )
     async def status(self, workspace_name: str, session_id: UUID) -> UploadSessionStatus:
         """Fetch upload session status.
 
         This method fetches the status of an upload session for a given workspace.
 
         :param workspace_name: Name of the workspace.
         :param session_id: ID of the session.
@@ -199,36 +213,48 @@
             raise FailedToSendUploadSessionRequest(
                 f"Failed to get upload session status. Status code: {response.status_code}."
             )
         response_body = response.json()
         return UploadSessionStatus(
             session_id=UUID(response_body["session_id"]),
             documentation_url=response_body["documentation_url"],
-            expires_at=datetime.datetime.fromisoformat(response_body["expires_at"]),
+            expires_at=from_isoformat(response_body["expires_at"]),
             ingestion_status=UploadSessionIngestionStatus(
                 failed_files=response_body["ingestion_status"]["failed_files"],
                 finished_files=response_body["ingestion_status"]["finished_files"],
             ),
         )
 
-    async def list(self, workspace_name: str, limit: int = 10, page_number: int = 1) -> UploadSessionDetailList:
+    @retry(
+        retry=retry_if_exception_type(FailedToSendUploadSessionRequest),
+        stop=stop_after_attempt(3),
+        wait=wait_fixed(1),
+        reraise=True,
+    )
+    async def list(
+        self, workspace_name: str, is_expired: Optional[bool] = False, limit: int = 10, page_number: int = 1
+    ) -> UploadSessionDetailList:
         """List upload sessions.
 
         This method lists all upload sessions for a given workspace.
 
         :param workspace_name: Name of the workspace.
         :param limit: Number of upload sessions to return.
         :param page_number: Page number of the upload sessions.
         :raises FailedToSendUploadSessionRequest: If the list could not be fetched.
         :return: UploadSessionDetailList object.
         """
+        params = {"limit": limit, "page_number": page_number}
+        if is_expired:
+            params["is_expired"] = is_expired
+
         response = await self._deepset_cloud_api.get(
             workspace_name=workspace_name,
-            endpoint=f"upload_sessions",
-            params={"limit": limit, "page_number": page_number},
+            endpoint="upload_sessions",
+            params=params,
         )
         if response.status_code != codes.OK:
             logger.error(
                 "Failed to get upload session status.",
                 status_code=response.status_code,
                 response_body=response.text,
             )
@@ -243,15 +269,15 @@
                 UploadSessionDetail(
                     session_id=UUID(upload_session["session_id"]),
                     created_by=UserInfo(
                         user_id=UUID(upload_session["created_by"]["user_id"]),
                         given_name=upload_session["created_by"]["given_name"],
                         family_name=upload_session["created_by"]["family_name"],
                     ),
-                    expires_at=datetime.datetime.fromisoformat(upload_session["expires_at"]),
-                    created_at=datetime.datetime.fromisoformat(upload_session["created_at"]),
+                    expires_at=from_isoformat(upload_session["expires_at"]),
+                    created_at=from_isoformat(upload_session["created_at"]),
                     write_mode=UploadSessionWriteModeEnum(upload_session["write_mode"]),
                     status=UploadSessionStatusEnum(upload_session["status"]),
                 )
                 for upload_session in response_body["data"]
             ],
         )
```

### Comparing `deepset_cloud_sdk-0.0.9/deepset_cloud_sdk/service/files_service.py` & `deepset_cloud_sdk-0.41/deepset_cloud_sdk/workflows/async_client/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,263 +1,239 @@
-"""Module for all file-related operations."""
-from __future__ import annotations
-
-import asyncio
-import os
-import time
-from contextlib import asynccontextmanager
+# pylint:disable=too-many-arguments
+"""This module contains async functions for uploading files and folders to deepset Cloud."""
 from pathlib import Path
-from typing import AsyncGenerator, List, Optional
+from typing import AsyncGenerator, List, Optional, Union
 from uuid import UUID
 
-import structlog
+from sniffio import AsyncLibraryNotFoundError
 
-from deepset_cloud_sdk.api.config import CommonConfig
-from deepset_cloud_sdk.api.deepset_cloud_api import DeepsetCloudAPI
-from deepset_cloud_sdk.api.files import File, FilesAPI
-from deepset_cloud_sdk.api.upload_sessions import (
-    UploadSession,
-    UploadSessionsAPI,
+from deepset_cloud_sdk._api.config import (
+    API_KEY,
+    API_URL,
+    DEFAULT_WORKSPACE_NAME,
+    CommonConfig,
+)
+from deepset_cloud_sdk._api.files import File
+from deepset_cloud_sdk._api.upload_sessions import (
+    UploadSessionDetail,
     UploadSessionStatus,
     WriteMode,
 )
-from deepset_cloud_sdk.models import DeepsetCloudFile
-from deepset_cloud_sdk.s3.upload import S3
+from deepset_cloud_sdk._s3.upload import S3UploadSummary
+from deepset_cloud_sdk._service.files_service import DeepsetCloudFile, FilesService
 
-logger = structlog.get_logger(__name__)
 
+def _get_config(api_key: Optional[str] = None, api_url: Optional[str] = None) -> CommonConfig:
+    return CommonConfig(api_key=api_key or API_KEY, api_url=api_url or API_URL)
 
-class FilesService:
-    """Service for all file-related operations."""
 
-    def __init__(self, upload_sessions: UploadSessionsAPI, files: FilesAPI, s3: S3):
-        """Initialize the service.
-
-        :param upload_sessions: API for upload sessions.
-        :param files: API for files.
-        :param aws: AWS client.
-        """
-        self._upload_sessions = upload_sessions
-        self._files = files
-        self._s3 = s3
-
-    @classmethod
-    @asynccontextmanager
-    async def factory(cls, config: CommonConfig) -> AsyncGenerator[FilesService, None]:
-        """Create a new instance of the service.
-
-        :param config: CommonConfig object.
-        :param client: httpx client.
-        :return: New instance of the service.
-        """
-        async with DeepsetCloudAPI.factory(config) as deepset_cloud_api:
-            files_api = FilesAPI(deepset_cloud_api)
-            upload_sessions_api = UploadSessionsAPI(deepset_cloud_api)
-
-            yield cls(upload_sessions_api, files_api, S3(concurrency=30))
-
-    async def _wait_for_finished(self, workspace_name: str, session_id: UUID, total_files: int, timeout_s: int) -> None:
-        start = time.time()
-        ingested_files = 0
-        while ingested_files < total_files:
-            if time.time() - start > timeout_s:
-                raise TimeoutError("Ingestion timed out.")
-
-            upload_session_status: UploadSessionStatus = await self._upload_sessions.status(
-                workspace_name=workspace_name, session_id=session_id
-            )
-            ingested_files = (
-                upload_session_status.ingestion_status.finished_files
-                + upload_session_status.ingestion_status.failed_files
-            )
-            logger.info(
-                "Waiting for ingestion to finish.",
-                finished_files=upload_session_status.ingestion_status.finished_files,
-                failed_files=upload_session_status.ingestion_status.failed_files,
-                total_files=total_files,
-            )
-            await asyncio.sleep(1)
-
-    @asynccontextmanager
-    async def _create_upload_session(
-        self,
-        workspace_name: str,
-        write_mode: WriteMode = WriteMode.KEEP,
-    ) -> AsyncGenerator[UploadSession, None]:
-        """Create a new upload session.
-
-        :param workspace_name: Name of the workspace to create the upload session for.
-        :return: Upload session id.
-        """
-        upload_session = await self._upload_sessions.create(workspace_name=workspace_name, write_mode=write_mode)
-        try:
-            yield upload_session
-        finally:
-            await self._upload_sessions.close(workspace_name=workspace_name, session_id=upload_session.session_id)
-
-    async def upload_file_paths(
-        self,
-        workspace_name: str,
-        file_paths: List[Path],
-        write_mode: WriteMode = WriteMode.KEEP,
-        blocking: bool = True,
-        timeout_s: int = 300,
-    ) -> None:
-        """Upload a list of files to a workspace.
-
-        Upload a list of files  to a selected workspace using upload sessions. If blocking is True, the function waits until
-        all files are uploaded and listed by deepset Cloud. If blocking is False, the function returns immediately after
-        the upload of the files is done. Note: It can take a while until the files are listed in deepset Cloud.
-
-        :param workspace_name: Name of the workspace to upload the files to.
-        :file_paths: List of file paths to upload.
-        :blocking: If True, blocks until the ingestion is finished.
-        :timeout_s: Timeout in seconds for the blocking ingestion.
-        :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
-        """
-        # create session to upload files to
-        async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
-            # upload file paths to session
-
-            upload_summary = await self._s3.upload_files_from_paths(
-                upload_session=upload_session, file_paths=file_paths
-            )
-            logger.info(
-                "Summary of S3 Uploads",
-                successful_uploads=upload_summary.successful_upload_count,
-                failed_uploads=upload_summary.failed_upload_count,
-                failed=upload_summary.failed,
-            )
-
-        # wait for ingestion to finish
-        if blocking:
-            total_files = len(list(filter(lambda x: not os.path.basename(x).endswith(".meta.json"), file_paths)))
-            await self._wait_for_finished(
+async def list_files(
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    name: Optional[str] = None,
+    content: Optional[str] = None,
+    odata_filter: Optional[str] = None,
+    batch_size: int = 100,
+    timeout_s: Optional[int] = None,
+) -> AsyncGenerator[List[File], None]:
+    """List all files in a workspace.
+
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to list the files from. It uses the workspace from the .ENV file by default.
+    :param name: Name of the file to odata_filter for.
+    :param content: Content of the file to odata_filter for.
+    :param odata_filter: The odata_filter to apply to the file list.
+    For example, `odata_filter="category eq 'news'"` lists files with metadata `{"meta": {"category": "news"}}`.
+    :param timeout_s: The timeout in seconds for this API call.
+    :param batch_size: Batch size for the listing.
+    :return: List of files.
+    """
+    try:
+        async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+            async for file_batch in file_service.list_all(
+                workspace_name=workspace_name,
+                name=name,
+                content=content,
+                odata_filter=odata_filter,
+                batch_size=batch_size,
+                timeout_s=timeout_s,
+            ):
+                yield file_batch
+    except AsyncLibraryNotFoundError:
+        # since we are using asyncio.run() in the sync wrapper, we need to catch this error
+        pass
+
+
+async def list_upload_sessions(
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    is_expired: Optional[bool] = None,
+    batch_size: int = 100,
+    timeout_s: Optional[int] = None,
+) -> AsyncGenerator[List[UploadSessionDetail], None]:
+    """List the details of all upload sessions for a given workspace, including the closed sessions.
+
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to list the files from. It uses the workspace from the .ENV file by default.
+    :param is_expired: Whether to list expired upload sessions.
+    :param batch_size: Batch size for the listing.
+    :param timeout_s: Timeout in seconds for the API requests.
+    :return: List of files.
+    """
+    try:
+        async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+            async for upload_session_batch in file_service.list_upload_sessions(
                 workspace_name=workspace_name,
-                session_id=upload_session.session_id,
-                total_files=total_files,
+                is_expired=is_expired,
+                batch_size=batch_size,
                 timeout_s=timeout_s,
-            )
+            ):
+                yield upload_session_batch
+    except AsyncLibraryNotFoundError:
+        # since we are using asyncio.run() in the sync wrapper, we need to catch this error
+        pass
+
+
+async def get_upload_session(
+    session_id: UUID,
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+) -> UploadSessionStatus:
+    """Get the status of an upload session.
+
+    :param session_id: ID of the upload session to get the status for.
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to list the files from.
+    :return: List of files.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        return await file_service.get_upload_session(
+            workspace_name=workspace_name,
+            session_id=session_id,
+        )
 
-    async def upload_folder(
-        self,
-        workspace_name: str,
-        folder_path: Path,
-        write_mode: WriteMode = WriteMode.KEEP,
-        blocking: bool = True,
-        timeout_s: int = 300,
-    ) -> None:
-        """Upload a folder to a workspace.
-
-        Upload a folder to a selected workspace using upload sessions. If blocking is True, the function waits until
-        all files are uploaded and listed by deepset Cloud. If blocking is False, the function returns immediately after
-        the upload of the files is done. Note: It can take a while until the files are listed in deepset Cloud.
-
-        :param workspace_name: Name of the workspace to upload the files to.
-        :folder_path: Path to the folder to upload.
-        :blocking: If True, blocks until the ingestion is finished.
-        :timeout_s: Timeout in seconds for the blocking ingestion.
-        :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
-        """
-        all_files = [path for path in folder_path.glob("**/*")]
-
-        file_paths = [
-            path
-            for path in all_files
-            if path.is_file() and ((path.suffix in [".txt", ".pdf"]) or path.name.endswith("meta.json"))
-        ]
-        if len(file_paths) < len(all_files):
-            logger.warning(
-                "Skipping files with unsupported file format.",
-                folder_path=folder_path,
-                skipped_files=len(all_files) - len(file_paths),
-            )
 
-        await self.upload_file_paths(
+async def upload(
+    paths: List[Path],
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    write_mode: WriteMode = WriteMode.KEEP,
+    blocking: bool = True,
+    timeout_s: Optional[int] = None,
+    show_progress: bool = True,
+    recursive: bool = False,
+) -> S3UploadSummary:
+    """Upload a folder to deepset Cloud.
+
+    :param paths: Path to the folder to upload. If the folder contains unsupported files, they're skipped.
+    during the upload. Supported file formats are TXT and PDF.
+    :param api_key: API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+    Possible options are:
+    KEEP - uploads the file with the same name and keeps both files in the workspace.
+    OVERWRITE - overwrites the file that is in the workspace.
+    FAIL - fails to upload the file with the same name.
+    :param blocking: Whether to wait for the upload to finish.
+    :param timeout_s: Timeout in seconds for the upload.
+    :param show_progress: Shows the upload progress.
+    :param recursive: Uploads files from subdirectories as well.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        return await file_service.upload(
             workspace_name=workspace_name,
-            file_paths=file_paths,
+            paths=paths,
             write_mode=write_mode,
             blocking=blocking,
             timeout_s=timeout_s,
+            show_progress=show_progress,
+            recursive=recursive,
         )
 
-    async def upload_texts(
-        self,
-        workspace_name: str,
-        dc_files: List[DeepsetCloudFile],
-        write_mode: WriteMode = WriteMode.KEEP,
-        blocking: bool = True,
-        timeout_s: int = 300,
-    ) -> None:
-        """
-        Upload a list of raw texts to a workspace.
-
-        Upload a list of raw texts to a selected workspace using upload sessions. This method accepts a list of DeepsetCloudFiles
-        which contain raw text, file name, and optional meta data.
-
-        If blocking is True, the function waits until all files are uploaded and listed by deepset Cloud.
-        If blocking is False, the function returns immediately after the upload of the files is done.
-        Note: It can take a while until the files are listed in deepset Cloud.
-
-        :param workspace_name: Name of the workspace to upload the files to.
-        :dc_files: List of DeepsetCloudFiles to upload.
-        :blocking: If True, blocks until the ingestion is finished.
-        :timeout_s: Timeout in seconds for blocking.
-        :raises TimeoutError: If blocking is True and the ingestion takes longer than timeout_s.
-        """
-        # create session to upload files to
-        async with self._create_upload_session(workspace_name=workspace_name, write_mode=write_mode) as upload_session:
-            await self._s3.upload_texts(upload_session=upload_session, dc_files=dc_files)
 
-        if blocking:
-            await self._wait_for_finished(
-                workspace_name=workspace_name,
-                session_id=upload_session.session_id,
-                total_files=len(dc_files),
-                timeout_s=timeout_s,
-            )
+async def download(
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    file_dir: Optional[Union[Path, str]] = None,
+    name: Optional[str] = None,
+    content: Optional[str] = None,
+    odata_filter: Optional[str] = None,
+    include_meta: bool = True,
+    batch_size: int = 50,
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    show_progress: bool = True,
+    timeout_s: Optional[int] = None,
+) -> None:
+    """Download a folder to deepset Cloud.
+
+    Downloads all files from a workspace to a local folder.
+
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param file_dir: Path to the folder to download. If the folder contains unsupported files, they're skipped.
+    during the upload. Supported file formats are TXT and PDF.
+    :param name: Name of the file to odata_filter by.
+    :param content: Content of a file to odata_filter by.
+    :param odata_filter: odata_filter by file meta data.
+    :param include_meta: Whether to include the file meta in the folder.
+    :param batch_size: Batch size for the listing.
+    :param api_key: API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param show_progress: Shows the upload progress.
+    :param timeout_s: Timeout in seconds for the download.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        await file_service.download(
+            workspace_name=workspace_name,
+            file_dir=file_dir,
+            name=name,
+            content=content,
+            odata_filter=odata_filter,
+            include_meta=include_meta,
+            batch_size=batch_size,
+            show_progress=show_progress,
+            timeout_s=timeout_s,
+        )
 
-    async def list_all(
-        self,
-        workspace_name: str,
-        name: Optional[str] = None,
-        content: Optional[str] = None,
-        odata_filter: Optional[str] = None,
-        batch_size: int = 100,
-        timeout_s: int = 20,
-    ) -> AsyncGenerator[List[File], None]:
-        """List all files in a workspace.
-
-        Returns an async generator that yields lists of files. The generator is finished when all files are listed.
-        You can specfy the batch size per number of returned files with batch_size.
-
-        :param workspace_name: Name of the workspace to use.
-        :param name: odata_filter by file name.
-        :param content: odata_filter by file content.
-        :param odata_filter: odata_filter by file meta data.
-        :param batch_size: Number of files to return per request.
-        :param timeout_s: Timeout in seconds for the listing.
-        :raises TimeoutError: If the listing takes longer than timeout_s.
-        """
-        start = time.time()
-        has_more = True
-
-        after_value = None
-        after_file_id = None
-        while has_more:
-            if time.time() - start > timeout_s:
-                raise TimeoutError(f"Listing all files in workspace {workspace_name} timed out.")
-            response = await self._files.list_paginated(
-                workspace_name,
-                name=name,
-                content=content,
-                odata_filter=odata_filter,
-                limit=batch_size,
-                after_file_id=after_file_id,
-                after_value=after_value,
-            )
-            has_more = response.has_more
-            if not response.data:
-                return
-            after_value = response.data[-1].created_at
-            after_file_id = response.data[-1].file_id
-            yield response.data
+
+async def upload_texts(
+    files: List[DeepsetCloudFile],
+    api_key: Optional[str] = None,
+    api_url: Optional[str] = None,
+    workspace_name: str = DEFAULT_WORKSPACE_NAME,
+    write_mode: WriteMode = WriteMode.KEEP,
+    blocking: bool = True,
+    timeout_s: Optional[int] = None,
+    show_progress: bool = True,
+) -> S3UploadSummary:
+    """Upload raw texts to deepset Cloud.
+
+    :param files: List of DeepsetCloudFiles to upload.
+    :param api_key: deepset Cloud API key to use for authentication.
+    :param api_url: API URL to use for authentication.
+    :param workspace_name: Name of the workspace to upload the files to. It uses the workspace from the .ENV file by default.
+    :param write_mode: Specifies what to do when a file with the same name already exists in the workspace.
+    Possible options are:
+    KEEP - uploads the file with the same name and keeps both files in the workspace.
+    OVERWRITE - overwrites the file that is in the workspace.
+    FAIL - fails to upload the file with the same name.
+    :param blocking: Whether to wait for the files to be listed and displayed in deepset Cloud.
+    This may take a couple of minutes.
+    :param timeout_s: Timeout in seconds for the `blocking` parameter.
+    :param show_progress: Shows the upload progress.
+    """
+    async with FilesService.factory(_get_config(api_key=api_key, api_url=api_url)) as file_service:
+        return await file_service.upload_texts(
+            workspace_name=workspace_name,
+            files=files,
+            write_mode=write_mode,
+            blocking=blocking,
+            timeout_s=timeout_s,
+            show_progress=show_progress,
+        )
```

### Comparing `deepset_cloud_sdk-0.0.9/examples/data/example.pdf` & `deepset_cloud_sdk-0.41/docs/examples/data/example.pdf`

 * *Files identical despite different names*

### Comparing `deepset_cloud_sdk-0.0.9/.gitignore` & `deepset_cloud_sdk-0.41/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
+*.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
@@ -161,9 +162,11 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .vscode
-
-requirements.txt
+temp
+.idea
+.python-version
+.DS_Store
```

### Comparing `deepset_cloud_sdk-0.0.9/README.md` & `deepset_cloud_sdk-0.41/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 <p align="center">
-  <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
+  <a href="https://cloud.deepset.ai/"><img src="https://raw.githubusercontent.com/deepset-ai/deepset-cloud-sdk/main/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
 
+[![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/tree/python-coverage-comment-action-data)
 [![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml)
 [![Deploy PyPi](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml)
 [![Compliance Checks](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml)
 
-The deepset Cloud SDK is an open source software development kit that provides convenient access and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks.
-This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
+The deepset Cloud SDK is an open source software development kit that provides convenient access and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks. To learn more about deepset Cloud, please have a look at the [official Documentation](https://docs.cloud.deepset.ai/).
 
 # Supported Features
 The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud using Python.
-You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
-- [SDK - Upload datasets](/examples/sdk/upload.py)
-- [CLI - Upload datasets](/examples/cli/README.md)
+You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/deepset-cloud-sdk/examples/cli).
+- [SDK Examples - Upload datasets](/deepset-cloud-sdk/examples/sdk)
+- [CLI Examples - Upload datasets](/deepset-cloud-sdk/examples/cli/)
 
 ## Installation
 The deepset Cloud SDK is available on PyPI and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
 After installing the deepset Cloud SDK, you can use it to interact with deepset Cloud. It comes with a command line interface (CLI), that you can use by calling:
 ```bash
-deepset-cloud-cli --help
+deepset-cloud --help
 ```
 
+<p align="center">
+  <a href="https://cloud.deepset.ai/"><img src="https://raw.githubusercontent.com/deepset-ai/deepset-cloud-sdk/main/assets/cli.gif"  alt="deepset Cloud CLI"></a>
+</p>
+
 ### Development Installation
 To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
 ```bash
 pip install hatch==1.7.0
 hatch build
 ```
 
-## Contributing
-We welcome contributions from the open source community to enhance the deepset Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines and instructions on how to get started.
-We appreciate your contributions, whether they're bug fixes, new features, or documentation improvements.
-
+Instead of calling the cli from the build package, you can call it directly from the source code:
+```bash
+python3 -m deepset_cloud_sdk.cli --help
+```
 
 ---
-
 ## Interested in deepset Cloud?
 If you are interested in exploring deepset Cloud, visit cloud.deepset.ai.
 deepset Cloud provides a range of NLP capabilities and services to help you build and deploy powerful
 natural language processing applications.
 
 ## Interested in Haystack?
 deepset Cloud is powered by Haystack, an open source framework for building end-to-end NLP pipelines.
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
                               _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _S_D_K_]
-[![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
-continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-
-cloud-sdk/actions/workflows/continuous-integration.yml) [![Deploy PyPi](https:/
-/github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
+[![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-
+coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-
+cloud-sdk/tree/python-coverage-comment-action-data) [![Tests](https://
+github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-
+integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/
+actions/workflows/continuous-integration.yml) [![Deploy PyPi](https://
+github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
 badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
 deploy-prod.yml) [![Compliance Checks](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/
 deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml) The deepset
 Cloud SDK is an open source software development kit that provides convenient
 access and integration with deepset Cloud, a powerful cloud offering for
-various natural language processing (NLP) tasks. This README provides an
-overview of the SDK and its features, and information on contributing to the
-project and exploring related resources. # Supported Features The following
-examples demonstrate how to use the deepset Cloud SDK to interact with deepset
-Cloud using Python. You can use the deepset Cloud SDK in the command line as
-well. For more information, see the [CLI documentation](/examples/cli/
-README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
-datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
-available on PyPI and you can install it using pip: ```bash pip install
-deepset-cloud-sdk ``` After installing the deepset Cloud SDK, you can use it to
-interact with deepset Cloud. It comes with a command line interface (CLI), that
-you can use by calling: ```bash deepset-cloud-cli --help ``` ### Development
-Installation To install the deepset Cloud SDK for development, clone the
-repository and install the package in editable mode: ```bash pip install
-hatch==1.7.0 hatch build ``` ## Contributing We welcome contributions from the
-open source community to enhance the deepset Cloud SDK. If you would like to
-contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines
-and instructions on how to get started. We appreciate your contributions,
-whether they're bug fixes, new features, or documentation improvements. --- ##
-Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
-visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
-services to help you build and deploy powerful natural language processing
-applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
-an open source framework for building end-to-end NLP pipelines. - [Project
-website](https://haystack.deepset.ai/) - [GitHub repository](https://
-github.com/deepset-ai/haystack)
+various natural language processing (NLP) tasks. To learn more about deepset
+Cloud, please have a look at the [official Documentation](https://
+docs.cloud.deepset.ai/). # Supported Features The following examples
+demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud
+using Python. You can use the deepset Cloud SDK in the command line as well.
+For more information, see the [CLI documentation](/deepset-cloud-sdk/examples/
+cli). - [SDK Examples - Upload datasets](/deepset-cloud-sdk/examples/sdk) -
+[CLI Examples - Upload datasets](/deepset-cloud-sdk/examples/cli/) ##
+Installation The deepset Cloud SDK is available on PyPI and you can install it
+using pip: ```bash pip install deepset-cloud-sdk ``` After installing the
+deepset Cloud SDK, you can use it to interact with deepset Cloud. It comes with
+a command line interface (CLI), that you can use by calling: ```bash deepset-
+cloud --help ```
+                              _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _C_L_I_]
+### Development Installation To install the deepset Cloud SDK for development,
+clone the repository and install the package in editable mode: ```bash pip
+install hatch==1.7.0 hatch build ``` Instead of calling the cli from the build
+package, you can call it directly from the source code: ```bash python3 -
+m deepset_cloud_sdk.cli --help ``` --- ## Interested in deepset Cloud? If you
+are interested in exploring deepset Cloud, visit cloud.deepset.ai. deepset
+Cloud provides a range of NLP capabilities and services to help you build and
+deploy powerful natural language processing applications. ## Interested in
+Haystack? deepset Cloud is powered by Haystack, an open source framework for
+building end-to-end NLP pipelines. - [Project website](https://
+haystack.deepset.ai/) - [GitHub repository](https://github.com/deepset-ai/
+haystack)
```

### Comparing `deepset_cloud_sdk-0.0.9/pyproject.toml` & `deepset_cloud_sdk-0.41/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deepset-cloud-sdk"
 dynamic = ["version"]
-description = 'deepset cloud SDK'
+description = 'deepset Cloud SDK'
 readme = "README.md"
-requires-python = ">=3.8"
-license = "MIT"
+requires-python = ">= 3.8"
+license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset", email = "rohan.janjua@deepset.ai" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -20,87 +20,99 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "structlog==23.1.0",
-  "httpx==0.24.0",
+  "structlog==24.1.0",
+  "httpx==0.26.0",
   "python-dotenv==1.0.0",
   "typer==0.9.0",
-  "tenacity==8.2.2",
-  "aiohttp==3.8.4",
+  "tenacity==8.2.3",
+  "aiohttp==3.9.1",
+  "aiofiles==23.2.1",
   "tabulate==0.9.0",
-  "progress==1.6"
+  "tqdm==4.66.1",
+  "yaspin==2.3.0",
+  "pyrate-limiter==3.4.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/deepset-cloud-sdk#readme"
 Issues = "https://github.com/deepset-ai/deepset-cloud-sdk/issues"
 Source = "https://github.com/deepset-ai/deepset-cloud-sdk"
 
 
 [project.scripts]
-deepset-cloud-cli  = "deepset_cloud_sdk.cli:run_packaged"
+deepset-cloud  = "deepset_cloud_sdk.cli:run_packaged"
 
 [tool.hatch.version]
 path = "deepset_cloud_sdk/__about__.py"
 
 [tool.hatch.envs.default.scripts]
 tests-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
-tests-integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
+tests-unit = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
+tests-integration = "pytest tests/integration"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10"]
 
 [tool.hatch.envs.default]
 dependencies = [
-  "structlog==23.1.0",
-  "httpx==0.24.0",
+  "structlog==24.1.0",
+  "httpx==0.26.0",
   "python-dotenv==1.0.0",
-  "tenacity==8.2.2",
-  "aiohttp==3.8.4"
+  "tenacity==8.2.3",
+  "aiohttp==3.9.1",
+  "pyrate-limiter==3.4.1",
 ]
 
 [tool.hatch.envs.test.scripts]
 unit-with-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/unit"
 integration = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=deepset_cloud_sdk tests/integration"
 
 [tool.hatch.envs.test]
 template='default'
 dependencies = [
   "pytest-cov==4.0.0",
   "pytest==7.3.1",
   "pytest-asyncio==0.21.0",
+  "Faker==19.13.0",
 ]
 
 
 [tool.hatch.envs.code-quality]
+python = "3.10"
 template='default'
 detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
 dependencies = [
-  "pylint==2.15.2",
+  "pylint==2.17.4",
   "pydocstyle==6.3.0",
   "black==23.3.0",
   "isort==5.12.0",
   "mypy==1.1.1",
   "pre-commit==2.20.0",
-  "types-tabulate==0.9.0.2"
+  "types-aiofiles==23.1.0.2",
+  "types-tabulate==0.9.0.2",
+  "autoflake==2.1.1"
 ]
 
 [tool.hatch.envs.code-quality.scripts]
 types = "mypy deepset_cloud_sdk tests"
 format = "black deepset_cloud_sdk tests --check"
 format-fix = "black deepset_cloud_sdk tests"
 lint = "pylint deepset_cloud_sdk"
 sort = "isort --check --profile black ."
+sort-fix = "isort --profile black ."
 hooks = "pre-commit install"
 docstrings = "pydocstyle deepset_cloud_sdk"
+flake = "autoflake --remove-all-unused-imports --remove-duplicate-keys --remove-unused-variables -v -r ./deepset_cloud_sdk"
+all = "hatch run types && hatch run format-fix && hatch run lint && hatch run sort && hatch run docstrings && hatch run flake"
 
 [tool.hatch.envs.tools]
 detached = false
 # Please keep these aligned with the versions defined in .pre-commit-config.yaml
 dependencies = [
   "pip-tools==6.13.0",
 ]
@@ -130,27 +142,27 @@
 warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 [tool.pylint.'MESSAGES CONTROL']
-max-line-length=120
+max-line-length=150
 disable = [
   "fixme",
   "c-extension-no-member",
   "wrong-spelling-in-comment",
   "wrong-spelling-in-docstring",
   "missing-module-docstring"
   ]
 [tool.pylint.'DESIGN']
 max-args=9
 
 [tool.pylint.'SIMILARITIES']
-min-similarity-lines=6
+min-similarity-lines=10
 
 [tool.pylint.'BASIC']
 good-names=[
   "i",
   "k",
   "v",
   "_",
```

### Comparing `deepset_cloud_sdk-0.0.9/PKG-INFO` & `deepset_cloud_sdk-0.41/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,66 @@
-Metadata-Version: 2.1
-Name: deepset-cloud-sdk
-Version: 0.0.9
-Summary: deepset cloud SDK
-Project-URL: Documentation, https://github.com/deepset-ai/deepset-cloud-sdk#readme
-Project-URL: Issues, https://github.com/deepset-ai/deepset-cloud-sdk/issues
-Project-URL: Source, https://github.com/deepset-ai/deepset-cloud-sdk
-Author-email: deepset <rohan.janjua@deepset.ai>
-License-Expression: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Requires-Dist: aiohttp==3.8.4
-Requires-Dist: httpx==0.24.0
-Requires-Dist: progress==1.6
-Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: structlog==23.1.0
-Requires-Dist: tabulate==0.9.0
-Requires-Dist: tenacity==8.2.2
-Requires-Dist: typer==0.9.0
-Description-Content-Type: text/markdown
-
 <p align="center">
   <a href="https://cloud.deepset.ai/"><img src="/assets/logo.png"  alt="deepset Cloud SDK"></a>
 </p>
 
+[![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/tree/python-coverage-comment-action-data)
 [![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-integration.yml)
 [![Deploy PyPi](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml)
 [![Compliance Checks](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml)
 
-The deepset Cloud SDK is an open source software development kit that provides convenient access and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks.
+The deepset Cloud SDK is an open source software development kit that provides convenient access to and integration with deepset Cloud, a powerful cloud offering for various natural language processing (NLP) tasks.
 This README provides an overview of the SDK and its features, and information on contributing to the project and exploring related resources.
 
+- [Official SDK Docs](https://sdk.cloud.deepset.ai)
+- [deepset Cloud Documentation](https://docs.cloud.deepset.ai/)
+- Tutorials: 
+    - [Uploading with CLI](https://docs.cloud.deepset.ai/docs/tutorial-uploading-files-with-cli) 
+    - [Uploading with Python Methods](https://docs.cloud.deepset.ai/docs/tutorial-uploading-files-with-python-methods)
+
 # Supported Features
+
+In its current shape, the SDK offers a suite of tools for seamless data upload to deepset Cloud. 
 The following examples demonstrate how to use the deepset Cloud SDK to interact with deepset Cloud using Python.
-You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](/examples/cli/README.md).
-- [SDK - Upload datasets](/examples/sdk/upload.py)
-- [CLI - Upload datasets](/examples/cli/README.md)
+You can use the deepset Cloud SDK in the command line as well. For more information, see the [CLI documentation](docs/examples/cli/README.md).
+
+-   [SDK Examples - Upload datasets](/docs/examples/sdk/upload.py)
+-   [CLI Examples - Upload datasets](/docs/examples/cli/README.md)
 
 ## Installation
-The deepset Cloud SDK is available on PyPI and you can install it using pip:
+The deepset Cloud SDK is available on [PyPI](https://pypi.org/project/deepset-cloud-sdk/) and you can install it using pip:
 ```bash
 pip install deepset-cloud-sdk
 ```
 
 After installing the deepset Cloud SDK, you can use it to interact with deepset Cloud. It comes with a command line interface (CLI), that you can use by calling:
 ```bash
-deepset-cloud-cli --help
+deepset-cloud --help
 ```
 
+<p align="center">
+  <a href="https://cloud.deepset.ai/"><img src="/assets/cli.gif"  alt="deepset Cloud CLI"></a>
+</p>
+
 ### Development Installation
 To install the deepset Cloud SDK for development, clone the repository and install the package in editable mode:
 ```bash
 pip install hatch==1.7.0
 hatch build
 ```
 
+Instead of calling the CLI from the build package, you can call it directly from the source code:
+```bash
+python3 -m deepset_cloud_sdk.cli --help
+```
+
 ## Contributing
 We welcome contributions from the open source community to enhance the deepset Cloud SDK. If you would like to contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines and instructions on how to get started.
 We appreciate your contributions, whether they're bug fixes, new features, or documentation improvements.
 
 
 ---
 
-## Interested in deepset Cloud?
-If you are interested in exploring deepset Cloud, visit cloud.deepset.ai.
-deepset Cloud provides a range of NLP capabilities and services to help you build and deploy powerful
-natural language processing applications.
-
 ## Interested in Haystack?
 deepset Cloud is powered by Haystack, an open source framework for building end-to-end NLP pipelines.
- - [Project website](https://haystack.deepset.ai/)
- - [GitHub repository](https://github.com/deepset-ai/haystack)
+
+ -    [Project website](https://haystack.deepset.ai/)
+ -    [GitHub repository](https://github.com/deepset-ai/haystack)
```

#### html2text {}

```diff
@@ -1,53 +1,47 @@
-Metadata-Version: 2.1 Name: deepset-cloud-sdk Version: 0.0.9 Summary: deepset
-cloud SDK Project-URL: Documentation, https://github.com/deepset-ai/deepset-
-cloud-sdk#readme Project-URL: Issues, https://github.com/deepset-ai/deepset-
-cloud-sdk/issues Project-URL: Source, https://github.com/deepset-ai/deepset-
-cloud-sdk Author-email: deepset
-deepset.ai> License-Expression: MIT Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8 Requires-Dist: aiohttp==3.8.4 Requires-Dist:
-httpx==0.24.0 Requires-Dist: progress==1.6 Requires-Dist: python-dotenv==1.0.0
-Requires-Dist: structlog==23.1.0 Requires-Dist: tabulate==0.9.0 Requires-Dist:
-tenacity==8.2.2 Requires-Dist: typer==0.9.0 Description-Content-Type: text/
-markdown
                               _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _S_D_K_]
-[![Tests](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
-continuous-integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-
-cloud-sdk/actions/workflows/continuous-integration.yml) [![Deploy PyPi](https:/
-/github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
+[![Coverage badge](https://github.com/deepset-ai/deepset-cloud-sdk/raw/python-
+coverage-comment-action-data/badge.svg)](https://github.com/deepset-ai/deepset-
+cloud-sdk/tree/python-coverage-comment-action-data) [![Tests](https://
+github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/continuous-
+integration.yml/badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/
+actions/workflows/continuous-integration.yml) [![Deploy PyPi](https://
+github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/deploy-prod.yml/
 badge.svg)](https://github.com/deepset-ai/deepset-cloud-sdk/actions/workflows/
 deploy-prod.yml) [![Compliance Checks](https://github.com/deepset-ai/deepset-
 cloud-sdk/actions/workflows/compliance.yml/badge.svg)](https://github.com/
 deepset-ai/deepset-cloud-sdk/actions/workflows/compliance.yml) The deepset
 Cloud SDK is an open source software development kit that provides convenient
-access and integration with deepset Cloud, a powerful cloud offering for
+access to and integration with deepset Cloud, a powerful cloud offering for
 various natural language processing (NLP) tasks. This README provides an
 overview of the SDK and its features, and information on contributing to the
-project and exploring related resources. # Supported Features The following
+project and exploring related resources. - [Official SDK Docs](https://
+sdk.cloud.deepset.ai) - [deepset Cloud Documentation](https://
+docs.cloud.deepset.ai/) - Tutorials: - [Uploading with CLI](https://
+docs.cloud.deepset.ai/docs/tutorial-uploading-files-with-cli) - [Uploading with
+Python Methods](https://docs.cloud.deepset.ai/docs/tutorial-uploading-files-
+with-python-methods) # Supported Features In its current shape, the SDK offers
+a suite of tools for seamless data upload to deepset Cloud. The following
 examples demonstrate how to use the deepset Cloud SDK to interact with deepset
 Cloud using Python. You can use the deepset Cloud SDK in the command line as
-well. For more information, see the [CLI documentation](/examples/cli/
-README.md). - [SDK - Upload datasets](/examples/sdk/upload.py) - [CLI - Upload
-datasets](/examples/cli/README.md) ## Installation The deepset Cloud SDK is
-available on PyPI and you can install it using pip: ```bash pip install
-deepset-cloud-sdk ``` After installing the deepset Cloud SDK, you can use it to
+well. For more information, see the [CLI documentation](docs/examples/cli/
+README.md). - [SDK Examples - Upload datasets](/docs/examples/sdk/upload.py) -
+[CLI Examples - Upload datasets](/docs/examples/cli/README.md) ## Installation
+The deepset Cloud SDK is available on [PyPI](https://pypi.org/project/deepset-
+cloud-sdk/) and you can install it using pip: ```bash pip install deepset-
+cloud-sdk ``` After installing the deepset Cloud SDK, you can use it to
 interact with deepset Cloud. It comes with a command line interface (CLI), that
-you can use by calling: ```bash deepset-cloud-cli --help ``` ### Development
-Installation To install the deepset Cloud SDK for development, clone the
-repository and install the package in editable mode: ```bash pip install
-hatch==1.7.0 hatch build ``` ## Contributing We welcome contributions from the
-open source community to enhance the deepset Cloud SDK. If you would like to
-contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines
-and instructions on how to get started. We appreciate your contributions,
-whether they're bug fixes, new features, or documentation improvements. --- ##
-Interested in deepset Cloud? If you are interested in exploring deepset Cloud,
-visit cloud.deepset.ai. deepset Cloud provides a range of NLP capabilities and
-services to help you build and deploy powerful natural language processing
-applications. ## Interested in Haystack? deepset Cloud is powered by Haystack,
-an open source framework for building end-to-end NLP pipelines. - [Project
-website](https://haystack.deepset.ai/) - [GitHub repository](https://
+you can use by calling: ```bash deepset-cloud --help ```
+                              _[_d_e_e_p_s_e_t_ _C_l_o_u_d_ _C_L_I_]
+### Development Installation To install the deepset Cloud SDK for development,
+clone the repository and install the package in editable mode: ```bash pip
+install hatch==1.7.0 hatch build ``` Instead of calling the CLI from the build
+package, you can call it directly from the source code: ```bash python3 -
+m deepset_cloud_sdk.cli --help ``` ## Contributing We welcome contributions
+from the open source community to enhance the deepset Cloud SDK. If you would
+like to contribute, have a look at [CONTRIBUTING.md](CONTRIBUTING.md) for
+guidelines and instructions on how to get started. We appreciate your
+contributions, whether they're bug fixes, new features, or documentation
+improvements. --- ## Interested in Haystack? deepset Cloud is powered by
+Haystack, an open source framework for building end-to-end NLP pipelines. -
+[Project website](https://haystack.deepset.ai/) - [GitHub repository](https://
 github.com/deepset-ai/haystack)
```

