# Comparing `tmp/arvados-llfuse-1.5.1.tar.gz` & `tmp/arvados-llfuse-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvados-llfuse-1.5.1.tar", last modified: Thu Mar 14 17:10:19 2024, max compression
+gzip compressed data, was "arvados-llfuse-1.5.2.tar", last modified: Fri Apr  5 16:27:11 2024, max compression
```

## Comparing `arvados-llfuse-1.5.1.tar` & `arvados-llfuse-1.5.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/
--rw-r--r--   0 peter     (1000) peter     (1000)    14310 2024-03-14 17:03:21.000000 arvados-llfuse-1.5.1/Changes.rst
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.724598 arvados-llfuse-1.5.1/Include/
--rw-r--r--   0 peter     (1000) peter     (1000)     1839 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/fuse_common.pxd
--rw-r--r--   0 peter     (1000) peter     (1000)     8492 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/Include/fuse_lowlevel.pxd
--rw-r--r--   0 peter     (1000) peter     (1000)      393 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/fuse_opt.pxd
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.724598 arvados-llfuse-1.5.1/Include/libc/
--rw-r--r--   0 peter     (1000) peter     (1000)       13 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/libc/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      546 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/libc/dirent.pxd
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.724598 arvados-llfuse-1.5.1/Include/libc/sys/
--rw-r--r--   0 peter     (1000) peter     (1000)       13 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/libc/sys/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      627 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/Include/libc/sys/statvfs.pxd
--rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/Include/pthread.pxd
--rw-r--r--   0 peter     (1000) peter     (1000)    25960 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)     2743 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1619 2024-03-14 15:17:52.000000 arvados-llfuse-1.5.1/README.rst
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.728598 arvados-llfuse-1.5.1/examples/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     5547 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/examples/lltest.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)    16688 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/examples/passthroughfs.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)    15948 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/examples/tmpfs.py
--rw-r--r--   0 peter     (1000) peter     (1000)       81 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/pyproject.toml
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.728598 arvados-llfuse-1.5.1/rst/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.728598 arvados-llfuse-1.5.1/rst/_static/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/_static/.placeholder
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.728598 arvados-llfuse-1.5.1/rst/_templates/
--rw-r--r--   0 peter     (1000) peter     (1000)       93 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/_templates/localtoc.html
--rw-r--r--   0 peter     (1000) peter     (1000)       80 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/about.rst
--rw-r--r--   0 peter     (1000) peter     (1000)       28 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/changes.rst
--rw-r--r--   0 peter     (1000) peter     (1000)     6955 2024-03-14 15:20:51.000000 arvados-llfuse-1.5.1/rst/conf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2927 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/rst/data.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      816 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/example.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      327 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/fuse_api.rst
--rw-r--r--   0 peter     (1000) peter     (1000)     3226 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/general.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      868 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/gotchas.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      409 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/index.rst
--rw-r--r--   0 peter     (1000) peter     (1000)     2826 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/rst/install.rst
--rw-r--r--   0 peter     (1000) peter     (1000)     2048 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/lock.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      198 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/operations.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      381 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/rst/util.rst
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     7693 2024-03-14 14:41:24.000000 arvados-llfuse-1.5.1/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/src/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     2743 2024-03-14 17:10:19.000000 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1190 2024-03-14 17:10:19.000000 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-03-14 17:10:19.000000 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2024-03-14 17:10:19.000000 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-03-14 17:06:12.000000 arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)     6145 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/darwin_compat.c
--rw-r--r--   0 peter     (1000) peter     (1000)     1376 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/darwin_compat.h
--rw-r--r--   0 peter     (1000) peter     (1000)    19531 2024-03-14 14:40:15.000000 arvados-llfuse-1.5.1/src/fuse_api.pxi
--rw-r--r--   0 peter     (1000) peter     (1000)      963 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/gettime.h
--rw-r--r--   0 peter     (1000) peter     (1000)    23731 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/src/handlers.pxi
--rw-r--r--   0 peter     (1000) peter     (1000)  2942121 2024-03-14 17:06:04.000000 arvados-llfuse-1.5.1/src/llfuse.c
--rw-r--r--   0 peter     (1000) peter     (1000)      924 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/llfuse.h
--rw-r--r--   0 peter     (1000) peter     (1000)     4220 2024-03-14 14:40:15.000000 arvados-llfuse-1.5.1/src/llfuse.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)     3893 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/lock.c
--rw-r--r--   0 peter     (1000) peter     (1000)      383 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/lock.h
--rw-r--r--   0 peter     (1000) peter     (1000)     1940 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.1/src/macros.c
--rw-r--r--   0 peter     (1000) peter     (1000)    21492 2024-03-14 14:40:15.000000 arvados-llfuse-1.5.1/src/misc.pxi
--rw-r--r--   0 peter     (1000) peter     (1000)    19987 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/src/operations.pxi
--rw-r--r--   0 peter     (1000) peter     (1000)     3500 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/src/xattr.h
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/test/
--rw-r--r--   0 peter     (1000) peter     (1000)     3660 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/conftest.py
--rw-r--r--   0 peter     (1000) peter     (1000)       81 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/pytest.ini
--rw-r--r--   0 peter     (1000) peter     (1000)     3885 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/pytest_checklogs.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2962 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/test_api.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)    11770 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/test_examples.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8337 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/test_fs.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1228 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/test_rounding.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3443 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/test/util.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-14 17:10:19.732598 arvados-llfuse-1.5.1/util/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      313 2024-03-14 17:10:16.000000 arvados-llfuse-1.5.1/util/sdist-sign
--rw-r--r--   0 peter     (1000) peter     (1000)     1021 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/util/sphinx_cython.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      270 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.1/util/upload-pypi
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/
+-rw-r--r--   0 peter     (1000) peter     (1000)    14310 2024-04-05 16:14:33.000000 arvados-llfuse-1.5.2/Changes.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/Include/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1839 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/fuse_common.pxd
+-rw-r--r--   0 peter     (1000) peter     (1000)     8492 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/Include/fuse_lowlevel.pxd
+-rw-r--r--   0 peter     (1000) peter     (1000)      393 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/fuse_opt.pxd
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/Include/libc/
+-rw-r--r--   0 peter     (1000) peter     (1000)       13 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/libc/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      546 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/libc/dirent.pxd
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/Include/libc/sys/
+-rw-r--r--   0 peter     (1000) peter     (1000)       13 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/libc/sys/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      627 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/Include/libc/sys/statvfs.pxd
+-rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/Include/pthread.pxd
+-rw-r--r--   0 peter     (1000) peter     (1000)    25960 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)     2893 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1619 2024-04-05 16:14:33.000000 arvados-llfuse-1.5.2/README.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/examples/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     5547 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/examples/lltest.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    16688 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/examples/passthroughfs.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    15948 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/examples/tmpfs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       81 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/pyproject.toml
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/rst/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/rst/_static/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/_static/.placeholder
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.219570 arvados-llfuse-1.5.2/rst/_templates/
+-rw-r--r--   0 peter     (1000) peter     (1000)       93 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/_templates/localtoc.html
+-rw-r--r--   0 peter     (1000) peter     (1000)       80 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/about.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)       28 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/changes.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     6955 2024-04-05 16:14:33.000000 arvados-llfuse-1.5.2/rst/conf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2927 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/rst/data.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      816 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/example.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      327 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/fuse_api.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     3226 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/general.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      868 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/gotchas.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      409 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2826 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/rst/install.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2048 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/lock.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      198 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/operations.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      381 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/rst/util.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     7885 2024-04-05 16:22:05.000000 arvados-llfuse-1.5.2/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/src/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2893 2024-04-05 16:27:11.000000 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1190 2024-04-05 16:27:11.000000 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-05 16:27:11.000000 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        7 2024-04-05 16:27:11.000000 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-03-14 17:06:12.000000 arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)     6145 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/darwin_compat.c
+-rw-r--r--   0 peter     (1000) peter     (1000)     1376 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/darwin_compat.h
+-rw-r--r--   0 peter     (1000) peter     (1000)    19531 2024-04-05 16:20:08.000000 arvados-llfuse-1.5.2/src/fuse_api.pxi
+-rw-r--r--   0 peter     (1000) peter     (1000)      963 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/gettime.h
+-rw-r--r--   0 peter     (1000) peter     (1000)    23731 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/src/handlers.pxi
+-rw-r--r--   0 peter     (1000) peter     (1000)  2942121 2024-04-05 16:25:42.000000 arvados-llfuse-1.5.2/src/llfuse.c
+-rw-r--r--   0 peter     (1000) peter     (1000)      924 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/llfuse.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     4220 2024-04-05 16:20:16.000000 arvados-llfuse-1.5.2/src/llfuse.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)     3893 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/lock.c
+-rw-r--r--   0 peter     (1000) peter     (1000)      383 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/lock.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     1940 2024-03-06 20:32:27.000000 arvados-llfuse-1.5.2/src/macros.c
+-rw-r--r--   0 peter     (1000) peter     (1000)    21492 2024-03-14 14:40:15.000000 arvados-llfuse-1.5.2/src/misc.pxi
+-rw-r--r--   0 peter     (1000) peter     (1000)    19987 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/src/operations.pxi
+-rw-r--r--   0 peter     (1000) peter     (1000)     3500 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/src/xattr.h
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/test/
+-rw-r--r--   0 peter     (1000) peter     (1000)     3660 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/conftest.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       81 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/pytest.ini
+-rw-r--r--   0 peter     (1000) peter     (1000)     3885 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/pytest_checklogs.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2962 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/test_api.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    11770 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/test_examples.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8337 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/test_fs.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1228 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/test_rounding.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3443 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/test/util.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-05 16:27:11.223570 arvados-llfuse-1.5.2/util/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      313 2024-04-05 16:14:33.000000 arvados-llfuse-1.5.2/util/sdist-sign
+-rw-r--r--   0 peter     (1000) peter     (1000)     1021 2024-03-13 00:08:47.000000 arvados-llfuse-1.5.2/util/sphinx_cython.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      278 2024-04-05 16:14:33.000000 arvados-llfuse-1.5.2/util/upload-pypi
```

### Comparing `arvados-llfuse-1.5.1/Changes.rst` & `arvados-llfuse-1.5.2/Changes.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/Include/fuse_common.pxd` & `arvados-llfuse-1.5.2/Include/fuse_common.pxd`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/Include/fuse_lowlevel.pxd` & `arvados-llfuse-1.5.2/Include/fuse_lowlevel.pxd`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/Include/libc/dirent.pxd` & `arvados-llfuse-1.5.2/Include/libc/dirent.pxd`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/Include/libc/sys/statvfs.pxd` & `arvados-llfuse-1.5.2/Include/libc/sys/statvfs.pxd`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/Include/pthread.pxd` & `arvados-llfuse-1.5.2/Include/pthread.pxd`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/LICENSE` & `arvados-llfuse-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/PKG-INFO` & `arvados-llfuse-1.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: arvados-llfuse
-Version: 1.5.1
+Version: 1.5.2
 Summary: Arvados fork of Python bindings for the low-level FUSE API
 Home-page: https://github.com/arvados/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
 Platform: FreeBSD
 Platform: OS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Provides: llfuse
-Requires-Python: >=3.8
+Requires-Python: >=3.5
 License-File: LICENSE
 
 ..
   NOTE: We cannot use sophisticated ReST syntax (like
   e.g. :file:`foo`) here because this isn't rendered correctly
   by PyPi.
```

### Comparing `arvados-llfuse-1.5.1/README.rst` & `arvados-llfuse-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/examples/lltest.py` & `arvados-llfuse-1.5.2/examples/lltest.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/examples/passthroughfs.py` & `arvados-llfuse-1.5.2/examples/passthroughfs.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/examples/tmpfs.py` & `arvados-llfuse-1.5.2/examples/tmpfs.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/conf.py` & `arvados-llfuse-1.5.2/rst/conf.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/data.rst` & `arvados-llfuse-1.5.2/rst/data.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/example.rst` & `arvados-llfuse-1.5.2/rst/example.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/general.rst` & `arvados-llfuse-1.5.2/rst/general.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/gotchas.rst` & `arvados-llfuse-1.5.2/rst/gotchas.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/install.rst` & `arvados-llfuse-1.5.2/rst/install.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/rst/lock.rst` & `arvados-llfuse-1.5.2/rst/lock.rst`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/setup.py` & `arvados-llfuse-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 DEVELOPER_MODE = os.getenv('DEVELOPER_MODE', '0') == '1'
 if DEVELOPER_MODE:
     print('running in developer mode')
     warnings.resetwarnings()
     warnings.simplefilter('default')
 
 
-LLFUSE_VERSION = '1.5.1'
+LLFUSE_VERSION = '1.5.2'
 
 def main():
 
     with open(os.path.join(basedir, 'README.rst')) as fh:
         long_desc = fh.read()
 
     compile_args = pkg_config('fuse', cflags=True, ldflags=False, min_ver='2.8.0')
@@ -106,14 +106,17 @@
           author_email='Nikolaus@rath.org',
           url='https://github.com/arvados/python-llfuse/',
           license='LGPL',
           classifiers=['Development Status :: 4 - Beta',
                        'Intended Audience :: Developers',
                        'Programming Language :: Python',
                        'Programming Language :: Python :: 3',
+                       'Programming Language :: Python :: 3.5',
+                       'Programming Language :: Python :: 3.6',
+                       'Programming Language :: Python :: 3.7',
                        'Programming Language :: Python :: 3.8',
                        'Programming Language :: Python :: 3.9',
                        'Programming Language :: Python :: 3.10',
                        'Programming Language :: Python :: 3.11',
                        'Programming Language :: Python :: 3.12',
                        'Topic :: Software Development :: Libraries :: Python Modules',
                        'Topic :: System :: Filesystems',
@@ -121,15 +124,15 @@
                        'Operating System :: POSIX :: Linux',
                        'Operating System :: MacOS :: MacOS X',
                        'Operating System :: POSIX :: BSD :: FreeBSD'],
           platforms=[ 'Linux', 'FreeBSD', 'OS X' ],
           keywords=['FUSE', 'python' ],
           package_dir={'': 'src'},
           packages=setuptools.find_packages('src'),
-          python_requires='>=3.8',
+          python_requires='>=3.5',
           tests_require=['pytest >= 3.4.0'],
           provides=['llfuse'],
           ext_modules=[Extension('llfuse', c_sources,
                                   extra_compile_args=compile_args,
                                   extra_link_args=link_args)],
           cmdclass={'build_cython': build_cython},
           )
```

### Comparing `arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/PKG-INFO` & `arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: arvados-llfuse
-Version: 1.5.1
+Version: 1.5.2
 Summary: Arvados fork of Python bindings for the low-level FUSE API
 Home-page: https://github.com/arvados/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
 Platform: FreeBSD
 Platform: OS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Provides: llfuse
-Requires-Python: >=3.8
+Requires-Python: >=3.5
 License-File: LICENSE
 
 ..
   NOTE: We cannot use sophisticated ReST syntax (like
   e.g. :file:`foo`) here because this isn't rendered correctly
   by PyPi.
```

### Comparing `arvados-llfuse-1.5.1/src/arvados_llfuse.egg-info/SOURCES.txt` & `arvados-llfuse-1.5.2/src/arvados_llfuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/darwin_compat.c` & `arvados-llfuse-1.5.2/src/darwin_compat.c`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/darwin_compat.h` & `arvados-llfuse-1.5.2/src/darwin_compat.h`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/fuse_api.pxi` & `arvados-llfuse-1.5.2/src/fuse_api.pxi`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/gettime.h` & `arvados-llfuse-1.5.2/src/gettime.h`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/handlers.pxi` & `arvados-llfuse-1.5.2/src/handlers.pxi`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/llfuse.c` & `arvados-llfuse-1.5.2/src/llfuse.c`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/llfuse.h` & `arvados-llfuse-1.5.2/src/llfuse.h`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/llfuse.pyx` & `arvados-llfuse-1.5.2/src/llfuse.pyx`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/lock.c` & `arvados-llfuse-1.5.2/src/lock.c`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/macros.c` & `arvados-llfuse-1.5.2/src/macros.c`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/misc.pxi` & `arvados-llfuse-1.5.2/src/misc.pxi`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/operations.pxi` & `arvados-llfuse-1.5.2/src/operations.pxi`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/src/xattr.h` & `arvados-llfuse-1.5.2/src/xattr.h`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/conftest.py` & `arvados-llfuse-1.5.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/pytest_checklogs.py` & `arvados-llfuse-1.5.2/test/pytest_checklogs.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/test_api.py` & `arvados-llfuse-1.5.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/test_examples.py` & `arvados-llfuse-1.5.2/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/test_fs.py` & `arvados-llfuse-1.5.2/test/test_fs.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/test_rounding.py` & `arvados-llfuse-1.5.2/test/test_rounding.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/test/util.py` & `arvados-llfuse-1.5.2/test/util.py`

 * *Files identical despite different names*

### Comparing `arvados-llfuse-1.5.1/util/sphinx_cython.py` & `arvados-llfuse-1.5.2/util/sphinx_cython.py`

 * *Files identical despite different names*

