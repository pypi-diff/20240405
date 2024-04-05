# Comparing `tmp/myllm-4.7.7.tar.gz` & `tmp/myllm-4.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-4.7.7.tar", max compression
+gzip compressed data, was "myllm-4.7.8.tar", max compression
```

## Comparing `myllm-4.7.7.tar` & `myllm-4.7.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-03 06:10:03.433798 myllm-4.7.7/LICENSE
--rw-r--r--   0        0        0     3014 2024-04-03 06:10:03.433798 myllm-4.7.7/README.md
--rw-r--r--   0        0        0       95 2024-04-03 06:10:44.838284 myllm-4.7.7/myllm/__init__.py
--rw-r--r--   0        0        0      772 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/config.py
--rw-r--r--   0        0        0     3094 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/default_settings.toml
--rw-r--r--   0        0        0     7189 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/main.py
--rw-r--r--   0        0        0      117 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/client.py
--rw-r--r--   0        0        0     1996 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/g4f.py
--rw-r--r--   0        0        0     2212 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/gemini.py
--rw-r--r--   0        0        0     2078 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/openai.py
--rw-r--r--   0        0        0     2322 2024-04-03 06:10:03.437798 myllm-4.7.7/myllm/provider/petals.py
--rw-r--r--   0        0        0     3924 2024-04-03 06:10:44.834284 myllm-4.7.7/pyproject.toml
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-05 06:29:58.261690 myllm-4.7.8/LICENSE
+-rw-r--r--   0        0        0     3014 2024-04-05 06:29:58.261690 myllm-4.7.8/README.md
+-rw-r--r--   0        0        0       95 2024-04-05 06:30:39.357566 myllm-4.7.8/myllm/__init__.py
+-rw-r--r--   0        0        0      772 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/config.py
+-rw-r--r--   0        0        0     3094 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/default_settings.toml
+-rw-r--r--   0        0        0     7189 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/main.py
+-rw-r--r--   0        0        0      117 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/client.py
+-rw-r--r--   0        0        0     1996 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/g4f.py
+-rw-r--r--   0        0        0     2212 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/gemini.py
+-rw-r--r--   0        0        0     2078 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/openai.py
+-rw-r--r--   0        0        0     2322 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/petals.py
+-rw-r--r--   0        0        0     3926 2024-04-05 06:30:39.357566 myllm-4.7.8/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.7.8/PKG-INFO
```

### Comparing `myllm-4.7.7/LICENSE` & `myllm-4.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/README.md` & `myllm-4.7.8/README.md`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/config.py` & `myllm-4.7.8/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/default_settings.toml` & `myllm-4.7.8/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/main.py` & `myllm-4.7.8/myllm/main.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/provider/client.py` & `myllm-4.7.8/myllm/provider/client.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/provider/g4f.py` & `myllm-4.7.8/myllm/provider/g4f.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/provider/gemini.py` & `myllm-4.7.8/myllm/provider/gemini.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/provider/openai.py` & `myllm-4.7.8/myllm/provider/openai.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/myllm/provider/petals.py` & `myllm-4.7.8/myllm/provider/petals.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.7/pyproject.toml` & `myllm-4.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MyLLM"
-version = "4.7.7"
+version = "4.7.8"
 description = "A python package to interact with llm model supported by g4f and langchain."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
@@ -28,15 +28,15 @@
 loguru = ">=0.6.0"
 httpx = ">=0.24.1"
 g4f = "0.2.7.2"
 js2py = "^0.74"
 PyExecJS2="1.6.1"
 curl_cffi = "0.6.2"
 Brotli = "1.1.0"
-openai = "1.16.1"
+openai = "1.16.2"
 # petals = "2.2.0.post1"
 # transformers = "4.32"
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = ">=8.0.8"
 ruff = "^0.3.0"
@@ -163,27 +163,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `myllm-4.7.7/PKG-INFO` & `myllm-4.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyLLM
-Version: 4.7.7
+Version: 4.7.8
 Summary: A python package to interact with llm model supported by g4f and langchain.
 License: MIT
 Keywords: chatgpt,llm,ai,llama,ai,g4f,freegpt
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Requires-Dist: curl_cffi (==0.6.2)
 Requires-Dist: dynaconf (>=3.2.0)
 Requires-Dist: fastapi (>=0.95.2)
 Requires-Dist: g4f (==0.2.7.2)
 Requires-Dist: httpx (>=0.24.1)
 Requires-Dist: js2py (>=0.74,<0.75)
 Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: openai (==1.16.1)
+Requires-Dist: openai (==1.16.2)
 Requires-Dist: uvicorn (>=0.22.0)
 Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions
 Description-Content-Type: text/markdown
 
 <table style="border: 1px solid transparent">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: MyLLM Version: 4.7.7 Summary: A python package to
+Metadata-Version: 2.1 Name: MyLLM Version: 4.7.8 Summary: A python package to
 interact with llm model supported by g4f and langchain. License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Brotli (==1.1.0) Requires-Dist:
 PyExecJS2 (==1.6.1) Requires-Dist: curl_cffi (==0.6.2) Requires-Dist: dynaconf
 (>=3.2.0) Requires-Dist: fastapi (>=0.95.2) Requires-Dist: g4f (==0.2.7.2)
 Requires-Dist: httpx (>=0.24.1) Requires-Dist: js2py (>=0.74,<0.75) Requires-
-Dist: loguru (>=0.6.0) Requires-Dist: openai (==1.16.1) Requires-Dist: uvicorn
+Dist: loguru (>=0.6.0) Requires-Dist: openai (==1.16.2) Requires-Dist: uvicorn
 (>=0.22.0) Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions Description-
 Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_W_i_k_i_-
 _%_2_3_0_0_0_0_0_0_._s_v_g_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_&_l_o_g_o_=_w_i_k_i_p_e_d_i_a_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/
```

