# Comparing `tmp/ai_model_dispatcher-0.0.1.dev2.tar.gz` & `tmp/ai_model_dispatcher-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_model_dispatcher-0.0.1.dev2.tar", max compression
+gzip compressed data, was "ai_model_dispatcher-0.0.1.dev3.tar", max compression
```

## Comparing `ai_model_dispatcher-0.0.1.dev2.tar` & `ai_model_dispatcher-0.0.1.dev3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 10:05:33.667531 ai_model_dispatcher-0.0.1.dev2/ai_model_dispatcher/__init__.py
--rw-r--r--   0        0        0       84 2024-03-29 08:00:31.969206 ai_model_dispatcher-0.0.1.dev2/ai_model_dispatcher/config.py
--rw-r--r--   0        0        0        0 2024-04-02 10:08:46.841981 ai_model_dispatcher-0.0.1.dev2/ai_model_dispatcher/dispatcher/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-02 15:08:14.368750 ai_model_dispatcher-0.0.1.dev2/ai_model_dispatcher/dispatcher/BaseDispatcher.py
--rw-r--r--   0        0        0      388 2024-04-02 15:14:40.596780 ai_model_dispatcher-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 10:05:33.667531 ai_model_dispatcher-0.0.1.dev2/README.md
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 ai_model_dispatcher-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 10:05:33.667531 ai_model_dispatcher-0.0.1.dev3/ai_model_dispatcher/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-05 05:59:44.089506 ai_model_dispatcher-0.0.1.dev3/ai_model_dispatcher/config.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:08:46.841981 ai_model_dispatcher-0.0.1.dev3/ai_model_dispatcher/dispatcher/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-02 15:08:14.368750 ai_model_dispatcher-0.0.1.dev3/ai_model_dispatcher/dispatcher/BaseDispatcher.py
+-rw-r--r--   0        0        0      388 2024-04-05 05:59:44.084559 ai_model_dispatcher-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 10:05:33.667531 ai_model_dispatcher-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 ai_model_dispatcher-0.0.1.dev3/PKG-INFO
```

### Comparing `ai_model_dispatcher-0.0.1.dev2/ai_model_dispatcher/dispatcher/BaseDispatcher.py` & `ai_model_dispatcher-0.0.1.dev3/ai_model_dispatcher/dispatcher/BaseDispatcher.py`

 * *Files identical despite different names*

