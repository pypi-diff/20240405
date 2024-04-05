# Comparing `tmp/kivera-sdk-1.7.0.tar.gz` & `tmp/kivera-sdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivera-sdk-1.7.0.tar", last modified: Tue Mar  5 22:53:30 2024, max compression
+gzip compressed data, was "kivera-sdk-1.8.0.tar", last modified: Fri Apr  5 00:17:29 2024, max compression
```

## Comparing `kivera-sdk-1.7.0.tar` & `kivera-sdk-1.8.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.730521 kivera-sdk-1.7.0/kivera/
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.730521 kivera-sdk-1.7.0/kivera/cloudtenants/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/cloudtenants/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.730521 kivera-sdk-1.7.0/kivera/compliancemappings/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/compliancemappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/compliancemappings/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.730521 kivera-sdk-1.7.0/kivera/config/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/config/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.730521 kivera-sdk-1.7.0/kivera/counters/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/counters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/counters/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/globalpolicyfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/globalpolicyfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/globalpolicyfunctions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/globalpolicyfunctions/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/globalservices/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/globalservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/globalservices/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/identities/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/identityprofiles/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identityprofiles/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/identitytypes/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identitytypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identitytypes/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/identitytypes/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/managedrules/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/managedrules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/managedrules/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/memberships/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/memberships/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/metrics/getcounterproxymetrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.734521 kivera-sdk-1.7.0/kivera/notificationdestinations/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationdestinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationdestinations/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationdestinations/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/notificationmonitors/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationmonitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationmonitors/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/notificationmonitors/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizations/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizations/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/organizations/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/plans/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/plans/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/profiles/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/providers/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/providers/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/providerversions/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/providerversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/providerversions/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.738521 kivera-sdk-1.7.0/kivera/proxies/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxies/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/proxyapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxyapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxyapikeys/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/proxydeployments/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxydeployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxydeployments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxydeployments/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxydeployments/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxydeployments/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/proxyproviders/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxyproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/proxyproviders/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/roles/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/roles/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/ruledependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruledependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruledependencies/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruledependencies/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/ruledependencyresources/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruledependencyresources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruledependencyresources/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/ruleparameters/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruleparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/ruleparameters/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/rules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/services/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/services/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.742521 kivera-sdk-1.7.0/kivera/trailblazerapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazerapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazerapikeys/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/kivera/trailblazeridentities/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazeridentities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/kivera/trailblazers/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/trailblazers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/kivera/userapikeys/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/userapikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/userapikeys/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/userapikeys/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/userapikeys/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/kivera/users/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/users/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/users/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/users/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/kivera/users/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/kivera_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-05 22:53:30.000000 kivera-sdk-1.7.0/kivera_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-05 22:53:30.000000 kivera-sdk-1.7.0/kivera_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 22:53:30.000000 kivera-sdk-1.7.0/kivera_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-05 22:53:30.000000 kivera-sdk-1.7.0/kivera_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 22:53:30.000000 kivera-sdk-1.7.0/kivera_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-05 22:53:30.746521 kivera-sdk-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-05 22:53:12.000000 kivera-sdk-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.198516 kivera-sdk-1.8.0/kivera/
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.198516 kivera-sdk-1.8.0/kivera/cloudtenants/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/cloudtenants/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/compliancemappings/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/compliancemappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/compliancemappings/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/config/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/counters/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/counters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/counters/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalpolicyfunctions/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/globalservices/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/globalservices/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identities/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identityprofiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identityprofiles/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.202516 kivera-sdk-1.8.0/kivera/identitytypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/identitytypes/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/managedrules/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/managedrules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/managedrules/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/memberships/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/memberships/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/metrics/getcounterproxymetrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/notificationdestinations/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationdestinations/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/notificationmonitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/notificationmonitors/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/organizations/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.206516 kivera-sdk-1.8.0/kivera/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/plans/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/profiles/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providers/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/providerversions/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providerversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/providerversions/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxies/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxies/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxyapikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyapikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyapikeys/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxydeployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxydeployments/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.210516 kivera-sdk-1.8.0/kivera/proxyproviders/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/proxyproviders/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/roles/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruledependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencies/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruledependencyresources/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencyresources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruledependencyresources/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/ruleparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruleparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/ruleparameters/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/rules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/services/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.214516 kivera-sdk-1.8.0/kivera/trailblazerapikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazerapikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazerapikeys/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/trailblazeridentities/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazeridentities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/trailblazers/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/trailblazers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/userapikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/userapikeys/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/kivera/users/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/kivera_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 00:17:29.000000 kivera-sdk-1.8.0/kivera_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 00:17:29.218516 kivera-sdk-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-05 00:17:02.000000 kivera-sdk-1.8.0/setup.py
```

### Comparing `kivera-sdk-1.7.0/LICENSE` & `kivera-sdk-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/PKG-INFO` & `kivera-sdk-1.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivera-sdk
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python library to interact with the Kivera Graphql API
 Home-page: https://github.com/kivera-io/python-client
 Author: Kivera
 Author-email: support@kivera.io
 License: MIT License
 Keywords: kivera graphql gql sdk client
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kivera-sdk-1.7.0/kivera/__init__.py` & `kivera-sdk-1.8.0/kivera/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "v1.7.0"
+__version__ = "v1.8.0"
 import json
 import requests
 from gql import Client as GqlClient
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.exceptions import TransportQueryError
 from jose import jwt, exceptions
 from datetime import datetime, timedelta
```

### Comparing `kivera-sdk-1.7.0/kivera/cloudtenants/create.py` & `kivera-sdk-1.8.0/kivera/cloudtenants/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/cloudtenants/delete.py` & `kivera-sdk-1.8.0/kivera/cloudtenants/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/cloudtenants/get.py` & `kivera-sdk-1.8.0/kivera/cloudtenants/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/cloudtenants/list.py` & `kivera-sdk-1.8.0/kivera/cloudtenants/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/cloudtenants/update.py` & `kivera-sdk-1.8.0/kivera/cloudtenants/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/compliancemappings/list.py` & `kivera-sdk-1.8.0/kivera/compliancemappings/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/config/get.py` & `kivera-sdk-1.8.0/kivera/config/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/counters/get.py` & `kivera-sdk-1.8.0/kivera/counters/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/globalpolicyfunctions/get.py` & `kivera-sdk-1.8.0/kivera/globalpolicyfunctions/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/globalpolicyfunctions/list.py` & `kivera-sdk-1.8.0/kivera/globalpolicyfunctions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/globalservices/list.py` & `kivera-sdk-1.8.0/kivera/globalservices/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identities/create.py` & `kivera-sdk-1.8.0/kivera/identities/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identities/delete.py` & `kivera-sdk-1.8.0/kivera/identities/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identities/get.py` & `kivera-sdk-1.8.0/kivera/identities/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identities/list.py` & `kivera-sdk-1.8.0/kivera/identities/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identities/update.py` & `kivera-sdk-1.8.0/kivera/identities/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identityprofiles/create.py` & `kivera-sdk-1.8.0/kivera/identityprofiles/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identityprofiles/delete.py` & `kivera-sdk-1.8.0/kivera/identityprofiles/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identityprofiles/get.py` & `kivera-sdk-1.8.0/kivera/identityprofiles/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identityprofiles/list.py` & `kivera-sdk-1.8.0/kivera/identityprofiles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identityprofiles/update.py` & `kivera-sdk-1.8.0/kivera/identityprofiles/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identitytypes/get.py` & `kivera-sdk-1.8.0/kivera/identitytypes/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/identitytypes/list.py` & `kivera-sdk-1.8.0/kivera/identitytypes/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/managedrules/list.py` & `kivera-sdk-1.8.0/kivera/users/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 from gql import gql
 from typing import Sequence
 
 class listMethods:
 
-    _ListManagedRulesQuery = """
-    query ListManagedRules {
-    ManagedRules{
-        id
-        type_id
-        description
-        policy
-        config
-        tags
-        version
-        risk_rating
-        compliance_mappings
-        Service {
-            id
-            GlobalService {
-                id
-                name
-                Provider {
-                    id
-                    name
-                }
-                Services {
-                    id
-                    inspection
-                }
-            }
+    _ListUsersQuery = """
+    query ListUsers {
+  Users {
+    id
+    verified
+    email
+    given_name
+    family_name
+    created_at
+    Memberships {
+      id
+      MembershipRoles {
+        Role {
+          role_name
+          id
         }
+      }
     }
+  }
 }
     """
 
-    def ListManagedRules(self):
-        query = gql(self._ListManagedRulesQuery)
+    def ListUsers(self):
+        query = gql(self._ListUsersQuery)
         variables = {
         }
-        operation_name = "ListManagedRules"
+        operation_name = "ListUsers"
+        operation_type = "read"
+        return self.execute(
+            query,
+            variable_values=variables,
+            operation_name=operation_name,
+            operation_type=operation_type,
+        )
+
+    _ListVerifiedUsersQuery = """
+    query ListVerifiedUsers {
+  Users(where: {verified: {_eq: true}}) {
+    id
+    email
+    given_name
+    family_name
+  }
+}
+    """
+
+    def ListVerifiedUsers(self):
+        query = gql(self._ListVerifiedUsersQuery)
+        variables = {
+        }
+        operation_name = "ListVerifiedUsers"
         operation_type = "read"
         return self.execute(
             query,
             variable_values=variables,
             operation_name=operation_name,
             operation_type=operation_type,
         )
```

### Comparing `kivera-sdk-1.7.0/kivera/memberships/create.py` & `kivera-sdk-1.8.0/kivera/memberships/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/memberships/delete.py` & `kivera-sdk-1.8.0/kivera/memberships/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/memberships/get.py` & `kivera-sdk-1.8.0/kivera/memberships/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/memberships/list.py` & `kivera-sdk-1.8.0/kivera/memberships/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/memberships/update.py` & `kivera-sdk-1.8.0/kivera/memberships/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/metrics/getcounterproxymetrics.py` & `kivera-sdk-1.8.0/kivera/metrics/getcounterproxymetrics.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/notificationdestinations/get.py` & `kivera-sdk-1.8.0/kivera/notificationdestinations/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/notificationdestinations/list.py` & `kivera-sdk-1.8.0/kivera/notificationdestinations/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/notificationmonitors/get.py` & `kivera-sdk-1.8.0/kivera/notificationmonitors/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/notificationmonitors/list.py` & `kivera-sdk-1.8.0/kivera/notificationmonitors/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/create.py` & `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/delete.py` & `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/get.py` & `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/list.py` & `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizationpolicyfunctions/update.py` & `kivera-sdk-1.8.0/kivera/organizationpolicyfunctions/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizations/get.py` & `kivera-sdk-1.8.0/kivera/organizations/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizations/list.py` & `kivera-sdk-1.8.0/kivera/organizations/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/organizations/update.py` & `kivera-sdk-1.8.0/kivera/organizations/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/plans/list.py` & `kivera-sdk-1.8.0/kivera/plans/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/attach.py` & `kivera-sdk-1.8.0/kivera/profiles/attach.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/create.py` & `kivera-sdk-1.8.0/kivera/profiles/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/delete.py` & `kivera-sdk-1.8.0/kivera/profiles/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/get.py` & `kivera-sdk-1.8.0/kivera/profiles/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/list.py` & `kivera-sdk-1.8.0/kivera/profiles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/profiles/update.py` & `kivera-sdk-1.8.0/kivera/profiles/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/providers/get.py` & `kivera-sdk-1.8.0/kivera/providers/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/providers/list.py` & `kivera-sdk-1.8.0/kivera/providers/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/providerversions/list.py` & `kivera-sdk-1.8.0/kivera/providerversions/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxies/create.py` & `kivera-sdk-1.8.0/kivera/proxies/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxies/delete.py` & `kivera-sdk-1.8.0/kivera/proxies/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxies/get.py` & `kivera-sdk-1.8.0/kivera/proxies/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxies/list.py` & `kivera-sdk-1.8.0/kivera/proxies/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxies/update.py` & `kivera-sdk-1.8.0/kivera/proxies/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxyapikeys/get.py` & `kivera-sdk-1.8.0/kivera/proxyapikeys/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxydeployments/create.py` & `kivera-sdk-1.8.0/kivera/proxydeployments/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxydeployments/get.py` & `kivera-sdk-1.8.0/kivera/proxydeployments/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxydeployments/list.py` & `kivera-sdk-1.8.0/kivera/proxydeployments/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxydeployments/update.py` & `kivera-sdk-1.8.0/kivera/proxydeployments/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/proxyproviders/list.py` & `kivera-sdk-1.8.0/kivera/proxyproviders/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/roles/list.py` & `kivera-sdk-1.8.0/kivera/roles/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/ruledependencies/attach.py` & `kivera-sdk-1.8.0/kivera/ruledependencies/attach.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/ruledependencies/get.py` & `kivera-sdk-1.8.0/kivera/ruledependencies/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/ruledependencyresources/get.py` & `kivera-sdk-1.8.0/kivera/ruledependencyresources/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/ruleparameters/get.py` & `kivera-sdk-1.8.0/kivera/ruleparameters/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/rules/create.py` & `kivera-sdk-1.8.0/kivera/rules/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/rules/delete.py` & `kivera-sdk-1.8.0/kivera/rules/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/rules/get.py` & `kivera-sdk-1.8.0/kivera/rules/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/rules/list.py` & `kivera-sdk-1.8.0/kivera/rules/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/rules/update.py` & `kivera-sdk-1.8.0/kivera/rules/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/services/create.py` & `kivera-sdk-1.8.0/kivera/services/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/services/delete.py` & `kivera-sdk-1.8.0/kivera/services/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/services/get.py` & `kivera-sdk-1.8.0/kivera/services/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/services/list.py` & `kivera-sdk-1.8.0/kivera/services/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/services/update.py` & `kivera-sdk-1.8.0/kivera/services/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazerapikeys/get.py` & `kivera-sdk-1.8.0/kivera/trailblazerapikeys/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazeridentities/create.py` & `kivera-sdk-1.8.0/kivera/trailblazeridentities/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazeridentities/delete.py` & `kivera-sdk-1.8.0/kivera/trailblazeridentities/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazeridentities/get.py` & `kivera-sdk-1.8.0/kivera/trailblazeridentities/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazeridentities/list.py` & `kivera-sdk-1.8.0/kivera/trailblazeridentities/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazeridentities/update.py` & `kivera-sdk-1.8.0/kivera/trailblazeridentities/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazers/create.py` & `kivera-sdk-1.8.0/kivera/trailblazers/create.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazers/delete.py` & `kivera-sdk-1.8.0/kivera/trailblazers/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazers/get.py` & `kivera-sdk-1.8.0/kivera/trailblazers/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazers/list.py` & `kivera-sdk-1.8.0/kivera/trailblazers/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/trailblazers/update.py` & `kivera-sdk-1.8.0/kivera/trailblazers/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/userapikeys/get.py` & `kivera-sdk-1.8.0/kivera/userapikeys/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/userapikeys/list.py` & `kivera-sdk-1.8.0/kivera/userapikeys/list.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/userapikeys/update.py` & `kivera-sdk-1.8.0/kivera/userapikeys/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/users/delete.py` & `kivera-sdk-1.8.0/kivera/users/delete.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/users/get.py` & `kivera-sdk-1.8.0/kivera/users/get.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera/users/update.py` & `kivera-sdk-1.8.0/kivera/users/update.py`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/kivera_sdk.egg-info/PKG-INFO` & `kivera-sdk-1.8.0/kivera_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivera-sdk
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python library to interact with the Kivera Graphql API
 Home-page: https://github.com/kivera-io/python-client
 Author: Kivera
 Author-email: support@kivera.io
 License: MIT License
 Keywords: kivera graphql gql sdk client
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kivera-sdk-1.7.0/kivera_sdk.egg-info/SOURCES.txt` & `kivera-sdk-1.8.0/kivera_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kivera-sdk-1.7.0/setup.py` & `kivera-sdk-1.8.0/setup.py`

 * *Files identical despite different names*

