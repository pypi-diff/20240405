# Comparing `tmp/linien-server-1.0.2.tar.gz` & `tmp/linien-server-1.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-1.0.2.tar", last modified: Fri Apr  5 08:49:22 2024, max compression
+gzip compressed data, was "linien-server-1.0.2rc1.tar", last modified: Fri Apr  5 08:31:36 2024, max compression
```

## Comparing `linien-server-1.0.2.tar` & `linien-server-1.0.2rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:22.728547 linien-server-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:49:22.728547 linien-server-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:22.724547 linien-server-1.0.2/linien_server/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:22.724547 linien-server-1.0.2/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (127)  2083740 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/gateware.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/linien_install_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/linien_start_server.sh
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/linien_stop_server.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/noise_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:22.728547 linien-server-1.0.2/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/approach_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-04-05 08:49:10.000000 linien-server-1.0.2/linien_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:49:22.728547 linien-server-1.0.2/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:49:22.000000 linien-server-1.0.2/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:49:22.728547 linien-server-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-05 08:49:10.000000 linien-server-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.631796 linien-server-1.0.2rc1/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.631796 linien-server-1.0.2rc1/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15789 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2083740 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/gateware.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_install_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_start_server.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/linien_stop_server.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/noise_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 08:31:36.000000 linien-server-1.0.2rc1/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:31:36.635796 linien-server-1.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-05 08:31:26.000000 linien-server-1.0.2rc1/setup.py
```

### Comparing `linien-server-1.0.2/PKG-INFO` & `linien-server-1.0.2rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 1.0.2
+Version: 1.0.2rc1
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
@@ -15,10 +15,10 @@
 Requires-Dist: certifi==2021.10.8; python_version < "3.10"
 Requires-Dist: click>=7.1.2
 Requires-Dist: cma>=3.0.3
 Requires-Dist: pylpsd>=0.1.4
 Requires-Dist: pyrp3<2.0,>=1.1.0; platform_machine == "armv7l"
 Requires-Dist: requests==2.25.1; python_version < "3.10"
 Requires-Dist: requests>=2.25.1; python_version >= "3.10"
-Requires-Dist: linien-common==1.0.2
+Requires-Dist: linien-common==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-server-1.0.2/linien_server/__init__.py` & `linien-server-1.0.2rc1/linien_server/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/acquisition.py` & `linien-server-1.0.2rc1/linien_server/acquisition.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/autolock/algorithm_selection.py` & `linien-server-1.0.2rc1/linien_server/autolock/algorithm_selection.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/autolock/autolock.py` & `linien-server-1.0.2rc1/linien_server/autolock/autolock.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/autolock/robust.py` & `linien-server-1.0.2rc1/linien_server/autolock/robust.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/autolock/simple.py` & `linien-server-1.0.2rc1/linien_server/autolock/simple.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/autolock/utils.py` & `linien-server-1.0.2rc1/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/csr.py` & `linien-server-1.0.2rc1/linien_server/csr.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/csrmap.py` & `linien-server-1.0.2rc1/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/gateware.bin` & `linien-server-1.0.2rc1/linien_server/gateware.bin`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/iir_coeffs.py` & `linien-server-1.0.2rc1/linien_server/iir_coeffs.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/influxdb.py` & `linien-server-1.0.2rc1/linien_server/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/noise_analysis.py` & `linien-server-1.0.2rc1/linien_server/noise_analysis.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/optimization/approach_line.py` & `linien-server-1.0.2rc1/linien_server/optimization/approach_line.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/optimization/engine.py` & `linien-server-1.0.2rc1/linien_server/optimization/engine.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/optimization/general.py` & `linien-server-1.0.2rc1/linien_server/optimization/general.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/optimization/optimization.py` & `linien-server-1.0.2rc1/linien_server/optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/optimization/utils.py` & `linien-server-1.0.2rc1/linien_server/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/parameters.py` & `linien-server-1.0.2rc1/linien_server/parameters.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/registers.py` & `linien-server-1.0.2rc1/linien_server/registers.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server/server.py` & `linien-server-1.0.2rc1/linien_server/server.py`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/linien_server.egg-info/PKG-INFO` & `linien-server-1.0.2rc1/linien_server.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 1.0.2
+Version: 1.0.2rc1
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
@@ -15,10 +15,10 @@
 Requires-Dist: certifi==2021.10.8; python_version < "3.10"
 Requires-Dist: click>=7.1.2
 Requires-Dist: cma>=3.0.3
 Requires-Dist: pylpsd>=0.1.4
 Requires-Dist: pyrp3<2.0,>=1.1.0; platform_machine == "armv7l"
 Requires-Dist: requests==2.25.1; python_version < "3.10"
 Requires-Dist: requests>=2.25.1; python_version >= "3.10"
-Requires-Dist: linien-common==1.0.2
+Requires-Dist: linien-common==1.0.2rc1
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien-server-1.0.2/linien_server.egg-info/SOURCES.txt` & `linien-server-1.0.2rc1/linien_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-server-1.0.2/setup.py` & `linien-server-1.0.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-server",
-    version="1.0.2",
+    version="1.0.2rc1",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Server components of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
@@ -41,15 +41,15 @@
         "certifi==2021.10.8;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
         "click>=7.1.2",
         "cma>=3.0.3",
         "pylpsd>=0.1.4",
         "pyrp3>=1.1.0,<2.0;platform_machine=='armv7l'",  # only install on RedPitaya
         "requests==2.25.1;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
         "requests>=2.25.1;python_version>='3.10'",
-        "linien-common==1.0.2",
+        "linien-common==1.0.2rc1",
     ],
     scripts=[
         "linien_server/linien_start_server.sh",
         "linien_server/linien_stop_server.sh",
         "linien_server/linien_install_requirements.sh",
     ],
     package_data={
```

