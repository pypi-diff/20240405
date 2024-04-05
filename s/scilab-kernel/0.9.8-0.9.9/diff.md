# Comparing `tmp/scilab_kernel-0.9.8.tar.gz` & `tmp/scilab_kernel-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scilab_kernel-0.9.8.tar", last modified: Mon Apr 29 10:48:03 2019, max compression
+gzip compressed data, was "dist/scilab_kernel-0.9.9.tar", last modified: Fri May  3 12:41:38 2019, max compression
```

## Comparing `scilab_kernel-0.9.8.tar` & `scilab_kernel-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/
--rw-r--r--   0 silvester  (1000) silvester  (1000)      752 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/HISTORY.rst
--rw-r--r--   0 silvester  (1000) silvester  (1000)      230 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/MANIFEST.in
--rw-r--r--   0 silvester  (1000) silvester  (1000)      969 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/Makefile
--rw-r--r--   0 silvester  (1000) silvester  (1000)     2447 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/PKG-INFO
--rw-r--r--   0 silvester  (1000) silvester  (1000)     1318 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/README.rst
-drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel/
--rw-r--r--   0 silvester  (1000) silvester  (1000)       57 2019-04-29 10:47:58.000000 scilab_kernel-0.9.8/scilab_kernel/__init__.py
--rw-r--r--   0 silvester  (1000) silvester  (1000)       93 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/scilab_kernel/__main__.py
--rwxr-xr-x   0 silvester  (1000) silvester  (1000)      528 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/scilab_kernel/_make_figures.sci
-drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel/images/
--rw-r--r--   0 silvester  (1000) silvester  (1000)     2670 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/scilab_kernel/images/logo-32x32.png
--rw-r--r--   0 silvester  (1000) silvester  (1000)     4891 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/scilab_kernel/images/logo-64x64.png
--rw-r--r--   0 silvester  (1000) silvester  (1000)      214 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/scilab_kernel/kernel.json
--rw-r--r--   0 silvester  (1000) silvester  (1000)     9253 2019-04-29 10:46:56.000000 scilab_kernel-0.9.8/scilab_kernel/kernel.py
-drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/
--rw-r--r--   0 silvester  (1000) silvester  (1000)     2447 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/PKG-INFO
--rw-r--r--   0 silvester  (1000) silvester  (1000)      464 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 silvester  (1000) silvester  (1000)        1 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 silvester  (1000) silvester  (1000)       52 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/requires.txt
--rw-r--r--   0 silvester  (1000) silvester  (1000)       14 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/scilab_kernel.egg-info/top_level.txt
--rw-r--r--   0 silvester  (1000) silvester  (1000)       38 2019-04-29 10:48:03.000000 scilab_kernel-0.9.8/setup.cfg
--rw-r--r--   0 silvester  (1000) silvester  (1000)     1996 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/setup.py
--rw-r--r--   0 silvester  (1000) silvester  (1000)      605 2019-04-18 13:08:00.000000 scilab_kernel-0.9.8/test_scilab_kernel.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      752 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/HISTORY.rst
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      230 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/MANIFEST.in
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      969 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/Makefile
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2870 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/PKG-INFO
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1621 2019-05-03 12:40:34.000000 scilab_kernel-0.9.9/README.rst
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/scilab_kernel/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       57 2019-05-03 12:41:34.000000 scilab_kernel-0.9.9/scilab_kernel/__init__.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       93 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/scilab_kernel/__main__.py
+-rwxr-xr-x   0 silvester  (1000) silvester  (1000)      528 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/scilab_kernel/_make_figures.sci
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      504 2019-05-03 12:37:32.000000 scilab_kernel-0.9.9/scilab_kernel/check.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/scilab_kernel/images/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2670 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/scilab_kernel/images/logo-32x32.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     4891 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/scilab_kernel/images/logo-64x64.png
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      214 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/scilab_kernel/kernel.json
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     9253 2019-04-29 10:46:56.000000 scilab_kernel-0.9.9/scilab_kernel/kernel.py
+drwxr-xr-x   0 silvester  (1000) silvester  (1000)        0 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     2870 2019-05-03 12:41:37.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      487 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)        1 2019-05-03 12:41:37.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       52 2019-05-03 12:41:37.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/requires.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       14 2019-05-03 12:41:37.000000 scilab_kernel-0.9.9/scilab_kernel.egg-info/top_level.txt
+-rw-r--r--   0 silvester  (1000) silvester  (1000)       38 2019-05-03 12:41:38.000000 scilab_kernel-0.9.9/setup.cfg
+-rw-r--r--   0 silvester  (1000) silvester  (1000)     1996 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/setup.py
+-rw-r--r--   0 silvester  (1000) silvester  (1000)      605 2019-04-18 13:08:00.000000 scilab_kernel-0.9.9/test_scilab_kernel.py
```

### Comparing `scilab_kernel-0.9.8/HISTORY.rst` & `scilab_kernel-0.9.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/Makefile` & `scilab_kernel-0.9.9/Makefile`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/PKG-INFO` & `scilab_kernel-0.9.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 Metadata-Version: 1.2
 Name: scilab_kernel
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Jupyter kernel for Scilab.
 Home-page: http://github.com/calsto/scilab_kernel
 Maintainer: Steven Silvester
 Maintainer-email: steven.silvester@ieee.org
 License: MIT
 Download-URL: http://github.com/calsto/scilab_kernel
 Description: A Jupyter kernel for Scilab
         
-        This requires Scilab and `Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
+        Prerequisites
+        -------------
+        `Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
         
-        To install::
+        Installation
+        ------------
         
             pip install scilab_kernel
         
         To use it, run one of:
         
         .. code:: shell
         
             ipython notebook
             # In the notebook interface, select Scilab from the 'New' menu
             ipython qtconsole --kernel scilab
             ipython console --kernel scilab
         
-        This is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
-        which means it features a standard set of magics.
+        This kernel is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
+        which means it features a standard set of magics.  For a full list of magics,
+        run ``%lsmagic`` in a cell.
         
         A sample notebook is available online_.
         
         You can specify the path to your Scilab executable by creating a ``SCILAB_EXECUTABLE`` environmental variable.  Use the ``scilab-adv-cli`` executable if using a Posix-like OS, and ``WScilex-cli.exe`` if using Windows.
         
         
-        Advanced Installation Notes::
+        Troubleshooting
+        ---------------
+        If the kernel is not starting, try running the following from a terminal.
+        
+        .. code
+          python -m scilab_kernel.check
+        
+        Please include that output if opening an issue.
+        
+        
+        Advanced Installation Notes
+        ---------------------------
         We automatically install a Jupyter kernelspec when installing the
         python package.  This location can be found using ``jupyter kernelspec list``.
         If the default location is not desired, you can remove the directory for the
         ``scilab`` kernel, and install using `python -m scilab_kernel install`.  See
         ``python -m scilab_kernel install --help`` for available options.
         
         .. _online: http://nbviewer.ipython.org/github/calysto/scilab_kernel/blob/master/scilab_kernel.ipynb
```

### Comparing `scilab_kernel-0.9.8/README.rst` & `scilab_kernel-0.9.9/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 A Jupyter kernel for Scilab
 
-This requires Scilab and `Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
+Prerequisites
+-------------
+`Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
 
-To install::
+Installation
+------------
 
     pip install scilab_kernel
 
 To use it, run one of:
 
 .. code:: shell
 
     ipython notebook
     # In the notebook interface, select Scilab from the 'New' menu
     ipython qtconsole --kernel scilab
     ipython console --kernel scilab
 
-This is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
-which means it features a standard set of magics.
+This kernel is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
+which means it features a standard set of magics.  For a full list of magics,
+run ``%lsmagic`` in a cell.
 
 A sample notebook is available online_.
 
 You can specify the path to your Scilab executable by creating a ``SCILAB_EXECUTABLE`` environmental variable.  Use the ``scilab-adv-cli`` executable if using a Posix-like OS, and ``WScilex-cli.exe`` if using Windows.
 
 
-Advanced Installation Notes::
+Troubleshooting
+---------------
+If the kernel is not starting, try running the following from a terminal.
+
+.. code
+  python -m scilab_kernel.check
+
+Please include that output if opening an issue.
+
+
+Advanced Installation Notes
+---------------------------
 We automatically install a Jupyter kernelspec when installing the
 python package.  This location can be found using ``jupyter kernelspec list``.
 If the default location is not desired, you can remove the directory for the
 ``scilab`` kernel, and install using `python -m scilab_kernel install`.  See
 ``python -m scilab_kernel install --help`` for available options.
 
 .. _online: http://nbviewer.ipython.org/github/calysto/scilab_kernel/blob/master/scilab_kernel.ipynb
```

### Comparing `scilab_kernel-0.9.8/scilab_kernel/_make_figures.sci` & `scilab_kernel-0.9.9/scilab_kernel/_make_figures.sci`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/scilab_kernel/images/logo-32x32.png` & `scilab_kernel-0.9.9/scilab_kernel/images/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/scilab_kernel/images/logo-64x64.png` & `scilab_kernel-0.9.9/scilab_kernel/images/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/scilab_kernel/kernel.py` & `scilab_kernel-0.9.9/scilab_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/scilab_kernel.egg-info/PKG-INFO` & `scilab_kernel-0.9.9/scilab_kernel.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 Metadata-Version: 1.2
 Name: scilab-kernel
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Jupyter kernel for Scilab.
 Home-page: http://github.com/calsto/scilab_kernel
 Maintainer: Steven Silvester
 Maintainer-email: steven.silvester@ieee.org
 License: MIT
 Download-URL: http://github.com/calsto/scilab_kernel
 Description: A Jupyter kernel for Scilab
         
-        This requires Scilab and `Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
+        Prerequisites
+        -------------
+        `Jupyter Notebook <http://jupyter.readthedocs.org/en/latest/install.html>`_, and `Scilab <http://www.scilab.org/download/latest>`_.
         
-        To install::
+        Installation
+        ------------
         
             pip install scilab_kernel
         
         To use it, run one of:
         
         .. code:: shell
         
             ipython notebook
             # In the notebook interface, select Scilab from the 'New' menu
             ipython qtconsole --kernel scilab
             ipython console --kernel scilab
         
-        This is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
-        which means it features a standard set of magics.
+        This kernel is based on `MetaKernel <http://pypi.python.org/pypi/metakernel>`_,
+        which means it features a standard set of magics.  For a full list of magics,
+        run ``%lsmagic`` in a cell.
         
         A sample notebook is available online_.
         
         You can specify the path to your Scilab executable by creating a ``SCILAB_EXECUTABLE`` environmental variable.  Use the ``scilab-adv-cli`` executable if using a Posix-like OS, and ``WScilex-cli.exe`` if using Windows.
         
         
-        Advanced Installation Notes::
+        Troubleshooting
+        ---------------
+        If the kernel is not starting, try running the following from a terminal.
+        
+        .. code
+          python -m scilab_kernel.check
+        
+        Please include that output if opening an issue.
+        
+        
+        Advanced Installation Notes
+        ---------------------------
         We automatically install a Jupyter kernelspec when installing the
         python package.  This location can be found using ``jupyter kernelspec list``.
         If the default location is not desired, you can remove the directory for the
         ``scilab`` kernel, and install using `python -m scilab_kernel install`.  See
         ``python -m scilab_kernel install --help`` for available options.
         
         .. _online: http://nbviewer.ipython.org/github/calysto/scilab_kernel/blob/master/scilab_kernel.ipynb
```

### Comparing `scilab_kernel-0.9.8/setup.py` & `scilab_kernel-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `scilab_kernel-0.9.8/test_scilab_kernel.py` & `scilab_kernel-0.9.9/test_scilab_kernel.py`

 * *Files identical despite different names*

