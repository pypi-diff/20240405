# Comparing `tmp/sequana_pipetools-1.0.0.tar.gz` & `tmp/sequana_pipetools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequana_pipetools-1.0.0.tar", max compression
+gzip compressed data, was "sequana_pipetools-1.0.1.tar", max compression
```

## Comparing `sequana_pipetools-1.0.0.tar` & `sequana_pipetools-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    19353 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/README.rst
--rw-r--r--   0        0        0     1824 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      754 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/__init__.py
--rw-r--r--   0        0        0     1587 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/info.py
--rw-r--r--   0        0        0     3187 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/misc.py
--rw-r--r--   0        0        0    21178 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/options.py
--rw-r--r--   0        0        0        0 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/resources/__init__.py
--rw-r--r--   0        0        0      826 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/resources/ext.py
--rw-r--r--   0        0        0      202 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/resources/local.yaml
--rw-r--r--   0        0        0      653 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/resources/slurm.yaml
--rw-r--r--   0        0        0        0 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/scripts/__init__.py
--rw-r--r--   0        0        0     9149 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/scripts/main.py
--rw-r--r--   0        0        0    26238 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/sequana_manager.py
--rw-r--r--   0        0        0      383 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/__init__.py
--rw-r--r--   0        0        0     4682 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/dot_parser.py
--rw-r--r--   0        0        0     1367 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/errors.py
--rw-r--r--   0        0        0    15694 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/file_factory.py
--rw-r--r--   0        0        0    10369 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/module.py
--rw-r--r--   0        0        0     2095 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/module_finder.py
--rw-r--r--   0        0        0    19095 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/pipeline_manager.py
--rw-r--r--   0        0        0     6038 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/pipeline_utils.py
--rw-r--r--   0        0        0     1047 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/profile.py
--rw-r--r--   0        0        0     8424 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/sequana_config.py
--rw-r--r--   0        0        0     5479 2024-03-29 19:55:50.821500 sequana_pipetools-1.0.0/sequana_pipetools/snaketools/slurm.py
--rw-r--r--   0        0        0    21069 1970-01-01 00:00:00.000000 sequana_pipetools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    19437 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/README.rst
+-rw-r--r--   0        0        0     1824 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      754 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/info.py
+-rw-r--r--   0        0        0     3187 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/misc.py
+-rw-r--r--   0        0        0    21178 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/options.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/resources/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/resources/ext.py
+-rw-r--r--   0        0        0      202 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/resources/local.yaml
+-rw-r--r--   0        0        0      653 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/resources/slurm.yaml
+-rw-r--r--   0        0        0        0 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/scripts/__init__.py
+-rw-r--r--   0        0        0     9149 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/scripts/main.py
+-rw-r--r--   0        0        0    26238 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/sequana_manager.py
+-rw-r--r--   0        0        0      383 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/__init__.py
+-rw-r--r--   0        0        0     4682 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/dot_parser.py
+-rw-r--r--   0        0        0     1367 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/errors.py
+-rw-r--r--   0        0        0    15694 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/file_factory.py
+-rw-r--r--   0        0        0    10369 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/module.py
+-rw-r--r--   0        0        0     2095 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/module_finder.py
+-rw-r--r--   0        0        0    19095 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/pipeline_manager.py
+-rw-r--r--   0        0        0     6038 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/pipeline_utils.py
+-rw-r--r--   0        0        0     1065 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/profile.py
+-rw-r--r--   0        0        0     8424 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/sequana_config.py
+-rw-r--r--   0        0        0     5479 2024-04-05 19:34:11.203454 sequana_pipetools-1.0.1/sequana_pipetools/snaketools/slurm.py
+-rw-r--r--   0        0        0    21153 1970-01-01 00:00:00.000000 sequana_pipetools-1.0.1/PKG-INFO
```

### Comparing `sequana_pipetools-1.0.0/README.rst` & `sequana_pipetools-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,16 @@
 
 Changelog
 =========
 
 ========= ======================================================================
 Version   Description
 ========= ======================================================================
+1.0.1     * hot fix in the profile creation (regression)
+1.0.0     * Stable release
 0.17.3    * remove useless code and fix a requirement
 0.17.2    * simpler logging
 0.17.1    * remove the --use-singulariry (replaced by --use-apptainer in
             previous release)
           * slight updates on logging and slight update on slurm module
 0.17.0    * Remove deprecated options and deprecated functions. More tests.
 0.16.9    * Fix slurm sys exit (replaced by print)
```

### Comparing `sequana_pipetools-1.0.0/pyproject.toml` & `sequana_pipetools-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 #maintainer ?#maintainer email
 [tool.poetry]
 name = "sequana_pipetools"
-version = "1.0.0"
+version = "1.0.1"
 description = "A set of tools to help building or using Sequana pipelines"
 authors = ["Sequana Team"]
 license = "BSD-3"
 repository = "https://github.com/sequana/sequana_pipetools"
 readme = "README.rst"
 keywords = ["snakemake", "sequana", "pipelines"]
 classifiers = [
```

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/__init__.py` & `sequana_pipetools-1.0.1/sequana_pipetools/__init__.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/info.py` & `sequana_pipetools-1.0.1/sequana_pipetools/info.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/misc.py` & `sequana_pipetools-1.0.1/sequana_pipetools/misc.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/options.py` & `sequana_pipetools-1.0.1/sequana_pipetools/options.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/resources/ext.py` & `sequana_pipetools-1.0.1/sequana_pipetools/resources/ext.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/resources/slurm.yaml` & `sequana_pipetools-1.0.1/sequana_pipetools/resources/slurm.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/scripts/main.py` & `sequana_pipetools-1.0.1/sequana_pipetools/scripts/main.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/sequana_manager.py` & `sequana_pipetools-1.0.1/sequana_pipetools/sequana_manager.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/dot_parser.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/dot_parser.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/errors.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/errors.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/file_factory.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/file_factory.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/module.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/module.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/module_finder.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/module_finder.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/pipeline_manager.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/pipeline_utils.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/profile.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 from pathlib import Path
 
 
 def create_profile(workdir: Path, profile: str, **kwargs) -> str:
     """Create profile config in working directory."""
     try:
-        slurm_file = resources.files("sequana_pipetools.resources").joinpath(f"{profile}.yaml")
-        with open(slurm_file, "r") as fin:
-            slurm_text = fin.read()
-            slurl_text = slurm_text.format(**kwargs)
+        profile_file = resources.files("sequana_pipetools.resources").joinpath(f"{profile}.yaml")
+        with open(profile_file, "r") as fin:
+            profile_text = fin.read()
+            profile_text = profile_text.format(**kwargs)
     except AttributeError:
         # python 3.8 support for back compatibility
-        with resources.path("sequana_pipetools.resources", f"{profile}.yaml") as slurm_file:
-            slurm_text = slurm_file.read_text().format(**kwargs)
+        with resources.path("sequana_pipetools.resources", f"{profile}.yaml") as profile_file:
+            profile_text = profile_file.read_text().format(**kwargs)
 
     outfile = workdir / f".sequana/profile_{profile}" / "config.yaml"
     outfile.parent.mkdir(parents=True, exist_ok=True)
-    outfile.write_text(slurm_text)
+    outfile.write_text(profile_text)
     return f".sequana/profile_{profile}"
```

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/sequana_config.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/sequana_config.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/sequana_pipetools/snaketools/slurm.py` & `sequana_pipetools-1.0.1/sequana_pipetools/snaketools/slurm.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-1.0.0/PKG-INFO` & `sequana_pipetools-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequana_pipetools
-Version: 1.0.0
+Version: 1.0.1
 Summary: A set of tools to help building or using Sequana pipelines
 Home-page: https://github.com/sequana/sequana_pipetools
 License: BSD-3
 Keywords: snakemake,sequana,pipelines
 Author: Sequana Team
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -350,14 +350,16 @@
 
 Changelog
 =========
 
 ========= ======================================================================
 Version   Description
 ========= ======================================================================
+1.0.1     * hot fix in the profile creation (regression)
+1.0.0     * Stable release
 0.17.3    * remove useless code and fix a requirement
 0.17.2    * simpler logging
 0.17.1    * remove the --use-singulariry (replaced by --use-apptainer in
             previous release)
           * slight updates on logging and slight update on slurm module
 0.17.0    * Remove deprecated options and deprecated functions. More tests.
 0.16.9    * Fix slurm sys exit (replaced by print)
```

