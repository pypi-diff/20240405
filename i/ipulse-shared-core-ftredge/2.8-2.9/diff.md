# Comparing `tmp/ipulse_shared_core_ftredge-2.8.tar.gz` & `tmp/ipulse_shared_core_ftredge-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipulse_shared_core_ftredge-2.8.tar", last modified: Tue Feb 20 06:07:20 2024, max compression
+gzip compressed data, was "ipulse_shared_core_ftredge-2.9.tar", last modified: Wed Feb 21 11:31:25 2024, max compression
```

## Comparing `ipulse_shared_core_ftredge-2.8.tar` & `ipulse_shared_core_ftredge-2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.322836 ipulse_shared_core_ftredge-2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.322836 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/audit_log_firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/organisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/pulse_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/resource_catalog_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_profile_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-20 06:07:05.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 06:07:20.330836 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-20 06:07:20.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-20 06:07:20.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 06:07:20.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-20 06:07:20.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-20 06:07:20.000000 ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.028315 ipulse_shared_core_ftredge-2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/audit_log_firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/pulse_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/resource_catalog_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_profile_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-21 11:31:10.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 11:31:25.032315 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-21 11:31:24.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-21 11:31:25.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 11:31:24.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-21 11:31:24.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-21 11:31:24.000000 ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/top_level.txt
```

### Comparing `ipulse_shared_core_ftredge-2.8/LICENCE` & `ipulse_shared_core_ftredge-2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/setup.py` & `ipulse_shared_core_ftredge-2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ipulse_shared_core_ftredge',
-    version='2.8',
+    version='2.9',
     package_dir={'': 'src'},  # Specify the source directory
     packages=find_packages(where='src'),  # Look for packages in 'src'
     install_requires=[
         # List your dependencies here
         'pydantic[email]~=2.5',
         'python-dateutil~=2.8',
         'pytest~=7.1',
```

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/organisation.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/organisation.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/pulse_enums.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/pulse_enums.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/resource_catalog_item.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/resource_catalog_item.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_profile.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_profile_update.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_profile_update.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/models/user_status.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/models/user_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 CLASS_VERSION = 2.1
 CLASS_REVISION_AUTHOR="Russlan Ramdowar;russlan@ftredge.com"
 CLASS_REVISION_DATE=datetime(2024, 2, 13, 20, 15)
 
 DOMAIN="user"
 OBJ_REF = "usrsttus"
 
-DEFAULT_USER_GROUPS={"pulseroot__authuser_open"}
+DEFAULT_USER_GROUPS={"pulseroot":["read_authuser_open"]}
 DEFAULT_SUBSCRIPTION_PLAN="subscription_free"
 DEFAULT_SUBSCRIPTION_STATUS="active"
 DEFAULT_SUBSCRIPTION_INSIGHT_CREDITS=7
 DEFAULT_EXTRA_INSIGHT_CREDITS=0
 
 class UserStatus(BaseModel):
     schema_version: float = Field(default=CLASS_VERSION, description="Version of this Class == version of DB Schema") #User can Read only
```

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge/tests/test.py` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge/tests/test.py`

 * *Files identical despite different names*

### Comparing `ipulse_shared_core_ftredge-2.8/src/ipulse_shared_core_ftredge.egg-info/SOURCES.txt` & `ipulse_shared_core_ftredge-2.9/src/ipulse_shared_core_ftredge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

