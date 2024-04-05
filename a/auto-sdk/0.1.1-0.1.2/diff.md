# Comparing `tmp/auto-sdk-0.1.1.tar.gz` & `tmp/auto-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-sdk-0.1.1.tar", last modified: Wed Apr  3 23:32:07 2024, max compression
+gzip compressed data, was "auto-sdk-0.1.2.tar", last modified: Fri Apr  5 14:23:12 2024, max compression
```

## Comparing `auto-sdk-0.1.1.tar` & `auto-sdk-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-03 23:32:07.593658 auto-sdk-0.1.1/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-03 23:32:07.593658 auto-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.1/README.md
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-03 23:32:07.593658 auto-sdk-0.1.1/auto_identity/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      916 2024-04-03 23:29:42.000000 auto-sdk-0.1.1/auto_identity/__init__.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1460 2024-03-22 21:37:58.000000 auto-sdk-0.1.1/auto_identity/auto_entity.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     2544 2024-03-28 21:52:31.000000 auto-sdk-0.1.1/auto_identity/certificate_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     3936 2024-04-03 23:27:25.000000 auto-sdk-0.1.1/auto_identity/key_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-03 19:43:21.000000 auto-sdk-0.1.1/auto_identity/registry.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-01 16:36:43.000000 auto-sdk-0.1.1/auto_identity/utils.py
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-03 23:32:07.593658 auto-sdk-0.1.1/auto_sdk.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-03 23:32:07.000000 auto-sdk-0.1.1/auto_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      353 2024-04-03 23:32:07.000000 auto-sdk-0.1.1/auto_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-03 23:32:07.000000 auto-sdk-0.1.1/auto_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-03 23:32:07.000000 auto-sdk-0.1.1/auto_sdk.egg-info/requires.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-03 23:32:07.000000 auto-sdk-0.1.1/auto_sdk.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-03 23:32:07.593658 auto-sdk-0.1.1/setup.cfg
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-03 23:30:46.000000 auto-sdk-0.1.1/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.2/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/auto_identity/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1101 2024-04-05 14:22:16.000000 auto-sdk-0.1.2/auto_identity/__init__.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     2544 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/certificate_management.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4845 2024-04-05 14:15:46.000000 auto-sdk-0.1.2/auto_identity/key_management.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/registry.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/utils.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/auto_sdk.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      324 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/requires.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-05 14:22:23.000000 auto-sdk-0.1.2/setup.py
```

### Comparing `auto-sdk-0.1.1/auto_identity/__init__.py` & `auto-sdk-0.1.2/auto_identity/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,40 @@
 Auto Identity Module
 
 This module provides functionalities for managing digital identities within the Auto SDK, 
 including key generation, Auto ID management, and Auto ID registration and verification.
 """
 
 from substrateinterface import Keypair
-from .key_management import generate_rsa_key_pair, generate_ed25519_key_pair, key_to_hex, load_private_key, load_public_key
+from .key_management import (
+    generate_rsa_key_pair,
+    generate_ed25519_key_pair,
+    key_to_hex,
+    key_to_pem,
+    pem_to_private_key,
+    load_private_key,
+    pem_to_public_key,
+    load_public_key,
+    save_key)
 from .certificate_management import create_csr, issue_certificate, self_issue_certificate, get_subject_common_name
 from .registry import Registry
 from .utils import der_encode_signature_algorithm_oid
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 __all__ = [
     "generate_rsa_key_pair",
     "generate_ed25519_key_pair",
     "key_to_hex",
     "load_private_key",
     "load_public_key",
+    "save_key",
+    "pem_to_private_key",
+    "pem_to_public_key",
+    "key_to_pem",
     "create_csr",
     "issue_certificate",
     "self_issue_certificate",
     "get_subject_common_name",
     "der_encode_signature_algorithm_oid",
     "Registry",
     "Keypair",
```

### Comparing `auto-sdk-0.1.1/auto_identity/certificate_management.py` & `auto-sdk-0.1.2/auto_identity/certificate_management.py`

 * *Files identical despite different names*

### Comparing `auto-sdk-0.1.1/auto_identity/key_management.py` & `auto-sdk-0.1.2/auto_identity/key_management.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,74 +30,111 @@
         tuple: A tuple containing the Ed25519 private key and public key.
     """
     private_key = ed25519.Ed25519PrivateKey.generate()
     public_key = private_key.public_key()
     return private_key, public_key
 
 
-def save_key(key, file_path: str, password: str = None) -> None:
+def key_to_pem(key, password: str = None) -> str:
     """
-    Saves a private or public key to a file. If it's a private key and a password is provided,
-    the key will be encrypted.
+    Converts a private or public key to a PEM string.
 
     Args:
-        key: The key to save (private or public).
-        file_path (str): Path to the file where the key should be saved.
-        password (str): Optional password to encrypt the private key.
+        key: The key to convert (private or public).
+        password (str): The password used to encrypt the key.
     """
     if hasattr(key, 'private_bytes'):
         encoding = serialization.Encoding.PEM
         format = serialization.PrivateFormat.PKCS8
         encryption_algorithm = (serialization.BestAvailableEncryption(password.encode())
                                 if password else serialization.NoEncryption())
         key_data = key.private_bytes(encoding, format, encryption_algorithm)
     else:
         encoding = serialization.Encoding.PEM
         format = serialization.PublicFormat.SubjectPublicKeyInfo
         key_data = key.public_bytes(encoding, format)
 
+    return key_data
+
+
+def save_key(key, file_path: str, password: str = None) -> None:
+    """
+    Saves a private or public key to a file. If it's a private key and a password is provided,
+    the key will be encrypted.
+
+    Args:
+        key: The key to save (private or public).
+        file_path (str): Path to the file where the key should be saved.
+        password (str): Optional password to encrypt the private key.
+    """
+    key_data = key_to_pem(key, password)
+
     with open(file_path, "wb") as key_file:
         key_file.write(key_data)
 
 
+def pem_to_private_key(pem_data: str, password: str = None):
+    """
+    Converts a PEM string to a private or public key. If the PEM string is encrypted, a password must be provided.
+
+    Args:
+        pem_data (str): The PEM string to convert.
+        password (str): The password used to encrypt the key.
+    """
+
+    private_key = serialization.load_pem_private_key(
+        pem_data,
+        password=password.encode() if password else None,
+        backend=default_backend()
+    )
+    return private_key
+
+
 def load_private_key(file_path: str, password: str = None):
     """
     Loads a private key from a file. If the file is encrypted, a password must be provided.
 
     Args:
         file_path (str): Path to the private key file.
         password (str): The password used to encrypt the key file.
 
     Returns:
         The private key.
     """
     with open(file_path, "rb") as key_file:
-        private_key = serialization.load_pem_private_key(
-            key_file.read(),
-            password=password.encode() if password else None,
-            backend=default_backend()
-        )
+        private_key = pem_to_private_key(key_file.read(), password)
     return private_key
 
 
+def pem_to_public_key(pem_data: str):
+    """
+    Converts a PEM string to a public key.
+
+    Args:
+        pem_data (str): The PEM string to convert.
+    """
+    public_key = serialization.load_pem_public_key(
+        pem_data,
+        backend=default_backend()
+    )
+    return public_key
+
+
 def load_public_key(file_path: str):
     """
     Loads a public key from a file.
 
     Args:
         file_path (str): Path to the public key file.
 
     Returns:
         The public key.
     """
     with open(file_path, "rb") as key_file:
-        public_key = serialization.load_pem_public_key(
-            key_file.read(),
-            backend=default_backend()
-        )
+        public_key = pem_to_public_key(key_file.read())
     return public_key
 
 
 def key_to_hex(key) -> str:
     """
     Converts a private or public key to a hex string.
```

### Comparing `auto-sdk-0.1.1/auto_identity/registry.py` & `auto-sdk-0.1.2/auto_identity/registry.py`

 * *Files identical despite different names*

### Comparing `auto-sdk-0.1.1/auto_identity/utils.py` & `auto-sdk-0.1.2/auto_identity/utils.py`

 * *Files identical despite different names*

