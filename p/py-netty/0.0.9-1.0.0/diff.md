# Comparing `tmp/py-netty-0.0.9.tar.gz` & `tmp/py-netty-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-netty-0.0.9.tar", last modified: Sun Sep 17 14:37:39 2023, max compression
+gzip compressed data, was "py-netty-1.0.0.tar", last modified: Fri Apr  5 02:09:41 2024, max compression
```

## Comparing `py-netty-0.0.9.tar` & `py-netty-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-17 14:37:39.528954 py-netty-0.0.9/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-09-15 14:42:10.000000 py-netty-0.0.9/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)     3659 2023-09-17 14:37:39.528747 py-netty-0.0.9/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)     2704 2023-09-16 15:05:54.000000 py-netty-0.0.9/README.md
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-17 14:37:39.525970 py-netty-0.0.9/py_netty/
--rw-r--r--   0 haoru      (501) staff       (20)      218 2023-09-16 10:11:43.000000 py-netty-0.0.9/py_netty/__init__.py
--rw-r--r--   0 haoru      (501) staff       (20)     2352 2023-09-17 14:10:50.000000 py-netty-0.0.9/py_netty/bootstrap.py
--rw-r--r--   0 haoru      (501) staff       (20)      434 2023-09-17 13:18:00.000000 py-netty-0.0.9/py_netty/bytebuf.py
--rw-r--r--   0 haoru      (501) staff       (20)     7064 2023-09-17 14:23:23.000000 py-netty-0.0.9/py_netty/channel.py
--rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-16 01:26:45.000000 py-netty-0.0.9/py_netty/eventfd.py
--rw-r--r--   0 haoru      (501) staff       (20)    11046 2023-09-17 14:31:29.000000 py-netty-0.0.9/py_netty/eventloop.py
--rw-r--r--   0 haoru      (501) staff       (20)     1334 2023-09-16 13:57:40.000000 py-netty-0.0.9/py_netty/handler.py
--rw-r--r--   0 haoru      (501) staff       (20)     3455 2023-09-16 04:00:09.000000 py-netty-0.0.9/py_netty/utils.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2023-09-17 14:37:39.528063 py-netty-0.0.9/py_netty.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     3659 2023-09-17 14:37:39.000000 py-netty-0.0.9/py_netty.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      327 2023-09-17 14:37:39.000000 py-netty-0.0.9/py_netty.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2023-09-17 14:37:39.000000 py-netty-0.0.9/py_netty.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)        9 2023-09-17 14:37:39.000000 py-netty-0.0.9/py_netty.egg-info/top_level.txt
--rw-r--r--   0 haoru      (501) staff       (20)      157 2023-09-17 14:37:39.529690 py-netty-0.0.9/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1576 2023-09-17 14:37:32.000000 py-netty-0.0.9/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.393479 py-netty-1.0.0/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-09-15 14:42:10.000000 py-netty-1.0.0/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-04-05 02:09:41.392754 py-netty-1.0.0/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)     7757 2024-02-07 07:00:46.000000 py-netty-1.0.0/README.md
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.388625 py-netty-1.0.0/py_netty/
+-rw-r--r--   0 haoru      (501) staff       (20)      218 2024-02-02 09:16:04.000000 py-netty-1.0.0/py_netty/__init__.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3758 2024-03-25 01:49:53.000000 py-netty-1.0.0/py_netty/bootstrap.py
+-rw-r--r--   0 haoru      (501) staff       (20)      487 2024-02-18 05:21:21.000000 py-netty-1.0.0/py_netty/bytebuf.py
+-rw-r--r--   0 haoru      (501) staff       (20)    16684 2024-03-24 15:54:43.000000 py-netty-1.0.0/py_netty/channel.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-16 01:26:45.000000 py-netty-1.0.0/py_netty/eventfd.py
+-rw-r--r--   0 haoru      (501) staff       (20)    15905 2024-03-25 01:53:25.000000 py-netty-1.0.0/py_netty/eventloop.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3138 2023-09-22 05:47:29.000000 py-netty-1.0.0/py_netty/handler.py
+-rw-r--r--   0 haoru      (501) staff       (20)     1922 2024-02-07 06:26:51.000000 py-netty-1.0.0/py_netty/utils.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.392117 py-netty-1.0.0/py_netty.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      358 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        6 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        9 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/top_level.txt
+-rw-r--r--   0 haoru      (501) staff       (20)      186 2024-04-05 02:09:41.394118 py-netty-1.0.0/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1524 2024-04-05 02:08:40.000000 py-netty-1.0.0/setup.py
```

### Comparing `py-netty-0.0.9/LICENSE` & `py-netty-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-netty-0.0.9/py_netty/eventfd.py` & `py-netty-1.0.0/py_netty/eventfd.py`

 * *Files identical despite different names*

### Comparing `py-netty-0.0.9/setup.py` & `py-netty-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,34 +2,29 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # install_requires = (this_directory / 'requirements.txt').read_text().splitlines()
 
-
-epoch = 9
-
-major = int(epoch / 100 / 100)
-minor = int(epoch / 100 % 100)
-micro = int(epoch % 100)
+version = '1.0.0'
 
 config = {
     'name': 'py-netty',
     'url': 'https://github.com/ruanhao/py-netty',
     'license': 'MIT',
     "long_description": long_description,
     "long_description_content_type": 'text/markdown',
     'description': 'TCP framework in flavor of Netty',
     'author' : 'Hao Ruan',
     'author_email': 'ruanhao1116@gmail.com',
-    'keywords': ['network', 'tcp'],
-    'version': f'{major}.{minor}.{micro}',
+    'keywords': ['network', 'tcp', 'non-blocking', 'epoll', 'nio', 'netty'],
+    'version': version,
     'packages': find_packages(),
-    'install_requires': [],
+    'install_requires': ['attrs'],
     'python_requires': ">=3.7, <4",
     'setup_requires': ['wheel'],
     'classifiers': [
         "Intended Audience :: Developers",
         'License :: OSI Approved :: MIT License',
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

