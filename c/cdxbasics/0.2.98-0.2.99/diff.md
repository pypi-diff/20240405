# Comparing `tmp/cdxbasics-0.2.98.tar.gz` & `tmp/cdxbasics-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdxbasics-0.2.98.tar", last modified: Fri Dec 15 21:57:49 2023, max compression
+gzip compressed data, was "cdxbasics-0.2.99.tar", last modified: Tue Dec 19 17:21:02 2023, max compression
```

## Comparing `cdxbasics-0.2.98.tar` & `cdxbasics-0.2.99.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 21:57:49.615590 cdxbasics-0.2.98/
--rw-rw-rw-   0        0        0     1090 2023-05-13 09:41:57.000000 cdxbasics-0.2.98/LICENSE
--rw-rw-rw-   0        0        0    54356 2023-12-15 21:57:49.614593 cdxbasics-0.2.98/PKG-INFO
--rw-rw-rw-   0        0        0    53919 2023-12-14 23:58:43.000000 cdxbasics-0.2.98/README.md
-drwxrwxrwx   0        0        0        0 2023-12-15 21:57:49.566855 cdxbasics-0.2.98/cdxbasics/
--rw-rw-rw-   0        0        0      236 2023-12-15 21:57:46.000000 cdxbasics-0.2.98/cdxbasics/__init__.py
--rw-rw-rw-   0        0        0    20489 2023-07-16 20:05:04.000000 cdxbasics-0.2.98/cdxbasics/cached.py
--rw-rw-rw-   0        0        0    58519 2023-08-28 07:50:11.000000 cdxbasics-0.2.98/cdxbasics/config.py
--rw-rw-rw-   0        0        0     3164 2023-12-12 23:35:04.000000 cdxbasics-0.2.98/cdxbasics/crman.py
--rw-rw-rw-   0        0        0     9239 2023-11-04 10:35:27.000000 cdxbasics-0.2.98/cdxbasics/deferred.py
--rw-rw-rw-   0        0        0    22997 2023-12-09 14:43:36.000000 cdxbasics-0.2.98/cdxbasics/dynaplot.py
--rw-rw-rw-   0        0        0     4353 2022-07-02 07:27:54.000000 cdxbasics-0.2.98/cdxbasics/kwargs.py
--rw-rw-rw-   0        0        0    11272 2023-01-02 20:03:55.000000 cdxbasics-0.2.98/cdxbasics/logger.py
--rw-rw-rw-   0        0        0    20469 2023-10-24 20:08:24.000000 cdxbasics-0.2.98/cdxbasics/np.py
--rw-rw-rw-   0        0        0    14192 2023-12-09 14:43:36.000000 cdxbasics-0.2.98/cdxbasics/npio.py
--rw-rw-rw-   0        0        0     6147 2023-01-02 23:00:09.000000 cdxbasics-0.2.98/cdxbasics/prettydict.py
--rw-rw-rw-   0        0        0    11484 2023-12-09 14:43:36.000000 cdxbasics-0.2.98/cdxbasics/sharedarray.py
--rw-rw-rw-   0        0        0    74694 2023-12-12 23:35:04.000000 cdxbasics-0.2.98/cdxbasics/subdir.py
--rw-rw-rw-   0        0        0    33322 2023-10-08 23:40:03.000000 cdxbasics-0.2.98/cdxbasics/util.py
--rw-rw-rw-   0        0        0    11811 2023-12-15 21:57:05.000000 cdxbasics-0.2.98/cdxbasics/verbose.py
--rw-rw-rw-   0        0        0    14619 2023-08-19 00:17:32.000000 cdxbasics-0.2.98/cdxbasics/version.py
-drwxrwxrwx   0        0        0        0 2023-12-15 21:57:49.611592 cdxbasics-0.2.98/cdxbasics.egg-info/
--rw-rw-rw-   0        0        0    54356 2023-12-15 21:57:48.000000 cdxbasics-0.2.98/cdxbasics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-12-15 21:57:49.000000 cdxbasics-0.2.98/cdxbasics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 21:57:48.000000 cdxbasics-0.2.98/cdxbasics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-12-15 21:57:48.000000 cdxbasics-0.2.98/cdxbasics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-15 21:57:48.000000 cdxbasics-0.2.98/cdxbasics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-15 21:57:49.616590 cdxbasics-0.2.98/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-12-15 21:57:46.000000 cdxbasics-0.2.98/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-19 17:21:02.619578 cdxbasics-0.2.99/
+-rw-rw-rw-   0        0        0     1090 2023-05-13 09:41:57.000000 cdxbasics-0.2.99/LICENSE
+-rw-rw-rw-   0        0        0    54356 2023-12-19 17:21:02.617582 cdxbasics-0.2.99/PKG-INFO
+-rw-rw-rw-   0        0        0    53919 2023-12-14 23:58:43.000000 cdxbasics-0.2.99/README.md
+drwxrwxrwx   0        0        0        0 2023-12-19 17:21:02.556121 cdxbasics-0.2.99/cdxbasics/
+-rw-rw-rw-   0        0        0      236 2023-12-19 17:20:58.000000 cdxbasics-0.2.99/cdxbasics/__init__.py
+-rw-rw-rw-   0        0        0    20489 2023-07-16 20:05:04.000000 cdxbasics-0.2.99/cdxbasics/cached.py
+-rw-rw-rw-   0        0        0    58519 2023-08-28 07:50:11.000000 cdxbasics-0.2.99/cdxbasics/config.py
+-rw-rw-rw-   0        0        0     3182 2023-12-19 17:20:38.000000 cdxbasics-0.2.99/cdxbasics/crman.py
+-rw-rw-rw-   0        0        0     9239 2023-11-04 10:35:27.000000 cdxbasics-0.2.99/cdxbasics/deferred.py
+-rw-rw-rw-   0        0        0    22997 2023-12-09 14:43:36.000000 cdxbasics-0.2.99/cdxbasics/dynaplot.py
+-rw-rw-rw-   0        0        0    10621 2023-12-19 17:20:38.000000 cdxbasics-0.2.99/cdxbasics/filelock.py
+-rw-rw-rw-   0        0        0     4353 2022-07-02 07:27:54.000000 cdxbasics-0.2.99/cdxbasics/kwargs.py
+-rw-rw-rw-   0        0        0    11272 2023-01-02 20:03:55.000000 cdxbasics-0.2.99/cdxbasics/logger.py
+-rw-rw-rw-   0        0        0    20480 2023-12-19 17:20:38.000000 cdxbasics-0.2.99/cdxbasics/np.py
+-rw-rw-rw-   0        0        0    14192 2023-12-09 14:43:36.000000 cdxbasics-0.2.99/cdxbasics/npio.py
+-rw-rw-rw-   0        0        0     6147 2023-01-02 23:00:09.000000 cdxbasics-0.2.99/cdxbasics/prettydict.py
+-rw-rw-rw-   0        0        0    11484 2023-12-09 14:43:36.000000 cdxbasics-0.2.99/cdxbasics/sharedarray.py
+-rw-rw-rw-   0        0        0    75408 2023-12-19 17:20:38.000000 cdxbasics-0.2.99/cdxbasics/subdir.py
+-rw-rw-rw-   0        0        0    33322 2023-10-08 23:40:03.000000 cdxbasics-0.2.99/cdxbasics/util.py
+-rw-rw-rw-   0        0        0    11811 2023-12-15 21:57:05.000000 cdxbasics-0.2.99/cdxbasics/verbose.py
+-rw-rw-rw-   0        0        0    14619 2023-08-19 00:17:32.000000 cdxbasics-0.2.99/cdxbasics/version.py
+drwxrwxrwx   0        0        0        0 2023-12-19 17:21:02.614576 cdxbasics-0.2.99/cdxbasics.egg-info/
+-rw-rw-rw-   0        0        0    54356 2023-12-19 17:21:01.000000 cdxbasics-0.2.99/cdxbasics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-12-19 17:21:02.000000 cdxbasics-0.2.99/cdxbasics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-19 17:21:01.000000 cdxbasics-0.2.99/cdxbasics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-12-19 17:21:01.000000 cdxbasics-0.2.99/cdxbasics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-12-19 17:21:01.000000 cdxbasics-0.2.99/cdxbasics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-19 17:21:02.619578 cdxbasics-0.2.99/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-12-19 17:20:58.000000 cdxbasics-0.2.99/setup.py
```

### Comparing `cdxbasics-0.2.98/LICENSE` & `cdxbasics-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/PKG-INFO` & `cdxbasics-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdxbasics
-Version: 0.2.98
+Version: 0.2.99
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdxbasics
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdxbasics-0.2.98/README.md` & `cdxbasics-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/cached.py` & `cdxbasics-0.2.99/cdxbasics/cached.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/config.py` & `cdxbasics-0.2.99/cdxbasics/config.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/crman.py` & `cdxbasics-0.2.99/cdxbasics/crman.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         line   = lines[0]
         icr    = line.rfind('\r')
         if icr == -1:
             line = self._current + line
         else:
             line = line[icr+1:]
         if len(self._current) > 0:
-            output    += '\r' + ' '*len(self._current) + '\r'
+            output    += '\r' + ' '*len(self._current) + '\r' + '\33[2K' + '\r'
         output        += line
         self._current = line
             
         if len(lines) > 1:
             output       += '\n'
             self._current = ""
```

### Comparing `cdxbasics-0.2.98/cdxbasics/deferred.py` & `cdxbasics-0.2.99/cdxbasics/deferred.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/dynaplot.py` & `cdxbasics-0.2.99/cdxbasics/dynaplot.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/kwargs.py` & `cdxbasics-0.2.99/cdxbasics/kwargs.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/logger.py` & `cdxbasics-0.2.99/cdxbasics/logger.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/np.py` & `cdxbasics-0.2.99/cdxbasics/np.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,20 +354,20 @@
         stds  = np.asarray( np.std( x[ixs[i]:ixs[i+1]], axis=axis) for i in range(len(ixs)-1))
     else:
         means = np.asarray( mean( P[ixs[i]:ixs[i+1]], x[ixs[i]:ixs[i+1]], axis=axis) for i in range(len(ixs)-1))
         stds  = np.asarray( std( P[ixs[i]:ixs[i+1]], x[ixs[i]:ixs[i+1]], axis=axis) for i in range(len(ixs)-1))
     return means, stds
 
 def np_european(   *,
-                   ttm : np.ndarray,
+                   ttm  : np.ndarray,
                    vols : np.ndarray,
-                   K : np.ndarray,
-                   cp : np.ndarray,
-                   DF : np.ndarray = 1.,
-                   F : np.ndarray = 1., 
+                   K    : np.ndarray,
+                   cp   : np.ndarray,
+                   DF   : np.ndarray = 1.,
+                   F    : np.ndarray = 1., 
                    price_only : bool = False) -> dict:
     """
     European option pricer
     Returns a dictionary with (price,fdelta,fgamma,vega,ftheta,frhoDF)
     
     Note that greeks are computed with respect to the input parameters, e.g.
         fdelta, fgamma are greeks with respect to F
@@ -461,15 +461,15 @@
     r         = - np.log( DF ) / ttm
     d1        = ( e + r * ttm + 0.5 * vols * vols * ttm  ) / ( vols*sqrtTTM )
     d2        = ( e + r * ttm - 0.5 * vols * vols * ttm  ) / ( vols*sqrtTTM )
     N1        = norm.cdf( d1 )
     N2        = norm.cdf( d2 )
     n1        = norm.pdf( d1 )
     cp0       = 0.5 * (1. - cp)   # 0 for call 1 for put
-    price     = DF * ( F * N1 - K * N2 + cp0 * ( K - F ) )
+    price     = DF * ( F * N1 - K * N2 + cp0 * ( F - K ) )
     assert not np.any(~np.isfinite(price)), ("Error computing European prices: NaN's returned:", price)
     fdelta    = DF * ( N1 - cp0 )
     vega      = DF * F * n1 * sqrtTTM
     fgamma    = DF * n1 / ( F * vols * sqrtTTM )
     dfrho     = price / DF
     voltheta  = - 0.5 * fgamma * F * F * vols * vols * ttm
```

### Comparing `cdxbasics-0.2.98/cdxbasics/npio.py` & `cdxbasics-0.2.99/cdxbasics/npio.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/prettydict.py` & `cdxbasics-0.2.99/cdxbasics/prettydict.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/sharedarray.py` & `cdxbasics-0.2.99/cdxbasics/sharedarray.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/subdir.py` & `cdxbasics-0.2.99/cdxbasics/subdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,32 @@
                 os.makedirs( self._path[:-1] )
             else:
                 if not os.path.isdir(self._path[:-1]): _log.throw( "Cannot use sub directory %s: object exists but is not a directory", self._path[:-1] )
                 # erase all content if requested
                 if eraseEverything:
                     self.eraseEverything(keepDirectory = True)
 
+    @staticmethod
+    def expandStandardRoot( name ):
+        """
+        Expands 'name' by a standardized root directory if provided:
+        If 'name' starts with -> return
+            ! -> tempDir()
+            . -> workingDir()
+            ~ -> userDir()
+        """        
+        if len(name) < 2 or name[0] not in ['.','!','~'] or name[1] not in ["\\","/"]:
+            return name
+        if name[0] == '!':
+            return SubDir.tempDir() + name[2:]
+        elif name[0] == ".":
+            return SubDir.workingDir() + name[2:]
+        else:
+            return SubDir.userDir() + name[2:]
+
     # -- self description --
 
     def __str__(self) -> str: # NOQA
         if self._path is None: return "(none)"
         return self._path if len(self._ext) == 0 else self._path + ";*" + self._ext
 
     def __repr__(self) -> str: # NOQA
@@ -441,17 +459,17 @@
         _log.verify( len(sub) == 0, "Extension '%s' contains directory information", ext)
 
         # remove internal characters
         _log.verify( ext[0] != "!", "Extension '%s' cannot start with '!' (this symbol indicates the temp directory)", ext)
         _log.verify( ext[0] != "~", "Extension '%s' cannot start with '~' (this symbol indicates the user's directory)", ext)
         return "." + ext
 
-    def fullKeyName(self, key : str, *, ext : str = None) -> str:
+    def fullFileName(self, key : str, *, ext : str = None) -> str:
         """
-        Returns fully qualified key name.
+        Returns fully qualified file name.
         The function tests that 'key' does not contain directory information.
 
         If 'self' is None, then this function returns None
         If key is None then this function returns None
 
         Parameters
         ----------
@@ -459,14 +477,16 @@
                 Core file name, e.g. the 'key' in a data base sense
             ext : str
                 If not None, use this extension rather than self.ext
 
         Returns
         -------
             Fully qualified system file name
+        
+        [This function has an alias 'fullKeyName' for backward compatibility]
         """
         if self._path is None or key is None:
             return None
         key = str(key)
         _log.verify( len(key) > 0, "'key' cannot be empty")
 
         sub, _ = os.path.split(key)
@@ -475,15 +495,15 @@
         _log.verify( key[0] != "!", "Key '%s' cannot start with '!' (this symbol indicates the temp directory)", key)
         _log.verify( key[0] != "~", "Key '%s' cannot start with '~' (this symbol indicates the user's directory)", key)
 
         ext = self._convert_ext( ext if not ext is None else self._ext )
         if len(ext) > 0 and key[-len(ext):] != ext:
             return self._path + key + ext
         return self._path + key
-    fullFileName = fullKeyName
+    fullKeyName = fullFileName
 
     @staticmethod
     def tempDir() -> str:
         """
         Return system temp directory. Short cut to tempfile.gettempdir()
         Result contains trailing '/'
         """
```

### Comparing `cdxbasics-0.2.98/cdxbasics/util.py` & `cdxbasics-0.2.99/cdxbasics/util.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/verbose.py` & `cdxbasics-0.2.99/cdxbasics/verbose.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics/version.py` & `cdxbasics-0.2.99/cdxbasics/version.py`

 * *Files identical despite different names*

### Comparing `cdxbasics-0.2.98/cdxbasics.egg-info/PKG-INFO` & `cdxbasics-0.2.99/cdxbasics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdxbasics
-Version: 0.2.98
+Version: 0.2.99
 Summary: Basic Python tools
 Home-page: https://github.com/hansbuehler/cdxbasics
 Author: Hans Buehler
 Author-email: github@buehler.london
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdxbasics-0.2.98/cdxbasics.egg-info/SOURCES.txt` & `cdxbasics-0.2.99/cdxbasics.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 cdxbasics/__init__.py
 cdxbasics/cached.py
 cdxbasics/config.py
 cdxbasics/crman.py
 cdxbasics/deferred.py
 cdxbasics/dynaplot.py
+cdxbasics/filelock.py
 cdxbasics/kwargs.py
 cdxbasics/logger.py
 cdxbasics/np.py
 cdxbasics/npio.py
 cdxbasics/prettydict.py
 cdxbasics/sharedarray.py
 cdxbasics/subdir.py
```

### Comparing `cdxbasics-0.2.98/setup.py` & `cdxbasics-0.2.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdxbasics",
-    version="0.2.98",  # will auto-update via pip_modify_setup.py
+    version="0.2.99",  # will auto-update via pip_modify_setup.py
     author="Hans Buehler",
     author_email="github@buehler.london",
     description="Basic Python tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hansbuehler/cdxbasics",
     packages=setuptools.find_packages(),
```

