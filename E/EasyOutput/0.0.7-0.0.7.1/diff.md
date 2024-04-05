# Comparing `tmp/easyoutput-0.0.7.tar.gz` & `tmp/easyoutput-0.0.7.1.tar.gz`

## Comparing `easyoutput-0.0.7.tar` & `easyoutput-0.0.7.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.github/ISSUE_TEMPLATE/🐞-bug-report.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.github/ISSUE_TEMPLATE/🚀feature-request.md
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 easyoutput-0.0.7/src/EasyOutput/EasyOutput.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.7/src/EasyOutput/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 easyoutput-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.7/LICENSE
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 easyoutput-0.0.7/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 easyoutput-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 easyoutput-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🐞-bug-report.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🚀feature-request.md
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/src/EasyOutput/EasyOutput.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/src/EasyOutput/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/tests/test.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/LICENSE
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/README.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 easyoutput-0.0.7.1/PKG-INFO
```

### Comparing `easyoutput-0.0.7/.github/ISSUE_TEMPLATE/🚀feature-request.md` & `easyoutput-0.0.7.1/.github/ISSUE_TEMPLATE/🚀feature-request.md`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.7/LICENSE` & `easyoutput-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyoutput-0.0.7/pyproject.toml` & `easyoutput-0.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyOutput"
-version = "0.0.7"
+version = "0.0.7.1"
 authors = [
   { name="FrankAustin", email="frankaustindev808@gmail.com" },
 ]
 description = "Colored messages in the palm of your hand"
 readme = "README.md"
 requires-python = ">=3.12"
 install_requires=['colorama']
```

### Comparing `easyoutput-0.0.7/PKG-INFO` & `easyoutput-0.0.7.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: EasyOutput
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Colored messages in the palm of your hand
 Project-URL: Homepage, https://github.com/FrankAustin808/EasyOut/
 Project-URL: Issues, https://github.com/FrankAustin808/EasyOut/issues/new/choose
 Author-email: FrankAustin <frankaustindev808@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 
 # Easy Output 
-
+```py 
+# How to use 👽
+from EasyOutput.EasyOutput import *
+```
 # Information
 **EasyOutput** consists of easy colored print options without the hassle of doing
 ```py
 print(f"{Fore.GREEN + Style.BRIGHT}Success{Style.RESET_ALL}: Your Message")
 ```
 
 In reality this is nothing special and just simply for my lazy use. You could easily make these yourself by doing
@@ -32,86 +35,39 @@
 
 Success("Your Success Message")
 ```
 
 If you would rather save time instead, you can always download it by entering **pip install EasyOutput** into your terminal!\
 Feel free to use this in any way you like, all I ask is that you show me your project when finished! 😄
 
-[Request a feature](https://github.com/FrankAustin808/EasyOut/issues/new/choose)\
-[Report an issue](https://github.com/FrankAustin808/EasyOut/issues/new/choose)
+[Request a feature](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)\
+[Report an issue](https://github.com/FrankAustin808/EasyOutput/issues/new/choose)
 
 **Updating as much as I can!**
 # Functions
 
 ### Success
 **Use:**
 ```py
-Success("EasyOutput")
-
-```
-**Shows:**
-
-Success: EasyOutput
-
-### Successful_Connection
-**Use:**
-```py
-Successful_Connection("EasyOutput")
+Success_Message("EasyOutput")
 
 ```
 **Shows:**
 
-Successful Connection: EasyOutput
+Success: EasyOutput 
 
 ### Error
 **Use:**
 ```py
-Error("EasyOutput")
-
-```
-**Shows:**
-
-Error: EasyOutput
-
-### Connection_Error
-**Use:**
-```py
-Connection_Error("EasyOutput")
+Error_Message("EasyOutput")
 
 ```
 **Shows:**
 
-Connection Error: EasyOutput
-
-### Note
-**Use:**
-```py
-Note("EasyOutput")
-
-```
-**Shows:**
-
-Note: EasyOutput
-
-### Wait
-**Use:**
-```py
-Wait("EasyOutput")
-
-```
-**Shows:**
-
-Wait: EasyOutput
-
-### Title
-**Use:**
-```py
-Title("EasyOutput")
-
-```
-**Shows:**
-
-=== EasyOutput === 
+Error: EasyOutput 
 
 ## PYPI
 
 [EasyOutput](https://pypi.org/project/EasyOutput/)
+
+
+Badges from: [Shields.io](https://shields.io/badges)
```

