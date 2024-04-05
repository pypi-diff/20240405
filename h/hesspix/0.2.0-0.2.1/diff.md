# Comparing `tmp/hesspix-0.2.0.tar.gz` & `tmp/hesspix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hesspix-0.2.0.tar", last modified: Thu Mar 28 13:55:16 2024, max compression
+gzip compressed data, was "hesspix-0.2.1.tar", last modified: Fri Apr  5 11:25:17 2024, max compression
```

## Comparing `hesspix-0.2.0.tar` & `hesspix-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.184509 hesspix-0.2.0/
--rw-r--r--   0 tamasgal   (501) staff       (20)      258 2024-03-28 09:25:10.000000 hesspix-0.2.0/.coveragerc
--rw-r--r--   0 tamasgal   (501) staff       (20)      442 2024-03-28 09:25:10.000000 hesspix-0.2.0/.gitignore
--rw-r--r--   0 tamasgal   (501) staff       (20)     2771 2024-03-28 09:25:10.000000 hesspix-0.2.0/.gitlab-ci.yml
--rw-r--r--   0 tamasgal   (501) staff       (20)      234 2024-03-28 09:25:10.000000 hesspix-0.2.0/CHANGELOG.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)     5499 2024-03-28 09:25:10.000000 hesspix-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)     1524 2024-03-28 09:25:10.000000 hesspix-0.2.0/LICENSE
--rw-r--r--   0 tamasgal   (501) staff       (20)       62 2024-03-28 09:25:10.000000 hesspix-0.2.0/MANIFEST.in
--rw-r--r--   0 tamasgal   (501) staff       (20)      942 2024-03-28 09:25:10.000000 hesspix-0.2.0/Makefile
--rw-r--r--   0 tamasgal   (501) staff       (20)     4873 2024-03-28 13:55:16.184440 hesspix-0.2.0/PKG-INFO
--rw-r--r--   0 tamasgal   (501) staff       (20)     2352 2024-03-28 13:52:40.000000 hesspix-0.2.0/README.rst
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.179778 hesspix-0.2.0/doc/
--rw-r--r--   0 tamasgal   (501) staff       (20)      634 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/Makefile
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.180367 hesspix-0.2.0/doc/_static/
--rw-r--r--   0 tamasgal   (501) staff       (20)       55 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/_static/default.css
--rw-r--r--   0 tamasgal   (501) staff       (20)    24268 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/_static/default_gallery_thumbnail.png
--rw-r--r--   0 tamasgal   (501) staff       (20)       51 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/changelog.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)     2977 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/conf.py
--rw-r--r--   0 tamasgal   (501) staff       (20)       33 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/contribute.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)       65 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/examples.rst
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.180853 hesspix-0.2.0/doc/gen_modules/
--rw-r--r--   0 tamasgal   (501) staff       (20)        0 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/gen_modules/.gitkeep
--rw-r--r--   0 tamasgal   (501) staff       (20)      351 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/index.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)      795 2024-03-28 09:25:10.000000 hesspix-0.2.0/doc/make.bat
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.181115 hesspix-0.2.0/examples/
--rw-r--r--   0 tamasgal   (501) staff       (20)      126 2024-03-28 09:25:10.000000 hesspix-0.2.0/examples/README.rst
--rw-r--r--   0 tamasgal   (501) staff       (20)      119 2024-03-28 09:28:04.000000 hesspix-0.2.0/examples/plot_basics.py
--rw-r--r--   0 tamasgal   (501) staff       (20)      142 2024-03-28 09:25:10.000000 hesspix-0.2.0/pyproject.toml
--rw-r--r--   0 tamasgal   (501) staff       (20)     1843 2024-03-28 13:55:16.184981 hesspix-0.2.0/setup.cfg
--rw-r--r--   0 tamasgal   (501) staff       (20)       83 2024-03-28 09:25:10.000000 hesspix-0.2.0/setup.py
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.176148 hesspix-0.2.0/src/
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.181811 hesspix-0.2.0/src/hesspix/
--rw-r--r--   0 tamasgal   (501) staff       (20)      243 2024-03-28 12:36:11.000000 hesspix-0.2.0/src/hesspix/__init__.py
--rw-r--r--   0 tamasgal   (501) staff       (20)     4391 2024-03-28 13:53:54.000000 hesspix-0.2.0/src/hesspix/ct5.py
--rw-r--r--   0 tamasgal   (501) staff       (20)      411 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix/version.py
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.182905 hesspix-0.2.0/src/hesspix.egg-info/
--rw-r--r--   0 tamasgal   (501) staff       (20)     4873 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix.egg-info/PKG-INFO
--rw-r--r--   0 tamasgal   (501) staff       (20)      650 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix.egg-info/SOURCES.txt
--rw-r--r--   0 tamasgal   (501) staff       (20)        1 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix.egg-info/dependency_links.txt
--rw-r--r--   0 tamasgal   (501) staff       (20)      418 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix.egg-info/requires.txt
--rw-r--r--   0 tamasgal   (501) staff       (20)        8 2024-03-28 13:55:16.000000 hesspix-0.2.0/src/hesspix.egg-info/top_level.txt
-drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-03-28 13:55:16.182615 hesspix-0.2.0/tests/
--rw-r--r--   0 tamasgal   (501) staff       (20)       71 2024-03-28 09:25:10.000000 hesspix-0.2.0/tests/test_is_mandatory.py
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.511711 hesspix-0.2.1/
+-rw-r--r--   0 tamasgal   (501) staff       (20)      258 2024-03-28 09:25:10.000000 hesspix-0.2.1/.coveragerc
+-rw-r--r--   0 tamasgal   (501) staff       (20)      442 2024-03-28 09:25:10.000000 hesspix-0.2.1/.gitignore
+-rw-r--r--   0 tamasgal   (501) staff       (20)     2771 2024-03-28 09:25:10.000000 hesspix-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0 tamasgal   (501) staff       (20)      234 2024-03-28 09:25:10.000000 hesspix-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)     5499 2024-03-28 09:25:10.000000 hesspix-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)     1524 2024-03-28 09:25:10.000000 hesspix-0.2.1/LICENSE
+-rw-r--r--   0 tamasgal   (501) staff       (20)       62 2024-03-28 09:25:10.000000 hesspix-0.2.1/MANIFEST.in
+-rw-r--r--   0 tamasgal   (501) staff       (20)      942 2024-03-28 09:25:10.000000 hesspix-0.2.1/Makefile
+-rw-r--r--   0 tamasgal   (501) staff       (20)     5091 2024-04-05 11:25:17.511610 hesspix-0.2.1/PKG-INFO
+-rw-r--r--   0 tamasgal   (501) staff       (20)     2570 2024-03-28 14:09:57.000000 hesspix-0.2.1/README.rst
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.505695 hesspix-0.2.1/doc/
+-rw-r--r--   0 tamasgal   (501) staff       (20)      634 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/Makefile
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.506287 hesspix-0.2.1/doc/_static/
+-rw-r--r--   0 tamasgal   (501) staff       (20)       55 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/_static/default.css
+-rw-r--r--   0 tamasgal   (501) staff       (20)    24268 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/_static/default_gallery_thumbnail.png
+-rw-r--r--   0 tamasgal   (501) staff       (20)       51 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/changelog.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)     2977 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/conf.py
+-rw-r--r--   0 tamasgal   (501) staff       (20)       33 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/contribute.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)       65 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/examples.rst
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.507006 hesspix-0.2.1/doc/gen_modules/
+-rw-r--r--   0 tamasgal   (501) staff       (20)        0 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/gen_modules/.gitkeep
+-rw-r--r--   0 tamasgal   (501) staff       (20)      351 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/index.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)      795 2024-03-28 09:25:10.000000 hesspix-0.2.1/doc/make.bat
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.507302 hesspix-0.2.1/examples/
+-rw-r--r--   0 tamasgal   (501) staff       (20)      126 2024-03-28 09:25:10.000000 hesspix-0.2.1/examples/README.rst
+-rw-r--r--   0 tamasgal   (501) staff       (20)      119 2024-03-28 09:28:04.000000 hesspix-0.2.1/examples/plot_basics.py
+-rw-r--r--   0 tamasgal   (501) staff       (20)      142 2024-03-28 09:25:10.000000 hesspix-0.2.1/pyproject.toml
+-rw-r--r--   0 tamasgal   (501) staff       (20)     1843 2024-04-05 11:25:17.512331 hesspix-0.2.1/setup.cfg
+-rw-r--r--   0 tamasgal   (501) staff       (20)       83 2024-03-28 09:25:10.000000 hesspix-0.2.1/setup.py
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.501103 hesspix-0.2.1/src/
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.508231 hesspix-0.2.1/src/hesspix/
+-rw-r--r--   0 tamasgal   (501) staff       (20)      243 2024-03-28 12:36:11.000000 hesspix-0.2.1/src/hesspix/__init__.py
+-rw-r--r--   0 tamasgal   (501) staff       (20)     4171 2024-04-05 11:23:55.000000 hesspix-0.2.1/src/hesspix/ct5.py
+-rw-r--r--   0 tamasgal   (501) staff       (20)      411 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix/version.py
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.509513 hesspix-0.2.1/src/hesspix.egg-info/
+-rw-r--r--   0 tamasgal   (501) staff       (20)     5091 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix.egg-info/PKG-INFO
+-rw-r--r--   0 tamasgal   (501) staff       (20)      650 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix.egg-info/SOURCES.txt
+-rw-r--r--   0 tamasgal   (501) staff       (20)        1 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix.egg-info/dependency_links.txt
+-rw-r--r--   0 tamasgal   (501) staff       (20)      418 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix.egg-info/requires.txt
+-rw-r--r--   0 tamasgal   (501) staff       (20)        8 2024-04-05 11:25:17.000000 hesspix-0.2.1/src/hesspix.egg-info/top_level.txt
+drwxr-xr-x   0 tamasgal   (501) staff       (20)        0 2024-04-05 11:25:17.509160 hesspix-0.2.1/tests/
+-rw-r--r--   0 tamasgal   (501) staff       (20)       71 2024-03-28 09:25:10.000000 hesspix-0.2.1/tests/test_is_mandatory.py
```

### Comparing `hesspix-0.2.0/.gitlab-ci.yml` & `hesspix-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/CONTRIBUTING.rst` & `hesspix-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/LICENSE` & `hesspix-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/Makefile` & `hesspix-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/PKG-INFO` & `hesspix-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hesspix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tiny library to read HESS pixel info from ROOT files.
 Home-page: https://git.ecap.work/tgal/hesspix
 Author: Tamas Gal
 Author-email: tamas.gal@fau.de
 Maintainer: Tamas Gal
 Maintainer-email: tamas.gal@fau.de
 License: MIT
@@ -62,45 +62,54 @@
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinxcontrib-versioning; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 hesspix 
 =======
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/pipeline.svg
-    :target: https://git.ecap.work/tgal/hesspix/pipelines
+``hesspix`` is a tiny library to read HESS pixel info from ROOT files. No ROOT
+is required.
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/coverage.svg
-    :target: https://tgal.pages.ecap.work/hesspix/coverage
+Installation
+~~~~~~~~~~~~
+
+``hesspix`` is a registered Python package. It can be installed using ``pip``::
+
+  pip install hesspix
 
-.. image:: https://git.km3net.de/examples/km3badges/-/raw/master/docs-latest-brightgreen.svg
-    :target: https://tgal.pages.ecap.work/hesspix
+To install the latest development version from the Git repository::
 
-``hesspix`` is a tiny library to read HESS pixel info from ROOT files.
+  pip install git+https://github.com/tamasgal/hesspix
 
 Usage
 ~~~~~
 
 It's as easy as::
 
     >>> import hesspix as hp
 
     >>> r = hp.CT5Reader("gamma_20deg_180deg_run4151.dst.root")
 
+accessing events via a global index, as written in the ROOT branch::
+
     >>> r[0]
     Event 801 (bunch 0) [10 pixels]
 
     >>> r[23]
     Event 19607 (bunch 0) [3 pixels]
 
+Grabbing an event with a given event number and bunch number::
+
     >>> r.get(event_nr=3902, bunch_nr=0)
     Event 3902 (bunch 0) [18 pixels]
 
     >>> event = r.get(event_nr=3902, bunch_nr=0)
 
+The pixel information is stored in ``pixinfo``::
+
     >>> event.pixinfo
     rec.array([( 352, 18.27153 , 3, 20.9375  ),
             ( 353, 23.193665, 3, 21.703125),
             ( 355, 11.846128, 3, 22.171875),
             ( 357, 15.300814, 3, 21.5     ),
             ( 513,  8.219065, 3, 21.046875),
             (1296, 15.051192, 3, 19.890625),
@@ -114,35 +123,35 @@
             (1324, 13.618393, 3, 20.75    ),
             (1325, 12.267553, 3, 20.953125),
             (1329,  8.492023, 3, 21.921875),
             (1339, 10.908205, 3, 20.953125),
             (1341, 21.191723, 3, 21.546875)],
             dtype=[('id', '<i4'), ('intensity', '>f4'), ('channel', 'i1'), ('time', '>f4')])
 
-    >>> for event in r:
-            ...
 
-Installation
-~~~~~~~~~~~~
+as a simple NumPy RecArray (struct of arrays)::
 
-``hesspix`` is a registered Python package. It can be installed using ``pip``::
+    >>> event.pixinfo.intensity
+    array([18.27153 , 23.193665, 11.846128, 15.300814,  8.219065, 15.051192,
+            9.525627,  9.479142, 14.532091, 22.21212 , 11.263601, 16.932125,
+        13.045629, 13.618393, 12.267553,  8.492023, 10.908205, 21.191723],
+        dtype='>f4')
 
-  pip install hesspix
+Accessing individual elements yields "struct-like" instances::
 
-To install the latest development version from the Git repository::
+    >>> event.pixinfo[4]
+    (513, 8.219065, 3, 21.046875)
 
-  pip install git+https://github.com/tamasgal/hesspix
-
-Or clone the repository and run::
-
-  make install
+    >>> event.pixinfo[4].time
+    21.046875
 
-To install all the development dependencies, in case you want to contribute or
-run the test suite::
+    >>> event.pixinfo[4].channel
+    3
 
-  make install-dev
-  make test
+Iterating through all the events in the file can be done with::
 
+    >>> for event in r:
+            ...
 
 ---
 
 *Created with ``cookiecutter https://git.km3net.de/templates/python-project``*
```

### Comparing `hesspix-0.2.0/README.rst` & `hesspix-0.2.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 hesspix 
 =======
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/pipeline.svg
-    :target: https://git.ecap.work/tgal/hesspix/pipelines
+``hesspix`` is a tiny library to read HESS pixel info from ROOT files. No ROOT
+is required.
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/coverage.svg
-    :target: https://tgal.pages.ecap.work/hesspix/coverage
+Installation
+~~~~~~~~~~~~
+
+``hesspix`` is a registered Python package. It can be installed using ``pip``::
+
+  pip install hesspix
 
-.. image:: https://git.km3net.de/examples/km3badges/-/raw/master/docs-latest-brightgreen.svg
-    :target: https://tgal.pages.ecap.work/hesspix
+To install the latest development version from the Git repository::
 
-``hesspix`` is a tiny library to read HESS pixel info from ROOT files.
+  pip install git+https://github.com/tamasgal/hesspix
 
 Usage
 ~~~~~
 
 It's as easy as::
 
     >>> import hesspix as hp
 
     >>> r = hp.CT5Reader("gamma_20deg_180deg_run4151.dst.root")
 
+accessing events via a global index, as written in the ROOT branch::
+
     >>> r[0]
     Event 801 (bunch 0) [10 pixels]
 
     >>> r[23]
     Event 19607 (bunch 0) [3 pixels]
 
+Grabbing an event with a given event number and bunch number::
+
     >>> r.get(event_nr=3902, bunch_nr=0)
     Event 3902 (bunch 0) [18 pixels]
 
     >>> event = r.get(event_nr=3902, bunch_nr=0)
 
+The pixel information is stored in ``pixinfo``::
+
     >>> event.pixinfo
     rec.array([( 352, 18.27153 , 3, 20.9375  ),
             ( 353, 23.193665, 3, 21.703125),
             ( 355, 11.846128, 3, 22.171875),
             ( 357, 15.300814, 3, 21.5     ),
             ( 513,  8.219065, 3, 21.046875),
             (1296, 15.051192, 3, 19.890625),
@@ -49,35 +58,35 @@
             (1324, 13.618393, 3, 20.75    ),
             (1325, 12.267553, 3, 20.953125),
             (1329,  8.492023, 3, 21.921875),
             (1339, 10.908205, 3, 20.953125),
             (1341, 21.191723, 3, 21.546875)],
             dtype=[('id', '<i4'), ('intensity', '>f4'), ('channel', 'i1'), ('time', '>f4')])
 
-    >>> for event in r:
-            ...
 
-Installation
-~~~~~~~~~~~~
+as a simple NumPy RecArray (struct of arrays)::
 
-``hesspix`` is a registered Python package. It can be installed using ``pip``::
+    >>> event.pixinfo.intensity
+    array([18.27153 , 23.193665, 11.846128, 15.300814,  8.219065, 15.051192,
+            9.525627,  9.479142, 14.532091, 22.21212 , 11.263601, 16.932125,
+        13.045629, 13.618393, 12.267553,  8.492023, 10.908205, 21.191723],
+        dtype='>f4')
 
-  pip install hesspix
+Accessing individual elements yields "struct-like" instances::
 
-To install the latest development version from the Git repository::
+    >>> event.pixinfo[4]
+    (513, 8.219065, 3, 21.046875)
 
-  pip install git+https://github.com/tamasgal/hesspix
-
-Or clone the repository and run::
-
-  make install
+    >>> event.pixinfo[4].time
+    21.046875
 
-To install all the development dependencies, in case you want to contribute or
-run the test suite::
+    >>> event.pixinfo[4].channel
+    3
 
-  make install-dev
-  make test
+Iterating through all the events in the file can be done with::
 
+    >>> for event in r:
+            ...
 
 ---
 
 *Created with ``cookiecutter https://git.km3net.de/templates/python-project``*
```

### Comparing `hesspix-0.2.0/doc/Makefile` & `hesspix-0.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/doc/_static/default_gallery_thumbnail.png` & `hesspix-0.2.1/doc/_static/default_gallery_thumbnail.png`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/doc/conf.py` & `hesspix-0.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/doc/make.bat` & `hesspix-0.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/setup.cfg` & `hesspix-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hesspix-0.2.0/src/hesspix/ct5.py` & `hesspix-0.2.1/src/hesspix/ct5.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         # TODO: skipping some header stuff
         s.read(48)
 
         masknbytes = read_uint(s)
         s.read(1)  # skip 1 byte, no idea why
 
-        pixmask = s.read(masknbytes)
+        pixmask = np.frombuffer(s.read(masknbytes), dtype="u1")
         npix = count_set_bits(pixmask)
 
         size = read_uint(s)  # total number of pixels
 
         intensity_data_mode = read_uint(s)
 
         if intensity_data_mode != 2: # enum value for `All`, presumable
@@ -128,27 +128,16 @@
     return bytestream.read(n).decode()
 
 
 def pixmask2pixelids(mask):
     """
     Converts a pixel mask to pixel IDs by returning the indices of set
     bits in the mask.
-
-    This function is rather slow and a good candidate for Numba.
     """
-    pixel_ids = []
-    for i, num in enumerate(mask):
-        for j in range(8):
-            if num & (1 << j):
-                pixel_ids.append(i*8 + j)
-    return pixel_ids
+    return np.where(np.unpackbits(mask, bitorder="little"))[0]
 
 
 def count_set_bits(arr):
     """
-    Count the number of set bits in an array of integers.
+    Count the number of set bits in an array of uint8.
     """
-    count = 0
-    for num in arr:
-        for j in range(8):
-            count += (num >> j) & 1
-    return count
+    return np.count_nonzero(np.unpackbits(arr))
```

### Comparing `hesspix-0.2.0/src/hesspix.egg-info/PKG-INFO` & `hesspix-0.2.1/src/hesspix.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hesspix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tiny library to read HESS pixel info from ROOT files.
 Home-page: https://git.ecap.work/tgal/hesspix
 Author: Tamas Gal
 Author-email: tamas.gal@fau.de
 Maintainer: Tamas Gal
 Maintainer-email: tamas.gal@fau.de
 License: MIT
@@ -62,45 +62,54 @@
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: sphinxcontrib-versioning; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 hesspix 
 =======
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/pipeline.svg
-    :target: https://git.ecap.work/tgal/hesspix/pipelines
+``hesspix`` is a tiny library to read HESS pixel info from ROOT files. No ROOT
+is required.
 
-.. image:: https://git.ecap.work/tgal/hesspix/badges/master/coverage.svg
-    :target: https://tgal.pages.ecap.work/hesspix/coverage
+Installation
+~~~~~~~~~~~~
+
+``hesspix`` is a registered Python package. It can be installed using ``pip``::
+
+  pip install hesspix
 
-.. image:: https://git.km3net.de/examples/km3badges/-/raw/master/docs-latest-brightgreen.svg
-    :target: https://tgal.pages.ecap.work/hesspix
+To install the latest development version from the Git repository::
 
-``hesspix`` is a tiny library to read HESS pixel info from ROOT files.
+  pip install git+https://github.com/tamasgal/hesspix
 
 Usage
 ~~~~~
 
 It's as easy as::
 
     >>> import hesspix as hp
 
     >>> r = hp.CT5Reader("gamma_20deg_180deg_run4151.dst.root")
 
+accessing events via a global index, as written in the ROOT branch::
+
     >>> r[0]
     Event 801 (bunch 0) [10 pixels]
 
     >>> r[23]
     Event 19607 (bunch 0) [3 pixels]
 
+Grabbing an event with a given event number and bunch number::
+
     >>> r.get(event_nr=3902, bunch_nr=0)
     Event 3902 (bunch 0) [18 pixels]
 
     >>> event = r.get(event_nr=3902, bunch_nr=0)
 
+The pixel information is stored in ``pixinfo``::
+
     >>> event.pixinfo
     rec.array([( 352, 18.27153 , 3, 20.9375  ),
             ( 353, 23.193665, 3, 21.703125),
             ( 355, 11.846128, 3, 22.171875),
             ( 357, 15.300814, 3, 21.5     ),
             ( 513,  8.219065, 3, 21.046875),
             (1296, 15.051192, 3, 19.890625),
@@ -114,35 +123,35 @@
             (1324, 13.618393, 3, 20.75    ),
             (1325, 12.267553, 3, 20.953125),
             (1329,  8.492023, 3, 21.921875),
             (1339, 10.908205, 3, 20.953125),
             (1341, 21.191723, 3, 21.546875)],
             dtype=[('id', '<i4'), ('intensity', '>f4'), ('channel', 'i1'), ('time', '>f4')])
 
-    >>> for event in r:
-            ...
 
-Installation
-~~~~~~~~~~~~
+as a simple NumPy RecArray (struct of arrays)::
 
-``hesspix`` is a registered Python package. It can be installed using ``pip``::
+    >>> event.pixinfo.intensity
+    array([18.27153 , 23.193665, 11.846128, 15.300814,  8.219065, 15.051192,
+            9.525627,  9.479142, 14.532091, 22.21212 , 11.263601, 16.932125,
+        13.045629, 13.618393, 12.267553,  8.492023, 10.908205, 21.191723],
+        dtype='>f4')
 
-  pip install hesspix
+Accessing individual elements yields "struct-like" instances::
 
-To install the latest development version from the Git repository::
+    >>> event.pixinfo[4]
+    (513, 8.219065, 3, 21.046875)
 
-  pip install git+https://github.com/tamasgal/hesspix
-
-Or clone the repository and run::
-
-  make install
+    >>> event.pixinfo[4].time
+    21.046875
 
-To install all the development dependencies, in case you want to contribute or
-run the test suite::
+    >>> event.pixinfo[4].channel
+    3
 
-  make install-dev
-  make test
+Iterating through all the events in the file can be done with::
 
+    >>> for event in r:
+            ...
 
 ---
 
 *Created with ``cookiecutter https://git.km3net.de/templates/python-project``*
```

### Comparing `hesspix-0.2.0/src/hesspix.egg-info/SOURCES.txt` & `hesspix-0.2.1/src/hesspix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

