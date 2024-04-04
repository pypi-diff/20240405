# Comparing `tmp/typer_cli-0.12.dev1.tar.gz` & `tmp/typer_cli-0.12.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_cli-0.12.dev1.tar", last modified: Sat Mar 30 01:34:13 2024, max compression
+gzip compressed data, was "typer_cli-0.12.dev2.tar", last modified: Sat Mar 30 01:51:47 2024, max compression
```

## Comparing `typer_cli-0.12.dev1.tar` & `typer_cli-0.12.dev2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2024-03-30 01:34:13.729591 typer_cli-0.12.dev1/LICENSE
--rw-r--r--   0        0        0     2056 2024-03-30 01:34:11.041577 typer_cli-0.12.dev1/README.md
--rw-r--r--   0        0        0     1237 2024-03-30 01:34:11.041577 typer_cli-0.12.dev1/pdm_build.py
--rw-r--r--   0        0        0     1646 2024-03-30 01:34:13.729591 typer_cli-0.12.dev1/pyproject.toml
--rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 typer_cli-0.12.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-30 01:51:47.541010 typer_cli-0.12.dev2/LICENSE
+-rw-r--r--   0        0        0     2056 2024-03-30 01:51:42.084978 typer_cli-0.12.dev2/README.md
+-rw-r--r--   0        0        0     1237 2024-03-30 01:51:42.084978 typer_cli-0.12.dev2/pdm_build.py
+-rw-r--r--   0        0        0     1646 2024-03-30 01:51:47.541010 typer_cli-0.12.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 typer_cli-0.12.dev2/PKG-INFO
```

### Comparing `typer_cli-0.12.dev1/LICENSE` & `typer_cli-0.12.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_cli-0.12.dev1/README.md` & `typer_cli-0.12.dev2/README.md`

 * *Files identical despite different names*

### Comparing `typer_cli-0.12.dev1/pdm_build.py` & `typer_cli-0.12.dev2/pdm_build.py`

 * *Files identical despite different names*

### Comparing `typer_cli-0.12.dev1/pyproject.toml` & `typer_cli-0.12.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "typer-slim[standard]==0.12.dev1",
+    "typer-slim[standard]==0.12.dev2",
 ]
-version = "0.12.dev1"
+version = "0.12.dev2"
 
 [project.urls]
 Documentation = "https://typer.tiangolo.com/"
 homepage = "https://github.com/tiangolo/typer"
 
 [project.optional-dependencies]
 all = []
```

### Comparing `typer_cli-0.12.dev1/PKG-INFO` & `typer_cli-0.12.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-cli
-Version: 0.12.dev1
+Version: 0.12.dev2
 Summary: Typer, build great CLIs. Easy to code. Based on Python type hints.
 Home-page: https://github.com/tiangolo/typer
 Author-Email: Sebastián Ramírez <tiangolo@gmail.com>
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://typer.tiangolo.com/
 Project-URL: Homepage, https://github.com/tiangolo/typer
 Requires-Python: >=3.7
-Requires-Dist: typer-slim[standard]==0.12.dev1
+Requires-Dist: typer-slim[standard]==0.12.dev2
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://typer.tiangolo.com"><img src="https://typer.tiangolo.com/img/logo-margin/logo-margin-vector.svg" alt="Typer"></a>
 </p>
 <p align="center">
     <em>Typer, build great CLIs. Easy to code. Based on Python type hints.</em>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: typer-cli Version: 0.12.dev1 Summary: Typer, build
+Metadata-Version: 2.1 Name: typer-cli Version: 0.12.dev2 Summary: Typer, build
 great CLIs. Easy to code. Based on Python type hints. Home-page: https://
 github.com/tiangolo/typer Author-Email: SebastiÃ¡n RamÃ­rez
 gmail.com> Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
@@ -12,15 +12,15 @@
 Developers Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Project-URL:
 Documentation, https://typer.tiangolo.com/ Project-URL: Homepage, https://
 github.com/tiangolo/typer Requires-Python: >=3.7 Requires-Dist: typer-slim
-[standard]==0.12.dev1 Description-Content-Type: text/markdown
+[standard]==0.12.dev2 Description-Content-Type: text/markdown
                                     _[_T_y_p_e_r_]
       TTyyppeerr,, bbuuiilldd ggrreeaatt CCLLIIss.. EEaassyy ttoo ccooddee.. BBaasseedd oonn PPyytthhoonn ttyyppee hhiinnttss..
                   _[_T_e_s_t_]_[_P_u_b_l_i_s_h_]_[_C_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_t_y_p_e_r_._t_i_a_n_g_o_l_o_._c_o_m_/_t_u_t_o_r_i_a_l_/_t_y_p_e_r_-_c_o_m_m_a_n_d_/
 **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_i_a_n_g_o_l_o_/_t_y_p_e_r --- Typer is a library for
 building CLI applications that users will **love using** and developers will
 **love creating**. Based on Python type hints. ## Typer CLI This package,
```

