# Comparing `tmp/pyimg4-0.8.2.tar.gz` & `tmp/pyimg4-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimg4-0.8.2.tar", max compression
+gzip compressed data, was "pyimg4-0.8.3.tar", max compression
```

## Comparing `pyimg4-0.8.2.tar` & `pyimg4-0.8.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-04-05 00:40:55.494810 pyimg4-0.8.2/LICENSE
--rw-r--r--   0        0        0     1861 2024-04-05 00:40:55.494810 pyimg4-0.8.2/README.md
--rw-r--r--   0        0        0      183 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/__init__.py
--rw-r--r--   0        0        0    28418 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/__main__.py
--rw-r--r--   0        0        0     1273 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/errors.py
--rw-r--r--   0        0        0    45343 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/parser.py
--rw-r--r--   0        0        0      313 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/types.py
--rw-r--r--   0        0        0     1377 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 pyimg4-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-05 19:38:56.486452 pyimg4-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1861 2024-04-05 19:38:56.486452 pyimg4-0.8.3/README.md
+-rw-r--r--   0        0        0      183 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/__init__.py
+-rw-r--r--   0        0        0    28418 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/__main__.py
+-rw-r--r--   0        0        0     1273 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/errors.py
+-rw-r--r--   0        0        0    45680 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyimg4/parser.py
+-rw-r--r--   0        0        0      313 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyimg4/types.py
+-rw-r--r--   0        0        0     1377 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 pyimg4-0.8.3/PKG-INFO
```

### Comparing `pyimg4-0.8.2/LICENSE` & `pyimg4-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.2/README.md` & `pyimg4-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.2/pyimg4/__main__.py` & `pyimg4-0.8.3/pyimg4/__main__.py`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.2/pyimg4/errors.py` & `pyimg4-0.8.3/pyimg4/errors.py`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.2/pyimg4/parser.py` & `pyimg4-0.8.3/pyimg4/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1158,15 +1158,15 @@
 
         self._keybags = []
         self.extra = extra
 
         self._detect_compression(size, data)
         if self.compression == Compression.LZSS:
             self._parse_complzss_header()
-        elif self.compression not in (Compression.NONE, Compression.LZFSE_ENCRYPTED):
+        elif self.compression == Compression.LZFSE:
             self.size = len(self._decompress_data(data, self.compression, size))
         else:
             self.size = size
 
     def __len__(self) -> int:
         return len(self.data)
 
@@ -1267,14 +1267,17 @@
 
         if size < 0:
             raise ValueError('Size cannot be less than 0.')
 
         if 0 < size < len(self.data):
             raise ValueError('Size cannot be less than the length of the payload data.')
 
+        if self.encrypted is True:
+            self._detect_compression(size, self._data)
+
         self._size = size
 
     def add_keybag(self, keybag: Keybag) -> None:
         if not isinstance(keybag, Keybag):
             raise UnexpectedDataError('Keybag', keybag)
 
         if any(kbag.type == keybag.type for kbag in self.keybags):
@@ -1356,14 +1359,20 @@
         self._data = self._decompress_data(self._data, self.compression, self.size)
         self._compression = Compression.NONE
         self._detect_compression(self.size, self._data)
 
     def decrypt(self, kbag: Keybag) -> None:
         self._data = AES.new(kbag.key, AES.MODE_CBC, kbag.iv).decrypt(self._data)
         self._keybags = []
+        self._detect_compression(self.size, self._data)
+
+        if self.compression == Compression.LZSS:
+            self._parse_complzss_header()
+        elif self.compression == Compression.LZFSE:
+            self.size = len(self._decompress_data(self.data, self.compression))
 
     def output(self) -> Payload:
         kbag_data = None
         if self.encrypted:
             self._encoder.start()
             with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
                 for kbag in self.keybags:
```

### Comparing `pyimg4-0.8.2/pyproject.toml` & `pyimg4-0.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyimg4"
-version = "0.8.2"
+version = "0.8.3"
 description = "A Python library/CLI tool for parsing Apple's Image4 format."
 authors = ["m1stadev <adamhamdi31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/m1stadev/PyIMG4"
 keywords = ["ios", "jailbreak", "iboot", "img4", "image4"]
 classifiers = [
```

### Comparing `pyimg4-0.8.2/PKG-INFO` & `pyimg4-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimg4
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python library/CLI tool for parsing Apple's Image4 format.
 Home-page: https://github.com/m1stadev/PyIMG4
 License: MIT
 Keywords: ios,jailbreak,iboot,img4,image4
 Author: m1stadev
 Author-email: adamhamdi31@gmail.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyimg4 Version: 0.8.2 Summary: A Python library/CLI
+Metadata-Version: 2.1 Name: pyimg4 Version: 0.8.3 Summary: A Python library/CLI
 tool for parsing Apple's Image4 format. Home-page: https://github.com/m1stadev/
 PyIMG4 License: MIT Keywords: ios,jailbreak,iboot,img4,image4 Author: m1stadev
 Author-email: adamhamdi31@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

