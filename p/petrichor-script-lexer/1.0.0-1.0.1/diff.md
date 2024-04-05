# Comparing `tmp/petrichor_script_lexer-1.0.0.tar.gz` & `tmp/petrichor_script_lexer-1.0.1.tar.gz`

## Comparing `petrichor_script_lexer-1.0.0.tar` & `petrichor_script_lexer-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/petrichor_script_lexer/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/petrichor_script_lexer/petrichorscriptlexer.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/.gitignore
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/LICENSE
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/petrichor_script_lexer/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/petrichor_script_lexer/petrichorscriptlexer.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/.gitignore
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/LICENSE
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 petrichor_script_lexer-1.0.1/PKG-INFO
```

### Comparing `petrichor_script_lexer-1.0.0/petrichor_script_lexer/petrichorscriptlexer.py` & `petrichor_script_lexer-1.0.1/petrichor_script_lexer/petrichorscriptlexer.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 __all__ = ('PetrichorScriptLexer')
 
 
 class PetrichorScriptLexer(RegexLexer):
 	name = 'PetrichorScript'
-	aliases = ['petrichor']
+	aliases = ['petrichor','ptcr']
 	filenames = ['*.petrichor','*.ptcr']
 
 	tokens = {
 		'root': [
 			(r'\s+', Text), # whitespace
 			(r'\\.', String.Escape), # escaped character
 			(r'//.*\n', Comment.Single),
```

### Comparing `petrichor_script_lexer-1.0.0/LICENSE` & `petrichor_script_lexer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `petrichor_script_lexer-1.0.0/pyproject.toml` & `petrichor_script_lexer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "petrichor-script-lexer"
 description = "A custom RegexLexer for Petrichor Script."
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "SparkliTwizzl", email = "github@sparklitwizzl.com" }
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `petrichor_script_lexer-1.0.0/PKG-INFO` & `petrichor_script_lexer-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: petrichor-script-lexer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A custom RegexLexer for Petrichor Script.
 Project-URL: Repository, https://github.com/sparklitwizzl/petrichor
 Project-URL: Issues, https://github.com/sparklitwizzl/petrichor/issues
 Author-email: SparkliTwizzl <github@sparklitwizzl.com>
 License: Petrichor Script Lexer
         Copyright (c) 2024 SparkliTwizzl
```

