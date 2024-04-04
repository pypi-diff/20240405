# Comparing `tmp/jaraco.context-4.3.0.tar.gz` & `tmp/jaraco.context-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.context-4.3.0.tar", last modified: Thu Jan 19 15:35:20 2023, max compression
+gzip compressed data, was "jaraco.context-5.0.0.tar", last modified: Thu Apr  4 18:59:12 2024, max compression
```

## Comparing `jaraco.context-4.3.0.tar` & `jaraco.context-5.0.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/jaraco/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:35:20.248215 jaraco.context-4.3.0/jaraco.context.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-19 15:35:20.000000 jaraco.context-4.3.0/jaraco.context.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-19 15:35:20.000000 jaraco.context-4.3.0/jaraco.context.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 15:35:20.000000 jaraco.context-4.3.0/jaraco.context.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-19 15:35:20.000000 jaraco.context-4.3.0/jaraco.context.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-19 15:35:20.000000 jaraco.context-4.3.0/jaraco.context.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-19 15:35:20.252215 jaraco.context-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-19 15:34:58.000000 jaraco.context-4.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.816538 jaraco.context-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.812538 jaraco.context-5.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.812538 jaraco.context-5.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-04 18:59:12.816538 jaraco.context-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.812538 jaraco.context-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.812538 jaraco.context-5.0.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/jaraco/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:59:12.812538 jaraco.context-5.0.0/jaraco.context.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-04 18:59:12.000000 jaraco.context-5.0.0/jaraco.context.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 18:59:12.000000 jaraco.context-5.0.0/jaraco.context.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:59:12.000000 jaraco.context-5.0.0/jaraco.context.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 18:59:12.000000 jaraco.context-5.0.0/jaraco.context.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 18:59:12.000000 jaraco.context-5.0.0/jaraco.context.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-04 18:59:12.816538 jaraco.context-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 18:58:54.000000 jaraco.context-5.0.0/tox.ini
```

### Comparing `jaraco.context-4.3.0/.github/workflows/main.yml` & `jaraco.context-5.0.0/.github/workflows/main.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,121 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
+
+permissions:
+  contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
-        - "3.11"
+        - "3.8"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run tests
+        run: python -m pip install tox
+      - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run tests
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Release
+        run: python -m pip install tox
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.context-4.3.0/CHANGES.rst` & `jaraco.context-5.0.0/NEWS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+v5.0.0
+======
+
+Features
+--------
+
+- Renamed tarball_context to tarball and deprecated tarball_context compatibility shim. (#3)
+- Disentangle pushd from tarball. (#4)
+
+
+Deprecations and Removals
+-------------------------
+
+- Removed deprecated 'runner' parameter to tarball_context.
+
+
 v4.3.0
 ======
 
 Deprecated ``runner`` parameter to ``tarball_context``.
 
 v4.2.1
 ======
```

### Comparing `jaraco.context-4.3.0/LICENSE` & `jaraco.context-5.0.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.context-4.3.0/docs/conf.py` & `jaraco.context-5.0.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.context-4.3.0/jaraco/context.py` & `jaraco.context-5.0.0/jaraco/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-import os
-import subprocess
+from __future__ import annotations
+
 import contextlib
 import functools
-import tempfile
-import shutil
 import operator
+import os
+import shutil
+import subprocess
+import tempfile
 import warnings
 
+from typing import Iterator
+
 
 @contextlib.contextmanager
-def pushd(dir):
+def pushd(dir: str | os.PathLike) -> Iterator[str | os.PathLike]:
     """
     >>> tmp_path = getfixture('tmp_path')
     >>> with pushd(tmp_path):
     ...     assert os.getcwd() == os.fspath(tmp_path)
     >>> assert os.getcwd() != os.fspath(tmp_path)
     """
 
@@ -22,43 +26,59 @@
     try:
         yield dir
     finally:
         os.chdir(orig)
 
 
 @contextlib.contextmanager
-def tarball_context(url, target_dir=None, runner=None, pushd=pushd):
+def tarball(
+    url, target_dir: str | os.PathLike | None = None
+) -> Iterator[str | os.PathLike]:
     """
-    Get a tarball, extract it, change to that directory, yield, then
-    clean up.
-    `runner` is the function to invoke commands.
-    `pushd` is a context manager for changing the directory.
+    Get a tarball, extract it, yield, then clean up.
     """
     if target_dir is None:
         target_dir = os.path.basename(url).replace('.tar.gz', '').replace('.tgz', '')
-    if runner is None:
-        runner = functools.partial(subprocess.check_call, shell=True)
-    else:
-        warnings.warn("runner parameter is deprecated", DeprecationWarning)
+    runner = functools.partial(subprocess.check_call, shell=True)
     # In the tar command, use --strip-components=1 to strip the first path and
     #  then
     #  use -C to cause the files to be extracted to {target_dir}. This ensures
     #  that we always know where the files were extracted.
     runner('mkdir {target_dir}'.format(**vars()))
     try:
         getter = 'wget {url} -O -'
         extract = 'tar x{compression} --strip-components=1 -C {target_dir}'
         cmd = ' | '.join((getter, extract))
         runner(cmd.format(compression=infer_compression(url), **vars()))
-        with pushd(target_dir):
-            yield target_dir
+        yield target_dir
     finally:
         runner('rm -Rf {target_dir}'.format(**vars()))
 
 
+@contextlib.contextmanager
+def tarball_cwd(*args, **kwargs) -> Iterator[str | os.PathLike]:
+    """
+    Convenience method for getting a tarball as the current working dir.
+    """
+    with tarball(*args, **kwargs) as tball, pushd(tball) as dir:
+        yield dir
+
+
+@contextlib.contextmanager
+def tarball_context(*args, **kwargs):
+    warnings.warn(
+        "tarball_context is deprecated. Use tarball or tarball_cwd instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+    pushd_ctx = kwargs.pop('pushd', pushd)
+    with tarball(*args, **kwargs) as tball, pushd_ctx(tball) as dir:
+        yield dir
+
+
 def infer_compression(url):
     """
     Given a URL or filename, infer the compression code for tar.
 
     >>> infer_compression('http://foo/bar.tar.gz')
     'z'
     >>> infer_compression('http://foo/bar.tgz')
@@ -116,14 +136,18 @@
 @contextlib.contextmanager
 def null():
     """
     A null context suitable to stand in for a meaningful context.
 
     >>> with null() as value:
     ...     assert value is None
+
+    This context is most useful when dealing with two or more code
+    branches but only some need a context. Wrap the others in a null
+    context to provide symmetry across all options.
     """
     yield
 
 
 class ExceptionTrap:
     """
     A context manager that will catch certain exceptions and provide an
```

### Comparing `jaraco.context-4.3.0/setup.cfg` & `jaraco.context-5.0.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 [metadata]
 name = jaraco.context
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
-description = Context managers by jaraco
+description = Useful decorators and context managers
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.context
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
-
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-mypy
+	pytest-enabler >= 2.2
+	pytest-ruff >= 0.2.1
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
```

