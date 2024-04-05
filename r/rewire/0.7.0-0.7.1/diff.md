# Comparing `tmp/rewire-0.7.0.tar.gz` & `tmp/rewire-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-0.7.0.tar", last modified: Sun Feb  4 02:46:36 2024, max compression
+gzip compressed data, was "rewire-0.7.1.tar", last modified: Fri Apr  5 14:58:31 2024, max compression
```

## Comparing `rewire-0.7.0.tar` & `rewire-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-04 02:46:36.972356 rewire-0.7.0/
--rw-rw-rw-   0        0        0     1086 2024-01-31 22:20:56.000000 rewire-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     3988 2024-02-04 02:46:36.972356 rewire-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2024-02-03 05:30:07.000000 rewire-0.7.0/README.md
--rw-rw-rw-   0        0        0      871 2024-02-04 02:45:50.000000 rewire-0.7.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-04 02:46:36.958353 rewire-0.7.0/rewire/
--rw-rw-rw-   0        0        0      350 2024-02-01 21:29:32.000000 rewire-0.7.0/rewire/__init__.py
--rw-rw-rw-   0        0        0      270 2024-01-23 02:13:31.000000 rewire-0.7.0/rewire/classproperty.py
--rw-rw-rw-   0        0        0    11572 2024-02-04 00:24:54.000000 rewire-0.7.0/rewire/config.py
--rw-rw-rw-   0        0        0     2023 2024-01-23 02:08:59.000000 rewire-0.7.0/rewire/context.py
--rw-rw-rw-   0        0        0    11802 2024-02-04 00:27:35.000000 rewire-0.7.0/rewire/dependencies.py
--rw-rw-rw-   0        0        0     4911 2024-02-04 02:42:07.000000 rewire-0.7.0/rewire/lifecycle.py
--rw-rw-rw-   0        0        0     1577 2024-02-01 21:01:39.000000 rewire-0.7.0/rewire/loader.py
--rw-rw-rw-   0        0        0     4649 2024-02-01 21:19:41.000000 rewire-0.7.0/rewire/log.py
--rw-rw-rw-   0        0        0     5583 2024-02-04 00:29:24.000000 rewire-0.7.0/rewire/plugins.py
--rw-rw-rw-   0        0        0     3222 2024-01-31 22:22:27.000000 rewire-0.7.0/rewire/space.py
--rw-rw-rw-   0        0        0      616 2024-01-31 22:22:27.000000 rewire-0.7.0/rewire/store.py
-drwxrwxrwx   0        0        0        0 2024-02-04 02:46:36.971356 rewire-0.7.0/rewire.egg-info/
--rw-rw-rw-   0        0        0     3988 2024-02-04 02:46:36.000000 rewire-0.7.0/rewire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-02-04 02:46:36.000000 rewire-0.7.0/rewire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-04 02:46:36.000000 rewire-0.7.0/rewire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-02-04 02:46:36.000000 rewire-0.7.0/rewire.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-04 02:46:36.000000 rewire-0.7.0/rewire.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-04 02:46:36.973357 rewire-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.740458 rewire-0.7.1/
+-rw-rw-rw-   0        0        0     1086 2024-01-31 22:20:56.000000 rewire-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4011 2024-04-05 14:58:31.739460 rewire-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2024-02-04 02:48:58.000000 rewire-0.7.1/README.md
+-rw-rw-rw-   0        0        0      871 2024-04-05 14:57:31.000000 rewire-0.7.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.725434 rewire-0.7.1/rewire/
+-rw-rw-rw-   0        0        0      350 2024-02-01 21:29:32.000000 rewire-0.7.1/rewire/__init__.py
+-rw-rw-rw-   0        0        0      270 2024-01-23 02:13:31.000000 rewire-0.7.1/rewire/classproperty.py
+-rw-rw-rw-   0        0        0    11572 2024-02-04 00:24:54.000000 rewire-0.7.1/rewire/config.py
+-rw-rw-rw-   0        0        0     2023 2024-01-23 02:08:59.000000 rewire-0.7.1/rewire/context.py
+-rw-rw-rw-   0        0        0    11802 2024-02-04 00:27:35.000000 rewire-0.7.1/rewire/dependencies.py
+-rw-rw-rw-   0        0        0     4911 2024-02-04 02:42:07.000000 rewire-0.7.1/rewire/lifecycle.py
+-rw-rw-rw-   0        0        0     1577 2024-02-01 21:01:39.000000 rewire-0.7.1/rewire/loader.py
+-rw-rw-rw-   0        0        0     4659 2024-02-19 04:03:12.000000 rewire-0.7.1/rewire/log.py
+-rw-rw-rw-   0        0        0     5583 2024-02-04 00:29:24.000000 rewire-0.7.1/rewire/plugins.py
+-rw-rw-rw-   0        0        0     3222 2024-01-31 22:22:27.000000 rewire-0.7.1/rewire/space.py
+-rw-rw-rw-   0        0        0      616 2024-01-31 22:22:27.000000 rewire-0.7.1/rewire/store.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:58:31.738458 rewire-0.7.1/rewire.egg-info/
+-rw-rw-rw-   0        0        0     4011 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 14:58:31.000000 rewire-0.7.1/rewire.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:58:31.740458 rewire-0.7.1/setup.cfg
```

### Comparing `rewire-0.7.0/LICENSE` & `rewire-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/PKG-INFO` & `rewire-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Streamlined Type-Based Dependency Injection Framework
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,15 @@
 while maintaining flexibility.
 
 ### Automatic File Import
 
 Automatically import required files based on defined configurations within your Rewire-powered application. Keep your project organized by trusting Rewire to handle file imports, promoting code
 reusability and minimizing potential errors.
 
-### Lifecycle Manager
+### [Lifecycle Manager](./docs/lifecycle.md)
 
 Easily manage the lifecycles of components with Rewire's robust start/stop manager. Control the initialization and disposal of resources efficiently, ensuring optimal resource usage.
 
 ### Extensibility & Hackability
 
 Rewire is designed to be both extensible and hackable, enabling developers to tailor the framework to their specific needs. Customize components, add new features, or integrate Rewire with other
 libraries as desired, making it a powerful choice for any project.
```

### Comparing `rewire-0.7.0/README.md` & `rewire-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 while maintaining flexibility.
 
 ### Automatic File Import
 
 Automatically import required files based on defined configurations within your Rewire-powered application. Keep your project organized by trusting Rewire to handle file imports, promoting code
 reusability and minimizing potential errors.
 
-### Lifecycle Manager
+### [Lifecycle Manager](./docs/lifecycle.md)
 
 Easily manage the lifecycles of components with Rewire's robust start/stop manager. Control the initialization and disposal of resources efficiently, ensuring optimal resource usage.
 
 ### Extensibility & Hackability
 
 Rewire is designed to be both extensible and hackable, enabling developers to tailor the framework to their specific needs. Customize components, add new features, or integrate Rewire with other
 libraries as desired, making it a powerful choice for any project.
```

### Comparing `rewire-0.7.0/pyproject.toml` & `rewire-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire"
-version = "0.7.0"
+version = "0.7.1"
 description = "A Streamlined Type-Based Dependency Injection Framework"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-0.7.0/rewire/config.py` & `rewire-0.7.1/rewire/config.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/context.py` & `rewire-0.7.1/rewire/context.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/dependencies.py` & `rewire-0.7.1/rewire/dependencies.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/lifecycle.py` & `rewire-0.7.1/rewire/lifecycle.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/loader.py` & `rewire-0.7.1/rewire/loader.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/log.py` & `rewire-0.7.1/rewire/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,19 +103,19 @@
     def get_sink(self):
         return sys.stdout
 
 
 def log_print(
     *values: object,
     sep: str = " ",
-    end: Optional[str] = "",
+    end: Optional[str] = None,
     **kw,
 ):
     if kw:
-        return print_(*values, sep, end if isinstance(end, str) else "\n", **kw)
+        return print_(*values, sep=sep, end=end if isinstance(end, str) else "\n", **kw)
     warnings.warn("print is deprecated, use logger.debug instead", stacklevel=2)
     data = f"{sep.join(map(str, values))}{end if isinstance(end, str) else ''}"
     logger.opt(depth=1).debug(data)
 
 
 def showwarning(
     message: Warning | str,
```

### Comparing `rewire-0.7.0/rewire/plugins.py` & `rewire-0.7.1/rewire/plugins.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/space.py` & `rewire-0.7.1/rewire/space.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire/store.py` & `rewire-0.7.1/rewire/store.py`

 * *Files identical despite different names*

### Comparing `rewire-0.7.0/rewire.egg-info/PKG-INFO` & `rewire-0.7.1/rewire.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Streamlined Type-Based Dependency Injection Framework
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,15 @@
 while maintaining flexibility.
 
 ### Automatic File Import
 
 Automatically import required files based on defined configurations within your Rewire-powered application. Keep your project organized by trusting Rewire to handle file imports, promoting code
 reusability and minimizing potential errors.
 
-### Lifecycle Manager
+### [Lifecycle Manager](./docs/lifecycle.md)
 
 Easily manage the lifecycles of components with Rewire's robust start/stop manager. Control the initialization and disposal of resources efficiently, ensuring optimal resource usage.
 
 ### Extensibility & Hackability
 
 Rewire is designed to be both extensible and hackable, enabling developers to tailor the framework to their specific needs. Customize components, add new features, or integrate Rewire with other
 libraries as desired, making it a powerful choice for any project.
```

