# Comparing `tmp/tokengrams-0.2.0-cp310-cp310-manylinux_2_31_x86_64.whl.zip` & `tmp/tokengrams-0.3.0-cp310-cp310-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 415044 bytes, number of entries: 8
--rw-r--r--  4.6 unx     1642 b- defN 24-Apr-03 01:36 tokengrams-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx      108 b- defN 24-Apr-03 01:36 tokengrams-0.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       63 b- defN 24-Apr-03 01:36 tokengrams/__init__.py
--rw-r--r--  4.6 unx        0 b- defN 24-Apr-03 01:36 tokengrams/tests/__init__.py
--rw-r--r--  4.6 unx     1605 b- defN 24-Apr-03 01:36 tokengrams/tests/test_gram_index.py
--rw-r--r--  4.6 unx     3587 b- defN 24-Apr-03 01:36 tokengrams/tokengrams.pyi
--rwxr-xr-x  4.6 unx  1071760 b- defN 24-Apr-03 01:36 tokengrams/tokengrams.cpython-310-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      662 b- defN 24-Apr-03 01:36 tokengrams-0.2.0.dist-info/RECORD
-8 files, 1079427 bytes uncompressed, 413888 bytes compressed:  61.7%
+Zip file size: 361290 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2764 b- defN 24-Apr-05 03:32 tokengrams-0.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      104 b- defN 24-Apr-05 03:32 tokengrams-0.3.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx        0 b- defN 24-Apr-05 03:32 tokengrams/tests/__init__.py
+-rw-r--r--  4.6 unx     1633 b- defN 24-Apr-05 03:32 tokengrams/tests/test_gram_index.py
+-rw-r--r--  4.6 unx     3928 b- defN 24-Apr-05 03:32 tokengrams/tokengrams.pyi
+-rw-r--r--  4.6 unx       93 b- defN 24-Apr-05 03:32 tokengrams/__init__.py
+-rwxr-xr-x  4.6 unx   857853 b- defN 24-Apr-05 03:32 tokengrams/tokengrams.cpython-310-darwin.so
+-rw-r--r--  4.6 unx      651 b- defN 24-Apr-05 03:32 tokengrams-0.3.0.dist-info/RECORD
+8 files, 867026 bytes uncompressed, 360154 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: tokengrams-0.2.0.dist-info/METADATA
+Filename: tokengrams-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: tokengrams-0.2.0.dist-info/WHEEL
-Comment: 
-
-Filename: tokengrams/__init__.py
+Filename: tokengrams-0.3.0.dist-info/WHEEL
 Comment: 
 
 Filename: tokengrams/tests/__init__.py
 Comment: 
 
 Filename: tokengrams/tests/test_gram_index.py
 Comment: 
 
 Filename: tokengrams/tokengrams.pyi
 Comment: 
 
-Filename: tokengrams/tokengrams.cpython-310-x86_64-linux-gnu.so
+Filename: tokengrams/__init__.py
+Comment: 
+
+Filename: tokengrams/tokengrams.cpython-310-darwin.so
 Comment: 
 
-Filename: tokengrams-0.2.0.dist-info/RECORD
+Filename: tokengrams-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tokengrams/__init__.py

```diff
@@ -1,4 +1,7 @@
+import os
+print(os.getcwd())
+
 from .tokengrams import (
     InMemoryIndex,
     MemmapIndex,
 )
```

## tokengrams/tests/test_gram_index.py

```diff
@@ -24,29 +24,29 @@
 @given(
     st.lists(
         st.integers(0, 2 ** 16 - 1), min_size=1,
     )
 )
 def test_gram_index(tokens: list[int]):
     # Construct index
-    index = InMemoryIndex(tokens)
+    index = InMemoryIndex(tokens, False)
     check_gram_index(index, tokens)
 
     # Save to disk and check that we can load it back
     with NamedTemporaryFile() as f:
         memmap = np.memmap(f, dtype=np.uint16, mode="w+", shape=(len(tokens),))
         memmap[:] = tokens
 
-        index = InMemoryIndex.from_token_file(f.name, None)
+        index = InMemoryIndex.from_token_file(f.name, False, None)
         check_gram_index(index, tokens)
 
         with NamedTemporaryFile() as idx:
-            index = MemmapIndex.build(f.name, idx.name)
+            index = MemmapIndex.build(f.name, idx.name, False)
             check_gram_index(index, tokens)
 
             index = MemmapIndex(f.name, idx.name)
             check_gram_index(index, tokens)
 
         # Now check limited token loading
         for limit in range(1, len(tokens) + 1):
-            index = InMemoryIndex.from_token_file(f.name, limit)
+            index = InMemoryIndex.from_token_file(f.name, False, limit)
             check_gram_index(index, tokens[:limit])
```

## tokengrams/tokengrams.pyi

```diff
@@ -1,27 +1,30 @@
 class InMemoryIndex:
     """An n-gram index."""
 
-    def __init__(self, tokens: list[int]) -> None:
+    def __init__(self, tokens: list[int], verbose: bool) -> None:
         ...
     
     @staticmethod
-    def from_token_file(path: str, token_limit: int | None) -> "InMemoryIndex":
+    def from_token_file(path: str, verbose: bool, token_limit: int | None) -> "InMemoryIndex":
         """Construct a `InMemoryIndex` from a file containing raw little-endian tokens."""
 
     def contains(self, query: list[int]) -> bool:
         """Check if `query` has nonzero count. Faster than `count(query) > 0`."""
     
     def count(self, query: list[int]) -> int:
         """Count the number of occurrences of `query` in the index."""
 
     def positions(self, query: list[int]) -> list[int]:
         """Returns an unordered list of positions where `query` starts in `text`."""
 
-    def batch_next_token_counts(self, queries: list[list[int]], vocab: int | None) -> list[list[int]]:
+    def count_next(self, query: list[int], vocab: int | None) -> list[int]:
+        """Count the occurrences of each token directly following `query`."""
+
+    def batch_count_next(self, queries: list[list[int]], vocab: int | None) -> list[list[int]]:
         """Count the occurrences of each token that directly follows each sequence in `queries`."""
 
     def sample(self, query: list[int], n: int, k: int) -> list[int]:
         """Autoregressively sample k characters from conditional distributions based 
         on the previous (n - 1) characters (n-gram prefix) in the sequence. If there are fewer than 
         (n - 1) characters all available characters are used.""" 
     
@@ -37,27 +40,30 @@
 class MemmapIndex:
     """An n-gram index backed by a memory-mapped file."""
 
     def __init__(self, token_file: str, index_file: str) -> None:
         """Load a prebuilt memory-mapped index from a pair of files."""
 
     @staticmethod
-    def build(token_file: str, index_file: str) -> "MemmapIndex":
+    def build(token_file: str, index_file: str, verbose: bool) -> "MemmapIndex":
         """Build a memory-mapped index from a token file."""
     
     def contains(self, query: list[int]) -> bool:
         """Check if `query` has nonzero count. Faster than `count(query) > 0`."""
     
     def count(self, query: list[int]) -> int:
         """Count the number of occurrences of `query` in the index."""
 
     def positions(self, query: list[int]) -> list[int]:
         """Returns an unordered list of positions where `query` starts in `text`."""
 
-    def batch_next_token_counts(self, queries: list[list[int]], vocab: int | None) -> list[list[int]]:
+    def count_next(self, query: list[int], vocab: int | None) -> list[int]:
+        """Count the occurrences of each token directly following `query`."""
+
+    def batch_count_next(self, queries: list[list[int]], vocab: int | None) -> list[list[int]]:
         """Count the occurrences of each token that directly follows each sequence in `queries`."""
 
     def sample(self, query: list[int], n: int, k: int) -> list[int]:
         """Autoregressively k characters from conditional distributions based 
         on the previous (n - 1) characters (n-gram prefix) in the sequence. If there are fewer than 
         (n - 1) characters all available characters are used."""
```

