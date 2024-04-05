# Comparing `tmp/scanreq-0.0.6.tar.gz` & `tmp/scanreq-0.0.7.tar.gz`

## Comparing `scanreq-0.0.6.tar` & `scanreq-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.6/requirements-dev.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.6/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.6/setup.cfg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.6/src/scanreq/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.6/src/scanreq/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 scanreq-0.0.6/src/scanreq/__main__.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 scanreq-0.0.6/src/scanreq/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 scanreq-0.0.6/tests/test_scanner.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.6/LICENSE
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 scanreq-0.0.6/README.md
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 scanreq-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 scanreq-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scanreq-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scanreq-0.0.7/requirements-dev.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scanreq-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 scanreq-0.0.7/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/__main__.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scanreq-0.0.7/src/scanreq/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scanreq-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 scanreq-0.0.7/tests/test_scanner.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 scanreq-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 scanreq-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 scanreq-0.0.7/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 scanreq-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 scanreq-0.0.7/PKG-INFO
```

### Comparing `scanreq-0.0.6/.pre-commit-config.yaml` & `scanreq-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.6/src/scanreq/scanner.py` & `scanreq-0.0.7/src/scanreq/scanner.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # allowed extensions to scan
 ALLOWED_EXTENSIONS: Tuple[str] = (
     ".py",
     ".conf",
     ".cfg",
     ".yml",
     ".yaml",
+    "Dockerfile",
 )
 
 
 def get_main_packages() -> dict:
     """
     Get the main packages available in the distribution.
 
@@ -122,7 +123,47 @@
             # Remove comments and leading/trailing whitespaces
             line = re.sub(r"#.*", "", line).strip()
             if line:
                 # Split the line to get the package name
                 package_name: str = line.split("==")[0].strip().lower()
                 package_names.append(package_name)
     return package_names
+
+
+def scan(requirement_file: str, project_path: str, output_path: str = None) -> None:
+    """
+    A function that scans for unused packages in a project based on a given requirements file.
+
+    Parameters:
+        - requirement_file (str): the path to the requirements file to be scanned.
+        - project_path (str): the path to the project to be scanned.
+        - output_path (str, optional): the path to the output file where unused packages will be saved. Defaults to None.
+
+    Returns:
+        - None
+    """
+    print("\n[i] Please wait! It may take few minutes to complete...")
+
+    package_names: List[str] = read_requirements(requirement_file)
+    main_packages: dict = get_main_packages()
+
+    print("[i] Scanning unused packages:")
+    unused_packages: List[str] = []
+    number: int = 1
+    for package_name in package_names:
+        for module_name, package_names in main_packages.items():
+            if package_name in package_names:
+                results: list = search_string_in_python_files(project_path, module_name)
+                if not results and (module_name not in unused_packages):
+                    unused_packages.append(package_name)
+                    number_str: str = f"{number}."
+                    print(
+                        f" {number_str: <4}Module: {module_name: <30}-> Package: {package_name}"
+                    )
+                    number += 1
+
+    if len(unused_packages) < 1:
+        print("[i] Great! No unused packages found.")
+
+    elif unused_packages and output_path:
+        with open(output_path, "w") as _file:
+            _file.writelines("\n".join(unused_packages) + "\n")
```

### Comparing `scanreq-0.0.6/tests/test_scanner.py` & `scanreq-0.0.7/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.6/.gitignore` & `scanreq-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.6/LICENSE` & `scanreq-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scanreq-0.0.6/README.md` & `scanreq-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # ScanReq
 
 [![PyPI - Version](https://img.shields.io/pypi/v/scanreq.svg)](https://pypi.org/project/scanreq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/scanreq.svg)](https://pypi.org/project/scanreq)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/agusmakmun/scan-unused-requirements/run-tests.yml?branch=master)](https://github.com/agusmakmun/scan-unused-requirements/actions/workflows/run-tests.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **ScanReq** - Python tool to scan all unused packages in requirements.txt file for your project.
 
 ## Background
 
 One popular tool for checking requirements in a Python project is `pipdeptree`. However, the problem arises when we don't know which packages listed in the `requirements.txt` file are actually being used in the project or not. It's easy to check if your project is small, but as your project grows larger, it becomes a headache to check one by one.
 
@@ -31,51 +33,72 @@
 ```console
 pip3 install scanreq
 ```
 
 
 ## Usage
 
+> **Note:** Ensure you're working on python environment.
+
 ```console
-(env-myproject) ➜  myproject git:(development) ✗ scanreq -r requirements.txt -p .
+scanreq -r requirements.txt -p . -o unused-requirements.txt
+```
 
+```
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
- 1. Module: rcssmin ---> Package: rcssmin
- 2. Module: model_utils ---> Package: django-model-utils
- 3. Module: pinax_theme_bootstrap ---> Package: pinax-theme-bootstrap
- 4. Module: phonenumbers ---> Package: phonenumbers
+ 1.  Module: rcssmin                       -> Package: rcssmin
+ 2.  Module: model_utils                   -> Package: django-model-utils
+ 3.  Module: pinax_theme_bootstrap         -> Package: pinax-theme-bootstrap
+ 4.  Module: phonenumbers                  -> Package: phonenumbers
+```
+
+```console
+cat unused-requirements.txt
+```
+
+```
+rcssmin
+django-model-utils
+pinax-theme-bootstrap
+phonenumbers
 ```
 
 Cool right? 😎
 
 ```console
-(env-myproject) ➜  myproject git:(development) ✗ scanreq --help
-usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH]
+scanreq --help
+```
+
+```
+usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
                         Path to the requirements.txt file to read packages from.
   -p PATH, --path PATH  Project path to scan for unused packages (default: current directory).
+  -o OUTPUT, --output OUTPUT
+                        Path to the output file where unused packages will be saved.
 ```
 
 > **Note:** Don't forget to cross-check the unused packages after finding them,
 > because sometimes they are used in different cases without being imported in the code.
 > For example: `argon2-cffi` used in `settings.PASSWORD_HASHERS = ["django.contrib.auth.hashers.Argon2PasswordHasher", ...]` for Django.
 
 
 ## ToDo List
 
 - [x] Support argument parser (command arguments)
    - [x] Directory to scan
    - [x] Requirement file to scan
+   - [x] Option to write the output of unused packages
    - [ ] Option to auto replace the package from requirements.txt file
    - [ ] Option to exclude or ignore some packages
 - [x] Support CLI - make it as a command
 - [x] Write some tests
 - [x] Publish to PyPi
+- [x] Support multiple python versions
 - [ ] Support scan the `pyproject.toml`
-- [ ] Support multiple python versions
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
```

### Comparing `scanreq-0.0.6/pyproject.toml` & `scanreq-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,17 @@
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["importlib_metadata>=7.1.0"]
 scripts.scanreq = "scanreq.__main__:main"
 
 [project.urls]
 Changelog = "https://github.com/agusmakmun/scan-unused-requirements/releases"
-Documentation = "https://github.com/agusmakmun/scanreq"
-Issues = "https://github.com/agusmakmun/scanreq/issues"
-Source = "https://github.com/agusmakmun/scanreq"
+Documentation = "https://github.com/agusmakmun/scan-unused-requirements"
+Issues = "https://github.com/agusmakmun/scan-unused-requirements/issues"
+Source = "https://github.com/agusmakmun/scan-unused-requirements"
 
 [tool.hatch.version]
 path = "src/scanreq/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]>=6.5", "pytest"]
 [tool.hatch.envs.default.scripts]
```

### Comparing `scanreq-0.0.6/PKG-INFO` & `scanreq-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: scanreq
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python tool to scan all unused packages in requirements.txt file for your project.
 Project-URL: Changelog, https://github.com/agusmakmun/scan-unused-requirements/releases
-Project-URL: Documentation, https://github.com/agusmakmun/scanreq
-Project-URL: Issues, https://github.com/agusmakmun/scanreq/issues
-Project-URL: Source, https://github.com/agusmakmun/scanreq
+Project-URL: Documentation, https://github.com/agusmakmun/scan-unused-requirements
+Project-URL: Issues, https://github.com/agusmakmun/scan-unused-requirements/issues
+Project-URL: Source, https://github.com/agusmakmun/scan-unused-requirements
 Author-email: agusmakmun <summon.agus@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: packages,requirements,scan,unused
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,16 @@
 Requires-Dist: importlib-metadata>=7.1.0
 Description-Content-Type: text/markdown
 
 # ScanReq
 
 [![PyPI - Version](https://img.shields.io/pypi/v/scanreq.svg)](https://pypi.org/project/scanreq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/scanreq.svg)](https://pypi.org/project/scanreq)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/agusmakmun/scan-unused-requirements/run-tests.yml?branch=master)](https://github.com/agusmakmun/scan-unused-requirements/actions/workflows/run-tests.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 **ScanReq** - Python tool to scan all unused packages in requirements.txt file for your project.
 
 ## Background
 
 One popular tool for checking requirements in a Python project is `pipdeptree`. However, the problem arises when we don't know which packages listed in the `requirements.txt` file are actually being used in the project or not. It's easy to check if your project is small, but as your project grows larger, it becomes a headache to check one by one.
 
@@ -59,51 +61,72 @@
 ```console
 pip3 install scanreq
 ```
 
 
 ## Usage
 
+> **Note:** Ensure you're working on python environment.
+
 ```console
-(env-myproject) ➜  myproject git:(development) ✗ scanreq -r requirements.txt -p .
+scanreq -r requirements.txt -p . -o unused-requirements.txt
+```
 
+```
 [i] Please wait! It may take few minutes to complete...
 [i] Scanning unused packages:
- 1. Module: rcssmin ---> Package: rcssmin
- 2. Module: model_utils ---> Package: django-model-utils
- 3. Module: pinax_theme_bootstrap ---> Package: pinax-theme-bootstrap
- 4. Module: phonenumbers ---> Package: phonenumbers
+ 1.  Module: rcssmin                       -> Package: rcssmin
+ 2.  Module: model_utils                   -> Package: django-model-utils
+ 3.  Module: pinax_theme_bootstrap         -> Package: pinax-theme-bootstrap
+ 4.  Module: phonenumbers                  -> Package: phonenumbers
+```
+
+```console
+cat unused-requirements.txt
+```
+
+```
+rcssmin
+django-model-utils
+pinax-theme-bootstrap
+phonenumbers
 ```
 
 Cool right? 😎
 
 ```console
-(env-myproject) ➜  myproject git:(development) ✗ scanreq --help
-usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH]
+scanreq --help
+```
+
+```
+usage: scan.py [-h] [-r REQUIREMENTS] [-p PATH] [-o OUTPUT]
 
 Scan for unused Python packages.
 
 optional arguments:
   -h, --help            show this help message and exit
   -r REQUIREMENTS, --requirements REQUIREMENTS
                         Path to the requirements.txt file to read packages from.
   -p PATH, --path PATH  Project path to scan for unused packages (default: current directory).
+  -o OUTPUT, --output OUTPUT
+                        Path to the output file where unused packages will be saved.
 ```
 
 > **Note:** Don't forget to cross-check the unused packages after finding them,
 > because sometimes they are used in different cases without being imported in the code.
 > For example: `argon2-cffi` used in `settings.PASSWORD_HASHERS = ["django.contrib.auth.hashers.Argon2PasswordHasher", ...]` for Django.
 
 
 ## ToDo List
 
 - [x] Support argument parser (command arguments)
    - [x] Directory to scan
    - [x] Requirement file to scan
+   - [x] Option to write the output of unused packages
    - [ ] Option to auto replace the package from requirements.txt file
    - [ ] Option to exclude or ignore some packages
 - [x] Support CLI - make it as a command
 - [x] Write some tests
 - [x] Publish to PyPi
+- [x] Support multiple python versions
 - [ ] Support scan the `pyproject.toml`
-- [ ] Support multiple python versions
 - [ ] Support multiple devices (Linux, Macbook, and Windows)
```

