# Comparing `tmp/petrichor_script_lexer-0.11.0.post2.tar.gz` & `tmp/petrichor_script_lexer-0.11.0.post3.tar.gz`

## Comparing `petrichor_script_lexer-0.11.0.post2.tar` & `petrichor_script_lexer-0.11.0.post3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/petrichor_script_lexer/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/petrichor_script_lexer/petrichorscriptlexer.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/.gitignore
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/LICENSE
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/pyproject.toml
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/petrichor_script_lexer/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/petrichor_script_lexer/petrichorscriptlexer.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/.gitignore
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/LICENSE
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/pyproject.toml
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post3/PKG-INFO
```

### Comparing `petrichor_script_lexer-0.11.0.post2/petrichor_script_lexer/petrichorscriptlexer.py` & `petrichor_script_lexer-0.11.0.post3/petrichor_script_lexer/petrichorscriptlexer.py`

 * *Files identical despite different names*

### Comparing `petrichor_script_lexer-0.11.0.post2/LICENSE` & `petrichor_script_lexer-0.11.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `petrichor_script_lexer-0.11.0.post2/pyproject.toml` & `petrichor_script_lexer-0.11.0.post3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "petrichor-script-lexer"
 description = "A custom RegexLexer for Petrichor Script."
-version = "0.11.0-2"
+version = "0.11.0-3"
 authors = [
     { name = "SparkliTwizzl", email = "github@sparklitwizzl.com" }
 ]
-license = { file="LICENSE" }
+license = { file = "LICENSE" }
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Free To Use But Restricted",
     "Operating System :: OS Independent",
 ]
 dependencies = [ "pygments" ]
```

### Comparing `petrichor_script_lexer-0.11.0.post2/PKG-INFO` & `petrichor_script_lexer-0.11.0.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: petrichor-script-lexer
-Version: 0.11.0.post2
+Version: 0.11.0.post3
 Summary: A custom RegexLexer for Petrichor Script.
 Project-URL: Repository, https://github.com/sparklitwizzl/petrichor
 Project-URL: Issues, https://github.com/sparklitwizzl/petrichor/issues
 Author-email: SparkliTwizzl <github@sparklitwizzl.com>
 License: Petrichor Script Lexer
         Copyright (c) 2024 SparkliTwizzl
```

