# Comparing `tmp/python_115-0.0.5.6.tar.gz` & `tmp/python_115-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.6.tar", max compression
+gzip compressed data, was "python_115-0.0.5.7.tar", max compression
```

## Comparing `python_115-0.0.5.6.tar` & `python_115-0.0.5.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.6/LICENSE
--rw-r--r--   0        0        0   258981 2024-04-03 08:35:00.590003 python_115-0.0.5.6/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.6/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.6/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.6/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.6/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.6/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.6/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.6/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.6/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.6/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.6/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.6/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.6/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.6/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.6/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.6/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.6/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.6/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.6/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.6/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.6/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-03 08:45:21.643117 python_115-0.0.5.6/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.6/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.7/LICENSE
+-rw-r--r--   0        0        0   261107 2024-04-05 06:47:37.395609 python_115-0.0.5.7/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.7/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.7/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.7/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.7/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.7/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.7/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.7/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.7/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.7/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.7/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.7/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.7/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.7/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.7/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.7/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.7/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.7/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.7/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.7/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.7/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-05 06:48:24.210543 python_115-0.0.5.7/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.7/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.7/PKG-INFO
```

### Comparing `python_115-0.0.5.6/LICENSE` & `python_115-0.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/__init__.py` & `python_115-0.0.5.7/p115/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,31 @@
 from contextlib import asynccontextmanager
 from datetime import date, datetime
 from email.utils import formatdate
 from functools import cached_property, partial, update_wrapper
 from hashlib import md5, sha1, file_digest
 from hmac import digest as hmac_digest
 from inspect import isawaitable, iscoroutinefunction
-from io import BufferedReader, BytesIO, TextIOWrapper, UnsupportedOperation, DEFAULT_BUFFER_SIZE
+from io import (
+    BufferedReader, BytesIO, TextIOWrapper, UnsupportedOperation, DEFAULT_BUFFER_SIZE, 
+)
 from itertools import count
 from json import dumps, loads
 from mimetypes import guess_type
 from os import fsdecode, fspath, fstat, makedirs, scandir, stat, stat_result, PathLike
 from os import path as ospath
 from posixpath import join as joinpath, splitext
 from re import compile as re_compile, escape as re_escape
 from shutil import copyfileobj, SameFileError
 from stat import S_IFDIR, S_IFREG
 from threading import Condition, Thread
 from time import sleep, time
 from typing import (
-    cast, overload, Any, ClassVar, Final, Generic, IO, Literal, Optional, Never, Self, TypeAlias, 
-    TypedDict, TypeVar, Unpack, 
+    cast, overload, Any, ClassVar, Final, Generic, IO, Literal, Never, Optional, Self, 
+    TypeAlias, TypeVar, Unpack, 
 )
 from types import MappingProxyType
 from urllib.parse import parse_qsl, quote, urlencode, urlparse
 from uuid import uuid4
 from warnings import filterwarnings
 from xml.etree.ElementTree import fromstring
 
@@ -62,41 +64,44 @@
 # NOTE: OR use `pyqrcode` instead
 import qrcode # type: ignore
 
 from .exception import AuthenticationError, LoginError
 from .util.args import argcount
 from .util.cipher import P115RSACipher, P115ECDHCipher, MD5_SALT
 from .util.download import DownloadTask
-from .util.file import bio_chunk_iter, bio_skip_bytes, get_filesize, HTTPFileReader, RequestsFileReader, SupportsRead, SupportsWrite, SupportsGetUrl
+from .util.file import (
+    bio_chunk_iter, bio_skip_bytes, get_filesize, HTTPFileReader, 
+    RequestsFileReader, SupportsRead, SupportsWrite, SupportsGetUrl, 
+)
 from .util.iter import asyncify_iter
 from .util.path import basename, commonpath, dirname, escape, joins, normpath, splits, unescape
 from .util.property import funcproperty
 from .util.response import get_content_length, get_filename, is_range_request
 from .util.text import cookies_str_to_dict, posix_glob_translate_iter, to_base64
 from .util.urlopen import urlopen
 
 
 filterwarnings("ignore", category=DeprecationWarning)
 
-IDOrPathType: TypeAlias = int | str | PathLike[str] | Sequence[str]
-M = TypeVar("M", bound=Mapping)
-T = TypeVar("T", dict, Callable)
+AttrDict: TypeAlias = dict # TODO: TypedDict with extra keys
+IDOrPathType: TypeAlias = int | str | PathLike[str] | Sequence[str] | AttrDict
+RequestVarT = TypeVar("RequestVarT", dict, Callable)
 P115FSType = TypeVar("P115FSType", bound="P115FileSystemBase")
 P115PathType = TypeVar("P115PathType", bound="P115PathBase")
 
-CRE_SHARE_LINK = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?")
+CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
 APP_VERSION: Final = "99.99.99.99"
 RSA_ENCODER: Final = P115RSACipher()
 ECDH_ENCODER: Final = P115ECDHCipher()
 
 if not hasattr(Response, "__del__"):
     Response.__del__ = Response.close # type: ignore
 
 
-def check_response(fn: T, /) -> T:
+def check_response(fn: RequestVarT, /) -> RequestVarT:
     if isinstance(fn, dict):
         resp = fn
         if not resp.get("state", True):
             raise OSError(errno.EIO, resp)
         return fn
     elif iscoroutinefunction(fn):
         async def wrapper(*args, **kwds):
@@ -166,18 +171,14 @@
     if keep_raw:
         info2["raw"] = info
     if extra_data:
         info2.update(extra_data)
     return info2
 
 
-class HeadersKeyword(TypedDict):
-    headers: Optional[Mapping]
-
-
 class P115Client:
     cookie: str
     session: Session
     user_id: int
     user_key: str
 
     def __init__(self, /, cookie=None, login_app: str = "web"):
@@ -3739,31 +3740,33 @@
 
     def captcha_all(
         self, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> bytes:
-        """返回一张包含 10 个汉字的图片，包含验证码中 4 个汉字（有相应的编号，从 0 开始，从左到右，从上到下的顺序）
+        """返回一张包含 10 个汉字的图片，包含验证码中 4 个汉字（有相应的编号，从 0 到 9，计数按照从左到右，从上到下的顺序）
         GET https://captchaapi.115.com/?ct=index&ac=code&t=all
         """
         api = "https://captchaapi.115.com/?ct=index&ac=code&t=all"
         request_kwargs["parse"] = lambda _, content: content
         return self.request(api, async_=async_, **request_kwargs)
 
     def captcha_single(
         self, 
         id: int, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> bytes:
-        """10 个汉字单独的图片，编号从 0 到 9
+        """10 个汉字单独的图片，包含验证码中 4 个汉字，编号从 0 到 9
         GET https://captchaapi.115.com/?ct=index&ac=code&t=single&id={id}
         """
+        if not 0 <= id <= 9:
+            raise ValueError(f"expected integer between 0 and 9, got {id}")
         api = f"https://captchaapi.115.com/?ct=index&ac=code&t=single&id={id}"
         request_kwargs["parse"] = lambda _, content: content
         return self.request(api, async_=async_, **request_kwargs)
 
     def captcha_verify(
         self, 
         payload: int | str | dict, 
@@ -3931,49 +3934,37 @@
 
 
 # TODO: 使用 id 而不是 path
 class P115PathBase(Generic[P115FSType], Mapping, PathLike[str]):
     fs: P115FSType
     path: str
 
-    def __init__(
-        self, 
-        /, 
-        fs: P115FSType, 
-        path: str | PathLike[str], 
-        **attr, 
-    ):
-        attr.update(fs=fs, path=fs.abspath(path))
+    def __init__(self, /, attr: AttrDict):
         super().__setattr__("__dict__", attr)
 
     def __and__(self, path: str | PathLike[str], /) -> Self:
-        return type(self)(self.fs, commonpath((self.path, self.fs.abspath(path))))
+        return type(self)({"fs": self.fs, "path": commonpath((self.path, self.fs.abspath(path)))})
 
     def __call__(self, /) -> Self:
-        fs = self.fs
-        attr = fs.attr(self)
-        try:
-            if self.__dict__["path"] != attr["path"]:
-                raise KeyError
-            super().__setattr__("__dict__", {"fs": fs, **attr})
-        except KeyError:
+        attr = self.fs.attr(self)
+        if self.__dict__ is not attr:
             self.__dict__.update(attr)
         return self
 
     def __contains__(self, key, /) -> bool:
         return key in self.__dict__
 
     def __eq__(self, path, /) -> bool:
         return type(self) is type(path) and self.fs.client == path.fs.client and self.path == path.path
 
     def __fspath__(self, /) -> str:
         return self.path
 
     def __getitem__(self, key, /):
-        if key not in self.__dict__ and not self.__dict__.get("lastest_update"):
+        if key not in self.__dict__ and not self.__dict__.get("last_update"):
             self()
         return self.__dict__[key]
 
     def __ge__(self, path, /) -> bool:
         if type(self) is not type(path) or self.fs.client != path.fs.client:
             return False
         return commonpath((self.path, path.path)) == path.path
@@ -4004,25 +3995,29 @@
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
-        return f"<{name}({', '.join(f'{k}={v!r}' for k, v in self.__dict__.items())})>"
+        return f"{name}({self.__dict__})"
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     def __str__(self, /) -> str:
         return self.path
 
     def __truediv__(self, path: str | PathLike[str], /) -> Self:
         return self.joinpath(path)
 
+    @property
+    def is_attr_loaded(self, /) -> bool:
+        return "last_update" in self.__dict__
+
     @cached_property
     def id(self, /) -> int:
         return self.fs.get_id(self.path)
 
     def keys(self, /) -> KeysView:
         return self.__dict__.keys()
 
@@ -4132,24 +4127,24 @@
             onerror=onerror, 
             **kwargs, 
         )
 
     def join(self, *names: str) -> Self:
         if not names:
             return self
-        return type(self)(self.fs, joinpath(self.path, joins(names)))
+        return type(self)({"fs": self.fs, "path": joinpath(self.path, joins(names))})
 
     def joinpath(self, *paths: str | PathLike[str]) -> Self:
         if not paths:
             return self
         path = self.path
         path_new = normpath(joinpath(path, *paths))
         if path == path_new:
             return self
-        return type(self)(self.fs, path_new)
+        return type(self)({"fs": self.fs, "path": path_new})
 
     def listdir(self, /, **kwargs) -> list[str]:
         return self.fs.listdir(self, **kwargs)
 
     def listdir_attr(self, /, **kwargs) -> list[dict]:
         return self.fs.listdir_attr(self, **kwargs)
 
@@ -4207,28 +4202,28 @@
     @property
     def parent(self, /) -> Self:
         path = self.path
         if path == "/":
             return self
         parent = dirname(path)
         try:
-            return type(self)(self.fs, parent, id=self.__dict__["parent_id"])
-        except:
-            return type(self)(self.fs, parent)
+            return type(self)({"id": self.__dict__["parent_id"], "fs": self.fs, "path": parent})
+        except KeyError:
+            return type(self)({"fs": self.fs, "path": parent})
 
     @cached_property
     def parents(self, /) -> tuple[Self, ...]:
         path = self.path
         if path == "/":
             return ()
         parents: list[Self] = []
         cls, fs = type(self), self.fs
         parent = dirname(path)
         while path != parent:
-            parents.append(cls(fs, parent))
+            parents.append(cls({"fs": fs, "path": parent}))
             path, parent = parent, dirname(parent)
         return tuple(parents)
 
     @cached_property
     def parts(self, /) -> tuple[str, ...]:
         return ("/", *splits(self.path, do_unescape=False)[0][1:])
 
@@ -4304,15 +4299,15 @@
             self if self.is_dir() else self.parent, 
             ignore_case=ignore_case, 
             allow_escaped_slash=allow_escaped_slash, 
         )
 
     @cached_property
     def root(self, /) -> Self:
-        return type(self)(self.fs, "/", id=0)
+        return type(self)({"fs": self.fs, "path": "/", "id": 0})
 
     def samefile(self, path: str | PathLike[str], /) -> bool:
         if type(self) is type(path):
             return self == path
         return path in ("", ".") or self.path == self.fs.abspath(path)
 
     def stat(self, /) -> stat_result:
@@ -4383,15 +4378,15 @@
     def with_stem(self, stem: str, /) -> Self:
         return self.parent.joinpath(stem + self.suffix)
 
     def with_suffix(self, suffix: str, /) -> Self:
         return self.parent.joinpath(self.stem + suffix)
 
 
-class P115FileSystemBase(Generic[M, P115PathType]):
+class P115FileSystemBase(Generic[P115PathType]):
     client: P115Client
     cid: int
     path: str
     path_class: type[P115PathType]
 
     def __contains__(self, id_or_path: IDOrPathType, /) -> bool:
         return self.exists(id_or_path)
@@ -4419,15 +4414,15 @@
 
     @abstractmethod
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> M:
+    )  -> AttrDict:
         ...
 
     @abstractmethod
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
@@ -4438,60 +4433,68 @@
 
     @abstractmethod
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> Iterator[M]:
+    ) -> Iterator[AttrDict]:
         ...
 
     def abspath(self, path: str | PathLike[str] = "", /) -> str:
         return self.get_path(path, self.cid)
 
     def as_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-        fetch_attr: bool = False, 
     ) -> P115PathType:
         path_class = type(self).path_class
+        attr: AttrDict
         if isinstance(id_or_path, path_class):
-            path = id_or_path
-            if fetch_attr:
-                path()
-            return path
+            return id_or_path
+        elif isinstance(id_or_path, dict):
+            attr = cast(AttrDict, id_or_path)
         elif isinstance(id_or_path, int):
-            return path_class(self, **self.attr(id_or_path))
-        if fetch_attr:
-            return path_class(self, **self.attr(id_or_path, pid))
-        return path_class(self, self.get_path(id_or_path, pid))
+            attr = self.attr(id_or_path)
+        else:
+            attr = self.attr(id_or_path, pid)
+        attr["fs"] = self
+        return path_class(attr)
 
     def chdir(
         self, 
         id_or_path: IDOrPathType = 0, 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
-        if isinstance(id_or_path, type(self).path_class):
-            self.__dict__.update(cid=id_or_path.id, path=id_or_path.path)
-            return id_or_path.id
+        path_class = type(self).path_class
+        if isinstance(id_or_path, path_class):
+            cid = id_or_path.id
+            self.__dict__.update(
+                cid  = cid, 
+                path = id_or_path["path"], 
+            )
+            return cid
         elif id_or_path in (0, "/"):
             self.__dict__.update(cid=0, path="/")
             return 0
         if isinstance(id_or_path, PathLike):
             id_or_path = fspath(id_or_path)
         if not id_or_path or id_or_path == ".":
             return self.cid
         attr = self.attr(id_or_path, pid)
         if self.cid == attr["id"]:
             return self.cid
         elif attr["is_directory"]:
-            self.__dict__.update(cid=attr["id"], path=self.get_path(id_or_path, pid))
+            self.__dict__.update(
+                cid  = attr["id"], 
+                path = self.get_path(id_or_path, pid), 
+            )
             return attr["id"]
         else:
             raise NotADirectoryError(
                 errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
 
     def download(
         self, 
@@ -4539,22 +4542,25 @@
         predicate: Optional[Callable[[P115PathType], bool]] = None, 
         onerror: None | bool | Callable[[BaseException], Any] = None, 
     ) -> Iterator[DownloadTask]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
+        pathes: Iterable[P115PathType]
         if attr["is_directory"]:
             if not no_root:
                 local_dir = ospath.join(local_dir, attr["name"])
                 if local_dir:
                     makedirs(local_dir, exist_ok=True)
-            pathes = self.listdir_path(attr["id"])
+            pathes = self.scandir(attr["id"])
         else:
-            pathes = [type(self).path_class(self, **attr)]
+            path_class = type(self).path_class
+            attr["fs"] = self
+            pathes = (path_class(attr),)
         for subpath in filter(predicate, pathes):
             if subpath["is_directory"]:
                 yield from self.download_tree(
                     subpath["id"], 
                     ospath.join(local_dir, subpath["name"]), 
                     write_mode=write_mode, 
                     submit=submit, 
@@ -4583,16 +4589,17 @@
 
     def exists(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
+        path_class = type(self).path_class
         try:
-            if isinstance(id_or_path, type(self).path_class):
+            if isinstance(id_or_path, path_class):
                 id_or_path()
             else:
                 self.attr(id_or_path, pid)
             return True
         except FileNotFoundError:
             return False
 
@@ -4606,17 +4613,18 @@
 
     def get_id(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
+        path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return self.cid
-        elif isinstance(id_or_path, type(self).path_class):
+        elif isinstance(id_or_path, path_class):
             return id_or_path.id
         elif isinstance(id_or_path, int):
             return id_or_path
         if id_or_path == "/":
             return 0
         try:
             path_to_id = getattr(self, "path_to_id", None)
@@ -4629,18 +4637,21 @@
 
     def get_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> str:
+        path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return self.path
-        elif isinstance(id_or_path, type(self).path_class):
+        elif isinstance(id_or_path, path_class):
             return id_or_path.path
+        elif isinstance(id_or_path, dict):
+            return id_or_path["path"]
         elif isinstance(id_or_path, int):
             id = id_or_path
             if id == 0:
                 return "/"
             return self.attr(id)["path"]
         if isinstance(id_or_path, (str, PathLike)):
             path = fspath(id_or_path)
@@ -4661,18 +4672,21 @@
 
     def get_patht(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> list[str]:
+        path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return splits(self.path)[0]
-        elif isinstance(id_or_path, type(self).path_class):
+        elif isinstance(id_or_path, path_class):
             return splits(id_or_path.path)[0]
+        elif isinstance(id_or_path, dict):
+            return splits(id_or_path["path"])[0]
         elif isinstance(id_or_path, int):
             id = id_or_path
             if id == 0:
                 return [""]
             return splits(self.attr(id)["path"])[0]
         if pid is None:
             pid = self.cid
@@ -4712,17 +4726,20 @@
         path_class = type(self).path_class
         if not pattern:
             try:
                 attr = self.attr(dirname)
             except FileNotFoundError:
                 return iter(())
             else:
-                return iter((path_class(self, **attr),))
+                attr["fs"] = self
+                return iter((path_class(attr),))
         elif not pattern.lstrip("/"):
-            return iter((path_class(self, **self.attr(0)),))
+            attr = self.attr(0)
+            attr["fs"] = self
+            return iter((path_class(attr),))
         splitted_pats = tuple(posix_glob_translate_iter(
             pattern, allow_escaped_slash=allow_escaped_slash))
         dirname_as_id = isinstance(dirname, (int, path_class))
         dirid: int
         if isinstance(dirname, path_class):
             dirid = dirname.id
         elif isinstance(dirname, int):
@@ -4754,15 +4771,16 @@
                     if dirname_as_id:
                         attr = self.attr(dir2, dirid)
                     else:
                         attr = self.attr(dir_)
                 except FileNotFoundError:
                     return iter(())
                 else:
-                    return iter((path_class(self, **attr),))
+                    attr["fs"] = self
+                    return iter((path_class(attr),))
             elif typ == "dstar" and i + 1 == len(splitted_pats):
                 if dirname_as_id:
                     return self.iter(dir2, dirid, max_depth=-1)
                 else:
                     return self.iter(dir_, max_depth=-1)
             if any(typ == "dstar" for _, typ, _ in splitted_pats):
                 pattern = joinpath(re_escape(dir_), "/".join(t[0] for t in splitted_pats[i:]))
@@ -4807,47 +4825,53 @@
                             pat = "(?i:%s)" % pat
                         cref = cref_cache[i] = re_compile(pat).fullmatch
                     if cref(subpath["name"]):
                         if at_end:
                             yield subpath
                         elif subpath["is_directory"]:
                             yield from glob_step_match(subpath, j)
-        path = path_class(self, dir_)
         if dirname_as_id:
-            path.__dict__["id"] = self.get_id(dir2, dirid)
-        if not path["is_directory"]:
+            attr = self.attr(dir2, dirid)
+        else:
+            attr = self.attr(dir_)
+        if not attr["is_directory"]:
             return iter(())
+        attr["fs"] = self
+        path = path_class(attr)
         return glob_step_match(path, i)
 
     def isdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
-        if isinstance(id_or_path, type(self).path_class):
+        path_class = type(self).path_class
+        if isinstance(id_or_path, path_class):
             return id_or_path["is_directory"]
         try:
             return self.attr(id_or_path, pid)["is_directory"]
         except FileNotFoundError:
             return False
 
     def isfile(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
-        if isinstance(id_or_path, type(self).path_class):
+        path_class = type(self).path_class
+        if isinstance(id_or_path, path_class):
             return not id_or_path["is_directory"]
         try:
             return not self.attr(id_or_path, pid)["is_directory"]
         except FileNotFoundError:
             return False
 
+    # TODO: 支持宽度优先遍历
     def iter(
         self, 
         top: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
@@ -4860,27 +4884,27 @@
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         path_class = type(self).path_class
         try:
-            for path in self.listdir_path(top, pid, **kwargs):
-                path = cast(P115PathType, path)
+            for attr in self.iterdir(top, pid, **kwargs):
+                path = path_class(attr)
                 yield_me = min_depth <= 0
                 if yield_me and predicate:
                     pred = predicate(path)
                     if pred is None:
                         continue
                     yield_me = pred 
                 if yield_me and topdown:
                     yield path
                 if path["is_directory"]:
                     yield from self.iter(
-                        path.path, 
+                        path, 
                         topdown=topdown, 
                         min_depth=min_depth, 
                         max_depth=max_depth, 
                         predicate=predicate, 
                         onerror=onerror, 
                     )
                 if yield_me and not topdown:
@@ -4906,26 +4930,26 @@
 
     def listdir_attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         **kwargs, 
-    ) -> list[M]:
+    ) -> list[AttrDict]:
         return list(self.iterdir(id_or_path, pid, **kwargs))
 
     def listdir_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         **kwargs, 
     ) -> list[P115PathType]:
         path_class = type(self).path_class
-        return [path_class(self, **attr) for attr in self.iterdir(id_or_path, pid, **kwargs)]
+        return [path_class(attr) for attr in self.iterdir(id_or_path, pid, **kwargs)]
 
     def dictdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         full_path: bool = False, 
@@ -4938,26 +4962,26 @@
 
     def dictdir_attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         **kwargs, 
-    ) -> dict[int, M]:
+    ) -> dict[int, AttrDict]:
         return {attr["id"]: attr for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def dictdir_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         **kwargs, 
     ) -> dict[int, P115PathType]:
         path_class = type(self).path_class
-        return {attr["id"]: path_class(self, **attr) for attr in self.iterdir(id_or_path, pid, **kwargs)}
+        return {attr["id"]: path_class(attr) for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def open(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         mode: str = "r", 
         buffering: Optional[int] = None, 
@@ -5055,15 +5079,15 @@
     def scandir(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
-        return iter(self.listdir_path(id_or_path, pid, **kwargs))
+        return map(type(self).path_class, self.iterdir(id_or_path, pid, **kwargs))
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
@@ -5091,16 +5115,16 @@
             max_depth -= 1
         yield_me = min_depth <= 0
         try:
             if not _top:
                 _top = self.get_path(top, pid)
             dirs: list[str] = []
             files: list[str] = []
-            attrs: list[M] = []
-            for attr in self.listdir_attr(top, pid, **kwargs):
+            attrs: list[AttrDict] = []
+            for attr in self.iterdir(top, pid, **kwargs):
                 if attr["is_directory"]:
                     attrs.append(attr)
                     dirs.append(attr["name"])
                 else:
                     files.append(attr["name"])
             if yield_me and topdown:
                 yield _top, dirs, files
@@ -5136,21 +5160,22 @@
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         yield_me = min_depth <= 0
+        path_class = type(self).path_class
         try:
             if not _top:
                 _top = self.get_path(top, pid)
             dirs: list[P115PathType] = []
             files: list[P115PathType] = []
-            for path in self.listdir_path(top, pid, **kwargs):
-                (dirs if path["is_directory"] else files).append(path)
+            for attr in self.iterdir(top, pid, **kwargs):
+                (dirs if attr["is_directory"] else files).append(path_class(attr))
             if yield_me and topdown:
                 yield _top, dirs, files
             for path in dirs:
                 yield from self.walk_path(
                     path["id"], 
                     topdown=topdown, 
                     min_depth=min_depth, 
@@ -5188,66 +5213,66 @@
             dst_path, 
             pid=pid, 
             overwrite_or_ignore=overwrite_or_ignore, 
             recursive=True, 
         )
         if attr is None:
             return None
-        return type(self)(self.fs, **attr)
+        return type(self)(attr)
 
     def mkdir(self, /, exist_ok: bool = True) -> Self:
         self.__dict__.update(self.fs.makedirs(self, exist_ok=exist_ok))
         return self
 
     def move(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None, 
     ) -> Self:
         attr = self.fs.move(self, dst_path, pid)
         if attr is None:
             return self
-        return type(self)(self.fs, **attr)
+        return type(self)(attr)
 
     def remove(self, /, recursive: bool = True) -> dict:
         return self.fs.remove(self, recursive=recursive)
 
     def rename(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None, 
     ) -> Self:
         attr = self.fs.rename(self, dst_path, pid)
         if attr is None:
             return self
-        return type(self)(self.fs, **attr)
+        return type(self)(attr)
 
     def renames(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None, 
     ) -> Self:
         attr = self.fs.renames(self, dst_path, pid)
         if attr is None:
             return self
-        return type(self)(self.fs, **attr)
+        return type(self)(attr)
 
     def replace(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None, 
     ) -> Self:
         attr = self.fs.replace(self, dst_path, pid)
         if attr is None:
             return self
-        return type(self)(self.fs, **attr)
+        return type(self)(attr)
 
     def rmdir(self, /) -> dict:
         return self.fs.rmdir(self)
 
     def touch(self, /) -> Self:
         self.__dict__.update(self.fs.touch(self))
         return self
@@ -5276,40 +5301,40 @@
             encoding=encoding, 
             errors=errors, 
             newline=newline, 
         ))
         return self
 
 
-class P115FileSystem(P115FileSystemBase[dict, P115Path]):
-    id_to_children: Optional[MutableMapping[int, dict]]
+class P115FileSystem(P115FileSystemBase[P115Path]):
+    attr_cache: Optional[MutableMapping[int, dict]]
     path_to_id: Optional[MutableMapping[str, int]]
     get_version: Optional[Callable]
     path_class = P115Path
 
     def __init__(
         self, 
         /, 
         client: P115Client, 
-        id_to_children: Optional[MutableMapping[int, dict]] = None, 
+        attr_cache: Optional[MutableMapping[int, dict]] = None, 
         path_to_id: Optional[MutableMapping[str, int]] = None, 
         get_version: Optional[Callable] = lambda attr: attr.get("mtime", 0), 
     ):
-        if id_to_children is not None:
-            id_to_children = {}
+        if attr_cache is not None:
+            attr_cache = {}
         if type(path_to_id) is dict:
             path_to_id["/"] = 0
         elif path_to_id is not None:
             path_to_id = ChainMap(path_to_id, {"/": 0})
         self.__dict__.update(
             client = client, 
             cid = 0, 
             path = "/", 
             path_to_id = path_to_id, 
-            id_to_children = id_to_children, 
+            attr_cache = attr_cache, 
             get_version = get_version, 
         )
 
     def __delitem__(self, id_or_path: IDOrPathType, /):
         self.rmtree(id_or_path)
 
     def __len__(self, /) -> int:
@@ -5415,22 +5440,22 @@
         try:
             return self._attr(id)
         except FileNotFoundError:
             self._files(pid, 1)
             return self._attr(id)
 
     def _clear_cache(self, attr: dict, /):
-        id_to_children = self.id_to_children
-        if id_to_children is None:
+        attr_cache = self.attr_cache
+        if attr_cache is None:
             return
         id = attr["id"]
         pid = attr["parent_id"]
         if id:
             try:
-                id_to_children[pid]["children"].pop(id, None)
+                attr_cache[pid]["children"].pop(id, None)
             except:
                 pass
         if attr["is_directory"]:
             path_to_id = self.path_to_id
             if path_to_id is None:
                 pop_path = None
             else:
@@ -5441,16 +5466,16 @@
                         pass
             startswith = str.startswith
             dq = deque((id,))
             get, put = dq.popleft, dq.append
             while dq:
                 cid = get()
                 try:
-                    cache = id_to_children[cid]
-                    del id_to_children[cid]
+                    cache = attr_cache[cid]
+                    del attr_cache[cid]
                 except KeyError:
                     pass
                 else:
                     for subid, subattr in cache["children"].items():
                         if pop_path is not None:
                             pop_path(subattr["path"])
                         if subattr["is_directory"]:
@@ -5459,27 +5484,27 @@
                 dirname = attr["path"]
                 pop_path(dirname)
                 dirname += "/"
                 for k in tuple(k for k in path_to_id if startswith(k, dirname)):
                     pop_path(k)
 
     def _update_cache_path(self, attr: dict, new_attr: dict, /):
-        id_to_children = self.id_to_children
-        if id_to_children is None:
+        attr_cache = self.attr_cache
+        if attr_cache is None:
             return
         id = attr["id"]
         opid = attr["parent_id"]
         npid = new_attr["parent_id"]
         if id and opid != npid:
             try:
-                id_to_children[opid]["children"].pop(id, None)
+                attr_cache[opid]["children"].pop(id, None)
             except:
                 pass
             try:
-                id_to_children[npid]["children"][id] = new_attr
+                attr_cache[npid]["children"][id] = new_attr
             except:
                 pass
         if attr["is_directory"]:
             path_to_id = self.path_to_id
             if path_to_id is None:
                 pop_path = None
             else:
@@ -5499,16 +5524,16 @@
             new_path += "/"
             len_old_path = len(old_path)
             dq = deque((id,))
             get, put = dq.popleft, dq.append
             while dq:
                 cid = get()
                 try:
-                    cache = id_to_children[cid]
-                    del id_to_children[cid]
+                    cache = attr_cache[cid]
+                    del attr_cache[cid]
                 except KeyError:
                     pass
                 else:
                     for subid, subattr in cache["children"].items():
                         subpath = subattr["path"]
                         if startswith(subpath, old_path):
                             new_subpath = subattr["path"] = new_path + subpath[len_old_path:]
@@ -5524,49 +5549,62 @@
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         refresh: bool = False, 
-    ) -> Iterator[dict]:
+    ) -> Iterator[AttrDict]:
         path_to_id = self.path_to_id
-        id_to_children = self.id_to_children
+        attr_cache = self.attr_cache
         get_version = self.get_version
         version = None
-        if id_to_children is None and isinstance(id_or_path, int):
+        if attr_cache is None and isinstance(id_or_path, int):
             id = id_or_path
         else:
-            attr = self.attr(id_or_path, pid)
+            attr = None
+            if not refresh:
+                path_class = type(self).path_class
+                if isinstance(id_or_path, dict):
+                    attr = id_or_path
+                elif isinstance(id_or_path, path_class):
+                    if id_or_path.is_attr_loaded:
+                        id_or_path()
+                    attr = id_or_path.__dict__
+            if attr is None:
+                attr = self.attr(id_or_path, pid)
             if not attr["is_directory"]:
-                raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
+                raise NotADirectoryError(
+                    errno.ENOTDIR, 
+                    f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
+                )
             id = attr["id"]
             if get_version is not None:
                 version = get_version(attr)
-        if id_to_children is None:
+        if attr_cache is None:
             pid_attrs = None
         else:
-            pid_attrs = id_to_children.get(id)
+            pid_attrs = attr_cache.get(id)
         if (
             refresh or 
             pid_attrs is None or 
             "version" not in pid_attrs or
             version != pid_attrs["version"]
         ):
             pagesize = 1 << 10
             def normalize_attr(attr, dirname, /, **extra):
                 attr = normalize_info(attr, **extra)
                 path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                 if path_to_id is not None:
                     path_to_id[path] = attr["id"]
-                if id_to_children is not None:
+                if attr_cache is not None:
                     try:
-                        id_attrs = id_to_children[attr["id"]]
+                        id_attrs = attr_cache[attr["id"]]
                     except LookupError:
-                        id_to_children[attr["id"]] = {"attr": attr}
+                        attr_cache[attr["id"]] = {"attr": attr}
                     else:
                         try:
                             old_attr = id_attrs["attr"]
                         except LookupError:
                             id_attrs["attr"] = attr
                         else:
                             if path != old_attr["path"] and path_to_id is not None:
@@ -5578,76 +5616,77 @@
                 return attr
             def iterdir():
                 get_files = self._files
                 resp = get_files(id, limit=pagesize)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
-                lastest_update = datetime.now()
+                last_update = datetime.now()
                 count = resp["count"]
                 for attr in resp["data"]:
-                    yield normalize_attr(attr, dirname, lastest_update=lastest_update)
+                    yield normalize_attr(attr, dirname, fs=self, last_update=last_update)
                 for offset in range(pagesize, count, 1 << 10):
                     resp = get_files(id, limit=pagesize, offset=offset)
-                    lastest_update = datetime.now()
+                    last_update = datetime.now()
                     if resp["count"] != count:
                         raise RuntimeError(f"{id} detected count changes during iteration")
                     for attr in resp["data"]:
-                        yield normalize_attr(attr, dirname, lastest_update=lastest_update)
+                        yield normalize_attr(attr, dirname, fs=self, last_update=last_update)
             children = {a["id"]: a for a in iterdir()}
-            if id_to_children is not None:
-                attrs = id_to_children[id] = {"version": version, "attr": attr, "children": children}
+            if attr_cache is not None:
+                attrs = attr_cache[id] = {"version": version, "attr": attr, "children": children}
         else:
             children = pid_attrs["children"]
         return iter(children.values())
 
-    def _attr(self, id: int, /) -> dict:
+    def _attr(self, id: int, /)  -> AttrDict:
         if id == 0:
-            lastest_update = datetime.now()
+            last_update = datetime.now()
             return {
                 "id": 0, 
                 "parent_id": 0, 
                 "name": "", 
                 "path": "/", 
                 "is_directory": True, 
-                "lastest_update": lastest_update, 
-                "etime": lastest_update, 
-                "utime": lastest_update, 
+                "etime": last_update, 
+                "utime": last_update, 
                 "ptime": datetime.fromtimestamp(0), 
-                "open_time": lastest_update, 
+                "open_time": last_update, 
+                "last_update": last_update, 
+                "fs": self, 
             }
-        id_to_children = self.id_to_children
+        attr_cache = self.attr_cache
         get_version = self.get_version
-        if id_to_children is None:
+        if attr_cache is None:
             attrs = None
         else:
-            attrs = id_to_children.get(id)
+            attrs = attr_cache.get(id)
         if attrs and "attr" in attrs and get_version is None:
             return attrs["attr"]
         try:
             data = self._info(id)["data"][0]
         except OSError as e:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}") from e
-        attr = normalize_info(data, lastest_update=datetime.now())
+        attr = normalize_info(data, fs=self, last_update=datetime.now())
         pid = attr["parent_id"]
         attr_old = None
-        if id_to_children is not None:
+        if attr_cache is not None:
             if get_version is None:
                 version = None
             else:
                 version = get_version(attr)
             if attrs is None or "attr" not in attrs:
                 if attrs is None:
-                    id_to_children[id] = {"attr": attr}
+                    attr_cache[id] = {"attr": attr}
                 else:
                     attrs["attr"] = attr
                 try:
-                    pid_attrs = id_to_children[pid]
+                    pid_attrs = attr_cache[pid]
                 except LookupError:
-                    pid_attrs = id_to_children[pid] = {}
+                    pid_attrs = attr_cache[pid] = {}
                 try:
                     children = pid_attrs["children"]
                 except LookupError:
                     children = pid_attrs["children"] = {}
                 children[id] = attr
             else:
                 attr_old = attrs["attr"]
@@ -5672,15 +5711,15 @@
         return attr
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
         pid: Optional[int] = None, 
-    ) -> dict:
+    )  -> AttrDict:
         if isinstance(path, PathLike):
             path = fspath(path)
         if pid is None:
             pid = self.cid
         if not path or path == ".":
             return self._attr(pid)
         patht = self.get_patht(path, pid)
@@ -5699,30 +5738,35 @@
             except:
                 pass
         attr = self._attr(pid)
         for name in patht[len(self.get_patht(pid)):]:
             if not attr["is_directory"]:
                 raise NotADirectoryError(
                     errno.ENOTDIR, f"`pid` does not point to a directory: {pid!r}")
-            for attr in self.listdir_attr(pid):
+            for attr in self.iterdir(pid):
                 if attr["name"] == name:
                     pid = cast(int, attr["id"])
                     break
             else:
                 raise FileNotFoundError(errno.ENOENT, f"no such file {name!r} (in {pid!r})")
         return attr
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> dict:
+    )  -> AttrDict:
         if isinstance(id_or_path, P115Path):
             return self._attr(id_or_path.id)
+        elif isinstance(id_or_path, dict):
+            attr = id_or_path
+            if "id" in attr:
+                return self._attr(attr["id"])
+            return self._attr_path(attr["path"])
         elif isinstance(id_or_path, int):
             return self._attr(id_or_path)
         else:
             return self._attr_path(id_or_path, pid)
 
     # TODO 各种 batch_* 方法
 
@@ -5889,15 +5933,15 @@
                     f"destination is not directory: {src_fullpath!r} -> {dst_fullpath!r}", 
                 )
             elif overwrite_or_ignore is None:
                 raise FileExistsError(
                     errno.EEXIST, 
                     f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}", 
                 )
-        for attr in self.listdir_attr(src_id, **kwargs):
+        for attr in self.iterdir(src_id, **kwargs):
             if attr["is_directory"]:
                 self.copytree(
                     attr["id"], 
                     [attr["name"]], 
                     dst_id, 
                     overwrite_or_ignore=overwrite_or_ignore, 
                 )
@@ -5966,20 +6010,22 @@
                 return True
         if attr["is_directory"]:
             return self.get_directory_capacity(attr["id"]) > 0
         return attr["size"] == 0
 
     def makedirs(
         self, 
-        path: str | PathLike[str] | Sequence[str], 
+        path: str | PathLike[str] | Sequence[str] | AttrDict, 
         /, 
         pid: Optional[int] = None, 
         exist_ok: bool = False, 
     ) -> dict:
-        if isinstance(path, (str, PathLike)):
+        if isinstance(path, dict):
+            patht, parents = splits(path["path"])
+        elif isinstance(path, (str, PathLike)):
             patht, parents = splits(fspath(path))
         else:
             patht = [p for p in path if p]
             parents = 0
         if pid is None:
             pid = self.cid
         get_attr = self.attr
@@ -6084,15 +6130,15 @@
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
         clear_cache = self._clear_cache
         if attr["is_directory"]:
             if not recursive:
                 raise IsADirectoryError(errno.EISDIR, f"{id_or_path!r} (in {pid!r}) is a directory")
             if id == 0:
-                for subattr in self.listdir_attr(0):
+                for subattr in self.iterdir(0):
                     cid = subattr["id"]
                     self._delete(cid)
                     clear_cache(subattr)
                 return attr
         self._delete(id)
         clear_cache(attr)
         return attr
@@ -6270,42 +6316,39 @@
         self, 
         search_value: str, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
         page_size: int = 1_000, 
         offset: int = 0, 
-        as_path: bool = False, 
         **kwargs, 
     ) -> Iterator[P115Path]:
         assert page_size > 0
         payload = {
             "cid": self.get_id(id_or_path, pid), 
             "search_value": search_value, 
             "limit": page_size, 
             "offset": offset, 
             **kwargs, 
         }
-        if as_path:
-            def wrap(attr):
-                attr = normalize_info(attr, lastest_update=lastest_update)
-                return P115Path(self, **attr)
-        else:
-            def wrap(attr):
-                return normalize_info(attr, lastest_update=lastest_update)
+        def wrap(attr):
+            attr = normalize_info(attr, fs=self, last_update=last_update)
+            return P115Path(attr)
         search = self._search
         while True:
             resp = search(payload)
-            lastest_update = datetime.now()
+            last_update = datetime.now()
             if resp["offset"] != offset:
                 break
             data = resp["data"]
             if not data:
                 return
-            yield from map(wrap, resp["data"])
+            for attr in resp["data"]:
+                attr = normalize_info(attr, fs=self, last_update=last_update)
+                yield P115Path(attr)
             offset = payload["offset"] = offset + resp["page_size"]
             if offset >= resp["count"]:
                 break
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
@@ -6482,39 +6525,39 @@
     rm  = remove
 
 
 class P115SharePath(P115PathBase):
     fs: P115ShareFileSystem
 
 
-class P115ShareFileSystem(P115FileSystemBase[MappingProxyType, P115SharePath]):
+class P115ShareFileSystem(P115FileSystemBase[P115SharePath]):
     share_link: str
     share_code: str
     receive_code: str
     user_id: int
     path_to_id: MutableMapping[str, int]
-    id_to_attr: MutableMapping[int, MappingProxyType]
-    id_to_children: MutableMapping[int, tuple[MappingProxyType]]
+    id_to_attr: MutableMapping[int, AttrDict]
+    attr_cache: MutableMapping[int, tuple[AttrDict]]
     full_loaded: bool
     path_class = P115SharePath
 
     def __init__(self, /, client: P115Client, share_link: str):
-        m = CRE_SHARE_LINK.search(share_link)
+        m = CRE_SHARE_LINK_search(share_link)
         if m is None:
             raise ValueError("not a valid 115 share link")
         self.__dict__.update(
             client=client, 
             cid=0, 
             path="/", 
             share_link=share_link, 
             share_code=m["share_code"], 
             receive_code= m["receive_code"] or "", 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
-            id_to_children={}, 
+            attr_cache={}, 
             full_loaded=False, 
         )
         self.__dict__["user_id"] = int(self.sharedata["userinfo"]["user_id"])
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
@@ -6571,30 +6614,32 @@
     def sharedata(self, /) -> dict:
         return self._files(limit=1)["data"]
 
     @property
     def shareinfo(self, /) -> dict:
         return self.sharedata["shareinfo"]
 
-    def _attr(self, id: int = 0, /) -> MappingProxyType:
+    def _attr(self, id: int = 0, /) -> AttrDict:
         try:
             return self.id_to_attr[id]
         except KeyError:
             pass
         if self.full_loaded:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}")
         if id == 0:
-            attr = self.id_to_attr[0] = MappingProxyType({
+            attr = self.id_to_attr[0] = {
                 "id": 0, 
                 "parent_id": 0, 
                 "name": "", 
                 "path": "/", 
                 "is_directory": True, 
                 "time": self.create_time, 
-            })
+                "last_update": datetime.now(), 
+                "fs": self, 
+            }
             return attr
         dq = deque((0,))
         while dq:
             pid = dq.popleft()
             for attr in self.iterdir(pid):
                 if attr["id"] == id:
                     return attr
@@ -6604,15 +6649,15 @@
         raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}")
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
         pid: Optional[int] = None, 
-    ) -> MappingProxyType:
+    ) -> AttrDict:
         if isinstance(path, PathLike):
             path = fspath(path)
         if pid is None:
             pid = self.cid
         if not path or path == ".":
             return self._attr(pid)
         patht = self.get_patht(path, pid)
@@ -6637,30 +6682,37 @@
         return attr
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> MappingProxyType:
-        if isinstance(id_or_path, P115SharePath):
+    ) -> AttrDict:
+        path_class = type(self).path_class
+        if isinstance(id_or_path, path_class):
             return self._attr(id_or_path["id"])
+        elif isinstance(id_or_path, dict):
+            attr = id_or_path
+            if "id" in attr:
+                return self._attr(attr["id"])
+            return self._attr_path(attr["path"])
         elif isinstance(id_or_path, int):
             return self._attr(id_or_path)
         else:
             return self._attr_path(id_or_path, pid)
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
     ) -> str:
-        if isinstance(id_or_path, (int, P115ZipPath)):
+        path_class = type(self).path_class
+        if isinstance(id_or_path, (int, path_class)):
             id = id_or_path if isinstance(id_or_path, int) else id_or_path.id
             if id in self.id_to_attr:
                 attr = self.id_to_attr[id]
                 if attr["is_directory"]:
                     raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         else:
             attr = self.attr(id_or_path, pid)
@@ -6674,51 +6726,56 @@
         }, headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> Iterator[MappingProxyType]:
-        if isinstance(id_or_path, (int, P115ZipPath)):
-            id = id_or_path if isinstance(id_or_path, int) else id_or_path.id
-            if id in self.id_to_attr:
-                attr = self.id_to_attr[id]
-                if not attr["is_directory"]:
-                    raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
-            else:
-                try:
-                    self.get_url(id)
-                except IsADirectoryError:
-                    pass
+    ) -> Iterator[AttrDict]:
+        path_class = type(self).path_class
+        if isinstance(id_or_path, int):
+            attr = self.attr(id_or_path)
+        elif isinstance(id_or_path, dict):
+            attr = id_or_path
+        elif isinstance(id_or_path, path_class):
+            attr = id_or_path.__dict__
         else:
             attr = self.attr(id_or_path, pid)
-            if not attr["is_directory"]:
-                raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
-            id = attr["id"]
+        if not attr["is_directory"]:
+            raise NotADirectoryError(
+                errno.ENOTDIR, 
+                f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
+            )
+        id = attr["id"]
         try:
-            return iter(self.id_to_children[id])
+            return iter(self.attr_cache[id])
         except KeyError:
             dirname = attr["path"]
             def iterdir():
                 page_size = 1 << 10
                 get_files = self._files
                 path_to_id = self.path_to_id
                 data = get_files(id, page_size)["data"]
+                last_update = datetime.now()
                 for attr in map(normalize_info, data["list"]):
+                    attr["fs"] = self
+                    attr["last_update"] = last_update
                     path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                     path_to_id[path] = attr["id"]
-                    yield MappingProxyType(attr)
+                    yield attr
                 for offset in range(page_size, data["count"], page_size):
                     data = get_files(id, page_size, offset)["data"]
+                    last_update = datetime.now()
                     for attr in map(normalize_info, data["list"]):
+                        attr["fs"] = self
+                        attr["last_update"] = last_update
                         path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                         path_to_id[path] = attr["id"]
-                        yield MappingProxyType(attr)
-            t = self.id_to_children[id] = tuple(iterdir())
+                        yield attr
+            t = self.attr_cache[id] = tuple(iterdir())
             self.id_to_attr.update((attr["id"], attr) for attr in t)
             return iter(t)
 
     def receive(self, ids: int | str | Iterable[int | str], /, cid: int = 0):
         if isinstance(ids, int):
             ids = str(ids)
         elif isinstance(ids, Iterable):
@@ -6737,26 +6794,26 @@
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
-        lastest_update = attr.get("lastest_update") or datetime.now()
+        last_update = attr.get("last_update") or datetime.now()
         return stat_result((
             (S_IFDIR if is_dir else S_IFREG) | 0o444, 
             attr["id"], 
             attr["parent_id"], 
             1, 
             self.user_id, 
             1, 
             0 if is_dir else attr["size"], 
-            attr.get("time", lastest_update).timestamp(), 
-            attr.get("time", lastest_update).timestamp(), 
-            attr.get("time", lastest_update).timestamp(), 
+            attr.get("time", last_update).timestamp(), 
+            attr.get("time", last_update).timestamp(), 
+            attr.get("time", last_update).timestamp(), 
         ))
 
 
 # TODO: 兼容 pathlib.Path 和 zipfile.Path 的接口
 class P115ZipPath(P115PathBase):
     fs: P115ZipFileSystem
     path: str
@@ -6893,20 +6950,20 @@
                     return
                 sleep(1)
         Thread(target=update_progress).start()
 
 
 # TODO: 参考 zipfile 模块的接口设计 namelist、filelist 等属性，以及其它的和 zipfile 兼容的接口
 # TODO: 当文件特别多时，可以用 zipfile 等模块来读取文件列表
-class P115ZipFileSystem(P115FileSystemBase[MappingProxyType, P115ZipPath]):
+class P115ZipFileSystem(P115FileSystemBase[P115ZipPath]):
     file_id: Optional[int]
     pick_code: str
     path_to_id: MutableMapping[str, int]
-    id_to_attr: MutableMapping[int, MappingProxyType]
-    id_to_children: MutableMapping[int, tuple[MappingProxyType]]
+    id_to_attr: MutableMapping[int, AttrDict]
+    attr_cache: MutableMapping[int, tuple[AttrDict]]
     full_loaded: bool
     path_class = P115ZipPath
 
     def __init__(
         self, 
         /, 
         client: P115Client, 
@@ -6926,15 +6983,15 @@
             client=client, 
             cid=0, 
             path="/", 
             pick_code=pick_code, 
             file_id=file_id, 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
-            id_to_children={}, 
+            attr_cache={}, 
             full_loaded=False, 
             _nextid=count(1).__next__, 
         )
         if file_id is None:
             self.__dict__["create_time"] = datetime.fromtimestamp(0)
 
     def __setattr__(self, attr, val, /) -> Never:
@@ -6964,33 +7021,35 @@
 
     @cached_property
     def create_time(self, /) -> datetime:
         if self.file_id is None:
             return datetime.fromtimestamp(0)
         return self.client.fs.attr(self.file_id)["ptime"]
 
-    def _attr(self, id: int = 0, /) -> MappingProxyType:
+    def _attr(self, id: int = 0, /) -> AttrDict:
         try:
             return self.id_to_attr[id]
         except KeyError:
             pass
         if self.full_loaded:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}")
         if id == 0:
-            attr = self.id_to_attr[0] = MappingProxyType({
+            attr = self.id_to_attr[0] = {
                 "id": 0, 
                 "parent_id": 0, 
                 "file_category": 0, 
                 "is_directory": True, 
                 "name": "", 
                 "path": "/", 
                 "size": 0, 
                 "time": self.create_time, 
                 "timestamp": int(self.create_time.timestamp()), 
-            })
+                "last_update": datetime.now(), 
+                "fs": self, 
+            }
             return attr
         dq = deque((0,))
         while dq:
             pid = dq.popleft()
             for attr in self.iterdir(pid):
                 if attr["id"] == id:
                     return attr
@@ -7000,15 +7059,15 @@
         raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}")
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
         pid: Optional[int] = None, 
-    ) -> MappingProxyType:
+    ) -> AttrDict:
         if isinstance(path, PathLike):
             path = fspath(path)
         if pid is None:
             pid = self.cid
         if not path or path == ".":
             return self._attr(pid)
         patht = self.get_patht(path, pid)
@@ -7033,17 +7092,23 @@
         return attr
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> MappingProxyType:
-        if isinstance(id_or_path, P115ZipPath):
+    ) -> AttrDict:
+        path_class = type(self).path_class
+        if isinstance(id_or_path, path_class):
             return self._attr(id_or_path["id"])
+        elif isinstance(id_or_path, dict):
+            attr = id_or_path
+            if "id" in attr:
+                return self._attr(attr["id"])
+            return self._attr_path(attr["path"])
         elif isinstance(id_or_path, int):
             return self._attr(id_or_path)
         else:
             return self._attr_path(id_or_path, pid)
 
     def extract(
         self, 
@@ -7067,56 +7132,61 @@
         return self.client.extract_download_url(self.pick_code, attr["path"], headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-    ) -> Iterator[MappingProxyType]:
+    ) -> Iterator[AttrDict]:
         def normalize_info(info):
             timestamp = info.get("time") or 0
             return {
                 "name": info["file_name"], 
                 "is_directory": info["file_category"] == 0, 
                 "file_category": info["file_category"], 
                 "size": info["size"], 
                 "time": datetime.fromtimestamp(timestamp), 
                 "timestamp": timestamp, 
+                "fs": self, 
             }
         attr = self.attr(id_or_path, pid)
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
         try:
-            return iter(self.id_to_children[id])
+            return iter(self.attr_cache[id])
         except KeyError:
             nextid = self.__dict__["_nextid"]
             dirname = attr["path"]
             def iterdir():
                 get_files = self._files
                 path_to_id = self.path_to_id
                 data = get_files(dirname)["data"]
+                last_update = datetime.now()
                 for attr in map(normalize_info, data["list"]):
+                    attr["last_update"] = last_update
                     path = joinpath(dirname, escape(attr["name"]))
                     attr.update(id=nextid(), parent_id=id, path=path)
                     path_to_id[path] = attr["id"]
-                    yield MappingProxyType(attr)
+                    yield attr
                 next_marker = data["next_marker"]
                 while next_marker:
                     data = get_files(dirname, next_marker)["data"]
+                    last_update = datetime.now()
                     for attr in map(normalize_info, data["list"]):
+                        attr["last_update"] = last_update
                         path = joinpath(dirname, escape(attr["name"]))
                         attr.update(id=nextid(), parent_id=id, path=path)
                         path_to_id[path] = attr["id"]
-                        yield MappingProxyType(attr)
+                        yield attr
                     next_marker = data["next_marker"]
-            t = self.id_to_children[id] = tuple(iterdir())
+            t = self.attr_cache[id] = tuple(iterdir())
             self.id_to_attr.update((attr["id"], attr) for attr in t)
             return iter(t)
 
 
 class P115Offline:
     __slots__ = ("client", "_sign_time")
 
@@ -7527,9 +7597,9 @@
         return self.client.share_update({"share_code": share_code, **payload})
 
 
 # TODO upload_tree 多线程和进度条，并且为每一个上传返回一个 task，可重试
 # TODO 能及时处理文件已不存在
 # TODO 为各个fs接口添加额外的请求参数
 # TODO 115中多个文件可以在同一目录下同名，如何处理
-# TODO 上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传了的话）
+# TODO 提供一个新的上传函数，上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传成功了的话）
 # TODO 如果压缩包尚未解压，则使用 zipfile 之类的模块，去模拟文件系统
```

### Comparing `python_115-0.0.5.6/p115/util/_init_mimetypes.py` & `python_115-0.0.5.7/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/cipher.py` & `python_115-0.0.5.7/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/concurrent.py` & `python_115-0.0.5.7/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/download.py` & `python_115-0.0.5.7/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/file.py` & `python_115-0.0.5.7/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/hash.py` & `python_115-0.0.5.7/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/ignore.py` & `python_115-0.0.5.7/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/iter.py` & `python_115-0.0.5.7/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/path.py` & `python_115-0.0.5.7/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/property.py` & `python_115-0.0.5.7/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/response.py` & `python_115-0.0.5.7/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/retry.py` & `python_115-0.0.5.7/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/text.py` & `python_115-0.0.5.7/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/p115/util/urlopen.py` & `python_115-0.0.5.7/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/pyproject.toml` & `python_115-0.0.5.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.6"
+version = "0.0.5.7"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.6/readme.md` & `python_115-0.0.5.7/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.6/PKG-INFO` & `python_115-0.0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.6
+Version: 0.0.5.7
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

