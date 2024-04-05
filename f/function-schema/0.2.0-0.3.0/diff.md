# Comparing `tmp/function_schema-0.2.0.tar.gz` & `tmp/function_schema-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_schema-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "function_schema-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `function_schema-0.2.0.tar` & `function_schema-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2547 2023-06-16 03:25:45.708628 function_schema-0.2.0/README.md
--rw-r--r--   0        0        0      192 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/__init__.py
--rw-r--r--   0        0        0      847 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/cli.py
--rw-r--r--   0        0        0     4748 2023-06-16 03:25:45.708628 function_schema-0.2.0/function_schema/core.py
--rw-r--r--   0        0        0      872 2023-06-16 03:25:45.708628 function_schema-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 function_schema-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4208 2024-04-05 06:20:44.476863 function_schema-0.3.0/README.md
+-rw-r--r--   0        0        0      192 2024-04-05 06:20:44.476863 function_schema-0.3.0/function_schema/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-05 06:20:44.480863 function_schema-0.3.0/function_schema/cli.py
+-rw-r--r--   0        0        0     5032 2024-04-05 06:20:44.480863 function_schema-0.3.0/function_schema/core.py
+-rw-r--r--   0        0        0      872 2024-04-05 06:20:44.480863 function_schema-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 function_schema-0.3.0/PKG-INFO
```

### Comparing `function_schema-0.2.0/function_schema/core.py` & `function_schema-0.3.0/function_schema/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import enum
 import typing
 import inspect
 
 
+class SchemaFormat(str, enum.Enum):
+    openai = "openai"
+    claude = "claude"
+
+
 def get_function_schema(
-    func: typing.Annotated[typing.Callable, "The function to get the schema for"]
+    func: typing.Annotated[typing.Callable, "The function to get the schema for"],
+    format: typing.Annotated[
+        typing.Optional[str], SchemaFormat, "The format of the schema to return"
+    ] = "openai",
 ) -> typing.Annotated[dict[str, typing.Any], "The JSON schema for the given function"]:
     """
     Returns a JSON schema for the given function.
 
     You can annotate your function parameters with the special Annotated type.
     Then get the schema for the function without writing the schema by hand.
 
@@ -99,48 +107,51 @@
             schema["properties"][name]["enum"] = [t.name for t in enum_]
 
         if default_value is not inspect._empty:
             schema["properties"][name]["default"] = default_value
 
         if not isinstance(None, T) and default_value is inspect._empty:
             schema["required"].append(name)
+
+    parms_key = "input_schema" if format == "claude" else "parameters"
+
     return {
         "name": func.__name__,
         "description": inspect.getdoc(func),
-        "parameters": schema,
+        parms_key: schema,
     }
 
 
 def guess_type(
-    T: typing.Annotated[type, "The type to guess the JSON schema type for"]
+    T: typing.Annotated[type, "The type to guess the JSON schema type for"],
 ) -> typing.Annotated[
     typing.Union[str, list[str]], "str | list of str that representing JSON schema type"
 ]:
     """Guesses the JSON schema type for the given python type."""
 
     # hacking around typing modules, `typing.Union` and `types.UnitonType`
     union_types = typing.get_args(T)
     if len(union_types) > 1:
         _types = []
         for union_type in union_types:
             _types.append(guess_type(union_type))
-        _types = [t for t in _types if t is not None] # exclude None
+        _types = [t for t in _types if t is not None]  # exclude None
 
         # number contains integer in JSON schema
-        if 'number' in _types and 'integer' in _types:
-            _types.remove('integer')
+        if "number" in _types and "integer" in _types:
+            _types.remove("integer")
 
         if len(_types) == 1:
             return _types[0]
         return _types
 
     if not isinstance(T, type):
         return
 
-    if T.__name__ == 'NoneType':
+    if T.__name__ == "NoneType":
         return
 
     if issubclass(T, str):
         return "string"
     if issubclass(T, bool):
         return "boolean"
     if issubclass(T, float):
```

### Comparing `function_schema-0.2.0/pyproject.toml` & `function_schema-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "function-schema"
-version = "0.2.0"
+version = "0.3.0"
 requires-python = ">= 3.9"
 description = "A small utility to generate JSON schemas for python functions."
 readme = "README.md"
 license = {text = "MIT License"}
 authors = [
   {name = "Changkyun Kim", email = "comfuture@gmail.com"}
 ]
```

