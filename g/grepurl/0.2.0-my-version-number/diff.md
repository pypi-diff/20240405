# Comparing `tmp/grepurl-0.2.0.tar.gz` & `tmp/grepurl-my-version-number.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grepurl-0.2.0.tar", last modified: Fri Apr  5 13:10:50 2024, max compression
+gzip compressed data, was "dist/grepurl-my-version-number.tar", last modified: Thu Aug 21 15:09:27 2014, max compression
```

## Comparing `grepurl-0.2.0.tar` & `grepurl-my-version-number.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2024-04-05 13:10:50.000000 grepurl-0.2.0/
--rw-rw-r--   0 arne      (1000) arne      (1000)      643 2024-04-05 13:05:25.000000 grepurl-0.2.0/setup.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1248 2024-04-05 13:05:25.000000 grepurl-0.2.0/README.rst
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/
--rw-rw-r--   0 arne      (1000) arne      (1000)      218 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/SOURCES.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)        1 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/dependency_links.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)     1513 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/PKG-INFO
--rw-rw-r--   0 arne      (1000) arne      (1000)       24 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/requires.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)        8 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/top_level.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)       42 2024-04-05 13:10:50.000000 grepurl-0.2.0/grepurl.egg-info/entry_points.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)     1513 2024-04-05 13:10:50.000000 grepurl-0.2.0/PKG-INFO
--rw-rw-r--   0 arne      (1000) arne      (1000)     4754 2024-04-05 13:05:25.000000 grepurl-0.2.0/grepurl.py
--rw-rw-r--   0 arne      (1000) arne      (1000)       38 2024-04-05 13:10:50.000000 grepurl-0.2.0/setup.cfg
+drwxr-xr-x   0 arne      (1000) arne      (1000)        0 2014-08-21 15:09:27.000000 grepurl-my-version-number/
+-rwxr-xr-x   0 arne      (1000) arne      (1000)     7061 2014-08-21 14:40:15.000000 grepurl-my-version-number/grepurl.py
+drwxr-xr-x   0 arne      (1000) arne      (1000)        0 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/
+-rw-r--r--   0 arne      (1000) arne      (1000)        8 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/top_level.txt
+-rw-r--r--   0 arne      (1000) arne      (1000)      188 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/SOURCES.txt
+-rw-r--r--   0 arne      (1000) arne      (1000)        1 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/dependency_links.txt
+-rw-r--r--   0 arne      (1000) arne      (1000)       42 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/entry_points.txt
+-rw-r--r--   0 arne      (1000) arne      (1000)     1230 2014-08-21 15:09:27.000000 grepurl-my-version-number/grepurl.egg-info/PKG-INFO
+-rw-r--r--   0 arne      (1000) arne      (1000)      660 2014-08-21 14:56:21.000000 grepurl-my-version-number/setup.py
+-rw-r--r--   0 arne      (1000) arne      (1000)       59 2014-08-21 15:09:27.000000 grepurl-my-version-number/setup.cfg
+-rw-r--r--   0 arne      (1000) arne      (1000)     1230 2014-08-21 15:09:27.000000 grepurl-my-version-number/PKG-INFO
+-rw-r--r--   0 arne      (1000) arne      (1000)      747 2014-08-21 14:54:16.000000 grepurl-my-version-number/README.rst
```

### Comparing `grepurl-0.2.0/README.rst` & `grepurl-my-version-number/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -5,47 +5,26 @@
 local HTML file).
 
 Usage
 -----
 
 ::
 
-    grepurl http://example.com/ # extract all URLs from links and images
+    grepurl http://example.com/
     grepurl -a http://example.com/foo.htm # only extract from <a> tags (i.e. links)
     grepurl -i http://example.com/bar.htm # only extract from <img> tags (i.e. images)
     grepurl -r "\.py$" http://example.com/ # only extract links that end in '.py'
-    grepurl -r "\.zip$" -d http://example.com/ # download all zip files
-    grepurl -r "\.zip$" -d -o download_dir http://example.com/ # download all zip files into download_dir
-
-Installation using pip
-----------------------
-
-::
-
-    pip install grepurl
-
-Installation from repository
-----------------------------
-
-::
-
-    git clone https://github.com/arne-cl/grepurl
-    cd grepurl
-    pip install -e .
 
 License
 -------
 
 GPLv2 or later.
 
 
 Authors
 -------
 
 Gerome Fournier (original author). His implementation is only available via the
 `Internet Archive`_.
-
 Arne Neumann (added -l option for local files, minor changes).
 
-GPT-4 (rewrote the script for Python 3 compatibility).
-
 .. _`Internet Archive`: http://web.archive.org/web/20101116071317/http://jefke.free.fr/stuff/python/grepurl/grepurl
```

