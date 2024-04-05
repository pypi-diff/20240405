# Comparing `tmp/rython_calc-0.4.1.tar.gz` & `tmp/rython_calc-0.4.3.tar.gz`

## Comparing `rython_calc-0.4.1.tar` & `rython_calc-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.1/Cargo.toml
--rw-r--r--   0     1001      127     3584 2024-04-02 19:58:30.000000 rython_calc-0.4.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-02 19:58:30.000000 rython_calc-0.4.1/.gitignore
--rw-r--r--   0     1001      127     1075 2024-04-02 19:58:30.000000 rython_calc-0.4.1/LICENSE
--rw-r--r--   0     1001      127      603 2024-04-02 19:58:30.000000 rython_calc-0.4.1/README.md
--rw-r--r--   0     1001      127    10298 2024-04-02 19:58:30.000000 rython_calc-0.4.1/poetry.lock
--rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/__init__.py
--rw-r--r--   0     1001      127     1743 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/py.typed
--rw-r--r--   0     1001      127      666 2024-04-02 19:58:30.000000 rython_calc-0.4.1/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     2924 2024-04-02 19:58:30.000000 rython_calc-0.4.1/src/lib.rs
--rw-r--r--   0     1001      127      347 2024-04-02 19:58:30.000000 rython_calc-0.4.1/test/rython/test_rython_calc.py
--rw-r--r--   0     1001      127     7857 2024-04-02 19:58:30.000000 rython_calc-0.4.1/Cargo.lock
--rw-r--r--   0     1001      127     1041 2024-04-02 19:58:30.000000 rython_calc-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 rython_calc-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      127      367 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4911 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.gitignore
+-rw-r--r--   0     1001      127     1075 2024-04-05 19:40:45.000000 rython_calc-0.4.3/LICENSE
+-rw-r--r--   0     1001      127      603 2024-04-05 19:40:45.000000 rython_calc-0.4.3/README.md
+-rw-r--r--   0     1001      127    10298 2024-04-05 19:40:45.000000 rython_calc-0.4.3/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1743 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/py.typed
+-rw-r--r--   0     1001      127      666 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     3030 2024-04-05 19:40:45.000000 rython_calc-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      127      347 2024-04-05 19:40:45.000000 rython_calc-0.4.3/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127     7857 2024-04-05 19:40:45.000000 rython_calc-0.4.3/Cargo.lock
+-rw-r--r--   0     1001      127     1057 2024-04-05 19:40:45.000000 rython_calc-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 rython_calc-0.4.3/PKG-INFO
```

### Comparing `rython_calc-0.4.1/.gitignore` & `rython_calc-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.1/LICENSE` & `rython_calc-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.1/README.md` & `rython_calc-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.1/poetry.lock` & `rython_calc-0.4.3/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -149,20 +149,20 @@
 pluggy = ">=1.4,<2.0"
 
 [package.extras]
 testing = ["argcomplete", "attrs (>=19.2)", "hypothesis (>=3.56)", "mock", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "typing-extensions"
-version = "4.10.0"
+version = "4.11.0"
 description = "Backported and Experimental Type Hints for Python 3.8+"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
-    {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.12"
-content-hash = "964c703c2df66d4d86f53a80d6224323c2401efb24dad7b1641d491ed3f8da57"
+content-hash = "9a7a4bf4563df4df31b038341083c9fb8e3a2c89f5f32dd097b81c7387a462da"
```

### Comparing `rython_calc-0.4.1/python/cli/main.py` & `rython_calc-0.4.3/python/cli/main.py`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.1/python/rython/rython_calc.pyi` & `rython_calc-0.4.3/python/rython/rython_calc.pyi`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.1/src/lib.rs` & `rython_calc-0.4.3/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,23 @@
 
     #[pyo3(text_signature = "($self, second_number: int) -> int")]
     fn add(&mut self, second_number: i32) -> PyResult<i32> {
         self.number = self.number.wrapping_add(second_number);
         Ok(self.number)
     }
 
-    #[pyo3(text_signature = "($self, number_of_loops: int, add_number: int, mul_number: int) -> int")]
-    fn loop_add_mul_seq(&mut self, number_of_loops: i32, add_number: i32, mul_number: i32) -> PyResult<i32> {
+    #[pyo3(
+        text_signature = "($self, number_of_loops: int, add_number: int, mul_number: int) -> int"
+    )]
+    fn loop_add_mul_seq(
+        &mut self,
+        number_of_loops: i32,
+        add_number: i32,
+        mul_number: i32,
+    ) -> PyResult<i32> {
         for _ in 0..number_of_loops {
             self.number = self.number.wrapping_add(add_number);
             self.number = self.number.wrapping_mul(mul_number);
         }
         Ok(self.number)
     }
 
@@ -67,16 +74,23 @@
 
     #[pyo3(text_signature = "($self, second_number: float) -> float")]
     fn add(&mut self, second_number: f64) -> PyResult<f64> {
         self.number += second_number;
         Ok(self.number)
     }
 
-    #[pyo3(text_signature = "($self, number_of_loops: int, add_number: float, mul_number: float) -> float")]
-    fn loop_add_mul_seq(&mut self, number_of_loops: i32, add_number: f64, mul_number: f64) -> PyResult<f64> {
+    #[pyo3(
+        text_signature = "($self, number_of_loops: int, add_number: float, mul_number: float) -> float"
+    )]
+    fn loop_add_mul_seq(
+        &mut self,
+        number_of_loops: i32,
+        add_number: f64,
+        mul_number: f64,
+    ) -> PyResult<f64> {
         for _ in 0..number_of_loops {
             self.number += add_number;
             self.number *= mul_number;
         }
         Ok(self.number)
     }
```

### Comparing `rython_calc-0.4.1/Cargo.lock` & `rython_calc-0.4.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rython"
-version = "0.4.1"
+version = "0.4.3"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -199,17 +199,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `rython_calc-0.4.1/pyproject.toml` & `rython_calc-0.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "rython-calc"
-version = "0.4.1"
+version = "0.4.3"
 description = "Rython package to test python and rust compatibility"
 authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 readme = "README.md"
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-mypy = "^1.9.0"
 
 [tool.poetry.group.dev.dependencies]
 maturin = "^1.5.1"
 pytest = "^8.1.1"
+mypy = "^1.9.0"
 
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rython_calc"
```

### Comparing `rython_calc-0.4.1/PKG-INFO` & `rython_calc-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.1
+Version: 0.4.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

