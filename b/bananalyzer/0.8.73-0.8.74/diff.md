# Comparing `tmp/bananalyzer-0.8.73.tar.gz` & `tmp/bananalyzer-0.8.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananalyzer-0.8.73.tar", max compression
+gzip compressed data, was "bananalyzer-0.8.74.tar", max compression
```

## Comparing `bananalyzer-0.8.73.tar` & `bananalyzer-0.8.74.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-11-23 23:05:17.895386 bananalyzer-0.8.73/LICENSE
--rw-r--r--   0        0        0     7149 2024-01-29 23:48:01.270146 bananalyzer-0.8.73/README.md
--rw-r--r--   0        0        0      380 2024-01-29 23:31:29.206701 bananalyzer-0.8.73/bananalyzer/__init__.py
--rw-r--r--   0        0        0    10925 2024-04-02 18:46:06.321568 bananalyzer-0.8.73/bananalyzer/__main__.py
--rw-r--r--   0        0        0       79 2024-01-18 00:36:02.748184 bananalyzer-0.8.73/bananalyzer/__version.py
--rw-r--r--   0        0        0        0 2023-11-23 23:05:17.898081 bananalyzer-0.8.73/bananalyzer/data/__init__.py
--rw-r--r--   0        0        0     1500 2024-04-02 18:44:14.621000 bananalyzer-0.8.73/bananalyzer/data/banana_seeds.py
--rw-r--r--   0        0        0     4583 2024-01-29 23:31:29.208551 bananalyzer-0.8.73/bananalyzer/data/examples.py
--rw-r--r--   0        0        0    13341 2024-03-19 05:36:25.357129 bananalyzer-0.8.73/bananalyzer/data/fetch_schemas.py
--rw-r--r--   0        0        0     5356 2024-02-15 22:53:28.228334 bananalyzer-0.8.73/bananalyzer/data/generate_examples.py
--rw-r--r--   0        0        0     6273 2024-03-19 05:36:25.358014 bananalyzer-0.8.73/bananalyzer/data/schemas.py
--rw-r--r--   0        0        0     6703 2024-01-29 23:31:29.209682 bananalyzer-0.8.73/bananalyzer/hooks.py
--rw-r--r--   0        0        0     1249 2024-01-29 23:31:29.209995 bananalyzer-0.8.73/bananalyzer/junit.py
--rw-r--r--   0        0        0        0 2023-11-23 23:05:17.900777 bananalyzer-0.8.73/bananalyzer/runner/__init__.py
--rw-r--r--   0        0        0      501 2023-11-28 00:11:43.853844 bananalyzer-0.8.73/bananalyzer/runner/agent_runner.py
--rw-r--r--   0        0        0     5006 2024-04-03 21:50:56.706436 bananalyzer-0.8.73/bananalyzer/runner/evals.py
--rw-r--r--   0        0        0     2402 2024-03-19 05:36:28.376065 bananalyzer-0.8.73/bananalyzer/runner/generator.py
--rw-r--r--   0        0        0     1306 2024-02-16 05:41:25.422171 bananalyzer-0.8.73/bananalyzer/runner/null_agent_wrapper.py
--rw-r--r--   0        0        0     4392 2024-03-19 05:36:28.376276 bananalyzer-0.8.73/bananalyzer/runner/runner.py
--rw-r--r--   0        0        0     1566 2023-11-23 23:05:17.903092 bananalyzer-0.8.73/bananalyzer/runner/website_responder.py
--rw-r--r--   0        0        0     1366 2024-02-19 05:54:13.593386 bananalyzer-0.8.73/bananalyzer/schema.py
--rw-r--r--   0        0        0     1320 2024-04-03 21:55:57.989313 bananalyzer-0.8.73/pyproject.toml
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 bananalyzer-0.8.73/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-23 23:05:17.895386 bananalyzer-0.8.74/LICENSE
+-rw-r--r--   0        0        0     7149 2024-01-29 23:48:01.270146 bananalyzer-0.8.74/README.md
+-rw-r--r--   0        0        0      380 2024-01-29 23:31:29.206701 bananalyzer-0.8.74/bananalyzer/__init__.py
+-rw-r--r--   0        0        0    10925 2024-04-02 18:46:06.321568 bananalyzer-0.8.74/bananalyzer/__main__.py
+-rw-r--r--   0        0        0       79 2024-01-18 00:36:02.748184 bananalyzer-0.8.74/bananalyzer/__version.py
+-rw-r--r--   0        0        0        0 2023-11-23 23:05:17.898081 bananalyzer-0.8.74/bananalyzer/data/__init__.py
+-rw-r--r--   0        0        0     1500 2024-04-02 18:44:14.621000 bananalyzer-0.8.74/bananalyzer/data/banana_seeds.py
+-rw-r--r--   0        0        0     4583 2024-01-29 23:31:29.208551 bananalyzer-0.8.74/bananalyzer/data/examples.py
+-rw-r--r--   0        0        0    13341 2024-03-19 05:36:25.357129 bananalyzer-0.8.74/bananalyzer/data/fetch_schemas.py
+-rw-r--r--   0        0        0     5356 2024-02-15 22:53:28.228334 bananalyzer-0.8.74/bananalyzer/data/generate_examples.py
+-rw-r--r--   0        0        0     7549 2024-04-05 03:30:13.918723 bananalyzer-0.8.74/bananalyzer/data/schemas.py
+-rw-r--r--   0        0        0     6703 2024-01-29 23:31:29.209682 bananalyzer-0.8.74/bananalyzer/hooks.py
+-rw-r--r--   0        0        0     1249 2024-01-29 23:31:29.209995 bananalyzer-0.8.74/bananalyzer/junit.py
+-rw-r--r--   0        0        0        0 2023-11-23 23:05:17.900777 bananalyzer-0.8.74/bananalyzer/runner/__init__.py
+-rw-r--r--   0        0        0      501 2023-11-28 00:11:43.853844 bananalyzer-0.8.74/bananalyzer/runner/agent_runner.py
+-rw-r--r--   0        0        0     5016 2024-04-05 03:13:12.228618 bananalyzer-0.8.74/bananalyzer/runner/evals.py
+-rw-r--r--   0        0        0     2402 2024-03-19 05:36:28.376065 bananalyzer-0.8.74/bananalyzer/runner/generator.py
+-rw-r--r--   0        0        0     1072 2024-04-05 03:37:53.885624 bananalyzer-0.8.74/bananalyzer/runner/null_agent_wrapper.py
+-rw-r--r--   0        0        0     4392 2024-03-19 05:36:28.376276 bananalyzer-0.8.74/bananalyzer/runner/runner.py
+-rw-r--r--   0        0        0     1566 2023-11-23 23:05:17.903092 bananalyzer-0.8.74/bananalyzer/runner/website_responder.py
+-rw-r--r--   0        0        0     1366 2024-02-19 05:54:13.593386 bananalyzer-0.8.74/bananalyzer/schema.py
+-rw-r--r--   0        0        0     1320 2024-04-05 03:40:59.804680 bananalyzer-0.8.74/pyproject.toml
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 bananalyzer-0.8.74/PKG-INFO
```

### Comparing `bananalyzer-0.8.73/LICENSE` & `bananalyzer-0.8.74/LICENSE`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/README.md` & `bananalyzer-0.8.74/README.md`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/__main__.py` & `bananalyzer-0.8.74/bananalyzer/__main__.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/data/banana_seeds.py` & `bananalyzer-0.8.74/bananalyzer/data/banana_seeds.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/data/examples.py` & `bananalyzer-0.8.74/bananalyzer/data/examples.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/data/fetch_schemas.py` & `bananalyzer-0.8.74/bananalyzer/data/fetch_schemas.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/data/generate_examples.py` & `bananalyzer-0.8.74/bananalyzer/data/generate_examples.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/data/schemas.py` & `bananalyzer-0.8.74/bananalyzer/data/schemas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from typing import Any, Dict, List, Literal, Optional, Type, Union
 
+import pytest
 from playwright.async_api import Page
 from pydantic import BaseModel, Field, model_validator
 
 from bananalyzer.runner.evals import (
     AllowedJSON,
     validate_end_url_match,
     validate_field_match,
@@ -25,40 +26,71 @@
 
 class Eval(BaseModel):
     """
     Base class for all evals. Evals are used to determine if an action or result is correct
     """
 
     type: Literal["json_match", "end_url_match"] = "json_match"
-    expected: AllowedJSON
+    expected: AllowedJSON | None = Field(default=None)
+    options: Optional[AllowedJSON] = Field(default=None)
+
+    @model_validator(mode='before')
+    def validate_expected_or_options(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        expected = values.get("expected")
+        options = values.get("options")
+
+        if expected is not None and options is not None:
+            raise ValueError("Only one of expected or options can be provided")
+
+        if expected is None and options is None:
+            raise ValueError("One of expected or options must be provided")
+
+        return values
 
     def eval_action(self, action: str) -> bool:
         """
         We don't care for action level evals at the moment
         """
         raise NotImplementedError("eval_action not implemented")
 
     def eval_results(
         self, page: Page, result: Dict[str, Any], field: Optional[str] = None
     ) -> None:
-        if (
-            self.type == "json_match"
-            and field is not None
-            and isinstance(self.expected, dict)
-        ):
-            return validate_field_match(self.expected, result, field)
-
-        if self.type == "json_match" and isinstance(self.expected, (list, dict)):
-            return validate_json_match(self.expected, result)
+        if self.type == "json_match":
+            return self.handle_json_match(result, field)
 
         if self.type == "end_url_match" and isinstance(self.expected, str):
             return validate_end_url_match(self.expected, page.url)
 
         raise NotImplementedError("No evaluation type implemented")
 
+    def handle_json_match(self, result: Dict[str, Any], field: Optional[str]) -> None:
+        options = self.options or [self.expected]
+        exceptions: list[ValueError] = []
+
+        # Try all options
+        for option in options:
+            try:
+                if (
+                    self.type == "json_match"
+                    and field is not None
+                    and isinstance(option, dict)
+                ):
+                    return validate_field_match(option, result, field)
+
+                if self.type == "json_match" and isinstance(option, (list, dict)):
+                    return validate_json_match(option, result)
+            except Exception as e:
+                exceptions.append(e)
+
+        if len(exceptions) == len(options):
+            if len(options) > 1:
+                pytest.fail(f"None of the available options matched. For example: {str(exceptions[0])}")
+            pytest.fail(str(exceptions[0]))
+
 
 FetchId = Literal[
     "job_posting",
     "manufacturing_commerce",
     "contact",
     "contract",
     "forum",
```

### Comparing `bananalyzer-0.8.73/bananalyzer/hooks.py` & `bananalyzer-0.8.74/bananalyzer/hooks.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/junit.py` & `bananalyzer-0.8.74/bananalyzer/junit.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/runner/evals.py` & `bananalyzer-0.8.74/bananalyzer/runner/evals.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     if expected_value is None and actual_value is None:
         pytest.skip(
             f"Field {field} is None in both expected and actual. Skipping this test."
         )
 
     if not check_match(expected_value, actual_value):
-        pytest.fail(f"{expected_value} != {actual_value}")
+        raise ValueError(f"{expected_value} != {actual_value}")
 
 
 def trim_strings(value: AllowedJSON) -> AllowedJSON:
     """Recursively trim strings in the given JSON structure."""
     if isinstance(value, dict):
         return {k: trim_strings(v) for k, v in value.items()}
     elif isinstance(value, list):
@@ -74,15 +74,15 @@
     )
     if diff:
         # Pretty print both expected and actual results
         pretty_expected = json.dumps(expected, indent=4)
         pretty_actual = json.dumps(actual, indent=4)
 
         diff_msg = f"Actual: {pretty_actual}\nExpected: {pretty_expected}"
-        pytest.fail(f"JSONEval mismatch!\n{diff_msg}")
+        raise ValueError(f"JSONEval mismatch!\n{diff_msg}")
 
 
 def validate_end_url_match(expected: str, actual: str) -> None:
     if actual != expected:
         diff_msg = f"Actual URL:\t{actual}\nExpected URL:\t{expected}"
         pytest.fail(f"URLEval mismatch!\n{diff_msg}")
```

### Comparing `bananalyzer-0.8.73/bananalyzer/runner/generator.py` & `bananalyzer-0.8.74/bananalyzer/runner/generator.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/runner/null_agent_wrapper.py` & `bananalyzer-0.8.74/bananalyzer/runner/null_agent_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import asyncio
-from random import random
-from typing import Any, cast
 
 from playwright.async_api import Page
 
 from bananalyzer.data.schemas import Example
 from bananalyzer.runner.agent_runner import AgentResult, AgentRunner
 
 
@@ -29,16 +27,11 @@
         # Ensure page is correct
         if example.evals[0].type == "end_url_match" and isinstance(
             example.evals[0].expected, str
         ):
             await page.goto(example.evals[0].expected)
             return example.evals[0].expected
 
-        if example.type == "links" or example.type == "links_fetch":
+        if example.evals[0].expected is not None:
             return example.evals[0].expected
-
-        copy = cast(dict[str, Any], example.evals[0].expected).copy()
-        for key, value in copy.items():
-            if random() < self.RANDOM_FAILURE_RATE:
-                copy[key] = "random"
-
-        return copy
+        else:
+            return example.evals[0].options[0]
```

### Comparing `bananalyzer-0.8.73/bananalyzer/runner/runner.py` & `bananalyzer-0.8.74/bananalyzer/runner/runner.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/runner/website_responder.py` & `bananalyzer-0.8.74/bananalyzer/runner/website_responder.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/bananalyzer/schema.py` & `bananalyzer-0.8.74/bananalyzer/schema.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.73/pyproject.toml` & `bananalyzer-0.8.74/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bananalyzer"
-version = "0.8.73"
+version = "0.8.74"
 
 description = "Open source AI Agent evaluation framework for web tasks 🐒🍌"
 authors = ["asim-shrestha <asim.shrestha@hotmail.com>", "awtkns <hello@awtkns.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 bananalyze = "bananalyzer.__main__:main"
```

### Comparing `bananalyzer-0.8.73/PKG-INFO` & `bananalyzer-0.8.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bananalyzer
-Version: 0.8.73
+Version: 0.8.74
 Summary: Open source AI Agent evaluation framework for web tasks 🐒🍌
 Author: asim-shrestha
 Author-email: asim.shrestha@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

