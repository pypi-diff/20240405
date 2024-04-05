# Comparing `tmp/cadcutils-1.5.1.2.tar.gz` & `tmp/cadcutils-1.5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadcutils-1.5.1.2.tar", last modified: Fri Jul 28 15:47:13 2023, max compression
+gzip compressed data, was "cadcutils-1.5.1.3.tar", last modified: Fri Apr  5 21:00:41 2024, max compression
```

## Comparing `cadcutils-1.5.1.2.tar` & `cadcutils-1.5.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.284331 cadcutils-1.5.1.2/cadcutils/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.292331 cadcutils-1.5.1.2/cadcutils/net/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14480 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9055 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/group_xml/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/group_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/user_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/group_xml/user_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29291 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/groups_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/netutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/net/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    20910 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_groups_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_int_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_netutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64620 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/tests/test_wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55249 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/ws.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12263 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/net/wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8457 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/old_get_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.296331 cadcutils-1.5.1.2/cadcutils/util/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/cadcutils/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 15:47:11.000000 cadcutils-1.5.1.2/cadcutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:47:13.288331 cadcutils-1.5.1.2/cadcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 15:47:13.000000 cadcutils-1.5.1.2/cadcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 15:47:13.300331 cadcutils-1.5.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3093 2023-07-28 15:46:59.000000 cadcutils-1.5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.003358 cadcutils-1.5.1.3/cadcutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.003358 cadcutils-1.5.1.3/cadcutils/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9055 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/group_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_user_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/user_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/user_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29291 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/netutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_int_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_netutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64620 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55249 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/ws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12263 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8457 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/old_get_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/cadcutils/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/cadcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/setup.py
```

### Comparing `cadcutils-1.5.1.2/LICENSE` & `cadcutils-1.5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/README.rst` & `cadcutils-1.5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/exceptions.py` & `cadcutils-1.5.1.3/cadcutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/__init__.py` & `cadcutils-1.5.1.3/cadcutils/net/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/auth.py` & `cadcutils-1.5.1.3/cadcutils/net/auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group.py` & `cadcutils-1.5.1.3/cadcutils/net/group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/__init__.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_reader.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_property_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_reader.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/group_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_reader.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/groups_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_group_reader_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_groups_reader_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_groups_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/tests/test_user_reader_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_user_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/user_reader.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/user_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/group_xml/user_writer.py` & `cadcutils-1.5.1.3/cadcutils/net/group_xml/user_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/groups_client.py` & `cadcutils-1.5.1.3/cadcutils/net/groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/netutils.py` & `cadcutils-1.5.1.3/cadcutils/net/netutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,23 +225,30 @@
                     param = ElementTree.SubElement(vos_view, "vos:param")
                     param.attrib['uri'] = CADC_VO_VIEWS[view]
                     param.text = cutout
             protocol_element = ElementTree.SubElement(transfer_xml,
                                                       "vos:protocol")
             protocol_element.attrib['uri'] = "{0}#{1}".format(
                 Transfer.IVOAURL, protocol[direction])
+
             if security_methods:
                 for sm in security_methods:
                     if sm not in SSO_SECURITY_METHODS.values():
                         raise AttributeError(
                             'Invalid security method {}. Supported values: {}'.
                             format(sm, SSO_SECURITY_METHODS.values))
                     security_element = ElementTree.SubElement(
                         protocol_element, "vos:securityMethod")
                     security_element.attrib['uri'] = sm
+            if security_methods:
+                # add the default anon method
+                protocol_element = ElementTree.SubElement(transfer_xml,
+                                                          "vos:protocol")
+                protocol_element.attrib['uri'] = "{0}#{1}".format(
+                    Transfer.IVOAURL, protocol[direction])
 
         logging.debug(ElementTree.tostring(transfer_xml))
         logging.debug("Sending to : {}".format(endpoint_url))
 
         data = ElementTree.tostring(transfer_xml)
         resp = self.session.post(
             endpoint_url, data=data, allow_redirects=False,
```

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_auth.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_group.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_groups_client.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_int_groups.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_int_groups.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_netutils.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_ws.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/tests/test_wscapabilities.py` & `cadcutils-1.5.1.3/cadcutils/net/tests/test_wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/ws.py` & `cadcutils-1.5.1.3/cadcutils/net/ws.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/net/wscapabilities.py` & `cadcutils-1.5.1.3/cadcutils/net/wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/old_get_cert.py` & `cadcutils-1.5.1.3/cadcutils/old_get_cert.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/util/__init__.py` & `cadcutils-1.5.1.3/cadcutils/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/util/config.py` & `cadcutils-1.5.1.3/cadcutils/util/config.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils/util/utils.py` & `cadcutils-1.5.1.3/cadcutils/util/utils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/cadcutils.egg-info/SOURCES.txt` & `cadcutils-1.5.1.3/cadcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.2/setup.cfg` & `cadcutils-1.5.1.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 long_description = Library of utilities. It includes generic utilities for logging and command line parsing, networking utilities, etc.
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 edit_on_github = False
 github_project = opencadc/cadctools
-version = 1.5.1.2
+version = 1.5.1.3
 
 [options]
 install_requires = 
 	setuptools>=36.0
 	requests>=2.8
 	lxml>=3.7.0
 	html2text
```

### Comparing `cadcutils-1.5.1.2/setup.py` & `cadcutils-1.5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import glob
 import os
 import sys
-import imp
 from setuptools.command.test import test as TestCommand
 from setuptools import find_packages
 
 from setuptools import setup
 
 import distutils.cmd
 import distutils.log
```

