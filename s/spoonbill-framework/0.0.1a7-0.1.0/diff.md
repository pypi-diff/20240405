# Comparing `tmp/spoonbill_framework-0.0.1a7.tar.gz` & `tmp/spoonbill_framework-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spoonbill_framework-0.0.1a7.tar", max compression
+gzip compressed data, was "spoonbill_framework-0.1.0.tar", max compression
```

## Comparing `spoonbill_framework-0.0.1a7.tar` & `spoonbill_framework-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1055 2023-01-03 22:33:05.588124 spoonbill_framework-0.0.1a7/LICENSE
--rw-r--r--   0        0        0    36060 2023-08-31 19:39:47.547099 spoonbill_framework-0.0.1a7/README.md
--rw-r--r--   0        0        0     1280 2023-08-30 15:13:06.312078 spoonbill_framework-0.0.1a7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-15 12:07:46.016696 spoonbill_framework-0.0.1a7/spoonbill/__init__.py
--rw-r--r--   0        0        0    11975 2023-08-31 18:58:06.760451 spoonbill_framework-0.0.1a7/spoonbill/datastores/__init__.py
--rw-r--r--   0        0        0     5000 2023-08-29 19:48:56.285091 spoonbill_framework-0.0.1a7/spoonbill/datastores/buckets.py
--rw-r--r--   0        0        0     7051 2023-08-29 19:48:56.285344 spoonbill_framework-0.0.1a7/spoonbill/datastores/cosmos.py
--rw-r--r--   0        0        0     9908 2023-08-29 19:48:56.285732 spoonbill_framework-0.0.1a7/spoonbill/datastores/dynamodb.py
--rw-r--r--   0        0        0     2076 2023-08-29 19:48:56.286036 spoonbill_framework-0.0.1a7/spoonbill/datastores/filesystem.py
--rw-r--r--   0        0        0     4895 2023-08-29 19:48:56.286179 spoonbill_framework-0.0.1a7/spoonbill/datastores/firestore.py
--rw-r--r--   0        0        0     1580 2023-08-29 19:48:56.286496 spoonbill_framework-0.0.1a7/spoonbill/datastores/inmemory.py
--rw-r--r--   0        0        0     4085 2023-08-31 18:58:06.760614 spoonbill_framework-0.0.1a7/spoonbill/datastores/leveldb.py
--rw-r--r--   0        0        0     2604 2023-08-29 19:48:56.286697 spoonbill_framework-0.0.1a7/spoonbill/datastores/lmdb.py
--rw-r--r--   0        0        0     4782 2023-08-29 19:48:56.286921 spoonbill_framework-0.0.1a7/spoonbill/datastores/modal.py
--rw-r--r--   0        0        0     6012 2023-08-29 19:48:56.287065 spoonbill_framework-0.0.1a7/spoonbill/datastores/mongodb.py
--rw-r--r--   0        0        0     2041 2023-08-29 19:48:56.287377 spoonbill_framework-0.0.1a7/spoonbill/datastores/pysos.py
--rw-r--r--   0        0        0     1763 2023-08-30 15:13:06.312359 spoonbill_framework-0.0.1a7/spoonbill/datastores/rdict.py
--rw-r--r--   0        0        0     6414 2023-08-29 19:48:56.287514 spoonbill_framework-0.0.1a7/spoonbill/datastores/redis.py
--rw-r--r--   0        0        0     1355 2023-08-30 15:13:06.312479 spoonbill_framework-0.0.1a7/spoonbill/datastores/rocksdb.py
--rw-r--r--   0        0        0     6989 2023-08-29 19:48:56.287742 spoonbill_framework-0.0.1a7/spoonbill/datastores/safetensors.py
--rw-r--r--   0        0        0      933 2023-08-29 19:48:56.287880 spoonbill_framework-0.0.1a7/spoonbill/datastores/shelve.py
--rw-r--r--   0        0        0     1272 2023-08-30 15:13:06.312623 spoonbill_framework-0.0.1a7/spoonbill/datastores/speedb.py
--rw-r--r--   0        0        0     2814 2023-08-30 12:40:00.594576 spoonbill_framework-0.0.1a7/spoonbill/datastores/unqlite.py
--rw-r--r--   0        0        0     1859 2023-01-03 22:33:05.592990 spoonbill_framework-0.0.1a7/spoonbill/filesystem.py
--rw-r--r--   0        0        0    37260 1970-01-01 00:00:00.000000 spoonbill_framework-0.0.1a7/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-01-03 22:33:05.588124 spoonbill_framework-0.1.0/LICENSE
+-rw-r--r--   0        0        0    37001 2024-04-05 20:28:53.275260 spoonbill_framework-0.1.0/README.md
+-rw-r--r--   0        0        0     1314 2024-04-05 20:28:53.275783 spoonbill_framework-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-15 12:07:46.016696 spoonbill_framework-0.1.0/spoonbill/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 20:28:53.275875 spoonbill_framework-0.1.0/spoonbill/datastores/__init__.py
+-rw-r--r--   0        0        0    10709 2024-04-05 20:28:53.276092 spoonbill_framework-0.1.0/spoonbill/datastores/base.py
+-rw-r--r--   0        0        0     4961 2024-04-05 20:28:53.276285 spoonbill_framework-0.1.0/spoonbill/datastores/buckets.py
+-rw-r--r--   0        0        0     7121 2024-04-05 20:28:53.276466 spoonbill_framework-0.1.0/spoonbill/datastores/cosmos.py
+-rw-r--r--   0        0        0    10037 2024-04-05 20:28:53.276672 spoonbill_framework-0.1.0/spoonbill/datastores/dynamodb.py
+-rw-r--r--   0        0        0     1985 2024-04-05 20:28:53.276842 spoonbill_framework-0.1.0/spoonbill/datastores/filesystem.py
+-rw-r--r--   0        0        0     4892 2024-04-05 20:28:53.277037 spoonbill_framework-0.1.0/spoonbill/datastores/firestore.py
+-rw-r--r--   0        0        0     1500 2024-04-05 20:28:53.277208 spoonbill_framework-0.1.0/spoonbill/datastores/inmemory.py
+-rw-r--r--   0        0        0     2346 2024-04-05 20:28:53.277369 spoonbill_framework-0.1.0/spoonbill/datastores/jsonstore.py
+-rw-r--r--   0        0        0     4103 2024-04-05 20:28:53.277544 spoonbill_framework-0.1.0/spoonbill/datastores/leveldb.py
+-rw-r--r--   0        0        0     2618 2024-04-05 20:28:53.277726 spoonbill_framework-0.1.0/spoonbill/datastores/lmdb.py
+-rw-r--r--   0        0        0     4787 2024-04-05 20:28:53.277950 spoonbill_framework-0.1.0/spoonbill/datastores/modal.py
+-rw-r--r--   0        0        0     6052 2024-04-05 20:28:53.278134 spoonbill_framework-0.1.0/spoonbill/datastores/mongodb.py
+-rw-r--r--   0        0        0     2027 2024-04-05 20:28:53.278359 spoonbill_framework-0.1.0/spoonbill/datastores/pysos.py
+-rw-r--r--   0        0        0     1781 2024-04-05 20:28:53.278530 spoonbill_framework-0.1.0/spoonbill/datastores/rdict.py
+-rw-r--r--   0        0        0     6447 2024-04-05 20:28:53.278725 spoonbill_framework-0.1.0/spoonbill/datastores/redis.py
+-rw-r--r--   0        0        0     1355 2023-08-30 15:13:06.312479 spoonbill_framework-0.1.0/spoonbill/datastores/rocksdb.py
+-rw-r--r--   0        0        0     7084 2024-04-05 20:28:53.278905 spoonbill_framework-0.1.0/spoonbill/datastores/safetensors.py
+-rw-r--r--   0        0        0      938 2024-04-05 20:28:53.279074 spoonbill_framework-0.1.0/spoonbill/datastores/shelve.py
+-rw-r--r--   0        0        0     1272 2023-08-30 15:13:06.312623 spoonbill_framework-0.1.0/spoonbill/datastores/speedb.py
+-rw-r--r--   0        0        0     2776 2024-04-05 20:28:53.279246 spoonbill_framework-0.1.0/spoonbill/datastores/unqlite.py
+-rw-r--r--   0        0        0      321 2024-04-05 19:57:44.397955 spoonbill_framework-0.1.0/spoonbill/datastores/utils.py
+-rw-r--r--   0        0        0     1859 2023-01-03 22:33:05.592990 spoonbill_framework-0.1.0/spoonbill/filesystem.py
+-rw-r--r--   0        0        0    38220 1970-01-01 00:00:00.000000 spoonbill_framework-0.1.0/PKG-INFO
```

### Comparing `spoonbill_framework-0.0.1a7/LICENSE` & `spoonbill_framework-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.0.1a7/README.md` & `spoonbill_framework-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -178,28 +178,49 @@
 # Also works with any dict-like object
 from collections import defaultdict, OrderedDict, Counter
 
 store = InMemoryStore(defaultdict)
 store = InMemoryStore(OrderedDict)
 store = InMemoryStore(Counter)
 ```
+## JsonStore
+
+A simple json-file store where each call read and write a json file.   
+Not very effeicint for many calls but great for a small configuration singelton file.   
+Biggest benefit is that the file which is written is human-readable.
+
+* `lockfile_path` can be used as a locking mechanism. Requires `pip install filelock`.
+* `use_jsonpickle` can be use instead of pure json to handle more complicated objects like numpy arrays. Requires `pip install jsonpickle`
+* Cloud-native, if the path is `s3,gs,az`, it should still work.   
+  
+> ⚠️ The cloud native is un-tested.
+
+```python
+from spoonbill.datastores.jsonstore import JsonStore
+
+store = JsonStore.open(path='file.json', 
+                      strict=True, 
+                      lockfile_path=tmpdir.name+'file.lock',
+                      use_jsonpickle=True)
+```
+
 
 ## [LmdbStore](https://github.com/Dobatymo/lmdb-python-dbm)
 
 An LMDB key-value store based on [lmdb-python-dbm](https://github.com/Dobatymo/lmdb-python-dbm). This is ideal for lists
 or datastores which either need persistence, are too big to fit in memory or both.   
 This is a Python DBM interface style wrapper around [LMDB](http://www.lmdb.tech/doc/) (Lightning Memory-Mapped Database)
 
 [Details](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database)
 
 Requirements:   
 ```pip install lmdbm```
 
 ```python
-from spoonbill.datastores import LmdbStore
+from spoonbill.datastores.lmdb import LmdbStore
 
 store = LmdbStore.open('tmp.db')
 ```
 
 ## [PysosStore](https://github.com/dagnelies/pysos)
 
 This is ideal for lists or dictionaries which either need persistence, are too big to fit in memory or both.
@@ -215,27 +236,27 @@
 * it is platform independent, unlike shelve which relies on an underlying dbm implementation, which may vary from system
   to system the data is stored in a plain text format
 
 Requirements:   
 ```pip install pysos```
 
 ```python
-from spoonbill.datastores import PysosStore
+from spoonbill.datastores.pysos import PysosStore
 
 store = PysosStore.open('tmp.db')
 ```
 
 ## [Shelve](https://docs.python.org/3/library/shelve.html)
 
 The difference with “dbm” databases is that the values (not the keys!) in a shelf can be essentially arbitrary Python
 objects — anything that the pickle module can handle. This includes most class instances, recursive data types, and
 objects containing lots of shared sub-objects. The keys are ordinary strings.
 
 ```python
-from spoonbill.datastores import ShelveStore
+from spoonbill.datastores.shelve import ShelveStore
 
 store = ShelveStore.open('tmp.db')
 ```
 
 ## [Safetensors](https://github.com/huggingface/safetensors)
 
 This is ideal whe you want to work with tensors from disc, but it is a frozen store - no set or update.
@@ -292,15 +313,15 @@
 * It supports caching
 * It can be exported to a local directory or other clouds (s3, gs, az, etc)
 
 For faster applications with cloud persistence, you can use InMemoryStore/LmdbStore and save/load to the cloud after
 updates.
 
 ```python
-from spoonbill.datastores import FilesystemStore
+from spoonbill.datastores.filesystem import FilesystemStore
 
 # set strict to True to use redis with its default behaviour which turns keys and values to strings
 store = FilesystemStore.open("s3://bucket/path/to/store")
 store.save("local_dir_path")
 ```
 
 ## [Redis](https://github.com/redis/redis-py)
@@ -312,15 +333,15 @@
   expect from redis.
 * Redis doesn't have any search for values.
 
 Requirements:   
 ```pip install redis```
 
 ```python
-from spoonbill.datastores import RedisStore
+from spoonbill.datastores.redis import RedisStore
 
 # set strict to True to use redis with its default behaviour which turns keys and values to strings
 store = RedisStore.open("redis://localhost:6379/1")
 store[1] = 1
 assert store[1] == store["1"] == "1"
 
 assert list(store.keys('1*')) == ['111', '1', '11']  # redis turn every key to string
@@ -338,15 +359,15 @@
     * Bad Example: `store['key'] = "a value which is not a dict"`
 
 Recommended using with `strict=True` to enjoy all the benefits of backends including **searches**.
 
 Searches API Example:
 
 ```python
-from spoonbill.datastores import MongoDBStore
+from spoonbill.datastores.mongodb import MongoDBStore
 
 store = MongoDBStore()
 store.keys(pattern="*", limit=10)  # scan keys to a pattern
 store.values(keys=['key1', 'key2'])  # retrieve a batch of values efficiently 
 store.items(conditions={'a': '1+', 'b': 1}, limit=10)  # filter based on match conditions
 ```
 
@@ -354,15 +375,15 @@
 
 * Save/load is only implemented for `strict=True`.
 
 Requirements:
 ```pip install pymongo```
 
 ```python
-from spoonbill.datastores import MongoDBStore
+from spoonbill.datastores.dynamodb import DynamoDBStore
 
 store = MongoDBStore.open(uri='mongodb://localhost:27017/')
 ```
 
 ## [DynamoDB]((https://aws.amazon.com/dynamodb/))
 
 Notes:
@@ -396,15 +417,15 @@
 7. Install google-cloud-firestore with
 
 ```bash
 pip install --upgrade google-cloud-firestore 
 ```
 
 ```python
-from spoonbill.datastores import Firestore
+from spoonbill.datastores.firestore import Firestore
 
 # this rest of the credentials are picked up from the file in the GOOGLE_APPLICATION_CREDENTIALS environment variable
 store = Firestore.open(table_name="my-collection")
 ```
 
 ## [Azure CosmosDB]((https://www.google.com/search?client=safari&rls=en&q=Azure+Cosmos&ie=UTF-8&oe=UTF-8))
 
@@ -418,15 +439,15 @@
 Prerequisites: [Quickstart](https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/quickstart-python?tabs=azure-portal%2Clinux)
 
 Requirements:
 
 ```pip install azure-cosmos```
 
 ```python
-from spoonbill.datastores import CosmosDBStore
+from spoonbill.datastores.cosmos import CosmosDBStore
 
 store = CosmosDBStore.open(database='db',
                            container='container',
                            endpoint='endpoint',
                            credential='credential')
 ```
 
@@ -455,15 +476,15 @@
 
 Within the runtime, the **context app** is passed to the store to be able to update the data.
 
 Within a function, only the **name** of the dict is needed.
 
 ```python 
 import modal
-from spoonbill.datastores import ModalStore
+from spoonbill.datastores.modal import ModalStore
 
 image = modal.Image.debian_slim().pip_install("spoonbill-framework")
 
 name = "data"
 stub = modal.Stub("app name", **kwargs)
 # with stub
 store = ModalStore.open(name=name, stub=stub, data={"key": "value"})  # data is optional
@@ -490,15 +511,15 @@
 UnQLite is a in-process software library which implements a self-contained, serverless, zero-configuration,
 transactional NoSQL database engine.
 
 Requirements:   
 ```pip install unqlite```
 
 ```python
-from spoonbill.datastores import UnQLiteStore
+from spoonbill.datastores.unqlite import UnQLiteStore
 
 store = UnQLiteStore.open('tmp.db')  # leave empty for in-memory
 ```
 
 ## [Speedb](https://github.com/speedb-io/speedb)
 
 A first-of-its-kind, community-led key-value storage engine, designed to support modern data sets.
@@ -511,15 +532,15 @@
   use [RocksDict](https://github.com/Congyuwang/RocksDict) directly.
 * The save and load is a bit different from the other stores. It is not a dump and load of the data, save to a file and
   ingest back.
 * Requirements:   
   ```pip install speedict```
 
 ```python
-from spoonbill.datastores import SpeedbStore
+from spoonbill.datastores.speedb import SpeedbStore
 
 store = SpeedbStore.open('directory/')
 
 store.save('file.sst')
 # load 
 store.ingest('file.sst')
 
@@ -541,15 +562,15 @@
 * The save and load is a bit different from the other stores. It is not a dump and load of the data, save to a file and
   ingest back.
 
 * Requirements:   
   ```pip install rocksdict```
 
 ```python
-from spoonbill.datastores import RocksDBStore
+from spoonbill.datastores.rocksdb import RocksDBStore
 
 store = RocksDBStore.open('directory/')
 
 store.save('file.sst')
 # load 
 store.ingest('file.sst')
 
@@ -572,13 +593,13 @@
 ```
 pip install plyvel
 # or 
 pip install plyvel-ci
 ```
 
 ```python
-from spoonbill.datastores import LevelDBStore
+from spoonbill.datastores.leveldb import LevelDBStore
 
 store = LevelDBStore.open('directory/')
 
 ```
```

### Comparing `spoonbill_framework-0.0.1a7/pyproject.toml` & `spoonbill_framework-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spoonbill-framework"
-version = "0.0.1a7"
+version = "0.1.0"
 license = "LICENSE"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["dict", "key-value", "gcp", "azure", "aws", "s3", "lmdb", "pysos", "redis", "dynamodb", "mongodb", "cosmosdb", "safetensors", "unqlite"]
@@ -32,14 +32,15 @@
 gcp = ["google-cloud-firestore"]
 azure = ["azure-cosmos"]
 dev = ["pytest", "sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints", "sphinxcontrib-napoleon", "sphinxcontrib-apidoc"]
 modal = ["modal-client"]
 unqlite = ["unqlite"]
 rocksdb = ["rocksdict"]
 speedb = ["speedict"]
+json = ["filelock", "cloudpathlib"]
 
 [tool.setuptools]
 packages = ["spoonbill"]
 
 [project.urls]
 Homepage = "https://github.com/xdssio/spoonbill"
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/__init__.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
-import contextlib
 import cloudpickle
 import re
 from spoonbill.filesystem import FileSystem
 
+
 KEY = 'ID__'
 VALUE = 'VALUE__'
 RANDOM_VALUE = '#5f1a7da3a2b04d629231108bb6548dcb#'
 
 
 class Strict:
     """
@@ -184,21 +184,22 @@
     def set(self, key, value):
         return self._store.set(self.encode_key(key), self.encode_value(value))
 
     def delete(self, key):
         return self.pop(key)
 
     def update(self, d):
-        self._store.update({self.encode_key(key): self.encode_value(value) for key, value in d.items()})
+        self._store.update({self.encode_key(key): self.encode_value(
+            value) for key, value in d.items()})
         return self
 
     def __repr__(self):
         size = len(self)
         items = str({key: value for i, (key, value) in enumerate(self.items()) if i < 5})[
-                :-1] + '...' if size > 5 else str({key: value for key, value in self.items()})
+            :-1] + '...' if size > 5 else str({key: value for key, value in self.items()})
         return f"{self.__class__.__name__}() of size {size}\n{items}"
 
     def _from_directory(self, path):
         mapper = FileSystem(path).get_mapper()
         self._flush()
 
         def decode_key(key):
@@ -301,73 +302,26 @@
 
     def popitem(self):
         with self.context as store:
             return self.encode_value(store.popitem())
 
     def update(self, d):
         with self.context as store:
-            store.update({self.encode_key(key): self.encode_value(value) for key, value in d.items()})
+            store.update({self.encode_key(key): self.encode_value(value)
+                         for key, value in d.items()})
         return self
 
     def _cp(self, source, target, **kwargs):
 
-        FileSystem(target).write_bytes(FileSystem(source, **kwargs).read_bytes())
+        FileSystem(target).write_bytes(
+            FileSystem(source, **kwargs).read_bytes())
 
         # save_bytes(target, load_bytes(source, **kwargs), **kwargs)
         return True
 
     def save(self, path):
         self._cp(self.store_path, path)
         return path
 
     def load(self, path):
         self._cp(path, self.store_path)
         return self
-
-
-from .inmemory import InMemoryStore
-from .shelve import ShelveStore
-
-with contextlib.suppress(ImportError):
-    from .redis import RedisStore
-
-with contextlib.suppress(ImportError):
-    from .lmdb import LmdbStore
-
-with contextlib.suppress(ImportError):
-    from .pysos import PysosStore
-
-with contextlib.suppress(ImportError):
-    from .dynamodb import DynamoDBStore
-
-with contextlib.suppress(ImportError):
-    from .firestore import Firestore
-
-with contextlib.suppress(ImportError):
-    from .filesystem import FilesystemStore
-
-with contextlib.suppress(ImportError):
-    from .cosmos import CosmosDBStore
-
-with contextlib.suppress(ImportError):
-    from .mongodb import MongoDBStore
-
-with contextlib.suppress(ImportError):
-    from .safetensors import SafetensorsStore, SafetensorsInMemoryStore, serialize, deserialize
-
-with contextlib.suppress(ImportError):
-    from .safetensors import SafetensorsLmdbStore
-
-with contextlib.suppress(ImportError):
-    from .modal import ModalStore
-
-with contextlib.suppress(ImportError):
-    from .unqlite import UnQLiteStore
-
-with contextlib.suppress(ImportError):
-    from .speedb import SpeedbStore
-
-with contextlib.suppress(ImportError):
-    from .rocksdb import RocksDBStore
-
-with contextlib.suppress(ImportError):
-    from .leveldb import LevelDBStore
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/buckets.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/buckets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import pathlib
-import re
 import shutil
-from spoonbill.datastores import KeyValueStore, VALUE
-
-
-def is_cloud_url(path):
-    return re.match("^s3:\/\/|^az:\/\/|^gs:\/\/", str(path)) is not None
+from spoonbill.datastores.base import KeyValueStore, VALUE
+from spoonbill.datastores.utils import is_cloud_url
 
 
 class BucketStore(KeyValueStore):
     """
     A dictionary implemented as a bucket of files.
     Pros: cloud persistent, cheap.
     Cons: slow.
@@ -97,15 +93,16 @@
             return self.decode_value(file.read_text())
         return default
 
     def set(self, key, value):
         self._put_item(key, value)
 
     def _iter_keys(self, pattern: str = None, limit: int = None):
-        iterator = self.bucket.glob(pattern) if pattern is not None else self.bucket.iterdir()
+        iterator = self.bucket.glob(
+            pattern) if pattern is not None else self.bucket.iterdir()
         for i, key in enumerate(iterator):
             if i == limit:
                 break
             if key.name == self.COUNT_KEY:
                 continue
             if key.is_file():
                 yield key
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/cosmos.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/cosmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import contextlib
-from spoonbill.datastores import KeyValueStore, VALUE
+from spoonbill.datastores.base import KeyValueStore, VALUE
 from azure.cosmos import CosmosClient, PartitionKey
 import azure.cosmos.exceptions
 import json
 
 ID = 'id'
 KEY = '_KEY_'
 
@@ -21,15 +21,16 @@
                  endpoint: str = None,
                  credential: str = None,
                  partition_key=DEFAULT_PARTITION_KEY,
                  strict=True):
         self.client = CosmosClient(url=endpoint or os.getenv('COSMOS_ENDPOINT'),
                                    credential=credential or os.getenv('COSMOS_KEY'))
         self.database_name = database
-        self.database = self.client.create_database_if_not_exists(id=self.database_name)
+        self.database = self.client.create_database_if_not_exists(
+            id=self.database_name)
         self.container = self.database.create_container_if_not_exists(
             id=container, partition_key=PartitionKey(path=partition_key), offer_throughput=400)
         self.strict = strict
         self.as_string = True
 
     @classmethod
     def open(cls, database: str = 'db', container: str = 'container', endpoint: str = None, credential: str = None,
@@ -51,15 +52,16 @@
 
     def _to_key_value(self, item):
         if item is not None:
             key = self.decode_value(item.pop(ID))
             if VALUE in item:
                 value = self.decode_value(item[VALUE])
             else:
-                value = {k: v for k, v in item.items() if not str(k).startswith('_')}
+                value = {k: v for k, v in item.items(
+                ) if not str(k).startswith('_')}
             key = self.decode_key(key)
             return key, value
 
     def _put_item(self, key, value):
         self.container.create_item(self._to_item(key, value))
 
     def _get_item(self, key):
@@ -107,15 +109,16 @@
     def _iter_items(self, conditions: dict = None, limit: int = None):
         conditions = conditions or {}
         wheres = []
         for feature, pattern in conditions.items():
             if isinstance(pattern, str):
                 wheres.append('c.{} LIKE "%{}%"'.format(feature, pattern))
             else:
-                wheres.append(f'c.{feature} = {pattern}'.format(feature, pattern))
+                wheres.append(
+                    f'c.{feature} = {pattern}'.format(feature, pattern))
         query = f"SELECT * FROM {self.container.id} c"
         if wheres:
             query = query + ' WHERE ' + ' AND '.join(wheres)
         if limit:
             query = query + f" OFFSET 0 LIMIT {limit}"
         for item in self.container.query_items(
                 query=query,
@@ -132,15 +135,16 @@
         for item in self.container.query_items(
                 query=query,
                 enable_cross_partition_query=True
         ):
             yield self._to_key_value(item)
 
     def keys(self, pattern: str = None, limit: int = None):
-        where = ' WHERE ' + 'c.id LIKE "%{}%"'.format(pattern) if pattern else None
+        where = ' WHERE ' + \
+            'c.id LIKE "%{}%"'.format(pattern) if pattern else None
         for item in self._iter_keys(where=where, limit=limit):
             yield item[0]
 
     def items(self, conditions: dict = None, limit: int = None):
         if conditions is not None and not hasattr(conditions, 'items'):
             conditions = {VALUE: conditions}
         for item in self._iter_items(conditions=conditions, limit=limit):
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/dynamodb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 import logging
 import warnings
 
-from spoonbill.datastores import KeyValueStore, KEY, VALUE
+from spoonbill.datastores.base import KeyValueStore, KEY, VALUE
 import boto3
 import decimal
 import botocore
 import time
 
 logger = logging.getLogger()
 
@@ -48,18 +48,20 @@
                      key_schema: typing.List[dict] = None,  # Partition key
                      attribute_definitions: typing.List[dict] = None,
                      billing_mode: str = None,
                      **kwargs):
         table_name = table_name or self.table_name
 
         if not table_name in self._list_tables():
-            key_schema = key_schema or kwargs.pop('AttributeDefinitions', [{'AttributeName': self.key, 'KeyType': 'HASH'}])
+            key_schema = key_schema or kwargs.pop(
+                'AttributeDefinitions', [{'AttributeName': self.key, 'KeyType': 'HASH'}])
             attribute_definitions = attribute_definitions or kwargs.pop('AttributeDefinitions', [
                 {'AttributeName': self.key, 'AttributeType': self.key_type}])
-            billing_mode = billing_mode or kwargs.pop('BillingMode', 'PAY_PER_REQUEST')
+            billing_mode = billing_mode or kwargs.pop(
+                'BillingMode', 'PAY_PER_REQUEST')
             return self.client.create_table(TableName=table_name, KeySchema=key_schema,
                                             AttributeDefinitions=attribute_definitions,
                                             BillingMode=billing_mode,
                                             **kwargs)
         return False
 
     def _delete_table(self, table_name: str = None):
@@ -105,23 +107,26 @@
     def _to_key_value(self, item):
         if isinstance(item, tuple):
             return item
         key = item.pop(KEY)
         return key, self._process_item(item)
 
     def _get_item(self, key: str):
-        response = self.table.get_item(TableName=self.table_name, Key=self._to_key(key))
+        response = self.table.get_item(
+            TableName=self.table_name, Key=self._to_key(key))
         if ITEM in response:
             return self._to_key_value(response[ITEM])
 
     def _put_item(self, key: str, value: str):
-        self.table.put_item(TableName=self.table_name, Item=self._to_item(key, value))
+        self.table.put_item(TableName=self.table_name,
+                            Item=self._to_item(key, value))
 
     def _delete_item(self, key: str):
-        self.table.delete_item(TableName=self.table_name, Key=self._to_key(key))
+        self.table.delete_item(TableName=self.table_name,
+                               Key=self._to_key(key))
 
     @property
     def description(self):
         return self.client.describe_table(TableName=self.table_name)
 
     def __len__(self):
         return int(self.client.scan(TableName=self.table_name, Select='COUNT')['Count'])
@@ -200,15 +205,16 @@
         responses = self.client.batch_get_item(
             RequestItems={self.table_name: {'Keys': [self._to_dynamodb_key(key) for key in keys]}})
         for item in responses['Responses'][self.table_name]:
             yield self._to_key_value(from_dynamodb_json(item))
 
     def keys(self, pattern: str = None, limit: int = None):
         is_valid = self._to_filter(KEY, pattern) if pattern else lambda x: True
-        params = {'TableName': self.table_name, 'Select': 'SPECIFIC_ATTRIBUTES', 'AttributesToGet': [KEY]}
+        params = {'TableName': self.table_name,
+                  'Select': 'SPECIFIC_ATTRIBUTES', 'AttributesToGet': [KEY]}
         i = 0
         for key, value in self._table_scan(params):
             if i == limit:
                 break
             if is_valid(key):
                 i += 1
                 yield key
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/filesystem.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from spoonbill.datastores import KeyValueStore, InMemoryStore
-from fsspec import AbstractFileSystem, get_filesystem_class
-from fsspec.implementations.cached import SimpleCacheFileSystem
-import typing
+from spoonbill.datastores.base import KeyValueStore
+from spoonbill.datastores.inmemory import InMemoryStore
+
 import fsspec
 
 import cloudpickle
 
 
 class FilesystemStore(KeyValueStore):
     """
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/firestore.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/firestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import typing
-
-from spoonbill.datastores import KeyValueStore, VALUE, KEY
+from spoonbill.datastores.base import KeyValueStore, VALUE
 from google.cloud import firestore
 import re
 
 
 class Firestore(KeyValueStore):
     """
     Google cloud firestore key-value store
@@ -55,15 +53,16 @@
         ref.set(self._to_item(value))
 
     def _delete_item(self, key: str):
         self.collection.document(self.encode_key(key)).delete()
 
     def __len__(self):
         i = -1
-        for i, value in enumerate(self.collection.stream()): pass
+        for i, value in enumerate(self.collection.stream()):
+            pass
         return i + 1
 
     def __getitem__(self, item):
         ret = self._get_item(item)
         if ret is None:
             raise KeyError(item)
         return ret
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/inmemory.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/inmemory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import json
-import pathlib
-import re
-from typing import Sequence
-
-import cloudpickle
-from spoonbill.datastores import KeyValueStore, KEY, VALUE
+from spoonbill.datastores.base import KeyValueStore
 
 
 class InMemoryStore(KeyValueStore):
     """
     A simple dictionary implementation.
     Pros: fast, cheap.
     Cons: Not persistent.
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/leveldb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/leveldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from spoonbill.datastores import KeyValueStore, KEY, VALUE
+from spoonbill.datastores.base import KeyValueStore, KEY, VALUE
 from typing import List
 import plyvel
 
 
 class LevelDBStore(KeyValueStore):
 
     NONE = '__NONE__'
@@ -88,15 +88,16 @@
         return self._size
 
     def __del__(self):
         self._store.close()
 
     @classmethod
     def load(cls, path, ssts: List[str], **kwargs):
-        raise NotImplementedError('load() is not implemented for SpeedbStore - try using ingest() instead')
+        raise NotImplementedError(
+            'load() is not implemented for SpeedbStore - try using ingest() instead')
 
     def ingest(self, path: str):
         self._store.ingest_external_file([path])
         self._size = self._count_all()
 
     def items(self, conditions: dict = None, limit: int = None):
         if conditions is not None and not hasattr(conditions, 'items'):
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/lmdb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/lmdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import contextlib
-
 import lmdbm
 import cloudpickle
 from lmdbm.lmdbm import remove_lmdbm
-from spoonbill.datastores import ContextStore
+from spoonbill.datastores.base import ContextStore
 from spoonbill.filesystem import FileSystem
 
 
 class CloudpickleEncoder(lmdbm.Lmdb):
     @staticmethod
     def encode(value):
         return cloudpickle.dumps(value)
@@ -43,15 +41,16 @@
     manager = CloudpickleEncoder
 
     def __init__(self, path: str, flag: str = "c", mode: int = 0o755, map_size: int = 2 ** 20, autogrow: bool = True,
                  strict=True):
         self.store_path = path
         self.strict = strict
         self.as_string = False
-        self.open_params = {"flag": flag, "mode": mode, "map_size": map_size, "autogrow": autogrow}
+        self.open_params = {"flag": flag, "mode": mode,
+                            "map_size": map_size, "autogrow": autogrow}
 
     @property
     def context(self):
         return CloudpickleEncoder.open(self.store_path, **self.open_params)
 
     def _flush(self):
         count = len(self)
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/modal.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/modal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from spoonbill.datastores import KeyValueStore, VALUE, KEY
+from spoonbill.datastores.base import KeyValueStore, VALUE, KEY
 import modal
 import re
 
 name_pattern = re.compile(r"[^a-zA-Z\d\s:]|[ ]")
 
 name_pattern.sub('_', "fdsaf asf _asfsa")
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/mongodb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from spoonbill.datastores import KeyValueStore, VALUE, KEY
+from spoonbill.datastores.base import KeyValueStore, VALUE, KEY
 import pymongo
 import bson
 
 ID = '_id'
 
 
 class MongoDBStore(KeyValueStore):
@@ -13,15 +13,16 @@
 
     def __init__(self, uri: str = None,
                  database: str = 'db',
                  collection: str = 'collection',
                  index=KEY,
                  strict=True):
 
-        self.client = pymongo.MongoClient(uri) if uri else pymongo.MongoClient()
+        self.client = pymongo.MongoClient(
+            uri) if uri else pymongo.MongoClient()
         self.database = self.client[database]
         self.collection = None
         self.strict = strict
         self.as_string = False
         self.index = index
         self._create_collections(collection)
 
@@ -48,15 +49,16 @@
         return item
 
     def _to_key_value(self, item):
         if item is None:
             return None
         key = self.decode_key(item.pop(self.index))
         _ = item.pop(ID, None)
-        value = item.get(VALUE) if isinstance(item, dict) and VALUE in item else item
+        value = item.get(VALUE) if isinstance(
+            item, dict) and VALUE in item else item
         value = self.decode_value(value)
         return key, value
 
     def _put_item(self, key, value):
         self.collection.insert_one(self._to_item(key, value))
 
     def _get_item(self, key):
@@ -122,15 +124,16 @@
 
     def items(self, conditions: dict = None, limit: int = None):
         for item in self._iter(conditions=conditions, limit=limit):
             key, value = self._to_key_value(item)
             yield key, value
 
     def values(self, keys: dict = None, limit: int = None):
-        params = {ID: {'$in': [self.encode_key(key) for key in keys]}} if keys else {}
+        params = {ID: {'$in': [self.encode_key(key) for key in keys]}} if keys else {
+        }
         for item in self.collection.find(params):
             key, value = self._to_key_value(item)
             yield value
 
     def update(self, d):
         operations = []
         for key, value in d.items():
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/pysos.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/pysos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
-import cloudpickle
 import pysos
 
-from spoonbill.datastores import KeyValueStore
+from spoonbill.datastores.base import KeyValueStore
 
 
 class PysosStore(KeyValueStore):
     """
     pySOS: Simple Objects Storage
 
     This is ideal for lists or datastores which either need persistence, are too big to fit in memory or both.
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/rdict.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/rdict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from spoonbill.datastores import KeyValueStore
+from spoonbill.datastores.base import KeyValueStore
 
 from typing import List
 
 
 class RdictBase(KeyValueStore):
     """
     A key-value store based on [speedict](https://github.com/speedb-io/speedb)
@@ -54,12 +54,13 @@
         return self._size
 
     def __del__(self):
         self._store.close()
 
     @classmethod
     def load(cls, path, ssts: List[str], **kwargs):
-        raise NotImplementedError('load() is not implemented for SpeedbStore - try using ingest() instead')
+        raise NotImplementedError(
+            'load() is not implemented for SpeedbStore - try using ingest() instead')
 
     def ingest(self, path: str):
         self._store.ingest_external_file([path])
         self._size = self._count_all()
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/redis.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import typing
 
 import redis
 
-from spoonbill.datastores import KeyValueStore, Strict
+from spoonbill.datastores.base import KeyValueStore, Strict
 
 REDIS_DEFAULT_HOST = 'localhost'
 REDIS_DEFAULT_PORT = 6379
 REDIS_DEFAULT_DB = 1
 
 
 class RedisStore(KeyValueStore, Strict):
@@ -71,18 +71,14 @@
 
     def get(self, key, default=None):
         return self.decode_value(self._store.get(self.encode_key(key))) or default
 
     def set(self, key, value):
         return self._store.set(self.encode_key(key), self.encode_value(value))
 
-
-
-
-
     def update(self, d):
         pipeline = self._store.pipeline()
         for key, value in d.items():
             pipeline.set(self.encode_key(key), self.encode_value(value))
         pipeline.execute()
         return True
 
@@ -150,15 +146,16 @@
         return RedisStore(store=redis.Redis.from_url(url, **kwargs), strict=strict)
 
     @classmethod
     def from_connection(cls, host: str = REDIS_DEFAULT_HOST, port: int = REDIS_DEFAULT_PORT,
                         db: int = None, strict: bool = False, **kwargs):
 
         if db is None:
-            store = redis.Redis(host=host, port=port, db=0, decode_responses=True)
+            store = redis.Redis(host=host, port=port, db=0,
+                                decode_responses=True)
             db = len(RedisStore._databases_names(store))  # TODO test this
         kwargs['decode_responses'] = kwargs.get('decode_responses', True)
         return RedisStore(store=redis.Redis(host=host, port=port, db=db, **kwargs), strict=strict)
 
     @property
     def _backup_path(self):
         return self._get_path(self._store.config_get('dir')['dir']).joinpath(
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/rocksdb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/rocksdb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/safetensors.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/safetensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 
-from spoonbill.datastores import ContextStore, InMemoryStore, VALUE
+from spoonbill.datastores.base import ContextStore, VALUE
+from spoonbill.datastores.inmemory import InMemoryStore
 
 
 def get_framework_save_file(framework):
     if framework == SafetensorsStore.TORCH:
         from safetensors.torch import save_file
     elif framework == SafetensorsStore.TENSORFLOW:
         from safetensors.tensorflow import save_file
@@ -138,15 +139,16 @@
         raise NotImplementedError("SafetensorsStore does not support pop")
 
     def get_slice(self, key, slice):
         with self.context as store:
             return store.get_slice(key)[slice]
 
     def save(self, path):
-        self._get_path(path).write_bytes(self._get_path(self.store_path).read_bytes())
+        self._get_path(path).write_bytes(
+            self._get_path(self.store_path).read_bytes())
 
     def load(self, path):
         self.store_path = path
 
 
 class SafetensorsInMemoryStore(InMemoryStore):
 
@@ -175,26 +177,26 @@
 
     def export_safetensors(self, path: str):
         return SafetensorsStore.from_dict({key: value for key, value in self.items()}, path, self.framework,
                                           self.device)
 
 
 with contextlib.suppress(ImportError):
-    from spoonbill.datastores import LmdbStore
-
+    from spoonbill.datastores.lmdb import LmdbStore
 
     class SafetensorsLmdbStore(LmdbStore):
 
         def __init__(self, path: str, flag: str = "c", mode: int = 0o755, map_size: int = 2 ** 20,
                      autogrow: bool = True,
                      framework='pt', device='cpu'):
             self.store_path = path
             self.strict = False
             self.as_string = True
-            self.open_params = {"flag": flag, "mode": mode, "map_size": map_size, "autogrow": autogrow}
+            self.open_params = {"flag": flag, "mode": mode,
+                                "map_size": map_size, "autogrow": autogrow}
             self.framework = framework
             self.device = device
 
         def encode_key(self, key):
             return str(key)
 
         def encode_value(self, value):
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/shelve.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/shelve.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 import os
 
 import shelve
-from spoonbill.datastores import ContextStore, Strict
+from spoonbill.datastores.base import ContextStore, Strict
 
 
 class ShelveStore(ContextStore, Strict):
     """
     A shelve key-value store based on [shelve](https://docs.python.org/3/library/shelve.html).
     """
     manager = shelve
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/speedb.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/speedb.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/datastores/unqlite.py` & `spoonbill_framework-0.1.0/spoonbill/datastores/unqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import contextlib
 import json
-import pickle
-import struct
-
 import cloudpickle
 
-from spoonbill.datastores import KeyValueStore, KEY, VALUE
+from spoonbill.datastores.base import KeyValueStore
 from unqlite import UnQLite
 
 
 class UnQLiteStore(KeyValueStore):
     """
     A simple dictionary implementation.
     Pros: fast, cheap.
@@ -92,9 +89,8 @@
             if self._is_encoded(value):
                 value = eval(value)
                 value = cloudpickle.loads(value)
                 return value
             return value
 
     def _is_encoded(self, value):
-        return  str(value)[:3] in ('b"\\', "b'\\", 'b"b', "b'b", 'b"b', "b'b")
-
+        return str(value)[:3] in ('b"\\', "b'\\", 'b"b', "b'b", 'b"b', "b'b")
```

### Comparing `spoonbill_framework-0.0.1a7/spoonbill/filesystem.py` & `spoonbill_framework-0.1.0/spoonbill/filesystem.py`

 * *Files identical despite different names*

### Comparing `spoonbill_framework-0.0.1a7/PKG-INFO` & `spoonbill_framework-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spoonbill-framework
-Version: 0.0.1a7
+Version: 0.1.0
 Summary: A lightweight, universal interface for Key-Values data stores
 License: LICENSE
 Keywords: dict,key-value,gcp,azure,aws,s3,lmdb,pysos,redis,dynamodb,mongodb,cosmosdb,safetensors,unqlite
 Author: xdssio
 Author-email: jonathan@xdss.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: dev
 Provides-Extra: gcp
+Provides-Extra: json
 Provides-Extra: lmdbm
 Provides-Extra: modal
 Provides-Extra: mongodb
 Provides-Extra: pysos
 Provides-Extra: redis
 Provides-Extra: rocksdb
 Provides-Extra: safetensors
@@ -213,28 +214,49 @@
 # Also works with any dict-like object
 from collections import defaultdict, OrderedDict, Counter
 
 store = InMemoryStore(defaultdict)
 store = InMemoryStore(OrderedDict)
 store = InMemoryStore(Counter)
 ```
+## JsonStore
+
+A simple json-file store where each call read and write a json file.   
+Not very effeicint for many calls but great for a small configuration singelton file.   
+Biggest benefit is that the file which is written is human-readable.
+
+* `lockfile_path` can be used as a locking mechanism. Requires `pip install filelock`.
+* `use_jsonpickle` can be use instead of pure json to handle more complicated objects like numpy arrays. Requires `pip install jsonpickle`
+* Cloud-native, if the path is `s3,gs,az`, it should still work.   
+  
+> ⚠️ The cloud native is un-tested.
+
+```python
+from spoonbill.datastores.jsonstore import JsonStore
+
+store = JsonStore.open(path='file.json', 
+                      strict=True, 
+                      lockfile_path=tmpdir.name+'file.lock',
+                      use_jsonpickle=True)
+```
+
 
 ## [LmdbStore](https://github.com/Dobatymo/lmdb-python-dbm)
 
 An LMDB key-value store based on [lmdb-python-dbm](https://github.com/Dobatymo/lmdb-python-dbm). This is ideal for lists
 or datastores which either need persistence, are too big to fit in memory or both.   
 This is a Python DBM interface style wrapper around [LMDB](http://www.lmdb.tech/doc/) (Lightning Memory-Mapped Database)
 
 [Details](https://en.wikipedia.org/wiki/Lightning_Memory-Mapped_Database)
 
 Requirements:   
 ```pip install lmdbm```
 
 ```python
-from spoonbill.datastores import LmdbStore
+from spoonbill.datastores.lmdb import LmdbStore
 
 store = LmdbStore.open('tmp.db')
 ```
 
 ## [PysosStore](https://github.com/dagnelies/pysos)
 
 This is ideal for lists or dictionaries which either need persistence, are too big to fit in memory or both.
@@ -250,27 +272,27 @@
 * it is platform independent, unlike shelve which relies on an underlying dbm implementation, which may vary from system
   to system the data is stored in a plain text format
 
 Requirements:   
 ```pip install pysos```
 
 ```python
-from spoonbill.datastores import PysosStore
+from spoonbill.datastores.pysos import PysosStore
 
 store = PysosStore.open('tmp.db')
 ```
 
 ## [Shelve](https://docs.python.org/3/library/shelve.html)
 
 The difference with “dbm” databases is that the values (not the keys!) in a shelf can be essentially arbitrary Python
 objects — anything that the pickle module can handle. This includes most class instances, recursive data types, and
 objects containing lots of shared sub-objects. The keys are ordinary strings.
 
 ```python
-from spoonbill.datastores import ShelveStore
+from spoonbill.datastores.shelve import ShelveStore
 
 store = ShelveStore.open('tmp.db')
 ```
 
 ## [Safetensors](https://github.com/huggingface/safetensors)
 
 This is ideal whe you want to work with tensors from disc, but it is a frozen store - no set or update.
@@ -327,15 +349,15 @@
 * It supports caching
 * It can be exported to a local directory or other clouds (s3, gs, az, etc)
 
 For faster applications with cloud persistence, you can use InMemoryStore/LmdbStore and save/load to the cloud after
 updates.
 
 ```python
-from spoonbill.datastores import FilesystemStore
+from spoonbill.datastores.filesystem import FilesystemStore
 
 # set strict to True to use redis with its default behaviour which turns keys and values to strings
 store = FilesystemStore.open("s3://bucket/path/to/store")
 store.save("local_dir_path")
 ```
 
 ## [Redis](https://github.com/redis/redis-py)
@@ -347,15 +369,15 @@
   expect from redis.
 * Redis doesn't have any search for values.
 
 Requirements:   
 ```pip install redis```
 
 ```python
-from spoonbill.datastores import RedisStore
+from spoonbill.datastores.redis import RedisStore
 
 # set strict to True to use redis with its default behaviour which turns keys and values to strings
 store = RedisStore.open("redis://localhost:6379/1")
 store[1] = 1
 assert store[1] == store["1"] == "1"
 
 assert list(store.keys('1*')) == ['111', '1', '11']  # redis turn every key to string
@@ -373,15 +395,15 @@
     * Bad Example: `store['key'] = "a value which is not a dict"`
 
 Recommended using with `strict=True` to enjoy all the benefits of backends including **searches**.
 
 Searches API Example:
 
 ```python
-from spoonbill.datastores import MongoDBStore
+from spoonbill.datastores.mongodb import MongoDBStore
 
 store = MongoDBStore()
 store.keys(pattern="*", limit=10)  # scan keys to a pattern
 store.values(keys=['key1', 'key2'])  # retrieve a batch of values efficiently 
 store.items(conditions={'a': '1+', 'b': 1}, limit=10)  # filter based on match conditions
 ```
 
@@ -389,15 +411,15 @@
 
 * Save/load is only implemented for `strict=True`.
 
 Requirements:
 ```pip install pymongo```
 
 ```python
-from spoonbill.datastores import MongoDBStore
+from spoonbill.datastores.dynamodb import DynamoDBStore
 
 store = MongoDBStore.open(uri='mongodb://localhost:27017/')
 ```
 
 ## [DynamoDB]((https://aws.amazon.com/dynamodb/))
 
 Notes:
@@ -431,15 +453,15 @@
 7. Install google-cloud-firestore with
 
 ```bash
 pip install --upgrade google-cloud-firestore 
 ```
 
 ```python
-from spoonbill.datastores import Firestore
+from spoonbill.datastores.firestore import Firestore
 
 # this rest of the credentials are picked up from the file in the GOOGLE_APPLICATION_CREDENTIALS environment variable
 store = Firestore.open(table_name="my-collection")
 ```
 
 ## [Azure CosmosDB]((https://www.google.com/search?client=safari&rls=en&q=Azure+Cosmos&ie=UTF-8&oe=UTF-8))
 
@@ -453,15 +475,15 @@
 Prerequisites: [Quickstart](https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/quickstart-python?tabs=azure-portal%2Clinux)
 
 Requirements:
 
 ```pip install azure-cosmos```
 
 ```python
-from spoonbill.datastores import CosmosDBStore
+from spoonbill.datastores.cosmos import CosmosDBStore
 
 store = CosmosDBStore.open(database='db',
                            container='container',
                            endpoint='endpoint',
                            credential='credential')
 ```
 
@@ -490,15 +512,15 @@
 
 Within the runtime, the **context app** is passed to the store to be able to update the data.
 
 Within a function, only the **name** of the dict is needed.
 
 ```python 
 import modal
-from spoonbill.datastores import ModalStore
+from spoonbill.datastores.modal import ModalStore
 
 image = modal.Image.debian_slim().pip_install("spoonbill-framework")
 
 name = "data"
 stub = modal.Stub("app name", **kwargs)
 # with stub
 store = ModalStore.open(name=name, stub=stub, data={"key": "value"})  # data is optional
@@ -525,15 +547,15 @@
 UnQLite is a in-process software library which implements a self-contained, serverless, zero-configuration,
 transactional NoSQL database engine.
 
 Requirements:   
 ```pip install unqlite```
 
 ```python
-from spoonbill.datastores import UnQLiteStore
+from spoonbill.datastores.unqlite import UnQLiteStore
 
 store = UnQLiteStore.open('tmp.db')  # leave empty for in-memory
 ```
 
 ## [Speedb](https://github.com/speedb-io/speedb)
 
 A first-of-its-kind, community-led key-value storage engine, designed to support modern data sets.
@@ -546,15 +568,15 @@
   use [RocksDict](https://github.com/Congyuwang/RocksDict) directly.
 * The save and load is a bit different from the other stores. It is not a dump and load of the data, save to a file and
   ingest back.
 * Requirements:   
   ```pip install speedict```
 
 ```python
-from spoonbill.datastores import SpeedbStore
+from spoonbill.datastores.speedb import SpeedbStore
 
 store = SpeedbStore.open('directory/')
 
 store.save('file.sst')
 # load 
 store.ingest('file.sst')
 
@@ -576,15 +598,15 @@
 * The save and load is a bit different from the other stores. It is not a dump and load of the data, save to a file and
   ingest back.
 
 * Requirements:   
   ```pip install rocksdict```
 
 ```python
-from spoonbill.datastores import RocksDBStore
+from spoonbill.datastores.rocksdb import RocksDBStore
 
 store = RocksDBStore.open('directory/')
 
 store.save('file.sst')
 # load 
 store.ingest('file.sst')
 
@@ -607,14 +629,14 @@
 ```
 pip install plyvel
 # or 
 pip install plyvel-ci
 ```
 
 ```python
-from spoonbill.datastores import LevelDBStore
+from spoonbill.datastores.leveldb import LevelDBStore
 
 store = LevelDBStore.open('directory/')
 
 ```
```

