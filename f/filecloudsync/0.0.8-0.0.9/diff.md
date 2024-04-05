# Comparing `tmp/filecloudsync-0.0.8.tar.gz` & `tmp/filecloudsync-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filecloudsync-0.0.8.tar", last modified: Fri Mar  1 10:54:21 2024, max compression
+gzip compressed data, was "filecloudsync-0.0.9.tar", last modified: Fri Mar  1 11:03:22 2024, max compression
```

## Comparing `filecloudsync-0.0.8.tar` & `filecloudsync-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 10:54:21.656093 filecloudsync-0.0.8/
--rw-rw-rw-   0        0        0    35823 2024-02-16 14:18:24.000000 filecloudsync-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     6051 2024-03-01 10:54:21.655094 filecloudsync-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5461 2024-03-01 10:53:55.000000 filecloudsync-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-01 10:54:21.640087 filecloudsync-0.0.8/filecloudsync/
--rw-rw-rw-   0        0        0        0 2024-02-22 14:21:41.000000 filecloudsync-0.0.8/filecloudsync/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-02-22 14:21:41.000000 filecloudsync-0.0.8/filecloudsync/file.py
-drwxrwxrwx   0        0        0        0 2024-03-01 10:54:21.651094 filecloudsync-0.0.8/filecloudsync/s3/
--rw-rw-rw-   0        0        0      269 2024-02-22 14:57:51.000000 filecloudsync-0.0.8/filecloudsync/s3/__init__.py
--rw-rw-rw-   0        0        0    31288 2024-02-27 13:59:45.000000 filecloudsync-0.0.8/filecloudsync/s3/core.py
--rw-rw-rw-   0        0        0      197 2024-02-22 14:21:41.000000 filecloudsync-0.0.8/filecloudsync/s3/exceptions.py
--rw-rw-rw-   0        0        0     5022 2024-03-01 10:28:41.000000 filecloudsync-0.0.8/filecloudsync/s3/monitor.py
-drwxrwxrwx   0        0        0        0 2024-03-01 10:54:21.646089 filecloudsync-0.0.8/filecloudsync.egg-info/
--rw-rw-rw-   0        0        0     6051 2024-03-01 10:54:21.000000 filecloudsync-0.0.8/filecloudsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-03-01 10:54:21.000000 filecloudsync-0.0.8/filecloudsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 10:54:21.000000 filecloudsync-0.0.8/filecloudsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-01 10:54:21.000000 filecloudsync-0.0.8/filecloudsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-01 10:54:21.656093 filecloudsync-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1545 2024-03-01 10:05:55.000000 filecloudsync-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-01 10:54:21.653094 filecloudsync-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 14:42:11.000000 filecloudsync-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0    24176 2024-03-01 10:41:09.000000 filecloudsync-0.0.8/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2024-03-01 11:03:22.291836 filecloudsync-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2024-02-16 14:18:24.000000 filecloudsync-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6051 2024-03-01 11:03:22.290836 filecloudsync-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5461 2024-03-01 10:53:55.000000 filecloudsync-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-01 11:03:22.276837 filecloudsync-0.0.9/filecloudsync/
+-rw-rw-rw-   0        0        0        0 2024-02-22 14:21:41.000000 filecloudsync-0.0.9/filecloudsync/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-02-22 14:21:41.000000 filecloudsync-0.0.9/filecloudsync/file.py
+drwxrwxrwx   0        0        0        0 2024-03-01 11:03:22.286836 filecloudsync-0.0.9/filecloudsync/s3/
+-rw-rw-rw-   0        0        0      269 2024-02-22 14:57:51.000000 filecloudsync-0.0.9/filecloudsync/s3/__init__.py
+-rw-rw-rw-   0        0        0    31288 2024-02-27 13:59:45.000000 filecloudsync-0.0.9/filecloudsync/s3/core.py
+-rw-rw-rw-   0        0        0      197 2024-02-22 14:21:41.000000 filecloudsync-0.0.9/filecloudsync/s3/exceptions.py
+-rw-rw-rw-   0        0        0     5042 2024-03-01 11:02:45.000000 filecloudsync-0.0.9/filecloudsync/s3/monitor.py
+drwxrwxrwx   0        0        0        0 2024-03-01 11:03:22.282836 filecloudsync-0.0.9/filecloudsync.egg-info/
+-rw-rw-rw-   0        0        0     6051 2024-03-01 11:03:22.000000 filecloudsync-0.0.9/filecloudsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-03-01 11:03:22.000000 filecloudsync-0.0.9/filecloudsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-01 11:03:22.000000 filecloudsync-0.0.9/filecloudsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-03-01 11:03:22.000000 filecloudsync-0.0.9/filecloudsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-01 11:03:22.291836 filecloudsync-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1545 2024-03-01 11:02:45.000000 filecloudsync-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-01 11:03:22.288836 filecloudsync-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 14:42:11.000000 filecloudsync-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0    24176 2024-03-01 10:41:09.000000 filecloudsync-0.0.9/tests/test_sync.py
```

### Comparing `filecloudsync-0.0.8/LICENSE` & `filecloudsync-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `filecloudsync-0.0.8/PKG-INFO` & `filecloudsync-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filecloudsync
-Version: 0.0.8
+Version: 0.0.9
 Summary: A method to synchronize files from several file cloud systems. At the moment, only S3 is implemented. Any help is welcome.
 Home-page: https://github.com/jmgomezsoriano/filecloudsync
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: GPL v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filecloudsync-0.0.8/README.md` & `filecloudsync-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `filecloudsync-0.0.8/filecloudsync/file.py` & `filecloudsync-0.0.9/filecloudsync/file.py`

 * *Files identical despite different names*

### Comparing `filecloudsync-0.0.8/filecloudsync/s3/core.py` & `filecloudsync-0.0.9/filecloudsync/s3/core.py`

 * *Files identical despite different names*

### Comparing `filecloudsync-0.0.8/filecloudsync/s3/monitor.py` & `filecloudsync-0.0.9/filecloudsync/s3/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     def stop(self):
         """ Stops the monitor """
         self._stop_event = True
         self._interrupt_event.set()
         self.join()
         if self.remove:
             s3.remove_sync_status(self._client.meta.endpoint_url, self.bucket, self.folder)
-            rmtree(self.folder)
+            rmtree(self.folder, ignore_errors=True)
 
     def join(self, timeout: int = None):
         """ Wait until the thread finishes or the timeout is reached """
         self._interrupt_event.set()
         super().join(timeout)
 
     def __enter__(self):
```

### Comparing `filecloudsync-0.0.8/filecloudsync.egg-info/PKG-INFO` & `filecloudsync-0.0.9/filecloudsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filecloudsync
-Version: 0.0.8
+Version: 0.0.9
 Summary: A method to synchronize files from several file cloud systems. At the moment, only S3 is implemented. Any help is welcome.
 Home-page: https://github.com/jmgomezsoriano/filecloudsync
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: GPL v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filecloudsync-0.0.8/setup.py` & `filecloudsync-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         for file in glob.glob('*.egg-info'):
             rmtree(file)
 
 
 setuptools.setup(
     cmdclass={'clean': CleanCommand},
     name='filecloudsync',
-    version='0.0.8',
+    version='0.0.9',
     url='https://github.com/jmgomezsoriano/filecloudsync',
     license='GPL v3',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='A method to synchronize files from several file cloud systems. '
```

### Comparing `filecloudsync-0.0.8/tests/test_sync.py` & `filecloudsync-0.0.9/tests/test_sync.py`

 * *Files identical despite different names*

