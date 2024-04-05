# Comparing `tmp/joker-filesys-0.2.1.tar.gz` & `tmp/joker-filesys-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-filesys-0.2.1.tar", last modified: Wed Nov 30 02:22:24 2022, max compression
+gzip compressed data, was "joker-filesys-0.2.2.tar", last modified: Fri Apr  5 03:45:40 2024, max compression
```

## Comparing `joker-filesys-0.2.1.tar` & `joker-filesys-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-30 02:22:24.220533 joker-filesys-0.2.1/
--rw-r--r--   0 Hailong    (502) staff       (20)    35140 2022-04-21 12:06:49.000000 joker-filesys-0.2.1/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-04-21 12:03:24.000000 joker-filesys-0.2.1/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1799 2022-11-30 02:22:24.220195 joker-filesys-0.2.1/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1046 2022-05-22 02:50:20.000000 joker-filesys-0.2.1/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-30 02:22:24.208200 joker-filesys-0.2.1/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-30 02:22:24.215678 joker-filesys-0.2.1/joker/filesys/
--rw-r--r--   0 Hailong    (502) staff       (20)       73 2022-11-30 02:21:14.000000 joker-filesys-0.2.1/joker/filesys/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2474 2022-05-13 12:57:29.000000 joker-filesys-0.2.1/joker/filesys/archives.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3398 2022-05-22 02:49:29.000000 joker-filesys-0.2.1/joker/filesys/cas.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3054 2022-05-13 12:57:29.000000 joker-filesys-0.2.1/joker/filesys/dirs.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2128 2022-07-26 03:33:00.000000 joker-filesys-0.2.1/joker/filesys/git.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4110 2022-06-02 05:58:50.000000 joker-filesys-0.2.1/joker/filesys/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-11-30 02:22:24.219634 joker-filesys-0.2.1/joker_filesys.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1799 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      460 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-11-30 02:22:24.000000 joker-filesys-0.2.1/joker_filesys.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       51 2022-06-09 09:32:55.000000 joker-filesys-0.2.1/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2022-11-30 02:22:24.220627 joker-filesys-0.2.1/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     1974 2022-11-03 14:45:03.000000 joker-filesys-0.2.1/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.687442 joker-filesys-0.2.2/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35140 2022-04-21 12:06:49.000000 joker-filesys-0.2.2/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-04-21 12:03:24.000000 joker-filesys-0.2.2/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1896 2024-04-05 03:45:40.687052 joker-filesys-0.2.2/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1046 2022-05-22 02:50:20.000000 joker-filesys-0.2.2/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.675850 joker-filesys-0.2.2/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.682404 joker-filesys-0.2.2/joker/filesys/
+-rw-r--r--   0 Hailong    (502) staff       (20)       73 2024-04-05 03:43:38.000000 joker-filesys-0.2.2/joker/filesys/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2474 2022-05-13 12:57:29.000000 joker-filesys-0.2.2/joker/filesys/archives.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3549 2024-04-05 03:43:38.000000 joker-filesys-0.2.2/joker/filesys/cas.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3054 2022-05-13 12:57:29.000000 joker-filesys-0.2.2/joker/filesys/dirs.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2128 2022-07-26 03:33:00.000000 joker-filesys-0.2.2/joker/filesys/git.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4446 2024-04-05 03:45:08.000000 joker-filesys-0.2.2/joker/filesys/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.685501 joker-filesys-0.2.2/joker_filesys.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1896 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      504 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-30 02:22:24.000000 joker-filesys-0.2.2/joker_filesys.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       51 2022-06-09 09:32:55.000000 joker-filesys-0.2.2/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-05 03:45:40.687524 joker-filesys-0.2.2/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     1974 2022-11-03 14:45:03.000000 joker-filesys-0.2.2/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.686355 joker-filesys-0.2.2/tests/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1844 2022-04-21 12:27:27.000000 joker-filesys-0.2.2/tests/test_filesys.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      506 2022-04-21 12:06:49.000000 joker-filesys-0.2.2/tests/test_imports.py
```

### Comparing `joker-filesys-0.2.1/LICENSE` & `joker-filesys-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.1/PKG-INFO` & `joker-filesys-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-filesys
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools dealing with files and directories.
 Home-page: https://github.com/frozflame/joker-filesys
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.20.0
+Requires-Dist: setuptools>=57.0.0
+Requires-Dist: volkanic>=0.4.0
 
 joker-filesys
 =============
 
 recent changes
 --------------
```

### Comparing `joker-filesys-0.2.1/README.md` & `joker-filesys-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.1/joker/filesys/archives.py` & `joker-filesys-0.2.2/joker/filesys/archives.py`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.1/joker/filesys/cas.py` & `joker-filesys-0.2.2/joker/filesys/cas.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import os
 from dataclasses import dataclass, field
 from functools import cached_property
 from pathlib import Path
 from typing import Iterable
 
 from joker.filesys import utils
-from joker.filesys.utils import PathLike
+from joker.filesys.utils import Pathlike, checksum_hexdigest
 
 
 @dataclass
 class ContentAddressedStorage:
-    base_dir: PathLike
-    dist_dirs: dict[str, PathLike] = field(default_factory=dict)
+    base_dir: Pathlike
+    dist_dirs: dict[str, Pathlike] = field(default_factory=dict)
     hash_algo: str = 'sha256'
     dir_depth: int = 2
     chunksize: int = 4096
 
     @classmethod
     def from_config(cls, cfg: dict | str):
         if isinstance(cfg, str):
@@ -107,9 +107,13 @@
             utils.moves(tmp, self.locate(cid))
             ho = None
         finally:
             if ho is not None:
                 tmp.unlink(missing_ok=True)
         return cid
 
+    def seize(self, path: Pathlike):
+        cid = checksum_hexdigest(path, 'sha256')
+        utils.moves(path, self.locate(cid))
+
 
 __all__ = ['ContentAddressedStorage']
```

### Comparing `joker-filesys-0.2.1/joker/filesys/dirs.py` & `joker-filesys-0.2.2/joker/filesys/dirs.py`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.1/joker/filesys/git.py` & `joker-filesys-0.2.2/joker/filesys/git.py`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.1/joker/filesys/utils.py` & `joker-filesys-0.2.2/joker/filesys/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 import mimetypes
 import os
 import shutil
 from pathlib import Path
 from typing import Generator, Union, Iterable
 from uuid import uuid4
 
-PathLike = Union[str, os.PathLike]
-FileLike = Union[str, os.PathLike, Iterable[bytes]]
+Pathlike = Union[str, os.PathLike]
+Filelike = Union[str, os.PathLike, Iterable[bytes]]
 
+# for compatibility; will be removed in version 0.3.0
+PathLike = Pathlike
+FileLike = Filelike
 
-def read_as_chunks(path: PathLike, length=-1, offset=0, chunksize=65536) \
+
+def read_as_chunks(path: Pathlike, length=-1, offset=0, chunksize=65536) \
         -> Generator[bytes, None, None]:
     if length == 0:
         return
     if length < 0:
         length = float('inf')
     chunksize = min(chunksize, length)
     with open(path, 'rb') as fin:
@@ -30,52 +34,52 @@
             if not chunk:
                 break
             yield chunk
             length -= chunksize
             chunksize = min(chunksize, length)
 
 
-def compute_checksum(path_or_chunks: FileLike, algo='sha1'):
+def compute_checksum(path_or_chunks: Filelike, algo='sha1'):
     hashobj = hashlib.new(algo) if isinstance(algo, str) else algo
     # path_or_chunks:str - a path
     if isinstance(path_or_chunks, str):
         chunks = read_as_chunks(path_or_chunks)
     else:
         chunks = path_or_chunks
     for chunk in chunks:
         hashobj.update(chunk)
     return hashobj
 
 
-def checksum(path: PathLike, algo='sha1', length=-1, offset=0):
+def checksum(path: Pathlike, algo='sha1', length=-1, offset=0):
     chunks = read_as_chunks(path, length=length, offset=offset)
     return compute_checksum(chunks, algo=algo)
 
 
-def checksum_hexdigest(path: PathLike, algo='sha1', length=-1, offset=0):
+def checksum_hexdigest(path: Pathlike, algo='sha1', length=-1, offset=0):
     hashobj = checksum(path, algo=algo, length=length, offset=offset)
     return hashobj.hexdigest()
 
 
-def b32_sha1sum(path: PathLike, length=-1, offset=0):
+def b32_sha1sum(path: Pathlike, length=-1, offset=0):
     hashobj = checksum(path, algo='sha1', length=length, offset=offset)
     return base64.b32encode(hashobj.digest()).upper().decode()
 
 
-def b64_sha384sum(path: PathLike, length=-1, offset=0):
+def b64_sha384sum(path: Pathlike, length=-1, offset=0):
     hashobj = checksum(path, algo='sha384', length=length, offset=offset)
     return base64.urlsafe_b64encode(hashobj.digest()).decode()
 
 
 def b64_encode_data_url(mediatype: str, content: bytes) -> str:
     b64 = base64.b64encode(content).decode('ascii')
     return 'data:{};base64,{}'.format(mediatype, b64)
 
 
-def b64_encode_local_file(path: PathLike) -> str:
+def b64_encode_local_file(path: Pathlike) -> str:
     mediatype = mimetypes.guess_type(path)[0]
     with open(path, 'rb') as fin:
         return b64_encode_data_url(mediatype, fin.read())
 
 
 def spread_by_prefix(filename: str, depth: int = 2, width: int = 2) -> list:
     names = []
@@ -111,34 +115,42 @@
 
 
 def gen_unique_filename(title: str = 'tmp'):
     u = uuid4().bytes.hex().upper()
     return f'{title}.{u}.part'
 
 
-def moves(old: Path, new: Path):
+def moves(old: Pathlike, new: Path):
     # old and new are possibly on different volumes
     # tmp and new are surely on the same volume
     new.parent.mkdir(parents=True, exist_ok=True)
     tmp = new.parent / gen_unique_filename(new.name)
     try:
         shutil.move(old, tmp)
         os.rename(tmp, new)
     finally:
         if tmp.exists():
             tmp.unlink(missing_ok=True)
 
 
-def saves(path: PathLike, chunks: Iterable[bytes]):
+def saves(path: Pathlike, chunks: Iterable[bytes]):
     """
     Save content safely.
     Args:
         path: the file to be created or replaced
         chunks: iterable of chunks of content to be saved
     """
     if not isinstance(path, Path):
         path = Path(path)
     tmp = path.with_name(gen_unique_filename())
     with open(tmp, 'wb') as fout:
         for chunk in chunks:
             fout.write(chunk)
     tmp.rename(path)
+
+
+def find_regular_files(dirpath, **kwargs):
+    for root, dirs, files in os.walk(dirpath, **kwargs):
+        for name in files:
+            path = os.path.join(root, name)
+            if os.path.isfile(path):
+                yield path
```

### Comparing `joker-filesys-0.2.1/joker_filesys.egg-info/PKG-INFO` & `joker-filesys-0.2.2/joker_filesys.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-filesys
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tools dealing with files and directories.
 Home-page: https://github.com/frozflame/joker-filesys
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.20.0
+Requires-Dist: setuptools>=57.0.0
+Requires-Dist: volkanic>=0.4.0
 
 joker-filesys
 =============
 
 recent changes
 --------------
```

### Comparing `joker-filesys-0.2.1/setup.py` & `joker-filesys-0.2.2/setup.py`

 * *Files identical despite different names*

