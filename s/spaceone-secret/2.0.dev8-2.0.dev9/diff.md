# Comparing `tmp/spaceone-secret-2.0.dev8.tar.gz` & `tmp/spaceone-secret-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-secret-2.0.dev8.tar", last modified: Mon Dec 18 12:36:17 2023, max compression
+gzip compressed data, was "spaceone-secret-2.0.dev9.tar", last modified: Mon Dec 18 13:51:43 2023, max compression
```

## Comparing `spaceone-secret-2.0.dev8.tar` & `spaceone-secret-2.0.dev9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/aws_secret_manager_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/consul_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/etcd_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/identity_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/mongodb_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/connector/vault_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/error/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/error/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/handler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/handler/encrypt_mutation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.569357 spaceone-secret-2.0.dev8/spaceone/secret/info/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/info/secret_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/info/trusted_secret_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone/secret/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/trusted_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone/secret/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/manager/secret_connector_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/manager/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/manager/trusted_secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone/secret/model/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/model/secret_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/model/trusted_secret_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone/secret/service/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/service/secret_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-12-18 12:35:56.000000 spaceone-secret-2.0.dev8/spaceone/secret/service/trusted_secret_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 12:36:17.573357 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-18 12:36:16.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-18 12:36:17.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 12:36:16.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 12:36:16.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-18 12:36:16.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-18 12:36:16.000000 spaceone-secret-2.0.dev8/spaceone_secret.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.977957 spaceone-secret-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-18 13:51:43.977957 spaceone-secret-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 13:51:43.977957 spaceone-secret-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.969957 spaceone-secret-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/aws_secret_manager_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/consul_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/etcd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/identity_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/mongodb_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/connector/vault_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/error/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/handler/encrypt_mutation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/info/secret_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/info/trusted_secret_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/trusted_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/manager/secret_connector_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/manager/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/manager/trusted_secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.973957 spaceone-secret-2.0.dev9/spaceone/secret/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/model/secret_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/model/trusted_secret_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.977957 spaceone-secret-2.0.dev9/spaceone/secret/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/service/secret_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-12-18 13:51:35.000000 spaceone-secret-2.0.dev9/spaceone/secret/service/trusted_secret_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 13:51:43.977957 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-18 13:51:43.000000 spaceone-secret-2.0.dev9/spaceone_secret.egg-info/top_level.txt
```

### Comparing `spaceone-secret-2.0.dev8/setup.py` & `spaceone-secret-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/conf/global_conf.py` & `spaceone-secret-2.0.dev9/spaceone/secret/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/aws_secret_manager_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/aws_secret_manager_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/consul_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/consul_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/etcd_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/etcd_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/identity_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/identity_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/mongodb_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/mongodb_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/connector/vault_connector.py` & `spaceone-secret-2.0.dev9/spaceone/secret/connector/vault_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/error/custom.py` & `spaceone-secret-2.0.dev9/spaceone/secret/error/custom.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/handler/encrypt_mutation_handler.py` & `spaceone-secret-2.0.dev9/spaceone/secret/handler/encrypt_mutation_handler.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/info/secret_info.py` & `spaceone-secret-2.0.dev9/spaceone/secret/info/secret_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/info/trusted_secret_info.py` & `spaceone-secret-2.0.dev9/spaceone/secret/info/trusted_secret_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/secret.py` & `spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/secret.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/interface/grpc/trusted_secret.py` & `spaceone-secret-2.0.dev9/spaceone/secret/interface/grpc/trusted_secret.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/manager/identity_manager.py` & `spaceone-secret-2.0.dev9/spaceone/secret/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/manager/secret_connector_manager.py` & `spaceone-secret-2.0.dev9/spaceone/secret/manager/secret_connector_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/manager/secret_manager.py` & `spaceone-secret-2.0.dev9/spaceone/secret/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/manager/trusted_secret_manager.py` & `spaceone-secret-2.0.dev9/spaceone/secret/manager/trusted_secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/model/secret_model.py` & `spaceone-secret-2.0.dev9/spaceone/secret/model/secret_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/model/trusted_secret_model.py` & `spaceone-secret-2.0.dev9/spaceone/secret/model/trusted_secret_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/service/secret_service.py` & `spaceone-secret-2.0.dev9/spaceone/secret/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone/secret/service/trusted_secret_service.py` & `spaceone-secret-2.0.dev9/spaceone/secret/service/trusted_secret_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-secret-2.0.dev8/spaceone_secret.egg-info/SOURCES.txt` & `spaceone-secret-2.0.dev9/spaceone_secret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

