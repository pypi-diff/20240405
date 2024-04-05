# Comparing `tmp/ai_model_worker-0.0.1.dev5.tar.gz` & `tmp/ai_model_worker-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_model_worker-0.0.1.dev5.tar", max compression
+gzip compressed data, was "ai_model_worker-0.0.1.dev6.tar", max compression
```

## Comparing `ai_model_worker-0.0.1.dev5.tar` & `ai_model_worker-0.0.1.dev6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-03-28 05:12:16.751329 ai_model_worker-0.0.1.dev5/ai_model_worker/__init__.py
--rw-r--r--   0        0        0       84 2024-03-29 08:00:31.969206 ai_model_worker-0.0.1.dev5/ai_model_worker/config.py
--rw-r--r--   0        0        0        0 2024-03-29 06:43:58.407552 ai_model_worker-0.0.1.dev5/ai_model_worker/worker/__init__.py
--rw-r--r--   0        0        0     1332 2024-04-02 13:29:50.964065 ai_model_worker-0.0.1.dev5/ai_model_worker/worker/BaseWorker.py
--rw-r--r--   0        0        0      384 2024-04-02 13:31:53.126001 ai_model_worker-0.0.1.dev5/pyproject.toml
--rw-r--r--   0        0        0       73 2024-03-29 03:32:18.742397 ai_model_worker-0.0.1.dev5/README.md
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 ai_model_worker-0.0.1.dev5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-28 05:12:16.751329 ai_model_worker-0.0.1.dev6/ai_model_worker/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-05 05:57:50.726987 ai_model_worker-0.0.1.dev6/ai_model_worker/config.py
+-rw-r--r--   0        0        0        0 2024-03-29 06:43:58.407552 ai_model_worker-0.0.1.dev6/ai_model_worker/worker/__init__.py
+-rw-r--r--   0        0        0     1332 2024-04-02 13:29:50.964065 ai_model_worker-0.0.1.dev6/ai_model_worker/worker/BaseWorker.py
+-rw-r--r--   0        0        0      384 2024-04-05 05:58:02.530804 ai_model_worker-0.0.1.dev6/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-03-29 03:32:18.742397 ai_model_worker-0.0.1.dev6/README.md
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 ai_model_worker-0.0.1.dev6/PKG-INFO
```

### Comparing `ai_model_worker-0.0.1.dev5/ai_model_worker/worker/BaseWorker.py` & `ai_model_worker-0.0.1.dev6/ai_model_worker/worker/BaseWorker.py`

 * *Files identical despite different names*

