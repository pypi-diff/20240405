# Comparing `tmp/autoupdater-0.8.0.tar.gz` & `tmp/autoupdater-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoupdater-0.8.0.tar", max compression
+gzip compressed data, was "autoupdater-0.9.0.tar", max compression
```

## Comparing `autoupdater-0.8.0.tar` & `autoupdater-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2024-03-05 22:16:20.720933 autoupdater-0.8.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:16:20.730584 autoupdater-0.8.0/README.md
--rw-r--r--   0        0        0        0 2024-03-05 22:16:20.730803 autoupdater-0.8.0/autoupdater/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-05 22:16:20.764131 autoupdater-0.8.0/autoupdater/__main__.py
--rw-r--r--   0        0        0     8793 2024-03-09 20:31:51.637106 autoupdater-0.8.0/autoupdater/core.py
--rw-r--r--   0        0        0      379 2024-03-09 20:31:54.674560 autoupdater-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 autoupdater-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-05 22:16:20.720933 autoupdater-0.9.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:16:20.730584 autoupdater-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-05 22:16:20.730803 autoupdater-0.9.0/autoupdater/__init__.py
+-rw-r--r--   0        0        0     1021 2024-03-05 22:16:20.764131 autoupdater-0.9.0/autoupdater/__main__.py
+-rw-r--r--   0        0        0     8807 2024-03-09 21:02:22.565337 autoupdater-0.9.0/autoupdater/core.py
+-rw-r--r--   0        0        0      379 2024-03-09 21:02:32.890595 autoupdater-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 autoupdater-0.9.0/PKG-INFO
```

### Comparing `autoupdater-0.8.0/LICENSE` & `autoupdater-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoupdater-0.8.0/autoupdater/__main__.py` & `autoupdater-0.9.0/autoupdater/__main__.py`

 * *Files identical despite different names*

### Comparing `autoupdater-0.8.0/autoupdater/core.py` & `autoupdater-0.9.0/autoupdater/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 def launch(
     venv: Venv,
     module: str,
     args: list[str],
 ) -> Iterator[Program]:
     command = [
         venv.spec.python_path().absolute(),
+        "-u",
         "-m",
         module,
     ] + args
     log.info("Starting process '%s'", " ".join(str(arg) for arg in command))
     process = subprocess.Popen(command)
     program = Program(
         process=process,
```

