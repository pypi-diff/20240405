# Comparing `tmp/kite_connect_lite-0.0.1.tar.gz` & `tmp/kite_connect_lite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kite_connect_lite-0.0.1.tar", max compression
+gzip compressed data, was "kite_connect_lite-0.0.2.tar", max compression
```

## Comparing `kite_connect_lite-0.0.1.tar` & `kite_connect_lite-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0       28 2024-03-30 12:27:24.288528 kite_connect_lite-0.0.1/README.md
--rw-r--r--   0        0        0       41 2024-03-30 18:18:08.943572 kite_connect_lite-0.0.1/kite_connect_lite/__init__.py
--rw-r--r--   0        0        0      586 2024-03-30 18:17:22.170041 kite_connect_lite-0.0.1/kite_connect_lite/greetings.py
--rw-r--r--   0        0        0      577 2024-03-30 18:40:53.765347 kite_connect_lite-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 kite_connect_lite-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2055 2024-04-04 15:35:07.458395 kite_connect_lite-0.0.2/README.md
+-rw-r--r--   0        0        0       41 2024-04-05 17:11:25.467207 kite_connect_lite-0.0.2/kite_connect_lite/__init__.py
+-rw-r--r--   0        0        0      739 2024-04-05 17:11:28.284178 kite_connect_lite-0.0.2/kite_connect_lite/main.py
+-rw-r--r--   0        0        0     1011 2024-04-05 16:53:16.515023 kite_connect_lite-0.0.2/kite_connect_lite/models/generate_session_model.py
+-rw-r--r--   0        0        0      518 2024-04-05 16:53:21.278048 kite_connect_lite-0.0.2/kite_connect_lite/models/login_url_model.py
+-rw-r--r--   0        0        0     1368 2024-04-05 17:03:25.841691 kite_connect_lite-0.0.2/kite_connect_lite/models/place_normal_order_model.py
+-rw-r--r--   0        0        0      608 2024-04-05 17:12:08.841881 kite_connect_lite-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 kite_connect_lite-0.0.2/PKG-INFO
```

### Comparing `kite_connect_lite-0.0.1/pyproject.toml` & `kite_connect_lite-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "kite_connect_lite"
-version = "0.0.1"
+version = "0.0.2"
 description = "A user-friendly wrapper for the Kite Connect library"
 authors = ["AST-LW <walkthroughfrom2020@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
 pydantic = "^2.6.4"
 pandas = "^2.2.1"
+python-dotenv = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 
-[[tool.poetry.source]]
-name = "pypi-test"
-url = "https://test.pypi.org/legacy/"
-priority = "secondary"
+# [[tool.poetry.source]]
+# name = "pypi-test"
+# url = "https://test.pypi.org/legacy/"
+# priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

