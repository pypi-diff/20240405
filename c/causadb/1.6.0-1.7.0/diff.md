# Comparing `tmp/causadb-1.6.0.tar.gz` & `tmp/causadb-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.6.0.tar", max compression
+gzip compressed data, was "causadb-1.7.0.tar", max compression
```

## Comparing `causadb-1.6.0.tar` & `causadb-1.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      642 2024-04-04 14:03:28.434420 causadb-1.6.0/README.md
--rw-r--r--   0        0        0      115 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-04 14:03:46.210371 causadb-1.6.0/causadb/__version__.py
--rw-r--r--   0        0        0     5189 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/examples/heating.py
--rw-r--r--   0        0        0    14837 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/model.py
--rw-r--r--   0        0        0      215 2024-04-04 14:03:28.434420 causadb-1.6.0/causadb/utils.py
--rw-r--r--   0        0        0      695 2024-04-04 14:03:45.478371 causadb-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-04 19:10:01.661629 causadb-1.7.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 19:10:21.978006 causadb-1.7.0/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15066 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/model.py
+-rw-r--r--   0        0        0      215 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/utils.py
+-rw-r--r--   0        0        0      715 2024-04-04 19:10:21.145991 causadb-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 causadb-1.7.0/PKG-INFO
```

### Comparing `causadb-1.6.0/README.md` & `causadb-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/causadb.py` & `causadb-1.7.0/causadb/causadb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import os
 import toml
+from pydantic import validate_call
 from .data import Data
 from .model import Model
 from .utils import get_causadb_url, set_causadb_url
 
 
 class CausaDB:
     """CausaDB client class to interact with the CausaDB system.
@@ -51,14 +52,15 @@
 
         token_secret = config \
             .get("default", {}) \
             .get("token_secret", None)
 
         return token_secret
 
+    @validate_call
     def set_token(self, token: str) -> None:
         """Set the token for the CausaDB client.
 
         Args:
             token (str): Token secret provided by CausaDB.
 
         Raises:
@@ -74,36 +76,39 @@
 
         # If the response is successful, set the tokens
         if response.status_code == 200:
             self.token = token
         else:
             raise Exception("Invalid token")
 
+    @validate_call
     def create_model(self, model_name: str) -> Model:
         """Create a model and add it to the CausaDB system.
 
         Args:
             model_name (str): The name of the model.
 
         Returns:
             Model: The model object.
         """
         return Model(model_name, self)
 
+    @validate_call
     def add_data(self, data_name: str) -> Data:
         """Add data to the CausaDB system.
 
         Args:
             data_name (str): The name of the data.
 
         Returns:
             Data: The data object.
         """
         return Data(data_name, self)
 
+    @validate_call
     def get_model(self, model_name: str) -> Model:
         """Get a model by name.
 
         Args:
             model_name (str): The name of the model.
 
         Returns:
@@ -119,14 +124,15 @@
             raise Exception(f"CausaDB server request failed: {e}")
 
         # If the model exists, return it
         model = Model(model_name, self)
 
         return model
 
+    @validate_call
     def list_models(self) -> list[Model]:
         """List all models.
 
         Returns:
             list[Model]: A list of model objects.
         """
         headers = {"token": self.token}
@@ -141,14 +147,15 @@
         model_list = []
         for model_spec in response.get("models", []):
             model = Model(model_spec["name"], self)
             model_list.append(model)
 
         return model_list
 
+    @validate_call
     def get_data(self, data_name: str) -> Data:
         """Get a data by name.
 
         Args:
             data_name (str): The name of the data.
 
         Returns:
```

### Comparing `causadb-1.6.0/causadb/cli/account.py` & `causadb-1.7.0/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/cli/data.py` & `causadb-1.7.0/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/cli/main.py` & `causadb-1.7.0/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/cli/models.py` & `causadb-1.7.0/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/cli/utils.py` & `causadb-1.7.0/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/data.py` & `causadb-1.7.0/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/examples/heating.py` & `causadb-1.7.0/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.6.0/causadb/model.py` & `causadb-1.7.0/causadb/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import time
 import pandas as pd
 import numpy as np
 from typing import Union
+from pydantic import validate_call
 
 from .utils import get_causadb_url
 
 
 class Model:
     def __init__(self, model_name: str, client: "CausaDB") -> None:
         """Initializes the Model class.
@@ -41,14 +42,15 @@
             requests.delete(
                 f"{get_causadb_url()}/models/{self.model_name}",
                 headers=headers,
             )
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
+    @validate_call
     def set_nodes(self, nodes: list[str]) -> None:
         """Set the nodes of the model.
 
         Args:
             nodes (list[str]): A list of node names.
 
         Example:
@@ -81,14 +83,15 @@
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
         return response["details"]["config"]["nodes"]
 
+    @validate_call
     def set_edges(self, edges: list[tuple[str, str]]) -> None:
         """Set the edges of the model.
 
         Args:
             edges (list[tuple[str, str]]): A list of tuples representing edges.
 
         Example:
@@ -126,14 +129,15 @@
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
         edges = response["details"]["config"]["edges"]
         # Convert the edges to a list of tuples
         return [(edge[0], edge[1]) for edge in edges]
 
+    @validate_call
     def set_node_types(self, node_types: dict) -> None:
         """Set the node types of the model.
 
         Args:
             node_types (dict): A dictionary of node types.
 
         Example:
@@ -151,14 +155,15 @@
             raise Exception(f"CausaDB server request failed: {e}")
 
         self.config = response["details"]["config"]
         self.config["node_types"] = node_types
 
         self._update()
 
+    @validate_call
     def get_node_types(self) -> dict:
         """Get the node types of the model.
 
         Returns:
             dict: A dictionary of node types.
         """
         headers = {"token": self.client.token}
@@ -168,14 +173,15 @@
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
         return response["details"]["config"]["node_types"]
 
+    @validate_call
     def attach(self, data_name: str) -> None:
         """Attach data to the model.
 
         Args:
             data_name (str): The name of the data to attach.
         """
         headers = {"token": self.client.token}
@@ -184,14 +190,15 @@
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/attach/{data_name}",
                 headers=headers
             ).json()
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
+    @validate_call
     def detach(self, data_name: str) -> None:
         """Detach data from the model.
 
         Args:
             data_name (str): The name of the data to detach.
         """
         headers = {"token": self.client.token}
@@ -200,14 +207,15 @@
             response = requests.delete(
                 f"{get_causadb_url()}/models/{self.model_name}/detach",
                 headers=headers
             ).json()
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
+    @validate_call
     def train(self, data_name: str = None, wait: bool = True, poll_interval: float = 0.2, poll_limit: float = 30.0, verbose: bool = False, progress_interval: float = 1.0) -> None:
         """Train the model.
 
         Args:
             wait (bool): Whether to wait for the model to finish training.
             poll_interval (float): The interval at which to poll the server for the model status.
             poll_limit (float): The maximum time to wait for the model to finish training.
@@ -273,14 +281,15 @@
         except Exception as e:
             raise Exception(f"CausaDB server request failed: {e}")
 
         model_status = response["details"]["status"]
 
         return model_status
 
+    @validate_call
     def simulate_actions(self, actions: dict, fixed: dict = {}, interval: float = 0.9, observation_noise: bool = False) -> dict:
         """Simulate an action on the model.
 
         Args:
             actions (dict): A dictionary representing the actions.
             fixed (dict): A dictionary representing the fixed nodes.
             interval (float): The interval at which to simulate the action.
@@ -318,15 +327,16 @@
                 "median": pd.DataFrame.from_dict(outcome["median"]),
                 "lower": pd.DataFrame.from_dict(outcome["lower"]),
                 "upper": pd.DataFrame.from_dict(outcome["upper"])
             }
 
         raise Exception("CausaDB server request failed")
 
-    def causal_effects(self, actions: Union[str, dict[str, tuple[np.ndarray, np.ndarray]]], fixed: dict[str, np.ndarray] = None, interval: float = 0.90, observation_noise=False) -> pd.DataFrame:
+    @validate_call
+    def causal_effects(self, actions: Union[str, dict[str, tuple[float, float]]], fixed: dict[str, float] = None, interval: float = 0.90, observation_noise=False) -> pd.DataFrame:
         """ Get the causal effects of actions on the model.
 
         Args:
             actions (Union[str, dict[str, tuple[np.ndarray, np.ndarray]]]): A dictionary representing the actions.
             fixed (dict): A dictionary representing the fixed nodes.
             interval (float): The interval at which to simulate the action.
             observation_noise (bool): Whether to include observation noise.
@@ -359,14 +369,15 @@
             raise Exception(f"CausaDB server request failed: {e}")
 
         if "outcome" in response:
             return pd.DataFrame.from_dict(response["outcome"])
 
         raise Exception("CausaDB server request failed")
 
+    @validate_call
     def find_best_actions(self, targets: dict[str, float], actionable: list[str], fixed: dict[str, float] = {}) -> dict:
         """Get the optimal actions for a given set of target outcomes.
 
         Args:
             targets (dict[str, float]): A dictionary representing the target outcomes.
             actionable (list[str]): A list of actionable nodes.
             fixed (dict[str, float]): A dictionary representing the fixed nodes.
@@ -398,14 +409,15 @@
             raise Exception(f"CausaDB server request failed: {e}")
 
         if "best_actions" in response:
             return pd.DataFrame.from_dict(response["best_actions"])
 
         raise Exception("CausaDB server request failed")
 
+    @validate_call
     def causal_attributions(self, outcome: str, normalise: bool = False) -> pd.DataFrame:
         """Get the causal attributions for an outcome.
 
         Args:
             outcome (str): The outcome node.
             normalise (bool): Whether to normalise the causal attributions.
```

### Comparing `causadb-1.6.0/pyproject.toml` & `causadb-1.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.6.0"
+version = "1.7.0"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
 
@@ -19,14 +19,15 @@
 rich = "^13.7.0"
 pandas = "^2.2.0"
 marko = "^2.0.2"
 setuptools = "^69.0.3"
 python-dotenv = "^1.0.1"
 pyarrow = "^15.0.0"
 tqdm = "^4.66.2"
+pydantic = "^2.6.4"
 
 [tool.poetry.group.dev.dependencies]
 invoke = "^2.2.0"
 pydoc-markdown = "^4.8.2"
 pytest = "^7.4.4"
 
 [build-system]
```

### Comparing `causadb-1.6.0/PKG-INFO` & `causadb-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.6.0
+Version: 1.7.0
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: marko (>=2.0.2,<3.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
```

