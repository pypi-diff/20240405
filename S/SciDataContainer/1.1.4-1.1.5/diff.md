# Comparing `tmp/scidatacontainer-1.1.4.tar.gz` & `tmp/scidatacontainer-1.1.5.tar.gz`

## Comparing `scidatacontainer-1.1.4.tar` & `scidatacontainer-1.1.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/Makefile
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/VERSION
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/build.bat
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/clean.bat
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/requirements.txt
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/setup.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/test_requirements.txt
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/Makefile
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/__init__.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/config.py
--rw-r--r--   0        0        0    25263 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/container.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/filebase.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/fileimage.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/filenumpy.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/jsonschema/SciDataContainer.content.1.0.0.schema.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/jsonschema/SciDataContainer.meta.1.0.0.schema.json
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/jsonschema/__init__.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/__init__.py
--rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/_abstract_container_test.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_config.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_download.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_filebinary.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_fileimage.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_filenumpy.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_filetext.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_json_schema.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_multistep_container.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_register_class.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_single_step_container.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_static_container.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/scidatacontainer/tests/test_upload.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/LICENSE
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 scidatacontainer-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/Makefile
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/VERSION
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/build.bat
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/clean.bat
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/requirements.txt
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/setup.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/test_requirements.txt
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/Makefile
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/config.py
+-rw-r--r--   0        0        0    27025 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/container.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/filebase.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/fileimage.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/filenumpy.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/jsonschema/SciDataContainer.content.1.0.0.schema.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/jsonschema/SciDataContainer.meta.1.0.0.schema.json
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/jsonschema/__init__.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/__init__.py
+-rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/_abstract_container_test.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_config.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_download.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_filebinary.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_fileimage.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_filenumpy.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_filetext.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_json_schema.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_multistep_container.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_orcid.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_register_class.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_single_step_container.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_static_container.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/scidatacontainer/tests/test_upload.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 scidatacontainer-1.1.5/PKG-INFO
```

### Comparing `scidatacontainer-1.1.4/Makefile` & `scidatacontainer-1.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/setup.py` & `scidatacontainer-1.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 
 from distutils.core import setup
 
 import setuptools  # noqa: F401 - required for command bdist_wheel
 
-version = "1.1.4"
+version = "1.1.5"
 
 with open("VERSION", "w") as fp:
     fp.write(version)
 
 with open("README.md", "r") as fp:
     readme = fp.read()
```

### Comparing `scidatacontainer-1.1.4/scidatacontainer/Makefile` & `scidatacontainer-1.1.5/scidatacontainer/Makefile`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/__init__.py` & `scidatacontainer-1.1.5/scidatacontainer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##########################################################################
-# Copyright (c) 2023 Reinhard Caspary                                    #
+# Copyright (c) 2023-2024 Reinhard Caspary                               #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
 # This package provides the Scientific Data Container as class Container
 # which may be stored as a ZIP package containing items (files). Based
 # on their file extension, the following item types are supported:
@@ -21,26 +21,28 @@
 # such a conversion class.
 #
 ##########################################################################
 
 __all__ = [
     "timestamp",
     "modelVersion",
+    "load_config",
     "register",
     "Container",
 ]
 
 import typing
 from importlib import import_module
 
+from .config import load_config
 from .container import MODELVERSION as modelVersion
 from .container import AbstractContainer, timestamp
 from .filebase import AbstractFile
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 suffixes = {}
 classes = {}
 formats = []
 
 
 def register(
```

### Comparing `scidatacontainer-1.1.4/scidatacontainer/config.py` & `scidatacontainer-1.1.5/scidatacontainer/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ##########################################################################
-# Copyright (c) 2023 Reinhard Caspary                                    #
+# Copyright (c) 2023-2024 Reinhard Caspary                               #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
-# This module provides the function getconfig() to read the default
+# This module provides the function load_config() to read the default
 # configuration parameters
 #
-# Parameter    | key
-# -------------+--------
-# author name  | author
-# author email | email
-# server URL   | server
-# server key   | key
+# Parameter           | key
+# --------------------+--------
+# author name         | author
+# author email        | email
+# author ORCiD        | orcid
+# author organization | organization
+# server URL          | server
+# server key          | key
 #
 # The values of these parameters are taken either from environment
 # variables or a config file. Both options are optional. Data from the
 # config file overides the environment variables.
 #
 # The name of the environment variable of key foo is DC_FOO.
 #
@@ -29,56 +31,75 @@
 #
 ##########################################################################
 
 import os
 import platform
 
 
-def load_config(config_path: str = None) -> dict:
-    """Get config data from environment variables and config file.
+def load_config(config_path: str = None, **kwargs) -> dict:
+    """Get author identity and server configuration.
 
-    This functions prefers values in the scidata config file and potentially
-    overwrites values that are present as environmental variables.
+    This function uses kwargs, the scidata config file and environmental
+    variables as sources for each parameter. The former sources
+    overriding the latter ones.
 
-    Usually, users doen't need to call this function. However, it can be used
-    for debugging purposes if the configuration parameters are not as expected.
+    Users may use the result of this function to inject the author
+    identity when building a new container:
+
+    config = load_config(author="John Doe", email="john@doe.com")
+    dc = Container(config=config)
 
     Args:
         str: Path of the config file. If this is None, the default file will
              be used. This filename is only required for testing.
 
+        kwargs: Parameter values as keyword arguments.
+
     Returns:
         dict: A dictionary containing information strings with keys "author",\
-              "email", "server", "key".
+              "email", "orcid", "organization", "server", "key".
     """
 
     # Initialize config dictionary
-    config = {"author": "", "email": "", "server": "", "key": ""}
+    config = {
+        "author": "",
+        "email": "",
+        "orcid": "",
+        "organization": "",
+        "server": "",
+        "key": "",
+    }
 
     # Get default values from environment variables
     for key in config:
         name = "DC_%s" % key.upper()
         if name in os.environ:
-            config[key] = os.environ[name]
+            config[key] = os.environ[name].strip()
 
-    # Get default values from config file
+    # Path to scidata config file
     if not config_path:
         if platform.system() == "Windows":
             config_path = os.path.join(os.path.expanduser("~"), "scidata.cfg")
         else:
             config_path = os.path.join(os.path.expanduser("~"), ".scidata")
 
+    # Get default values from config file
     if os.path.exists(config_path):
         with open(config_path, "r") as fp:
             for line in fp.readlines():
                 line = line.strip()
                 if line[:1] == "#":
                     continue
                 line = line.split("=", 1)
                 if len(line) < 2:
                     continue
                 key = line[0].strip().lower()
                 if key in config:
                     config[key] = line[1].strip()
 
+    # Use keyword arguments
+    for key in config:
+        if key in kwargs:
+            config[key] = kwargs[key].strip()
+
     # Return config dictionary
     return config
```

### Comparing `scidatacontainer-1.1.4/scidatacontainer/container.py` & `scidatacontainer-1.1.5/scidatacontainer/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##########################################################################
-# Copyright (c) 2023 Reinhard Caspary                                    #
+# Copyright (c) 2023-2024 Reinhard Caspary                               #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
 # This module provides the Scientific Data Container as class
 # DataContainer which may be stored or uploaded as a ZIP package
 # containing items (files). Do not use this class directly! Use the
@@ -23,16 +23,14 @@
 from zipfile import ZIP_DEFLATED, ZipFile
 
 import requests
 
 from .config import load_config
 from .filebase import BinaryFile, JsonFile, TextFile
 
-config = load_config()
-
 # Version of the implemented data model
 MODELVERSION = "1.0.0"
 
 
 ##########################################################################
 # Timestamp function
 
@@ -55,28 +53,25 @@
 
     The following file types are supported:
         - .json <-> dict
         - .txt <-> str
         - .bin <-> bytes
     """
 
-    _config = config
+    _config = None
     _suffixes = {"json": JsonFile, "txt": TextFile, "bin": BinaryFile}
     _classes = {dict: JsonFile, str: TextFile, bytes: BinaryFile}
     _formats = [TextFile]
 
     def __init__(
         self,
         items: dict = None,
         file: str = None,
         uuid: str = None,
-        author: str = None,
-        email: str = None,
-        server: str = None,
-        key: str = None,
+        config: dict = None,
         compression: int = ZIP_DEFLATED,
         compresslevel: int = -1,
         **kwargs,
     ):
         """Construct a DataContainer object.
 
         It will try the following in the specified order:
@@ -95,55 +90,59 @@
             compression: Numeric constant for the compression method
             compresslevel: Level of compression, 0-fastest, 9-best compression
         """
         self.kwargs = {
             "items": items,
             "file": file,
             "uuid": uuid,
-            "author": author,
-            "email": email,
-            "server": server,
-            "key": key,
+            "config": config,
             "compression": compression,
             "compresslevel": compresslevel,
         }
         self.kwargs.update(kwargs)
 
         self.__pre_init__()
 
-        # load variables from kwargs in namespace
+        # Load variables from kwargs in namespace
         n = SimpleNamespace(**self.kwargs)
 
         # Container must be mutable initially
         self.mutable = True
 
+        # Load configuration
+        if n.config is not None:
+            self._config = dict(n.config)
+        else:
+            self._config = load_config()
+
         # Store all items in the container
         if n.items is not None:
-            if n.author is not None:
-                n.items["meta.json"]["author"] = n.author
-            if n.email is not None:
-                n.items["meta.json"]["email"] = n.email
             self._store(n.items, True, False)
             self.mutable = not self["content.json"]["static"]
 
         # Load local container file
         elif n.file is not None:
             self._read(fn=n.file)
 
         # Download container from server
         elif n.uuid is not None:
-            self._download(uuid=n.uuid, server=n.server, key=n.key)
+            server = self._config["server"]
+            key = self._config["key"]
+            self._download(uuid=n.uuid, server=server, key=key)
 
         # No data source
         else:
             raise RuntimeError("No data!")
 
         self.compression = n.compression
         self.compresslevel = n.compresslevel
 
+        # Check validity of author ORCID
+        self._norm_orcid()
+
         self.__post_init__()
 
     def __pre_init__(self):
         """Manipulate the container before initialization.
 
         This method can be overwritten by inheriting classes to manipulate the
         container object or the arguments passed to __init__ before the
@@ -359,17 +358,21 @@
         if not meta["author"]:
             raise RuntimeError("Author name is missing!")
 
         # Author email address is required
         if "email" not in meta:
             meta["email"] = self._config["email"]
 
+        # Author ORCiD is optional
+        if "orcid" not in meta:
+            meta["orcid"] = self._config["orcid"]
+
         # Author affiliation is optional
         if "organization" not in meta:
-            meta["organization"] = ""
+            meta["organization"] = self._config["organization"]
 
         # Comment on dataset is optional
         if "comment" not in meta:
             meta["comment"] = ""
 
         # Title of dataset is required
         if "title" not in meta:
@@ -482,14 +485,18 @@
             content.pop(key, None)
         self.validate_content()
 
     def encode(self):
         """Encode container as ZIP package. Return package as binary
         string.
         """
+
+        # Check/format of author ORCID
+        self._norm_orcid()
+
         items = {p: self._items[p].encode() for p in self.items()}
         with io.BytesIO() as f:
             with ZipFile(
                 f,
                 "w",
                 compression=self.compression,
                 compresslevel=self.compresslevel,
@@ -706,7 +713,59 @@
         if content["hash"]:
             s.append("  hash:        " + content["hash"])
         s.append("  created:     " + content["created"])
         s.append("  storageTime: " + content["storageTime"])
         s.append("  author:      " + meta["author"])
 
         return "\n".join(s)
+
+    def _norm_orcid(self, orcid: typing.Optional[str] = None) -> None:
+        """Set ORCID to normalized string if the given string is a valid ORCiD
+        or to an empty string otherwise."""
+
+        if orcid is None:
+            orcid = self["meta.json"]["orcid"]
+
+        assert isinstance(orcid, str)
+
+        # Pick all digits and normalize
+        orcid = orcid.replace("-", "").replace(" ", "").upper()
+        if len(orcid) != 16:
+            self["meta.json"]["orcid"] = ""
+            return
+
+        # Check if ORCID is in the correct number space.
+        try:
+            orcid_number = int(orcid[:-1])
+        except ValueError:
+            self["meta.json"]["orcid"] = ""
+            return
+
+        if not (
+            (15000000 <= int(orcid_number) <= 35000000)
+            or (900000000000 <= int(orcid_number) <= 900100000000)
+        ):
+            self["meta.json"]["orcid"] = ""
+            return
+
+        # Calculate checksum product
+        r = 2
+        m = 11
+        try:
+            product = 0
+            for digit in orcid[:-1]:
+                product = ((int(digit) + product) * r) % m
+        except ValueError:
+            self["meta.json"]["orcid"] = ""
+            return
+
+        # Calculate checksum digit
+        checksum = (m + 1 - product) % m
+        check = "0123456789X"[checksum]
+        if orcid[-1] != check:
+            self["meta.json"]["orcid"] = ""
+            return
+
+        # Valid ORCID. Set orcid variable to formatted string
+        self["meta.json"]["orcid"] = (
+            orcid[:4] + "-" + orcid[4:8] + "-" + orcid[8:12] + "-" + orcid[12:]
+        )
```

### Comparing `scidatacontainer-1.1.4/scidatacontainer/filebase.py` & `scidatacontainer-1.1.5/scidatacontainer/filebase.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/fileimage.py` & `scidatacontainer-1.1.5/scidatacontainer/fileimage.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/filenumpy.py` & `scidatacontainer-1.1.5/scidatacontainer/filenumpy.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/jsonschema/SciDataContainer.content.1.0.0.schema.json` & `scidatacontainer-1.1.5/scidatacontainer/jsonschema/SciDataContainer.content.1.0.0.schema.json`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/jsonschema/SciDataContainer.meta.1.0.0.schema.json` & `scidatacontainer-1.1.5/scidatacontainer/jsonschema/SciDataContainer.meta.1.0.0.schema.json`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/jsonschema/__init__.py` & `scidatacontainer-1.1.5/scidatacontainer/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/__init__.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/_abstract_container_test.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/_abstract_container_test.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_config.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_download.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_filebinary.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_filebinary.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_fileimage.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_fileimage.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_filenumpy.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_filenumpy.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_filetext.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_filetext.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_json_schema.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_multistep_container.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_multistep_container.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_register_class.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_register_class.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_single_step_container.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_single_step_container.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_static_container.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_static_container.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/scidatacontainer/tests/test_upload.py` & `scidatacontainer-1.1.5/scidatacontainer/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/.gitignore` & `scidatacontainer-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/LICENSE` & `scidatacontainer-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/README.md` & `scidatacontainer-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scidatacontainer-1.1.4/pyproject.toml` & `scidatacontainer-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SciDataContainer"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Reinhard Caspary", email="reinhard.caspary@phoenixd.uni-hannover.de" },
 ]
 description = "A container class for the storage of scientific data together with meta data."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `scidatacontainer-1.1.4/PKG-INFO` & `scidatacontainer-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: SciDataContainer
-Version: 1.1.4
+Version: 1.1.5
 Summary: A container class for the storage of scientific data together with meta data.
 Project-URL: Homepage, https://github.com/SciDataContainer/SciDataContainer
 Project-URL: Documentation, https://scidatacontainer.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/SciDataContainer/SciDataContainer/issues
 Author-email: Reinhard Caspary <reinhard.caspary@phoenixd.uni-hannover.de>
 License: MIT License
```

