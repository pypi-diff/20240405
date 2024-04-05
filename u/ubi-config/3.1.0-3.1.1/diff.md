# Comparing `tmp/ubi-config-3.1.0.tar.gz` & `tmp/ubi-config-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubi-config-3.1.0.tar", last modified: Fri Nov 10 10:28:27 2023, max compression
+gzip compressed data, was "ubi-config-3.1.1.tar", last modified: Fri Apr  5 08:17:42 2024, max compression
```

## Comparing `ubi-config-3.1.0.tar` & `ubi-config-3.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-11-10 10:28:17.000000 ubi-config-3.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35069 2023-11-10 10:28:17.000000 ubi-config-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-10 10:28:17.000000 ubi-config-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-11-10 10:28:27.810157 ubi-config-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-11-10 10:28:17.000000 ubi-config-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-10 10:28:17.000000 ubi-config-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 10:28:27.810157 ubi-config-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-11-10 10:28:17.000000 ubi-config-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubi_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-11-10 10:28:27.000000 ubi-config-3.1.0/ubi_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-11-10 10:28:27.000000 ubi-config-3.1.0/ubi_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 10:28:27.000000 ubi-config-3.1.0/ubi_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-10 10:28:27.000000 ubi-config-3.1.0/ubi_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-10 10:28:27.000000 ubi-config-3.1.0/ubi_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/_impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/_impl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/_impl/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/_impl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/_impl/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/_impl/loaders/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/_impl/loaders/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/config_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/config_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/config_types/content_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/config_types/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/config_types/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/config_types/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/ubi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:27.810157 ubi-config-3.1.0/ubiconfig/utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/utils/api/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/utils/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-10 10:28:17.000000 ubi-config-3.1.0/ubiconfig/utils/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-05 08:17:30.000000 ubi-config-3.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35069 2024-04-05 08:17:30.000000 ubi-config-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 08:17:30.000000 ubi-config-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-05 08:17:42.407559 ubi-config-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-05 08:17:30.000000 ubi-config-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 08:17:30.000000 ubi-config-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:17:42.407559 ubi-config-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-05 08:17:30.000000 ubi-config-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubi_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-05 08:17:42.000000 ubi-config-3.1.1/ubi_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 08:17:42.000000 ubi-config-3.1.1/ubi_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:17:42.000000 ubi-config-3.1.1/ubi_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 08:17:42.000000 ubi-config-3.1.1/ubi_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 08:17:42.000000 ubi-config-3.1.1/ubi_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/_impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/_impl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/_impl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/_impl/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/_impl/loaders/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/_impl/loaders/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/config_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/config_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/config_types/content_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/config_types/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/config_types/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/config_types/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/ubi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:42.407559 ubi-config-3.1.1/ubiconfig/utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/utils/api/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/utils/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 08:17:30.000000 ubi-config-3.1.1/ubiconfig/utils/config_validation.py
```

### Comparing `ubi-config-3.1.0/CHANGELOG.md` & `ubi-config-3.1.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 - n/a
 
+## [v3.1.1] - 2024-04-05
+
+### Changed
+
+- `LocalLoader` is now able to load files from directories with custom names
+- Improved `GitLabLoader` logging
+
 ## [v3.1.0] - 2023-11-10
 
 ### Added
 
 - `GitlabLoader` now retries failed requests to GitLab
 
 ## [v3.0.0] - 2023-08-29
```

### Comparing `ubi-config-3.1.0/LICENSE` & `ubi-config-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/PKG-INFO` & `ubi-config-3.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubi-config
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Python Library for accessing Universal Base Image configuration
 Home-page: https://github.com/release-engineering/ubi-config
 Author: 
 Author-email: 
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/ubi-config/
 Description:
```

### Comparing `ubi-config-3.1.0/README.md` & `ubi-config-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/setup.py` & `ubi-config-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="ubi-config",
-    version="3.1.0",
+    version="3.1.1",
     author="",
     author_email="",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ubiconfig": ["utils/config_schema.json"]},
     url="https://github.com/release-engineering/ubi-config",
     license="GNU General Public License",
     description=get_description(),
```

### Comparing `ubi-config-3.1.0/ubi_config.egg-info/PKG-INFO` & `ubi-config-3.1.1/ubi_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubi-config
-Version: 3.1.0
+Version: 3.1.1
 Summary: A Python Library for accessing Universal Base Image configuration
 Home-page: https://github.com/release-engineering/ubi-config
 Author: 
 Author-email: 
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/ubi-config/
 Description:
```

### Comparing `ubi-config-3.1.0/ubi_config.egg-info/SOURCES.txt` & `ubi-config-3.1.1/ubi_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/_impl/loaders/base.py` & `ubi-config-3.1.1/ubiconfig/_impl/loaders/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+import re
+
+PREFIX_VERSION_RE = re.compile(
+    r"^(?P<prefix>[A-Za-z_-]{1,25})(?P<default_version>[\d]{1,2})(\.(?P<minor_version>[\d]{1,2}))?$"
+)
+
+
 class Loader(object):
     """Load UBI configuration.
 
     Don't construct instances of this class directly;
     use the :func:`~ubiconfig.get_loader` function.
     """
```

### Comparing `ubi-config-3.1.0/ubiconfig/_impl/loaders/gitlab.py` & `ubi-config-3.1.1/ubiconfig/_impl/loaders/gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 from urllib3 import Retry
 from requests.adapters import HTTPAdapter
 
 from ubiconfig.utils.api.gitlab import RepoApi
 from ubiconfig.utils.config_validation import validate_config
 from ubiconfig.config_types import UbiConfig
 
-from .base import Loader
+from .base import Loader, PREFIX_VERSION_RE
 
 LOG = logging.getLogger("ubiconfig")
 
-BRANCH_RE = re.compile(r"^(?P<prefix>[\w-]{1,25})(?P<default_version>[\d]{1,2})")
-
 GITLAB_RETRIES = int(os.getenv("UBICONFIG_GITLAB_RETRIES", "5"))
 GITLAB_BACKOFF = float(os.getenv("UBICONFIG_GITLAB_BACKOFF", "0.5"))
 
 
 class GitlabLoader(Loader):
     """Load configuration from a remote repo on gitlab."""
 
@@ -80,15 +78,15 @@
             )
 
         if file_name not in self._files_branch_map:
             raise ValueError(
                 "Couldn't find file %s from remote repo %s" % (file_name, self._url)
             )
 
-        match = re.match(BRANCH_RE, version)
+        match = re.match(PREFIX_VERSION_RE, version)
         if not match:
             raise ValueError("Invalid version (branch name) %s" % version)
 
         prefix = match.group("prefix")
         default_version = match.group("default_version")
 
         default_branch = f"{prefix}{default_version}"
@@ -161,15 +159,15 @@
 
         return files_branch_map
 
     def _get_branches(self):
         """Get a {branch: sha1} mapping for all branches of a given repo"""
         branch_sha1 = {}
 
-        LOG.info("Getting branches of the repo")
+        LOG.info("Getting branches of the repo %s", self._url)
         branches_list_api = self._repo_api.get_branch_list_api()
         response = self.do_request(method="GET", url=branches_list_api)
         data = self.try_json(response)
 
         if not data:
             raise RuntimeError("Please check %s is in right format" % self._url)
         for b in data:
```

### Comparing `ubi-config-3.1.0/ubiconfig/_impl/loaders/local.py` & `ubi-config-3.1.1/ubiconfig/_impl/loaders/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 
 import yaml
 from jsonschema.exceptions import ValidationError
 
 from ubiconfig.utils.config_validation import validate_config
 from ubiconfig.config_types import UbiConfig
-
+from .base import PREFIX_VERSION_RE
 
 LOG = logging.getLogger("ubiconfig")
 
 
 class LocalLoader(object):
     """Load configuration from a local directory tree."""
 
@@ -44,31 +44,33 @@
         if not self._isroot:
             file_path = os.path.join(self._path, file_name)
         else:
             file_path = file_name
 
         if version is None:
             # get version from path, such as configs/ubi7.1/config.yaml, get
-            # ubi7.1.
+            # ubi7.1
             version = os.path.basename(os.path.dirname(os.path.abspath(file_path)))
 
-        if not re.search(r"ubi[0-9]\.[0-9]{1,2}$|ubi[0-9]$", version):
+        match = re.match(PREFIX_VERSION_RE, version)
+
+        if not match:
             raise ValueError(
-                "Expect directories named in format ubi[0-9].([0-9]{1,2})$' or ubi[0-9]$, but got %s"
-                % version
+                f"Expected directories named in format '<PREFIX><MAJOR_VERSION>[.<MINOR_VERSION>]', but got {version}"
             )
+        prefix = match.group("prefix")
 
         LOG.info("Loading configuration file locally: %s", file_path)
 
         with open(file_path, "r") as f:
             config_dict = yaml.load(f, Loader=yaml.BaseLoader)
         # validate input data
         validate_config(config_dict)
 
-        return UbiConfig.load_from_dict(config_dict, file_name, version[3:])
+        return UbiConfig.load_from_dict(config_dict, file_name, version.lstrip(prefix))
 
     def load_all(self):
         """Load all config file from a local directory and all its subdirectories"""
 
         ubi_configs = []
         self._isroot = True
```

### Comparing `ubi-config-3.1.0/ubiconfig/config_types/__init__.py` & `ubi-config-3.1.1/ubiconfig/config_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/config_types/content_sets.py` & `ubi-config-3.1.1/ubiconfig/config_types/content_sets.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/config_types/flags.py` & `ubi-config-3.1.1/ubiconfig/config_types/flags.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/config_types/modules.py` & `ubi-config-3.1.1/ubiconfig/config_types/modules.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/config_types/packages.py` & `ubi-config-3.1.1/ubiconfig/config_types/packages.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/ubi.py` & `ubi-config-3.1.1/ubiconfig/ubi.py`

 * *Files identical despite different names*

### Comparing `ubi-config-3.1.0/ubiconfig/utils/api/gitlab.py` & `ubi-config-3.1.1/ubiconfig/utils/api/gitlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """provide gitlab api used to read repositories"""
+
 import os
 import re
 
 from urllib.parse import urljoin
 
 
 DEFAULT_GIT_LAB_URL_FMT = re.compile(r"(?P<host>.+com|org|net)/(?P<project>.+)")
```

### Comparing `ubi-config-3.1.0/ubiconfig/utils/config_schema.json` & `ubi-config-3.1.1/ubiconfig/utils/config_schema.json`

 * *Files identical despite different names*

