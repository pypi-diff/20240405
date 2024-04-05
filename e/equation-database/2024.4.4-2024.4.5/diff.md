# Comparing `tmp/equation_database-2024.4.4.tar.gz` & `tmp/equation_database-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equation_database-2024.4.4.tar", max compression
+gzip compressed data, was "equation_database-2024.4.5.tar", max compression
```

## Comparing `equation_database-2024.4.4.tar` & `equation_database-2024.4.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       20 2024-03-30 21:01:48.299405 equation_database-2024.4.4/README.md
--rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.4.4/equation_database/__init__.py
--rw-r--r--   0        0        0     2016 2024-03-30 22:29:25.673432 equation_database-2024.4.4/equation_database/arxiv_2202_13416/__init__.py
--rw-r--r--   0        0        0     1129 2024-03-30 22:29:25.673432 equation_database-2024.4.4/equation_database/doi_10_1103_physrev_176_1700/__init__.py
--rw-r--r--   0        0        0      860 2024-04-04 08:12:03.884020 equation_database-2024.4.4/equation_database/isbn_9780201483628/__init__.py
--rw-r--r--   0        0        0      718 2024-03-31 16:08:15.816482 equation_database-2024.4.4/equation_database/isbn_9780471887416/__init__.py
--rw-r--r--   0        0        0     2869 2024-04-04 08:12:03.884020 equation_database-2024.4.4/equation_database/isbn_9780511628788/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.4.4/equation_database/util/__init__.py
--rw-r--r--   0        0        0      160 2024-03-30 22:29:25.673432 equation_database-2024.4.4/equation_database/util/parse.py
--rw-r--r--   0        0        0      215 2024-03-30 21:01:48.299405 equation_database-2024.4.4/equation_database/util/test.py
--rw-r--r--   0        0        0     1208 2024-04-04 08:12:47.808025 equation_database-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 equation_database-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-03-30 21:01:48.299405 equation_database-2024.4.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.4.5/equation_database/__init__.py
+-rw-r--r--   0        0        0     2016 2024-03-30 22:29:25.673432 equation_database-2024.4.5/equation_database/arxiv_2202_13416/__init__.py
+-rw-r--r--   0        0        0     1142 2024-04-05 12:09:26.447246 equation_database-2024.4.5/equation_database/doi_10_1103_PhysRevD_16_3251/__init__.py
+-rw-r--r--   0        0        0     1129 2024-03-30 22:29:25.673432 equation_database-2024.4.5/equation_database/doi_10_1103_physrev_176_1700/__init__.py
+-rw-r--r--   0        0        0     1712 2024-04-05 11:57:50.190922 equation_database-2024.4.5/equation_database/isbn_9780201483628/__init__.py
+-rw-r--r--   0        0        0     1129 2024-04-04 12:45:37.722905 equation_database-2024.4.5/equation_database/isbn_9780471887416/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-05 11:11:10.688889 equation_database-2024.4.5/equation_database/isbn_9780511628788/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.4.5/equation_database/util/__init__.py
+-rw-r--r--   0        0        0      160 2024-03-30 22:29:25.673432 equation_database-2024.4.5/equation_database/util/parse.py
+-rw-r--r--   0        0        0      215 2024-03-30 21:01:48.299405 equation_database-2024.4.5/equation_database/util/test.py
+-rw-r--r--   0        0        0     1208 2024-04-05 12:22:25.721447 equation_database-2024.4.5/pyproject.toml
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 equation_database-2024.4.5/PKG-INFO
```

### Comparing `equation_database-2024.4.4/equation_database/arxiv_2202_13416/__init__.py` & `equation_database-2024.4.5/equation_database/arxiv_2202_13416/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.4.4/equation_database/doi_10_1103_physrev_176_1700/__init__.py` & `equation_database-2024.4.5/equation_database/doi_10_1103_physrev_176_1700/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.4.4/equation_database/isbn_9780471887416/__init__.py` & `equation_database-2024.4.5/equation_database/isbn_9780471887416/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,26 @@
 """unpolarized e-mu- -> e-mu- scattering amplitude"""
 equation_6_31 = 2*e**4 * (t**2 + u **2)/s**2
 """unpolarized e-e+ -> mu-mu+ scattering amplitude"""
 
 equation_6_113 = 2*e**4 * (- u/s - s/u)
 """spin averaged Compton amplitude"""
 
+N = sympy.Symbol('N')
+"""Normalization factor"""
+x_q = sympy.Symbol('x_q')
+"""Quark momentum fraction"""
+x_qbar = sympy.Symbol('x_qbar')
+"""Antiquark momentum fraction"""
+x_g = sympy.Symbol('x_g')
+"""Gluon momentum fraction"""
+
+equation_11_35 = N * (x_q**2 + x_qbar**2)/((1-x_q)*(1-x_qbar))
+"""spin and color averaged matrix element for electron-positron annihilation into quark-antiquark-gluon final state"""
+
 bibtex : str = """
 @book{Halzen:1984mc,
     author = "Halzen, F. and Martin, Alan D.",
     title = "{QUARKS AND LEPTONS: AN INTRODUCTORY COURSE IN MODERN PARTICLE PHYSICS}",
     isbn = "978-0-471-88741-6",
     year = "1984"
 }
```

### Comparing `equation_database-2024.4.4/equation_database/isbn_9780511628788/__init__.py` & `equation_database-2024.4.5/equation_database/isbn_9780511628788/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 
 table_7_2 = {
     "quark_quarkbar_to_gammastar_gluon" :  (N**2-1)/N**2 * (t**2+u**2 + 2*s * (s+t+u))/(t*u),
     "gluon_quark_to_gammastar_quark"     : - 1/N * (s**2 + u**2 + s*t*(s+t+u)/(s*u)),
 }
 """Lowest order processes for virtual photon production. The colour and spin indices are averaged (summed) over initial (final) states. For a real photon (s +1 + u) = 0 and for SU(3) we have N = 3"""
 
+# Backwards compatibility
+table_7_1_qqp_qqp =  table_7_1["quark_quarkprime_to_quark_quarkprime"]
+table_7_1_qqpb_qqpb = table_7_1["quark_quarkprimebar_to_quark_quarkprimebar"]
+table_7_1_qq_qq = table_7_1["quark_quark_to_quark_quark"]
+table_7_1_qqb_qpqpb = table_7_1["quark_quarkbar_to_quarkprime_quarkprimebar"]
+table_7_1_qqb_qqb = table_7_1["quark_quarkbar_to_quark_quarkbar"]
+table_7_1_qqb_gg = table_7_1["quark_quarkbar_to_gluon_gluon"]
+table_7_1_gg_qqb = table_7_1["gluon_gluon_to_quark_quarkbar"]
+table_7_1_gq_gq = table_7_1 ["gluon_quark_to_gluon_quark"]
+table_7_1_gg_gg = table_7_1["gluon_gluon_to_gluon_gluon"]
+
 bibtex : str = """
 @book{Ellis:1996mzs,
     author = "Ellis, R. Keith and Stirling, W. James and Webber, B. R.",
     title = "{QCD and collider physics}",
     doi = "10.1017/CBO9780511628788",
     isbn = "978-0-511-82328-2, 978-0-521-54589-1",
     publisher = "Cambridge University Press",
     volume = "8",
     month = "2",
     year = "2011"
 }
 """
-
-# Backward compatibility
-table_7_1_qqp_qqp =  table_7_1["quark_quarkprime_to_quark_quarkprime"]
-table_7_1_qqpb_qqpb = table_7_1["quark_quarkprimebar_to_quark_quarkprimebar"]
-table_7_1_qq_qq = table_7_1["quark_quark_to_quark_quark"]
-table_7_1_qqb_qpqpb = table_7_1["quark_quarkbar_to_quarkprime_quarkprimebar"]
-table_7_1_qqb_qqb = table_7_1["quark_quarkbar_to_quark_quarkbar"]
-table_7_1_qqb_gg = table_7_1["quark_quarkbar_to_gluon_gluon"]
-table_7_1_gg_qqb = table_7_1["gluon_gluon_to_quark_quarkbar"]
-table_7_1_gq_gq = table_7_1 ["gluon_quark_to_gluon_quark"]
-table_7_1_gg_gg = table_7_1["gluon_gluon_to_gluon_gluon"]
```

### Comparing `equation_database-2024.4.4/pyproject.toml` & `equation_database-2024.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "equation-database"
-version = "2024.4.4"
+version = "2024.4.5"
 description = "A collection of equations"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sympy = "*"
```

### Comparing `equation_database-2024.4.4/PKG-INFO` & `equation_database-2024.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-database
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: A collection of equations
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

