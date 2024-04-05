# Comparing `tmp/prefixmaps-0.2.2.tar.gz` & `tmp/prefixmaps-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefixmaps-0.2.2.tar", max compression
+gzip compressed data, was "prefixmaps-0.2.3.tar", max compression
```

## Comparing `prefixmaps-0.2.2.tar` & `prefixmaps-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11356 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/LICENSE
--rw-r--r--   0        0        0     6238 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/README.md
--rw-r--r--   0        0        0     1696 2024-02-16 21:16:56.176173 prefixmaps-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      441 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/src/prefixmaps/__init__.py
--rw-r--r--   0        0        0      273 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/src/prefixmaps/data/__init__.py
--rw-r--r--   0        0        0    34630 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/src/prefixmaps/data/bioportal.csv
--rw-r--r--   0        0        0    25666 2024-02-16 21:16:41.764217 prefixmaps-0.2.2/src/prefixmaps/data/bioportal.curated.yaml
--rw-r--r--   0        0        0   983368 2024-02-16 21:16:41.768218 prefixmaps-0.2.2/src/prefixmaps/data/bioregistry.csv
--rw-r--r--   0        0        0   983368 2024-02-16 21:16:41.772218 prefixmaps-0.2.2/src/prefixmaps/data/bioregistry.upper.csv
--rw-r--r--   0        0        0     1688 2024-02-16 21:16:41.772218 prefixmaps-0.2.2/src/prefixmaps/data/contexts.curated.yaml
--rw-r--r--   0        0        0     3248 2024-02-16 21:16:41.772218 prefixmaps-0.2.2/src/prefixmaps/data/go.csv
--rw-r--r--   0        0        0     1184 2024-02-16 21:16:41.772218 prefixmaps-0.2.2/src/prefixmaps/data/linked_data.csv
--rw-r--r--   0        0        0      859 2024-02-16 21:16:41.772218 prefixmaps-0.2.2/src/prefixmaps/data/linked_data.curated.yaml
--rw-r--r--   0        0        0  1268584 2024-02-16 21:16:41.776218 prefixmaps-0.2.2/src/prefixmaps/data/merged.csv
--rw-r--r--   0        0        0  1401752 2024-02-16 21:16:41.780218 prefixmaps-0.2.2/src/prefixmaps/data/merged.monarch.csv
--rw-r--r--   0        0        0  1335168 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/data/merged.oak.csv
--rw-r--r--   0        0        0    14760 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/data/obo.csv
--rw-r--r--   0        0        0   189720 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/data/prefixcc.csv
--rw-r--r--   0        0        0    59629 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/data/w3id.csv
--rw-r--r--   0        0        0        0 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/datamodel/__init__.py
--rw-r--r--   0        0        0    12603 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/datamodel/context.py
--rw-r--r--   0        0        0        0 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/ingest/__init__.py
--rw-r--r--   0        0        0     3553 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/ingest/etl_runner.py
--rw-r--r--   0        0        0     1586 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_bioportal.py
--rw-r--r--   0        0        0     3349 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_bioregistry.py
--rwxr-xr-x   0        0        0     1020 2024-02-16 21:16:41.784218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_go.py
--rw-r--r--   0        0        0     2732 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_jsonld.py
--rw-r--r--   0        0        0     1066 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_linkml.py
--rw-r--r--   0        0        0     1838 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_shacl.py
--rw-r--r--   0        0        0      839 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_w3id.py
--rw-r--r--   0        0        0        0 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/io/__init__.py
--rw-r--r--   0        0        0     2416 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/io/parser.py
--rw-r--r--   0        0        0     1300 2024-02-16 21:16:41.788218 prefixmaps-0.2.2/src/prefixmaps/io/writer.py
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 prefixmaps-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6238 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/README.md
+-rw-r--r--   0        0        0     1696 2024-04-05 13:46:46.573206 prefixmaps-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      441 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/src/prefixmaps/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/src/prefixmaps/data/__init__.py
+-rw-r--r--   0        0        0    34630 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/src/prefixmaps/data/bioportal.csv
+-rw-r--r--   0        0        0    25666 2024-04-05 13:46:31.581235 prefixmaps-0.2.3/src/prefixmaps/data/bioportal.curated.yaml
+-rw-r--r--   0        0        0   983368 2024-04-05 13:46:31.585235 prefixmaps-0.2.3/src/prefixmaps/data/bioregistry.csv
+-rw-r--r--   0        0        0   983368 2024-04-05 13:46:31.589235 prefixmaps-0.2.3/src/prefixmaps/data/bioregistry.upper.csv
+-rw-r--r--   0        0        0     1688 2024-04-05 13:46:31.589235 prefixmaps-0.2.3/src/prefixmaps/data/contexts.curated.yaml
+-rw-r--r--   0        0        0     3248 2024-04-05 13:46:31.589235 prefixmaps-0.2.3/src/prefixmaps/data/go.csv
+-rw-r--r--   0        0        0     1184 2024-04-05 13:46:31.589235 prefixmaps-0.2.3/src/prefixmaps/data/linked_data.csv
+-rw-r--r--   0        0        0      859 2024-04-05 13:46:31.589235 prefixmaps-0.2.3/src/prefixmaps/data/linked_data.curated.yaml
+-rw-r--r--   0        0        0  1268584 2024-04-05 13:46:31.593235 prefixmaps-0.2.3/src/prefixmaps/data/merged.csv
+-rw-r--r--   0        0        0  1401752 2024-04-05 13:46:31.597235 prefixmaps-0.2.3/src/prefixmaps/data/merged.monarch.csv
+-rw-r--r--   0        0        0  1335168 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/data/merged.oak.csv
+-rw-r--r--   0        0        0    14760 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/data/obo.csv
+-rw-r--r--   0        0        0   189720 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/data/prefixcc.csv
+-rw-r--r--   0        0        0    59629 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/data/w3id.csv
+-rw-r--r--   0        0        0        0 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/datamodel/__init__.py
+-rw-r--r--   0        0        0    14446 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/datamodel/context.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/__init__.py
+-rw-r--r--   0        0        0     3553 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/etl_runner.py
+-rw-r--r--   0        0        0     1586 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_bioportal.py
+-rw-r--r--   0        0        0     3349 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_bioregistry.py
+-rwxr-xr-x   0        0        0     1020 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_go.py
+-rw-r--r--   0        0        0     2732 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_jsonld.py
+-rw-r--r--   0        0        0     1066 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_linkml.py
+-rw-r--r--   0        0        0     1838 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_shacl.py
+-rw-r--r--   0        0        0      839 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_w3id.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/io/__init__.py
+-rw-r--r--   0        0        0     2416 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/io/parser.py
+-rw-r--r--   0        0        0     1300 2024-04-05 13:46:31.601235 prefixmaps-0.2.3/src/prefixmaps/io/writer.py
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 prefixmaps-0.2.3/PKG-INFO
```

### Comparing `prefixmaps-0.2.2/LICENSE` & `prefixmaps-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/README.md` & `prefixmaps-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/pyproject.toml` & `prefixmaps-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefixmaps"
-version = "0.2.2"
+version = "0.2.3"
 description = "A python library for retrieving semantic prefix maps"
 readme = "README.md"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 keywords = ["semantic web", "bioinformatics"]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/bioportal.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/bioportal.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/bioportal.curated.yaml` & `prefixmaps-0.2.3/src/prefixmaps/data/bioportal.curated.yaml`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/bioregistry.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/bioregistry.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/bioregistry.upper.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/bioregistry.upper.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/contexts.curated.yaml` & `prefixmaps-0.2.3/src/prefixmaps/data/contexts.curated.yaml`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/go.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/go.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/linked_data.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/linked_data.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/linked_data.curated.yaml` & `prefixmaps-0.2.3/src/prefixmaps/data/linked_data.curated.yaml`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/merged.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/merged.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/merged.monarch.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/merged.monarch.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/merged.oak.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/merged.oak.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/obo.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/obo.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/prefixcc.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/prefixcc.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/data/w3id.csv` & `prefixmaps-0.2.3/src/prefixmaps/data/w3id.csv`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/datamodel/context.py` & `prefixmaps-0.2.3/src/prefixmaps/datamodel/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Classes for managing individual Contexts."""
 
 import logging
 import re
 from collections import defaultdict
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import List, Mapping, Optional
+from typing import List, Mapping, Optional, Set, Union
 
 import curies
 
 __all__ = [
     "StatusType",
     "PrefixExpansion",
     "Context",
@@ -139,14 +139,22 @@
     """Optional comments on the context."""
 
     location: Optional[str] = None
     format: Optional[str] = None
     merged_from: Optional[List[str]] = None
     upper: bool = None
     lower: bool = None
+    _prefixes: Set[str] = field(default_factory=set)
+    """Private attr to speed up duplicate lookups"""
+    _prefixes_lower: Set[str] = field(default_factory=set)
+    """Private attr to speed up duplicate lookups"""
+    _namespaces: Set[str] = field(default_factory=set)
+    """Private attr to speed up duplicate lookups"""
+    _namespaces_lower: Set[str] = field(default_factory=set)
+    """Private attr to speed up duplicate lookups"""
 
     def combine(self, context: "Context"):
         """
         Merge a context into this one.
 
         If there are conflicts, the current context takes precedence,
         and the merged expansions are marked as non-canonical
@@ -160,14 +168,15 @@
     def add_prefix(
         self,
         prefix: PREFIX,
         namespace: NAMESPACE,
         status: StatusType = StatusType.canonical,
         preferred: bool = False,
         expansion_source: Optional[str] = None,
+        force: bool = False,
     ):
         """
         Adds a prefix expansion to this context.
 
         The current context stays canonical. Additional prefixes
         added may be classified as non-canonical.
 
@@ -178,44 +187,51 @@
         :param prefix: prefix to be added
         :param namespace: namespace to be added
         :param status: the status of the prefix being added
         :param preferred:
         :param expansion_source: An optional annotation to be used when merging contexts together.
             The source will keep track of the original context that a given prefix
             expansion came from. This is used in :meth:`Context.combine`.
+        :param force: if True, recompute namespaces and prefixes. default False.
         :return:
         """
         # TODO: check status
+        _prefix = prefix
         if not preferred:
             if self.upper:
                 prefix = prefix.upper()
                 if self.lower:
                     raise ValueError("Cannot set both upper AND lower")
             if self.lower:
                 prefix = prefix.lower()
-        prefixes = self.prefixes(lower=True)
-        namespaces = self.namespaces(lower=True)
+        prefixes = self.prefixes(lower=True, force=force, as_list=False)
+        namespaces = self.namespaces(lower=True, force=force, as_list=False)
         if prefix.lower() in prefixes:
             if namespace.lower() in namespaces:
                 return
                 # status = StatusType.multi_alias
             else:
                 status = StatusType.prefix_alias
         else:
             if namespace.lower() in namespaces:
                 status = StatusType.namespace_alias
+
         self.prefix_expansions.append(
             PrefixExpansion(
                 context=self.name,
                 prefix=prefix,
                 namespace=namespace,
                 status=status,
                 expansion_source=expansion_source,
             )
         )
+        self._prefixes.add(_prefix)
+        self._prefixes_lower.add(prefix.lower())
+        self._namespaces.add(namespace)
+        self._namespaces_lower.add(namespace.lower())
 
     def filter(self, prefix: PREFIX = None, namespace: NAMESPACE = None):
         """
         Returns namespaces matching query.
 
         :param prefix:
         :param namespace:
@@ -226,37 +242,65 @@
             if prefix is not None and prefix != pe.prefix:
                 continue
             if namespace is not None and namespace != pe.namespace:
                 continue
             filtered_pes.append(pe)
         return filtered_pes
 
-    def prefixes(self, lower=False) -> List[str]:
+    def prefixes(
+        self, lower=False, force: bool = True, as_list: bool = True
+    ) -> Union[List[str], Set[str]]:
         """
         All unique prefixes in all prefix expansions.
 
         :param lower: if True, the prefix is normalized to lowercase.
+        :param force: if True, recompute. if False, return cached
+        :param as_list: if True (default), return as a list. Otherwise a set
         :return:
         """
         if lower:
-            return list({pe.prefix.lower() for pe in self.prefix_expansions})
+            if force or len(self._prefixes_lower) == 0:
+                self._prefixes_lower = {pe.prefix.lower() for pe in self.prefix_expansions}
+            res = self._prefixes_lower
+
+        else:
+            if force or len(self._prefixes) == 0:
+                self._prefixes = {pe.prefix for pe in self.prefix_expansions}
+            res = self._prefixes
+
+        if as_list:
+            return list(res)
         else:
-            return list({pe.prefix for pe in self.prefix_expansions})
+            return res
 
-    def namespaces(self, lower=False) -> List[str]:
+    def namespaces(
+        self, lower=False, force: bool = True, as_list: bool = True
+    ) -> Union[List[str], Set[str]]:
         """
         All unique namespaces in all prefix expansions
 
         :param lower: if True, the namespace is normalized to lowercase.
+        :param force: if True, recompute. if False, return cached
+        :param as_list: if True (default), return as a list. Otherwise a set
         :return:
         """
         if lower:
-            return list({pe.namespace.lower() for pe in self.prefix_expansions})
+            if force or len(self._namespaces_lower) == 0:
+                self._namespaces_lower = {pe.namespace.lower() for pe in self.prefix_expansions}
+            res = self._namespaces_lower
+
+        else:
+            if force or len(self._namespaces) == 0:
+                self._namespaces = {pe.namespace for pe in self.prefix_expansions}
+            res = self._namespaces
+
+        if as_list:
+            return list(res)
         else:
-            return list({pe.namespace for pe in self.prefix_expansions})
+            return res
 
     def as_dict(self) -> PREFIX_EXPANSION_DICT:
         """
         Returns a mapping between canonical prefixes and expansions.
 
         This only includes canonical expansions. The results can be safely used
         in the header of RDF syntax documents.
```

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/etl_runner.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/etl_runner.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_bioportal.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_bioportal.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_bioregistry.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_bioregistry.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_go.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_go.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_jsonld.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_jsonld.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_linkml.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_linkml.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_shacl.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_shacl.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/ingest/ingest_w3id.py` & `prefixmaps-0.2.3/src/prefixmaps/ingest/ingest_w3id.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/io/parser.py` & `prefixmaps-0.2.3/src/prefixmaps/io/parser.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/src/prefixmaps/io/writer.py` & `prefixmaps-0.2.3/src/prefixmaps/io/writer.py`

 * *Files identical despite different names*

### Comparing `prefixmaps-0.2.2/PKG-INFO` & `prefixmaps-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefixmaps
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python library for retrieving semantic prefix maps
 License: Apache-2.0
 Keywords: semantic web,bioinformatics
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
```

