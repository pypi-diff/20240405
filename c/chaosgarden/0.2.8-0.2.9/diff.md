# Comparing `tmp/chaosgarden-0.2.8.tar.gz` & `tmp/chaosgarden-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaosgarden-0.2.8.tar", last modified: Wed Feb 28 13:28:44 2024, max compression
+gzip compressed data, was "chaosgarden-0.2.9.tar", last modified: Fri Apr  5 09:43:35 2024, max compression
```

## Comparing `chaosgarden-0.2.8.tar` & `chaosgarden-0.2.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.047778 chaosgarden-0.2.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2370 2024-02-28 13:28:44.047778 chaosgarden-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/alicloud/
--rw-r--r--   0 root         (0) root         (0)    28062 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/alicloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17105 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/alicloud/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/aws/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12710 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/aws/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/azure/
--rw-r--r--   0 root         (0) root         (0)     7694 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14897 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/azure/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/garden/
--rw-r--r--   0 root         (0) root         (0)      621 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/garden/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23358 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/garden/actions.py
--rw-r--r--   0 root         (0) root         (0)     4235 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/garden/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/gcp/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/gcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15392 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/gcp/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.039778 chaosgarden-0.2.8/chaosgarden/human/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/human/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/human/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/k8s/
--rw-r--r--   0 root         (0) root         (0)     6886 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4714 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/k8s/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3425 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/api/authenticators.py
--rw-r--r--   0 root         (0) root         (0)     7365 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/api/clients.py
--rw-r--r--   0 root         (0) root         (0)     2143 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/api/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/k8s/probe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11170 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2416 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/generate_resources.py
--rw-r--r--   0 root         (0) root         (0)    14856 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/probe_pod.py
--rw-r--r--   0 root         (0) root         (0)     2012 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/suicidal_pod.py
--rw-r--r--   0 root         (0) root         (0)     8099 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/templated_resources.yaml
--rw-r--r--   0 root         (0) root         (0)     1943 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probe/thresholds.py
--rw-r--r--   0 root         (0) root         (0)    20971 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/k8s/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/metal/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/metal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/openstack/
--rw-r--r--   0 root         (0) root         (0)     4446 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/openstack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13046 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/openstack/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.043778 chaosgarden-0.2.8/chaosgarden/util/
--rw-r--r--   0 root         (0) root         (0)      916 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/util/terminator.py
--rw-r--r--   0 root         (0) root         (0)     3712 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/util/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.047778 chaosgarden-0.2.8/chaosgarden/vsphere/
--rw-r--r--   0 root         (0) root         (0)    11990 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/vsphere/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10486 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/vsphere/actions.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/chaosgarden/vsphere/pchelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:28:44.047778 chaosgarden-0.2.8/chaosgarden.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2024-02-28 13:28:43.000000 chaosgarden-0.2.8/chaosgarden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1443 2024-02-28 13:28:44.000000 chaosgarden-0.2.8/chaosgarden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 13:28:43.000000 chaosgarden-0.2.8/chaosgarden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      436 2024-02-28 13:28:43.000000 chaosgarden-0.2.8/chaosgarden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-02-28 13:28:43.000000 chaosgarden-0.2.8/chaosgarden.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-28 13:28:44.047778 chaosgarden-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3331 2024-02-28 13:27:40.000000 chaosgarden-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.823026 chaosgarden-0.2.9/chaosgarden/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.823026 chaosgarden-0.2.9/chaosgarden/alicloud/
+-rw-r--r--   0 root         (0) root         (0)    28062 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/alicloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17105 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/alicloud/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.823026 chaosgarden-0.2.9/chaosgarden/aws/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12710 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/aws/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.823026 chaosgarden-0.2.9/chaosgarden/azure/
+-rw-r--r--   0 root         (0) root         (0)     7694 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14897 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/azure/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/garden/
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/garden/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23358 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/garden/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/garden/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/gcp/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/gcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15392 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/gcp/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/human/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/human/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/human/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/k8s/
+-rw-r--r--   0 root         (0) root         (0)     6886 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/k8s/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/api/authenticators.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/api/clients.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/api/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.827026 chaosgarden-0.2.9/chaosgarden/k8s/probe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11170 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/generate_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14856 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/probe_pod.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/suicidal_pod.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/templated_resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probe/thresholds.py
+-rw-r--r--   0 root         (0) root         (0)    20971 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/k8s/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden/metal/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/metal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden/openstack/
+-rw-r--r--   0 root         (0) root         (0)     4446 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/openstack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13046 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/openstack/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden/util/
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/util/terminator.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/util/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden/vsphere/
+-rw-r--r--   0 root         (0) root         (0)    11990 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/vsphere/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10486 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/vsphere/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/chaosgarden/vsphere/pchelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/chaosgarden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-05 09:43:35.000000 chaosgarden-0.2.9/chaosgarden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-04-05 09:43:35.000000 chaosgarden-0.2.9/chaosgarden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 09:43:35.000000 chaosgarden-0.2.9/chaosgarden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-05 09:43:35.000000 chaosgarden-0.2.9/chaosgarden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-05 09:43:35.000000 chaosgarden-0.2.9/chaosgarden.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 09:43:35.831026 chaosgarden-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-04-05 09:42:42.000000 chaosgarden-0.2.9/setup.py
```

### Comparing `chaosgarden-0.2.8/LICENSE` & `chaosgarden-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/PKG-INFO` & `chaosgarden-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
@@ -19,15 +19,15 @@
 Requires-Dist: azure-mgmt-network<23,>=22.2.0
 Requires-Dist: chaostoolkit<2,>=1.15.0
 Requires-Dist: chaostoolkit-lib<2,>=1.33.1
 Requires-Dist: chaostoolkit-aws<1,>=0.21.2
 Requires-Dist: chaostoolkit-azure<1,>=0.11.0
 Requires-Dist: chaostoolkit-google-cloud-platform<1,>=0.8.0
 Requires-Dist: chaostoolkit-kubernetes<1,>=0.26.3
-Requires-Dist: kubernetes>=24.2.0
+Requires-Dist: kubernetes>=28.1.0
 Requires-Dist: Mako<2,>=1.2.4
 Requires-Dist: openstacksdk<2,>=1.0.1
 Requires-Dist: python-box<8,>=7.0.0
 Requires-Dist: PyYAML<7,>=6.0
 Requires-Dist: urllib3<2,>=1.26.14
 Requires-Dist: aliyun-python-sdk-core<3,>=2.13.36
 Requires-Dist: aliyun-python-sdk-ecs<5,>=4.24.30
```

### Comparing `chaosgarden-0.2.8/chaosgarden/alicloud/__init__.py` & `chaosgarden-0.2.9/chaosgarden/alicloud/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/alicloud/actions.py` & `chaosgarden-0.2.9/chaosgarden/alicloud/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/aws/actions.py` & `chaosgarden-0.2.9/chaosgarden/aws/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/azure/__init__.py` & `chaosgarden-0.2.9/chaosgarden/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/azure/actions.py` & `chaosgarden-0.2.9/chaosgarden/azure/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/garden/__init__.py` & `chaosgarden-0.2.9/chaosgarden/garden/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/garden/actions.py` & `chaosgarden-0.2.9/chaosgarden/garden/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/garden/probes.py` & `chaosgarden-0.2.9/chaosgarden/garden/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/gcp/__init__.py` & `chaosgarden-0.2.9/chaosgarden/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/gcp/actions.py` & `chaosgarden-0.2.9/chaosgarden/gcp/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/__init__.py` & `chaosgarden-0.2.9/chaosgarden/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/actions.py` & `chaosgarden-0.2.9/chaosgarden/k8s/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/api/authenticators.py` & `chaosgarden-0.2.9/chaosgarden/k8s/api/authenticators.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/api/clients.py` & `chaosgarden-0.2.9/chaosgarden/k8s/api/clients.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/api/cluster.py` & `chaosgarden-0.2.9/chaosgarden/k8s/api/cluster.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/metrics.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/metrics.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/generate_resources.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/generate_resources.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/probe_pod.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/probe_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/suicidal_pod.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/suicidal_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/resources/templated_resources.yaml` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/resources/templated_resources.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
       containers:
       - name: probe
         image: python:3.9.15-slim-bullseye
         imagePullPolicy: IfNotPresent
         command:
         - 'bash'
         - '-c'
-        - 'pip install kubernetes==24.2.0 Flask==2.2.2; python -u /app/probe-pod.py'
+        - 'pip install kubernetes==28.1.0 Flask==2.3.3; python -u /app/probe-pod.py'
         readinessProbe:
           httpGet:
             scheme: 'HTTPS'
             port: 8080
             path: '/readyz'
           initialDelaySeconds: 5
           periodSeconds: 5
@@ -245,15 +245,15 @@
       containers:
       - name: probe
         image: python:3.9.15-slim-bullseye
         imagePullPolicy: IfNotPresent
         command:
         - 'bash'
         - '-c'
-        - 'pip install kubernetes==24.2.0; python -u /app/suicidal-pod.py'
+        - 'pip install kubernetes==28.1.0; python -u /app/suicidal-pod.py'
         volumeMounts:
         - name: probe
           mountPath: '/app'
           readOnly: true
         - name: pod
           mountPath: /pod
           readOnly: true
```

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probe/thresholds.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probe/thresholds.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/k8s/probes.py` & `chaosgarden-0.2.9/chaosgarden/k8s/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/openstack/__init__.py` & `chaosgarden-0.2.9/chaosgarden/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/openstack/actions.py` & `chaosgarden-0.2.9/chaosgarden/openstack/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/util/__init__.py` & `chaosgarden-0.2.9/chaosgarden/util/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/util/terminator.py` & `chaosgarden-0.2.9/chaosgarden/util/terminator.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/util/threading.py` & `chaosgarden-0.2.9/chaosgarden/util/threading.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/vsphere/__init__.py` & `chaosgarden-0.2.9/chaosgarden/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/vsphere/actions.py` & `chaosgarden-0.2.9/chaosgarden/vsphere/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden/vsphere/pchelper.py` & `chaosgarden-0.2.9/chaosgarden/vsphere/pchelper.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/chaosgarden.egg-info/PKG-INFO` & `chaosgarden-0.2.9/chaosgarden.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
@@ -19,15 +19,15 @@
 Requires-Dist: azure-mgmt-network<23,>=22.2.0
 Requires-Dist: chaostoolkit<2,>=1.15.0
 Requires-Dist: chaostoolkit-lib<2,>=1.33.1
 Requires-Dist: chaostoolkit-aws<1,>=0.21.2
 Requires-Dist: chaostoolkit-azure<1,>=0.11.0
 Requires-Dist: chaostoolkit-google-cloud-platform<1,>=0.8.0
 Requires-Dist: chaostoolkit-kubernetes<1,>=0.26.3
-Requires-Dist: kubernetes>=24.2.0
+Requires-Dist: kubernetes>=28.1.0
 Requires-Dist: Mako<2,>=1.2.4
 Requires-Dist: openstacksdk<2,>=1.0.1
 Requires-Dist: python-box<8,>=7.0.0
 Requires-Dist: PyYAML<7,>=6.0
 Requires-Dist: urllib3<2,>=1.26.14
 Requires-Dist: aliyun-python-sdk-core<3,>=2.13.36
 Requires-Dist: aliyun-python-sdk-ecs<5,>=4.24.30
```

### Comparing `chaosgarden-0.2.8/chaosgarden.egg-info/SOURCES.txt` & `chaosgarden-0.2.9/chaosgarden.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.8/setup.py` & `chaosgarden-0.2.9/setup.py`

 * *Files identical despite different names*

