# Comparing `tmp/poetry_aws_plugin-0.1.2.tar.gz` & `tmp/poetry_aws_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.2.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.3.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.2.tar` & `poetry_aws_plugin-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-04 16:43:29.996219 poetry_aws_plugin-0.1.2/LICENSE
--rw-r--r--   0        0        0     2629 2024-04-04 16:49:21.086127 poetry_aws_plugin-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-04 16:43:29.996219 poetry_aws_plugin-0.1.2/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6411 2024-04-04 16:52:36.096094 poetry_aws_plugin-0.1.2/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-04 16:49:47.766122 poetry_aws_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2634 2024-04-05 17:44:43.428417 poetry_aws_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.3/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     6487 2024-04-05 17:45:40.640420 poetry_aws_plugin-0.1.3/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-05 17:45:13.176419 poetry_aws_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.3/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.2/LICENSE` & `poetry_aws_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.2/README.md` & `poetry_aws_plugin-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run `codeartifact.GetAuthorizationToken`.
 
-**If you are use IAM roles, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
+**To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
 
 For example:
 
 ```bash
 export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'
 poetry install
 ```
```

### Comparing `poetry_aws_plugin-0.1.2/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.3/poetry_aws_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,18 @@
         url: str,
         raise_for_status: bool = True,
         **kwargs: Any,
     ) -> requests.Response:
         response = request(self, method=method, url=url, raise_for_status=False, **kwargs)
 
         if is_retryable(response):
-            io.write_line("\nFailed to get authorization for CodeArtifact\n")
+            io.write_line(
+                "\nFailed to get authorization for CodeArtifact\n",
+                verbosity=Verbosity.VERBOSE,
+            )
 
             match = re.match(CODEARTIFACT_URL_REGEX, response.url)
             domain, domain_owner = match.groups()
 
             auth_token = get_auth_token(domain, domain_owner)
             if not auth_token:
                 raise PoetryException(RETRY_ERROR_MESSAGE)
```

### Comparing `poetry_aws_plugin-0.1.2/pyproject.toml` & `poetry_aws_plugin-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.2"
+version = "0.1.3"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.2/PKG-INFO` & `poetry_aws_plugin-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -50,15 +50,15 @@
 When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run `codeartifact.GetAuthorizationToken`.
 
-**If you are use IAM roles, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
+**To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
 
 For example:
 
 ```bash
 export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'
 poetry install
 ```
```

