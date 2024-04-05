# Comparing `tmp/metaflow-netflixext-1.1.2.tar.gz` & `tmp/metaflow-netflixext-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-1.1.2.tar", last modified: Thu Jan 11 10:10:51 2024, max compression
+gzip compressed data, was "metaflow-netflixext-1.1.3.tar", last modified: Fri Apr  5 17:20:01 2024, max compression
```

## Comparing `metaflow-netflixext-1.1.2.tar` & `metaflow-netflixext-1.1.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.090326 metaflow-netflixext-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-01-11 10:10:51.090326 metaflow-netflixext-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.078326 metaflow-netflixext-1.1.2/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.082326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.082326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.082326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44223 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.082326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.082326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.086326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   112586 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25941 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    26542 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    51745 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (127)    39711 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.086326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.086326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (127)   113678 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    24592 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.086326 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/toplevel/netflixext_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 10:10:51.090326 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-01-11 10:10:51.000000 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-01-11 10:10:51.000000 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 10:10:51.000000 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-11 10:10:51.000000 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-11 10:10:51.000000 metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 10:10:51.090326 metaflow-netflixext-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-11 10:10:40.000000 metaflow-netflixext-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.119743 metaflow-netflixext-1.1.3/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44627 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113856 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51887 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40232 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   113678 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/netflixext_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/setup.py
```

### Comparing `metaflow-netflixext-1.1.2/LICENSE` & `metaflow-netflixext-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/PKG-INFO` & `metaflow-netflixext-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 1.1.2
+Version: 1.1.3
 Summary: Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `metaflow-netflixext-1.1.2/README.md` & `metaflow-netflixext-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,22 +322,28 @@
         # We need to install ipykernel into the resolved environment
         obj.echo("    Resolving an environment compatible with Jupyter ...", nl=False)
 
         # We use envsresolver to properly deal with builder environments and what not
         resolver = EnvsResolver(obj.conda)
         # We force the env_type to be the same as the base env since we don't modify that
         # by adding these deps.
+
+        # We also force the use of use_latest because we are not really doing anything
+        # that would require a re-resolve (ie: the user doesn't really care about the
+        # version of ipykernel most likely).
         resolver.add_environment(
             arch_id(),
             user_deps={
                 "pypi" if env.env_type == EnvType.PYPI_ONLY else "conda": ["ipykernel"]
             },
             user_sources={},
             extras={},
             base_env=env,
+            local_only=local_only,
+            use_latest=":any:",
         )
         resolver.resolve_environments(obj.echo)
         update_envs = []  # type: List[ResolvedEnvironment]
         if obj.datastore_type != "local":
             # We may need to update caches
             # Note that it is possible that something we needed to resolve, we don't need
             # to cache (if we resolved to something already cached).
@@ -1003,14 +1009,16 @@
                 )
             elif first_word == "--extra-index-url" and rem:
                 sources.setdefault("pypi", []).append(rem)
             elif first_word in ("-f", "--find-links", "--trusted-host") and rem:
                 extra_args.setdefault("pypi", []).append(" ".join([first_word, rem]))
             elif first_word in ("--pre", "--no-index"):
                 extra_args.setdefault("pypi", []).append(first_word)
+            elif first_word == "--conda-channel" and rem:
+                sources.setdefault("conda", []).append(rem)
             elif first_word == "--conda-pkg":
                 # Special extension to allow non-python conda package specification
                 split_res = REQ_SPLIT_LINE.match(splits[1])
                 if split_res is None:
                     raise InvalidEnvironmentException(
                         "Could not parse conda package '%s'" % splits[1]
                     )
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 CONDA_S3ROOT = from_conf(
     "CONDA_S3ROOT",
     os.path.join(DATASTORE_SYSROOT_S3, "conda_env") if DATASTORE_SYSROOT_S3 else None,
 )
 
 CONDA_AZUREROOT = from_conf(
     "CONDA_AZUREROOT",
-    os.path.join(DATASTORE_SYSROOT_AZURE, "conda_env")
-    if DATASTORE_SYSROOT_AZURE
-    else None,
+    (
+        os.path.join(DATASTORE_SYSROOT_AZURE, "conda_env")
+        if DATASTORE_SYSROOT_AZURE
+        else None
+    ),
 )
 
 CONDA_GSROOT = from_conf(
     "CONDA_GSROOT",
     os.path.join(DATASTORE_SYSROOT_GS, "conda_env") if DATASTORE_SYSROOT_GS else None,
 )
 
 CONDA_LOCALROOT = from_conf(
     "CONDA_LOCALROOT",
-    os.path.join(DATASTORE_SYSROOT_LOCAL, "conda_env")
-    if DATASTORE_SYSROOT_LOCAL
-    else None,
+    (
+        os.path.join(DATASTORE_SYSROOT_LOCAL, "conda_env")
+        if DATASTORE_SYSROOT_LOCAL
+        else None
+    ),
 )
 
 CONDA_MAGIC_FILE_V2 = "conda_v2.cnd"
 
 # Use an alternate dependency resolver for conda packages instead of conda
 # Mamba promises faster package dependency resolution times, which
 # should result in an appreciable speedup in flow environment initialization.
@@ -128,18 +132,27 @@
         "linux-64": {"__glibc": os.environ.get("CONDA_OVERRIDE_GLIBC", "2.27")},
     },
 )
 
 # Packages to add when building for GPU machines (ie: if there is a GPU resource
 # requirement). As an example you can set this to:
 # CONDA_SYS_DEFAULT_GPU_PACKAGES = {
-#     "__cuda": os.environ.get("CONDA_OVERRIDE_CUDA", "11.8")
+#     "__cuda": os.environ.get("CONDA_OVERRIDE_CUDA", "11.8=0")
 # }
 CONDA_SYS_DEFAULT_GPU_PACKAGES = {}
 
+# Packages that are needed when creating an intermediate conda environment to resolve
+# a pypi environment. This can be used to add packages needed for authentication for
+# example.
+builder_packages = []
+if os.environ.get("GOOGLE_APPLICATION_CREDENTIALS"):
+    builder_packages = ["keyrings.google-artifactregistry-auth"]
+
+CONDA_BUILDER_ENV_PACKAGES = from_conf("CONDA_BUILDER_ENV_PACKAGES", builder_packages)
+
 
 def _validate_remote_latest(name, value):
     if not value:
         raise MetaflowException("%s must not be empty." % name)
     if value[0] == ":" and value not in (":none:", ":username:", ":any:"):
         raise MetaflowException(
             "%s can only have special values ':none:', ':username:' or ':any:'" % name
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,18 @@
         return {
             k: v
             for k, v in self._created_envs(prefix).items()
             if k.req_id != "_invalid"
         }
 
     def environment(
-        self, env_id: EnvID, local_only: bool = False
+        self,
+        env_id: EnvID,
+        local_only: bool = False,
+        use_latest: str = CONDA_USE_REMOTE_LATEST,
     ) -> Optional[ResolvedEnvironment]:
         """
         Returns the resolved environment for a given environment ID.
 
         Note that this does not return the instance of the environment (use
         a variant of `created_environment` for that) but instead returns if we know
         how to resolve the environment.
@@ -555,14 +558,19 @@
         Parameters
         ----------
         env_id : EnvID
             Environment ID we are looking for
         local_only : bool, optional
             If True, does not look in the remote cache for resolved environments,
             by default False
+        use_latest : str, default METAFLOW_CONDA_USE_REMOTE_LATEST
+            For default environments, determine if we allow fetching the latest environment
+            remotely resolved. If ":none:", we don't fetch anything. If ":username:", we
+            fetch the latest environment resolved by the current user. If ":any:", we fetch
+            the latest environment resolved by any user.
 
         Returns
         -------
         Optional[ResolvedEnvironment]
             The ResolvedEnvironment corresponding to the input EnvID
         """
         # First look if we have from_env_id locally
@@ -574,29 +582,29 @@
 
         # We never have a "_default" remotely so save time and don't go try to
         # look for one UNLESS the user configured to use the latest as the default
         if not local_only and self._storage:
             if env_id.full_id != "_default":
                 env = self._remote_env_fetch([env_id])
                 env = env[0] if env else None
-            elif CONDA_USE_REMOTE_LATEST != ":none:":
+            elif use_latest != ":none:":
                 # Here we fetch all the environments first and sort them so most
                 # recent (biggest date) is first
                 all_environments = self.environments(env_id.req_id, env_id.arch)
                 current_user = get_username()
-                if CONDA_USE_REMOTE_LATEST == ":username:":
+                if use_latest == ":username:":
                     current_user = cast(str, get_username())
                     filter_func = lambda x: x[1].resolved_by == current_user
-                elif CONDA_USE_REMOTE_LATEST == ":any:":
+                elif use_latest == ":any:":
                     filter_func = lambda x: True
                 else:
                     allowed_usernames = list(
                         map(
                             lambda x: x.strip(),
-                            cast(str, CONDA_USE_REMOTE_LATEST).split(","),
+                            cast(str, use_latest).split(","),
                         )
                     )
                     filter_func = lambda x: x in allowed_usernames
 
                 env = list(
                     filter(
                         filter_func,
@@ -2343,26 +2351,39 @@
         with tempfile.NamedTemporaryFile(
             mode="w", encoding="utf-8", delete=not debug.conda
         ) as explicit_list:
             # We create an explicit file
             lines = ["@EXPLICIT\n"] + explicit_urls
             explicit_list.writelines(lines)
             explicit_list.flush()
-            self.call_binary(
+            args = [
+                "create",
+                "--yes",
+                "--quiet",
+                "--offline",
+                "--no-deps",
+            ]
+            if self._conda_executable_type == "micromamba":
+                # micromamba seems to have a bug when compiling .py files. In some
+                # circumstances, it just hangs forever. We avoid this by not compiling
+                # any file and letting things get compiled lazily. This may have the
+                # added benefit of a faster environment creation.
+                # This option is only available for micromamba so we don't add it
+                # for anything else. This should cover all remote installations though.
+                args.append("--no-pyc")
+            args.extend(
                 [
-                    "create",
-                    "--yes",
-                    "--quiet",
-                    "--offline",
-                    "--no-deps",
                     "--name",
                     env_name,
                     "--file",
                     explicit_list.name,
-                ],
+                ]
+            )
+            self.call_binary(
+                args,
                 # Creating with micromamba is faster as it extracts in parallel. Prefer
                 # it if it exists.
                 binary="micromamba"
                 if self._bins and "micromamba" in self._bins
                 else "conda",
             )
 
@@ -2378,17 +2399,19 @@
                     arg_list = [
                         python_exec,
                         "-m",
                         "pip",
                         "install",
                         "--no-deps",
                         "--no-input",
-                        "-r",
-                        pypi_list.name,
                     ]
+                    if self._conda_executable_type == "micromamba":
+                        # Be consistent with what we install with micromamba
+                        arg_list.append("--no-compile")
+                    arg_list.extend(["-r", pypi_list.name])
                     debug.conda_exec("Pip call: %s" % " ".join(arg_list))
                     subprocess.check_output(arg_list, stderr=subprocess.STDOUT)
                 except subprocess.CalledProcessError as e:
                     print(
                         "Pretty-printed STDOUT:\n%s" % e.output.decode("utf-8")
                         if e.output
                         else "No STDOUT",
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,29 +176,37 @@
         self.conda = Conda(echo, datastore_type)
 
         return self.base_env.validate_environment(echo, datastore_type)
 
     def decospecs(self) -> Tuple[str, ...]:
         return ("conda_env_internal",) + self.base_env.decospecs()
 
-    def bootstrap_commands(self, step_name: str, datastore_type: str) -> List[str]:
+    def bootstrap_commands(
+        self,
+        step_name: str,
+        datastore_type: str,
+        default_executable_path: Optional[str] = None,
+    ) -> List[str]:
         # Bootstrap conda and execution environment for step
         env_id = self.get_env_id_noconda(step_name)
         if env_id is not None:
             if isinstance(env_id, EnvID):
                 arg1 = env_id.req_id
                 arg2 = env_id.full_id
             else:
                 arg1 = env_id
                 arg2 = "_fetch_exec"
             return [
                 "export CONDA_START=$(date +%s)",
                 "echo 'Bootstrapping environment ...'",
-                'python -m %s.remote_bootstrap "%s" "%s" %s %s %s'
+                '%s -m %s.remote_bootstrap "%s" "%s" %s %s %s'
                 % (
+                    "python"
+                    if default_executable_path is None
+                    else default_executable_path,
                     "metaflow_extensions.netflix_ext.plugins.conda",
                     self._flow.name,
                     step_name,
                     arg1,
                     arg2,
                     datastore_type,
                 ),
@@ -545,14 +553,35 @@
             if has_conda and has_pypi:
                 env_type = EnvType.MIXED
             elif has_pypi:
                 env_type = EnvType.PYPI_ONLY
 
             if final_req.python is None:
                 final_req.python = platform.python_version()
+                # HACK to prevent looking for python versions that do not exist on
+                # conda-forge. Only do this for non-user specified version. If the
+                # version is user specified, the user can change it easily.
+                version_maps = {
+                    "3.7.4": "3.7.5",
+                    "3.7.7": "3.7.8",
+                    "3.7.11": "3.7.12",
+                    "3.7.13": "3.7.12",
+                    "3.7.14": "3.7.12",
+                    "3.7.15": "3.7.12",
+                    "3.7.16": "3.7.12",
+                    "3.7.17": "3.7.12",
+                    "3.8.7": "3.8.8",
+                    "3.8.9": "3.8.10",
+                    "3.8.11": "3.8.12",
+                    "3.9.3": "3.9.4",
+                    "3.9.8": "3.9.9",
+                    "3.9.11": "3.9.12",
+                    "3.10.3": "3.10.4",
+                }
+                final_req.python = version_maps.get(final_req.python, final_req.python)
             all_packages.setdefault("conda", {})["python"] = canonicalize_version(
                 final_req.python
             )
 
         # Add pinned dependencies based on env-type; we prefer conda dependencies if
         # env-type is mixed
         if env_type == EnvType.PYPI_ONLY:
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,14 @@
     """
 
     name = "sys_packages"
 
 
 # Here for legacy reason -- use @pypi instead
 class PipRequirementStepDecorator(PypiRequirementStepDecorator):
-    name = "pip"
     """
     Specifies the Pypi packages for the step.
 
     DEPRECATED: please use `@pypi` instead.
 
     Parameters
     ----------
@@ -328,14 +327,16 @@
         specified. This is useful, for example, if you want this step to always use
         the latest named environment when it runs as opposed to the latest when it
         is deployed.
     disabled : bool, default False
         If set to True, uses the external environment.
     """
 
+    name = "pip"
+
     def step_init(
         self,
         flow: FlowSpec,
         graph: FlowGraph,
         step_name: str,
         decorators: List[StepDecorator],
         environment: MetaflowEnvironment,
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1399,9 +1399,13 @@
                 # Not a new file
                 f.seek(0)
                 current_content = CachedEnvironmentInfo.from_dict(json.load(f))
             f.seek(0)
             f.truncate(0)
             current_content.update(info)
             json.dump(current_content.to_dict(), f)
+
+            # Flush data from python file object to OS buffer and eventually to disk.
+            f.flush()
+            os.fsync(f.fileno())
         finally:
             fcntl.flock(f, fcntl.LOCK_UN)
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from metaflow.metaflow_config import (
     CONDA_DEPENDENCY_RESOLVER,
     CONDA_PREFERRED_FORMAT,
     CONDA_MIXED_DEPENDENCY_RESOLVER,
     CONDA_PYPI_DEPENDENCY_RESOLVER,
     CONDA_SYS_DEPENDENCIES,
     CONDA_SYS_DEFAULT_PACKAGES,
+    CONDA_USE_REMOTE_LATEST,
 )
 from metaflow.metaflow_environment import InvalidEnvironmentException
 
 from metaflow._vendor.packaging.version import parse as parse_version
 from .env_descr import (
     EnvID,
     EnvType,
@@ -80,14 +81,15 @@
         user_deps: Dict[str, List[str]],
         user_sources: Dict[str, List[str]],
         extras: Dict[str, List[str]],
         step_name: str = "ad-hoc",
         base_env: Optional[ResolvedEnvironment] = None,
         base_from_full_id: bool = False,
         local_only: bool = False,
+        use_latest: str = CONDA_USE_REMOTE_LATEST,
         force: bool = False,
         force_co_resolve: bool = False,
     ):
         """
         Add an environment to resolve to this EnvsResolver. The EnvsResolver will resolve
         the same environment only once and will mutualize anything it can.
 
@@ -111,14 +113,19 @@
             The base environment, if any, this environment is derived from, by default None
         base_from_full_id : bool, optional
             True if the base environment was extracted using just the full ID of the
             environment which makes it imprecise, by default False
         local_only : bool, optional
             True if we should only look for resolved environments locally and not
             remotely, by default False
+        use_latest : str, default METAFLOW_CONDA_USE_REMOTE_LATEST
+            For default environments, determine if we allow fetching the latest environment
+            remotely resolved. If ":none:", we don't fetch anything. If ":username:", we
+            fetch the latest environment resolved by the current user. If ":any:", we fetch
+            the latest environment resolved by any user.
         force : bool, optional
             True if we should force resolution even if this environment is known,
             by default False
         force_co_resolve : bool, optional
             True if we should force co-resolution, by default False
         """
         self._non_step_envs = True
@@ -151,15 +158,17 @@
             and base_env
             and base_env.env_id.req_id == env_id.req_id
             and base_env.env_id.arch == env_id.arch
         ):
             resolved_env = base_env
         else:
             resolved_env = (
-                self._conda.environment(env_id, local_only) if not force else None
+                self._conda.environment(env_id, local_only, use_latest)
+                if not force
+                else None
             )
 
         # Check if we have already requested this environment
         if env_id not in self._requested_envs:
             if force_co_resolve:
                 if resolved_env is None:
                     # Invalidate any previously resolved environment with the same req_id
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,18 @@
 from .utils import (
     CondaException,
     arch_id,
     auth_from_urls,
     change_pypi_package_version,
     correct_splitext,
     parse_explicit_path_pypi,
+    version_to_str,
 )
 
-_DEV_TRANS = str.maketrans("abcdef", "123456")
+_DEV_TRANS = str.maketrans("abcdef", "012345")
 
 
 # This is a dataclass -- can move to that when we only support 3.7+
 class PackageToBuild:
     def __init__(
         self,
         url: str,
@@ -277,31 +278,39 @@
             # If the source is not an actual URL, we are going to change the name
             # of the package to avoid any potential conflict. We consider that
             # packages derived from internet URLs (so likely a source package)
             # do not need name changes
             if not pkg_spec.is_downloadable_url():
                 pkg_version = parse_wheel_filename(parse_result.filename + ".whl")[1]
 
-                pkg_version_str = str(pkg_version)
-                if not pkg_version.dev:
+                pkg_dev = pkg_version.dev
+                pkg_local = pkg_version.local
+                if not pkg_dev:
                     wheel_hash = PypiPackageSpecification.hash_pkg(wheel_file)
-                    pkg_version_str += ".dev" + wheel_hash[:8].translate(_DEV_TRANS)
-                pkg_version_str += "+mfbuild"
+
+                    pkg_dev = int(wheel_hash[:8].translate(_DEV_TRANS))
+                if pkg_local:
+                    pkg_local += "_mfbuild"
+                else:
+                    pkg_local = "mfbuild"
+                pkg_version_str = version_to_str(
+                    pkg_version, {"dev": pkg_dev, "local": pkg_local}
+                )
                 wheel_file = change_pypi_package_version(
                     builder_python, wheel_file, pkg_version_str
                 )
                 parse_result = parse_explicit_path_pypi("file://%s" % wheel_file)
 
             debug.conda_exec("Package for '%s' built in '%s'" % (key, wheel_file))
 
             # We update because we need to change the filename mostly so that it
             # now reflects the abi, etc and all that goes in a wheel filename.
             pkg_spec = pkg_spec.clone_with_filename(parse_result.filename)
             to_build_pkg_info[key].spec = pkg_spec
-            pkg_spec.add_local_file(".whl", wheel_file)
+            pkg_spec.add_local_file(".whl", wheel_file, pkg_hash=parse_result.hash)
 
         if unsupported_wheel:
             raise CondaException(
                 "Some built pypi packages are not compatible with the target "
                 "architecture. This can happen when some dependencies do not have "
                 "an available wheel for the target architecture and you are resolving "
                 "an environment for a different architecture than the one you are on. "
@@ -318,23 +327,25 @@
     key: str,
     spec: PypiPackageSpecification,
     build_url: str,
 ):
     src = spec.local_file(spec.url_format) or build_url
     debug.conda_exec("%s: building from '%s' in '%s'" % (key, src, dest_path))
 
+    addl_env = {"PATH": os.path.dirname(binary) + ":" + os.environ["PATH"]}
     conda.call_binary(
         [
             "-m",
             "pip",
             "--isolated",
             "wheel",
             "--no-deps",
             "--progress-bar",
             "off",
             "-w",
             dest_path,
             src,
         ],
         binary=binary,
+        addl_env=addl_env,
     )
     return key, dest_path
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 # If arch_id() == architecture, we also use the same virtual packages
                 # as the ones that exist on the machine to mimic the current behavior
                 # of conda/mamba. If not the same architecture, we pass the system
                 # overrides (currently __cuda) down as well.
                 if arch_id() == architecture or sys_overrides:
                     lines = ["subdirs:\n", "  %s:\n" % architecture, "    packages:\n"]
                     lines.extend(
-                        "      %s: %s\n" % (virt_pkg, virt_build_str)
+                        '      %s: "%s"\n' % (virt_pkg, virt_build_str)
                         for virt_pkg, virt_build_str in self._conda.virtual_packages.items()
                         if virt_pkg not in sys_overrides
                     )
                     lines.extend(
                         "      %s: %s\n" % (k, v) for k, v in sys_overrides.items()
                     )
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                 )
         sys_overrides = {k: v for d in deps.get("sys", []) for k, v in [d.split("==")]}
         real_deps = list(chain(deps.get("conda", []), deps.get("npconda", [])))
         packages = []  # type: List[PackageSpecification]
         with tempfile.TemporaryDirectory() as mamba_dir:
             args = [
                 "create",
+                "--yes",
                 "--prefix",
                 os.path.join(mamba_dir, "prefix"),
                 "--dry-run",
             ]
             have_channels = False
             for c in set(sources.get("conda", [])).difference(
                 map(channel_or_url, self._conda.default_conda_channels)
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,18 @@
             )
 
         # Create the environment in which we will call pip
         debug.conda_exec("Creating builder conda environment")
         builder_python = os.path.join(
             self._conda.create_builder_env(builder_env), "bin", "python"
         )
+        # Add the path to the binary dir of the builder environment because
+        # things in there may be needed to build/resolve the environment (one that has
+        # come up is git-lfs)
+        addl_env = {"PATH": os.path.dirname(builder_python) + ":" + os.environ["PATH"]}
 
         packages = []  # type: List[PackageSpecification]
         with tempfile.TemporaryDirectory() as pypi_dir:
             args = [
                 "-m",
                 "pip",
                 "-v",
@@ -251,15 +255,15 @@
                     if splits[1][0] in ("=", "<", ">", "!", "~"):
                         # Something originally like pkg==<=ver
                         args.append("".join(splits))
                     else:
                         # Something originally like pkg==ver
                         args.append(d)
 
-            self._conda.call_binary(args, binary=builder_python)
+            self._conda.call_binary(args, binary=builder_python, addl_env=addl_env)
 
             # We should now have a json blob in out.json
             with open(
                 os.path.join(pypi_dir, "out.json"), mode="r", encoding="utf-8"
             ) as f:
                 desc = json.load(f)
 
@@ -283,14 +287,36 @@
                         k: v
                         for k, v in package_desc.items()
                         if k in ("download_info", "vcs_info", "url", "subdirectory")
                     }
                     debug.conda_exec("Need to install %s" % str(package_desc))
                 dl_info = package_desc["download_info"]
                 url = dl_info["url"]
+                # Extract hash if we have it
+                # We have "archive_info"
+                file_hash = None
+                if "archive_info" in dl_info:
+                    if "hashes" in dl_info["archive_info"]:
+                        hashes = dl_info["archive_info"]["hashes"]
+                        for fmt, val in hashes.items():
+                            if fmt == PypiPackageSpecification.base_hash_name():
+                                file_hash = "%s=%s" % (fmt, val)
+                                break
+                        else:
+                            raise CondaException(
+                                "Cannot find hash '%s' for package at '%s'"
+                                % (
+                                    PypiPackageSpecification.base_hash_name(),
+                                    url,
+                                )
+                            )
+                    else:
+                        # Fallback on older "hash" field
+                        file_hash = dl_info["archive_info"]["hash"]
+
                 if "dir_info" in dl_info or url.startswith("file://"):
                     url = unquote(url)
                     to_build_local_pkg = None  # type: Optional[str]
                     local_path = url[7:]
                     if "dir_info" in dl_info and dl_info["dir_info"].get(
                         "editable", False
                     ):
@@ -304,14 +330,15 @@
                                     [
                                         os.path.join(local_path, "setup.py"),
                                         "-q",
                                         "--name",
                                         "--version",
                                     ],
                                     binary=builder_python,
+                                    addl_env=addl_env,
                                 )
                                 .decode(encoding="utf-8")
                                 .splitlines()
                             )
                         elif os.path.isfile(os.path.join(local_path, "pyproject.toml")):
                             package_name, package_version = (
                                 self._conda.call_binary(
@@ -320,14 +347,15 @@
                                         "import tomli; f = open('%s', mode='rb'); "
                                         "d = tomli.load(f); "
                                         "print(d.get('poetry', d['tool']['poetry'])['name']); "
                                         "print(d.get('poetry', d['tool']['poetry'])['version'])"
                                         % os.path.join(local_path, "pyproject.toml"),
                                     ],
                                     binary=builder_python,
+                                    addl_env=addl_env,
                                 )
                                 .decode(encoding="utf-8")
                                 .splitlines()
                             )
                         else:
                             raise CondaException(
                                 "Local directory '%s' is not supported as it is "
@@ -360,35 +388,46 @@
                                     ),
                                     replace=True,
                                 )
                             else:
                                 debug.conda_exec("Known package already in place")
                             packages.append(pkg_spec)
                         else:
-                            parse_result = parse_explicit_path_pypi(url)
+                            parse_result = parse_explicit_path_pypi(
+                                url,
+                                hash_value=file_hash.split("=")[1]
+                                if file_hash
+                                else None,
+                            )
                             if parse_result.url_format != ".whl":
                                 # This is a source package so we need to build it
                                 to_build_local_pkg = dl_info["url"]
                             else:
                                 package_spec = PypiPackageSpecification(
                                     parse_result.filename,
                                     parse_result.url,
                                     is_real_url=False,
                                     url_format=parse_result.url_format,
                                 )
                                 # We extract the actual local file so we can use that for now
                                 # Note that the url in PypiPackageSpecication is a fake
-                                # one that looks like file://local-file/... which is meant
+                                # one that looks like file://local-<hash>/... which is meant
                                 # to act as a key for the package.
                                 package_spec.add_local_file(
                                     parse_result.url_format, url[7:]
                                 )
                                 packages.append(package_spec)
                     if to_build_local_pkg:
-                        parse_result = parse_explicit_path_pypi(to_build_local_pkg)
+                        # Note the hash value here is the hash of the *source* tarball
+                        # This is fine as it still uniquely identifies the package
+                        # we will be building.
+                        parse_result = parse_explicit_path_pypi(
+                            to_build_local_pkg,
+                            hash_value=file_hash.split("=")[1] if file_hash else None,
+                        )
                         cache_base_url = PypiCachePackage.make_partial_cache_url(
                             parse_result.url, is_real_url=False
                         )
 
                         to_build_pkg_info[cache_base_url] = PackageToBuild(
                             dl_info["url"],
                             # We get the name once we build the package
@@ -432,50 +471,27 @@
                             _FAKE_WHEEL,
                             base_pkg_url,
                             is_real_url=False,
                             url_format=".whl",
                         ),
                     )
                 else:
-                    # We have "archive_info"
-                    if "hashes" in dl_info["archive_info"]:
-                        hashes = dl_info["archive_info"]["hashes"]
-                        for fmt, val in hashes.items():
-                            if fmt == PypiPackageSpecification.base_hash_name():
-                                hash = "%s=%s" % (fmt, val)
-                                break
-                        else:
-                            raise CondaException(
-                                "Cannot find hash '%s' for package at '%s'"
-                                % (
-                                    PypiPackageSpecification.base_hash_name(),
-                                    url,
-                                )
-                            )
-                    else:
-                        # Fallback on older "hash" field
-                        hash = dl_info["archive_info"]["hash"]
-
-                    parse_result = parse_explicit_url_pypi("%s#%s" % (url, hash))
+                    # Here we have archive_info
+                    parse_result = parse_explicit_url_pypi("%s#%s" % (url, file_hash))
                     if parse_result.url_format != ".whl":
                         # We need to build non wheel files.
                         url_parse_result = urlparse(cast(str, dl_info["url"]))
 
                         is_real_url = False
                         if url_parse_result.scheme == "file":
-                            # TODO: Not sure if this case happens.
-                            parse_result = parse_explicit_path_pypi(dl_info["url"])
-                            cache_base_url = PypiCachePackage.make_partial_cache_url(
-                                parse_result.url, is_real_url=False
+                            raise CondaException(
+                                "URL %s should have been identified as a local file"
+                                % dl_info["url"]
                             )
                         else:
-                            # We don't have the hash so we ignore.
-                            parse_result = parse_explicit_url_pypi(
-                                "%s#" % dl_info["url"]
-                            )
                             cache_base_url = PypiCachePackage.make_partial_cache_url(
                                 parse_result.url, is_real_url=True
                             )
                             is_real_url = True
 
                         spec = PypiPackageSpecification(
                             parse_result.filename,
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
 from __future__ import annotations
 
 import email.parser
 import email.policy
+import hashlib
 import os
 import platform
 import re
 import shutil
 import subprocess
 import tempfile
-import uuid
 
 from enum import Enum
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
+    Any,
     Dict,
     FrozenSet,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
@@ -38,19 +39,22 @@
     mac_platforms,
     Tag,
 )
 
 from metaflow._vendor.packaging.utils import BuildTag, parse_wheel_filename
 
 from metaflow._vendor.packaging.version import Version
+from metaflow._vendor.packaging.requirements import Requirement
+from metaflow._vendor.packaging.specifiers import SpecifierSet
 
 from metaflow.debug import debug
 from metaflow.exception import MetaflowException
 import metaflow.metaflow_config as mf_config
 from metaflow.metaflow_config import (
+    CONDA_BUILDER_ENV_PACKAGES,  # type: ignore
     CONDA_MAGIC_FILE_V2,  # type: ignore
     CONDA_PREFERRED_FORMAT,  # type: ignore
     CONDA_SRCS_AUTH_INFO,  # type: ignore
     CONDA_SYS_DEPENDENCIES,  # type: ignore
     CONDA_SYS_DEFAULT_PACKAGES,  # type: ignore
     CONDA_SYS_DEFAULT_GPU_PACKAGES,  # type: ignore
 )
@@ -66,15 +70,19 @@
 _ALL_CONDA_FORMATS = (".tar.bz2", ".conda")
 # NOTE: Order is important as it is a preference order
 _ALL_PYPI_FORMATS = (".whl", ".tar.gz", ".zip")
 _VALID_IMAGE_NAME = "[^-a-z0-9_/]"
 _VALID_TAG_NAME = "[^-a-z0-9_]"
 
 # Things that need to be put in any of the builder environments
-_BUILDER_ENVS_PACKAGES = ("pip", "wheel", "tomli", "setuptools")
+# HACK: Workaround bad wheel package in conda-forge
+# See: https://github.com/conda-forge/wheel-feedstock/issues/61
+# We could check the version of python but it was hard to do in all cases
+# since we don't have the full version so just pin to 0.42.0 for now
+_BUILDER_ENVS_PACKAGES = ("pip", "wheel==0.42.0", "tomli", "setuptools")
 
 
 class AliasType(Enum):
     PATHSPEC = "pathspec"
     FULL_ID = "full-id"
     REQ_FULL_ID = "both-id"
     GENERIC = "generic"
@@ -107,19 +115,31 @@
         msg = "Step(s): {steps}, Error: {error}".format(
             steps=steps, error=exception.message
         )
         super(CondaStepException, self).__init__(msg)
 
 
 def get_builder_envs_dep(orig_deps: List[str]) -> List[str]:
-    builder_deps = []  # type: List[str]
-    for pkg in _BUILDER_ENVS_PACKAGES:
-        dep = [d for d in orig_deps if d.startswith("%s==" % pkg)]
-        builder_deps.extend(dep or [pkg])
-    return builder_deps
+    builder_packages = {}  # type: Dict[str, SpecifierSet]
+    for pkg_req in chain(_BUILDER_ENVS_PACKAGES, CONDA_BUILDER_ENV_PACKAGES):
+        r = Requirement(pkg_req)
+        builder_packages[r.name] = (
+            builder_packages.setdefault(r.name, SpecifierSet()) & r.specifier
+        )
+    for d in orig_deps:
+        splits = d.split("==", 1)
+        if len(splits) == 2 and splits[0] in builder_packages:
+            # If it is just the package name, we don't care because no other specification
+            builder_packages[splits[0]] = builder_packages[splits[0]] & SpecifierSet(
+                splits[1]
+            )
+    return [
+        "%s==%s" % (k, str(v).lstrip("=")) if v else k
+        for k, v in builder_packages.items()
+    ]
 
 
 def convert_filepath(path: str, file_format: Optional[str] = None) -> Tuple[str, str]:
     if file_format and not path.endswith(file_format):
         path, cur_ext = correct_splitext(path)
         if cur_ext not in _ALL_CONDA_FORMATS:
             raise ValueError(
@@ -174,15 +194,15 @@
     # The goal of this function is to take the list of virtual_packages and to return
     # the sys packages we need to add to the user dependencies (so packages that start with
     # sys::). The reason for having them as part of user packages is that we can then
     # use them in computing the user request hash (since these will impact the packages
     # that are installed). The sys:: packages will then be properly added when resolving
     # the environment as virtual packages (either through CONDA_OVERRIDE_XXX or directly
     # as part of a virtual_packages.yml for conda-lock)
-    if virtual_packages:
+    if virtual_packages and arch_requested == arch_id():
         result = dict(virtual_packages)
     else:
         result = dict(CONDA_SYS_DEFAULT_PACKAGES.get(arch_requested, {}))
 
     if gpu_requested:
         result.update(CONDA_SYS_DEFAULT_GPU_PACKAGES)
 
@@ -288,34 +308,52 @@
         )
     filename = unquote(filename)
     return ParseExplicitResult(
         filename=filename, url=url_clean, url_format=url_format, hash=url_hash
     )
 
 
-def parse_explicit_path_pypi(path: str) -> ParseExplicitResult:
+def parse_explicit_path_pypi(
+    path: str, hash_value: Optional[str] = None
+) -> ParseExplicitResult:
+    # Prevent circular import
+    from .env_descr import PypiPackageSpecification
+
     # Takes a filename in the form file://<path> and returns:
     #  - the filename
-    #  - the URL (always file://local-<uuid>/<filename> so there is no way another
+    #  - the URL (always file://local-<hash>/<filename> so there is no way another
     #    build/user conflicts. We consider them to be all distinct.
     #  - the format of the URL
     #  - the hash will be set to None
     if not path.startswith("file://"):
         raise CondaException("Local path '%s' does not start with file://" % path)
     path = path[7:]
     orig_filename, url_format = correct_splitext(os.path.basename(path))
     if url_format not in _ALL_PYPI_FORMATS:
         raise CondaException(
             "Path '%s' is not a supported format (%s)" % (path, str(_ALL_PYPI_FORMATS))
         )
+    if hash_value is None:
+        if not os.path.isfile(path):
+            # This is not a file so we can't get a hash. Instead, we will compute
+            # the last modified time for files within the directory containing it. This only happens
+            # when the user has a local directory and is trying to build a package
+            # from there. The modified time will act a bit like a hash to determine
+            # if the package being built has changed. If it has, the hash will be different
+            # and the "fake URL" will be different so we won't find the package
+            # in the cache. If it hasn't changed, the hash will be the same and we will
+            # avoid randomly rebuilding the package.
+            hash_value = hash_directory(os.path.dirname(path))
+        else:
+            hash_value = PypiPackageSpecification.hash_pkg(path)
     return ParseExplicitResult(
         filename=unquote(orig_filename),
-        url="file://local-%s/%s" % (str(uuid.uuid4()), orig_filename),
+        url="file://local-%s/%s" % (hash_value, orig_filename),
         url_format=url_format,
-        hash=None,
+        hash=hash_value,
     )
 
 
 def parse_explicit_url_pypi(url: str) -> ParseExplicitResult:
     # Takes a URL in the form url#hash and returns:
     #  - the filename
     #  - the URL (without the hash)
@@ -568,14 +606,51 @@
             )
             auth_provider = self._my_auths.get(h or "<none>")
             if auth_provider:
                 return auth_provider(r)
         return r
 
 
+def version_to_str(v: Version, overrides: Dict[str, Any]) -> str:
+    # This code copies __str__ from Version basically but allows components to be
+    # changed
+    parts = []  # type: List[str]
+
+    # Epoch
+    val = int(overrides.get("epoch", v.epoch))
+    if v != 0:
+        parts.append(f"{val}!")
+
+    # Release segment
+    val = overrides.get("release", v.release)
+    parts.append(".".join(str(x) for x in val))
+
+    # Pre-release
+    val = overrides.get("pre", v.pre)
+    if val is not None:
+        parts.append("".join(str(x) for x in val))
+
+    # Post-release
+    val = overrides.get("post", v.post)
+    if val is not None:
+        parts.append(f".post{val}")
+
+    # Development release
+    val = overrides.get("dev", v.dev)
+    if val is not None:
+        parts.append(f".dev{val}")
+
+    # Local version segment
+    val = overrides.get("local", v.local)
+    if val is not None:
+        parts.append(f"+{val}")
+
+    return "".join(parts)
+
+
 # Function heavily inspired from https://github.com/hauntsaninja/change_wheel_version
 # MIT license of that source file:
 # MIT License
 
 # Copyright (c) 2023 hauntsaninja
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -686,14 +761,53 @@
             return os.path.join(base_dir, expected_name)
         raise RuntimeError(
             "Could not rename wheel '%s'; expected '%s' got: %s"
             % (wheel_path, expected_name, ", ".join(os.listdir(build_dir)))
         )
 
 
+def hash_directory(path: str) -> str:
+    # The "hash" of a directory will be the last modified time and last modified
+    # file. We could just use the time probably but this will hopefully inject
+    # even more safety.
+    last_modified_time = 0
+    last_modified_file = None  # type: Optional[str]
+
+    # Walk through all files and directories in the root directory
+    top_level = True
+    for directory, dirs, files in os.walk(path):
+        if top_level:
+            # Skip build and .egg-info since we don't want them to affect the
+            # last modified file (it's not source)
+            to_remove = []  # type: List[str]
+            for d in dirs:
+                if d == "build":
+                    to_remove.append(d)
+                if d.endswith(".egg-info"):
+                    to_remove.append(d)
+            for d in to_remove:
+                dirs.remove(d)
+            top_level = False
+
+        for file in files:
+            filename = os.path.join(directory, file)
+            mod_time = os.path.getmtime(filename)
+            # If this file is the most recently modified, update max_mod_time and max_file_dir
+            if mod_time > last_modified_time:
+                last_modified_time, last_modified_file = mod_time, filename
+
+    debug.conda_exec(
+        "Last modified file in '%s': '%s' at %s"
+        % (path, last_modified_file, last_modified_time)
+    )
+    return hashlib.sha256(
+        ("%s:%s" % (last_modified_time, last_modified_file)).encode()
+    ).hexdigest()
+
+
 class WithDir:
     # WARNING: os.chdir is not compatible with thread processing so do not use in
     # a context where multiple threads can exist.
     def __init__(self, new_dir: str):
         self._current_dir = os.getcwd()
         self._new_dir = new_dir
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py` & `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 1.1.2
+Version: 1.1.3
 Summary: Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `metaflow-netflixext-1.1.2/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.2/setup.py` & `metaflow-netflixext-1.1.3/setup.py`

 * *Files identical despite different names*

