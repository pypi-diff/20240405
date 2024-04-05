# Comparing `tmp/aprl-0.0.0.tar.gz` & `tmp/aprl-2024.4.5.1813.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprl-0.0.0.tar", last modified: Tue Apr  2 11:28:56 2024, max compression
+gzip compressed data, was "aprl-2024.4.5.1813.tar", last modified: Fri Apr  5 16:13:49 2024, max compression
```

## Comparing `aprl-0.0.0.tar` & `aprl-2024.4.5.1813.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.952473 aprl-0.0.0/
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)    11357 2024-03-29 18:38:23.000000 aprl-0.0.0/LICENSE
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      185 2024-04-02 11:28:56.952473 aprl-0.0.0/PKG-INFO
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      167 2024-03-29 17:26:48.000000 aprl-0.0.0/README.md
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.948473 aprl-0.0.0/aprl/
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.948473 aprl-0.0.0/aprl/experimental/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-0.0.0/aprl/experimental/__init__.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2601 2024-03-29 18:05:18.000000 aprl-0.0.0/aprl/experimental/depinject.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-0.0.0/aprl/experimental/dvcspec.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.948473 aprl-0.0.0/aprl/module/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     1784 2024-03-31 11:43:42.000000 aprl-0.0.0/aprl/module/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.952473 aprl-0.0.0/aprl/pipeline/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     3174 2024-03-29 18:50:43.000000 aprl-0.0.0/aprl/pipeline/__init__.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.952473 aprl-0.0.0/aprl/utils/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2132 2024-04-02 11:25:12.000000 aprl-0.0.0/aprl/utils/__init__.py
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      434 2024-03-31 16:04:02.000000 aprl-0.0.0/aprl/utils/run.py
-drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-02 11:28:56.952473 aprl-0.0.0/aprl.egg-info/
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      185 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/PKG-INFO
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      383 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/SOURCES.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/dependency_links.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       53 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/entry_points.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       16 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/requires.txt
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        5 2024-04-02 11:28:56.000000 aprl-0.0.0/aprl.egg-info/top_level.txt
--rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      299 2024-04-02 11:27:03.000000 aprl-0.0.0/pyproject.toml
--rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-02 11:28:56.952473 aprl-0.0.0/setup.cfg
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)    11357 2024-03-29 18:38:23.000000 aprl-2024.4.5.1813/LICENSE
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/PKG-INFO
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     1488 2024-04-05 14:20:33.000000 aprl-2024.4.5.1813/README.md
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)       81 2024-04-05 16:06:46.000000 aprl-2024.4.5.1813/aprl/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl/appareil/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     4226 2024-04-05 14:03:19.000000 aprl-2024.4.5.1813/aprl/appareil/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl/experimental/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.5.1813/aprl/experimental/__init__.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2601 2024-03-29 18:05:18.000000 aprl-2024.4.5.1813/aprl/experimental/depinject.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-03-29 17:02:21.000000 aprl-2024.4.5.1813/aprl/experimental/dvcspec.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 13:40:34.000000 aprl-2024.4.5.1813/aprl/experimental/multirun_example.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl/part/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2852 2024-04-05 14:04:42.000000 aprl-2024.4.5.1813/aprl/part/__init__.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl/utils/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)     2131 2024-04-05 14:05:27.000000 aprl-2024.4.5.1813/aprl/utils/__init__.py
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      436 2024-04-05 14:45:13.000000 aprl-2024.4.5.1813/aprl/utils/run.py
+drwxrwxr-x   0 q20febvr  (1000) q20febvr  (1000)        0 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/aprl.egg-info/
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      193 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/PKG-INFO
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)      436 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/SOURCES.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        1 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/dependency_links.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       53 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/entry_points.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       16 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/requires.txt
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)        5 2024-04-05 16:13:49.000000 aprl-2024.4.5.1813/aprl.egg-info/top_level.txt
+-rw-r--r--   0 q20febvr  (1000) q20febvr  (1000)      364 2024-04-05 16:08:17.000000 aprl-2024.4.5.1813/pyproject.toml
+-rw-rw-r--   0 q20febvr  (1000) q20febvr  (1000)       38 2024-04-05 16:13:49.805410 aprl-2024.4.5.1813/setup.cfg
```

### Comparing `aprl-0.0.0/LICENSE` & `aprl-2024.4.5.1813/LICENSE`

 * *Files identical despite different names*

### Comparing `aprl-0.0.0/aprl/experimental/depinject.py` & `aprl-2024.4.5.1813/aprl/experimental/depinject.py`

 * *Files identical despite different names*

### Comparing `aprl-0.0.0/aprl/utils/__init__.py` & `aprl-2024.4.5.1813/aprl/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from omegaconf import OmegaConf
 
 
 def call(fn: Callable):
     return fn()
 
 
-def appareil(fn: Callable, inject: dict[str, Callable], params: dict[str, Any]):
+def aprlify(fn: Callable, inject: dict[str, Callable], params: dict[str, Any]):
     log.debug(f"Params {params}")
     log.debug(f"Injecting {inject} to {fn}")
     fn_cfg = OmegaConf.create(hydra_zen.builds(fn))
     fn_dict = OmegaConf.to_container(fn_cfg)
 
     for k in sorted(inject.keys(), reverse=False):
         kl = k.split(".")
```

