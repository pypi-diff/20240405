# Comparing `tmp/backend.ai-kernel-24.3.0rc3.tar.gz` & `tmp/backend.ai-kernel-24.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:37 2024, max compression
+gzip compressed data, was "backend.ai-kernel-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:01 2024, max compression
```

## Comparing `backend.ai-kernel-24.3.0rc3.tar` & `backend.ai-kernel-24.3.0rc4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.130041 backend.ai-kernel-24.3.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.114040 backend.ai-kernel-24.3.0rc3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.114040 backend.ai-kernel-24.3.0rc3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/app/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/c/
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/git/
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/golang/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/golang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/haskell/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/haskell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/java/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/julia/
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/lua/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/lua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/nodejs/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/nodejs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/octave/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/octave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/php/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/php/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.122041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r_server_ms/
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r_server_ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/rust/
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/scheme/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/service_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/aws_polly/
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/aws_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/aws_polly/inproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/h2o/
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/h2o/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.126041 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:37.000000 backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:37.130041 backend.ai-kernel-24.3.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-05 02:25:36.000000 backend.ai-kernel-24.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.953385 backend.ai-kernel-24.3.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-05 03:40:01.953385 backend.ai-kernel-24.3.0rc4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.941385 backend.ai-kernel-24.3.0rc4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.941385 backend.ai-kernel-24.3.0rc4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/git/
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/golang/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/golang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/haskell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/haskell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/java/
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/julia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/lua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.945385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/nodejs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/nodejs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/octave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/octave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/php/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/php/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r_server_ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r_server_ms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/scheme/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/service_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/aws_polly/
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/aws_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/aws_polly/inproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.949385 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/h2o/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/h2o/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.953385 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:01.000000 backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:01.953385 backend.ai-kernel-24.3.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-05 03:40:00.000000 backend.ai-kernel-24.3.0rc4/setup.py
```

### Comparing `backend.ai-kernel-24.3.0rc3/PKG-INFO` & `backend.ai-kernel-24.3.0rc4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/__main__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/app/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/app/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/base.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/c/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/c/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/compat.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/cpp/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/git/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/git/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/golang/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/haskell/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/haskell/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/intrinsic.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/intrinsic.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/java/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/java/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/julia/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/jupyter_client.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/logging.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/lua/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/lua/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/nodejs/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/nodejs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/octave/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/php/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/php/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/canvas.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/canvas.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/color.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/color.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/drawing/turtle.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/drawing/turtle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/sitecustomize.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/python/types.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/python/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/r_server_ms/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/r_server_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/rust/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/scheme/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/service.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/service_actions.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/service_actions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/terminal.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/terminal.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/utils.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/aws_polly/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/aws_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/aws_polly/inproc.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/aws_polly/inproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/ai/backend/kernel/vendor/h2o/__init__.py` & `backend.ai-kernel-24.3.0rc4/ai/backend/kernel/vendor/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/PKG-INFO` & `backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 24.3.0rc3
+Version: 24.3.0rc4
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-24.3.0rc3/backend.ai_kernel.egg-info/SOURCES.txt` & `backend.ai-kernel-24.3.0rc4/backend.ai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/backend_shim.py` & `backend.ai-kernel-24.3.0rc4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-24.3.0rc3/setup.py` & `backend.ai-kernel-24.3.0rc4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,11 +71,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc3
+    'version': """24.03.0rc4
 """,
     'zip_safe': False,
 })
```

