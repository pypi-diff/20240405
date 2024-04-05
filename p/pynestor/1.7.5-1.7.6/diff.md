# Comparing `tmp/pynestor-1.7.5.tar.gz` & `tmp/pynestor-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynestor-1.7.5.tar", last modified: Tue Mar 26 15:13:24 2024, max compression
+gzip compressed data, was "pynestor-1.7.6.tar", last modified: Fri Apr  5 07:25:03 2024, max compression
```

## Comparing `pynestor-1.7.5.tar` & `pynestor-1.7.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:13:24.326557 pynestor-1.7.5/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-03-26 15:13:24.326557 pynestor-1.7.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-15 14:47:04.000000 pynestor-1.7.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      600 2024-03-15 14:47:04.000000 pynestor-1.7.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-03-26 15:13:24.326557 pynestor-1.7.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:13:24.326557 pynestor-1.7.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:13:24.326557 pynestor-1.7.5/src/pynestor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-15 14:47:04.000000 pynestor-1.7.5/src/pynestor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2641 2024-03-15 14:47:04.000000 pynestor-1.7.5/src/pynestor/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-03-15 14:47:04.000000 pynestor-1.7.5/src/pynestor/default-preview-nestor-cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)    19961 2024-03-26 15:09:29.000000 pynestor-1.7.5/src/pynestor/preview_odoo_nestor.py
--rw-rw-rw-   0 root         (0) root         (0)    20508 2024-03-15 14:47:04.000000 pynestor-1.7.5/src/pynestor/pynestor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:13:24.326557 pynestor-1.7.5/src/pynestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-03-26 15:13:24.000000 pynestor-1.7.5/src/pynestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      368 2024-03-26 15:13:24.000000 pynestor-1.7.5/src/pynestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 15:13:24.000000 pynestor-1.7.5/src/pynestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-26 15:13:24.000000 pynestor-1.7.5/src/pynestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-26 15:13:24.000000 pynestor-1.7.5/src/pynestor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-05 07:25:03.124643 pynestor-1.7.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-04 11:40:06.000000 pynestor-1.7.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      600 2024-03-15 14:47:04.000000 pynestor-1.7.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-05 07:25:03.124643 pynestor-1.7.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.120643 pynestor-1.7.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.120643 pynestor-1.7.6/src/pynestor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2641 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/default-preview-nestor-cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)    20913 2024-04-04 11:40:06.000000 pynestor-1.7.6/src/pynestor/preview_odoo_nestor.py
+-rw-rw-rw-   0 root         (0) root         (0)    20612 2024-04-04 09:32:46.000000 pynestor-1.7.6/src/pynestor/pynestor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/src/pynestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2024-04-04 11:40:06.000000 pynestor-1.7.6/tests/tests_spec.py
```

### Comparing `pynestor-1.7.5/pyproject.toml` & `pynestor-1.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.5/setup.cfg` & `pynestor-1.7.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pynestor
-version = 1.7.5
+version = 1.7.6
 description = Nestor wrapper in python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.ndp-systemes.fr/python-libs/py-nestor
 author = Alexis Pasquier
 author_email = contact@ndp-systemes.fr
 classifiers =
```

### Comparing `pynestor-1.7.5/src/pynestor/__main__.py` & `pynestor-1.7.6/src/pynestor/__main__.py`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.5/src/pynestor/default-preview-nestor-cfg.yml` & `pynestor-1.7.6/src/pynestor/default-preview-nestor-cfg.yml`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.5/src/pynestor/preview_odoo_nestor.py` & `pynestor-1.7.6/src/pynestor/preview_odoo_nestor.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,31 @@
 
 
 class EnvironementConfig:
     def __init__(self, base_env_vars=None):
         base_env_vars = dict(base_env_vars or {}, **os.environ)
         self.NESTOR_NAME = base_env_vars.get("NESTOR_NAME") or base_env_vars.get("CI_COMMIT_REF_SLUG")
         self.NESTOR_NAME_PREFIX = base_env_vars.get("NESTOR_NAME_PREFIX")
-        self.ALWAYS_DELETE = base_env_vars.get("ALWAYS_DELETE")
+        self.ALWAYS_DELETE: bool = base_env_vars.get("ALWAYS_DELETE", str(False)).capitalize() == str(True).capitalize()
+        self.ALWAYS_RESTORE: bool = (
+            base_env_vars.get("ALWAYS_RESTORE", str(False)).capitalize() == str(True).capitalize()
+        )
         self.CI_COMMIT_REF_NAME = base_env_vars.get("CI_COMMIT_REF_NAME")
         self.CI_PROJECT_DIR = base_env_vars.get("CI_PROJECT_DIR")
         self.CI_BUILDS_DIR = base_env_vars.get("CI_BUILDS_DIR")
         self.CI_PROJECT_PATH = base_env_vars.get("CI_PROJECT_PATH")
         self.GITLAB_TOKEN = base_env_vars.get("GITLAB_TOKEN")
         self.ODOO_VERSION = base_env_vars.get("ODOO_VERSION")
         self.S3_SECRET_PREVIEW = base_env_vars.get("S3_SECRET_PREVIEW")
         self.S3_DUMP_SECRET = base_env_vars.get("S3_DUMP_SECRET")
         self.S3_DUMP_BUCKET = base_env_vars.get("S3_DUMP_BUCKET")
         self.VERBOSE = bool(base_env_vars.get("VERBOSE"))
         self.DATE = base_env_vars.get("DATE")
         self.S3_BUCKET = base_env_vars.get("S3_BUCKET")
+        self.ENABLE_QUEUE_JOB = base_env_vars.get("ENABLE_QUEUE_JOB")
         self.PROD_INSTANCE_NAME = base_env_vars.get("PROD_INSTANCE_NAME") or base_env_vars.get("CI_PROJECT_NAME")
         self.DB_NAME = base_env_vars.get("DB_NAME")
         self.ODOO_DEPENDS = base_env_vars.get("ODOO_DEPENDS")
         self.DUMP_PATH = base_env_vars.get("PATH_DUMP")
         self.NO_DB_DUMP: bool = base_env_vars.get("NO_DB_DUMP", str(False)).capitalize() == str(True).capitalize()
         self.MODULES_WITHOUT_DEMO: str = base_env_vars.get("MODULES_WITHOUT_DEMO", str(False).capitalize())
         self.NESTOR_CFG_FILENAME = os.environ.get("NESTOR_CFG_FILENAME", ".nestor-cfg.yml")
@@ -285,29 +289,35 @@
         self.inst.wait(up=False, postgres=True, timeout=5 * 60)
         self.inst.wait(up=False, timeout=5 * 60)
 
     def stop(self):
         self.inst.delete_and_exit_if_failed(self.inst.stop())
         self.inst.delete_and_exit_if_failed(self.inst.wait(up=False, postgres=False, timeout=5 * 60))  # Timeout de 5min
 
-    def enable_s3_spec(self, values):
+    def enable_s3_spec(self, values) -> NestorDescSet:
         if self.inst.version(values) not in SUPPORTED_S3:
             log("Version", self.inst.version(values), "don't support S3 in preview: allowed are", SUPPORTED_S3)
             return values
         if values["persistence.s3.secret"]:
             values.add(
                 self.inst.filestore.enable_on_s3_spec(
                     s3_secret="s3-ndp-preview", s3_bucket=self.config.S3_BUCKET, values=values
                 )
             )
         client = self._get_s3_client()
         if not client.bucket_exists(self.config.S3_BUCKET):
             client.make_bucket(self.config.S3_BUCKET)
         return values
 
+    def enable_queue_job(self, values: NestorDescSet = None) -> NestorDescSet:
+        channels = values["options.queueJobs.channels"] or NestorOpt("options.queueJobs.channels", "root:1")
+        values.add(channels)
+        values.add(NestorOpt("options.queueJobs.enabled", True))
+        return values
+
     def log_spec(self, spec_values: NestorDescSet):
         log("")
         log("Spec Nestor", self.inst.name)
         log(spec_values.to_str(pretty=True))
         log("")
 
     def run_script(self) -> int:
@@ -349,14 +359,16 @@
 
     def get_spec_values(self, *, stage: str) -> NestorDescSet:
         values = self.preview_utils.get_spec_values(
             sections=["default", "preview", self.config.CI_COMMIT_REF_NAME], stage=stage
         )
         values.add(self.preview_utils._create_all_spec_sources(self.config.CI_PROJECT_PATH))
         values = self.enable_s3_spec(values)
+        if self.config.ENABLE_QUEUE_JOB:
+            values = self.enable_queue_job(values)
         if self.config.NO_DB_DUMP:
             values = self.add_with_demo_option(values)
         if self._is_container(values.get("spec.dockerImage", "")):
             # container image supports only https git fetching
             values = self._change_git_method_to_https(values)
         return values
 
@@ -390,20 +402,24 @@
     def run_script(self):
         if not self.inst.name:
             log("Instance don't have a name")
             return 1
         if self.config.ALWAYS_DELETE:
             if self.inst.exist():
                 self.delete()
-
-        if not self.inst.exist():
+                # it seems that the instance is not really deleted event if nestor says it is, so we wait a little
+                time.sleep(30)
+        instance_doesnt_exist = not self.inst.exist()
+        if instance_doesnt_exist:
             log("Create instance")
             values = self.get_spec_values(stage="restore")
             self.log_spec(values)
             self.create_with_values(values)
+
+        if self.config.ALWAYS_RESTORE or instance_doesnt_exist:
             if not self.config.NO_DB_DUMP:
                 self.restore_db()
             if self.config.MODULE_TO_INSTALL:
                 log("Install -i", self.config.MODULE_TO_INSTALL)
                 self.inst.install(self.config.MODULE_TO_INSTALL)
 
         log("MAJ de l'instance", self.inst.name)
```

### Comparing `pynestor-1.7.5/src/pynestor/pynestor.py` & `pynestor-1.7.6/src/pynestor/pynestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 import os
 import re
 import subprocess
 import sys
 from functools import cached_property
-from typing import List, Optional, Union
+from typing import List, Optional, Set, Union
 
 from yaml import load
 
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
@@ -42,17 +42,90 @@
             if isinstance(value, dict):
                 result += Utils.flat_dico(parent_keys=new_key, dico=value)
             else:
                 result.append((new_key, value))
         return result
 
 
+class NestorDesc:
+    def to_set_opt(self) -> "NestorDescSet":
+        """Return a list of valid parameters for the --set arg for the 'nestor new' command"""
+        raise NotImplementedError()
+
+    def _key_hash(self):
+        raise NotImplementedError()
+
+    def __hash__(self):
+        return hash(self._key_hash())
+
+    def __eq__(self, other):
+        if isinstance(other, NestorDesc):
+            return self._key_hash() == other._key_hash()
+        return False
+
+    def __str__(self):
+        return str(self.to_set_opt())
+
+    def __ge__(self, other):
+        if isinstance(other, NestorDesc):
+            return self._key_hash().__ge__(other._key_hash())
+        raise TypeError
+
+    def __le__(self, other):
+        if isinstance(other, NestorDesc):
+            return self._key_hash().__le__(other._key_hash())
+        raise TypeError
+
+    def __lt__(self, other):
+        if isinstance(other, NestorDesc):
+            return self._key_hash().__lt__(other._key_hash())
+        raise TypeError
+
+    def __gt__(self, other):
+        if isinstance(other, NestorDesc):
+            return self._key_hash().__gt__(other._key_hash())
+        raise TypeError
+
+
+class NestorOpt(NestorDesc):
+    _prefix = "spec."
+
+    def __init__(self, name, value):
+        self.name = name
+        self.value = value
+
+    def to_set_opt(self):
+        """Return a list of valid parameters for the --set arg for the 'nestor new' command"""
+        return NestorDescSet([self])
+
+    def _key_hash(self):
+        name = self.name
+        if not name.startswith(NestorOpt._prefix):
+            name = NestorOpt._prefix + name
+        return name
+
+    def __str__(self):
+        name = self.name
+        if not name.startswith(NestorOpt._prefix):
+            name = NestorOpt._prefix + name
+        return "%s=%s" % (name, Utils.quote_if_needed(self.value))
+
+    def __repr__(self):
+        return '%s("%s", %s)' % (
+            type(self).__name__,
+            self.name,
+            Utils.quote_if_needed(self.value),
+        )
+
+
 class NestorDescSet:
+    """Représente un ensemble de NestorOpt (qui sont des paires clef / valeur)"""
+
     def __init__(self, init: List["NestorDesc"] = None):
-        self.values = set()
+        self.values: Set[NestorOpt] = set()
         self.add(init or [])
 
     def add(self, other: Union[List["NestorDescSet"], "NestorDescSet", "NestorDesc", List["NestorDesc"]]) -> None:
         if not isinstance(other, list):
             other = [other]
         for vo in other:
             if isinstance(vo, NestorOpt):
@@ -73,15 +146,15 @@
             other = [other]
         for vo in other:
             if not isinstance(vo, NestorDescSet):
                 raise ValueError("Can't add type %s" % type(vo))
             self.values |= vo.values
         return self
 
-    def __getitem__(self, item: Union[str, "NestorDesc"]) -> Optional["NestorDesc"]:
+    def __getitem__(self, item: Union[str, "NestorDesc"]) -> Optional[NestorOpt]:
         to_find = item
         if isinstance(to_find, str):
             # __hash__ only on the key not on the value, TODO replace with custom lib internal class
             to_find = NestorOpt(item, 0)
 
         for el in self.values:
             if el == to_find:
@@ -132,85 +205,14 @@
                     lambda it: str(it),
                     self.values,
                 )
             )
         )
 
 
-class NestorDesc:
-    def to_set_opt(self) -> NestorDescSet:
-        """Return a list of valid parameters for the --set arg for the 'nestor new' command"""
-        raise NotImplementedError()
-
-    def _key_hash(self):
-        raise NotImplementedError()
-
-    def __hash__(self):
-        return hash(self._key_hash())
-
-    def __eq__(self, other):
-        if isinstance(other, NestorDesc):
-            return self._key_hash() == other._key_hash()
-        return False
-
-    def __str__(self):
-        return str(self.to_set_opt())
-
-    def __ge__(self, other):
-        if isinstance(other, NestorDesc):
-            return self._key_hash().__ge__(other._key_hash())
-        raise TypeError
-
-    def __le__(self, other):
-        if isinstance(other, NestorDesc):
-            return self._key_hash().__le__(other._key_hash())
-        raise TypeError
-
-    def __lt__(self, other):
-        if isinstance(other, NestorDesc):
-            return self._key_hash().__lt__(other._key_hash())
-        raise TypeError
-
-    def __gt__(self, other):
-        if isinstance(other, NestorDesc):
-            return self._key_hash().__gt__(other._key_hash())
-        raise TypeError
-
-
-class NestorOpt(NestorDesc):
-    _prefix = "spec."
-
-    def __init__(self, name, value):
-        self.name = name
-        self.value = value
-
-    def to_set_opt(self):
-        """Return a list of valid parameters for the --set arg for the 'nestor new' command"""
-        return NestorDescSet([self])
-
-    def _key_hash(self):
-        name = self.name
-        if not name.startswith(NestorOpt._prefix):
-            name = NestorOpt._prefix + name
-        return name
-
-    def __str__(self):
-        name = self.name
-        if not name.startswith(NestorOpt._prefix):
-            name = NestorOpt._prefix + name
-        return "%s=%s" % (name, Utils.quote_if_needed(self.value))
-
-    def __repr__(self):
-        return '%s("%s", %s)' % (
-            type(self).__name__,
-            self.name,
-            Utils.quote_if_needed(self.value),
-        )
-
-
 class NestorGitDesc(NestorDesc):
     """Python class to handle the yml part of the Odoo operator
     branch: ""
           method: ssh
           path: odoo-addons/community-addons
           secret: ""
           server: ""
```

