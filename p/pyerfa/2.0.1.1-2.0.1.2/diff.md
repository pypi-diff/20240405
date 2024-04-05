# Comparing `tmp/pyerfa-2.0.1.1.tar.gz` & `tmp/pyerfa-2.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerfa-2.0.1.1.tar", last modified: Thu Oct 19 18:22:44 2023, max compression
+gzip compressed data, was "pyerfa-2.0.1.2.tar", last modified: Thu Apr  4 18:23:14 2024, max compression
```

## Comparing `pyerfa-2.0.1.1.tar` & `pyerfa-2.0.1.2.tar`

### file list

```diff
@@ -1,350 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.759023 pyerfa-2.0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/README_REPO_IMPORT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.763023 pyerfa-2.0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.763023 pyerfa-2.0.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.767023 pyerfa-2.0.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.771023 pyerfa-2.0.1.1/erfa/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/erfa/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   738983 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/core.py.templ
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.775023 pyerfa-2.0.1.1/erfa/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/test_erfa.py
--rw-r--r--   0 runner    (1001) docker     (127)   154942 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/tests/test_ufunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/test_ufunc.py.templ
--rw-r--r--   0 runner    (1001) docker     (127)   451427 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/ufunc.c
--rw-r--r--   0 runner    (1001) docker     (127)    35932 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/ufunc.c.templ
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36765 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/liberfa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.779023 pyerfa-2.0.1.1/liberfa/erfa/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/liberfa/erfa/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.779023 pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    28654 2023-10-19 18:22:37.000000 pyerfa-2.0.1.1/liberfa/erfa/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)    42494 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/aclocal.m4
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.787023 pyerfa-2.0.1.1/liberfa/erfa/build-aux/
--rwxrwxrwx   0 runner    (1001) docker     (127)     7400 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/compile
--rwxrwxrwx   0 runner    (1001) docker     (127)    49482 2022-01-31 14:43:17.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.guess
--rwxrwxrwx   0 runner    (1001) docker     (127)    35406 2022-01-31 14:43:17.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.sub
--rwxrwxrwx   0 runner    (1001) docker     (127)    23568 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/depcomp
--rwxrwxrwx   0 runner    (1001) docker     (127)    15358 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/install-sh
--rwxrwxrwx   0 runner    (1001) docker     (127)   327299 2022-03-24 16:13:52.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/ltmain.sh
--rwxrwxrwx   0 runner    (1001) docker     (127)     6878 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/missing
--rwxrwxrwx   0 runner    (1001) docker     (127)     4879 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/test-driver
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (127)   441029 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/configure
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/configure.ac
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/erfa.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.791023 pyerfa-2.0.1.1/liberfa/erfa/m4/
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/m4/erfa-numver.m4
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.899024 pyerfa-2.0.1.1/liberfa/erfa/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    83996 2023-10-19 18:22:37.000000 pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/a2af.c
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/a2tf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ab.c
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ae2hd.c
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/af2a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/anp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/anpm.c
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcg.c
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcg13.c
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apci.c
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apci13.c
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apco.c
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apco13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcs.c
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcs13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aper.c
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aper13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apio13.c
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atcc13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atccq.c
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atci13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciq.c
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciqn.c
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciqz.c
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atco13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atic13.c
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aticq.c
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aticqn.c
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atio13.c
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atioq.c
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoc13.c
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoi13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoiq.c
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bi00.c
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bp00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bp06.c
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bpn2xy.c
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ibpn.c
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ixy.c
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ixys.c
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2tcio.c
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2teqx.c
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2tpe.c
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2txy.c
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cal2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cr.c
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/d2dtf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/d2tf.c
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dat.c
--rw-r--r--   0 runner    (1001) docker     (127)    62193 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dtdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dtf2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eceq06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ecm06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee06a.c
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eect00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eform.c
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eo06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eors.c
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epb.c
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epb2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epj.c
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epj2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)   150627 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epv00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eqec06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eqeq94.c
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/era00.c
--rw-r--r--   0 runner    (1001) docker     (127)    27288 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfa.h
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.c
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.h
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfaextra.h
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfam.h
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfaversion.c
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fad03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fae03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faf03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faju03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fal03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/falp03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fama03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fame03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fane03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faom03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fapa03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fasa03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faur03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fave03.c
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk425.c
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk45z.c
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk524.c
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk52h.c
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk54z.c
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk5hip.c
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk5hz.c
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fw2m.c
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fw2xy.c
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/g2icrs.c
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gc2gd.c
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gc2gde.c
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gd2gc.c
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gd2gce.c
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst82.c
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst94.c
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/h2fk5.c
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hd2ae.c
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hd2pa.c
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hfk5z.c
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/icrs2g.c
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ir.c
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/jd2cal.c
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/jdcalf.c
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ld.c
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ldn.c
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ldsun.c
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/lteceq.c
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltecm.c
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/lteqec.c
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltp.c
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpb.c
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpecl.c
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpequ.c
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)    23973 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/moon98.c
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/numat.c
--rw-r--r--   0 runner    (1001) docker     (127)   118469 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut00a.c
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut06a.c
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nutm80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/obl06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/obl80.c
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p06e.c
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p2pv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pap.c
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pas.c
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pb06.c
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pdp.c
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pfw06.c
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/plan94.c
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pm.c
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat76.c
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmp.c
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmpx.c
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmsafe.c
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn.c
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00.c
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pom00.c
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ppp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ppsp.c
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pr00.c
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/prec76.c
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pv2p.c
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pv2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvdpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvm.c
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvmpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvppv.c
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvstar.c
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvtob.c
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvu.c
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvup.c
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pxp.c
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/refco.c
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rm2v.c
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rv2m.c
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rx.c
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxr.c
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ry.c
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rz.c
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00.c
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00b.c
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2c.c
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2p.c
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2pv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2xpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sepp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/seps.c
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sp00.c
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/starpm.c
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/starpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)   242393 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c_extra.c
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taitt.c
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taiut1.c
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taiutc.c
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tcbtdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tcgtt.c
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tdbtcb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tdbtt.c
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tf2a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tf2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpors.c
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tporv.c
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpsts.c
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpstv.c
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpxes.c
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpxev.c
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tr.c
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/trxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/trxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttai.c
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttcg.c
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ttut1.c
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1tai.c
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1tt.c
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1utc.c
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/utctai.c
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/utcut1.c
--rw-r--r--   0 runner    (1001) docker     (127)   132290 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xy06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.903024 pyerfa-2.0.1.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/licenses/ERFA.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/licenses/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.903024 pyerfa-2.0.1.1/pyerfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.916943 pyerfa-2.0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.800942 pyerfa-2.0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.804942 pyerfa-2.0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-04 18:23:14.916943 pyerfa-2.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/README_REPO_IMPORT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.808942 pyerfa-2.0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.800942 pyerfa-2.0.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.808942 pyerfa-2.0.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.808942 pyerfa-2.0.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.808942 pyerfa-2.0.1.2/erfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/erfa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   738450 2024-04-04 18:23:05.000000 pyerfa-2.0.1.2/erfa/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/core.py.templ
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.812942 pyerfa-2.0.1.2/erfa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/tests/test_erfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154942 2024-04-04 18:23:05.000000 pyerfa-2.0.1.2/erfa/tests/test_ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/tests/test_ufunc.py.templ
+-rw-r--r--   0 runner    (1001) docker     (127)   451776 2024-04-04 18:23:05.000000 pyerfa-2.0.1.2/erfa/ufunc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36281 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/ufunc.c.templ
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36765 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/erfa_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.800942 pyerfa-2.0.1.2/liberfa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.812942 pyerfa-2.0.1.2/liberfa/erfa/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/.git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.804942 pyerfa-2.0.1.2/liberfa/erfa/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.812942 pyerfa-2.0.1.2/liberfa/erfa/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    28654 2024-04-04 18:23:09.000000 pyerfa-2.0.1.2/liberfa/erfa/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42494 2024-04-04 18:23:08.000000 pyerfa-2.0.1.2/liberfa/erfa/aclocal.m4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.816942 pyerfa-2.0.1.2/liberfa/erfa/build-aux/
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7400 2022-03-18 13:09:08.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/compile
+-rwxrwxrwx   0 runner    (1001) docker     (127)    49482 2022-01-31 14:43:17.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/config.guess
+-rwxrwxrwx   0 runner    (1001) docker     (127)    35406 2022-01-31 14:43:17.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/config.sub
+-rwxrwxrwx   0 runner    (1001) docker     (127)    23568 2022-03-18 13:09:08.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/depcomp
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15358 2022-03-18 13:09:08.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/install-sh
+-rwxrwxrwx   0 runner    (1001) docker     (127)   327299 2022-03-24 16:13:52.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/ltmain.sh
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6878 2022-03-18 13:09:08.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/missing
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4879 2022-03-18 13:09:08.000000 pyerfa-2.0.1.2/liberfa/erfa/build-aux/test-driver
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 18:23:09.000000 pyerfa-2.0.1.2/liberfa/erfa/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)   441029 2024-04-04 18:23:09.000000 pyerfa-2.0.1.2/liberfa/erfa/configure
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/erfa.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.868942 pyerfa-2.0.1.2/liberfa/erfa/m4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/m4/erfa-numver.m4
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.916943 pyerfa-2.0.1.2/liberfa/erfa/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    83996 2024-04-04 18:23:09.000000 pyerfa-2.0.1.2/liberfa/erfa/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/a2af.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/a2tf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ab.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ae2hd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/af2a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/anp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/anpm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apcg.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apcg13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apci.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apci13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apco.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apco13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apcs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apcs13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/aper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/aper13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/apio13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atcc13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atccq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atci13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atciq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atciqn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atciqz.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atco13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atic13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/aticq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/aticqn.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atio13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atioq.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atoc13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atoi13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/atoiq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/bi00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/bp00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/bp06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/bpn2xy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2i00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2i00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2i06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2ibpn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2ixy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2ixys.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2t00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2t00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2t06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2tcio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2teqx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2tpe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/c2txy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/cal2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/cp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/cpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/cr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/d2dtf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/d2tf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/dat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    62193 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/dtdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/dtf2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eceq06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ecm06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ee00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ee00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ee00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ee06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eect00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eform.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eo06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/epb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/epb2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/epj.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/epj2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)   150627 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/epv00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eqec06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/eqeq94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/era00.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27288 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfadatextra.c
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfadatextra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfaextra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfam.h
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/erfaversion.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fad03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fae03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/faf03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/faju03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fal03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/falp03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fama03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fame03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fane03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/faom03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fapa03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fasa03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/faur03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fave03.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk425.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk45z.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk524.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk52h.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk54z.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk5hip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fk5hz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fw2m.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/fw2xy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/g2icrs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gc2gd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gc2gde.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gd2gc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gd2gce.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gmst00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gmst06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gmst82.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gst00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gst00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gst06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gst06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/gst94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/h2fk5.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/hd2ae.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/hd2pa.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/hfk5z.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/icrs2g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ir.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/jd2cal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/jdcalf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ld.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ldn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ldsun.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/lteceq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ltecm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/lteqec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ltp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ltpb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ltpecl.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ltpequ.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)    23973 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/moon98.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/num00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/num00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/num06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/numat.c
+-rw-r--r--   0 runner    (1001) docker     (127)   118469 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/nut00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/nut00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/nut06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/nut80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/nutm80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/obl06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/obl80.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/p06e.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/p2pv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/p2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pas.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pb06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pfw06.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/plan94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmat00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmat06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmat76.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmpx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pmsafe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pn06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pnm00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pnm00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pnm06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pnm80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pom00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ppp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ppsp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pr00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/prec76.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pv2p.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pv2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvdpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvmpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvppv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvstar.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvtob.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvu.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvup.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pvxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/pxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/refco.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rm2v.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rv2m.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rxr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ry.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/rz.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s2c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s2p.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s2pv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/s2xpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/sepp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/seps.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/sp00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/starpm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/starpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/sxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/sxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)   242393 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/t_erfa_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/t_erfa_c_extra.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/taitt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/taiut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/taiutc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tcbtdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tcgtt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tdbtcb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tdbtt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tf2a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tf2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tpors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tporv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tpsts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tpstv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tpxes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tpxev.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/trxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/trxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tttai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tttcg.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/tttdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ttut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ut1tai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ut1tt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/ut1utc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/utctai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/utcut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132290 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/xy06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/xys00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/xys00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/xys06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/zp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/zpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-04 18:22:55.000000 pyerfa-2.0.1.2/liberfa/erfa/src/zr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.916943 pyerfa-2.0.1.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/licenses/ERFA.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/licenses/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:23:14.916943 pyerfa-2.0.1.2/pyerfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 18:23:14.000000 pyerfa-2.0.1.2/pyerfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-04 18:23:14.920943 pyerfa-2.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-04 18:22:54.000000 pyerfa-2.0.1.2/tox.ini
```

### Comparing `pyerfa-2.0.1.1/AUTHORS.rst` & `pyerfa-2.0.1.2/AUTHORS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 * Erik M. Bray
 * Stuart Littlefair
 * Brigitta Sipocz
 * Sergio Pascual
 
 (If you have contributed to PyERFA and your name is missing, please
-`open a pull request for this page <https://github.com/liberfa/pyerfa/blob/master/AUTHORS.rst>`_
+`open a pull request for this page <https://github.com/liberfa/pyerfa/blob/main/AUTHORS.rst>`_
 in the `PyERFA repository <https://github.com/liberfa/pyerfa>`_)
 
 .. _Numpy: https://numpy.org/
 .. _Astropy: https://www.astropy.org
 .. _Jinja2: https://palletsprojects.com/p/jinja/
```

### Comparing `pyerfa-2.0.1.1/CHANGES.rst` & `pyerfa-2.0.1.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.0.1.2 (2024-04-04)
+====================
+No new features, but wheels that are compatible with numpy 2.0
+as well as older supported versions of numpy 1.x.
+
 2.0.1.1 (2023-10-19)
 ====================
 - Ensured pyerfa works on PyPy too with the Python limited API. [gh-120]
 - Ensure any non-contigous multi-dimensional inputs are recognized
   properly, so that, e.g., a non-contiguous matrix is copied as
   needed before input to the erfa functions. [gh-124]
```

### Comparing `pyerfa-2.0.1.1/LICENSE.rst` & `pyerfa-2.0.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/MANIFEST.in` & `pyerfa-2.0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/PKG-INFO` & `pyerfa-2.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerfa
-Version: 2.0.1.1
+Version: 2.0.1.2
 Summary: Python bindings for ERFA
 Home-page: https://github.com/liberfa/pyerfa
 Author: The PyERFA Developers
 License: BSD 3-Clause License
 Keywords: astronomy,astrophysics,cosmology,space,science,coordinate
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyerfa-2.0.1.1/README.rst` & `pyerfa-2.0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/README_REPO_IMPORT.rst` & `pyerfa-2.0.1.2/README_REPO_IMPORT.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/docs/Makefile` & `pyerfa-2.0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/docs/_templates/layout.html` & `pyerfa-2.0.1.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/docs/conf.py` & `pyerfa-2.0.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [('index', project.lower(), project + u' Documentation',
               [author], 1)]
 
 # Setting this URL is requited by sphinx-astropy
 github_issues_url = 'https://github.com/liberfa/pyerfa/issues/'
-edit_on_github_branch = 'master'
+edit_on_github_branch = 'main'
 
 
 # -- Options for linkcheck output --------------------------------------------
 linkcheck_retry = 5
 linkcheck_ignore = [
     r'https://github\.com/liberfa/pyerfa/(?:issues|pull)/\d+',
 ]
```

### Comparing `pyerfa-2.0.1.1/docs/make.bat` & `pyerfa-2.0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/erfa/core.py` & `pyerfa-2.0.1.2/erfa/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 function is scalar, you'll get back a length-10 1D array.
 (Note that the ufuncs take this into account using structured dtypes.)
 
 Note that the ufunc part of these functions are implemented in a separate
 module (compiled as ``ufunc``), derived from the ``ufunc.c`` file.
 """
 
-import warnings
+from warnings import warn
 
-import numpy
+import numpy as np
 
 from . import ufunc
 
 __all__ = [
     'ErfaError', 'ErfaWarning',
     'cal2jd', 'epb', 'epb2jd', 'epj', 'epj2jd', 'jd2cal', 'jdcalf', 'ab', 'apcg',
     'apcg13', 'apci', 'apci13', 'apco', 'apco13', 'apcs', 'apcs13', 'aper',
@@ -98,71 +98,49 @@
 # such as to turn errors into warnings.
 STATUS_CODES_REMAP = {
     'cal2jd': {-3: 3}
 }
 
 
 def check_errwarn(statcodes, func_name):
-    if not numpy.any(statcodes):
+    if not np.any(statcodes):
         return
     # Remap any errors into warnings in the STATUS_CODES_REMAP dict.
     if func_name in STATUS_CODES_REMAP:
         for before, after in STATUS_CODES_REMAP[func_name].items():
             statcodes[statcodes == before] = after
             STATUS_CODES[func_name][after] = STATUS_CODES[func_name][before]
 
-    if numpy.any(statcodes < 0):
+    # Use non-zero to be able to index (need >=1-D for this to work).
+    # Conveniently, this also gets rid of any masked elements.
+    statcodes = np.atleast_1d(statcodes)
+    erridx = (statcodes < 0).nonzero()
+    if erridx[0].size > 0:
         # Errors present - only report the errors.
-        if statcodes.shape:
-            statcodes = statcodes[statcodes < 0]
-
-        errcodes = numpy.unique(statcodes)
-
-        errcounts = dict([(e, numpy.sum(statcodes == e)) for e in errcodes])
-
+        errcodes, counts = np.unique(statcodes[erridx], return_counts=True)
         elsemsg = STATUS_CODES[func_name].get('else', None)
-        if elsemsg is None:
-            errmsgs = dict([(e, STATUS_CODES[func_name].get(
-                e, 'Return code ' + str(e))) for e in errcodes])
-        else:
-            errmsgs = dict([(e, STATUS_CODES[func_name].get(
-                e, elsemsg)) for e in errcodes])
-
-        emsg = ', '.join(['{0} of "{1}"'.format(errcounts[e], errmsgs[e])
-                          for e in errcodes])
-        raise ErfaError('ERFA function "{}" yielded {}'
-                        .format(func_name, emsg))
-
-    elif numpy.any(statcodes > 0):
-        # Only warnings present.
-        if statcodes.shape:
-            statcodes = statcodes[statcodes > 0]
-
-        warncodes = numpy.unique(statcodes)
-
-        warncounts = dict([(w, numpy.sum(statcodes == w)) for w in warncodes])
-
+        msgs = [STATUS_CODES[func_name].get(e, elsemsg or f'Return code {e}')
+                for e in errcodes]
+        emsg = ', '.join([f'{c} of "{msg}"' for c, msg in zip(counts, msgs)])
+        raise ErfaError(f'ERFA function "{func_name}" yielded {emsg}')
+
+    warnidx = (statcodes > 0).nonzero()
+    if warnidx[0].size > 0:
+        warncodes, counts = np.unique(statcodes[warnidx], return_counts=True)
         elsemsg = STATUS_CODES[func_name].get('else', None)
-        if elsemsg is None:
-            warnmsgs = dict([(w, STATUS_CODES[func_name].get(
-                w, 'Return code ' + str(w))) for w in warncodes])
-        else:
-            warnmsgs = dict([(w, STATUS_CODES[func_name].get(
-                w, elsemsg)) for w in warncodes])
-
-        wmsg = ', '.join(['{0} of "{1}"'.format(warncounts[w], warnmsgs[w])
-                          for w in warncodes])
-        warnings.warn('ERFA function "{}" yielded {}'.format(func_name, wmsg),
-                      ErfaWarning)
+        msgs = [STATUS_CODES[func_name].get(w, elsemsg or f'Return code {w}')
+                for w in warncodes]
+        wmsg = ', '.join([f'{c} of "{msg}"' for c, msg in zip(counts, msgs)])
+        warn(f'ERFA function "{func_name}" yielded {wmsg}', ErfaWarning)
 
 
 # <------------------------structured dtype conversion------------------------>
 
-dt_bytes1 = numpy.dtype('S1')
-dt_bytes12 = numpy.dtype('S12')
+dt_bytes1 = np.dtype('S1')
+dt_bytes12 = np.dtype('S12')
 
 # <--------------------------Actual ERFA-wrapping code------------------------>
 
 
 DPI = (3.141592653589793238462643)
 """Pi"""
 D2PI = (6.283185307179586476925287)
```

### Comparing `pyerfa-2.0.1.1/erfa/core.py.templ` & `pyerfa-2.0.1.2/erfa/core.py.templ`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 function is scalar, you'll get back a length-10 1D array.
 (Note that the ufuncs take this into account using structured dtypes.)
 
 Note that the ufunc part of these functions are implemented in a separate
 module (compiled as ``ufunc``), derived from the ``ufunc.c`` file.
 """
 
-import warnings
+from warnings import warn
 
-import numpy
+import numpy as np
 
 from . import ufunc
 
 __all__ = [
     'ErfaError', 'ErfaWarning',
     {{ funcs | map(attribute='pyname') | surround("'","'")
        | join(", ") | wordwrap(wrapstring='\n    ') }},
@@ -69,71 +69,49 @@
 # such as to turn errors into warnings.
 STATUS_CODES_REMAP = {
     'cal2jd': {-3: 3}
 }
 
 
 def check_errwarn(statcodes, func_name):
-    if not numpy.any(statcodes):
+    if not np.any(statcodes):
         return
     # Remap any errors into warnings in the STATUS_CODES_REMAP dict.
     if func_name in STATUS_CODES_REMAP:
         for before, after in STATUS_CODES_REMAP[func_name].items():
             statcodes[statcodes == before] = after
             STATUS_CODES[func_name][after] = STATUS_CODES[func_name][before]
 
-    if numpy.any(statcodes < 0):
+    # Use non-zero to be able to index (need >=1-D for this to work).
+    # Conveniently, this also gets rid of any masked elements.
+    statcodes = np.atleast_1d(statcodes)
+    erridx = (statcodes < 0).nonzero()
+    if erridx[0].size > 0:
         # Errors present - only report the errors.
-        if statcodes.shape:
-            statcodes = statcodes[statcodes < 0]
-
-        errcodes = numpy.unique(statcodes)
-
-        errcounts = dict([(e, numpy.sum(statcodes == e)) for e in errcodes])
-
+        errcodes, counts = np.unique(statcodes[erridx], return_counts=True)
         elsemsg = STATUS_CODES[func_name].get('else', None)
-        if elsemsg is None:
-            errmsgs = dict([(e, STATUS_CODES[func_name].get(
-                e, 'Return code ' + str(e))) for e in errcodes])
-        else:
-            errmsgs = dict([(e, STATUS_CODES[func_name].get(
-                e, elsemsg)) for e in errcodes])
-
-        emsg = ', '.join(['{0} of "{1}"'.format(errcounts[e], errmsgs[e])
-                          for e in errcodes])
-        raise ErfaError('ERFA function "{}" yielded {}'
-                        .format(func_name, emsg))
-
-    elif numpy.any(statcodes > 0):
-        # Only warnings present.
-        if statcodes.shape:
-            statcodes = statcodes[statcodes > 0]
-
-        warncodes = numpy.unique(statcodes)
-
-        warncounts = dict([(w, numpy.sum(statcodes == w)) for w in warncodes])
-
+        msgs = [STATUS_CODES[func_name].get(e, elsemsg or f'Return code {e}')
+                for e in errcodes]
+        emsg = ', '.join([f'{c} of "{msg}"' for c, msg in zip(counts, msgs)])
+        raise ErfaError(f'ERFA function "{func_name}" yielded {emsg}')
+
+    warnidx = (statcodes > 0).nonzero()
+    if warnidx[0].size > 0:
+        warncodes, counts = np.unique(statcodes[warnidx], return_counts=True)
         elsemsg = STATUS_CODES[func_name].get('else', None)
-        if elsemsg is None:
-            warnmsgs = dict([(w, STATUS_CODES[func_name].get(
-                w, 'Return code ' + str(w))) for w in warncodes])
-        else:
-            warnmsgs = dict([(w, STATUS_CODES[func_name].get(
-                w, elsemsg)) for w in warncodes])
-
-        wmsg = ', '.join(['{0} of "{1}"'.format(warncounts[w], warnmsgs[w])
-                          for w in warncodes])
-        warnings.warn('ERFA function "{}" yielded {}'.format(func_name, wmsg),
-                      ErfaWarning)
+        msgs = [STATUS_CODES[func_name].get(w, elsemsg or f'Return code {w}')
+                for w in warncodes]
+        wmsg = ', '.join([f'{c} of "{msg}"' for c, msg in zip(counts, msgs)])
+        warn(f'ERFA function "{func_name}" yielded {wmsg}', ErfaWarning)
 
 
 # <------------------------structured dtype conversion------------------------>
 
-dt_bytes1 = numpy.dtype('S1')
-dt_bytes12 = numpy.dtype('S12')
+dt_bytes1 = np.dtype('S1')
+dt_bytes12 = np.dtype('S12')
 
 # <--------------------------Actual ERFA-wrapping code------------------------>
 
 {% for constant in constants %}
 {{ constant.name }} = {{ constant.value }}
 """{{ constant.doc|join(' ')|wordwrap() }}"""
 {%- endfor %}
@@ -208,8 +186,8 @@
     {{ '{!r}'.format(key) }}: {{ '{!r}'.format(value) }},
 {%- endfor %}
 }
 {%- endif %}
 {%- endfor %}
 {%- endif %}
 {%- endfor %}
-{# done! (note: this comment also ensures final new line!) #}
+{# done! (note: this comment also ensures final new line!) #}
```

### Comparing `pyerfa-2.0.1.1/erfa/helpers.py` & `pyerfa-2.0.1.2/erfa/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import numpy as np
 
 from .core import ErfaWarning
 
 from .ufunc import get_leap_seconds, set_leap_seconds, dt_eraLEAPSECOND
 
 
+NUMPY_LT_2_0 = np.__version__.startswith("1.")
+
 _NotFound = object()
 
 
 # TODO: This can still be made to work for setters by implementing an
 # accompanying metaclass that supports it; we just don't need that right this
 # second
 class classproperty(property):
@@ -265,16 +267,16 @@
                      f"parsing it raised {exc!r}", ErfaWarning)
                 expires = None
 
         # Take care of astropy Table.
         if hasattr(table, '__array__'):
             table = table.__array__()[list(dt_eraLEAPSECOND.names)]
 
-        table = np.array(table, dtype=dt_eraLEAPSECOND, copy=False,
-                         ndmin=1)
+        table = np.array(table, dtype=dt_eraLEAPSECOND, ndmin=1,
+                         copy=False if NUMPY_LT_2_0 else None)
 
         # Simple sanity checks.
         if table.ndim > 1:
             raise ValueError("can only pass in one-dimensional tables.")
 
         if not np.all(((day == 1) &
                        (table['month'] == 1) | (table['month'] == 7)) |
```

### Comparing `pyerfa-2.0.1.1/erfa/tests/test_erfa.py` & `pyerfa-2.0.1.2/erfa/tests/test_erfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from datetime import datetime
 
 import pytest
 import numpy as np
 from numpy.testing import assert_array_equal, assert_array_almost_equal, assert_allclose
 
 import erfa
-from erfa.tests.helper import catch_warnings
 
 try:
     from astropy.time import Time
 except ImportError:
     # astropy not available for testing
     class Time:
         _DUMMY = True
@@ -168,26 +167,22 @@
     Test that the ERFA error reporting mechanism works as it should
     """
 
     # no warning
     erfa.dat(1990, 1, 1, 0.5)
 
     # check warning is raised for a scalar
-    with catch_warnings() as w:
+    with pytest.warns(erfa.ErfaWarning, match=r'1 of "dubious year \(Note 1\)"') as w:
         erfa.dat(100, 1, 1, 0.5)
         assert len(w) == 1
-        assert w[0].category == erfa.ErfaWarning
-        assert '1 of "dubious year (Note 1)"' in str(w[0].message)
 
     # and that the count is right for a vector.
-    with catch_warnings() as w:
+    with pytest.warns(erfa.ErfaWarning, match=r'2 of "dubious year \(Note 1\)"') as w:
         erfa.dat([100, 200, 1990], 1, 1, 0.5)
         assert len(w) == 1
-        assert w[0].category == erfa.ErfaWarning
-        assert '2 of "dubious year (Note 1)"' in str(w[0].message)
 
     try:
         erfa.dat(1990, [1, 34, 2], [1, 1, 43], 0.5)
     except erfa.ErfaError as e:
         if '1 of "bad day (Note 3)", 1 of "bad month"' not in e.args[0]:
             assert False, 'Raised the correct type of error, but wrong message: ' + e.args[0]
```

### Comparing `pyerfa-2.0.1.1/erfa/tests/test_ufunc.py` & `pyerfa-2.0.1.2/erfa/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/erfa/tests/test_ufunc.py.templ` & `pyerfa-2.0.1.2/erfa/tests/test_ufunc.py.templ`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/erfa/ufunc.c` & `pyerfa-2.0.1.2/erfa/ufunc.c`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 #define Py_LIMITED_API 0x030900f0
 #include "Python.h"
 #include "numpy/arrayobject.h"
 #include "numpy/ufuncobject.h"
 #include "erfa.h"
 #include "erfaextra.h"
 
+// Backported NumPy 2 API (can be removed if numpy 2 is required)
+#if NPY_ABI_VERSION < 0x02000000
+#define PyDataType_ELSIZE(descr) ((descr)->elsize)
+#endif
+
 // On gcc<10 we can run into the following:
 //
 //   error: dereferencing pointer to incomplete type 'PyTypeObject'
 //
 // As mentioned in https://github.com/numpy/numpy/issues/16970,
 // the workaround is to define a fake _typeobject struct.
 
@@ -9511,35 +9516,35 @@
     for (i = 0; i < nin; ++i) {
         PyArray_Descr *op_descr = PyArray_DESCR(op[i]);
         /*
          * Check for NPY_VOID with an associated struct dtype.
          */
         if (types[i] == NPY_VOID && dtypes != NULL) {
             int op_descr_type_num = op_descr->type_num;
-            int dtype_elsize = dtypes[i]->elsize;
+            npy_intp dtype_elsize = PyDataType_ELSIZE(dtypes[i]);
             /*
              * MHvK: we do our own check on casting, since by default
              * all items can cast to structured dtypes (see gh-11114),
              * which is not OK. So, we only allow VOID->same VOID,
              * and STRING -> VOID-of-STRING (which works well; we
              * recognize VOID-of-STRING by the dtype element size;
              * it would be rather costly to go look at dtype->fields).
              */
             if (op_descr_type_num == NPY_VOID) {
                 /* allow only the same structured to structured */
                 if (!PyArray_EquivTypes(op_descr, dtypes[i])) {
                     return 0;
                 }
             }
-            else if (dtypes[i]->elsize == 1 || dtypes[i]->elsize == 12) {
+            else if (dtype_elsize == 1 || dtype_elsize == 12) {
                 /* string structured array; string argument is OK */
                 if (!((op_descr_type_num == NPY_STRING &&
-                       op_descr->elsize <= dtype_elsize) ||
+                       PyDataType_ELSIZE(op_descr) <= dtype_elsize) ||
                       (op_descr_type_num == NPY_UNICODE &&
-                       op_descr->elsize >> 2 <= dtype_elsize))) {
+                       PyDataType_ELSIZE(op_descr) >> 2 <= dtype_elsize))) {
                     return 0;
                 }
             }
             else {
                 return 0;
             }
         }
@@ -9707,15 +9712,17 @@
                                  NPY_CASTING casting,
                                  PyArrayObject **operands,
                                  PyObject *type_tup,
                                  PyArray_Descr **out_dtypes)
 {
     int *types;
     PyArray_Descr **dtypes;
-    int types_array[NPY_MAXARGS];
+
+    /* This array needs to be at least as long as nint+nout. In practice, 32 suffices */
+    int types_array[32];
 
     if (ufunc->userloops) {
         Py_ssize_t unused_pos = 0;
         PyObject *userloop;
         PyUFunc_Loop1d *funcdata;
 
         if (ufunc->ntypes > 0 || PyDict_Size(ufunc->userloops) != 1) {
@@ -9887,15 +9894,18 @@
     /* structured dtypes and their definition */
     PyObject *dtype_def;
     PyArray_Descr *dt_double = NULL, *dt_int = NULL;
     PyArray_Descr *dt_pv = NULL, *dt_pvdpv = NULL;
     PyArray_Descr *dt_ymdf = NULL, *dt_hmsf = NULL, *dt_dmsf = NULL;
     PyArray_Descr *dt_sign = NULL, *dt_type = NULL;
     PyArray_Descr *dt_eraASTROM = NULL, *dt_eraLDBODY = NULL;
-    PyArray_Descr *dtypes[NPY_MAXARGS];
+
+    /* This array needs to be at least as long as nint+nout. In practice, 32 suffices */
+    PyArray_Descr *dtypes[32];
+
     /* ufuncs and their definitions */
     int status;
     PyUFuncObject *ufunc;
     static void *data[1] = {NULL};
     static char types_cal2jd[6] = {NPY_INT, NPY_INT, NPY_INT, NPY_DOUBLE, NPY_DOUBLE, NPY_INT};
     static PyUFuncGenericFunction funcs_cal2jd[1] = { &ufunc_loop_cal2jd };
     static char types_epb[3] = {NPY_DOUBLE, NPY_DOUBLE, NPY_DOUBLE};
```

### Comparing `pyerfa-2.0.1.1/erfa/ufunc.c.templ` & `pyerfa-2.0.1.2/erfa/ufunc.c.templ`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 #define Py_LIMITED_API 0x030900f0
 #include "Python.h"
 #include "numpy/arrayobject.h"
 #include "numpy/ufuncobject.h"
 #include "erfa.h"
 #include "erfaextra.h"
 
+// Backported NumPy 2 API (can be removed if numpy 2 is required)
+#if NPY_ABI_VERSION < 0x02000000
+#define PyDataType_ELSIZE(descr) ((descr)->elsize)
+#endif
+
 // On gcc<10 we can run into the following:
 //
 //   error: dereferencing pointer to incomplete type 'PyTypeObject'
 //
 // As mentioned in https://github.com/numpy/numpy/issues/16970,
 // the workaround is to define a fake _typeobject struct.
 
@@ -372,35 +377,35 @@
     for (i = 0; i < nin; ++i) {
         PyArray_Descr *op_descr = PyArray_DESCR(op[i]);
         /*
          * Check for NPY_VOID with an associated struct dtype.
          */
         if (types[i] == NPY_VOID && dtypes != NULL) {
             int op_descr_type_num = op_descr->type_num;
-            int dtype_elsize = dtypes[i]->elsize;
+            npy_intp dtype_elsize = PyDataType_ELSIZE(dtypes[i]);
             /*
              * MHvK: we do our own check on casting, since by default
              * all items can cast to structured dtypes (see gh-11114),
              * which is not OK. So, we only allow VOID->same VOID,
              * and STRING -> VOID-of-STRING (which works well; we
              * recognize VOID-of-STRING by the dtype element size;
              * it would be rather costly to go look at dtype->fields).
              */
             if (op_descr_type_num == NPY_VOID) {
                 /* allow only the same structured to structured */
                 if (!PyArray_EquivTypes(op_descr, dtypes[i])) {
                     return 0;
                 }
             }
-            else if (dtypes[i]->elsize == 1 || dtypes[i]->elsize == 12) {
+            else if (dtype_elsize == 1 || dtype_elsize == 12) {
                 /* string structured array; string argument is OK */
                 if (!((op_descr_type_num == NPY_STRING &&
-                       op_descr->elsize <= dtype_elsize) ||
+                       PyDataType_ELSIZE(op_descr) <= dtype_elsize) ||
                       (op_descr_type_num == NPY_UNICODE &&
-                       op_descr->elsize >> 2 <= dtype_elsize))) {
+                       PyDataType_ELSIZE(op_descr) >> 2 <= dtype_elsize))) {
                     return 0;
                 }
             }
             else {
                 return 0;
             }
         }
@@ -568,15 +573,17 @@
                                  NPY_CASTING casting,
                                  PyArrayObject **operands,
                                  PyObject *type_tup,
                                  PyArray_Descr **out_dtypes)
 {
     int *types;
     PyArray_Descr **dtypes;
-    int types_array[NPY_MAXARGS];
+
+    /* This array needs to be at least as long as nint+nout. In practice, 32 suffices */
+    int types_array[32];
 
     if (ufunc->userloops) {
         Py_ssize_t unused_pos = 0;
         PyObject *userloop;
         PyUFunc_Loop1d *funcdata;
 
         if (ufunc->ntypes > 0 || PyDict_Size(ufunc->userloops) != 1) {
@@ -748,15 +755,18 @@
     /* structured dtypes and their definition */
     PyObject *dtype_def;
     PyArray_Descr *dt_double = NULL, *dt_int = NULL;
     PyArray_Descr *dt_pv = NULL, *dt_pvdpv = NULL;
     PyArray_Descr *dt_ymdf = NULL, *dt_hmsf = NULL, *dt_dmsf = NULL;
     PyArray_Descr *dt_sign = NULL, *dt_type = NULL;
     PyArray_Descr *dt_eraASTROM = NULL, *dt_eraLDBODY = NULL;
-    PyArray_Descr *dtypes[NPY_MAXARGS];
+
+    /* This array needs to be at least as long as nint+nout. In practice, 32 suffices */
+    PyArray_Descr *dtypes[32];
+
     /* ufuncs and their definitions */
     int status;
     PyUFuncObject *ufunc;
     static void *data[1] = {NULL};
     {#- /* for non-structured functions, define there types and functions
            as these do not get copied */ #}
     {%- for func in funcs %}
```

### Comparing `pyerfa-2.0.1.1/erfa/version.py` & `pyerfa-2.0.1.2/erfa/version.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/erfa_generator.py` & `pyerfa-2.0.1.2/erfa_generator.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/ci_workflows.yml` & `pyerfa-2.0.1.2/liberfa/erfa/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/INFO` & `pyerfa-2.0.1.2/liberfa/erfa/INFO`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/LICENSE` & `pyerfa-2.0.1.2/liberfa/erfa/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/Makefile.in` & `pyerfa-2.0.1.2/liberfa/erfa/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/README.rst` & `pyerfa-2.0.1.2/liberfa/erfa/README.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/RELEASE.rst` & `pyerfa-2.0.1.2/liberfa/erfa/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/aclocal.m4` & `pyerfa-2.0.1.2/liberfa/erfa/aclocal.m4`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/compile` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/compile`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.guess` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/config.guess`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.sub` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/config.sub`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/depcomp` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/depcomp`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/install-sh` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/install-sh`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/ltmain.sh` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/ltmain.sh`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/missing` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/missing`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/build-aux/test-driver` & `pyerfa-2.0.1.2/liberfa/erfa/build-aux/test-driver`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/config.h.in` & `pyerfa-2.0.1.2/liberfa/erfa/config.h.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/configure` & `pyerfa-2.0.1.2/liberfa/erfa/configure`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/configure.ac` & `pyerfa-2.0.1.2/liberfa/erfa/configure.ac`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/m4/erfa-numver.m4` & `pyerfa-2.0.1.2/liberfa/erfa/m4/erfa-numver.m4`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/meson.build` & `pyerfa-2.0.1.2/liberfa/erfa/meson.build`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.am` & `pyerfa-2.0.1.2/liberfa/erfa/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.in` & `pyerfa-2.0.1.2/liberfa/erfa/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/a2af.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/a2af.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/a2tf.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/a2tf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ab.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ab.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ae2hd.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ae2hd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/af2a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/af2a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/anp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/anp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/anpm.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/anpm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apcg.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apcg.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apcg13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apcg13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apci.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apci.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apci13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apci13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apco.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apco.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apco13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apco13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apcs.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apcs.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apcs13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apcs13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/aper.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/aper.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/aper13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/aper13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apio.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apio.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/apio13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/apio13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atcc13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atcc13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atccq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atccq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atci13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atci13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atciq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atciq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atciqn.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atciqn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atciqz.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atciqz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atco13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atco13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atic13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atic13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/aticq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/aticq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/aticqn.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/aticqn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atio13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atio13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atioq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atioq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atoc13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atoc13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atoi13.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atoi13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/atoiq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/atoiq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/bi00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/bi00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/bp00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/bp00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/bp06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/bp06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/bpn2xy.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2i00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2i00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2i00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2i00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2i06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2i06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2ibpn.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2ixy.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2ixy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2ixys.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2ixys.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2s.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2t00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2t00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2t00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2t00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2t06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2t06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2tcio.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2tcio.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2teqx.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2teqx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2tpe.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2tpe.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/c2txy.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/c2txy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/cal2jd.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/cal2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/cp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/cp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/cpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/cpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/cr.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/cr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/d2dtf.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/d2dtf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/d2tf.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/d2tf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/dat.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/dat.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/dtdb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/dtdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/dtf2d.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/dtf2d.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eceq06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eceq06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ecm06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ecm06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ee00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ee00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ee00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ee00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ee00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ee00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ee06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ee06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eect00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eect00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eform.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eform.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eo06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eo06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eors.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eors.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/epb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/epb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/epb2jd.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/epb2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/epj.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/epj.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/epj2jd.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/epj2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/epv00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/epv00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eqec06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eqec06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/eqeq94.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/eqeq94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/era00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/era00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfa.h` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfa.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfadatextra.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.h` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfadatextra.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfaextra.h` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfaextra.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfam.h` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfam.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/erfaversion.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/erfaversion.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fad03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fad03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fae03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fae03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/faf03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/faf03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/faju03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/faju03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fal03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fal03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/falp03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/falp03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fama03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fama03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fame03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fame03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fane03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fane03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/faom03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/faom03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fapa03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fapa03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fasa03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fasa03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/faur03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/faur03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fave03.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fave03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk425.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk425.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk45z.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk45z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk524.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk524.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk52h.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk52h.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk54z.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk54z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk5hip.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk5hip.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fk5hz.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fk5hz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fw2m.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fw2m.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/fw2xy.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/fw2xy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/g2icrs.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/g2icrs.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gc2gd.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gc2gd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gc2gde.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gc2gde.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gd2gc.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gd2gc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gd2gce.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gd2gce.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gmst00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gmst00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gmst06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gmst06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gmst82.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gmst82.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gst00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gst00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gst00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gst00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gst06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gst06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gst06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gst06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/gst94.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/gst94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/h2fk5.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/h2fk5.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/hd2ae.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/hd2ae.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/hd2pa.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/hd2pa.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/hfk5z.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/hfk5z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/icrs2g.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/icrs2g.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ir.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ir.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/jd2cal.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/jd2cal.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/jdcalf.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/jdcalf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ld.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ld.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ldn.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ldn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ldsun.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ldsun.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/lteceq.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/lteceq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ltecm.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ltecm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/lteqec.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/lteqec.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ltp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ltp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ltpb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ltpb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ltpecl.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ltpecl.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ltpequ.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ltpequ.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/meson.build` & `pyerfa-2.0.1.2/liberfa/erfa/src/meson.build`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/moon98.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/moon98.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/num00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/num00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/num00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/num00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/num06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/num06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/numat.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/numat.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/nut00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/nut00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/nut00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/nut00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/nut06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/nut06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/nut80.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/nut80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/nutm80.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/nutm80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/obl06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/obl06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/obl80.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/obl80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/p06e.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/p06e.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/p2pv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/p2pv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/p2s.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/p2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pap.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pap.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pas.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pas.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pb06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pb06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pdp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pdp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pfw06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pfw06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/plan94.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/plan94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pm.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmat00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmat00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmat06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmat06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmat76.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmat76.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmpx.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmpx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pmsafe.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pmsafe.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pn06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pn06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pnm00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pnm00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pnm00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pnm00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pnm06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pnm06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pnm80.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pnm80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pom00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pom00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ppp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ppp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ppsp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ppsp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pr00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pr00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/prec76.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/prec76.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pv2p.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pv2p.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pv2s.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pv2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvdpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvdpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvm.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvmpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvmpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvppv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvppv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvstar.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvstar.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvtob.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvtob.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvu.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvu.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvup.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvup.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pvxpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pvxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/pxp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/pxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/refco.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/refco.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rm2v.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rm2v.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rv2m.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rv2m.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rx.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rxp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rxpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rxr.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rxr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ry.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ry.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/rz.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/rz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s2c.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s2c.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s2p.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s2p.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s2pv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s2pv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/s2xpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/s2xpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/sepp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/sepp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/seps.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/seps.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/sp00.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/sp00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/starpm.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/starpm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/starpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/starpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/sxp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/sxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/sxpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/sxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/t_erfa_c.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c_extra.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/t_erfa_c_extra.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/taitt.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/taitt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/taiut1.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/taiut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/taiutc.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/taiutc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tcbtdb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tcgtt.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tcgtt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tdbtcb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tdbtt.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tdbtt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tf2a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tf2a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tf2d.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tf2d.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tpors.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tpors.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tporv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tporv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tpsts.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tpsts.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tpstv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tpstv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tpxes.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tpxes.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tpxev.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tpxev.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tr.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/trxp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/trxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/trxpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/trxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tttai.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tttai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tttcg.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tttcg.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/tttdb.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/tttdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ttut1.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ttut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ut1tai.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ut1tai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ut1tt.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ut1tt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/ut1utc.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/ut1utc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/utctai.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/utctai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/utcut1.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/utcut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/xy06.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/xy06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/xys00a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/xys00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/xys00b.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/xys00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/xys06a.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/xys06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/zp.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/zp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/zpv.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/zpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/liberfa/erfa/src/zr.c` & `pyerfa-2.0.1.2/liberfa/erfa/src/zr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/licenses/ERFA.rst` & `pyerfa-2.0.1.2/licenses/ERFA.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/pyerfa.egg-info/PKG-INFO` & `pyerfa-2.0.1.2/pyerfa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerfa
-Version: 2.0.1.1
+Version: 2.0.1.2
 Summary: Python bindings for ERFA
 Home-page: https://github.com/liberfa/pyerfa
 Author: The PyERFA Developers
 License: BSD 3-Clause License
 Keywords: astronomy,astrophysics,cosmology,space,science,coordinate
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyerfa-2.0.1.1/pyerfa.egg-info/SOURCES.txt` & `pyerfa-2.0.1.2/pyerfa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 RELEASING.rst
 erfa_generator.py
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci_workflows.yml
+.github/workflows/publish.yml
 docs/Makefile
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/credits.rst
 docs/index.rst
 docs/license.rst
@@ -30,15 +31,14 @@
 erfa/core.py
 erfa/core.py.templ
 erfa/helpers.py
 erfa/ufunc.c
 erfa/ufunc.c.templ
 erfa/version.py
 erfa/tests/__init__.py
-erfa/tests/helper.py
 erfa/tests/test_erfa.py
 erfa/tests/test_ufunc.py
 erfa/tests/test_ufunc.py.templ
 liberfa/erfa/.git
 liberfa/erfa/.gitignore
 liberfa/erfa/INFO
 liberfa/erfa/LICENSE
```

### Comparing `pyerfa-2.0.1.1/setup.cfg` & `pyerfa-2.0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/setup.py` & `pyerfa-2.0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1.1/tox.ini` & `pyerfa-2.0.1.2/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     olddeps: numpy==1.20.*  # something potentially problematic (see gh-101)
     devdeps: numpy>=0.0.dev0
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
 
+install_command =
+    !devdeps: python -I -m pip install
+    devdeps: python -I -m pip install -v --pre
+
 commands =
     pip freeze
     python -c 'import erfa'  # To give useful error message if liberfa is too old.
     pytest --pyargs erfa {toxinidir}/docs {posargs}
 
 [testenv:build_docs]
 changedir = docs
```

