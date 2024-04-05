# Comparing `tmp/guardian_client-0.2.1.tar.gz` & `tmp/guardian_client-0.2.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardian_client-0.2.1.tar", max compression
+gzip compressed data, was "guardian_client-0.2.1.dev0.tar", max compression
```

## Comparing `guardian_client-0.2.1.tar` & `guardian_client-0.2.1.dev0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5762 2024-03-26 17:06:59.766705 guardian_client-0.2.1/README.md
--rw-r--r--   0        0        0      105 2024-03-26 17:06:59.766705 guardian_client-0.2.1/guardian_client/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 17:07:19.386768 guardian_client-0.2.1/guardian_client/_version.py
--rw-r--r--   0        0        0        0 2024-03-26 17:06:59.766705 guardian_client-0.2.1/guardian_client/python/__init__.py
--rw-r--r--   0        0        0     7115 2024-03-26 17:06:59.766705 guardian_client-0.2.1/guardian_client/python/api.py
--rw-r--r--   0        0        0     4644 2024-03-26 17:06:59.766705 guardian_client-0.2.1/guardian_client/python/credentials.py
--rw-r--r--   0        0        0     4262 2024-03-26 17:06:59.766705 guardian_client-0.2.1/guardian_client/python/guardian.py
--rw-r--r--   0        0        0      752 2024-03-26 17:07:19.826769 guardian_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 guardian_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4628 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/README.md
+-rw-r--r--   0        0        0      105 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-05 21:32:32.135271 guardian_client-0.2.1.dev0/guardian_client/_version.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/__init__.py
+-rw-r--r--   0        0        0     5384 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/api.py
+-rw-r--r--   0        0        0     4644 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/credentials.py
+-rw-r--r--   0        0        0     3949 2024-04-05 21:32:16.655185 guardian_client-0.2.1.dev0/guardian_client/python/guardian.py
+-rw-r--r--   0        0        0      757 2024-04-05 21:32:32.479273 guardian_client-0.2.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 guardian_client-0.2.1.dev0/PKG-INFO
```

### Comparing `guardian_client-0.2.1/README.md` & `guardian_client-0.2.1.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: guardian-client
+Version: 0.2.1.dev0
+Summary: Python SDK for Protect AI Guardian
+License: Apache-2.0
+Author: ProtectAI
+Author-email: community@protectai.com
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 # Protect AI Guardian Client
 
 A CLI and SDK client for Protect AI's Guardian service. You can find more information about this service here: https://protectai.com/guardian
 
 # Using CLI
 
 The Guardian Scanner's CLI offers a convenient way of submitting a scan and receiving the scan report along with an exit code that can be used to block model deployment depending upon the discovered vulnerabilities.
@@ -31,53 +49,50 @@
 ## Running Your Scans
 
 That's it!. Now you should be all set to start scanning your models.
 
 ``` shell
 
 guardian-client <base_url> <model_uri> \
-       [--threshold <threshold>] \
        [--block-on-errors] \
        [--log-level <log-level>] \
        [--silent] || echo $?
 ```
 
 ### Arguments
 
 - `base_url` The API URL (required)
 
 - `model_uri` The Path where the model is stored e.g. S3 bucket (required)
 
-- `--threshold` The minimum threshold at which a model should be blocked. Take following values: low, medium, high, critical. Default is critical
-
 - `--block-on-errors` A boolean flag indicating the error in scanning should also lead to a block. These errors are only specific to model scanning.
 
 - `--log-level` Can be set to any of the following: error, info, or debug
 
 - `--silent` Disable all logging / reporting
 
 - `--report-only` Print out the scan report and skip evaluating it for blocking.
 
 - `--poll-interval-secs` The interval in seconds to wait before polling the server for scan status. Default is 5.
 
 ### Exit Codes
 The CLI returns following exit codes that can be used by the downstream applications to block a deployment.
 
-- **0** Successful scan without issues at or above the threshold (default is CRITICAL)
+- **0** Successful scan without violating any of your organization's policies
 
-- **1** Successful scan with issues at or above the threshold (default is CRITICAL)
+- **1** Successful scan with issues violating your organization's policies
 
 - **2** Scan failed for any reason
 
 ## Examples
 
-### To get a block decision for model vulnerability at or higher than "MEDIUM"
+### To get a block decision for a model in S3
 
 ``` shell
-guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --threshold MEDIUM || echo $?
+guardian-client https://protectai.dev/guardian s3://a-bucket/path/ || echo $?
 ```
 ### To only see the report from scanning the model.
 
 ```
 guardian-client https://protectai.dev/guardian s3://a-bucket/path/ --report-only
 
 ```
@@ -99,23 +114,21 @@
 # Initiate the client
 guardian = GuardianAPIClient(base_url=base_url)
 
 # Scan the model
 response = guardian.scan(model_uri=model_uri)
 
 
-# Evaluate the scan response against a threshold
+# Retrieve the pass/fail decision from Guardian
 assert response.get("http_status_code") == 200
 assert response.get("scan_status_json") != None
-assert response.get("scan_status_json").get("status") == "FINISHED"
-
-reason, should_block = guardian.evaluate(response.get("scan_status_json"))
+assert response.get("scan_status_json").get("aggregate_eval_outcome") != "ERROR"
   
-if should_block:
-  print(f"Model {model_uri} was blocked with reason: {reason}")
+if response.get("scan_status_json").get("aggregate_eval_outcome") == "FAIL":
+  print(f"Model {model_uri} was blocked because it failed your organization's security policies")
 ```
 
 ## Reference
 
 ### Class GuardianAPIClient
 
 ``` python
@@ -157,30 +170,7 @@
           dict: A dictionary containing the HTTP status code and the scan status JSON.
                 If an error occurs during the scan submission or polling, the dictionary
                 will also contain the error details.
 
       """
 ```
 
-#### GuardianAPIClient.evaluate
-``` python
-  def evaluate(
-      self,
-      status_json: Dict[str, Any],
-      threshold: str = "CRITICAL",
-      block_on_scan_errors: bool = False,
-  ) -> Tuple[str, bool]:
-      """
-      Evaluates the status of a scan based on the provided status JSON.
-
-      Args:
-          status_json (object): The status JSON object containing scan information obtained from scan method.
-          threshold (str, optional): The threshold level to consider for blocking. Defaults to "CRITICAL".
-          block_on_scan_errors (bool, optional): Whether to block if there are errors in scanning. Defaults to False.
-
-      Returns:
-          Tuple[str, bool]: A tuple containing the evaluation result message and a boolean indicating if blocking is required.
-
-          Raises:
-              ValueError: If the threshold is not one of "LOW", "MEDIUM", "HIGH", or "CRITICAL".
-      """
-```
```

### Comparing `guardian_client-0.2.1/guardian_client/python/credentials.py` & `guardian_client-0.2.1.dev0/guardian_client/python/credentials.py`

 * *Files identical despite different names*

### Comparing `guardian_client-0.2.1/pyproject.toml` & `guardian_client-0.2.1.dev0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guardian-client"
-version = "0.2.1"
+version = "0.2.1.dev0"
 license = "Apache License 2.0"
 description = "Python SDK for Protect AI Guardian"
 authors = ["ProtectAI <community@protectai.com>"]
 readme = "README.md"
 packages = [
     { include = "guardian_client" },
 ]
```

