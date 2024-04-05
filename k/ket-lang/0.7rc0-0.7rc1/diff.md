# Comparing `tmp/ket-lang-0.7rc0.tar.gz` & `tmp/ket-lang-0.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.7rc0.tar", last modified: Thu Jan 18 18:40:36 2024, max compression
+gzip compressed data, was "ket-lang-0.7rc1.tar", last modified: Tue Jan 23 18:22:10 2024, max compression
```

## Comparing `ket-lang-0.7rc0.tar` & `ket-lang-0.7rc1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.122619 ket-lang-0.7rc0/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5334 2024-01-18 18:40:36.122619 ket-lang-0.7rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4577 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-01-18 18:40:36.122619 ket-lang-0.7rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.109619 ket-lang-0.7rc0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.112619 ket-lang-0.7rc0/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     2538 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32377 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.113619 ket-lang-0.7rc0/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.113619 ket-lang-0.7rc0/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.114619 ket-lang-0.7rc0/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-18 18:40:24.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.114619 ket-lang-0.7rc0/src/ket/clib/libs/kbw/.reuse/
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/.reuse/dep5
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      888 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.115619 ket-lang-0.7rc0/src/ket/clib/libs/kbw/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.116619 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/c_api.rs
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    12423 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2219 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)    11489 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    12101 2024-01-18 18:40:25.000000 ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.118619 ket-lang-0.7rc0/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-18 18:40:24.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.118619 ket-lang-0.7rc0/src/ket/clib/libs/libket/.reuse/
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/.reuse/dep5
--rw-rw-rw-   0 root         (0) root         (0)     1049 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      851 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.118619 ket-lang-0.7rc0/src/ket/clib/libs/libket/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.118619 ket-lang-0.7rc0/src/ket/clib/libs/libket/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/examples/bell.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.119619 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.120619 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/
--rw-rw-rw-   0 root         (0) root         (0)     1772 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     1751 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    11963 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     4064 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     3890 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)     3098 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     2852 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    21218 2024-01-18 18:40:26.000000 ket-lang-0.7rc0/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     2415 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/clib/wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     8770 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/expv.py
--rw-rw-rw-   0 root         (0) root         (0)    16342 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/gates.py
--rw-rw-rw-   0 root         (0) root         (0)     9221 2024-01-18 18:40:23.000000 ket-lang-0.7rc0/src/ket/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 18:40:36.121619 ket-lang-0.7rc0/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5334 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1762 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2024-01-18 18:40:36.000000 ket-lang-0.7rc0/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.837642 ket-lang-0.7rc1/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5334 2024-01-23 18:22:10.837642 ket-lang-0.7rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-01-23 18:22:10.838642 ket-lang-0.7rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.824642 ket-lang-0.7rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.826642 ket-lang-0.7rc1/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32377 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.827642 ket-lang-0.7rc1/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.827642 ket-lang-0.7rc1/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.829642 ket-lang-0.7rc1/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.829642 ket-lang-0.7rc1/src/ket/clib/libs/kbw/.reuse/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/.reuse/dep5
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.829642 ket-lang-0.7rc1/src/ket/clib/libs/kbw/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.831642 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/c_api.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    12423 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)    11489 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    12101 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.832642 ket-lang-0.7rc1/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.833642 ket-lang-0.7rc1/src/ket/clib/libs/libket/.reuse/
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/.reuse/dep5
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.833642 ket-lang-0.7rc1/src/ket/clib/libs/libket/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.833642 ket-lang-0.7rc1/src/ket/clib/libs/libket/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/examples/bell.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.834642 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.835642 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/
+-rw-rw-rw-   0 root         (0) root         (0)     2453 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    16231 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4258 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    27327 2024-01-23 18:22:01.000000 ket-lang-0.7rc1/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/clib/wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     8804 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/expv.py
+-rw-rw-rw-   0 root         (0) root         (0)    14105 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     6079 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     9221 2024-01-23 18:22:00.000000 ket-lang-0.7rc1/src/ket/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 18:22:10.837642 ket-lang-0.7rc1/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5334 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2024-01-23 18:22:10.000000 ket-lang-0.7rc1/src/ket_lang.egg-info/top_level.txt
```

### Comparing `ket-lang-0.7rc0/LICENSE` & `ket-lang-0.7rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/PKG-INFO` & `ket-lang-0.7rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.7rc0
+Version: 0.7rc1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.7rc0/README.md` & `ket-lang-0.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/setup.cfg` & `ket-lang-0.7rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/__init__.py` & `ket-lang-0.7rc1/src/ket/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 classes to build quantum algorithms and applications. It facilitates the manipulation and storage of
 quantum states, measurement operations, and the computation of expected values.
 
 Explore the documentation of individual submodules for in-depth information and more practical code
 examples.
 
 All the functionality from the submodules is conveniently accessible within the ``ket`` namespace.
+Except for the `lib` module.
 
 Examples:
 
     - Grover algorithm
 
     .. code-block:: python
 
@@ -82,11 +83,12 @@
 from .base import __all__ as all_base
 from .operations import *
 from .operations import __all__ as all_func
 from .gates import *
 from .gates import __all__ as all_gate
 from .expv import *
 from .expv import __all__ as all_expv
+from . import lib
 
-__version__ = "0.7rc0"
+__version__ = "0.7rc1"
 
-__all__ = all_base + all_func + all_gate + all_expv
+__all__ = all_base + all_func + all_gate + all_expv + ["lib"]
```

### Comparing `ket-lang-0.7rc0/src/ket/base.py` & `ket-lang-0.7rc1/src/ket/base.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/kbw.py` & `ket-lang-0.7rc1/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libket.py` & `ket-lang-0.7rc1/src/ket/clib/libket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/__init__.py` & `ket-lang-0.7rc1/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/CHANGELOG.md` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Changelog
 
+## 0.2.0
+
+- Updated Libket to version 0.4.0, adding the `batch` and `live` execution modes.
+
 ## 0.1.7
 
 - Fixed for Libket version 0.3.1.
 
 ## 0.1.6
 
 - Updated Libket to version 0.3.0.
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 # SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [package]
 name = "kbw"
-version = "0.1.7"
+version = "0.2.0"
 authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Ket Bitwise Simulator"
 repository = "https://gitlab.com/quantum-ket/kbw"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-libket = { git = "https://gitlab.com/quantum-ket/libket.git", branch = "0.4.0" }
+libket = "0.4.0"
 num = "0.4"
 rand = "0.8.5"
 rayon = "1.5.3"
 twox-hash = "1.6.3"
 itertools = "0.12.0"
 log = "0.4.20"
-env_logger = "0.10.1"
+env_logger = "0.11.0"
+thiserror = "1.0.56"
+
 
 [lib]
 crate-type = ["cdylib", "rlib"]
 
 [profile.release]
 strip = true
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/LICENSES/Apache-2.0.txt` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/c_api.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/c_api.rs`

 * *Files 14% similar despite different names*

```diff
@@ -24,19 +24,36 @@
 
     KBWError::Success.error_code()
 }
 
 pub mod error {
     use crate::error::{KBWError, Result};
 
+    /// Returns the error message for the given error code.
+    ///
+    /// # Safety
+    ///
+    /// This functions is unsafe because it assumes that the error code is valid.
     #[no_mangle]
-    pub extern "C" fn kbw_error_message(error_code: i32, size: &mut usize) -> *const u8 {
-        let msg = KBWError::from_error_code(error_code).to_str();
-        *size = msg.len();
-        msg.as_ptr()
+    pub unsafe extern "C" fn kbw_error_message(
+        error_code: i32,
+        buffer: *mut u8,
+        buffer_size: usize,
+        write_size: &mut usize,
+    ) -> i32 {
+        let msg = unsafe { KBWError::from_error_code(error_code) }.to_string();
+        let msg = msg.as_bytes();
+        *write_size = msg.len();
+        if buffer_size >= *write_size {
+            let buffer = unsafe { std::slice::from_raw_parts_mut(buffer, buffer_size) };
+            buffer[..*write_size].copy_from_slice(msg);
+            0
+        } else {
+            1
+        }
     }
 
     pub fn wrapper(error: Result<()>) -> i32 {
         match error {
             Ok(_) => KBWError::Success.error_code(),
             Err(error) => error.error_code(),
         }
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/error.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 // SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 // SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 //
 // SPDX-License-Identifier: Apache-2.0
 
-use std::{error::Error, fmt::Display, result};
+use std::result;
 
-#[derive(Debug, Clone, Copy)]
+/// Enumeration of possible errors in the KBW simulator.
+#[derive(thiserror::Error, Debug, Clone, Copy)]
 #[repr(i32)]
 pub enum KBWError {
+    #[error("The function call completed successfully.")]
     Success,
+
+    #[error("An undefined error occurred.")]
+    UndefinedError,
+
+    #[error("The quantum execution has timed out.")]
     Timeout,
+
+    #[error(
+        "Cannot allocate more qubits. Ensure you are not deallocating too many qubits as dirty."
+    )]
     OutOfQubits,
+
+    #[error("The number of requested qubits is not supported.")]
     UnsupportedNumberOfQubits,
+
+    #[error("The process is not yet ready for execution.")]
     NotReadyForExecution,
-    UndefinedDataType,
+
+    #[error("The simulation mode is undefined.")]
     UndefinedSimMode,
-    UndefinedError,
+
+    #[error("The data type is undefined.")]
+    UndefinedDataType,
 }
 
+/// Result type for KBW library functions.
 pub type Result<T> = result::Result<T, KBWError>;
 
 impl KBWError {
-    pub fn to_str(&self) -> &'static str {
-        match self {
-            KBWError::Success => "The function call completed successfully.",
-            KBWError::UndefinedError => "An undefined error occurred.",
-            KBWError::Timeout => "The quantum execution has timed out.",
-            KBWError::OutOfQubits => "Cannot allocate more qubits. Ensure you are not deallocating too many qubits as dirty.",
-            KBWError::UnsupportedNumberOfQubits => "The number of requested qubits is not supported.",
-            KBWError::NotReadyForExecution => "The process is not yet ready for execution.",
-            KBWError::UndefinedSimMode => "The simulation mode is undefined.",
-            KBWError::UndefinedDataType => "The data type is undefined.",
-        }
-    }
-
+    /// Returns the error code as an integer.
     pub fn error_code(&self) -> i32 {
         *self as i32
     }
 
-    pub fn from_error_code(error_code: i32) -> KBWError {
+    /// Converts an error code into a KBWError.
+    ///
+    /// # Safety
+    ///
+    /// This function is unsafe because it assumes that the error code is valid.
+    pub unsafe fn from_error_code(error_code: i32) -> KBWError {
         unsafe { std::mem::transmute(error_code) }
     }
 }
 
-impl Display for KBWError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "{}", self.to_str())
-    }
-}
-
-impl Error for KBWError {}
-
 #[cfg(test)]
 mod tests {
     use super::KBWError;
 
     #[test]
     fn success_is_zero() {
         assert!(KBWError::Success.error_code() == 0)
     }
 
     #[test]
     fn print_error_code() {
         let mut error_code = 0;
         loop {
-            let error = KBWError::from_error_code(error_code);
+            let error = unsafe { KBWError::from_error_code(error_code) };
             println!("#define KBW_{:#?} {}", error, error_code);
 
             if let KBWError::UndefinedError = error {
                 break;
             } else {
                 error_code += 1;
             }
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 num = "0.4"
 log = "0.4.20"
-env_logger = "0.10.1"
+env_logger = "0.11.0"
+thiserror = "1.0.56"
 
 
 [lib]
 name = "ket"
 crate-type = ["cdylib", "rlib"]
 
 [profile.release]
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/LICENSES/Apache-2.0.txt` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/src/c_api/process.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/src/c_api/process.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 // SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 // SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 //
 // SPDX-License-Identifier: Apache-2.0
 
+//! C API for the `Process` struct.
+
 use log::trace;
 
 use crate::{
     error::KetError, process::Process, Angle, Configuration, Pauli, PauliHamiltonian, PauliProduct,
     PauliTerm, QuantumGate,
 };
 
 use super::error::wrapper;
 
 /// Creates a new `Process` instance with the given process ID.
 ///
 /// # Arguments
 ///
-/// * `pid` -  \[in\] The process ID.
+/// * `config` -  \[in\] A mutable pointer to a `Configuration` instance.
 /// * `process` -  \[out\] A mutable pointer to a `Process` pointer.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 ///
 /// # Safety
@@ -58,16 +60,15 @@
 }
 
 /// Allocates a qubit for the `Process` instance.
 ///
 /// # Arguments
 ///
 /// * `process` -  \[in\] A mutable reference to the `Process` instance.
-/// * `dirty` -  \[in\] A boolean indicating whether the allocated qubit should be initialized as dirty.
-/// * `qubit` -  \[out\] A mutable pointer to a `Qubit` pointer.
+/// * `qubit` -  \[out\] A mutable pointer to a `usize`.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 #[no_mangle]
 pub extern "C" fn ket_process_allocate_qubit(process: &mut Process, qubit: &mut usize) -> i32 {
     match process.allocate_qubit() {
@@ -80,16 +81,15 @@
 }
 
 /// Frees the allocated qubit from the `Process` instance.
 ///
 /// # Arguments
 ///
 /// * `process` -  \[in\] A mutable reference to the `Process` instance.
-/// * `qubit` -  \[in\] A mutable reference to the `Qubit` instance to be freed.
-/// * `dirty` -  \[in\] A boolean indicating whether the qubit should be marked as dirty before freeing.
+/// * `qubit` -  \[in\] A `usize` representing the qubit index to be freed.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 #[no_mangle]
 pub extern "C" fn ket_process_free_qubit(process: &mut Process, qubit: usize) -> i32 {
     wrapper(process.free_qubit(qubit))
@@ -97,15 +97,17 @@
 
 /// Applies a quantum gate to the target `Qubit` in the `Process` instance.
 ///
 /// # Arguments
 ///
 /// * `process` -  \[in\] A mutable reference to the `Process` instance.
 /// * `gate` -  \[in\] An integer representing the gate type. See the function body for the mapping of gate values to gate types.
-/// * `param` -  \[in\] A floating-point parameter value used by certain gate types.
+/// * `pi_fraction_top` -  \[in\] The numerator of the fraction part of the angle, used by certain gate types.
+/// * `pi_fraction_bottom` -  \[in\] The denominator of the fraction part of the angle, used by certain gate types.
+/// * `scalar` -  \[in\] A floating-point parameter value used by certain gate types.
 /// * `target` -  \[in\] A reference to the target `Qubit` instance.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 #[no_mangle]
 pub extern "C" fn ket_process_apply_gate(
@@ -148,15 +150,15 @@
 /// Measures the specified qubits in the `Process` instance.
 ///
 /// # Arguments
 ///
 /// * `process` -  \[in\] A mutable reference to the `Process` instance.
 /// * `qubits` -  \[in\] A mutable pointer to an array of mutable references to `Qubit` instances.
 /// * `qubits_size` -  \[in\] The size of the `qubits` array.
-/// * `future` -  \[out\] A mutable pointer to a `Future` pointer.
+/// * `result` -  \[out\] A mutable pointer to a `usize` where the measurement result will be stored.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 ///
 /// # Safety
 ///
@@ -182,22 +184,48 @@
 
             KetError::Success.error_code()
         }
         Err(error) => error.error_code(),
     }
 }
 
+/// Creates a new `PauliHamiltonian` instance.
+///
+/// # Arguments
+///
+/// * `hamiltonian` -  \[out\] A mutable pointer to a `PauliHamiltonian` pointer.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
 #[no_mangle]
 pub extern "C" fn ket_hamiltonian_new(hamiltonian: &mut *mut PauliHamiltonian) -> i32 {
     *hamiltonian = Box::into_raw(Box::default());
 
     KetError::Success.error_code()
 }
 
+/// Adds a term to the `PauliHamiltonian`.
+///
+/// # Arguments
+///
+/// * `hamiltonian` -  \[in\] A mutable reference to the `PauliHamiltonian` instance.
+/// * `pauli` -  \[in\] A pointer to an array of integers representing the Pauli operators (1 for X, 2 for Y, 3 for Z).
+/// * `pauli_size` -  \[in\] The size of the `pauli` array.
+/// * `qubits` -  \[in\] A pointer to an array of integers representing the qubit indices for each Pauli operator.
+/// * `qubits_size` -  \[in\] The size of the `qubits` array.
+/// * `coefficients` -  \[in\] The coefficient for the term.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_hamiltonian_add(
     hamiltonian: &mut PauliHamiltonian,
     pauli: *const i32,
     pauli_size: usize,
     qubits: *const usize,
     qubits_size: usize,
@@ -228,34 +256,64 @@
 
     hamiltonian.products.push(pauli_product);
     hamiltonian.coefficients.push(coefficients);
 
     KetError::Success.error_code()
 }
 
+/// Calculates the expected value of the `PauliHamiltonian` in the `Process` instance.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+/// * `hamiltonian` -  \[in\] A mutable pointer to a `PauliHamiltonian`.
+/// * `result` -  \[out\] A mutable pointer to a `usize` where the result identifier will be stored.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_process_exp_value(
     process: &mut Process,
     hamiltonian: *mut PauliHamiltonian,
     result: &mut usize,
 ) -> i32 {
     let hamiltonian = unsafe { Box::from_raw(hamiltonian) };
-    trace!("ket_process_exp_value( hamiltonian={:?} )", hamiltonian,);
+    trace!("ket_process_exp_value( hamiltonian={:?} )", hamiltonian);
     match process.exp_values(*hamiltonian) {
         Ok(result_id) => {
             *result = result_id;
 
             KetError::Success.error_code()
         }
         Err(error) => error.error_code(),
     }
 }
 
+/// Samples the specified qubits in the `Process` instance.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+/// * `qubits` -  \[in\] A pointer to an array of integers representing the qubit indices to be sampled.
+/// * `qubits_size` -  \[in\] The size of the `qubits` array.
+/// * `shots` -  \[in\] The number of measurement shots.
+/// * `result` -  \[out\] A mutable pointer to a `usize` where the result identifier will be stored.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_process_sample(
     process: &mut Process,
     qubits: *const usize,
     qubits_size: usize,
     shots: u64,
     result: &mut usize,
@@ -275,15 +333,30 @@
 
             KetError::Success.error_code()
         }
         Err(error) => error.error_code(),
     }
 }
 
+/// Dumps the state of the specified qubits in the `Process` instance.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+/// * `qubits` -  \[in\] A pointer to an array of qubit indices to be dumped.
+/// * `qubits_size` -  \[in\] The size of the `qubits` array.
+/// * `result` -  \[out\] A mutable pointer to a `usize` representing the result index of the dump.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_process_dump(
     process: &mut Process,
     qubits: *const usize,
     qubits_size: usize,
     result: &mut usize,
 ) -> i32 {
@@ -306,15 +379,15 @@
 }
 
 /// Pushes control qubits onto the control stack in the `Process` instance.
 ///
 /// # Arguments
 ///
 /// * `process` -  \[in\] A mutable reference to the `Process` instance.
-/// * `qubits` -  \[in\] A pointer to an array of references to `Qubit` instances.
+/// * `qubits` -  \[in\] A pointer to an array of qubit indices to be pushed onto the control stack.
 /// * `qubits_size` -  \[in\] The size of the `qubits` array.
 ///
 /// # Returns
 ///
 /// An integer representing the error code. `0` indicates success.
 ///
 /// # Safety
@@ -377,22 +450,46 @@
 #[no_mangle]
 pub extern "C" fn ket_process_adj_end(process: &mut Process) -> i32 {
     trace!("ket_process_adj_end()");
 
     wrapper(process.adj_end())
 }
 
+/// Prepares the `Process` instance for execution.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
 #[no_mangle]
 pub extern "C" fn ket_process_prepare_for_execution(process: &mut Process) -> i32 {
     trace!("ket_process_prepare_for_execution()");
 
     wrapper(process.prepare_for_execution())
 }
 
+/// Gets the JSON representation of the instructions in the `Process` instance.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+/// * `buffer` -  \[in/out\] A mutable pointer to a buffer to store the JSON representation.
+/// * `buffer_size` -  \[in\] The size of the provided buffer.
+/// * `write_size` -  \[out\] A mutable pointer to the actual size of the written data.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_process_instructions_json(
     process: &mut Process,
     buffer: *mut u8,
     buffer_size: usize,
     write_size: &mut usize,
 ) -> i32 {
@@ -403,15 +500,30 @@
         let buffer = unsafe { std::slice::from_raw_parts_mut(buffer, buffer_size) };
         buffer[..*write_size].copy_from_slice(instructions);
     }
 
     KetError::Success.error_code()
 }
 
+/// Gets the JSON representation of the metadata in the `Process` instance.
+///
+/// # Arguments
+///
+/// * `process` -  \[in\] A mutable reference to the `Process` instance.
+/// * `buffer` -  \[in/out\] A mutable pointer to a buffer to store the JSON representation.
+/// * `buffer_size` -  \[in\] The size of the provided buffer.
+/// * `write_size` -  \[out\] A mutable pointer to the actual size of the written data.
+///
+/// # Returns
+///
+/// An integer representing the error code. `0` indicates success.
+///
 /// # Safety
+///
+/// This function is marked as unsafe due to the use of raw pointers.
 #[no_mangle]
 pub unsafe extern "C" fn ket_process_metadata_json(
     process: &mut Process,
     buffer: *mut u8,
     buffer_size: usize,
     write_size: &mut usize,
 ) -> i32 {
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/src/error.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,108 @@
 // SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 // SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 //
 // SPDX-License-Identifier: Apache-2.0
 
-use std::{error::Error, fmt::Display, result};
+//! This module defines the error types used in the quantum programming library.
 
-#[derive(Debug, Clone, Copy)]
+use std::result;
+/// Enumeration of possible errors in the quantum processing library.
+#[derive(thiserror::Error, Debug, Clone, Copy)]
 #[repr(i32)]
+#[allow(missing_docs)]
 pub enum KetError {
+    #[error("The operation completed successfully.")]
     Success,
+
+    #[error("Cannot set a qubit as a control twice.")]
     ControlTwice,
+
+    #[error("Requested data is not available.")]
     DataNotAvailable,
+
+    #[error("Cannot operate with a deallocated qubit.")]
     DeallocatedQubit,
+
+    #[error("The provided qubit index is out of bounds.")]
     QubitIndexOutOfBounds,
+
+    #[error("The number of qubits exceeds the allowed limit.")]
     NumberOfQubitsExceeded,
+
+    #[error("No inverse scope to end.")]
     NoAdj,
+
+    #[error("No control scope to end.")]
     NoCtrl,
+
+    #[error("Cannot apply a non-gate instruction within a controlled or inverse scope.")]
     NonGateInstructionInAdj,
+
+    #[error("A qubit cannot be both targeted and controlled at the same time.")]
     TargetInControl,
+
+    #[error("Cannot append statements to a terminated process.")]
     ProcessReadyToExecute,
+
+    #[error("Result does not contain the expected number of values.")]
     UnexpectedResultData,
+
+    #[error("Cannot dump qubits (feature disabled).")]
     DumpNotAllowed,
+
+    #[error("Cannot calculate the expected value (feature disabled).")]
     ExpValueNotAllowed,
+
+    #[error("Cannot sampling qubits (feature disabled).")]
     SampleNotAllowed,
+
+    #[error("Cannot measure qubit (feature disabled).")]
     MeasureNotAllowed,
+
+    #[error("The provided buffer is too small.")]
     SmallBufferSize,
+
+    #[error("An undefined error occurred.")]
     UndefinedError,
 }
 
+/// Alias for a `Result` type using `KetError` as the error variant.
 pub type Result<T> = result::Result<T, KetError>;
 
 impl KetError {
-    pub fn to_str(&self) -> &'static str {
-        match self {
-            KetError::Success => "The operation completed successfully.",
-            KetError::ControlTwice => "Cannot set a qubit as a control twice.",
-            KetError::DeallocatedQubit => "Cannot operate with a deallocated qubit.",
-            KetError::NoAdj => "No inverse scope to end.",
-            KetError::NoCtrl => "No control scope to end.",
-            KetError::NonGateInstructionInAdj => {
-                "Cannot apply a non-gate instruction within a controlled or inverse scope."
-            }
-            KetError::TargetInControl => {
-                "A qubit cannot be both targeted and controlled at the same time."
-            }
-            KetError::ProcessReadyToExecute => "Cannot append statements to a terminated process.",
-            KetError::UnexpectedResultData => {
-                "Result does not contain the expected number of values."
-            }
-            KetError::UndefinedError => "An undefined error occurred.",
-            KetError::DataNotAvailable => "Requested data is not available.",
-            KetError::DumpNotAllowed => "Cannot dump qubits (feature disabled).",
-            KetError::MeasureNotAllowed => "Cannot measure qubit (feature disabled).",
-            KetError::QubitIndexOutOfBounds => "The provided qubit index is out of bounds.",
-            KetError::NumberOfQubitsExceeded => "The number of qubits exceeds the allowed limit.",
-            KetError::ExpValueNotAllowed => {
-                "Cannot calculate the expected value (feature disabled)."
-            }
-            KetError::SampleNotAllowed => "Cannot sampling qubits (feature disabled).",
-            KetError::SmallBufferSize => "The provided buffer is too small.",
-        }
-    }
-
+    /// Returns the numeric error code associated with the error variant.
     pub fn error_code(&self) -> i32 {
         *self as i32
     }
 
-    pub fn from_error_code(error_code: i32) -> KetError {
+    /// Converts an error code to a `KetError` variant.
+    ///
+    /// # Safety
+    ///
+    /// This function is unsafe because it assumes that the error code is valid.
+    pub unsafe fn from_error_code(error_code: i32) -> KetError {
         unsafe { std::mem::transmute(error_code) }
     }
 }
 
-impl Display for KetError {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        write!(f, "{}", self.to_str())
-    }
-}
-
-impl Error for KetError {}
-
 #[cfg(test)]
 mod tests {
     use super::KetError;
 
     #[test]
     fn success_is_zero() {
         assert!(KetError::Success.error_code() == 0)
     }
 
     #[test]
     fn print_error_code() {
         let mut error_code = 0;
         loop {
-            let error = KetError::from_error_code(error_code);
+            let error = unsafe { KetError::from_error_code(error_code) };
             let error_str = format!("{:#?}", error);
             let error_str = error_str
                 .split_inclusive(char::is_uppercase)
                 .map(|part| {
                     let size = part.len();
                     let lest = part.chars().last().unwrap();
                     if size > 1 && char::is_uppercase(lest) {
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/libs/libket/src/process.rs` & `ket-lang-0.7rc1/src/ket/clib/libs/libket/src/process.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,105 @@
 // SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 // SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 //
 // SPDX-License-Identifier: Apache-2.0
 
+//! This module contains the `Process` struct, which encapsulates the necessary information for
+//! handling qubit allocations and creating quantum circuits.
+
 use log::info;
 
 use crate::{
     error::{KetError, Result},
     ir::{Instruction, Metadata, PauliHamiltonian, ProcessStatus, QuantumGate, ResultData},
-    objects::{Configuration, Dump, ExpValue, Measurement, QubitStatus, Sample},
+    objects::{Dump, ExpValue, Measurement, QubitStatus, Sample},
+    Configuration,
 };
 
-/// Represents a quantum process.
+/// Quantum Process for managing qubit allocation and circuit creation.
+///
+/// This struct encapsulates the necessary information for handling qubit allocations and
+/// creating quantum circuits. It provides functions to apply quantum gates, measure
+/// qubits, and execute quantum code.
+///
+/// # Examples
+///
+/// ```rust
+/// # use ket::error::KetError;
+/// use ket::{Configuration, Process, QuantumGate};
+///
+/// # fn main() -> Result<(), KetError> {
+/// // Configuration instance must be provided by the quantum execution.
+/// // See the KBW documentation for examples.
+/// let configuration = Configuration::new(2);
+///
+/// // Create a new process with the provided configurations.
+/// // The configuration will specify the maximum number of qubits the quantum
+/// // execution can handle, the execution mode, and more.
+/// let mut process = Process::new(configuration);
+///
+/// // Allocate qubits and return their references for later usage.
+/// let qubit_a = process.allocate_qubit()?;
+/// let qubit_b = process.allocate_qubit()?;
+///
+/// // Apply a Hadamard gate to the first qubit.
+/// process.apply_gate(QuantumGate::Hadamard, qubit_a)?;
+///
+/// // Push the first qubit to the control stack, apply a Pauli X gate to the second qubit,
+/// // and pop the qubit from the control stack.
+/// process.ctrl_push(&[qubit_a])?;
+/// process.apply_gate(QuantumGate::PauliX, qubit_b)?;
+/// process.ctrl_pop()?;
+///
+/// // Measure the qubits and return the results references.
+/// let m_a = process.measure(&[qubit_a])?;
+/// let m_b = process.measure(&[qubit_b])?;
+///
+/// # Ok(())
+/// # }
+/// ```
 pub struct Process {
-    /// Metrics associated with the process.
+    /// Metadata generated in the process lifetime
     metadata: Metadata,
 
-    /// Features associated with the process.
+    /// Configuration provided by the quantum executor (QPU or Simulator)
     config: Configuration,
 
-    /// The quantum circuit
+    /// List of quantum instructions (the quantum circuit)
     instructions: Vec<Instruction>,
 
-    /// Control stack for managing nested control scopes.
+    /// Qubit stack for managing nested control scopes.
     ctrl_stack: Vec<Vec<usize>>,
+
+    /// Control qubit list generated from the control stack
     ctrl_list: Vec<usize>,
     ctrl_list_is_up_to_date: bool,
 
-    /// Inverse instructions stack for managing nested inverse scopes.
+    /// Instructions stack fo handling nested inverse scopes
     adj_stack: Vec<Vec<Instruction>>,
 
-    /// List of futures associated with the process.
+    /// List of measurement results
     measurements: Vec<Measurement>,
 
     /// List of expected values
     exp_values: Vec<ExpValue>,
 
+    /// List of samples result
     samples: Vec<Sample>,
 
-    /// List of dump data associated with the process.
+    /// List of quantum state dump results
     dumps: Vec<Dump>,
 
+    /// Number of qubits allocated
     qubit_allocated: usize,
     qubits: Vec<QubitStatus>,
 }
 
 impl Process {
-    /// Creates a new `Process` with the specified process ID, using default values for other fields.
-    ///
-    /// # Arguments
-    ///
-    /// * `pid` - The process ID.
-    ///
-    /// # Returns
-    ///
-    /// A new `Process` instance.
+    /// Creates a new `Process` with the given configurations
     pub fn new(config: Configuration) -> Self {
         Self {
             metadata: Metadata::new(config.live_quantum_execution.is_some()),
             config,
             instructions: Default::default(),
             ctrl_stack: Default::default(),
             ctrl_list: Default::default(),
@@ -69,74 +110,91 @@
             samples: Default::default(),
             dumps: Default::default(),
             qubit_allocated: Default::default(),
             qubits: Default::default(),
         }
     }
 
+    /// Returns a list of control qubits
+    ///
+    /// Update the control qubits list if necessary and return it.
     fn get_control_qubits(&mut self) -> &[usize] {
         if !self.ctrl_list_is_up_to_date {
             self.ctrl_list_is_up_to_date = true;
             self.ctrl_list = Vec::new();
             for inner_ctrl in self.ctrl_stack.iter() {
                 self.ctrl_list.extend(inner_ctrl.iter());
             }
         }
         &self.ctrl_list
     }
 
+    /// Return an error if the given qubit index is in the control qubit list
     fn assert_target_not_in_control(&mut self, target: usize) -> Result<()> {
         if self.get_control_qubits().contains(&target) {
             Err(KetError::TargetInControl)
         } else {
             Ok(())
         }
     }
 
+    /// Return an error if the given qubit index has the allocated status `false`
     fn assert_qubit_allocated(&self, qubit: usize) -> Result<()> {
         let qubit = self.qubits.get(qubit);
         match qubit {
             Some(qubit) => {
                 if !qubit.allocated {
                     Err(KetError::DeallocatedQubit)
                 } else {
                     Ok(())
                 }
             }
             None => Err(KetError::QubitIndexOutOfBounds),
         }
     }
 
+    /// Return and error if the process is read for execute
     fn assert_not_ready_for_execution(&self) -> Result<()> {
         match self.metadata.status {
             ProcessStatus::Building | ProcessStatus::Live => Ok(()),
             _ => Err(KetError::ProcessReadyToExecute),
         }
     }
 
+    /// Returns an error if there are no inverse scopes opened
     fn assert_not_adj(&self) -> Result<()> {
         if self.adj_stack.is_empty() {
             Ok(())
         } else {
             Err(KetError::NonGateInstructionInAdj)
         }
     }
 
-    /// Allocates a qubit in the current process.
-    ///
-    /// # Arguments
+    /// Allocate a qubit and return its index.
     ///
-    /// * `dirty` - A flag indicating whether the allocated qubit can be in a dirty state.
+    /// The qubit index resulting from the allocation is used in quantum gate application,
+    /// measurement, quantum state dump, and expected value calculations.
     ///
-    /// # Returns
+    /// # Examples
     ///
-    /// A result containing the allocated `Qubit` if successful, or an error if allocation fails.
-    /// Possible error variants include `KetError::DirtyNotAllowed` if dirty qubits are not allowed,
-    /// and other errors related to instruction addition or qubit management.
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_index = process.allocate_qubit()?;
+    /// // Now you can use the allocated qubit_index in quantum operations.
+    /// # Ok(())
+    /// # }
+    /// ```
+    /// # Errors
     ///
+    /// Returns an error if the process is in an inverse scope, if it is ready for
+    /// execution, or if the number of allocated qubits exceeds the configured limit.
     pub fn allocate_qubit(&mut self) -> Result<usize> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
         if self.qubit_allocated >= self.config.num_qubits {
             return Err(KetError::NumberOfQubitsExceeded);
         }
 
@@ -154,28 +212,35 @@
         if let Some(processor) = self.config.live_quantum_execution.as_mut() {
             processor.alloc(index);
         }
 
         Ok(index)
     }
 
-    /// Frees a previously allocated qubit in the current process.
-    ///
-    /// # Arguments
+    /// Frees a previously allocated qubit
     ///
-    /// * `qubit` - A mutable reference to the qubit to be freed.
-    /// * `dirty` - A flag indicating whether the qubit should be freed in a dirty state.
+    /// # Examples
     ///
-    /// # Returns
-    ///
-    /// A result indicating the success or failure of the operation.
-    /// Possible error variants include `KetError::DirtyNotAllowed` if dirty qubits are not allowed,
-    /// `KetError::FreeNotAllowed` if freeing qubits is not allowed,
-    /// and other errors related to instruction addition or qubit management.
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_index = process.allocate_qubit()?;
+    /// // Perform quantum operations...
+    /// process.free_qubit(qubit_index)?;
+    /// // Qubit has been freed and can no longer be used in quantum operations.
+    /// # Ok(())
+    /// # }
+    /// ```
+    /// # Errors
     ///
+    /// Returns an error if the process is in an inverse scope, if it is ready for
+    /// execution, or if the specified qubit has not been allocated.
     pub fn free_qubit(&mut self, qubit: usize) -> Result<()> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
         self.assert_qubit_allocated(qubit)?;
 
         self.instructions.push(Instruction::Free { target: qubit });
 
@@ -184,29 +249,42 @@
         if let Some(processor) = self.config.live_quantum_execution.as_mut() {
             processor.free(qubit);
         }
 
         Ok(())
     }
 
-    /// Applies a quantum gate to a target qubit in the current process.
-    ///
-    /// # Arguments
+    /// Applies a quantum gate to a target qubit
     ///
-    /// * `gate` - The quantum gate to be applied.
-    /// * `target` - A reference to the target qubit.
+    /// This function considers the control qubit list to apply the quantum gate
+    /// in the target qubit.
     ///
-    /// # Returns
-    ///
-    /// A result indicating the success or failure of the operation.
-    /// Possible error variants include `KetError::QubitNotAllocated` if the target qubit is not allocated,
-    /// `KetError::PidMismatch` if the target qubit belongs to a different process,
-    /// `KetError::TargetInControl` if the target qubit is also a control qubit,
-    /// and other errors related to instruction addition or gate decomposition.
+    /// If the process has an opened inverse scope, the gate will only be applied
+    /// when the scope is closed.
     ///
+    /// # Examples
+    ///
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process, QuantumGate};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_index = process.allocate_qubit()?;
+    /// process.apply_gate(QuantumGate::Hadamard, qubit_index)?;
+    /// // Perform additional quantum operations...
+    /// # Ok(())
+    /// # }
+    /// ```
+    ///
+    /// # Errors
+    ///
+    /// Returns an error if the process is ready for execution, if the specified
+    /// qubit has not been allocated, or if the target qubit is part of the control
+    ///  qubits.
     pub fn apply_gate(&mut self, gate: QuantumGate, target: usize) -> Result<()> {
         self.assert_not_ready_for_execution()?;
         self.assert_qubit_allocated(target)?;
         self.assert_target_not_in_control(target)?;
         let control = self.get_control_qubits().to_vec();
 
         if self.config.decompose {
@@ -246,28 +324,40 @@
                 control,
             });
         }
 
         Ok(())
     }
 
-    /// Measures the specified qubits in the current process.
-    ///
-    /// # Arguments
-    ///
-    /// * `qubits` - An array of mutable references to the qubits to be measured.
-    ///
-    /// # Returns
-    ///
-    /// A result containing a `Future` representing the measurement result if successful, or an error if measurement fails.
-    /// Possible error variants include `KetError::MeasureNotAllowed` if measuring qubits is not allowed,
-    /// `KetError::PidMismatch` if any of the qubits belong to a different process,
-    /// `KetError::DeallocatedQubit` if a qubit is not allocated,
-    /// and other errors related to instruction addition or future creation.
+    /// Measures the specified qubits
     ///
+    /// This function performs measurements on the specified qubits.
+    /// It updates the internal state of the process, records measurement instructions, and
+    /// returns the index of the measurement result.
+    ///
+    /// # Examples
+    ///
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_index = process.allocate_qubit()?;
+    /// let measurement_index = process.measure(&[qubit_index])?;
+    /// // Perform additional quantum operations or measurements...
+    /// # Ok(())
+    /// # }
+    /// ```
+    ///     
+    /// # Errors
+    ///
+    /// Returns an error if the process is in an adjacent scope, if the process
+    /// is ready for execution, or if measurements are not allowed based on the
+    /// process configuration.
     pub fn measure(&mut self, qubits: &[usize]) -> Result<usize> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
         if !self.config.allow_measure {
             return Err(KetError::MeasureNotAllowed);
         }
 
@@ -299,14 +389,55 @@
             qubits: qubits.to_vec(),
             output: measure_index,
         });
 
         Ok(measure_index)
     }
 
+    /// Calculates the expected values of a Pauli Hamiltonian
+    ///
+    /// This function calculates the expected values of a Pauli Hamiltonian. It updates
+    /// the internal state of the process, records the calculation instructions, and
+    /// returns the index of the expected value result.
+    ///
+    /// # Examples
+    ///
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// use ket::{Pauli, PauliHamiltonian, PauliTerm};
+    ///
+    /// # fn main() -> Result<(), KetError> {
+    /// # let configuration = Configuration::new(2);
+    /// # let mut process = Process::new(configuration);
+    /// let qubit_a = process.allocate_qubit()?;
+    /// let qubit_b = process.allocate_qubit()?;
+    /// let _exp = process.exp_values(PauliHamiltonian {
+    ///     coefficients: vec![1.0],
+    ///     products: vec![vec![
+    ///         PauliTerm {
+    ///             pauli: Pauli::PauliX,
+    ///             qubit: qubit_a,
+    ///         },
+    ///         PauliTerm {
+    ///             pauli: Pauli::PauliX,
+    ///             qubit: qubit_b,
+    ///         },
+    ///     ]],
+    /// })?;
+    /// # Ok(())
+    /// # }    
+    /// ```
+    ///     
+    /// # Errors
+    ///
+    /// Returns an error if the process is in an adjacent scope, if the process
+    /// is ready for execution, or if expected value calculations are not allowed based on the
+    /// process configuration. Additionally, it verifies whether the qubits involved in the
+    /// Hamiltonian are allocated.
     pub fn exp_values(&mut self, hamiltonian: PauliHamiltonian) -> Result<usize> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
 
         if !self.config.allow_exp_value {
             return Err(KetError::ExpValueNotAllowed);
         }
@@ -336,14 +467,43 @@
         if !self.config.continue_after_exp_value {
             self.prepare_for_execution()?;
         }
 
         Ok(index)
     }
 
+    /// Performs sampling on specified qubits
+    ///
+    /// This function performs sampling on the specified qubits with a specified number of shots.
+    /// It updates the internal state of the process, records sampling instructions, and
+    /// returns the index of the sample result.
+    ///
+    /// # Examples
+    ///
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_a = process.allocate_qubit()?;
+    /// let qubit_b = process.allocate_qubit()?;
+    /// let shots = 1000;
+    /// let sample_index = process.sample(&[qubit_a, qubit_b], shots)?;
+    /// // Perform additional quantum operations or sampling...
+    /// # Ok(())
+    /// # }
+    /// ```
+    ///     
+    /// # Errors
+    ///
+    /// Returns an error if the process is in an adjacent scope, if the process
+    /// is ready for execution, or if sampling is not allowed based on the
+    /// process configuration. Additionally, it verifies whether the qubits involved in the
+    /// sampling are allocated.
     pub fn sample(&mut self, qubits: &[usize], shots: u64) -> Result<usize> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
 
         if !self.config.allow_sample {
             return Err(KetError::SampleNotAllowed);
         }
@@ -375,25 +535,41 @@
         if !self.config.continue_after_exp_value {
             self.prepare_for_execution()?;
         }
 
         Ok(index)
     }
 
-    /// Dumps the state of the specified qubits.
-    ///
-    /// # Arguments
+    /// Dumps the state of specified qubits
     ///
-    /// * `qubits` - The mutable references to the qubits to be dumped.
+    /// This function dumps the state of the specified qubits. It updates the internal state
+    /// of the process, records dump instructions, and returns the index of the dump result.
     ///
-    /// # Returns
-    ///
-    /// A result containing a new dump object if dumping is allowed by the features,
-    /// or an error (`KetError::DumpNotAllowed`) if dumping is not allowed.
+    /// # Examples
     ///
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_a = process.allocate_qubit()?;
+    /// let qubit_b = process.allocate_qubit()?;
+    /// let dump_index = process.dump(&[qubit_a, qubit_b])?;
+    /// // Perform additional quantum operations or dumps...
+    /// # Ok(())
+    /// # }
+    /// ```
+    ///     
+    /// # Errors
+    ///
+    /// Returns an error if the process is in an adjacent scope, if the process
+    /// is ready for execution, or if dumping is not allowed based on the
+    /// process configuration. Additionally, it verifies whether the qubits involved in the
+    /// dump operation are allocated.
     pub fn dump(&mut self, qubits: &[usize]) -> Result<usize> {
         self.assert_not_adj()?;
         self.assert_not_ready_for_execution()?;
 
         if !self.config.allow_dump {
             return Err(KetError::DumpNotAllowed);
         }
@@ -423,27 +599,39 @@
         if !self.config.continue_after_dump {
             self.prepare_for_execution()?;
         }
 
         Ok(dump_index)
     }
 
-    /// Pushes control qubits onto the control stack.
-    ///
-    /// # Arguments
+    /// Pushes control qubits onto the control stack
     ///
-    /// * `qubits` - An array of references to the control qubits.
+    /// This function pushes control qubits onto the control stack. It updates the internal state
+    /// of the process and ensures that qubits are not controlled more than once.
     ///
-    /// # Returns
+    /// # Examples
     ///
-    /// A result indicating success or an error if the control configuration is invalid.
-    /// Possible error variants include `KetError::DeallocatedQubit` if any of the control qubits are not allocated,
-    /// `KetError::PidMismatch` if any of the control qubits belong to a different process,
-    /// and `KetError::ControlTwice` if a control qubit is included in multiple control configurations.
+    /// ```rust
+    /// # use ket::error::KetError;
+    /// # use ket::{Configuration, Process};
+    /// #
+    /// # fn main() -> Result<(), KetError> {
+    /// # let mut process = Process::new(Configuration::new(2));
+    /// let qubit_a = process.allocate_qubit()?;
+    /// let qubit_b = process.allocate_qubit()?;
+    /// process.ctrl_push(&[qubit_a, qubit_b])?;
+    /// // Perform additional quantum operations...
+    /// # Ok(())
+    /// # }
+    /// ```
+    ///     
+    /// # Errors
     ///
+    /// Returns an error if the process is ready for execution or if the control qubits
+    /// are allocated more than once during a control operation.
     pub fn ctrl_push(&mut self, qubits: &[usize]) -> Result<()> {
         self.assert_not_ready_for_execution()?;
         let qubits = qubits.to_vec();
         for ctrl_list in self.ctrl_stack.iter() {
             for qubit in &qubits {
                 self.assert_qubit_allocated(*qubit)?;
                 if ctrl_list.contains(qubit) {
@@ -455,51 +643,47 @@
         self.ctrl_stack.push(qubits);
 
         self.ctrl_list_is_up_to_date = false;
 
         Ok(())
     }
 
-    /// Pops the top control qubit configuration from the control stack.
-    ///
-    /// # Returns
-    ///
-    /// A result indicating success or an error if the control stack is empty (`KetError::NoCtrl`).
+    /// Pops the last added control qubits from the control stack
+    ///     
+    /// # Errors
     ///
+    /// Returns an error if the process is ready for execution or if there are no control
+    /// configurations on the control stack to pop.
     pub fn ctrl_pop(&mut self) -> Result<()> {
         self.assert_not_ready_for_execution()?;
         self.ctrl_list_is_up_to_date = false;
 
         match self.ctrl_stack.pop() {
             Some(_) => Ok(()),
             None => Err(KetError::NoCtrl),
         }
     }
 
-    /// Begins an adjoint block, where gates are inverted upon insertion.
-    ///
-    /// # Returns
+    /// Begins an adjoint block, where gates are inverted upon insertion
     ///
-    /// A result indicating success or an error if there are issues with the current block.
-    /// Possible error variants include `KetError::TerminatedBlock` if the current block ended.
+    /// # Errors
     ///
+    /// Returns an error if the process is ready for execution.
     pub fn adj_begin(&mut self) -> Result<()> {
         self.assert_not_ready_for_execution()?;
 
         self.adj_stack.push(Vec::new());
         Ok(())
     }
 
-    /// Ends the adjoint block, reverting to normal gate insertion.
+    /// Ends the adjoint block, reverting to normal gate insertion
     ///
-    /// # Returns
-    ///
-    /// A result indicating success or an error if there are issues with the current block.
-    /// Possible error variants include `KetError::TerminatedBlock` if the current block ended.
+    /// # Errors
     ///
+    /// Returns an error if the process is ready for execution or if there is no adjoint block to end.
     pub fn adj_end(&mut self) -> Result<()> {
         self.assert_not_ready_for_execution()?;
 
         if self.adj_stack.is_empty() {
             return Err(KetError::NoAdj);
         }
 
@@ -530,14 +714,15 @@
                 self.adj_stack.last_mut().unwrap().push(instruction);
             }
         }
 
         Ok(())
     }
 
+    /// Prepares the process for quantum execution
     pub fn prepare_for_execution(&mut self) -> Result<()> {
         if let ProcessStatus::Building = self.metadata.status {
             let mut result = None;
             if let Some(processor) = self.config.batch_execution.as_mut() {
                 processor.submit_execution(&self.instructions);
                 self.metadata.status = ProcessStatus::Running;
                 result = Some(processor.get_result());
@@ -549,54 +734,49 @@
             if let Some(result) = result {
                 self.set_result(result)?;
             }
         }
         Ok(())
     }
 
+    /// Returns the status of the specified qubit
     pub fn get_qubit_status(&self, qubit: usize) -> &QubitStatus {
         &self.qubits[qubit]
     }
 
+    /// Returns the measurement result at the specified index
     pub fn get_measurement(&self, index: usize) -> &Measurement {
         &self.measurements[index]
     }
 
+    /// Returns the expected value result at the specified index
     pub fn get_exp_value(&self, index: usize) -> &ExpValue {
         &self.exp_values[index]
     }
 
+    /// Returns the sample result at the specified index
     pub fn get_sample(&self, index: usize) -> &Sample {
         &self.samples[index]
     }
 
+    /// Returns the dump result at the specified index
     pub fn get_dump(&self, index: usize) -> &Dump {
         &self.dumps[index]
     }
 
-    /// Returns a reference to the metrics of the quantum code.
-    ///
-    /// # Returns
-    ///
-    /// A reference to the `Metrics` struct containing various metrics of the quantum code.
-    ///
+    /// Return process metadata
     pub fn get_metadata(&self) -> &Metadata {
         &self.metadata
     }
 
-    /// Sets the result of the quantum code execution.
-    ///
-    /// # Arguments
-    ///
-    /// * `result` - The result data containing the future values, dump values, and execution time.
-    ///
-    /// # Returns
-    ///
-    /// A `Result` indicating success (`Ok`) or an error (`Err`) if the result data is unexpected.
+    /// Set the quantum execution result
     ///
+    /// This function allow to manually set the quantum execution result for the process.
+    /// However, this function should only be used for testing purposes. The result must be provided
+    /// by the quantum executor set in the configuration.
     pub fn set_result(&mut self, mut results: ResultData) -> Result<()> {
         if self.measurements.len() != results.measurements.len()
             || self.exp_values.len() != results.exp_values.len()
             || self.samples.len() != results.samples.len()
             || self.dumps.len() != results.dumps.len()
         {
             return Err(KetError::UnexpectedResultData);
@@ -636,53 +816,24 @@
 
         self.metadata.execution_time = results.execution_time;
 
         self.metadata.status = ProcessStatus::Terminated;
         Ok(())
     }
 
+    /// Return the instructions in JSON
+    ///
+    /// This functions is used in the C API for get the instructions out of the process.
     pub(crate) fn instructions_json(&self) -> String {
         serde_json::to_string(&self.instructions).unwrap()
     }
 
+    /// Return the metadata in JSON
+    ///
+    /// This functions is used in the C API for get the metadata out of the process.
     pub(crate) fn metadata_json(&self) -> String {
         serde_json::to_string(&self.metadata).unwrap()
     }
 }
 
 #[cfg(test)]
-mod tests {
-    use crate::ir::Angle;
-
-    use super::*;
-
-    #[test]
-    fn bell_state() -> Result<()> {
-        let feature = Configuration::new(2);
-        let mut process = Process::new(feature);
-        let qubit_a = process.allocate_qubit()?;
-        let qubit_b = process.allocate_qubit()?;
-
-        process.apply_gate(QuantumGate::Hadamard, qubit_a)?;
-        process.ctrl_push(&[qubit_a])?;
-        process.apply_gate(QuantumGate::RotationX(Angle::pi()), qubit_b)?;
-        process.ctrl_pop()?;
-
-        let m_a = process.measure(&[qubit_a])?;
-        let m_b = process.measure(&[qubit_b])?;
-
-        process.prepare_for_execution()?;
-
-        process.set_result(ResultData {
-            measurements: vec![1, 1],
-            exp_values: vec![],
-            samples: vec![],
-            dumps: vec![],
-            execution_time: None,
-        })?;
-
-        println!("{:?}", process.get_measurement(m_a));
-        println!("{:?}", process.get_measurement(m_b));
-
-        Ok(())
-    }
-}
+mod tests {}
```

### Comparing `ket-lang-0.7rc0/src/ket/clib/wrapper.py` & `ket-lang-0.7rc1/src/ket/clib/wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -45,33 +45,42 @@
         self.output = output
         self.error_message = error_message
 
     def __call__(self, *args):
         out = [c_type() for c_type in self.output]
         error_code = self.c_call(*args, *out)
         if error_code != 0:
-            size = c_size_t()
-            error_msg = self.error_message(error_code, size)
-            raise CLibError(
-                self.lib_name + ": " + from_u8_to_str(error_msg, size), error_code
-            )
+            error_msg_buffer_size = 128
+            error_message_buffer = (c_uint8 * error_msg_buffer_size)()
+            write_size = c_size_t()
+            while (
+                self.error_message(
+                    error_code, error_message_buffer, error_msg_buffer_size, write_size
+                )
+                != 0
+            ):
+                error_msg_buffer_size = write_size.value
+                error_message_buffer = (c_uint8 * error_msg_buffer_size)()
+
+            error_msg = bytearray(error_message_buffer[: write_size.value]).decode()
+            raise CLibError(f"{self.lib_name}: {error_msg}", error_code)
         if len(out) == 1:
             return out[0]
         if len(out) != 0:
             return out
         return None
 
 
 def load_lib(lib_name, lib_path, api_argtypes, error_message):
     """Load clib"""
 
     lib = cdll.LoadLibrary(lib_path)
     error_message = lib.__getattr__(error_message)  # pylint: disable=C2801
-    error_message.argtypes = [c_int32, POINTER(c_size_t)]
-    error_message.restype = POINTER(c_uint8)
+    error_message.argtypes = [c_int32, POINTER(c_uint8), c_size_t, POINTER(c_size_t)]
+    error_message.restype = c_int32
 
     api = {}
     for name in api_argtypes:
         c_call = lib.__getattr__(name)  # pylint: disable=C2801
         c_call.argtypes = [
             *api_argtypes[name][0],
             *[POINTER(t) for t in api_argtypes[name][1]],
```

### Comparing `ket-lang-0.7rc0/src/ket/expv.py` & `ket-lang-0.7rc1/src/ket/expv.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from __future__ import annotations
 
 # SPDX-FileCopyrightText: 2020 Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>
 # SPDX-FileCopyrightText: 2020 Rafael de Santiago <r.santiago@ufsc.br>
 #
 # SPDX-License-Identifier: Apache-2.0
 
+# pylint: disable=duplicate-code
+
 from ctypes import c_int32, c_size_t
 from typing import Literal
 
 from .base import Process, Quant
 
 from .clib.libket import API
```

### Comparing `ket-lang-0.7rc0/src/ket/gates.py` & `ket-lang-0.7rc1/src/ket/gates.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,16 +77,14 @@
     "SD",
     "TD",
     "CNOT",
     "SWAP",
     "RXX",
     "RZZ",
     "RYY",
-    "flip_to_control",
-    "phase_oracle",
 ]
 
 
 def _gate_docstring(name, matrix, effect=None) -> str:
     return f"""Apply the {name} gate.
     
     .. csv-table::
@@ -334,15 +332,17 @@
     r"T^\dagger\left|1\right> = & e^{-i\pi/4}\left|1\right> \end{matrix}",
 )
 
 
 def CNOT(  # pylint: disable=invalid-name missing-function-docstring
     control_qubit: Quant, target_qubit: Quant
 ) -> tuple[Quant, Quant]:
-    return ctrl(control_qubit, X)(target_qubit)
+    for c, t in zip(control_qubit, target_qubit):
+        ctrl(c, X)(t)
+    return control_qubit, target_qubit
 
 
 CNOT.__doc__ = _gate_docstring(
     "Controlled NOT",
     r"\begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \end{bmatrix}",  # pylint: disable=line-too-long
     r"\begin{matrix} \text{CNOT}\left|00\right> = & \left|00\right> \\"
     r"\text{CNOT}\left|01\right> = & \left|01\right> \\"
@@ -437,79 +437,7 @@
 RYY.__doc__ = _gate_docstring(
     "YY rotation",
     r"\begin{bmatrix} \cos\frac{\theta}{2} & 0 & 0 & i\sin\frac{\theta}{2} \\"
     r"0 & \cos\frac{\theta}{2} & -i\sin\frac{\theta}{2} & 0 \\"
     r"0 & -i\sin\frac{\theta}{2} & \cos\frac{\theta}{2} & 0 \\"
     r"i\sin\frac{\theta}{2} & 0 & 0 & \cos\frac{\theta}{2} \end{bmatrix}",
 )
-
-
-def flip_to_control(
-    control_state: int | list[int], qubits: Quant | None = None
-) -> Quant | Callable[[Quant], Quant]:
-    r"""Flip qubits from :math:`\ket{\texttt{control_state}}` to :math:`\ket{1\dots1}`.
-
-    The primary usage of this gate is to change the state when controlled applications are applied.
-    For instance, all controlled operations are only applied if the control qubits' state is
-    :math:`\ket{1}`. This gate is useful for using another state as control.
-
-    Example:
-
-        .. code-block:: python
-
-            from ket import *
-
-            p = Process()
-            q = p.alloc(3)
-
-            H(q[:2])
-
-            with around(flip_to_control(0b01), q[:2]):
-                ctrl(q[:2], X)(q[2])
-    """
-
-    def inner(qubits: Quant) -> Quant:
-        if not isinstance(qubits, Quant):
-            qubits = reduce(add, qubits)
-
-        length = len(qubits)
-        if hasattr(control_state, "__iter__"):
-            if len(control_state) != length:
-                raise ValueError(
-                    f"'to' received a list of length {len(control_state)} to use on {length} qubits"
-                )
-        else:
-            if length < control_state.bit_length():
-                raise ValueError(
-                    f"To flip with control_state={control_state} "
-                    f"you need at least {control_state.bit_length()} qubits"
-                )
-
-            state = [int(i) for i in f"{{:0{length}b}}".format(control_state)]
-
-        for i, qubit in zip(state, qubits):
-            if i == 0:
-                X(qubit)
-        return qubits
-
-    if qubits is None:
-        return inner
-    return inner(qubits)
-
-
-def phase_oracle(
-    state: int, qubits: Quant | None = None
-) -> Quant | Callable[[Quant], Quant]:
-    r"""Transform qubits from :math:`\ket{\texttt{state}}` to :math:`-\ket{\texttt{state}}`.
-
-    This gate is useful for marking states in Grover's algorithm.
-    """
-
-    def inner(qubits: Quant) -> Quant:
-        init, last = qubits[:-1], qubits[-1]
-        with around(flip_to_control(state >> 1), init):
-            with around(lambda q: X(q) if state & 1 == 0 else None, last):
-                ctrl(init, Z)(last)
-
-    if qubits is None:
-        return inner
-    return inner(qubits)
```

### Comparing `ket-lang-0.7rc0/src/ket/operations.py` & `ket-lang-0.7rc1/src/ket/operations.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.7rc0/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.7rc1/src/ket_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.7rc0
+Version: 0.7rc1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.7rc0/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.7rc1/src/ket_lang.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/ket/__init__.py
 src/ket/base.py
 src/ket/expv.py
 src/ket/gates.py
+src/ket/lib.py
 src/ket/operations.py
 src/ket/clib/__init__.py
 src/ket/clib/kbw.py
 src/ket/clib/libket.py
 src/ket/clib/wrapper.py
 src/ket/clib/libs/__init__.py
 src/ket/clib/libs/kbw/.git
@@ -36,14 +37,15 @@
 src/ket/clib/libs/libket/Cargo.toml
 src/ket/clib/libs/libket/LICENSE
 src/ket/clib/libs/libket/README.md
 src/ket/clib/libs/libket/.reuse/dep5
 src/ket/clib/libs/libket/LICENSES/Apache-2.0.txt
 src/ket/clib/libs/libket/examples/bell.rs
 src/ket/clib/libs/libket/src/error.rs
+src/ket/clib/libs/libket/src/execution.rs
 src/ket/clib/libs/libket/src/ir.rs
 src/ket/clib/libs/libket/src/lib.rs
 src/ket/clib/libs/libket/src/objects.rs
 src/ket/clib/libs/libket/src/process.rs
 src/ket/clib/libs/libket/src/c_api/error.rs
 src/ket/clib/libs/libket/src/c_api/mod.rs
 src/ket/clib/libs/libket/src/c_api/objects.rs
```

