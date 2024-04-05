# Comparing `tmp/i_bip_wallet-1.0.0rc2.tar.gz` & `tmp/i_bip_wallet-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i_bip_wallet-1.0.0rc2.tar", max compression
+gzip compressed data, was "i_bip_wallet-1.0.0rc3.tar", max compression
```

## Comparing `i_bip_wallet-1.0.0rc2.tar` & `i_bip_wallet-1.0.0rc3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      209 2024-04-05 16:51:58.904563 i_bip_wallet-1.0.0rc2/i_bip_wallet/__init__.py
--rw-r--r--   0        0        0     1091 2024-03-29 22:45:12.865642 i_bip_wallet-1.0.0rc2/i_bip_wallet/_PrivateKey.py
--rw-r--r--   0        0        0     1865 2024-03-29 22:34:01.562392 i_bip_wallet-1.0.0rc2/i_bip_wallet/_PublicKey.py
--rw-r--r--   0        0        0     2150 2024-03-29 22:44:37.417557 i_bip_wallet-1.0.0rc2/i_bip_wallet/_Ripemd.py
--rw-r--r--   0        0        0     1353 2024-03-29 22:43:47.949333 i_bip_wallet-1.0.0rc2/i_bip_wallet/_Utils.py
--rw-r--r--   0        0        0      385 2024-04-05 16:52:09.554916 i_bip_wallet-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 22:02:44.981718 i_bip_wallet-1.0.0rc2/README.md
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc2/setup.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-05 16:51:58.904563 i_bip_wallet-1.0.0rc3/i_bip_wallet/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-05 17:03:44.240554 i_bip_wallet-1.0.0rc3/i_bip_wallet/_PrivateKey.py
+-rw-r--r--   0        0        0     1865 2024-03-29 22:34:01.562392 i_bip_wallet-1.0.0rc3/i_bip_wallet/_PublicKey.py
+-rw-r--r--   0        0        0     2150 2024-03-29 22:44:37.417557 i_bip_wallet-1.0.0rc3/i_bip_wallet/_Ripemd.py
+-rw-r--r--   0        0        0     1353 2024-03-29 22:43:47.949333 i_bip_wallet-1.0.0rc3/i_bip_wallet/_Utils.py
+-rw-r--r--   0        0        0      385 2024-04-05 17:04:04.257461 i_bip_wallet-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-29 22:02:44.981718 i_bip_wallet-1.0.0rc3/README.md
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc3/setup.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 i_bip_wallet-1.0.0rc3/PKG-INFO
```

### Comparing `i_bip_wallet-1.0.0rc2/i_bip_wallet/_PrivateKey.py` & `i_bip_wallet-1.0.0rc3/i_bip_wallet/_PublicKey.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,54 @@
-import secrets
+import binascii
 from typing import Union
 
 from hexbytes import HexBytes
 
-class PrivateKey:
+import ecdsa
 
-    def __init__(self, Keys: Union[str, bytes, bytearray, HexBytes, int]) -> None:
+from ._PrivateKey import PrivateKey
+
+class PublicKey:
+
+    def __init__(self, Keys: Union[PrivateKey, str, bytes, bytearray, HexBytes, int], Compressed: bool = True) -> None:
         if isinstance(Keys, str): 
             self.__keys__ = HexBytes(Keys)
         elif isinstance(Keys, (bytes, bytearray, HexBytes)):
             self.__keys__ = HexBytes(Keys)
         elif isinstance(Keys, int):
             self.__keys__ = HexBytes(hex(Keys))
+        elif isinstance(Keys, int):
+            self.__keys__ = HexBytes(hex(Keys))
+        elif isinstance(Keys, PrivateKey):
+            if Compressed:
+                __keys__ = ecdsa.SigningKey.from_string(HexBytes(bytes(Keys)), curve=ecdsa.SECP256k1).get_verifying_key().to_string()
+                x_coord = __keys__[:int(len(__keys__) / 2)]
+                if int(binascii.hexlify(__keys__[int(len(__keys__) / 2):]), 16) % 2 == 0:
+                    self.__keys__ = HexBytes(b'\x02' + x_coord)
+                else:
+                    self.__keys__ = HexBytes(b'\x03' + x_coord)
+            else:
+                self.__keys__ = HexBytes(b'\x04' + ecdsa.SigningKey.from_string(HexBytes(bytes(Keys)), curve=ecdsa.SECP256k1).get_verifying_key().to_string())
 
     def __str__(self) -> str:
         return self.__keys__.hex()
     
     def __bytes__(self) -> bytes:
         return HexBytes(self.__keys__)
     
     @classmethod
-    def generate(cls):
-        return cls(HexBytes(secrets.token_hex(32))) # Generate random PrivateKey
+    def FromPrivateKey(cls, Keys: PrivateKey):
+        return cls(Keys)
     
     @classmethod
     def FromHex(cls, Keys: str):
         return cls(Keys)
     
     @classmethod
     def FromBytes(cls, Keys: Union[bytes, bytearray, HexBytes]):
         return cls(Keys)
     
     @classmethod
     def FromInt(cls, Keys: int):
         return cls(Keys)
     
-    @classmethod
-    def FromWif(cls):
-        return 'Not Found'
+
```

### Comparing `i_bip_wallet-1.0.0rc2/i_bip_wallet/_PublicKey.py` & `i_bip_wallet-1.0.0rc3/i_bip_wallet/_Ripemd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 import binascii
 from typing import Union
 
-from hexbytes import HexBytes
-
 import ecdsa
+from hexbytes import HexBytes
 
 from ._PrivateKey import PrivateKey
+from ._PublicKey import PublicKey
+from ._Utils import Utils
 
-class PublicKey:
+class Ripemd:
 
-    def __init__(self, Keys: Union[PrivateKey, str, bytes, bytearray, HexBytes, int], Compressed: bool = True) -> None:
+    def __init__(self, Keys: Union[PrivateKey, PublicKey, str, bytes, bytearray, HexBytes, int], Compressed: bool = True) -> None:
         if isinstance(Keys, str): 
             self.__keys__ = HexBytes(Keys)
         elif isinstance(Keys, (bytes, bytearray, HexBytes)):
             self.__keys__ = HexBytes(Keys)
         elif isinstance(Keys, int):
             self.__keys__ = HexBytes(hex(Keys))
         elif isinstance(Keys, int):
             self.__keys__ = HexBytes(hex(Keys))
         elif isinstance(Keys, PrivateKey):
             if Compressed:
                 __keys__ = ecdsa.SigningKey.from_string(HexBytes(bytes(Keys)), curve=ecdsa.SECP256k1).get_verifying_key().to_string()
                 x_coord = __keys__[:int(len(__keys__) / 2)]
                 if int(binascii.hexlify(__keys__[int(len(__keys__) / 2):]), 16) % 2 == 0:
-                    self.__keys__ = HexBytes(b'\x02' + x_coord)
+                    _keys = HexBytes(b'\x02' + x_coord)
                 else:
-                    self.__keys__ = HexBytes(b'\x03' + x_coord)
+                    _keys = HexBytes(b'\x03' + x_coord)
             else:
-                self.__keys__ = HexBytes(b'\x04' + ecdsa.SigningKey.from_string(HexBytes(bytes(Keys)), curve=ecdsa.SECP256k1).get_verifying_key().to_string())
+                _keys = HexBytes(b'\x04' + ecdsa.SigningKey.from_string(HexBytes(bytes(Keys)), curve=ecdsa.SECP256k1).get_verifying_key().to_string())
+            self.__keys__ = Utils.Ripemd(_keys)
+        elif isinstance(Keys, PublicKey):
+            self.__keys__ = Utils.Ripemd(HexBytes(bytes(Keys)))
 
     def __str__(self) -> str:
         return self.__keys__.hex()
     
     def __bytes__(self) -> bytes:
         return HexBytes(self.__keys__)
     
     @classmethod
     def FromPrivateKey(cls, Keys: PrivateKey):
         return cls(Keys)
     
     @classmethod
+    def FromPublicKey(cls, Keys: PublicKey):
+        return cls(Keys)
+    
+    @classmethod
     def FromHex(cls, Keys: str):
         return cls(Keys)
     
     @classmethod
     def FromBytes(cls, Keys: Union[bytes, bytearray, HexBytes]):
         return cls(Keys)
     
     @classmethod
     def FromInt(cls, Keys: int):
-        return cls(Keys)
-    
-    
+        return cls(Keys)
```

### Comparing `i_bip_wallet-1.0.0rc2/i_bip_wallet/_Utils.py` & `i_bip_wallet-1.0.0rc3/i_bip_wallet/_Utils.py`

 * *Files identical despite different names*

### Comparing `i_bip_wallet-1.0.0rc2/setup.py` & `i_bip_wallet-1.0.0rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['ecdsa>=0.18.0,<0.19.0', 'pycryptodomex>=3.20.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'i-bip-wallet',
-    'version': '1.0.0rc2',
+    'version': '1.0.0rc3',
     'description': '',
     'long_description': '',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `i_bip_wallet-1.0.0rc2/PKG-INFO` & `i_bip_wallet-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-bip-wallet
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

