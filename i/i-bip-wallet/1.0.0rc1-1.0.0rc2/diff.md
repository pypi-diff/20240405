# Comparing `tmp/i_bip_wallet-1.0.0rc1.tar.gz` & `tmp/i_bip_wallet-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_bip_wallet-1.0.0rc1.tar", max compression
+gzip compressed data, was "i_bip_wallet-1.0.0rc2.tar", max compression
```

## Comparing `i_bip_wallet-1.0.0rc1.tar` & `i_bip_wallet-1.0.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      765 2024-04-05 16:47:33.525449 i_bip_wallet-1.0.0rc1/i_bip_wallet/__init__.py
--rw-r--r--   0        0        0     1091 2024-03-29 22:45:12.865642 i_bip_wallet-1.0.0rc1/i_bip_wallet/_PrivateKey.py
--rw-r--r--   0        0        0     1865 2024-03-29 22:34:01.562392 i_bip_wallet-1.0.0rc1/i_bip_wallet/_PublicKey.py
--rw-r--r--   0        0        0     2150 2024-03-29 22:44:37.417557 i_bip_wallet-1.0.0rc1/i_bip_wallet/_Ripemd.py
--rw-r--r--   0        0        0     1353 2024-03-29 22:43:47.949333 i_bip_wallet-1.0.0rc1/i_bip_wallet/_Utils.py
--rw-r--r--   0        0        0      385 2024-04-05 16:48:42.920971 i_bip_wallet-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 22:02:44.981718 i_bip_wallet-1.0.0rc1/README.md
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc1/setup.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-05 16:51:58.904563 i_bip_wallet-1.0.0rc2/i_bip_wallet/__init__.py
+-rw-r--r--   0        0        0     1091 2024-03-29 22:45:12.865642 i_bip_wallet-1.0.0rc2/i_bip_wallet/_PrivateKey.py
+-rw-r--r--   0        0        0     1865 2024-03-29 22:34:01.562392 i_bip_wallet-1.0.0rc2/i_bip_wallet/_PublicKey.py
+-rw-r--r--   0        0        0     2150 2024-03-29 22:44:37.417557 i_bip_wallet-1.0.0rc2/i_bip_wallet/_Ripemd.py
+-rw-r--r--   0        0        0     1353 2024-03-29 22:43:47.949333 i_bip_wallet-1.0.0rc2/i_bip_wallet/_Utils.py
+-rw-r--r--   0        0        0      385 2024-04-05 16:52:09.554916 i_bip_wallet-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-29 22:02:44.981718 i_bip_wallet-1.0.0rc2/README.md
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc2/setup.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc2/PKG-INFO
```

### Comparing `i_bip_wallet-1.0.0rc1/i_bip_wallet/_PrivateKey.py` & `i_bip_wallet-1.0.0rc2/i_bip_wallet/_PrivateKey.py`

 * *Files identical despite different names*

### Comparing `i_bip_wallet-1.0.0rc1/i_bip_wallet/_PublicKey.py` & `i_bip_wallet-1.0.0rc2/i_bip_wallet/_PublicKey.py`

 * *Files identical despite different names*

### Comparing `i_bip_wallet-1.0.0rc1/i_bip_wallet/_Ripemd.py` & `i_bip_wallet-1.0.0rc2/i_bip_wallet/_Ripemd.py`

 * *Files identical despite different names*

### Comparing `i_bip_wallet-1.0.0rc1/i_bip_wallet/_Utils.py` & `i_bip_wallet-1.0.0rc2/i_bip_wallet/_Utils.py`

 * *Files identical despite different names*

### Comparing `i_bip_wallet-1.0.0rc1/setup.py` & `i_bip_wallet-1.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ecdsa>=0.18.0,<0.19.0', 'pycryptodomex>=3.20.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'i-bip-wallet',
-    'version': '1.0.0rc1',
+    'version': '1.0.0rc2',
     'description': '',
     'long_description': '',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `i_bip_wallet-1.0.0rc1/PKG-INFO` & `i_bip_wallet-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-bip-wallet
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

