# Comparing `tmp/netops-0.2.8.tar.gz` & `tmp/netops-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netops-0.2.8.tar", last modified: Fri May 20 01:54:15 2022, max compression
+gzip compressed data, was "netops-0.2.9.tar", last modified: Wed May 25 03:44:58 2022, max compression
```

## Comparing `netops-0.2.8.tar` & `netops-0.2.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.348000 netops-0.2.8/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1067 2022-01-11 15:34:33.000000 netops-0.2.8/LICENSE
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       25 2022-01-11 15:28:52.000000 netops-0.2.8/MANIFEST.in
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      765 2022-05-20 01:54:15.348000 netops-0.2.8/PKG-INFO
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       92 2022-01-11 17:23:06.000000 netops-0.2.8/README.md
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.340000 netops-0.2.8/netops/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       13 2022-01-11 15:55:10.000000 netops-0.2.8/netops/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       98 2022-05-20 01:12:54.000000 netops-0.2.8/netops/__version__.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.340000 netops-0.2.8/netops/api/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2021-12-07 15:14:13.000000 netops-0.2.8/netops/api/__init__.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/api/monipe/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:07.000000 netops-0.2.8/netops/api/monipe/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     3496 2022-02-02 19:44:26.000000 netops-0.2.8/netops/api/monipe/homologation_manager.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1545 2022-02-10 16:59:08.000000 netops-0.2.8/netops/api/monipe/homologation_requester.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/api/netbox/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:09.000000 netops-0.2.8/netops/api/netbox/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)    10037 2022-01-31 16:10:11.000000 netops-0.2.8/netops/api/netbox/inventory_plugin.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     4771 2022-01-31 16:19:38.000000 netops-0.2.8/netops/api/netbox/netbox_manager.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     7639 2022-01-31 16:11:10.000000 netops-0.2.8/netops/api/netbox/util.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/api/zabbix/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:12.000000 netops-0.2.8/netops/api/zabbix/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     5887 2022-01-10 16:16:28.000000 netops-0.2.8/netops/api/zabbix/zabbix.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/configs/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:27:42.000000 netops-0.2.8/netops/configs/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)    11278 2022-03-09 01:11:42.000000 netops-0.2.8/netops/configs/apply_devices_configuration.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     3519 2022-01-12 13:28:05.000000 netops-0.2.8/netops/configs/configs.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     3515 2022-01-12 13:28:57.000000 netops-0.2.8/netops/configs/configuration_generator.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     2958 2022-05-17 05:34:16.000000 netops-0.2.8/netops/configs/get_configs.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     2210 2022-05-17 05:35:05.000000 netops-0.2.8/netops/configs/models.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      740 2022-03-09 01:12:44.000000 netops-0.2.8/netops/configs/remote_commands.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1979 2022-04-27 04:00:12.000000 netops-0.2.8/netops/configs/tests.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/digital_twin/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-05-16 22:06:10.000000 netops-0.2.8/netops/digital_twin/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      213 2022-05-17 01:53:37.000000 netops-0.2.8/netops/digital_twin/models.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     5149 2022-05-17 04:54:49.000000 netops-0.2.8/netops/digital_twin/port_mapping.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.344000 netops-0.2.8/netops/infra/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:30:41.000000 netops-0.2.8/netops/infra/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1857 2022-01-12 13:29:45.000000 netops-0.2.8/netops/infra/infra.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.348000 netops-0.2.8/netops/utils/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:31:28.000000 netops-0.2.8/netops/utils/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     3046 2022-05-16 22:30:54.000000 netops-0.2.8/netops/utils/databases.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     2651 2022-02-03 16:59:39.000000 netops-0.2.8/netops/utils/email.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      407 2022-01-13 22:57:57.000000 netops-0.2.8/netops/utils/env_variables.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      724 2022-01-12 13:33:51.000000 netops-0.2.8/netops/utils/monipe_requests.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      339 2022-01-10 16:33:23.000000 netops-0.2.8/netops/utils/paths.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      838 2022-01-10 16:33:45.000000 netops-0.2.8/netops/utils/template_rendering.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     4337 2022-05-16 22:24:47.000000 netops-0.2.8/netops/utils/utils.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.348000 netops-0.2.8/netops/validation_tests/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:34:27.000000 netops-0.2.8/netops/validation_tests/__init__.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.348000 netops-0.2.8/netops/validation_tests/junos/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-02-14 18:42:26.000000 netops-0.2.8/netops/validation_tests/junos/__init__.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1012 2022-02-14 18:59:42.000000 netops-0.2.8/netops/validation_tests/junos/tests.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1311 2022-01-10 16:34:47.000000 netops-0.2.8/netops/validation_tests/reachability.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     5570 2022-05-20 01:12:39.000000 netops-0.2.8/netops/validation_tests/service_tests.py
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1387 2022-01-10 16:35:18.000000 netops-0.2.8/netops/validation_tests/traceroute.py
-drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-20 01:54:15.340000 netops-0.2.8/netops.egg-info/
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      765 2022-05-20 01:54:15.000000 netops-0.2.8/netops.egg-info/PKG-INFO
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     1404 2022-05-20 01:54:15.000000 netops-0.2.8/netops.egg-info/SOURCES.txt
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        1 2022-05-20 01:54:15.000000 netops-0.2.8/netops.egg-info/dependency_links.txt
--rw-rw-r--   0 pedro     (1001) pedro     (1001)      139 2022-05-20 01:54:15.000000 netops-0.2.8/netops.egg-info/requires.txt
--rw-rw-r--   0 pedro     (1001) pedro     (1001)        7 2022-05-20 01:54:15.000000 netops-0.2.8/netops.egg-info/top_level.txt
--rw-rw-r--   0 pedro     (1001) pedro     (1001)       38 2022-05-20 01:54:15.348000 netops-0.2.8/setup.cfg
--rw-rw-r--   0 pedro     (1001) pedro     (1001)     3954 2022-01-11 20:39:52.000000 netops-0.2.8/setup.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.044000 netops-0.2.9/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1067 2022-01-11 15:34:33.000000 netops-0.2.9/LICENSE
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       25 2022-01-11 15:28:52.000000 netops-0.2.9/MANIFEST.in
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      765 2022-05-25 03:44:58.044000 netops-0.2.9/PKG-INFO
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       92 2022-01-11 17:23:06.000000 netops-0.2.9/README.md
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       13 2022-01-11 15:55:10.000000 netops-0.2.9/netops/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       98 2022-05-25 03:43:32.000000 netops-0.2.9/netops/__version__.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops/api/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2021-12-07 15:14:13.000000 netops-0.2.9/netops/api/__init__.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops/api/monipe/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:07.000000 netops-0.2.9/netops/api/monipe/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3496 2022-02-02 19:44:26.000000 netops-0.2.9/netops/api/monipe/homologation_manager.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1545 2022-02-10 16:59:08.000000 netops-0.2.9/netops/api/monipe/homologation_requester.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops/api/netbox/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:09.000000 netops-0.2.9/netops/api/netbox/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)    10037 2022-01-31 16:10:11.000000 netops-0.2.9/netops/api/netbox/inventory_plugin.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     4771 2022-01-31 16:19:38.000000 netops-0.2.9/netops/api/netbox/netbox_manager.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     7639 2022-01-31 16:11:10.000000 netops-0.2.9/netops/api/netbox/util.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops/api/zabbix/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        0 2022-01-11 19:35:12.000000 netops-0.2.9/netops/api/zabbix/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     5887 2022-01-10 16:16:28.000000 netops-0.2.9/netops/api/zabbix/zabbix.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.040000 netops-0.2.9/netops/configs/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:27:42.000000 netops-0.2.9/netops/configs/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)    11278 2022-03-09 01:11:42.000000 netops-0.2.9/netops/configs/apply_devices_configuration.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3519 2022-01-12 13:28:05.000000 netops-0.2.9/netops/configs/configs.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3515 2022-01-12 13:28:57.000000 netops-0.2.9/netops/configs/configuration_generator.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     2987 2022-05-25 03:42:26.000000 netops-0.2.9/netops/configs/get_configs.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     2210 2022-05-17 05:35:05.000000 netops-0.2.9/netops/configs/models.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      740 2022-03-09 01:12:44.000000 netops-0.2.9/netops/configs/remote_commands.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1979 2022-04-27 04:00:12.000000 netops-0.2.9/netops/configs/tests.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.040000 netops-0.2.9/netops/digital_twin/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-05-16 22:06:10.000000 netops-0.2.9/netops/digital_twin/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      213 2022-05-17 01:53:37.000000 netops-0.2.9/netops/digital_twin/models.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     5149 2022-05-17 04:54:49.000000 netops-0.2.9/netops/digital_twin/port_mapping.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.040000 netops-0.2.9/netops/infra/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:30:41.000000 netops-0.2.9/netops/infra/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1857 2022-01-12 13:29:45.000000 netops-0.2.9/netops/infra/infra.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.040000 netops-0.2.9/netops/utils/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:31:28.000000 netops-0.2.9/netops/utils/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3046 2022-05-16 22:30:54.000000 netops-0.2.9/netops/utils/databases.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     2651 2022-02-03 16:59:39.000000 netops-0.2.9/netops/utils/email.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      407 2022-01-13 22:57:57.000000 netops-0.2.9/netops/utils/env_variables.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      724 2022-01-12 13:33:51.000000 netops-0.2.9/netops/utils/monipe_requests.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      339 2022-01-10 16:33:23.000000 netops-0.2.9/netops/utils/paths.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      838 2022-01-10 16:33:45.000000 netops-0.2.9/netops/utils/template_rendering.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     4337 2022-05-16 22:24:47.000000 netops-0.2.9/netops/utils/utils.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.040000 netops-0.2.9/netops/validation_tests/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-01-10 16:34:27.000000 netops-0.2.9/netops/validation_tests/__init__.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.044000 netops-0.2.9/netops/validation_tests/junos/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       30 2022-02-14 18:42:26.000000 netops-0.2.9/netops/validation_tests/junos/__init__.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1012 2022-02-14 18:59:42.000000 netops-0.2.9/netops/validation_tests/junos/tests.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1311 2022-01-10 16:34:47.000000 netops-0.2.9/netops/validation_tests/reachability.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     5570 2022-05-20 01:12:39.000000 netops-0.2.9/netops/validation_tests/service_tests.py
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1387 2022-01-10 16:35:18.000000 netops-0.2.9/netops/validation_tests/traceroute.py
+drwxrwxr-x   0 pedro     (1001) pedro     (1001)        0 2022-05-25 03:44:58.036000 netops-0.2.9/netops.egg-info/
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      765 2022-05-25 03:44:57.000000 netops-0.2.9/netops.egg-info/PKG-INFO
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     1404 2022-05-25 03:44:57.000000 netops-0.2.9/netops.egg-info/SOURCES.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        1 2022-05-25 03:44:57.000000 netops-0.2.9/netops.egg-info/dependency_links.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)      139 2022-05-25 03:44:57.000000 netops-0.2.9/netops.egg-info/requires.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)        7 2022-05-25 03:44:57.000000 netops-0.2.9/netops.egg-info/top_level.txt
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)       38 2022-05-25 03:44:58.044000 netops-0.2.9/setup.cfg
+-rw-rw-r--   0 pedro     (1001) pedro     (1001)     3954 2022-01-11 20:39:52.000000 netops-0.2.9/setup.py
```

### Comparing `netops-0.2.8/LICENSE` & `netops-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/PKG-INFO` & `netops-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netops
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities for NetGitOps Python use cases.
 Home-page: https://git.rnp.br/pop-rj/netops
 Author: Pedro Diniz
 Author-email: pedro.diniz@pop-rj.rnp.br
 License: MIT
 Description: 
         # NetOps
```

### Comparing `netops-0.2.8/netops/api/monipe/homologation_manager.py` & `netops-0.2.9/netops/api/monipe/homologation_manager.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/api/monipe/homologation_requester.py` & `netops-0.2.9/netops/api/monipe/homologation_requester.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/api/netbox/inventory_plugin.py` & `netops-0.2.9/netops/api/netbox/inventory_plugin.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/api/netbox/netbox_manager.py` & `netops-0.2.9/netops/api/netbox/netbox_manager.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/api/netbox/util.py` & `netops-0.2.9/netops/api/netbox/util.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/api/zabbix/zabbix.py` & `netops-0.2.9/netops/api/zabbix/zabbix.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/apply_devices_configuration.py` & `netops-0.2.9/netops/configs/apply_devices_configuration.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/configs.py` & `netops-0.2.9/netops/configs/configs.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/configuration_generator.py` & `netops-0.2.9/netops/configs/configuration_generator.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/get_configs.py` & `netops-0.2.9/netops/configs/get_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
     if format:
         if format.lower() in ['json']:
             data_str = data
         else:
             data_str = etree.tostring(data, encoding='unicode', pretty_print=True)
     else: #default case
+        print("XML: ", data)
         d_data = elem2dict(data)
         data_str = etree.tostring(data, encoding='unicode', pretty_print=True)
 
     if get_print:
         if d_data:
             print_json(d_data)
         else:
```

### Comparing `netops-0.2.8/netops/configs/models.py` & `netops-0.2.9/netops/configs/models.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/remote_commands.py` & `netops-0.2.9/netops/configs/remote_commands.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/configs/tests.py` & `netops-0.2.9/netops/configs/tests.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/digital_twin/port_mapping.py` & `netops-0.2.9/netops/digital_twin/port_mapping.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/infra/infra.py` & `netops-0.2.9/netops/infra/infra.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/utils/databases.py` & `netops-0.2.9/netops/utils/databases.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/utils/email.py` & `netops-0.2.9/netops/utils/email.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/utils/monipe_requests.py` & `netops-0.2.9/netops/utils/monipe_requests.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/utils/template_rendering.py` & `netops-0.2.9/netops/utils/template_rendering.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/utils/utils.py` & `netops-0.2.9/netops/utils/utils.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/validation_tests/junos/tests.py` & `netops-0.2.9/netops/validation_tests/junos/tests.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/validation_tests/reachability.py` & `netops-0.2.9/netops/validation_tests/reachability.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/validation_tests/service_tests.py` & `netops-0.2.9/netops/validation_tests/service_tests.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops/validation_tests/traceroute.py` & `netops-0.2.9/netops/validation_tests/traceroute.py`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/netops.egg-info/PKG-INFO` & `netops-0.2.9/netops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netops
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utilities for NetGitOps Python use cases.
 Home-page: https://git.rnp.br/pop-rj/netops
 Author: Pedro Diniz
 Author-email: pedro.diniz@pop-rj.rnp.br
 License: MIT
 Description: 
         # NetOps
```

### Comparing `netops-0.2.8/netops.egg-info/SOURCES.txt` & `netops-0.2.9/netops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netops-0.2.8/setup.py` & `netops-0.2.9/setup.py`

 * *Files identical despite different names*

