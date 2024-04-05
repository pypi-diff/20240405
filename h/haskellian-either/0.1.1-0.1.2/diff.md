# Comparing `tmp/haskellian-either-0.1.1.tar.gz` & `tmp/haskellian-either-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.1.tar", last modified: Thu Apr  4 06:20:54 2024, max compression
+gzip compressed data, was "haskellian-either-0.1.2.tar", last modified: Thu Apr  4 16:14:25 2024, max compression
```

## Comparing `haskellian-either-0.1.1.tar` & `haskellian-either-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      492 2024-04-04 06:20:50.000000 haskellian-either-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-02 10:45:11.000000 haskellian-either-0.1.1/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1911 2024-04-02 17:04:36.000000 haskellian-either-0.1.1/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2257 2024-04-03 05:57:59.000000 haskellian-either-0.1.1/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      492 2024-04-04 16:14:20.000000 haskellian-either-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.583188 haskellian-either-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.583188 haskellian-either-0.1.2/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-04 11:11:34.000000 haskellian-either-0.1.2/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2190 2024-04-04 11:13:26.000000 haskellian-either-0.1.2/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2257 2024-04-03 05:57:59.000000 haskellian-either-0.1.2/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 16:14:25.593189 haskellian-either-0.1.2/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 16:14:25.000000 haskellian-either-0.1.2/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian-either-0.1.1/src/haskellian/either/funcs.py` & `haskellian-either-0.1.2/src/haskellian/either/funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,26 @@
   """List of lefts if any (thus with length in `[1, len(eithers)]`), otherwise list of all rights (with length `len(eithers)`)"""
   lefts: list[L] = []
   rights: list[R] = []
   for x in eithers:
     x.match(lefts.append, rights.append)
   return Right(rights) if lefts == [] else Left(lefts)
 
+def filter(eithers: Iterable[Either[L, R]]) -> Iterable[R]:
+  for e in eithers:
+    match e:
+      case Right(value):
+        yield value
+
+def filter_lefts(eithers: Iterable[Either[L, R]]) -> Iterable[L]:
+  for e in eithers:
+    match e:
+      case Left(err):
+        yield err
+
 def secure(*Exceptions: type[BaseException]):
   """Secure a function that throws some of `Exceptions` into one that returns `Either[Exceptions, R]` (doesn't catch other exceptions)"""
   def decorator(func: Callable[..., R]):
     @wraps(func)
     def _f(*args, **kwargs) -> Either[Union[*Exceptions], R]:
       try:
         return Right(func(*args, **kwargs))
```

### Comparing `haskellian-either-0.1.1/src/haskellian/either/type.py` & `haskellian-either-0.1.2/src/haskellian/either/type.py`

 * *Files identical despite different names*

