# Comparing `tmp/pharmacelera_utils-0.1.60.tar.gz` & `tmp/pharmacelera_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmacelera_utils-0.1.60.tar", last modified: Thu Nov  2 11:16:18 2023, max compression
+gzip compressed data, was "pharmacelera_utils-0.2.0.tar", last modified: Fri Apr  5 13:52:00 2024, max compression
```

## Comparing `pharmacelera_utils-0.1.60.tar` & `pharmacelera_utils-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2023-11-02 11:16:18.764874 pharmacelera_utils-0.1.60/
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    16724 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/LICENSE
--rw-r--r--   0 eherrero  (1003) eherrero  (1004)      564 2023-11-02 11:16:18.764874 pharmacelera_utils-0.1.60/PKG-INFO
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     2480 2023-11-02 10:55:35.000000 pharmacelera_utils-0.1.60/README.md
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       38 2023-11-02 11:16:18.764874 pharmacelera_utils-0.1.60/setup.cfg
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     1018 2023-11-02 11:04:24.000000 pharmacelera_utils-0.1.60/setup.py
-drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2023-11-02 11:16:18.760874 pharmacelera_utils-0.1.60/src/
-drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2023-11-02 11:16:18.760874 pharmacelera_utils-0.1.60/src/pharmacelera_utils/
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       74 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/__init__.py
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     6259 2023-11-02 10:34:29.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/commands.py
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     2323 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/errors.py
--rwxrwxr-x   0 eherrero  (1003) eherrero  (1004)    11180 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/launch.py
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     5531 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/services.py
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    10825 2023-11-02 10:43:37.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils/utils.py
-drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2023-11-02 11:16:18.760874 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/
--rw-r--r--   0 eherrero  (1003) eherrero  (1004)      564 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/PKG-INFO
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)      546 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)        1 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)      121 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/entry_points.txt
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       64 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/requires.txt
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       66 2023-11-02 11:16:18.000000 pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/top_level.txt
-drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2023-11-02 11:16:18.764874 pharmacelera_utils-0.1.60/tests/
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    10218 2023-11-02 10:47:03.000000 pharmacelera_utils-0.1.60/tests/test_cmd.py
--rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     6161 2023-10-09 22:04:11.000000 pharmacelera_utils-0.1.60/tests/test_launch.py
+drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    16724 2023-10-09 22:04:11.000000 pharmacelera_utils-0.2.0/LICENSE
+-rw-r--r--   0 eherrero  (1003) eherrero  (1004)      563 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/PKG-INFO
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     3510 2024-04-05 13:49:22.000000 pharmacelera_utils-0.2.0/README.md
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       38 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/setup.cfg
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     1018 2024-03-20 13:33:27.000000 pharmacelera_utils-0.2.0/setup.py
+drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/src/
+drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/src/pharmacelera_utils/
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       74 2023-10-09 22:04:11.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/__init__.py
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     9069 2024-03-20 13:33:27.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/commands.py
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     2323 2023-10-09 22:04:11.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/errors.py
+-rwxrwxr-x   0 eherrero  (1003) eherrero  (1004)    11180 2023-10-09 22:04:11.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/launch.py
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     6910 2024-03-20 13:33:27.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/services.py
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    11903 2024-03-20 13:33:27.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils/utils.py
+drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/
+-rw-r--r--   0 eherrero  (1003) eherrero  (1004)      563 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)      546 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)        1 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)      121 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       64 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/requires.txt
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)       66 2024-04-05 13:52:00.000000 pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/top_level.txt
+drwxrwxr-x   0 eherrero  (1003) eherrero  (1004)        0 2024-04-05 13:52:00.710480 pharmacelera_utils-0.2.0/tests/
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)    10218 2024-02-23 10:17:17.000000 pharmacelera_utils-0.2.0/tests/test_cmd.py
+-rw-rw-r--   0 eherrero  (1003) eherrero  (1004)     6161 2024-03-11 21:15:13.000000 pharmacelera_utils-0.2.0/tests/test_launch.py
```

### Comparing `pharmacelera_utils-0.1.60/LICENSE` & `pharmacelera_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmacelera_utils-0.1.60/PKG-INFO` & `pharmacelera_utils-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmacelera_utils
-Version: 0.1.60
+Version: 0.2.0
 Summary: Utility functions to execute pharmacelera scripts
 Home-page: https://bitbucket.org/pharmacelera/api-examples.git
 Author: Pharmacelera developers
 Author-email: support@pharmacelera.com
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pharmacelera_utils-0.1.60/README.md` & `pharmacelera_utils-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,32 +9,44 @@
 
 After launch an experiment, there is a helper commands to check and controll the experiments.
 
 `pharmacelera-cmd`
 
 This command accepts multiple arguments as a parameter.
 
-`--option`:  OPTION    Type of the command to call Pharmacelera endpoint. Possible options: `get`, `list`, `download`, `kill`, `remove`, `upload`. Default: `get`. Note: `list` option supports filter by status, eg: `list?status=running`.
+`--option`:  OPTION    Type of the command to call Pharmacelera endpoint. Possible options: `get`, `list`, `download`, `kill`, `remove`, `upload`, `listLib`, `removeLib`, `uploadLib`. Default: `get`. Note: `list` option supports filter by status, eg: `list?status=running`.
 
 `--id`: ID            Unique id of the experiment
 
 `--uri` URI          Host name of the endpoint. Default: http://localhost
 
 `--port` PORT        endpoint port number. Default: 8080
 
 `--type` TYPE        Type of the binary to upload: [pharmqsar, pharmscreen, exascreen]. default: pharmqsar
 
 `--binary` BINARY    Path and filename of the binary file to upload
 
 `--license` LICENSE  Path and filename of the license file to upload.
 
+`--library` LIBRARY  Path and filename of the library file to upload or remove.
+
 To get one experiment status: 
 
 `pharmacelera-cmd --uri http:127.0.0.1 --port 3000 --id 507f1f77bcf86cd799439011`
 
+## Test package
+
+Requirements:
+- Have access to the Pharmacelera API deployed at AWS (http://ec2-34-249-78-179.eu-west-1.compute.amazonaws.com:8081/home)
+- Have installed the package locally
+- Make sure the deployed API in AWS is updated
+- Make sure the AWS batch worker image is updated
+
+`run-test.sh`
+
 ## Production install
 
 ```bash
 
 install pharmacelera-utils
 
 ```
@@ -49,32 +61,56 @@
 pip install -e .
 
 ```
 
 This will use source code of the package from folder and install it as a library.
 
 ## Deployment
+There are two repositories for this package, one for production and one for preproduction.
+They can be found here:
+https://pypi.org/project/pharmacelera-utils/ (Production)
+https://test.pypi.org/project/pharmacelera-utils/ (Preproduction)
+
+### Deploy dependencies
 Install depoy dependencies
 
 ```bash
 
 pip install wheel
 pip install build
 conda install -c anaconda twine
 
 ```
 
+### Upload package to repository
 simply run `publish.sh` to deploy new version of pip package into the production. For testing purpose, run 
 `publish_test.sh` to deploy it to test.pypi.
 
+Username: __token__
+Password: Insert token here
+
 for installing it from test repo:
 
+```bash
+
 Linux: python3 -m pip install --index-url https://test.pypi.org/simple/ pharmacelera-utils
 
 Windows: py -m pip install --index-url https://test.pypi.org/simple/ pharmacelera-utils
 
+```
+
+for updating it from test repo:
+
+```bash
+
+Linux: python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ pharmacelera-utils
+
+Windows: py -m pip install --upgrade --index-url https://test.pypi.org/simple/ pharmacelera-utils
+
+```
+
 ## Known errors
 
 ERROR: Cannot install pharmacelera-utils==0.1.5, pharmacelera-utils==0.1.51 and pharmacelera-utils==0.1.52 because these package versions have conflicting dependencies.
 
 Fix: Install a specific version, e.g. pip install pharmacelera-utils==0.1.52
      Install manually the correct dependency versions
```

### Comparing `pharmacelera_utils-0.1.60/setup.py` & `pharmacelera_utils-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pharmacelera_utils",
-    version="0.1.60",
+    version="0.2.00",
     description="Utility functions to execute pharmacelera scripts",
     url="https://bitbucket.org/pharmacelera/api-examples.git",
     author="Pharmacelera developers",
     author_email="support@pharmacelera.com",
     license="Mozilla Public License Version 2.0",
     packages=find_packages(where="src"),
     install_requires=["requests==2.31.0", "PyYAML==6.0.1", "boto3==1.28.62", "botocore==1.31.62"],
```

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils/commands.py` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.init_arguments()
 
     def init_arguments(self):
         """Define cmd input arguments."""
         parser = argparse.ArgumentParser("")
         parser.add_argument(
             "--option",
-            help="Type of the command to call Pharmacelera endpoint. Possible options: get, list, download, kill, remove, upload. Default: get. Note: list option supports filter by status, eg: list?status=running.",
+            help="Type of the command to call Pharmacelera endpoint. Possible options: get, list, download, kill, remove, upload, listLib, removeLib, uploadLib. Default: get. Note: list option supports filter by status, eg: list?status=running.",
             type=str,
             default="get",
         )
         parser.add_argument("--id", help="Unique id of the experiment", type=str)
         parser.add_argument(
             "--uri", help="Host name of the endpoint. Default: http://localhost", type=str, default="http://localhost"
         )
@@ -35,14 +35,19 @@
         )
         parser.add_argument("--binary", help="Path and filename of the binary file to upload", type=str)
         parser.add_argument(
             "--license",
             help="Path and filename of the license file to upload.",
             type=str,
         )
+        parser.add_argument(
+            "--library",
+            help="Path and filename of the library file to upload or remove.",
+            type=str,
+        )
         self.args = parser.parse_args()
 
 
 class AppConfiguration:
     client: Calls
     utils: Utils
     args: argparse.Namespace
@@ -125,28 +130,86 @@
         response = self.client.upload(files)
         body = response.get("body")
         if body:
             print(f'{Colors.OKGREEN}{body.get("msg")}{Colors.ENDC}')
         else:
             print(response)
 
+    def listLib(self):
+        print(f"{Colors.BOLD}Listing libraries ...{Colors.ENDC}")
+        response = self.client.listLib()
+        if not response:
+            print(f"{Colors.FAIL}Unexpected error.{Colors.ENDC}")
+            return
+        if response.get("statusCode", None) == 200:
+            body = response.get("body", None)
+            if len(body):
+                self.printLibs(body)
+        else:
+            msg = response["body"].get("msg", None)
+            print(f"{Colors.FAIL}{msg}{Colors.ENDC}")
+
+    def removeLib(self):
+        print(f"{Colors.BOLD}Removing library ...{Colors.ENDC}")
+        library_filename = self.args.library
+        if not library_filename:
+            print(f"{Colors.FAIL}Please define library filename.{Colors.ENDC}")
+            return
+        response = self.client.removeLib(library_filename)
+        if not response:
+            print(f"{Colors.FAIL}Unexpected error.{Colors.ENDC}")
+            return
+        msg = response["body"].get("msg", None)
+        if response.get("statusCode", None) == 200:
+            print(f"{Colors.OKGREEN}{msg}{Colors.ENDC}") 
+        else:
+            print(f"{Colors.FAIL}{msg}{Colors.ENDC}")                
+
+    def uploadLib(self):
+        print(f"{Colors.BOLD}Uploading library ...{Colors.ENDC}")
+        library_path = self.args.library
+        if not library_path:
+            print(f"{Colors.FAIL}Please define library path and filename.{Colors.ENDC}")
+            return
+        files = self.utils.define_library_file(library_path)
+        if not files:
+            return
+        response = self.client.uploadLib(files)
+        if not response:
+            print(f"{Colors.FAIL}Unexpected error.{Colors.ENDC}")
+            return
+        msg = response["body"].get("msg", None)
+        if response.get("statusCode", None) == 200:
+            print(f"{Colors.OKGREEN}{msg}{Colors.ENDC}") 
+        else:
+            print(f"{Colors.FAIL}{msg}{Colors.ENDC}") 
+
     def print(self, experiment_lists):
         for index, experiment in enumerate(experiment_lists):
             print(f"{Colors.OKBLUE}Count: {index + 1}{Colors.ENDC}")
             print(120 * "-")
             single_list_experiment = list(experiment.items())
             single_list_experiment.sort(key=self.get_length)
             sorted_single_experiment = {str(elem[0]): str(elem[1]) for elem in single_list_experiment}
             colon_distance = str(len(list(sorted_single_experiment)[-1]))
             row_format = "{:<" + colon_distance + "} : {:<30}"
             for key, value in sorted_single_experiment.items():
                 if key in self.printables:
                     print(f"{Colors.OKGREEN}{row_format.format(key, value)}{Colors.ENDC}")
             print(120 * "-" + "\n")
 
+    def printLibs(self, library_list):
+        for index, library in enumerate(library_list["libraries"]):
+            print(f"{Colors.OKBLUE}Count: {index + 1}{Colors.ENDC}")
+            print(120 * "-")
+            colon_distance = str(len(list(library)[-1]))
+            row_format = "{:<" + colon_distance + "} : {:<30}"
+            print(f"{Colors.OKGREEN}{library}{Colors.ENDC}")
+            print(120 * "-" + "\n")            
+
     def get_length(self, key):
         return len(key[0])
 
     def redirect(self, option: str):
         option = option.split("?")
         query_param = option[1] if len(option) > 1 else None
         if option[0] == "get":
@@ -157,14 +220,20 @@
             return self.download()
         elif option[0] == "kill":
             return self.kill()
         elif option[0] == "remove":
             return self.remove()
         elif option[0] == "upload":
             return self.upload()
+        elif option[0] == "listLib":
+            return self.listLib()
+        elif option[0] == "removeLib":
+            return self.removeLib()
+        elif option[0] == "uploadLib":
+            return self.uploadLib()
         else:
             print("Option value is unknown.")
 
 
 def run():
     parser = ArgumentParser()
     app = AppConfiguration(parser.args)
```

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils/errors.py` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils/errors.py`

 * *Files identical despite different names*

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils/launch.py` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils/launch.py`

 * *Files identical despite different names*

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils/services.py` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils/services.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,21 +24,24 @@
         self.__path = params.get("MODEL_NAME") or ""
         self.__port = os.getenv("PORT") or params.get("PORT")
         self.__url = f"{params.get('URI')}:{self.__port}"
 
     def upload(self, files):
         """Upload binary and license inside container."""
         url = f"{self.__url}/uploadBinary"
-        response = requests.request(
-            "POST",
-            url,
-            files=files,
-        )
-        result = json.loads(response.text)
-        return result
+        try:
+            response = requests.request(
+                "POST",
+                url,
+                files=files,
+            )
+            result = json.loads(response.text)
+            return result
+        except Exception as exp:
+            self.__errors.requestException(exp)    
 
     def launch(self, endpoint, payload, files):
         """Launch an experiment with given data."""
         url = f"{self.__url}/{endpoint}"
         try:
             response = requests.request(
                 "POST",
@@ -123,14 +126,50 @@
             url = f"{self.__url}/remove?id={id}"
             response = requests.request("DELETE", url)
             result = json.loads(response.text)
             return result
         except Exception as exp:
             self.__errors.requestException(exp)
 
+    def listLib(self):
+        try:
+            """List all libraries."""
+            url = f"{self.__url}/listLibraries"
+            response = requests.request("GET", url)
+            result = json.loads(response.text)
+            return result
+        except Exception as exp:
+            self.__errors.requestException(exp)
+
+    def removeLib(self, library_filename):
+        """Remove library file."""
+        try:
+            url = f"{self.__url}/removeLibrary"
+            headers={'Content-type': 'application/json'}
+            jsondata={"file": library_filename}
+            response = requests.request("DELETE", url, headers=headers, json=jsondata, data={})
+            result = json.loads(response.text)
+            return result
+        except Exception as exp:
+            self.__errors.requestException(exp)    
+
+    def uploadLib(self, library):
+        """Upload library inside container."""
+        url = f"{self.__url}/uploadLibrary"
+        try:
+            response = requests.request(
+                "POST",
+                url,
+                files=library,
+            )
+            result = json.loads(response.text)
+            return result
+        except Exception as exp:
+            self.__errors.requestException(exp) 
+
     def extractFiles(self, zip_path, zipName):
         """Extract sdf files from compressed files."""
         dirname = pathlib.Path().absolute()
         with zipfile.ZipFile(os.path.join(dirname, zip_path, zipName)) as zipped:
             for file in zipped.namelist():
                 if (
                     file.endswith((".sdf", "mol2"))
```

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils/utils.py` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -111,14 +111,45 @@
                             open(license, "rb"),
                             "application/octet-stream",
                         ),
                     )
                 )
         return files
 
+    def define_library_file(self, library: str) -> List:
+        """Define library file names.
+        Args:
+            library (str): path and filename of the library file
+
+        Returns:
+            files (list): list of the opened library file stream.
+        """
+        files = []
+        abs_path: str = Path().absolute()
+        lib_name = os.path.basename(library)
+        if library:
+            if not isabs(library):
+                library = os.path.join(abs_path, library)
+            if not isfile(library):
+                print(
+                    f"{Colors.FAIL}Could not find the library, please make sure library is in the current folder or use absolute path.{Colors.ENDC}"
+                )
+            else:
+                files.append(
+                    (
+                        "library",
+                        (
+                            lib_name,
+                            open(library, "rb"),
+                            "application/octet-stream",
+                        ),
+                    )
+                )
+        return files
+
     def best_model_selector(self, folder_path, statics, config=None):
         """Unzip all output files and list all log files,
         then parse line by line to extract the best component among all experiments
         """
         all_components = []
         self.best = statics["MODEL_NAME"]
         self.upload = statics["UPLOAD_S3"]
```

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/PKG-INFO` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pharmacelera-utils
-Version: 0.1.60
+Name: pharmacelera_utils
+Version: 0.2.0
 Summary: Utility functions to execute pharmacelera scripts
 Home-page: https://bitbucket.org/pharmacelera/api-examples.git
 Author: Pharmacelera developers
 Author-email: support@pharmacelera.com
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pharmacelera_utils-0.1.60/src/pharmacelera_utils.egg-info/SOURCES.txt` & `pharmacelera_utils-0.2.0/src/pharmacelera_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pharmacelera_utils-0.1.60/tests/test_cmd.py` & `pharmacelera_utils-0.2.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `pharmacelera_utils-0.1.60/tests/test_launch.py` & `pharmacelera_utils-0.2.0/tests/test_launch.py`

 * *Files identical despite different names*

