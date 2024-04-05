# Comparing `tmp/mov-cli-files-1.0.0.tar.gz` & `tmp/mov-cli-files-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-files-1.0.0.tar", last modified: Fri Apr  5 05:42:54 2024, max compression
+gzip compressed data, was "mov-cli-files-1.0.1.tar", last modified: Fri Apr  5 05:59:33 2024, max compression
```

## Comparing `mov-cli-files-1.0.0.tar` & `mov-cli-files-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 05:42:54.530950 mov-cli-files-1.0.0/
--rw-rw-rw-   0        0        0     1085 2024-04-05 05:34:53.000000 mov-cli-files-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2857 2024-04-05 05:42:54.529950 mov-cli-files-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-04-05 05:39:45.000000 mov-cli-files-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 05:42:54.496943 mov-cli-files-1.0.0/mov_cli_files/
--rw-rw-rw-   0        0        0      351 2024-04-05 05:37:19.000000 mov-cli-files-1.0.0/mov_cli_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:42:54.525951 mov-cli-files-1.0.0/mov_cli_files/files/
--rw-rw-rw-   0        0        0       22 2024-03-21 12:20:57.000000 mov-cli-files-1.0.0/mov_cli_files/files/__init__.py
--rw-rw-rw-   0        0        0     2236 2024-04-05 05:36:59.000000 mov-cli-files-1.0.0/mov_cli_files/files/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:42:54.527949 mov-cli-files-1.0.0/mov_cli_files.egg-info/
--rw-rw-rw-   0        0        0     2857 2024-04-05 05:42:54.000000 mov-cli-files-1.0.0/mov_cli_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-05 05:42:54.000000 mov-cli-files-1.0.0/mov_cli_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 05:42:54.000000 mov-cli-files-1.0.0/mov_cli_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-05 05:42:54.000000 mov-cli-files-1.0.0/mov_cli_files.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 05:42:54.000000 mov-cli-files-1.0.0/mov_cli_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1377 2024-04-05 05:41:14.000000 mov-cli-files-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 05:42:54.531950 mov-cli-files-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.371242 mov-cli-files-1.0.1/
+-rw-rw-rw-   0        0        0     1085 2024-04-05 05:34:53.000000 mov-cli-files-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2970 2024-04-05 05:59:33.369243 mov-cli-files-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-05 05:55:40.000000 mov-cli-files-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.354238 mov-cli-files-1.0.1/mov_cli_files/
+-rw-rw-rw-   0        0        0      351 2024-04-05 05:54:56.000000 mov-cli-files-1.0.1/mov_cli_files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.366241 mov-cli-files-1.0.1/mov_cli_files/files/
+-rw-rw-rw-   0        0        0       22 2024-03-21 12:20:57.000000 mov-cli-files-1.0.1/mov_cli_files/files/__init__.py
+-rw-rw-rw-   0        0        0     2688 2024-04-05 05:58:46.000000 mov-cli-files-1.0.1/mov_cli_files/files/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 05:59:33.368241 mov-cli-files-1.0.1/mov_cli_files.egg-info/
+-rw-rw-rw-   0        0        0     2970 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-05 05:59:33.000000 mov-cli-files-1.0.1/mov_cli_files.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1377 2024-04-05 05:41:14.000000 mov-cli-files-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 05:59:33.371242 mov-cli-files-1.0.1/setup.cfg
```

### Comparing `mov-cli-files-1.0.0/LICENSE` & `mov-cli-files-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-files-1.0.0/PKG-INFO` & `mov-cli-files-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.0.0
+Version: 1.0.1
 Summary:  A mov-cli v4 plugin for watching files on your device.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,16 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-files 
   <sub>A mov-cli v4 plugin for watching files on your device.</sub>
+  
+  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
 
 </div>
 
 
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
```

### Comparing `mov-cli-files-1.0.0/mov_cli_files.egg-info/PKG-INFO` & `mov-cli-files-1.0.1/mov_cli_files.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.0.0
+Version: 1.0.1
 Summary:  A mov-cli v4 plugin for watching files on your device.
 Author-email: Ananas <ananas@r3tr0ananas.lol>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,16 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-files 
   <sub>A mov-cli v4 plugin for watching files on your device.</sub>
+  
+  ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
 
 </div>
 
 
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
```

### Comparing `mov-cli-files-1.0.0/pyproject.toml` & `mov-cli-files-1.0.1/pyproject.toml`

 * *Files identical despite different names*

