# Comparing `tmp/multiset-3.0.2.tar.gz` & `tmp/multiset-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiset-3.0.2.tar", last modified: Sat Dec 30 12:33:49 2023, max compression
+gzip compressed data, was "multiset-3.1.0.tar", last modified: Fri Apr  5 20:48:54 2024, max compression
```

## Comparing `multiset-3.0.2.tar` & `multiset-3.1.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-30 12:33:31.000000 multiset-3.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-30 12:33:31.000000 multiset-3.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-30 12:33:31.000000 multiset-3.0.2/.github/workflows/python-dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-12-30 12:33:31.000000 multiset-3.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-12-30 12:33:31.000000 multiset-3.0.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-30 12:33:31.000000 multiset-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13042 2023-12-30 12:33:31.000000 multiset-3.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-30 12:33:31.000000 multiset-3.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-30 12:33:31.000000 multiset-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-30 12:33:31.000000 multiset-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-30 12:33:31.000000 multiset-3.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-12-30 12:33:49.852294 multiset-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2023-12-30 12:33:31.000000 multiset-3.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-30 12:33:31.000000 multiset-3.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-30 12:33:31.000000 multiset-3.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-30 12:33:31.000000 multiset-3.0.2/flit.ini
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-30 12:33:31.000000 multiset-3.0.2/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/multiset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2023-12-30 12:33:49.000000 multiset-3.0.2/multiset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-30 12:33:49.000000 multiset-3.0.2/multiset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 12:33:49.000000 multiset-3.0.2/multiset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-30 12:33:49.000000 multiset-3.0.2/multiset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 12:33:49.000000 multiset-3.0.2/multiset.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    39068 2023-12-30 12:33:31.000000 multiset-3.0.2/multiset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2023-12-30 12:33:31.000000 multiset-3.0.2/multiset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:31.000000 multiset-3.0.2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-12-30 12:33:31.000000 multiset-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-30 12:33:49.856294 multiset-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-30 12:33:31.000000 multiset-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 12:33:49.852294 multiset-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-30 12:33:31.000000 multiset-3.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    27115 2023-12-30 12:33:31.000000 multiset-3.0.2/tests/test_multiset.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-30 12:33:31.000000 multiset-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.765650 multiset-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 20:48:43.000000 multiset-3.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.761649 multiset-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 20:48:43.000000 multiset-3.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.761649 multiset-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-05 20:48:43.000000 multiset-3.1.0/.github/workflows/python-dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-05 20:48:43.000000 multiset-3.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-05 20:48:43.000000 multiset-3.1.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-05 20:48:43.000000 multiset-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2024-04-05 20:48:43.000000 multiset-3.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 20:48:43.000000 multiset-3.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-05 20:48:43.000000 multiset-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 20:48:43.000000 multiset-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 20:48:43.000000 multiset-3.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-05 20:48:54.765650 multiset-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-05 20:48:43.000000 multiset-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 20:48:43.000000 multiset-3.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.761649 multiset-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 20:48:43.000000 multiset-3.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 20:48:43.000000 multiset-3.1.0/flit.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 20:48:43.000000 multiset-3.1.0/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.761649 multiset-3.1.0/multiset/
+-rw-r--r--   0 runner    (1001) docker     (127)    39597 2024-04-05 20:48:43.000000 multiset-3.1.0/multiset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-05 20:48:43.000000 multiset-3.1.0/multiset/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:43.000000 multiset-3.1.0/multiset/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.765650 multiset-3.1.0/multiset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-05 20:48:54.000000 multiset-3.1.0/multiset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 20:48:54.000000 multiset-3.1.0/multiset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:48:54.000000 multiset-3.1.0/multiset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 20:48:54.000000 multiset-3.1.0/multiset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:48:54.000000 multiset-3.1.0/multiset.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-05 20:48:43.000000 multiset-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-05 20:48:54.765650 multiset-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 20:48:43.000000 multiset-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:48:54.765650 multiset-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 20:48:43.000000 multiset-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27115 2024-04-05 20:48:43.000000 multiset-3.1.0/tests/test_multiset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-05 20:48:43.000000 multiset-3.1.0/tox.ini
```

### Comparing `multiset-3.0.2/.github/workflows/python-publish.yml` & `multiset-3.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/.github/workflows/python-test.yml` & `multiset-3.1.0/.github/workflows/python-test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 name: Tests
 
 on:
   push:
     branches:
-    - master
+      - master
   pull_request:
     branches:
-    - master
+      - master
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    if: ${{ github.actor != 'dependabot[bot]' }}
     strategy:
       matrix:
-        python-version: [ '3.7', '3.8', '3.9', '3.10' ]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     name: Run tests
     steps:
       - uses: actions/checkout@v2
       - name: Setup python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: Install dependencies
         run: make init
       - name: Lint
         run: make check
-        if: matrix.python-version == 'disabled'
+        if: matrix.python-version == '3.8'
+        continue-on-error: true
       - name: Run tests
         run: make test
+      - name: Run stubtest
+        run: make stubtest
+      - name: Build
+        run: make build
       - name: Upload coverage
         run: make coverage
       - name: Coveralls Parallel
         uses: coverallsapp/github-action@v2
         with:
           flag-name: run-${{ join(matrix.*, '-') }}
           parallel: true
 
   finish:
     needs: build
     if: ${{ always() }}
     runs-on: ubuntu-latest
     steps:
-    - name: Coveralls Finished
-      uses: coverallsapp/github-action@v2
-      with:
-        parallel-finished: true
-        carryforward: "run-3.8"
+      - name: Coveralls Finished
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel-finished: true
+          carryforward: "run-3.8"
```

### Comparing `multiset-3.0.2/.gitignore` & `multiset-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/.pylintrc` & `multiset-3.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/LICENSE` & `multiset-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/PKG-INFO` & `multiset-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: multiset
-Version: 3.0.2
+Version: 3.1.0
 Summary: An implementation of a multiset.
 Home-page: https://github.com/wheerd/multiset
 Author: Manuel Krebber
 Author-email: Manuel Krebber <admin@wheerd.de>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 multiset
 ========
 
 This package provides a multiset_ implementation for python.
```

### Comparing `multiset-3.0.2/README.rst` & `multiset-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/docs/Makefile` & `multiset-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/docs/conf.py` & `multiset-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/docs/index.rst` & `multiset-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/docs/make.bat` & `multiset-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/multiset.egg-info/PKG-INFO` & `multiset-3.1.0/multiset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: multiset
-Version: 3.0.2
+Version: 3.1.0
 Summary: An implementation of a multiset.
 Home-page: https://github.com/wheerd/multiset
 Author: Manuel Krebber
 Author-email: Manuel Krebber <admin@wheerd.de>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 multiset
 ========
 
 This package provides a multiset_ implementation for python.
```

### Comparing `multiset-3.0.2/multiset.egg-info/SOURCES.txt` & `multiset-3.1.0/multiset.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 dev-requirements.txt
 flit.ini
 make.bat
-multiset.py
-multiset.pyi
-py.typed
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/dependabot.yml
 .github/workflows/python-dependabot.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
+multiset/__init__.py
+multiset/__init__.pyi
+multiset/py.typed
 multiset.egg-info/PKG-INFO
 multiset.egg-info/SOURCES.txt
 multiset.egg-info/dependency_links.txt
 multiset.egg-info/top_level.txt
 multiset.egg-info/zip-safe
 tests/conftest.py
 tests/test_multiset.py
```

### Comparing `multiset-3.0.2/multiset.py` & `multiset-3.1.0/multiset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,15 @@
         _elements = self._elements
         if element in _elements:
             self._total -= _elements[element]
             del _elements[element]
         else:
             raise KeyError("Could not delete {!r} from the multiset, because it is not in it.".format(element))
 
-    def update(self, *others):
+    def update(self, *others, **kwargs):
         r"""Like :meth:`dict.update` but add multiplicities instead of replacing them.
 
         >>> ms = Multiset('aab')
         >>> ms.update('abc')
         >>> sorted(ms)
         ['a', 'a', 'a', 'b', 'b', 'c']
 
@@ -694,22 +694,35 @@
         >>> ms += Multiset('bc')
         >>> sorted(ms)
         ['a', 'a', 'a', 'b', 'b', 'b', 'c', 'c']
 
         For a variant of the operation which does not modify the multiset, but returns a new
         multiset instead see :meth:`combine`.
 
+        Any keyword arguments are also added to the multiset:
+
+        >>> ms = Multiset('ab')
+        >>> ms.update(a=1, e=2)
+        >>> sorted(ms)
+        ['a', 'a', 'b', 'e', 'e']
+
         Args:
             others: The other sets to add to this multiset. Can also be any :class:`~typing.Iterable`\[~T]
                 or :class:`~typing.Mapping`\[~T, :class:`int`] which are then converted to :class:`Multiset`\[~T].
+            kwargs: Additional pairs of values and multiplicities to be added to multiset.
         """
         _elements = self._elements
-        for other in map(self._as_mapping, others):
+        _total = self._total
+        for other in map(self._as_mapping, others + (kwargs, )):
             for element, multiplicity in other.items():
-                self[element] += multiplicity
+                if multiplicity > 0:
+                    old_multiplicity = _elements.get(element, 0)
+                    _elements[element] = multiplicity + old_multiplicity
+                    _total += multiplicity
+        self._total = _total
 
     def union_update(self, *others):
         r"""Update the multiset, adding elements from all others using the maximum multiplicity.
 
         >>> ms = Multiset('aab')
         >>> ms.union_update('bc')
         >>> sorted(ms)
```

### Comparing `multiset-3.0.2/pyproject.toml` & `multiset-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,28 @@
     "setuptools_scm[toml]>=3.4",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiset"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 description = "An implementation of a multiset."
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 authors = [
     {name = "Manuel Krebber", email = "admin@wheerd.de"},
 ]
 readme = {file = "README.rst", content-type="text/x-rst"}
 dynamic = ["version"]
```

### Comparing `multiset-3.0.2/setup.cfg` & `multiset-3.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 home_page = https://github.com/wheerd/multiset
 repository = https://github.com/wheerd/multiset
 documentation = https://multiset.readthedocs.io/
 author = Manuel Krebber
 author_email = admin@wheerd.de
 readme = file: README.rst
 
 [options]
 zip_safe = True
 include_package_data = True
 setup_requires = 
 	setuptools >= 46
 	setuptools_scm
-python_requires = >= 3.7
-py_modules = multiset
+python_requires = >= 3.8
+packages = multiset
 test_suite = tests
 
 [options.package_data]
 multiset = *.pyi, py.typed
 
 [flake8]
 max-line-length = 120
```

### Comparing `multiset-3.0.2/tests/conftest.py` & `multiset-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `multiset-3.0.2/tests/test_multiset.py` & `multiset-3.1.0/tests/test_multiset.py`

 * *Files identical despite different names*

