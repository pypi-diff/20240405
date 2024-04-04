# Comparing `tmp/licensecheck-2024.1.4.tar.gz` & `tmp/licensecheck-2024.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensecheck-2024.1.4.tar", max compression
+gzip compressed data, was "licensecheck-2024.1.5.tar", max compression
```

## Comparing `licensecheck-2024.1.4.tar` & `licensecheck-2024.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2024.1.4/LICENSE.md
-drwxr-xr-x   0        0        0        0 2024-03-20 17:37:00.918045 licensecheck-2024.1.4/licensecheck/
--rw-r--r--   0        0        0      103 2024-03-20 17:39:18.275010 licensecheck-2024.1.4/licensecheck/__init__.py
--rw-r--r--   0        0        0      119 2024-03-16 10:43:41.079320 licensecheck-2024.1.4/licensecheck/__main__.py
--rw-r--r--   0        0        0     4472 2024-03-20 18:00:48.751286 licensecheck-2024.1.4/licensecheck/cli.py
--rw-r--r--   0        0        0     7512 2024-03-20 17:39:18.489008 licensecheck-2024.1.4/licensecheck/formatter.py
--rw-r--r--   0        0        0     7672 2024-03-20 18:03:25.397881 licensecheck-2024.1.4/licensecheck/get_deps.py
--rw-r--r--   0        0        0     4978 2024-03-20 18:07:07.760013 licensecheck-2024.1.4/licensecheck/license_matrix.py
--rw-r--r--   0        0        0     1789 2024-03-17 13:05:01.686551 licensecheck-2024.1.4/licensecheck/matrix.csv
--rw-r--r--   0        0        0     6053 2024-03-30 14:40:39.106973 licensecheck-2024.1.4/licensecheck/packageinfo.py
--rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2024.1.4/licensecheck/pypi_licenses/osi_approved.txt
--rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2024.1.4/licensecheck/pypi_licenses/other.txt
--rw-r--r--   0        0        0      134 2024-03-20 17:39:18.486705 licensecheck-2024.1.4/licensecheck/session.py
--rw-r--r--   0        0        0     1782 2024-03-20 18:04:09.591540 licensecheck-2024.1.4/licensecheck/types.py
--rw-r--r--   0        0        0     2512 2024-03-30 14:41:44.121115 licensecheck-2024.1.4/pyproject.toml
--rw-r--r--   0        0        0    25718 2024-03-16 09:12:32.791095 licensecheck-2024.1.4/README.md
--rw-r--r--   0        0        0    27423 1970-01-01 00:00:00.000000 licensecheck-2024.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-01-01 17:53:39.457996 licensecheck-2024.1.5/LICENSE.md
+drwxr-xr-x   0        0        0        0 2024-03-20 17:37:00.918045 licensecheck-2024.1.5/licensecheck/
+-rw-r--r--   0        0        0      103 2024-03-20 17:39:18.275010 licensecheck-2024.1.5/licensecheck/__init__.py
+-rw-r--r--   0        0        0      119 2024-03-16 10:43:41.079320 licensecheck-2024.1.5/licensecheck/__main__.py
+-rw-r--r--   0        0        0     4472 2024-03-20 18:00:48.751286 licensecheck-2024.1.5/licensecheck/cli.py
+-rw-r--r--   0        0        0     7512 2024-03-20 17:39:18.489008 licensecheck-2024.1.5/licensecheck/formatter.py
+-rw-r--r--   0        0        0     7672 2024-03-20 18:03:25.397881 licensecheck-2024.1.5/licensecheck/get_deps.py
+-rw-r--r--   0        0        0     4978 2024-03-20 18:07:07.760013 licensecheck-2024.1.5/licensecheck/license_matrix.py
+-rw-r--r--   0        0        0     1789 2024-03-17 13:05:01.686551 licensecheck-2024.1.5/licensecheck/matrix.csv
+-rw-r--r--   0        0        0     6143 2024-04-04 21:59:45.051523 licensecheck-2024.1.5/licensecheck/packageinfo.py
+-rw-r--r--   0        0        0     2459 2023-01-01 17:53:39.466968 licensecheck-2024.1.5/licensecheck/pypi_licenses/osi_approved.txt
+-rw-r--r--   0        0        0      652 2023-01-01 17:53:39.466968 licensecheck-2024.1.5/licensecheck/pypi_licenses/other.txt
+-rw-r--r--   0        0        0      134 2024-03-20 17:39:18.486705 licensecheck-2024.1.5/licensecheck/session.py
+-rw-r--r--   0        0        0     1782 2024-03-20 18:04:09.591540 licensecheck-2024.1.5/licensecheck/types.py
+-rw-r--r--   0        0        0     2512 2024-04-04 22:02:29.554640 licensecheck-2024.1.5/pyproject.toml
+-rw-r--r--   0        0        0    25718 2024-03-16 09:12:32.791095 licensecheck-2024.1.5/README.md
+-rw-r--r--   0        0        0    27423 1970-01-01 00:00:00.000000 licensecheck-2024.1.5/PKG-INFO
```

### Comparing `licensecheck-2024.1.4/LICENSE.md` & `licensecheck-2024.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/cli.py` & `licensecheck-2024.1.5/licensecheck/cli.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/formatter.py` & `licensecheck-2024.1.5/licensecheck/formatter.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/get_deps.py` & `licensecheck-2024.1.5/licensecheck/get_deps.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/license_matrix.py` & `licensecheck-2024.1.5/licensecheck/license_matrix.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/matrix.csv` & `licensecheck-2024.1.5/licensecheck/matrix.csv`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/packageinfo.py` & `licensecheck-2024.1.5/licensecheck/packageinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Get information for installed and online packages."""
 
 from __future__ import annotations
 
 import configparser
 import contextlib
+from collections.abc import Iterable
 from importlib import metadata
 from pathlib import Path
 from typing import Any
 
 import tomli
 
 from licensecheck.session import session
 from licensecheck.types import JOINS, UNKNOWN, PackageInfo, ucstr
 
 
 def _pkgMetadataGet(pkgMetadata: metadata.PackageMetadata | dict[str, Any], key: str) -> str:
 	"""Get a string from a key from pkgMetadata."""
 	value = pkgMetadata.get(key, UNKNOWN)
-	if not isinstance(value, str):
-		value = JOINS.join(value)
-	return value or UNKNOWN
+	if not isinstance(value, str) and isinstance(value, Iterable):
+		value = JOINS.join(str(x) for x in value)
+	return str(value) or UNKNOWN
 
 
 def getPackageInfoLocal(requirement: ucstr) -> PackageInfo:
 	"""Get package info from local files including version, author
 	and	the license.
 
 	:param str requirement: name of the package
```

### Comparing `licensecheck-2024.1.4/licensecheck/pypi_licenses/osi_approved.txt` & `licensecheck-2024.1.5/licensecheck/pypi_licenses/osi_approved.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/pypi_licenses/other.txt` & `licensecheck-2024.1.5/licensecheck/pypi_licenses/other.txt`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/licensecheck/types.py` & `licensecheck-2024.1.5/licensecheck/types.py`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/pyproject.toml` & `licensecheck-2024.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "licensecheck"
-version = "2024.1.4"
+version = "2024.1.5"
 license = "mit"
 description = "Output the licenses used by dependencies and check if these are compatible with the project license"
 authors = ["FredHappyface"]
 classifiers = [
 	"Environment :: Console",
 	"Environment :: MacOS X",
 	"Environment :: Win32 (MS Windows)",
```

### Comparing `licensecheck-2024.1.4/README.md` & `licensecheck-2024.1.5/README.md`

 * *Files identical despite different names*

### Comparing `licensecheck-2024.1.4/PKG-INFO` & `licensecheck-2024.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensecheck
-Version: 2024.1.4
+Version: 2024.1.5
 Summary: Output the licenses used by dependencies and check if these are compatible with the project license
 Home-page: https://github.com/FHPythonUtils/LicenseCheck
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

