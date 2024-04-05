# Comparing `tmp/puggle-0.2.8.tar.gz` & `tmp/puggle-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puggle-0.2.8.tar", max compression
+gzip compressed data, was "puggle-0.2.9.tar", max compression
```

## Comparing `puggle-0.2.8.tar` & `puggle-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      122 2023-10-31 12:59:01.551828 puggle-0.2.8/puggle/__init__.py
--rw-r--r--   0        0        0     7035 2023-11-07 07:02:24.185805 puggle-0.2.8/puggle/Annotation.py
--rw-r--r--   0        0        0      254 2023-10-31 12:59:01.551828 puggle-0.2.8/puggle/data_utils/__init__.py
--rw-r--r--   0        0        0     4783 2023-11-01 14:21:39.660465 puggle-0.2.8/puggle/data_utils/manipulation.py
--rw-r--r--   0        0        0     9234 2023-11-07 06:37:42.417507 puggle-0.2.8/puggle/data_utils/sampling.py
--rw-r--r--   0        0        0     1700 2023-11-01 14:12:19.873347 puggle-0.2.8/puggle/data_utils/statistics.py
--rw-r--r--   0        0        0    18316 2023-11-19 11:41:56.330812 puggle-0.2.8/puggle/Dataset.py
--rw-r--r--   0        0        0     1201 2023-11-01 14:09:05.981425 puggle-0.2.8/puggle/Document.py
--rw-r--r--   0        0        0      211 2023-10-31 12:59:01.552828 puggle-0.2.8/puggle/logger.py
--rw-r--r--   0        0        0     1603 2023-11-07 07:02:06.987375 puggle-0.2.8/puggle/Mention.py
--rw-r--r--   0        0        0     1544 2023-11-01 14:19:17.774357 puggle-0.2.8/puggle/Relation.py
--rw-r--r--   0        0        0      271 2023-11-19 06:48:01.385057 puggle-0.2.8/puggle/size_limits.py
--rw-r--r--   0        0        0     2344 2023-11-01 14:20:41.472423 puggle-0.2.8/puggle/utils.py
--rw-r--r--   0        0        0      510 2023-11-19 11:42:09.842595 puggle-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1494 2023-11-01 08:34:22.311356 puggle-0.2.8/README.md
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 puggle-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      122 2023-10-31 12:59:01.551828 puggle-0.2.9/puggle/__init__.py
+-rw-r--r--   0        0        0     7035 2023-11-07 07:02:24.185805 puggle-0.2.9/puggle/Annotation.py
+-rw-r--r--   0        0        0      254 2023-10-31 12:59:01.551828 puggle-0.2.9/puggle/data_utils/__init__.py
+-rw-r--r--   0        0        0     4783 2023-11-01 14:21:39.660465 puggle-0.2.9/puggle/data_utils/manipulation.py
+-rw-r--r--   0        0        0     9234 2023-11-07 06:37:42.417507 puggle-0.2.9/puggle/data_utils/sampling.py
+-rw-r--r--   0        0        0     1700 2023-11-01 14:12:19.873347 puggle-0.2.9/puggle/data_utils/statistics.py
+-rw-r--r--   0        0        0    18378 2023-11-20 08:12:13.951786 puggle-0.2.9/puggle/Dataset.py
+-rw-r--r--   0        0        0     1201 2023-11-01 14:09:05.981425 puggle-0.2.9/puggle/Document.py
+-rw-r--r--   0        0        0      211 2023-10-31 12:59:01.552828 puggle-0.2.9/puggle/logger.py
+-rw-r--r--   0        0        0     1603 2023-11-07 07:02:06.987375 puggle-0.2.9/puggle/Mention.py
+-rw-r--r--   0        0        0     1544 2023-11-01 14:19:17.774357 puggle-0.2.9/puggle/Relation.py
+-rw-r--r--   0        0        0      271 2023-11-19 06:48:01.385057 puggle-0.2.9/puggle/size_limits.py
+-rw-r--r--   0        0        0     2344 2023-11-01 14:20:41.472423 puggle-0.2.9/puggle/utils.py
+-rw-r--r--   0        0        0      510 2023-11-20 08:12:23.115809 puggle-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-11-01 08:34:22.311356 puggle-0.2.9/README.md
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 puggle-0.2.9/PKG-INFO
```

### Comparing `puggle-0.2.8/puggle/Annotation.py` & `puggle-0.2.9/puggle/Annotation.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/data_utils/manipulation.py` & `puggle-0.2.9/puggle/data_utils/manipulation.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/data_utils/sampling.py` & `puggle-0.2.9/puggle/data_utils/sampling.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/data_utils/statistics.py` & `puggle-0.2.9/puggle/data_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/Dataset.py` & `puggle-0.2.9/puggle/Dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,15 @@
                 e2_idx = ent_idxs[
                     tuple([rel.end.label, " ".join(rel.end.tokens)])
                 ]
 
                 rels.add(
                     tuple(
                         [
+                            i,
                             e1_idx,
                             e2_idx,
                             rel.start.label,
                             " ".join(rel.start.tokens),
                             rel.end.label,
                             " ".join(rel.end.tokens),
                             rel.label,
@@ -294,14 +295,15 @@
                 "Saved %d entities to %s." % (len(ents), entities_path)
             )
 
         with open(relations_path, "w", newline="", encoding="utf-8") as f:
             writer = csv.writer(f)
             writer.writerow(
                 [
+                    "doc_idx",
                     "rel_idx",
                     "e1_idx",
                     "e2_idx",
                     "e1_label",
                     "e1_tokens",
                     "e2_label",
                     "e2_tokens",
```

### Comparing `puggle-0.2.8/puggle/Document.py` & `puggle-0.2.9/puggle/Document.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/Mention.py` & `puggle-0.2.9/puggle/Mention.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/Relation.py` & `puggle-0.2.9/puggle/Relation.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/puggle/utils.py` & `puggle-0.2.9/puggle/utils.py`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/README.md` & `puggle-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `puggle-0.2.8/PKG-INFO` & `puggle-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puggle
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Michael Stewart
 Author-email: michael.stewart.webdev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: puggle Version: 0.2.8 Summary: Author: Michael
+Metadata-Version: 2.1 Name: puggle Version: 0.2.9 Summary: Author: Michael
 Stewart Author-email: michael.stewart.webdev@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: colorama (>=0.4.6,<0.5.0) Requires-Dist: loguru
 (>=0.7.2,<0.8.0) Requires-Dist: py2neo (>=2021.2.4,<2022.0.0) Requires-Dist:
 python-dotenv (>=1.0.0,<2.0.0) Description-Content-Type: text/markdown # Puggle
 [![Pytest Status](https://github.com/nlp-tlp/puggle/actions/workflows/run-
```

