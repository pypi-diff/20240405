# Comparing `tmp/petrichor_script_lexer-0.11.0.tar.gz` & `tmp/petrichor_script_lexer-0.11.0.post1.tar.gz`

## Comparing `petrichor_script_lexer-0.11.0.tar` & `petrichor_script_lexer-0.11.0.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/petrichor_script_lexer/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/petrichor_script_lexer/petrichorscriptlexer.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/.gitignore
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/LICENSE.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/pyproject.toml
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/petrichor_script_lexer/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/petrichor_script_lexer/petrichorscriptlexer.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/.gitignore
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/LICENSE.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 petrichor_script_lexer-0.11.0.post1/PKG-INFO
```

### Comparing `petrichor_script_lexer-0.11.0/petrichor_script_lexer/petrichorscriptlexer.py` & `petrichor_script_lexer-0.11.0.post1/petrichor_script_lexer/petrichorscriptlexer.py`

 * *Files identical despite different names*

### Comparing `petrichor_script_lexer-0.11.0/LICENSE.md` & `petrichor_script_lexer-0.11.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `petrichor_script_lexer-0.11.0/pyproject.toml` & `petrichor_script_lexer-0.11.0.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
-requires = ["hatchling"]
+requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "petrichor-script-lexer"
-description = "A custom RegexLexer for Petrichor Script"
-version = "0.11.0"
+description = "A custom RegexLexer for Petrichor Script."
+version = "0.11.0-1"
 authors = [
     { name = "SparkliTwizzl", email = "github@sparklitwizzl.com" }
 ]
-license = {file = "LICENSE.md"}
+license = { file="LICENSE.md" }
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "License :: Free To Use But Restricted",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pygments"]
+dependencies = [ "pygments" ]
 
 [project.entry-points."pygments.lexers"]
-commandlexer = "petrichorscriptlexer.petrichorscriptlexer:PetrichorScriptLexer"
+petrichorscriptlexer = "petrichorscriptlexer.petrichorscriptlexer:PetrichorScriptLexer"
 
 [project.urls]
 Repository = "https://github.com/sparklitwizzl/petrichor"
 Issues = "https://github.com/sparklitwizzl/petrichor/issues"
```

### Comparing `petrichor_script_lexer-0.11.0/PKG-INFO` & `petrichor_script_lexer-0.11.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: petrichor-script-lexer
-Version: 0.11.0
-Summary: A custom RegexLexer for Petrichor Script
+Version: 0.11.0.post1
+Summary: A custom RegexLexer for Petrichor Script.
 Project-URL: Repository, https://github.com/sparklitwizzl/petrichor
 Project-URL: Issues, https://github.com/sparklitwizzl/petrichor/issues
 Author-email: SparkliTwizzl <github@sparklitwizzl.com>
 License: <h1 align="center">Petrichor Script Lexer</h1>
         <h3 align="center">Copyright (c) 2024 SparkliTwizzl</h3>
         
         <h4 align="center"><a href="https://github.com/SparkliTwizzl/anti-exploitation-license/releases/tag/AEL-1.1">Anti-Exploitation License Noncommmercial Attribution v1.1 (AEL-NC-AT 1.1)</a></h4>
@@ -49,11 +49,12 @@
         7. The User does not engage in and/or promote any of the activities listed in Item 5, and is not affiliated with any group and/or organization that engages in and/or promotes any of such activities. The User does not behave in a manner counter to the priciples listed in Item 6, and is not affiliated with any group and/or organization that behaves in a manner counter to such principles.
         
         8. The User does not resell the Project or any part of the Project.
         
         
         The Project is provided "as is", without express or implied warranty of any kind, including but not limtied to the warranties of: merchantability; fitness for a particular purpose; noninfringement. In no event shall the Authors be liable for any claim; damages; or other liability, whether in action of contract; tort; or otherwise, arising from; out of; or in connection with, the Project; or the use of or dealings in the Project.
 License-File: LICENSE.md
+Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Requires-Dist: pygments
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.3 Name: petrichor-script-lexer Version: 0.11.0 Summary: A
-custom RegexLexer for Petrichor Script Project-URL: Repository, https://
-github.com/sparklitwizzl/petrichor Project-URL: Issues, https://github.com/
-sparklitwizzl/petrichor/issues Author-email: SparkliTwizzl
+Metadata-Version: 2.3 Name: petrichor-script-lexer Version: 0.11.0.post1
+Summary: A custom RegexLexer for Petrichor Script. Project-URL: Repository,
+https://github.com/sparklitwizzl/petrichor Project-URL: Issues, https://
+github.com/sparklitwizzl/petrichor/issues Author-email: SparkliTwizzl
 sparklitwizzl.com> License:
                      ************ PPeettrriicchhoorr SSccrriipptt LLeexxeerr ************
                   ******** CCooppyyrriigghhtt ((cc)) 22002244 SSppaarrkklliiTTwwiizzzzll ********
  ****** _AA_nn_tt_ii_--_EE_xx_pp_ll_oo_ii_tt_aa_tt_ii_oo_nn_ _LL_ii_cc_ee_nn_ss_ee_ _NN_oo_nn_cc_oo_mm_mm_mm_ee_rr_cc_ii_aa_ll_ _AA_tt_tt_rr_ii_bb_uu_tt_ii_oo_nn_ _vv_11_.._11_ _((_AA_EE_LL_--_NN_CC_--_AA_TT_ _11_.._11_))
                                       ******
 This is an anti-capitalist, anti-fascist, anti-bigotry, pro-human-rights
 project, released for free use by individuals and organizations who are tired
@@ -67,9 +67,10 @@
 principles. 8. The User does not resell the Project or any part of the Project.
 The Project is provided "as is", without express or implied warranty of any
 kind, including but not limtied to the warranties of: merchantability; fitness
 for a particular purpose; noninfringement. In no event shall the Authors be
 liable for any claim; damages; or other liability, whether in action of
 contract; tort; or otherwise, arising from; out of; or in connection with, the
 Project; or the use of or dealings in the Project. License-File: LICENSE.md
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Requires-Python: >=3.12 Requires-Dist: pygments
+Classifier: License :: Free To Use But Restricted Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
+Python: >=3.12 Requires-Dist: pygments
```

