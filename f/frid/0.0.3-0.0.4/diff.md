# Comparing `tmp/frid-0.0.3.tar.gz` & `tmp/frid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.3.tar", last modified: Tue Apr  2 02:20:18 2024, max compression
+gzip compressed data, was "frid-0.0.4.tar", last modified: Thu Apr  4 22:01:05 2024, max compression
```

## Comparing `frid-0.0.3.tar` & `frid-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.3/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-02 02:20:18.445206 frid-0.0.3/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.3/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      347 2024-04-02 02:16:36.000000 frid-0.0.3/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    23981 2024-03-29 23:28:02.000000 frid-0.0.3/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.3/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    12841 2024-03-29 23:28:02.000000 frid-0.0.3/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-03-29 23:28:02.000000 frid-0.0.3/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     6504 2024-04-01 22:27:27.000000 frid-0.0.3/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     4061 2024-03-29 23:28:02.000000 frid-0.0.3/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    21302 2024-04-01 15:36:11.000000 frid-0.0.3/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.3/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.3/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2082 2024-04-01 15:53:05.000000 frid-0.0.3/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11113 2024-03-29 23:28:02.000000 frid-0.0.3/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-02 02:20:18.445206 frid-0.0.3/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      328 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-02 02:20:18.000000 frid-0.0.3/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-02 02:18:11.000000 frid-0.0.3/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-02 02:20:18.445206 frid-0.0.3/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.4/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-04 22:01:05.546019 frid-0.0.4/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.4/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      473 2024-04-04 14:54:45.000000 frid-0.0.4/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    23981 2024-03-29 23:28:02.000000 frid-0.0.4/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.4/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.4/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    12841 2024-03-29 23:28:02.000000 frid-0.0.4/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.4/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     7762 2024-04-03 22:34:38.000000 frid-0.0.4/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8503 2024-04-02 17:42:49.000000 frid-0.0.4/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    21302 2024-04-01 15:36:11.000000 frid-0.0.4/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.4/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.4/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2082 2024-04-01 15:53:05.000000 frid-0.0.4/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.4/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-04 21:56:55.000000 frid-0.0.4/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-04 22:01:05.546019 frid-0.0.4/setup.cfg
```

### Comparing `frid-0.0.3/LICENSE` & `frid-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/PKG-INFO` & `frid-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.3/README.md` & `frid-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/__main__.py` & `frid-0.0.4/frid/__main__.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/chrono.py` & `frid-0.0.4/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/dumper.py` & `frid-0.0.4/frid/dumper.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/errors.py` & `frid-0.0.4/frid/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
             self.trace = list(trace)
             self.with_traceback(None)
         else:
             raise ValueError(f"Invalid trace type {type(trace)}")
 
     @classmethod
     def frid_from(cls, name: str, *args, error: str, trace: Sequence[str]|None=None,
-                  cause: str|None=None, **kwas):
+                  cause: str|None=None, **kwds):
         # The `trace` and `cause` are not accepting TrackbackType and BaseException;
         # and `error` is passed as the first argument.
         assert name in cls.frid_keys()
-        return FridError(error, trace=trace, **kwas)
+        return FridError(error, trace=trace, **kwds)
 
     def frid_repr(self) -> dict[str,str|int|list[str]]:
         out: dict[str,str|int|list[str]] = {'error': str(self)}
         trace = []
         if self.trace is not None:
             trace.extend(self.trace)
             trace.append("")
```

### Comparing `frid-0.0.3/frid/guards.py` & `frid-0.0.4/frid/guards.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,15 @@
-from collections.abc import Iterable, Mapping, Sequence
-from typing import Literal, TypeGuard, TypeVar, overload
+from collections.abc import Callable, Iterable, Mapping, Sequence
+from typing import Any, Literal, TypeGuard, TypeVar, overload
 
-from .typing import BlobTypes, StrKeyMap
+from .typing import BlobTypes, DateTypes, FridArray, FridMixin, FridPrime, FridValue, StrKeyMap
 
 K = TypeVar('K')
 V = TypeVar('V')
 
-@overload
-def as_type(dtype: type[V], data, /, allow_none: Literal[False]=False) -> V: ...
-@overload
-def as_type(dtype: type[V], data, /, allow_none: Literal[True]) -> V|None: ...
-def as_type(dtype: type[V], data, /, allow_none: bool=False) -> V|None:
-    if data is None and allow_none:
-        return None
-    if not isinstance(data, dtype):
-        raise ValueError(f"Expecting type {dtype}, got {type(data).__name__}")
-    return data
-@overload
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
-                /, allow_none: Literal[False]=False) -> V: ...
-@overload
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
-                /, allow_none: Literal[True]) -> V|None: ...
-def get_as_type(dtype: type[V], map: StrKeyMap, key: str, /, allow_none: bool=False) -> V|None:
-    return as_type(dtype, map.get(key))
-
 def is_text_list_like(data, /) -> TypeGuard[Sequence[str]]:
     """Type guard for a sequence of string elements."""
     if not isinstance(data, Sequence) or isinstance(data, str|BlobTypes):
         return False
     return all(isinstance(x, str) for x in data)
 
 def is_blob_list_like(data, /) -> TypeGuard[Sequence[BlobTypes]]:
@@ -45,33 +26,47 @@
 def is_list_like(
         data, /, etype: type[V], *, allow_none: Literal[False]=False
 ) -> TypeGuard[Sequence[V]]: ...
 @overload
 def is_list_like(
         data, /, etype: type[V], *, allow_none: Literal[True]
 ) -> TypeGuard[Sequence[V|None]]: ...
+@overload
+def is_list_like(
+        data, /, etype: Callable[[Any],TypeGuard[V]], *, allow_none: Literal[False]=False
+) -> TypeGuard[Sequence[V]]: ...
+@overload
 def is_list_like(
-        data, /, etype: type|None=None, *, allow_none: bool=False
+        data, /, etype: Callable[[Any],TypeGuard[V]], *, allow_none: Literal[True]
+) -> TypeGuard[Sequence[V|None]]: ...
+def is_list_like(
+        data, /, etype: Callable[[Any],bool]|type|None=None, *, allow_none: bool=False
 ) -> TypeGuard[Sequence]:
     """Type guard for a sequence type.
     Arguments:
     - `data`: the input data to be type-checked.
     - `etype`: the type for individual elements (default: any).
     - `allow_none`: if set to true, the element values is allowed to be None
       in addition to the given `etype`.
     """
     if not isinstance(data, Sequence):
         return False
     if isinstance(data, str|BlobTypes):
         return False
     if etype is None:
         return True
-    if not allow_none:
-        return all(isinstance(x, etype) for x in data)
-    return all(isinstance(x, etype) or x is None for x in data)
+    if isinstance(etype, type):
+        if not allow_none:
+            return all(isinstance(x, etype) for x in data)
+        return all(isinstance(x, etype) or x is None for x in data)
+    if callable(etype):
+        if not allow_none:
+            return all(etype(x) for x in data)
+        return all(etype(x) or x is None for x in data)
+    raise ValueError(f"Invalid etype specification: {etype}")
 
 @overload
 def is_dict_like(
         data, vtypes: None=None, /, *, allow_none=False
 ) -> TypeGuard[Mapping]: ...
 @overload
 def is_dict_like(
@@ -99,14 +94,33 @@
     if vtypes is None:
         return True
     if not allow_none:
         return all(isinstance(x, ktypes) for x in data.values())
     return all(isinstance(x, vtypes) or x is None for x in data.values())
 
 
+@overload
+def as_type(dtype: type[V], data, /, allow_none: Literal[False]=False) -> V: ...
+@overload
+def as_type(dtype: type[V], data, /, allow_none: Literal[True]) -> V|None: ...
+def as_type(dtype: type[V], data, /, allow_none: bool=False) -> V|None:
+    if data is None and allow_none:
+        return None
+    if not isinstance(data, dtype):
+        raise ValueError(f"Expecting type {dtype}, got {type(data).__name__}")
+    return data
+@overload
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
+                /, allow_none: Literal[False]=False) -> V: ...
+@overload
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
+                /, allow_none: Literal[True]) -> V|None: ...
+def get_as_type(dtype: type[V], map: StrKeyMap, key: str, /, allow_none: bool=False) -> V|None:
+    return as_type(dtype, map.get(key))
+
 def as_key_value_pair(
         data: Sequence[tuple[K,V]]|Mapping[K,V]|Iterable
 ) -> Sequence[tuple[K,V]]:
     """Converts the `data` to a sequence of key value pairs.
     - If the `data` is a map, convert it to a list of pairs.
     - If the `data` is already a sequence, return it as is.
     - If the `data` is an iterable but not a sequence, convert it to a list.
@@ -117,14 +131,27 @@
         return list(data.items())
     if isinstance(data, Sequence):
         return data
     if isinstance(data, Iterable):
         return list(data)
     raise ValueError(f"The input is not an iterable: {type(data)}")
 
+
+def is_frid_prime(data) -> TypeGuard[FridPrime]:
+    return data is None or isinstance(data, str|BlobTypes|DateTypes|int|float|bool)
+def is_frid_array(data) -> TypeGuard[FridArray]:
+    return isinstance(data, Sequence) and all(is_frid_value(x) for x in data)
+def is_frid_skmap(data) -> TypeGuard[StrKeyMap]:
+    return isinstance(data, Mapping) and all(
+        isinstance(k, str) and is_frid_value(v) for k, v in data.items()
+    )
+def is_frid_value(data) -> TypeGuard[FridValue]:
+    return (is_frid_prime(data) or is_frid_array(data) or is_frid_skmap(data)
+            or isinstance(data, FridMixin))
+
 def is_identifier_head(c: str) -> bool:
     """Returns if `c` can be first character of an indentifier."""
     return c.isalpha() or c in "_"
 
 def is_identifier_char(c: str) -> bool:
     """Returns if `c` can be middle character of an indentifier."""
     return c.isalnum() or c in "_.+-"
```

### Comparing `frid-0.0.3/frid/loader.py` & `frid-0.0.4/frid/loader.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/pretty.py` & `frid-0.0.4/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/strops.py` & `frid-0.0.4/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/typing.py` & `frid-0.0.4/frid/typing.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.3/frid/webapp.py` & `frid-0.0.4/frid/webapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os, json
-from collections.abc import AsyncIterator, Iterable, Mapping
-from typing import Literal
+from collections.abc import AsyncIterable, Iterable, Mapping
+from typing import Any, Literal
 from urllib.parse import unquote
 
 from .typing import BlobTypes, FridValue
 from .errors import FridError
+from .helper import get_type_name
+from .guards import is_frid_value
 from .loader import load_from_str
 from .dumper import dump_into_str
 
 
 DEF_ESCAPE_SEQ = os.getenv('FRID_ESCAPE_SEQ', "#!")
 FRID_MIME_TYPE = "text/vnd.askherefirst.frid"
 
@@ -48,14 +50,15 @@
         qsargs.append((key, value))
         try:
             kwargs[key] = load_from_str(value)
         except Exception:
             kwargs[key] = value
     return (qsargs, kwargs)
 
+
 class HttpMixin:
     """The generic mixin class that stores additional HTTP data.
 
     It can also be constructed standalone to hold data for either an HTTP
     request or an HTTP response. Constructor arguments (all optional/keyword):
     - `ht_status`: the HTTP status code; default to 0.
     - `http_head`: the headers as str-to-str map.
@@ -63,19 +66,19 @@
       strings in the case of streamming (need unicode strings not binary).
     - `mime_type`: the mime_type with one of the following shortcuts:
       `text`, `blob`, `html`, `json`, `frid`.
     - `http_data`: the data as supported by Frid.
     """
     def __init__(self, /, *args, ht_status: int=0, http_head: Mapping[str,str]|None=None,
                  http_body: BlobTypes|None=None, mime_type: str|ShortMimeType|None=None,
-                 http_data: FridValue|AsyncIterator[FridValue]=None, **kwargs):
+                 http_data: FridValue|AsyncIterable[FridValue|Any]=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.ht_status: int = ht_status
-        self.http_body: BlobTypes|AsyncIterator[BlobTypes]|None = http_body
-        self.http_data: FridValue|AsyncIterator[FridValue]|None = http_data
+        self.http_body: BlobTypes|AsyncIterable[BlobTypes]|None = http_body
+        self.http_data: FridValue|AsyncIterable[FridValue|Any]|None = http_data
         self.mime_type: str|ShortMimeType|None = mime_type
         self.http_head: dict[str,str] = dict(http_head) if http_head is not None else {}
 
     @classmethod
     def from_request(cls, rawdata: bytes|None, headers: InputHttpHead,
                      *args, **kwargs) -> 'HttpMixin':
         """Processing the HTTP request headers and data and create an object.
@@ -133,27 +136,36 @@
                 case 'application/x-www-form-urlencoded':
                     http_data = parse_http_query(rawdata.decode(encoding))
                     mime_type = 'form'
                 case 'application/json' | 'text/json':
                     http_data = json.loads(rawdata.decode(encoding))
                     mime_type = 'json'
                 case _:
-                    if mime_type == FRID_MIME_TYPE:
+                    if not mime_type:  # If not specified try to parse as json
+                        try:
+                            http_data = json.loads(rawdata.decode(encoding))
+                            mime_type = 'json'
+                        except Exception:
+                            pass
+                    elif mime_type == FRID_MIME_TYPE:
                         http_data = load_from_str(rawdata.decode(encoding))
                         mime_type = 'frid'
         return cls(*args, http_head=http_head, mime_type=mime_type, http_body=rawdata,
                    http_data=http_data, **kwargs)
 
     @staticmethod
-    async def _streaming(stream: AsyncIterator[FridValue]):
+    async def _streaming(stream: AsyncIterable[FridValue|Any]):
         """This is an agent iterator that convert data to string."""
         async for item in stream:
-            yield ("data: " + dump_into_str(
-                item, json_level=5, escape_seq=DEF_ESCAPE_SEQ
-            ) + "\n\n").encode()
+            if is_frid_value(item):
+                yield b"data: " + dump_into_str(
+                    item, json_level=5, escape_seq=DEF_ESCAPE_SEQ
+                ).encode() + b"\n\n"
+            else:
+                yield b"event: other\ndata: " + get_type_name(item).encode() + b"\n\n"
 
     def set_response(self) -> 'HttpMixin':
         """Update other HTTP fields according to http_data.
         - Returns `self` for chaining, so one can just do
           `var = HttpMixin(...).set_response()`
         The following fields will be updated if not present:
         - `http_body`: the content of the body in binary dump `http_data`:
@@ -178,15 +190,15 @@
                 return self
             if isinstance(self.http_data, bytes):
                 body = self.http_data
                 mime_type = 'blob'
             elif isinstance(self.http_data, str):
                 body = self.http_data.encode()
                 mime_type = 'text'
-            elif isinstance(self.http_data, AsyncIterator):
+            elif isinstance(self.http_data, AsyncIterable):
                 body = self._streaming(self.http_data)
                 mime_type = "text/event-stream"
             elif self.mime_type == 'json':
                 body = json.dumps(self.http_data, json_level=1).encode()
                 mime_type = self.mime_type
             elif self.mime_type == 'frid':
                 body = dump_into_str(self.http_data).encode()
```

### Comparing `frid-0.0.3/frid.egg-info/PKG-INFO` & `frid-0.0.4/frid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.3/pyproject.toml` & `frid-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

