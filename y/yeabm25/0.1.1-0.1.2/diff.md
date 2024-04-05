# Comparing `tmp/yeabm25-0.1.1.tar.gz` & `tmp/yeabm25-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeabm25-0.1.1.tar", last modified: Sun Mar 31 15:55:33 2024, max compression
+gzip compressed data, was "yeabm25-0.1.2.tar", last modified: Fri Apr  5 10:10:54 2024, max compression
```

## Comparing `yeabm25-0.1.1.tar` & `yeabm25-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 15:55:33.215166 yeabm25-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-03-24 19:44:05.000000 yeabm25-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    16878 2024-03-31 15:55:33.215166 yeabm25-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3094 2024-03-31 15:12:44.000000 yeabm25-0.1.1/README.md
--rw-rw-rw-   0        0        0      848 2024-03-31 15:47:58.000000 yeabm25-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 15:55:33.215166 yeabm25-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-31 15:55:33.199523 yeabm25-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 15:55:33.199523 yeabm25-0.1.1/src/yeabm25/
--rw-rw-rw-   0        0        0       39 2024-03-23 17:47:15.000000 yeabm25-0.1.1/src/yeabm25/__init__.py
--rw-rw-rw-   0        0        0    10354 2024-03-31 14:57:02.000000 yeabm25-0.1.1/src/yeabm25/bm25.py
-drwxrwxrwx   0        0        0        0 2024-03-31 15:55:33.215166 yeabm25-0.1.1/src/yeabm25.egg-info/
--rw-rw-rw-   0        0        0    16878 2024-03-31 15:55:33.000000 yeabm25-0.1.1/src/yeabm25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-03-31 15:55:33.000000 yeabm25-0.1.1/src/yeabm25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 15:55:33.000000 yeabm25-0.1.1/src/yeabm25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-31 15:55:33.000000 yeabm25-0.1.1/src/yeabm25.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-31 15:55:33.000000 yeabm25-0.1.1/src/yeabm25.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 15:55:33.215166 yeabm25-0.1.1/tests/
--rw-rw-rw-   0        0        0     1806 2024-03-31 15:19:12.000000 yeabm25-0.1.1/tests/test_yeabm25.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-03-24 19:44:05.000000 yeabm25-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    16841 2024-04-05 10:10:54.326377 yeabm25-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3057 2024-04-02 16:49:16.000000 yeabm25-0.1.2/README.md
+-rw-rw-rw-   0        0        0      848 2024-04-05 10:10:14.000000 yeabm25-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 10:10:54.326377 yeabm25-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.295130 yeabm25-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.310752 yeabm25-0.1.2/src/yeabm25/
+-rw-rw-rw-   0        0        0       39 2024-03-23 17:47:15.000000 yeabm25-0.1.2/src/yeabm25/__init__.py
+-rw-rw-rw-   0        0        0    11440 2024-04-03 19:45:20.000000 yeabm25-0.1.2/src/yeabm25/bm25.py
+drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/src/yeabm25.egg-info/
+-rw-rw-rw-   0        0        0    16841 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 10:10:54.000000 yeabm25-0.1.2/src/yeabm25.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 10:10:54.326377 yeabm25-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1806 2024-03-31 15:19:12.000000 yeabm25-0.1.2/tests/test_yeabm25.py
```

### Comparing `yeabm25-0.1.1/LICENSE` & `yeabm25-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yeabm25-0.1.1/PKG-INFO` & `yeabm25-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeabm25
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Author-email: Demir Tonchev <{surname}.{name}@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -252,15 +252,15 @@
 assert yeabm.doc_len == bm_update.doc_len
 assert yeabm.average_idf == bm_update.average_idf
 assert yeabm.idf == bm_update.idf
 assert yeabm.get_scores(['fox', 'jump']) == bm_update.get_scores(['fox', 'jump'])).all()
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
-The main focus is creating document and query vectors (sparse vectors support - soon(hopefully not "Blizzard soon")). Then using the vectors with your favourite Vector DB.
+The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
 # recommended approach for large corpus, returns iterator. Each element is list[float]
 # returns generator object
 yeabm.iter_document_vectors()
 # use it
```

### Comparing `yeabm25-0.1.1/README.md` & `yeabm25-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 assert yeabm.doc_len == bm_update.doc_len
 assert yeabm.average_idf == bm_update.average_idf
 assert yeabm.idf == bm_update.idf
 assert yeabm.get_scores(['fox', 'jump']) == bm_update.get_scores(['fox', 'jump'])).all()
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
-The main focus is creating document and query vectors (sparse vectors support - soon(hopefully not "Blizzard soon")). Then using the vectors with your favourite Vector DB.
+The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
 # recommended approach for large corpus, returns iterator. Each element is list[float]
 # returns generator object
 yeabm.iter_document_vectors()
 # use it
```

### Comparing `yeabm25-0.1.1/pyproject.toml` & `yeabm25-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package-dir = {"" = "src"}
 
 [project]
 name = "yeabm25"
 description = """Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Also you can get document and query vectors to use with any Vector DB."""
 requires-python = ">=3.10"
-version = "0.1.1"
+version = "0.1.2"
 keywords = ["text", "bm25", "dense vector embeddings", "information retrieval", "hybrid search"]
 readme = "README.md"
 dependencies = [
   "numpy>=1.26",
 ]
 authors = [
   {name = "Demir Tonchev", email = "{surname}.{name}@gmail.com"},
```

### Comparing `yeabm25-0.1.1/src/yeabm25/bm25.py` & `yeabm25-0.1.2/src/yeabm25/bm25.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import numpy as np
 from collections import defaultdict, Counter
 from dataclasses import dataclass, field
 from typing import TypeAlias, Optional
 
 # type alias just for readability
 Vector1d: TypeAlias = np.ndarray | list[float]
-
+SparseVector: TypeAlias = dict[int, float]  # #TODO | Iterable[Tuple[int, float]], scipy sparse
 
 # experimental
 # this is created with possible compatibility with haystack>2.0
+
+
 @dataclass
 class BMDocument:
     content: list[str]
     meta: dict = field(default_factory=dict)
     embedding: Optional[Vector1d] = None
 
     def __len__(self):
@@ -106,14 +108,15 @@
         self.doc_len = []  # number of words in each document
         self.avgdl: float = 0.
         # word -> number of documents with word {'cat': 50} means 'cat' is in 50 documents from the corpus
         self.word_df = defaultdict(int)
         self.idf: dict = {}
         self.average_idf: float = 0
         self.corpus_size: int = 0
+        self.ftoi: dict[str, int]  # feature name to index map
         self.__isfit = False
 
     def _process_doc(self, document: list[str]) -> None:
         """Gets a documents, which is represented as a list of words(strings).
         Appends frequencies of words per document and builds the word document frequencies. Wodf df is used for idf.
         """
         frequencies = Counter(document)
@@ -156,34 +159,38 @@
         self.doc_len = [len(doc) for doc in corpus]
         self.avgdl = sum(self.doc_len) / self.corpus_size
 
         for document in corpus:
             self._process_doc(document)
 
         self._calc_idf()
+        self._ftoi()
         self.__isfit = True
         return self
 
     def update(self, corpus: list[list[str]] | list[BMDocument]):
         self.corpus_size += len(corpus)
         self.doc_len += [len(doc) for doc in corpus]
         self.avgdl = sum(self.doc_len) / self.corpus_size
 
         for document in corpus:
             self._process_doc(document)
 
         self._calc_idf()
-
+        self._ftoi()
         return self
 
     # sklearn like api
     @property
     def features_(self):
         return [word for word in self.idf]
 
+    def _ftoi(self):
+        self.ftoi = {feat: idx for idx, feat in enumerate(self.features_)}
+
     def get_scores(self, query: list[str]):
         score = np.zeros(self.corpus_size)
         doc_len = np.asarray(self.doc_len)
         for q in set(query):
             q_freq = np.array([doc.get(q, 0) for doc in self.doc_freqs])
             score += self.idf.get(q, 0) * (q_freq * (self.k1 + 1) /
                                            (q_freq + self.k1 * (1 - self.b + self.b * doc_len / self.avgdl)))
@@ -192,37 +199,53 @@
     def get_top_n(self, query: list[str], n=5):
         """Returns the indexes of the top n documents and scores in sorted order.
         """
         scores = self.get_scores(query)
         isort = np.argsort(scores)[-n:][::-1]
         return {i: s for i, s in zip(isort, scores[isort].round(2))}
 
-    def document_self_scores(self, idx: int):
+    def document_self_scores(self, idx: int) -> dict[str, float]:
         scores = {}
         for q, q_freq in self.doc_freqs[idx].items():
             s = self.idf.get(q, 0) * (
                 q_freq * (self.k1 + 1) /
                 (q_freq + self.k1 * (1 - self.b + self.b * self.doc_len[idx] / self.avgdl))
             )
             scores[q] = s
         return scores
 
-    def document_vector(self, idx: int):
+    def encode_document(self, idx: int, outputtype: str = 'dict') -> SparseVector:
+        """Encodes document at index as a sparse vector. Ideal for vector DB.
+        """
+        return {self.ftoi[f]: s for f, s in self.document_self_scores(idx).items()}
+
+    def encode_document_dense(self, idx: int) -> list[float]:
+        """Encodes document at index as a dense vector.
+        """
         feats = self.features_
         scores = self.document_self_scores(idx)
         return [scores[f] if f in scores else 0. for f in feats]
 
     def iter_document_vectors(self):
-        """Iterate over the vectors, for example if you to store them in a Vector DB.
+        """Iterate over the vectors(dense), for example if you to store them in a Vector DB.
+        """
+        for idx in range(len(self.doc_freqs)):
+            yield self.encode_document_dense(idx)
+
+    def iter_document_vectors_sparse(self):
+        """Iterate over the vectors(sparse), for example if you to store them in a Vector DB.
         """
         for idx in range(len(self.doc_freqs)):
-            yield self.document_vector(idx)
+            yield self.encode_document(idx)
+
+    def encode_query(self, query: list[str]) -> SparseVector:
+        return {self.ftoi[f]: 1. for f in query if f in self.features_}
 
-    def encode_query(self, query: list[str]) -> list[float]:
-        return [1 if f in query else 0 for f in self.features_]
+    def encode_query_dense(self, query: list[str]) -> list[float]:
+        return [1. if f in query else 0. for f in self.features_]
 
     def get_embeddings(self) -> np.ndarray:
         """This should be used only if the index is relatively small.
         """
         matrix = np.zeros(shape=(len(self.doc_len), len(self.idf)))  # numdocs rows and num words cols
         doc_len = np.asarray(self.doc_len)
         for idx, word in enumerate(self.features_):
```

### Comparing `yeabm25-0.1.1/src/yeabm25.egg-info/PKG-INFO` & `yeabm25-0.1.2/src/yeabm25.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yeabm25
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet Another BM25 algorithm implementation with update method, so that you dont need to fit on old + new documents.
 Author-email: Demir Tonchev <{surname}.{name}@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -252,15 +252,15 @@
 assert yeabm.doc_len == bm_update.doc_len
 assert yeabm.average_idf == bm_update.average_idf
 assert yeabm.idf == bm_update.idf
 assert yeabm.get_scores(['fox', 'jump']) == bm_update.get_scores(['fox', 'jump'])).all()
 ```
 
 This work is inspired(and uses some code and ideas) by this great package - https://github.com/dorianbrown/rank_bm25/tree/master.
-The main focus is creating document and query vectors (sparse vectors support - soon(hopefully not "Blizzard soon")). Then using the vectors with your favourite Vector DB.
+The main focus is creating document and query vectors (supports sparse vectors). Then using the vectors with your favourite Vector DB.
 
 How to get the document and query vectors: 
 ```python
 # recommended approach for large corpus, returns iterator. Each element is list[float]
 # returns generator object
 yeabm.iter_document_vectors()
 # use it
```

### Comparing `yeabm25-0.1.1/tests/test_yeabm25.py` & `yeabm25-0.1.2/tests/test_yeabm25.py`

 * *Files identical despite different names*

