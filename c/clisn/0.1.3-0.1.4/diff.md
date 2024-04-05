# Comparing `tmp/clisn-0.1.3.tar.gz` & `tmp/clisn-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clisn-0.1.3.tar", max compression
+gzip compressed data, was "clisn-0.1.4.tar", max compression
```

## Comparing `clisn-0.1.3.tar` & `clisn-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-08-07 07:22:06.852172 clisn-0.1.3/LICENSE
--rw-r--r--   0        0        0     2254 2023-08-09 05:30:51.624198 clisn-0.1.3/README.md
--rw-r--r--   0        0        0       82 2023-08-08 15:01:04.465348 clisn-0.1.3/clisn/__init__.py
--rw-r--r--   0        0        0      948 2023-08-11 04:32:44.425605 clisn-0.1.3/clisn/manager.py
--rw-r--r--   0        0        0      885 2023-12-04 15:45:47.717906 clisn-0.1.3/clisn/namespaces.py
--rw-r--r--   0        0        0      275 2023-12-04 15:47:42.118100 clisn-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 clisn-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-07 07:22:06.852172 clisn-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2254 2023-08-09 05:30:51.624198 clisn-0.1.4/README.md
+-rw-r--r--   0        0        0       82 2023-08-08 15:01:04.465348 clisn-0.1.4/clisn/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-11 04:32:44.425605 clisn-0.1.4/clisn/manager.py
+-rw-r--r--   0        0        0      821 2024-04-05 10:09:47.970093 clisn-0.1.4/clisn/namespaces.py
+-rw-r--r--   0        0        0      275 2024-04-05 10:12:28.834638 clisn-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 clisn-0.1.4/PKG-INFO
```

### Comparing `clisn-0.1.3/LICENSE` & `clisn-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clisn-0.1.3/README.md` & `clisn-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `clisn-0.1.3/clisn/manager.py` & `clisn-0.1.4/clisn/manager.py`

 * *Files identical despite different names*

### Comparing `clisn-0.1.3/clisn/namespaces.py` & `clisn-0.1.4/clisn/namespaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from rdflib import Graph, Namespace
 
 
 # namespaces
 crm = Namespace("http://www.cidoc-crm.org/cidoc-crm/")
 crmcls = Namespace("https://clscor.io/ontologies/CRMcls/")
-# clst = Namespace("https://core.clscor.io/entity/type/")
-# clscore = Namespace("https://core.clscor.io/entity/")
+clscore = Namespace("https://clscor.io/entity/")
+
 frbroo = Namespace("http://iflastandards.info/ns/fr/frbr/frbroo/")
 crmdig = Namespace("http://www.ics.forth.gr/isl/CRMdig/")
 lrm = Namespace("http://iflastandards.info/ns/lrm/lrmoo/")
 pem = Namespace("http://parthenos.d4science.org/CRMext/CRMpe.rdfs")
 
 
 def corpus_base(corpus_key: str) -> Namespace:
```

### Comparing `clisn-0.1.3/PKG-INFO` & `clisn-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clisn
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
```

