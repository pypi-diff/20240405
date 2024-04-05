# Comparing `tmp/aws_lambda_env_modeler-1.0.6.tar.gz` & `tmp/aws_lambda_env_modeler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_env_modeler-1.0.6.tar", max compression
+gzip compressed data, was "aws_lambda_env_modeler-1.0.7.tar", max compression
```

## Comparing `aws_lambda_env_modeler-1.0.6.tar` & `aws_lambda_env_modeler-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/LICENSE
--rw-r--r--   0        0        0     4917 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/README.md
--rw-r--r--   0        0        0      281 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/aws_lambda_env_modeler/__init__.py
--rw-r--r--   0        0        0     2396 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/aws_lambda_env_modeler/modeler.py
--rw-r--r--   0        0        0        0 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/aws_lambda_env_modeler/py.typed
--rw-r--r--   0        0        0      136 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/aws_lambda_env_modeler/types.py
--rw-r--r--   0        0        0     2852 2023-12-15 06:43:38.201116 aws_lambda_env_modeler-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     6270 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/LICENSE
+-rw-r--r--   0        0        0     6919 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/README.md
+-rw-r--r--   0        0        0      410 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/__init__.py
+-rw-r--r--   0        0        0     2428 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/modeler.py
+-rw-r--r--   0        0        0     1275 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/modeler_impl.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/py.typed
+-rw-r--r--   0        0        0      276 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/types.py
+-rw-r--r--   0        0        0     2857 2024-04-05 06:44:56.765020 aws_lambda_env_modeler-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8272 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.7/PKG-INFO
```

### Comparing `aws_lambda_env_modeler-1.0.6/LICENSE` & `aws_lambda_env_modeler-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.6/README.md` & `aws_lambda_env_modeler-1.0.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -69,15 +69,19 @@
     DB_PORT: int
     DB_USER: str
     DB_PASS: str
     FLAG_X:  bool
     API_URL: HttpUrl
 ```
 
-You must first use the `@init_environment_variables` decorator to automatically validate and initialize the environment variables before executing a function:
+Before executing a function, you must use the `@init_environment_variables` decorator to validate and initialize the environment variables automatically.
+
+The decorator guarantees that the function will run with the correct variable configuration.
+
+Then, you can fetch the environment variables using the global getter function, 'get_environment_variables,' and use them just like a data class. At this point, they are parsed and validated.
 
 ```python
 from aws_lambda_env_modeler import init_environment_variables
 
 @init_environment_variables(MyEnvVariables)
 def my_handler_entry_function(event, context):
     # At this point, environment variables are already validated and initialized
@@ -89,14 +93,59 @@
 ```python
 from aws_lambda_env_modeler import get_environment_variables
 
 env_vars = get_environment_variables(MyEnvVariables)
 print(env_vars.DB_HOST)
 ```
 
+## Disabling Cache for Testing
+
+By default, the modeler uses cache - the parsed model is cached for performance improvement for multiple 'get' calls.
+
+In some cases, such as during testing, you may want to turn off the cache. You can do this by setting the `LAMBDA_ENV_MODELER_DISABLE_CACHE` environment variable to 'True.'
+
+This is especially useful in tests where you want to run multiple tests concurrently, each with a different set of environment variables.
+
+Here's an example of how you can use this in a pytest test:
+
+```python
+import json
+from http import HTTPStatus
+from typing import Any, Dict
+from unittest.mock import patch
+
+from pydantic import BaseModel
+from typing_extensions import Literal
+
+from aws_lambda_env_modeler import LAMBDA_ENV_MODELER_DISABLE_CACHE, get_environment_variables, init_environment_variables
+
+
+class MyHandlerEnvVars(BaseModel):
+    LOG_LEVEL: Literal['DEBUG', 'INFO', 'ERROR', 'CRITICAL', 'WARNING', 'EXCEPTION']
+
+
+@init_environment_variables(model=MyHandlerEnvVars)
+def my_handler(event: Dict[str, Any], context) -> Dict[str, Any]:
+    env_vars = get_environment_variables(model=MyHandlerEnvVars)  # noqa: F841
+    # can access directly env_vars.LOG_LEVEL as dataclass
+    return {
+        'statusCode': HTTPStatus.OK,
+        'headers': {'Content-Type': 'application/json'},
+        'body': json.dumps({'message': 'success'}),
+    }
+
+
+@patch.dict('os.environ', {LAMBDA_ENV_MODELER_DISABLE_CACHE: 'true', 'LOG_LEVEL': 'DEBUG'})
+def test_my_handler():
+    response = my_handler({}, None)
+    assert response['statusCode'] == HTTPStatus.OK
+    assert response['headers'] == {'Content-Type': 'application/json'}
+    assert json.loads(response['body']) == {'message': 'success'}
+```
+
 ## Code Contributions
 Code contributions are welcomed. Read this [guide.](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/CONTRIBUTING.md)
 
 ## Code of Conduct
 Read our code of conduct [here.](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/CODE_OF_CONDUCT.md)
 
 ## Connect
```

### Comparing `aws_lambda_env_modeler-1.0.6/aws_lambda_env_modeler/modeler.py` & `aws_lambda_env_modeler-1.0.7/aws_lambda_env_modeler/modeler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,50 @@
-import os
-from functools import lru_cache, wraps
+from functools import wraps
 from typing import Any, Callable, Dict, Type
 
+from aws_lambda_env_modeler.modeler_impl import __get_environment_variables_impl
 from aws_lambda_env_modeler.types import Model
 
 
-def get_environment_variables(model: Type[Model]) -> Model:
-    """
-    This function receives a model of type Model, uses it to validate the environment variables, and returns the
-    validated model.
-
-    Args:
-        model (Type[Model]): A Pydantic model that defines the structure and types of the expected environment variables.
-
-    Returns:
-        Model: An instance of the provided model filled with the values of the validated environment variables.
-    """
-    return __parse_model(model)
-
-
 def init_environment_variables(model: Type[Model]):
     """
-    A decorator function for AWS Lambda handler functions that initializes environment variables based on the given Pydantic model before executing
-    the decorated function. The decorator validates the environment variables according to the model structure before
-    running the handler.
+    A decorator for AWS Lambda handler functions. It initializes and validates environment variables based on the provided Pydantic model before the execution of the decorated function.
+    It uses LRU Cache by model class type to optimize parsing time. Cache can be disabled by setting the environment variable 'LAMBDA_ENV_MODELER_DISABLE_CACHE' to FALSE (default: cache is enabled)
 
     Args:
-        model (Type[Model]): A Pydantic model that defines the structure and types of the expected environment variables.
+        model (Type[Model]): A Pydantic model that outlines the structure and types of the expected environment variables.
 
     Returns:
-        Callable: A decorated function that first initializes the environment variables and then runs the function.
+        Callable: A decorated function that first initializes and validates the environment variables, then executes the original function.
+
+    Raises:
+        ValueError: If the environment variables do not align with the model's structure or fail validation.
     """
 
     def decorator(lambda_handler_function: Callable):
         @wraps(lambda_handler_function)
         def wrapper(event: Dict[str, Any], context, **kwargs):
-            __parse_model(model)
+            # Initialize and validate environment variables before executing the lambda handler function
+            __get_environment_variables_impl(model)
             return lambda_handler_function(event, context, **kwargs)
 
         return wrapper
 
     return decorator
 
 
-@lru_cache
-def __parse_model(model: Type[Model]) -> Model:
+def get_environment_variables(model: Type[Model]) -> Model:
     """
-    A helper function to validate and parse environment variables based on a given Pydantic model. This function is
-    also cached to improve performance in successive calls.
+    Retrieves and validates environment variables based on the provided Pydantic model.
+    It uses LRU Cache by model class type to optimize parsing time. Cache can be disabled by setting the environment variable 'LAMBDA_ENV_MODELER_DISABLE_CACHE' to FALSE (default: cache is enabled)
+    It's recommended to use anywhere in the function's after init_environment_variables decorator was used on the handler function.
 
     Args:
-        model (Type[Model]): A Pydantic model that defines the structure and types of the expected environment variables.
+        model (Type[Model]): A Pydantic model that outlines the structure and types of the expected environment variables.
 
     Returns:
-        Model: An instance of the provided model filled with the values of the validated environment variables.
+        Model: An instance of the provided model populated with the values of the validated environment variables.
 
     Raises:
-        ValueError: If the environment variables do not match the structure of the model or cannot be validated.
+        ValueError: If the environment variables do not align with the model's structure or fail validation.
     """
-    try:
-        return model.model_validate(os.environ)
-    except Exception as exc:
-        raise ValueError(f'failed to load environment variables, exception={str(exc)}') from exc
+    return __get_environment_variables_impl(model)
```

### Comparing `aws_lambda_env_modeler-1.0.6/pyproject.toml` & `aws_lambda_env_modeler-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_env_modeler"
-version = "1.0.6"
+version = "1.0.7"
 description = "AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions."
 authors = ["Ran Isenberg"]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -108,9 +108,9 @@
 
 # Like Black, indent with spaces, rather than tabs.
 indent-style = "space"
 
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-third-party = ["pydantic", "aws_lambda_powertools"]
```

### Comparing `aws_lambda_env_modeler-1.0.6/PKG-INFO` & `aws_lambda_env_modeler-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_env_modeler
-Version: 1.0.6
+Version: 1.0.7
 Summary: AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
 Home-page: https://github.com/ran-isenberg/aws-lambda-env-modeler
 License: MIT-0
 Keywords: environment variables parser,aws lambda,serverless best practices,aws serverless,lambda environment variables
 Author: Ran Isenberg
 Requires-Python: >=3.8.17,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -95,15 +95,19 @@
     DB_PORT: int
     DB_USER: str
     DB_PASS: str
     FLAG_X:  bool
     API_URL: HttpUrl
 ```
 
-You must first use the `@init_environment_variables` decorator to automatically validate and initialize the environment variables before executing a function:
+Before executing a function, you must use the `@init_environment_variables` decorator to validate and initialize the environment variables automatically.
+
+The decorator guarantees that the function will run with the correct variable configuration.
+
+Then, you can fetch the environment variables using the global getter function, 'get_environment_variables,' and use them just like a data class. At this point, they are parsed and validated.
 
 ```python
 from aws_lambda_env_modeler import init_environment_variables
 
 @init_environment_variables(MyEnvVariables)
 def my_handler_entry_function(event, context):
     # At this point, environment variables are already validated and initialized
@@ -115,14 +119,59 @@
 ```python
 from aws_lambda_env_modeler import get_environment_variables
 
 env_vars = get_environment_variables(MyEnvVariables)
 print(env_vars.DB_HOST)
 ```
 
+## Disabling Cache for Testing
+
+By default, the modeler uses cache - the parsed model is cached for performance improvement for multiple 'get' calls.
+
+In some cases, such as during testing, you may want to turn off the cache. You can do this by setting the `LAMBDA_ENV_MODELER_DISABLE_CACHE` environment variable to 'True.'
+
+This is especially useful in tests where you want to run multiple tests concurrently, each with a different set of environment variables.
+
+Here's an example of how you can use this in a pytest test:
+
+```python
+import json
+from http import HTTPStatus
+from typing import Any, Dict
+from unittest.mock import patch
+
+from pydantic import BaseModel
+from typing_extensions import Literal
+
+from aws_lambda_env_modeler import LAMBDA_ENV_MODELER_DISABLE_CACHE, get_environment_variables, init_environment_variables
+
+
+class MyHandlerEnvVars(BaseModel):
+    LOG_LEVEL: Literal['DEBUG', 'INFO', 'ERROR', 'CRITICAL', 'WARNING', 'EXCEPTION']
+
+
+@init_environment_variables(model=MyHandlerEnvVars)
+def my_handler(event: Dict[str, Any], context) -> Dict[str, Any]:
+    env_vars = get_environment_variables(model=MyHandlerEnvVars)  # noqa: F841
+    # can access directly env_vars.LOG_LEVEL as dataclass
+    return {
+        'statusCode': HTTPStatus.OK,
+        'headers': {'Content-Type': 'application/json'},
+        'body': json.dumps({'message': 'success'}),
+    }
+
+
+@patch.dict('os.environ', {LAMBDA_ENV_MODELER_DISABLE_CACHE: 'true', 'LOG_LEVEL': 'DEBUG'})
+def test_my_handler():
+    response = my_handler({}, None)
+    assert response['statusCode'] == HTTPStatus.OK
+    assert response['headers'] == {'Content-Type': 'application/json'}
+    assert json.loads(response['body']) == {'message': 'success'}
+```
+
 ## Code Contributions
 Code contributions are welcomed. Read this [guide.](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/CONTRIBUTING.md)
 
 ## Code of Conduct
 Read our code of conduct [here.](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/CODE_OF_CONDUCT.md)
 
 ## Connect
```

