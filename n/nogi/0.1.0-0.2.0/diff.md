# Comparing `tmp/nogi-0.1.0.tar.gz` & `tmp/nogi-0.2.0.tar.gz`

## Comparing `nogi-0.1.0.tar` & `nogi-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nogi-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nogi-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nogi-0.1.0/setup.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nogi-0.1.0/test-requirements.txt
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nogi-0.1.0/tox.ini
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 nogi-0.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nogi-0.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nogi-0.1.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/make.bat
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/requirements.txt
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/source/conf.py
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/source/index.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/source/reference/api/modules.rst
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 nogi-0.1.0/doc/source/reference/api/nogi.rst
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 nogi-0.1.0/examples/example.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nogi-0.1.0/examples/sample.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 nogi-0.1.0/nogi/__init__.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 nogi-0.1.0/nogi/client.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nogi-0.1.0/tests/test_init.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 nogi-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nogi-0.1.0/LICENSE
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 nogi-0.1.0/README.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 nogi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 nogi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nogi-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nogi-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 nogi-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nogi-0.2.0/setup.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nogi-0.2.0/test-requirements.txt
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nogi-0.2.0/tox.ini
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 nogi-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nogi-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nogi-0.2.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/make.bat
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/requirements.txt
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/source/conf.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/source/index.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/source/reference/api/modules.rst
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 nogi-0.2.0/doc/source/reference/api/nogi.rst
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 nogi-0.2.0/examples/example.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nogi-0.2.0/examples/sample.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 nogi-0.2.0/nogi/__init__.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 nogi-0.2.0/nogi/client.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nogi-0.2.0/tests/test_init.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 nogi-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nogi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 nogi-0.2.0/README.md
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 nogi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 nogi-0.2.0/PKG-INFO
```

### Comparing `nogi-0.1.0/.pre-commit-config.yaml` & `nogi-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/.readthedocs.yaml` & `nogi-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/tox.ini` & `nogi-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/.github/workflows/main.yml` & `nogi-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/.github/workflows/python-app.yml` & `nogi-0.2.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/doc/Makefile` & `nogi-0.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/doc/make.bat` & `nogi-0.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/doc/source/conf.py` & `nogi-0.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/doc/source/index.rst` & `nogi-0.2.0/doc/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 at runtime. Nogi is based on the backbone of your Python runtime, CPython
 itself. Nogi interact directly with the low level of your app to catch events
 to audit.
 
 Why Nogi?
 ---------
 
-Nogi could be, in some ways, compored to Userland Statically Defined Tracing
+Nogi could be, in some ways, compared to Userland Statically Defined Tracing
 (USDT, `see this article for more details about USDT
 <https://docs.openvswitch.org/en/latest/topics/usdt-probes/>`_).
 
 After weeks of studies and researches about USDT, I found that CPython
 ecosystem is a bit poor concerning them.
 
 I wrote several related debug notes:
```

### Comparing `nogi-0.1.0/examples/example.py` & `nogi-0.2.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/nogi/__init__.py` & `nogi-0.2.0/nogi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         This handler is executed in a dedicated thread to not block the
         main process.
         """
         log.debug("Starting the default audit server")
         serving = True
         while serving:
             try:
-                topic, data = self.q.get(block=False)
+                topic, data = self.q.get()
             except queue.Empty:
                 continue
             if topic == STOP_NOGI_SERVER_SEQUENCE:
                 serving = False
                 continue
             self.publisher.send_string(f"{topic}{DEFAULT_DELIMITER}{data}")
             self.q.task_done()
```

### Comparing `nogi-0.1.0/nogi/client.py` & `nogi-0.2.0/nogi/client.py`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/.gitignore` & `nogi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/LICENSE` & `nogi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/README.md` & `nogi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/pyproject.toml` & `nogi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nogi-0.1.0/PKG-INFO` & `nogi-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nogi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Audit any running python process.
 Project-URL: Homepage, https://github.com/4383/nogi
 Project-URL: History, https://github.com/4383/nogi/blob/main/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/4383
 Project-URL: Tracker, https://github.com/4383/nogi/issues
 Project-URL: Source, https://github.com/4383/nogi
 Author-email: Hervé Beraud <herveberaud.pro@gmail.com>
```

