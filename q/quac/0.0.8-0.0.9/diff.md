# Comparing `tmp/quac-0.0.8.tar.gz` & `tmp/quac-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quac-0.0.8.tar", last modified: Fri Mar  8 15:17:17 2024, max compression
+gzip compressed data, was "quac-0.0.9.tar", last modified: Fri Mar  8 15:34:57 2024, max compression
```

## Comparing `quac-0.0.8.tar` & `quac-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:17:17.082085 quac-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-27 14:59:07.000000 quac-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-27 14:59:07.000000 quac-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-08 15:17:17.081946 quac-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2024-03-05 14:01:53.000000 quac-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:17:17.080832 quac-0.0.8/quac/
--rw-r--r--   0 solst      (501) staff       (20)     1106 2024-03-08 15:16:39.000000 quac-0.0.8/quac/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    42864 2024-03-08 15:16:39.000000 quac-0.0.8/quac/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1741 2024-03-08 15:16:39.000000 quac-0.0.8/quac/base.py
--rw-r--r--   0 solst      (501) staff       (20)     9762 2024-03-08 15:16:39.000000 quac-0.0.8/quac/chic.py
--rw-r--r--   0 solst      (501) staff       (20)     4986 2024-03-08 15:16:39.000000 quac-0.0.8/quac/cons.py
--rw-r--r--   0 solst      (501) staff       (20)    32167 2024-03-08 15:16:39.000000 quac-0.0.8/quac/duck.py
--rw-r--r--   0 solst      (501) staff       (20)    22471 2024-03-08 15:16:39.000000 quac-0.0.8/quac/eggs.py
--rw-r--r--   0 solst      (501) staff       (20)     3084 2024-03-08 15:16:39.000000 quac-0.0.8/quac/enum.py
--rw-r--r--   0 solst      (501) staff       (20)      716 2024-03-08 15:16:39.000000 quac-0.0.8/quac/errs.py
--rw-r--r--   0 solst      (501) staff       (20)    11884 2024-03-08 15:16:39.000000 quac-0.0.8/quac/grds.py
--rw-r--r--   0 solst      (501) staff       (20)    19854 2024-03-08 15:16:39.000000 quac-0.0.8/quac/meta.py
--rw-r--r--   0 solst      (501) staff       (20)     9096 2024-03-08 15:16:39.000000 quac-0.0.8/quac/misc.py
--rw-r--r--   0 solst      (501) staff       (20)     6045 2024-03-08 15:16:39.000000 quac-0.0.8/quac/mods.py
--rw-r--r--   0 solst      (501) staff       (20)     4683 2024-03-08 15:16:39.000000 quac-0.0.8/quac/prot.py
--rw-r--r--   0 solst      (501) staff       (20)     1466 2024-03-08 15:16:39.000000 quac-0.0.8/quac/solo.py
--rw-r--r--   0 solst      (501) staff       (20)     3080 2024-03-08 15:16:39.000000 quac-0.0.8/quac/spec.py
--rw-r--r--   0 solst      (501) staff       (20)      652 2024-03-08 15:16:39.000000 quac-0.0.8/quac/type.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:17:17.081755 quac-0.0.8/quac.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      476 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-04 15:56:42.000000 quac-0.0.8/quac.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-08 15:17:17.000000 quac-0.0.8/quac.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      735 2024-03-08 14:50:07.000000 quac-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-08 15:17:17.082120 quac-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-02-27 14:59:07.000000 quac-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:34:57.801147 quac-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-27 14:59:07.000000 quac-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-27 14:59:07.000000 quac-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-08 15:34:57.800947 quac-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2024-03-05 14:01:53.000000 quac-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:34:57.799947 quac-0.0.9/quac/
+-rw-r--r--   0 solst      (501) staff       (20)     1106 2024-03-08 15:34:51.000000 quac-0.0.9/quac/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    42975 2024-03-08 15:34:51.000000 quac-0.0.9/quac/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1741 2024-03-08 15:34:51.000000 quac-0.0.9/quac/base.py
+-rw-r--r--   0 solst      (501) staff       (20)    10177 2024-03-08 15:34:51.000000 quac-0.0.9/quac/chic.py
+-rw-r--r--   0 solst      (501) staff       (20)     4986 2024-03-08 15:34:51.000000 quac-0.0.9/quac/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)    33239 2024-03-08 15:34:51.000000 quac-0.0.9/quac/duck.py
+-rw-r--r--   0 solst      (501) staff       (20)    22471 2024-03-08 15:34:51.000000 quac-0.0.9/quac/eggs.py
+-rw-r--r--   0 solst      (501) staff       (20)     3084 2024-03-08 15:34:51.000000 quac-0.0.9/quac/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)      716 2024-03-08 15:34:51.000000 quac-0.0.9/quac/errs.py
+-rw-r--r--   0 solst      (501) staff       (20)    11884 2024-03-08 15:34:51.000000 quac-0.0.9/quac/grds.py
+-rw-r--r--   0 solst      (501) staff       (20)    19854 2024-03-08 15:34:51.000000 quac-0.0.9/quac/meta.py
+-rw-r--r--   0 solst      (501) staff       (20)     9096 2024-03-08 15:34:51.000000 quac-0.0.9/quac/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)     6045 2024-03-08 15:34:51.000000 quac-0.0.9/quac/mods.py
+-rw-r--r--   0 solst      (501) staff       (20)     4683 2024-03-08 15:34:51.000000 quac-0.0.9/quac/prot.py
+-rw-r--r--   0 solst      (501) staff       (20)     1466 2024-03-08 15:34:51.000000 quac-0.0.9/quac/solo.py
+-rw-r--r--   0 solst      (501) staff       (20)     3080 2024-03-08 15:34:51.000000 quac-0.0.9/quac/spec.py
+-rw-r--r--   0 solst      (501) staff       (20)      652 2024-03-08 15:34:51.000000 quac-0.0.9/quac/type.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-08 15:34:57.800794 quac-0.0.9/quac.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      476 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-04 15:56:42.000000 quac-0.0.9/quac.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-08 15:34:57.000000 quac-0.0.9/quac.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      735 2024-03-08 15:18:23.000000 quac-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-08 15:34:57.801208 quac-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-02-27 14:59:07.000000 quac-0.0.9/setup.py
```

### Comparing `quac-0.0.8/LICENSE` & `quac-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/PKG-INFO` & `quac-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quac
-Version: 0.0.8
+Version: 0.0.9
 Summary: quac
 Home-page: https://github.com/dsm-72/quac
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: quac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `quac-0.0.8/README.md` & `quac-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/__init__.py` & `quac-0.0.9/quac/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = ['loadmod']
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `quac-0.0.8/quac/_modidx.py` & `quac-0.0.9/quac/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
                            'quac.duck.csrarray': ('duck.html#csrarray', 'quac/duck.py'),
                            'quac.duck.csrmatrix': ('duck.html#csrmatrix', 'quac/duck.py'),
                            'quac.duck.cv2vidcap': ('duck.html#cv2vidcap', 'quac/duck.py'),
                            'quac.duck.dataframe': ('duck.html#dataframe', 'quac/duck.py'),
                            'quac.duck.datasource': ('duck.html#datasource', 'quac/duck.py'),
                            'quac.duck.datatype': ('duck.html#datatype', 'quac/duck.py'),
                            'quac.duck.device': ('duck.html#device', 'quac/duck.py'),
+                           'quac.duck.device.__metahook__': ('duck.html#device.__metahook__', 'quac/duck.py'),
                            'quac.duck.deviceq': ('duck.html#deviceq', 'quac/duck.py'),
                            'quac.duck.diaarray': ('duck.html#diaarray', 'quac/duck.py'),
                            'quac.duck.diamatrix': ('duck.html#diamatrix', 'quac/duck.py'),
                            'quac.duck.dictitems': ('duck.html#dictitems', 'quac/duck.py'),
                            'quac.duck.dictkeys': ('duck.html#dictkeys', 'quac/duck.py'),
                            'quac.duck.dictq': ('duck.html#dictq', 'quac/duck.py'),
                            'quac.duck.dictvalues': ('duck.html#dictvalues', 'quac/duck.py'),
```

### Comparing `quac-0.0.8/quac/base.py` & `quac-0.0.9/quac/base.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/chic.py` & `quac-0.0.9/quac/chic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/50_chic.ipynb.
 
 # %% auto 0
 __all__ = ['boolfunc', 'flagfunc', 'numeric', 'numbers', 'emptystring', 'notemptystring', 'pttn', 'dirpath', 'dirnames',
            'filenames', 'enummember', 'layer', 'boundingbox', 'coordinate', 'coord', 'point', 'xypos', 'width',
            'height', 'rect', 'clsint', 'clsset', 'clsstr', 'clsobj', 'clsbool', 'clsbool01', 'clscall', 'clstype',
            'clslist', 'clsfloat', 'clsnum', 'clscomplex', 'slc', 'slcs', 'path', 'boolidx', 'bidx', 'catidx', 'cidx',
-           'boolcall', 'boolcallq', 'boolcalls', 'docgenfn', 'axesidxs', 'argstype', 'sysexcinfotype', 'sysformatstyle',
-           'bbox', 'rgb', 'rgba', 'color', 'imagesize', 'videosize', 'imagesizeq', 'videosizeq', 'mixin']
+           'anndata', 'anndatas', 'series', 'index', 'boolcall', 'boolcallq', 'boolcalls', 'docgenfn', 'axesidxs',
+           'argstype', 'sysexcinfotype', 'sysformatstyle', 'bbox', 'rgb', 'rgba', 'color', 'imagesize', 'videosize',
+           'imagesizeq', 'videosizeq', 'mixin']
 
 # %% ../nbs/50_chic.ipynb 6
 from enum import member, _EnumDict
 
 # %% ../nbs/50_chic.ipynb 8
 from types import ModuleType, TracebackType
 
@@ -264,7 +265,20 @@
 bidx: TypeAlias = duck.boolindex
 '''A type alias for a boolean index.''';
 catidx: TypeAlias = duck.catindex
 '''A type alias for a categorical index.''';
 cidx: TypeAlias = duck.catindex
 '''A type alias for a categorical index.''';
 
+
+# %% ../nbs/50_chic.ipynb 46
+anndata: TypeAlias = duck.adata
+'''A type alias for an `AnnData` object.''';
+
+anndatas: TypeAlias = duck.adatas
+'''A type alias for a list of  `AnnData` object.''';
+
+series: TypeAlias = duck.pdseries
+'''A type alias for a `pandas.Series` object.''';
+
+index: TypeAlias = duck.pdindex
+'''A type alias for a `pandas.Index` object.''';
```

### Comparing `quac-0.0.8/quac/cons.py` & `quac-0.0.9/quac/cons.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/duck.py` & `quac-0.0.9/quac/duck.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,20 +302,20 @@
     __ducktype__ = (eggs.pl_path, )
 
 class posixpath(Duck):
     '''`pathlib.PosixPath`'''
     __ducktype__ = (eggs.pl_posixpath, )
 
 # %% ../nbs/40_duck.ipynb 68
-class pathlike(Duck):
+class pathlike(Duck, Generic[*Ts]):
     '''`os.PathLike`, `pathlib.Path`, `pathlib.PosixPath`'''
     __ducktype__ = (str, bytes, eggs.os_pathlike, eggs.pl_path, eggs.pl_posixpath)    
 
 # %% ../nbs/40_duck.ipynb 69
-class pathq(pathlike):
+class pathq(pathlike, Generic[*Ts]):
     __species__ = Species.OPT
 
 # %% ../nbs/40_duck.ipynb 71
 class paths(notiterstr):
     '''A type alias for a list of paths.'''
     __expected__ = dict(dtype=pathlike)
 
@@ -363,15 +363,15 @@
     __ducktype__ = (eggs.t_functiontype, )
     
 class mapping(Duck):
     '''`collections.Mapping`'''
     __ducktype__ = (eggs.c_mapping, )
 
 # %% ../nbs/40_duck.ipynb 78
-class moduleq(moduletype):
+class moduleq(moduletype, Generic[T]):
     '''`Optional[types.ModuleType]`'''
     __species__ = Species.OPT
 
 # %% ../nbs/40_duck.ipynb 80
 class callq(Duck[Callable[P, T]]):
     '''`Optional[Callable[P, T]]`'''
     __ducktype__ = (Callable, )
@@ -482,41 +482,41 @@
 
 class mplaxes(Duck): 
     '''`matplotlib.axes._axes.Axes`'''
     __ducktype__ = (eggs.mpl_axes, )
     
 
 # %% ../nbs/40_duck.ipynb 97
-class nparray(Duck):
+class nparray(Duck, Generic[*Ts]): 
     '''`numpy.ndarray`''';
     __ducktype__ = (eggs.np_array, )
     
-class npmatrix(Duck):
+class npmatrix(Duck, Generic[*Ts]): 
     '''`numpy.matrix`''';
     __ducktype__ = (eggs.np_matrix, )
 
-class recarray(Duck):
+class recarray(Duck, Generic[*Ts]): 
     '''`numpy.recarray`''';
     __ducktype__ = (eggs.np_recarray, )
     
 class npempty(Duck):
     '''`numpy.empty`''';
     __ducktype__ = (eggs.np_empty, )
 
 # %% ../nbs/40_duck.ipynb 98
 class npdatasource(Duck): 
     '''`numpy.DataSource`''';
     __ducktype__ = (eggs.np_datasource, )
 
 # %% ../nbs/40_duck.ipynb 100
-class sparray(Duck): 
+class sparray(Duck, Generic[*Ts]): 
     '''`scipy.sparse.aparray`''';
     __ducktype__ = (eggs.sp_sparray, )
 
-class spmatrix(Duck): 
+class spmatrix(Duck, Generic[*Ts]): 
     '''`scipy.sparse.spmatrix`''';
     __ducktype__ = (eggs.sp_spmatrix, )
     
 
 # %% ../nbs/40_duck.ipynb 102
 class cscarray(Duck):
     '''`scipy.sparse.csc_array`''';
@@ -571,40 +571,40 @@
     __ducktype__ = (eggs.sp_bsr_array, )
 
 class bsrmatrix(Duck):
     '''`scipy.sparse.bsr_matrix`''';
     __ducktype__ = (eggs.sp_bsr_matrix, )
 
 # %% ../nbs/40_duck.ipynb 104
-class sparsearray(Duck): 
+class sparsearray(Duck, Generic[*Ts]): 
     '''sparse array (e.g. 
     `scipy.sparse.sparray`, `scipy.sparse.cscarray`, `scipy.sparse.cooarray`, 
     `scipy.sparse.csrarray`, `scipy.sparse.diaarray`, `scipy.sparse.dokarray`, 
     `scipy.sparse.lilarray`, or `scipy.sparse.bsrarray`)'''
     __ducktype__ = (sparray, cscarray, cooarray, csrarray, diaarray, dokarray, lilarray, bsrarray)
     
     
-class sparsematrix(Duck): 
+class sparsematrix(Duck, Generic[*Ts]): 
     '''sparse type (e.g.  
     `scipy.sparse.spmatrix`, `scipy.sparse.cscmatrix`, `scipy.sparse.coomatrix`, 
     `scipy.sparse.csrmatrix`, `scipy.sparse.diamatrix`, `scipy.sparse.dokmatrix`, 
     `scipy.sparse.lilmatrix`, or `scipy.sparse.bsrmatrix`)'''
     __ducktype__ = (spmatrix, cscmatrix, coomatrix, csrmatrix, diamatrix, dokmatrix, lilmatrix, bsrmatrix)
 
 
 # %% ../nbs/40_duck.ipynb 106
-class sparse(Duck): 
+class sparse(Duck, Generic[*Ts]): 
     '''sparse type (e.g. `sparsearray` or `sparsematrix`)'''
     __ducktype__ = (sparray, sparsematrix)
     
-class array(Duck): 
+class array(Duck, Generic[*Ts]): 
     '''array type (e.g. `np.array`, `np.recarray`, `sp.sparray`, `itertype`, or `list`)'''
     __ducktype__ = (nparray, recarray, sparray, itertype, list)
     
-class matrix(Duck): 
+class matrix(Duck, Generic[*Ts]): 
     '''matrix type(e.g. `np.matrix`, `sp.matrix`, `itertype`, or `list`)'''
     __ducktype__ = (npmatrix, spmatrix, itertype, list)
 
 # %% ../nbs/40_duck.ipynb 107
 class sparseq(sparse): 
     '''Optional sparse type (e.g. `sparsearray` or `sparsematrix`)'''
     __species__ = Species.OPT
@@ -656,25 +656,25 @@
     __ducktype__ = (eggs.pd_index, )
     
 class pdcatindex(Duck):
     '''`pandas.CategoricalIndex`''';
     __ducktype__ = (eggs.pd_catindex, )
 
 # %% ../nbs/40_duck.ipynb 121
-class pdseries(Duck):
+class pdseries(Duck, Generic[*Ts]):
     '''`pandas.Series`''';
     __ducktype__ = (eggs.pd_series, )
 
 # %% ../nbs/40_duck.ipynb 123
-class boolindex(Duck): 
+class boolindex(Duck, Generic[*Ts]):
     '''boolean index'''
     __ducktype__ = (list, pdindex, nparray, bools, )
     __expected__ = dict(dtype=bool01)
     
-class catindex(Duck): 
+class catindex(Duck, Generic[*Ts]):
     '''categorical index'''
     __ducktype__ = (pdcatindex, )
 
 # %% ../nbs/40_duck.ipynb 124
 class boolindexq(Duck): 
     '''Optional[booleanindex]'''
     __species__ = Species.OPT
@@ -691,98 +691,98 @@
     
 class indexlike(Duck): 
     '''index-like objects (e.g. `list`, `tuple`,`bools`, `nums`, 
     `itertype`, `pd.Index`, `pd.CategoricalIndex`, `boolindex`, or `np.array`)'''
     __ducktype__ = (list, tuple, bools, nums, itertype, pdindex, pdcatindex, boolindex, nparray)
 
 # %% ../nbs/40_duck.ipynb 128
-class seriestype(Duck): 
+class seriestype(Duck, Generic[*Ts]):
     '''series type (e.g. `pd.Series`, `np.array`, `np.recarray`, `list`, or `indexlike`)'''
     __ducktype__ = (pdseries, nparray, recarray, list, indexlike)
     
 
-class serieslike(Duck): 
+class serieslike(Duck, Generic[*Ts]):
     '''series-like type'''
     __ducktype__ = (pdseries, nparray, recarray, list, indexlike)
 
 # %% ../nbs/40_duck.ipynb 130
-class pddataframe(Duck): 
+class pddataframe(Duck, Generic[*Ts]):
     '''`pandas.DataFrame`''';
     __ducktype__ = (eggs.pd_dataframe, )
 
 # %% ../nbs/40_duck.ipynb 132
-class dataframe(Duck): 
+class dataframe(Duck, Generic[*Ts]):
     '''`pandas.DataFrame`''';
     __ducktype__ = (eggs.pd_dataframe, )
 
 # %% ../nbs/40_duck.ipynb 135
-class pttype(Duck): 
+class pttype(Duck, Generic[*Ts]):
     '''`torch.dtype`'''
     __ducktype__ = (eggs.pt_type, )
 
 # %% ../nbs/40_duck.ipynb 137
 class memfmt(Duck): 
     '''`torch.memory_format`''';
     __ducktype__ = (eggs.pt_memoryformat, )
 
 class presfmt(Duck): 
     '''`torch.preserve_format`''';
     __ducktype__ = (eggs.pt_preserveformat, )
 
 # %% ../nbs/40_duck.ipynb 139
-class ptsize(Duck): 
+class ptsize(Duck, Generic[*Ts]):
     '''`torch.Size`'''
     __ducktype__ = (eggs.pt_size, iterable, tuple, )
 
 # %% ../nbs/40_duck.ipynb 141
-class ptdevice(Duck): 
+class ptdevice(Duck, Generic[*Ts]):
     '''`torch.device`'''
     __ducktype__ = (eggs.pt_device, iterable, tuple, )
 
-class ptdeviceq(ptdevice):
+class ptdeviceq(ptdevice, Generic[*Ts]):
     '''`Optional[torch.device]`'''
     __species__ = Species.OPT
 
 # %% ../nbs/40_duck.ipynb 143
-class pttensor(Duck): 
+class pttensor(Duck, Generic[*Ts]): 
     '''`torch.Tensor`''';
     __ducktype__ = (eggs.pt_tensor, )
     
-class inttensor(Duck): 
+class inttensor(Duck, Generic[*Ts]): 
     '''`torch.IntTensor`''';
     __ducktype__ = (eggs.pt_inttensor, )
     
-class booltensor(Duck): 
+class booltensor(Duck, Generic[*Ts]): 
     '''`torch.BoolTensor`''';
     __ducktype__ = (eggs.pt_booltensor, )
     
-class floattensor(Duck): 
+class floattensor(Duck, Generic[*Ts]): 
     '''`torch.FloatTensor`''';
     __ducktype__ = (eggs.pt_floattensor, )
     
-class longtensor(Duck): 
+class longtensor(Duck, Generic[*Ts]): 
     '''`torch.LongTensor`''';
     __ducktype__ = (eggs.pt_longtensor, )
     
-class doubletensor(Duck): 
+class doubletensor(Duck, Generic[*Ts]): 
     '''`torch.DoubleTensor`''';
     __ducktype__ = (eggs.pt_doubletensor, )
 
 # %% ../nbs/40_duck.ipynb 145
-class nantensor(Duck): 
+class nantensor(Duck, Generic[*Ts]): 
     '''tensor of `nan`s'''
     __ducktype__ = (pttensor, nans, )
     __expected__ = dict(dtype=nan)
 
 # %% ../nbs/40_duck.ipynb 147
-class tensor(Duck): 
+class tensor(Duck, Generic[*Ts]): 
     '''tensor type (e.g. `torch.tensor`, `torch.IntTensor`, `torch.BoolTensor`, or `torch.FloatTensor`)'''
     __ducktype__ = (pttensor, inttensor, booltensor, floattensor, longtensor, doubletensor, )
     
-class tensorq(tensor):
+class tensorq(tensor, Generic[*Ts]): 
     '''`Optional[tensor]`'''
     __species__ = Species.OPT
 
 # %% ../nbs/40_duck.ipynb 149
 class ptmodule(Duck): 
     '''`torch.nn.Module`'''
     __ducktype__ = (eggs.pt_module, )
@@ -845,60 +845,71 @@
 
 class brownianintervial(Duck): 
     '''`torchsde.BrownianInterval`'''
     __ducktype__ = (eggs.ts_brownianinterval, )
 
 
 # %% ../nbs/40_duck.ipynb 163
-class dtype(Duck): 
+class dtype(Duck, Generic[*Ts]):
     '''Type of data (e.g. `np.dtype` or `torch.dtype`)'''
     __ducktype__ = (type, eggs.np_type, eggs.pt_type, )
 
 # %% ../nbs/40_duck.ipynb 165
-class device(Duck): 
+class device(Duck, Generic[*Ts]):
     '''`torch.device`'''
-    __ducktype__ = (eggs.pt_device, )
+    __ducktype__ = (eggs.pt_device, str, )
+    __extrafns__ = dict(type=lambda obj, val: getattr(obj, 'type', None) == val)
+    __dev__: ClassVar[str] = None
     
-class deviceq(Duck): 
+    @classmethod
+    def __metahook__(cls, mcls, name, bases, namespace, **kwargs):
+        super().__metahook__(mcls, name, bases, namespace, **kwargs)
+        d = cls.__dev__
+        isdev = lambda obj, val: grds.isnone(val) or (grds.notnone(val) and hasattr(obj, 'type') and val == d)
+        cls.__expected__.update(__dev__=d)
+        cls.__extrafns__.update(__dev__=isdev)
+        return cls
+    
+class deviceq(Duck, Generic[*Ts]): 
     '''`Optional [torch.device]`'''
     __species__ = Species.OPT
 
 # %% ../nbs/40_duck.ipynb 167
 class size(Duck, Generic[*Ts]): 
     '''size type (e.g. `tuple`, `torch.Size`, `itertype`)'''
     __ducktype__ = (tuple, ptsize, itertype, )
     __expected__ = dict(dtype=int)
 
 # %% ../nbs/40_duck.ipynb 169
-class datasource(Duck): 
+class datasource(Duck, Generic[*Ts]): 
     '''`numpy.DataSource`''';
     __ducktype__ = (eggs.np_datasource, )   
 
 # %% ../nbs/40_duck.ipynb 171
 class adata(Duck): 
     '''`anndata.AnnData`''';
     __ducktype__ = (eggs.ad_adata, )
 
-class adatas(Duck): 
+class adatas(Duck, Generic[*Ts]): 
     '''`anndata.AnnData`''';
     __ducktype__ = (itertype, )
     __expected__ = dict(dtype=adata)
 
 # %% ../nbs/40_duck.ipynb 173
-class graphtype(Duck): 
+class graphtype(Duck, Generic[*Ts]): 
     '''graph type (e.g. `BaseGraph`, `DataGraph`, `LandmarkGraph`, `kNNGraph`, `TraditionalGraph`, 
     `MNNGraph`, `kNNLandmarkGraph`, `TraditionalLandmarkGraph`, or `MNNLandmarkGraph`)'''
     __ducktype__ = (
         eggs.gt_bgraph, eggs.gt_dgraph, eggs.gt_lgraph, 
         eggs.gt_kgraph, eggs.gt_tgraph, eggs.gt_mgraph, 
         eggs.gt_klgraph, eggs.gt_tlgraph, eggs.gt_mlgraph
     )
 
 # %% ../nbs/40_duck.ipynb 175
-class datatype(Duck): 
+class datatype(Duck, Generic[*Ts]):
     '''data type (e.g.  `np.array`, `np.matrix`, `sp.array`, `sp.matrix`,  `np.recarray`, or `anndata`)'''
     __ducktype__ = (array, matrix, adata, )
 
 
 # %% ../nbs/40_duck.ipynb 177
 class nnum(nums, nlen[*Ts]):
     @classmethod
```

### Comparing `quac-0.0.8/quac/eggs.py` & `quac-0.0.9/quac/eggs.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/enum.py` & `quac-0.0.9/quac/enum.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/errs.py` & `quac-0.0.9/quac/errs.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/grds.py` & `quac-0.0.9/quac/grds.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/meta.py` & `quac-0.0.9/quac/meta.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/misc.py` & `quac-0.0.9/quac/misc.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/mods.py` & `quac-0.0.9/quac/mods.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/prot.py` & `quac-0.0.9/quac/prot.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/solo.py` & `quac-0.0.9/quac/solo.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/spec.py` & `quac-0.0.9/quac/spec.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac/type.py` & `quac-0.0.9/quac/type.py`

 * *Files identical despite different names*

### Comparing `quac-0.0.8/quac.egg-info/PKG-INFO` & `quac-0.0.9/quac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quac
-Version: 0.0.8
+Version: 0.0.9
 Summary: quac
 Home-page: https://github.com/dsm-72/quac
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: quac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `quac-0.0.8/settings.ini` & `quac-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = quac
 lib_name = quac
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = quac
 nbs_path = nbs
 recursive = True
```

### Comparing `quac-0.0.8/setup.py` & `quac-0.0.9/setup.py`

 * *Files identical despite different names*

