# Comparing `tmp/linien-client-1.0.1rc1.tar.gz` & `tmp/linien-client-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-client-1.0.1rc1.tar", last modified: Fri Dec 22 14:16:41 2023, max compression
+gzip compressed data, was "linien-client-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:41 2024, max compression
```

## Comparing `linien-client-1.0.1rc1.tar` & `linien-client-1.0.2rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:41.043892 linien-client-1.0.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-12-22 14:16:41.043892 linien-client-1.0.1rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:41.043892 linien-client-1.0.1rc1/linien_client/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/linien_client/remote_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:41.043892 linien-client-1.0.1rc1/linien_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-12-22 14:16:41.000000 linien-client-1.0.1rc1/linien_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-22 14:16:41.000000 linien-client-1.0.1rc1/linien_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 14:16:41.000000 linien-client-1.0.1rc1/linien_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-22 14:16:41.000000 linien-client-1.0.1rc1/linien_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 14:16:41.000000 linien-client-1.0.1rc1/linien_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 14:16:41.043892 linien-client-1.0.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-12-22 14:16:05.000000 linien-client-1.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.523799 linien-client-1.0.2rc1/linien_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/linien_client/remote_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/linien_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:41.000000 linien-client-1.0.2rc1/linien_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:41.527799 linien-client-1.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-05 08:31:26.000000 linien-client-1.0.2rc1/setup.py
```

### Comparing `linien-client-1.0.1rc1/PKG-INFO` & `linien-client-1.0.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fabric>=2.7.0
 Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: linien-common==1.0.1rc1
+Requires-Dist: linien-common==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-client-1.0.1rc1/linien_client/__init__.py` & `linien-client-1.0.2rc1/linien_client/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client/communication.py` & `linien-client-1.0.2rc1/linien_client/communication.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client/connection.py` & `linien-client-1.0.2rc1/linien_client/connection.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client/deploy.py` & `linien-client-1.0.2rc1/linien_client/deploy.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client/exceptions.py` & `linien-client-1.0.2rc1/linien_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client/remote_parameters.py` & `linien-client-1.0.2rc1/linien_client/remote_parameters.py`

 * *Files identical despite different names*

### Comparing `linien-client-1.0.1rc1/linien_client.egg-info/PKG-INFO` & `linien-client-1.0.2rc1/linien_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: linien-client
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Client components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien/
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fabric>=2.7.0
 Requires-Dist: typing_extensions>=4.5.0
-Requires-Dist: linien-common==1.0.1rc1
+Requires-Dist: linien-common==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-client-1.0.1rc1/setup.py` & `linien-client-1.0.2rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "1.0.1rc1"
+version = "1.0.2rc1"
 
 setup(
     name="linien-client",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -37,10 +37,10 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=[
         "fabric>=2.7.0",
         "typing_extensions>=4.5.0",
-        "linien-common==1.0.1rc1",
+        "linien-common==1.0.2rc1",
     ],
 )
```

