# Comparing `tmp/linien-common-1.0.1rc1.tar.gz` & `tmp/linien-common-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-1.0.1rc1.tar", last modified: Fri Dec 22 14:16:16 2023, max compression
+gzip compressed data, was "linien-common-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:32 2024, max compression
```

## Comparing `linien-common-1.0.1rc1.tar` & `linien-common-1.0.2rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:16.971896 linien-common-1.0.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-22 14:16:16.967896 linien-common-1.0.1rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:16.967896 linien-common-1.0.1rc1/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:16:16.967896 linien-common-1.0.1rc1/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-12-22 14:16:16.000000 linien-common-1.0.1rc1/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-22 14:16:16.000000 linien-common-1.0.1rc1/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 14:16:16.000000 linien-common-1.0.1rc1/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 14:16:16.000000 linien-common-1.0.1rc1/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 14:16:16.000000 linien-common-1.0.1rc1/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 14:16:16.971896 linien-common-1.0.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-12-22 14:16:05.000000 linien-common-1.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:32.000000 linien-common-1.0.2rc1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:32.323795 linien-common-1.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 08:31:26.000000 linien-common-1.0.2rc1/setup.py
```

### Comparing `linien-common-1.0.1rc1/PKG-INFO` & `linien-common-1.0.2rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-1.0.1rc1/linien_common/__init__.py` & `linien-common-1.0.2rc1/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.1rc1/linien_common/common.py` & `linien-common-1.0.2rc1/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.1rc1/linien_common/communication.py` & `linien-common-1.0.2rc1/linien_common/communication.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.1rc1/linien_common/config.py` & `linien-common-1.0.2rc1/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.1rc1/linien_common/influxdb.py` & `linien-common-1.0.2rc1/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-common-1.0.1rc1/linien_common.egg-info/PKG-INFO` & `linien-common-1.0.2rc1/linien_common.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 1.0.1rc1
+Version: 1.0.2rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-1.0.1rc1/setup.py` & `linien-common-1.0.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-common",
-    version="1.0.1rc1",
+    version="1.0.2rc1",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Shared components of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
```

