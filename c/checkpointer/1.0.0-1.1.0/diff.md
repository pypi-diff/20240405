# Comparing `tmp/checkpointer-1.0.0-py3-none-any.whl.zip` & `tmp/checkpointer-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7397 bytes, number of entries: 13
+Zip file size: 7368 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      380 b- defN 22-Jan-18 08:50 checkpointer/__init__.py
--rw-r--r--  2.0 unx     2367 b- defN 22-Jan-18 08:50 checkpointer/checkpoint.py
--rw-r--r--  2.0 unx     1760 b- defN 22-Jan-18 08:50 checkpointer/function_body.py
+-rw-r--r--  2.0 unx     2367 b- defN 24-Apr-05 16:46 checkpointer/checkpoint.py
+-rw-r--r--  2.0 unx     1703 b- defN 24-Apr-05 16:52 checkpointer/function_body.py
 -rw-r--r--  2.0 unx     1782 b- defN 22-Jan-18 08:50 checkpointer/storage.py
--rw-r--r--  2.0 unx      381 b- defN 22-Jan-18 08:50 checkpointer/utils.py
+-rw-r--r--  2.0 unx      377 b- defN 24-Apr-05 16:43 checkpointer/utils.py
 -rw-r--r--  2.0 unx     2728 b- defN 22-Jan-18 08:50 checkpointer/storages/bcolz_storage.py
 -rw-r--r--  2.0 unx      364 b- defN 22-Jan-18 08:50 checkpointer/storages/memory_storage.py
 -rw-r--r--  2.0 unx     1542 b- defN 22-Jan-18 08:50 checkpointer/storages/pickle_storage.py
--rw-r--r--  2.0 unx     1054 b- defN 22-Jan-18 08:52 checkpointer-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      317 b- defN 22-Jan-18 08:52 checkpointer-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-18 08:52 checkpointer-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Jan-18 08:52 checkpointer-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1106 b- defN 22-Jan-18 08:52 checkpointer-1.0.0.dist-info/RECORD
-13 files, 13886 bytes uncompressed, 5533 bytes compressed:  60.2%
+-rw-r--r--  2.0 unx     1054 b- defN 24-Apr-05 16:55 checkpointer-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-05 16:55 checkpointer-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 16:55 checkpointer-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-05 16:55 checkpointer-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1106 b- defN 24-Apr-05 16:55 checkpointer-1.1.0.dist-info/RECORD
+13 files, 13781 bytes uncompressed, 5504 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: checkpointer/storages/memory_storage.py
 Comment: 
 
 Filename: checkpointer/storages/pickle_storage.py
 Comment: 
 
-Filename: checkpointer-1.0.0.dist-info/LICENSE.txt
+Filename: checkpointer-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: checkpointer-1.0.0.dist-info/METADATA
+Filename: checkpointer-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: checkpointer-1.0.0.dist-info/WHEEL
+Filename: checkpointer-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: checkpointer-1.0.0.dist-info/top_level.txt
+Filename: checkpointer-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: checkpointer-1.0.0.dist-info/RECORD
+Filename: checkpointer-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## checkpointer/function_body.py

```diff
@@ -1,10 +1,9 @@
 import inspect
 from types import FunctionType, CodeType
-from relib.raypipe import raypipe
 import relib.hashing as hashing
 from pathlib import Path
 from .utils import unwrap_func
 
 cwd = Path.cwd()
 
 def get_func_path(func):
@@ -14,45 +13,40 @@
   # TODO: Strip comments
   lines = inspect.getsourcelines(func)[0]
   lines = [line.rstrip() for line in lines]
   lines = [line for line in lines if line]
   return '\n'.join(lines)
 
 def get_code_children(__code__):
-  return raypipe \
-    .filter(lambda const: isinstance(const, CodeType)) \
-    .flat_map(get_code_children) \
-    .do(lambda children: list(__code__.co_names) + children) \
-    .compute(__code__.co_consts)
+  consts = [const for const in __code__.co_consts if isinstance(const, CodeType)]
+  children = [child for const in consts for child in get_code_children(const)]
+  return list(__code__.co_names) + children
 
 def get_func_children(func, neighbor_funcs=[]):
   def get_candidate_func(co_name):
     candidate_func = func.__globals__.get(co_name, None)
     return unwrap_func(candidate_func)
 
   def clear_candidate(candidate_func):
     return isinstance(candidate_func, FunctionType) \
       and candidate_func not in neighbor_funcs \
       and cwd in get_func_path(candidate_func).parents
 
   code_children = get_code_children(func.__code__)
 
-  func_children = raypipe \
-    .map(get_candidate_func) \
-    .filter(clear_candidate) \
-    .compute(code_children)
-
-  funcs = raypipe \
-    .flat_map(lambda child_func: \
-      get_func_children(child_func, func_children)
-    ) \
-    .do(lambda grand_children: [func] + grand_children) \
-    .sort_distinct(lambda func: func.__name__) \
-    .compute(func_children)
+  func_children = [get_candidate_func(child) for child in code_children]
+  func_children = [child for child in func_children if clear_candidate(child)]
+
+  funcs = [func] + [
+    deep_child
+    for child_func in func_children
+    for deep_child in get_func_children(child_func, func_children)
+  ]
+  funcs = sorted(set(funcs), key=lambda func: func.__name__)
 
   return funcs
 
 def get_function_hash(func):
   funcs = [func] + get_func_children(func)
-  function_bodies = raypipe.map(get_function_body).compute(funcs)
+  function_bodies = list(map(get_function_body, funcs))
   function_bodies_hash = hashing.hash(function_bodies)
   return function_bodies_hash
```

## checkpointer/utils.py

```diff
@@ -1,16 +1,16 @@
-import asyncio
+import types
 
 def unwrap_func(func):
   if hasattr(func, '__wrapped__'):
     return unwrap_func(func.__wrapped__)
   else:
     return func
 
-@asyncio.coroutine
+@types.coroutine
 def coroutine_as_generator(coroutine):
   val = yield from coroutine
   return val
 
 def sync_resolve_coroutine(coroutine):
   try:
     next(coroutine_as_generator(coroutine))
```

## Comparing `checkpointer-1.0.0.dist-info/LICENSE.txt` & `checkpointer-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `checkpointer-1.0.0.dist-info/RECORD` & `checkpointer-1.1.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 checkpointer/__init__.py,sha256=_RYcKsZbeUf08KZ-DcXlNn4eAMWh2LN9o-KvchYVmmk,380
 checkpointer/checkpoint.py,sha256=FyL78HvAvPtgl-esiAkt-CdekT18J2Sh0SriMtX4QLc,2367
-checkpointer/function_body.py,sha256=kBsgCPeNgQzgXFToTuqQYYvAQicetXtv-UGwyd5b4Ew,1760
+checkpointer/function_body.py,sha256=aitzBFoEIo_E-aL2oe4Nr_T_Oy8ehKInGb1XYjeLzX8,1703
 checkpointer/storage.py,sha256=Ofuh0dKF5vk4_B4djt3Q6qyZhIO5f59uCNCZjMrto0U,1782
-checkpointer/utils.py,sha256=5CFQHUAlrORFpcg-TGuvAUQDeCEXvvx6yPl8mor5jh8,381
+checkpointer/utils.py,sha256=Kzh2qXxq2Lgjiqfv6KcOwXdw7sh70uCn4a_uXYwLhiM,377
 checkpointer/storages/bcolz_storage.py,sha256=Yk7FI75noe9hZBWVFIRetiFSR7tkzbryYlBmxX-lVlw,2728
 checkpointer/storages/memory_storage.py,sha256=S4SgKSApbQE-pxxKRWLNJqyZMRQwaw5-N0DOIsZM7mE,364
 checkpointer/storages/pickle_storage.py,sha256=zcnX1GG6XPHvVxi7gCab5oFxKoz5E7LZHYH74VL1hkY,1542
-checkpointer-1.0.0.dist-info/LICENSE.txt,sha256=2c7g4mni-RUemFGkk6GnoFwknh-leF04BF_J_3gp4sg,1054
-checkpointer-1.0.0.dist-info/METADATA,sha256=kmuSQOTbRa5KaFBlr48K-Fin7bRD3L7aIZiC0Lx8v6o,317
-checkpointer-1.0.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-checkpointer-1.0.0.dist-info/top_level.txt,sha256=uF0eyHpShnsHI3sobErnhQ8LWCT8DPViqAznKeTaZlw,13
-checkpointer-1.0.0.dist-info/RECORD,,
+checkpointer-1.1.0.dist-info/LICENSE.txt,sha256=2c7g4mni-RUemFGkk6GnoFwknh-leF04BF_J_3gp4sg,1054
+checkpointer-1.1.0.dist-info/METADATA,sha256=_isCKu9zdEI1Z-umSB6mr-X7lEVBVjlU_QvRNYolUNQ,273
+checkpointer-1.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+checkpointer-1.1.0.dist-info/top_level.txt,sha256=uF0eyHpShnsHI3sobErnhQ8LWCT8DPViqAznKeTaZlw,13
+checkpointer-1.1.0.dist-info/RECORD,,
```

