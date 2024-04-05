# Comparing `tmp/diamondpack-1.4.1.tar.gz` & `tmp/diamondpack-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamondpack-1.4.1.tar", last modified: Thu Dec 28 15:28:26 2023, max compression
+gzip compressed data, was "diamondpack-1.4.5.tar", last modified: Fri Apr  5 18:34:12 2024, max compression
```

## Comparing `diamondpack-1.4.1.tar` & `diamondpack-1.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-12-28 15:28:26.381354 diamondpack-1.4.1/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1079 2023-12-20 21:28:30.000000 diamondpack-1.4.1/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       35 2023-12-12 05:21:09.000000 diamondpack-1.4.1/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3987 2023-12-28 15:28:26.381354 diamondpack-1.4.1/PKG-INFO
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1879 2023-12-24 02:49:12.000000 diamondpack-1.4.1/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-12-28 15:28:26.374688 diamondpack-1.4.1/diamondpack/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-12-11 19:18:04.000000 diamondpack-1.4.1/diamondpack/__init__.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3071 2023-12-28 15:28:05.000000 diamondpack-1.4.1/diamondpack/__main__.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-12-28 15:28:26.378021 diamondpack-1.4.1/diamondpack/app-templates/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      200 2023-12-20 04:43:55.000000 diamondpack-1.4.1/diamondpack/app-templates/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      182 2023-12-20 20:42:17.000000 diamondpack-1.4.1/diamondpack/app-templates/app.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3246 2023-12-28 15:28:05.000000 diamondpack-1.4.1/diamondpack/app-templates/app.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      221 2023-12-20 05:18:32.000000 diamondpack-1.4.1/diamondpack/app-templates/app.sh
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1644 2023-12-20 21:34:00.000000 diamondpack-1.4.1/diamondpack/app-templates/diamondpack-license.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1243 2023-12-24 02:43:41.000000 diamondpack-1.4.1/diamondpack/dpconfig.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      513 2023-12-28 15:28:05.000000 diamondpack-1.4.1/diamondpack/dplog.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9033 2023-12-28 14:58:19.000000 diamondpack-1.4.1/diamondpack/pack.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-12-28 15:28:26.381354 diamondpack-1.4.1/diamondpack.egg-info/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3987 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/PKG-INFO
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      561 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/SOURCES.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        1 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/dependency_links.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       58 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/entry_points.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       79 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/requires.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       12 2023-12-28 15:28:26.000000 diamondpack-1.4.1/diamondpack.egg-info/top_level.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1084 2023-12-28 15:28:05.000000 diamondpack-1.4.1/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2023-12-28 15:28:26.381354 diamondpack-1.4.1/setup.cfg
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-04-05 18:34:12.344302 diamondpack-1.4.5/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1079 2023-12-20 21:28:30.000000 diamondpack-1.4.5/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       35 2023-12-12 05:21:09.000000 diamondpack-1.4.5/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4707 2024-04-05 18:34:12.344302 diamondpack-1.4.5/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2599 2024-04-05 18:32:20.000000 diamondpack-1.4.5/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-04-05 18:34:12.344302 diamondpack-1.4.5/diamondpack/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-12-11 19:18:04.000000 diamondpack-1.4.5/diamondpack/__init__.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4369 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/__main__.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-04-05 18:34:12.344302 diamondpack-1.4.5/diamondpack/app-templates/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      350 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/app-templates/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      134 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/app-templates/app.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3488 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/app-templates/app.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      217 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/app-templates/app.sh
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1644 2024-04-05 18:31:19.000000 diamondpack-1.4.5/diamondpack/app-templates/diamondpack-license.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1580 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/config.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      513 2023-12-28 15:28:05.000000 diamondpack-1.4.5/diamondpack/log.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12502 2024-04-05 18:30:18.000000 diamondpack-1.4.5/diamondpack/pack.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-04-05 18:34:12.344302 diamondpack-1.4.5/diamondpack.egg-info/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4707 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      557 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/SOURCES.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        1 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/dependency_links.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       58 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/entry_points.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       79 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/requires.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       12 2024-04-05 18:34:12.000000 diamondpack-1.4.5/diamondpack.egg-info/top_level.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1084 2024-04-05 15:07:29.000000 diamondpack-1.4.5/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2024-04-05 18:34:12.344302 diamondpack-1.4.5/setup.cfg
```

### Comparing `diamondpack-1.4.1/LICENSE` & `diamondpack-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `diamondpack-1.4.1/PKG-INFO` & `diamondpack-1.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondpack
-Version: 1.4.1
+Version: 1.4.5
 Summary: A simple packager for creating distributable python applications
 Author: Alagyn
 License: MIT License
         
         Copyright (c) 2023 Ben "Alagyn" Kimbrough
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,22 +70,45 @@
 `pip install diamondpack[app]`
 or
 `pip install cmake`
 
 ## Usage:
 
 ### 1. Configure DiamondPack via your `pyproject.toml`
+
 ```toml
 [project.scripts]
 # Each script named here will generate a new executable
 myScript = "examplePackage.myScript:main"
 
 [tool.diamondpack]
 mode = "app"
+
+# Prevents specific installed packages from being reduced to only .pyc files
+# Some packages complaing about this. This is a list of the MODULE's name, same as it is imported as
+# NOT the pip package name
+py-cache-blacklist = ["opencv"]
+
+# Prevents specific stdlib packages from being copied to reduce package size
+stdlib-blacklist = ["email", "turtle", "unittest"]
+
+# Flag to copy required tk/tcl files
+include-tk = false
+
+# Additional data files can be copied into your distribution like this
+# File globs are copied to the specified path in the dist.
+data-globs = [
+    ["myData/img*.jpg", "destinationDir"],
+    ["myData/data.dat", "data"]
+]
+
+# Enable some additional logging for the "app" mode
+debug-logs = true
 ```
+
 Mode can be `app` or `script`:
 - `app` will generate a compiled executable (requires CMake and a compiler installed)
 - `script` will generate a bash (Linux) or batch (Windows) script
 
 
 ### 2. Build your application into a wheel
 `python -m build --wheel`
```

### Comparing `diamondpack-1.4.1/README.md` & `diamondpack-1.4.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,45 @@
 `pip install diamondpack[app]`
 or
 `pip install cmake`
 
 ## Usage:
 
 ### 1. Configure DiamondPack via your `pyproject.toml`
+
 ```toml
 [project.scripts]
 # Each script named here will generate a new executable
 myScript = "examplePackage.myScript:main"
 
 [tool.diamondpack]
 mode = "app"
+
+# Prevents specific installed packages from being reduced to only .pyc files
+# Some packages complaing about this. This is a list of the MODULE's name, same as it is imported as
+# NOT the pip package name
+py-cache-blacklist = ["opencv"]
+
+# Prevents specific stdlib packages from being copied to reduce package size
+stdlib-blacklist = ["email", "turtle", "unittest"]
+
+# Flag to copy required tk/tcl files
+include-tk = false
+
+# Additional data files can be copied into your distribution like this
+# File globs are copied to the specified path in the dist.
+data-globs = [
+    ["myData/img*.jpg", "destinationDir"],
+    ["myData/data.dat", "data"]
+]
+
+# Enable some additional logging for the "app" mode
+debug-logs = true
 ```
+
 Mode can be `app` or `script`:
 - `app` will generate a compiled executable (requires CMake and a compiler installed)
 - `script` will generate a bash (Linux) or batch (Windows) script
 
 
 ### 2. Build your application into a wheel
 `python -m build --wheel`
```

### Comparing `diamondpack-1.4.1/diamondpack/__main__.py` & `diamondpack-1.4.5/diamondpack/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,41 +4,59 @@
 from typing import Optional
 import re
 import glob
 
 if sys.version_info.major == 3 and sys.version_info.minor < 11:
     import tomli  # type: ignore
 else:
-    import tomllib as tomli # type: ignore
+    import tomllib as tomli  # type: ignore
 
-from diamondpack.dpconfig import DPConfig, DPMode, DPScript
+from diamondpack.config import PackConfig, DPMode, App
 from diamondpack.pack import DiamondPacker
-from diamondpack.dplog import logErr, log
+from diamondpack.log import logErr, log
 
-VERSION = "1.4.1"
+VERSION = "1.4.5"
 
 PROJECT_FILE = "pyproject.toml"
 
 SCRIPT_RE = re.compile(r'((?P<name>[^=]+)=)?(?P<path>[^:]+)(:(?P<entry>.+))?')
 
 
-def parse_project() -> Optional[DPConfig]:
-    with open(PROJECT_FILE, mode='rb') as f:
-        root = tomli.load(f)
+class ConfigKeys:
+    MODE = "mode"
+    PYCACHE_BL = "py-cache-blacklist"
+    STDLIB_BL = "stdlib-blacklist"
+    INC_TK = "include-tk"
+    DATA_GLOBS = "data-globs"
+    DEBUG_LOGS = "debug-logs"
 
-    config = DPConfig()
+    VALID_KEYS = [MODE, PYCACHE_BL, STDLIB_BL, INC_TK, DATA_GLOBS, DEBUG_LOGS]
+
+
+def parse_project() -> Optional[PackConfig]:
+    """
+    Load the pyproject.toml file
+    """
+    try:
+        with open(PROJECT_FILE, mode='rb') as f:
+            root = tomli.load(f)
+    except FileNotFoundError:
+        logErr("Cannot find pyproject.toml")
+        return None
+
+    config = PackConfig()
 
     try:
         project = root['project']
     except KeyError:
         logErr("'project' missing from pyproject.toml")
         return None
 
     try:
-        name = project['name']
+        projectName = str(project['name'])
     except KeyError:
         logErr("'project.name' missing from pyproject.toml")
         return None
 
     try:
         version = project['version']
     except KeyError:
@@ -48,54 +66,90 @@
     try:
         scripts = project['scripts']
     except KeyError:
         logErr("'project.scripts' missing from pyproject.toml")
         return None
 
     try:
-        mode = root['tool']['diamondpack']['mode']
+        dpConfigs = root['tool']['diamondpack']
+    except KeyError:
+        dpConfigs = {}
+
+    badConfig = False
+    for key in dpConfigs.keys():
+        if key not in ConfigKeys.VALID_KEYS:
+            badConfig = True
+            logErr(f'Invalid project config tool.diamondpack.{key}')
+
+    if badConfig:
+        return None
+
+    try:
+        mode = dpConfigs[ConfigKeys.MODE]
         if mode == 'app':
             config.mode = DPMode.APP
         elif mode == 'script':
             config.mode = DPMode.SCRIPT
         else:
             logErr(f"Invalid value for 'tool.diamondpack.mode': '{mode}', expected 'app' or 'script'")
             return None
 
     except KeyError:
         config.mode = DPMode.APP
 
     try:
-        config.stdlib_copy_block = root['tool']['diamondpack']['stdlib-blacklist']
+        config.stdlib_copy_block = dpConfigs[ConfigKeys.STDLIB_BL]
+    except KeyError:
+        pass
+
+    try:
+        config.include_tk = dpConfigs[ConfigKeys.INC_TK]
+    except KeyError:
+        pass
+
+    try:
+        config.cache_block = dpConfigs[ConfigKeys.PYCACHE_BL]
+    except KeyError:
+        pass
+
+    try:
+        config.data_globs = dpConfigs[ConfigKeys.DATA_GLOBS]
     except KeyError:
         pass
 
-    config.name = f'{name}-{version}'
+    try:
+        config.debug_logs = dpConfigs[ConfigKeys.DEBUG_LOGS]
+    except KeyError:
+        pass
+
+    config.name = f'{projectName}-{version}'
 
     if not os.path.isdir("dist"):
-        logErr("Cannot find 'dist' directory")
+        logErr("Cannot find 'dist' directory, did you build your package to a wheel?")
         return None
 
-    files = glob.glob(os.path.join('dist', f'{config.name}*.whl'))
+    wheelGlob = os.path.join('dist', f'{projectName.replace("-", "_")}-{version}*.whl')
+
+    files = glob.glob(wheelGlob)
     if len(files) != 1:
-        logErr(f"Error finding exact wheel, potentials: {files}")
+        logErr(f"Error finding exact wheel (glob='{wheelGlob}'), potentials: {files}")
         return None
 
     config.wheels = [files[0]]
 
     error = False
     for name, value in scripts.items():
         m = SCRIPT_RE.fullmatch(value)
         if m is None:
             logErr(f"Invalid script spec: '{value}'")
             error = True
             continue
         path = m.group('path')
         entry = m.group('entry')
-        config.scripts.append(DPScript(name, path, entry))
+        config.scripts.append(App(name, path, entry))
 
     if error:
         return None
 
     return config
```

### Comparing `diamondpack-1.4.1/diamondpack/app-templates/app.cpp` & `diamondpack-1.4.5/diamondpack/app-templates/app.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 */
 #ifdef _MSC_VER
     #define WIN32_LEAN_AND_MEAN
 
     #include <Windows.h>
     #include <strsafe.h>
     #include <winbase.h>
+
+    // Use backslashes
+    #define SEP "\\"
 #else
     #include <cstring>
     #include <errno.h>
     #include <stdlib.h>
+
+    // Use forward slashes
+    #define SEP "/"
 #endif
 
 #include <filesystem>
 #include <iostream>
 #include <sstream>
 #include <string>
 #include <vector>
 
 #ifdef DIAMOND_LOGGING
-    #define LOG(x) std::cout << x
+    #define LOG(x) std::cout << "<> " << x
 #else
     #define LOG(x)
 #endif
 
 bool write_env(const char* name, const std::string& value)
 {
     LOG("Setting " << name << "=" << value << std::endl);
@@ -91,56 +97,60 @@
         installDir = std::filesystem::current_path().string();
     }
 
     LOG("App location: " << installDir << std::endl);
 
     // Set up the PYTHONHOME var
     std::stringstream ss;
-    ss << installDir << "/venv/stdlib";
+    ss << installDir << SEP "venv";
     if(!write_env("PYTHONHOME", ss.str()))
     {
         return -1;
     }
 
-    // Set up the PYTHONPATH var
-    ss = std::stringstream();
-    ss << installDir
-       << "/venv/lib/"
-#ifndef _MSC_VER
-          "@@PYTHON@@/"
-#endif
-          "site-packages";
-
-    if(!write_env("PYTHONPATH", ss.str()))
-    {
-        return -1;
-    }
-
 #ifndef _MSC_VER
     ss = std::stringstream();
     ss << installDir << "/venv/bin";
     if(!write_env("LD_LIBRARY_PATH", ss.str()))
     {
         return -1;
     }
 #endif
 
     // Set up exec string
     ss = std::stringstream();
-    ss << installDir
+    ss << "\""
+#ifdef _MSC_VER
+       /*
+           Windows is wack, so we have to double quote this otherwise it gets
+          stripped
+       */
+       << "\""
+#endif
+       << installDir
+
 #ifdef _MSC_VER
-       << "/venv/Scripts/python.exe"
+       << SEP "venv" SEP "Scripts" SEP "python.exe"
 #else
        << "/venv/bin/python"
 #endif
-          " @@COMMAND@@ ";
+              "\" @@COMMAND@@ "
+
+#ifdef _MSC_VER
+              //Close for the double quote
+              "\""
+#endif
+        ;
 
     // Add all remaining cmd line args
     for(int i = 1; i < argc; ++i)
     {
         ss << " " << argv[i];
     }
 
     // Exec the app
-    LOG("Executing: " << program << std::endl);
-    return std::system(ss.str().c_str());
+    // TODO change windows to use CreateProcess?
+    LOG("Executing: " << ss.str() << std::endl);
+    int out = std::system(ss.str().c_str());
+    LOG("Return Code: " << out << std::endl);
+    return out;
 }
```

### Comparing `diamondpack-1.4.1/diamondpack/app-templates/diamondpack-license.txt` & `diamondpack-1.4.5/diamondpack/app-templates/diamondpack-license.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-This application(s) was packaged using Diamondpack. This results in portions
+This application(s) was packaged using DiamondPack. This results in portions
 of the DiamondPack source code to be included/compiled with this application.
 In particular, this includes code/terminal scripts that bootstrap and launch
 the packaged Python application. This code is subject to the below license.
 
 DiamondPack source code is available here:
 https://github.com/alagyn/DiamondPack
```

### Comparing `diamondpack-1.4.1/diamondpack/dpconfig.py` & `diamondpack-1.4.5/diamondpack/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,42 +3,50 @@
 
 
 class DPMode(enum.IntEnum):
     APP = enum.auto()
     SCRIPT = enum.auto()
 
 
-class DPScript:
+class App:
 
     def __init__(self, name: str, path: str, entry: Optional[str]) -> None:
         """
-        Configs for a single diamondpack executable script
+        Configs for a single diamondpack executable app
 
         :param name: The output name of the app
         :param path: The module path to the python script
         :param entry: Optional entry point, should reference an object of the type Callable[[], Any]
         """
         # The name of the output script, doesn't have to be the same
         #  as the actual python file being executed
         self.name = name
         self.path = path
         self.entry = entry
 
 
-class DPConfig:
+class PackConfig:
     """
     Wrapper for diamondpack configuration
     """
 
     def __init__(self) -> None:
         # packages to install
         self.wheels: List[str] = []
         # (name, module, entry point or None)
-        self.scripts: List[DPScript] = []
+        self.scripts: List[App] = []
         # Overall package name
         self.name = ""
         # Packaging mode
         self.mode: DPMode = DPMode.APP
         # Build directory
         self.build_dir = "build"
+        # blacklisted modules to not remove .py files
+        self.cache_block: List[str] = []
         # blacklisted stdlibs to not copy
         self.stdlib_copy_block: List[str] = []
+        # whether we should copy tk stuff
+        self.include_tk = False
+        # list of file globs and dest dir to copy into the package
+        self.data_globs: List[Tuple[str, str]] = []
+        # enable debug logs
+        self.debug_logs = False
```

### Comparing `diamondpack-1.4.1/diamondpack/dplog.py` & `diamondpack-1.4.5/diamondpack/log.py`

 * *Files identical despite different names*

### Comparing `diamondpack-1.4.1/diamondpack/pack.py` & `diamondpack-1.4.5/diamondpack/pack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Packaging
 import sys
 import os
 import shutil
 import subprocess as sp
-from typing import Optional, List, Dict, Any
+from typing import List, Dict
 import glob
 import re
 import sysconfig
 
-from diamondpack.dpconfig import DPScript, DPConfig, DPMode
-from diamondpack.dplog import log
+from diamondpack.config import App, PackConfig, DPMode
+from diamondpack.log import log
 
 _IS_WINDOWS = sys.platform == 'win32'
 
 _CMD_REPLACE = '@@COMMAND@@'
 _PY_REPLACE = '@@PYTHON@@'
 
 _PACKAGE_DIR = os.path.split(__file__)[0]
@@ -21,14 +21,20 @@
 
 _REPLACE_RE = re.compile("@@[A-Z]+@@")
 
 _PY_VERSION = f'python{sys.version_info.major}.{sys.version_info.minor}'
 
 
 def _do_replace(template: str, outfile: str, replacements: Dict[str, str]) -> None:
+    """
+    Copy the contents of the template to the output path replacing values according to the map
+    :param template: The template file path
+    :param outfile: The output file path
+    :param replacements: Dict of replacement values like @@KEY@@: "value"
+    """
     with open(outfile, mode='w') as outF, open(os.path.join(_TEMPLATE_DIR, template), mode='r') as inF:
         for line in inF:
             line = _REPLACE_RE.sub(lambda x: replacements[x.group(0)], line)
             outF.write(line)
 
 
 def execute(args: List[str], env=None) -> int:
@@ -39,37 +45,60 @@
             print("  \u2502", line, end='')
     print("  \u2514")
     sys.stdout.flush()
 
     return run.wait()
 
 
+LIB_RE = re.compile(r'[a-zA-Z._0-9/\-+]+ => (?P<filename>[a-zA-Z._0-9\-/\\]+) \(0x[0-9a-f]+\)')
+
+
+def _copy_linux_required_libs(target: str, outDir: str):
+    out = sp.run(["ldd", target], capture_output=True)
+    libStr = out.stdout.decode()
+    libList = [x.strip() for x in libStr.split("\n")]
+    for x in libList:
+        m = LIB_RE.fullmatch(x)
+        if m is None:
+            continue
+        file = m.group('filename')
+        libName = os.path.split(file)[1]
+        shutil.copyfile(file, os.path.join(outDir, libName))
+
+
 class DiamondPacker:
 
-    def __init__(self, config: DPConfig) -> None:
+    def __init__(self, config: PackConfig) -> None:
         self._config = config
         self._buildDir = config.build_dir
         self._outputDir = os.path.join("dist", config.name)
         self._venvDir = os.path.join(self._outputDir, "venv")
         if _IS_WINDOWS:
-            self.venvBin = os.path.join(self._venvDir, "Scripts")
+            self._venvBin = os.path.join(self._venvDir, "Scripts")
+            self._venvLib = os.path.join(self._venvDir, "Lib")
         else:
-            self.venvBin = os.path.join(self._venvDir, "bin")
+            self._venvBin = os.path.join(self._venvDir, "bin")
+            self._venvLib = os.path.join(self._venvDir, "lib", _PY_VERSION)
 
     def pack(self):
+        """
+        Main entry point for packing
+        """
         log(f"Building Virtual Environment")
         self._build_env()
 
         for script in self._config.scripts:
             log(f"Generating app - {script.name}")
             if self._config.mode == DPMode.APP:
                 self._make_exec(script)
             else:
                 self._make_script(script)
 
+        self._copy_data()
+
     def _build_env(self):
         """
         Creates a virtual env and optionally installs requirements
 
         :param build_dir: Output build directory
         :param wheels: A list of wheels to install into the venv
         """
@@ -78,15 +107,15 @@
 
         if os.path.exists(self._venvDir):
             shutil.rmtree(self._venvDir)
 
         log("Calling venv")
         execute([python_exec, '-m', 'venv', self._venvDir, '--copies'])
 
-        venvExec = os.path.join(self.venvBin, "python")
+        venvExec = os.path.join(self._venvBin, "python")
 
         args = [
             venvExec,
             "-m",
             "pip",
             "install",
             "--disable-pip-version-check",
@@ -101,58 +130,67 @@
         venvCfgFile = os.path.join(self._venvDir, "pyvenv.cfg")
         os.remove(venvCfgFile)
 
         # Remove scripts
         toRemove = ["*ctivate*", "pip*", "python*"]
 
         for xxx in toRemove:
-            for f in glob.glob(os.path.join(self.venvBin, xxx)):
+            for f in glob.glob(os.path.join(self._venvBin, xxx)):
                 os.remove(f)
 
         # Copy required libraries
         log("Copying required libraries")
         if _IS_WINDOWS:
             libpath = sysconfig.get_config_var("installed_base")
             for file in glob.glob(os.path.join(libpath, "*.dll")):
                 fname = os.path.split(file)[1]
-                shutil.copyfile(file, os.path.join(self.venvBin, fname))
+                shutil.copyfile(file, os.path.join(self._venvLib, fname))
+            otherDLLs = os.path.join(libpath, 'DLLs')
+            for file in glob.glob(os.path.join(otherDLLs, "*.dll")):
+                fname = os.path.split(file)[1]
+                shutil.copyfile(file, os.path.join(self._venvLib, fname))
+            for file in glob.glob(os.path.join(otherDLLs, "*.pyd")):
+                fname = os.path.split(file)[1]
+                shutil.copyfile(file, os.path.join(self._venvLib, fname))
+            if self._config.include_tk:
+                shutil.copytree(os.path.join(libpath, "tcl", "tcl8.6"), os.path.join(self._venvDir, "Lib", "tcl8.6"))
+                shutil.copytree(os.path.join(libpath, "tcl", "tk8.6"), os.path.join(self._venvDir, "Lib", "tk8.6"))
         else:
-            out = sp.run(["ldd", python_exec], capture_output=True)
-            libStr = out.stdout.decode()
-            libList = [x.strip() for x in libStr.split("\n")]
-            LIB_RE = re.compile(r'[a-zA-Z._0-9\-]+ => (?P<filename>[a-zA-Z._0-9\-/\\]+) \(0x[0-9a-f]+\)')
-
-            for x in libList:
-                m = LIB_RE.fullmatch(x)
-                if m is None:
-                    continue
-                file = m.group('filename')
-                libName = os.path.split(file)[1]
-                shutil.copyfile(file, os.path.join(self.venvBin, libName))
+            _copy_linux_required_libs(python_exec, self._venvBin)
+
+            if self._config.include_tk:
+                _copy_linux_required_libs("/usr/lib/libtk8.6.so", self._venvBin)
+
+            if self._config.include_tk:
+                shutil.copy("/usr/lib/libtk8.6.so", os.path.join(self._venvBin, "libtk8.6.so"))
+                shutil.copytree("/usr/lib/tk8.6", os.path.join(self._venvDir, 'lib', "tk8.6"))
+
+                shutil.copy("/usr/lib/libtcl8.6.so", os.path.join(self._venvBin, "libtcl8.6.so"))
+                shutil.copytree("/usr/lib/tcl8.6", os.path.join(self._venvDir, 'lib', "tcl8.6"))
 
         log("Copying python executable")
         # Copy the python executable
-        newExec = os.path.join(self.venvBin, "python")
+        newExec = os.path.join(self._venvBin, "python")
         if _IS_WINDOWS:
             newExec += ".exe"
             python_exec = os.path.join(sysconfig.get_config_var("installed_base"), "python.exe")
         shutil.copyfile(python_exec, newExec)
         # Set permissions
         os.chmod(newExec, 0o755)
 
         log("Copying stdlib")
         # Copy the stdlib
         globalStdlib = sysconfig.get_path('stdlib')
 
-        if _IS_WINDOWS:
-            privateStdLib = os.path.join(self._venvDir, "stdlib", "Lib")
-        else:
-            privateStdLib = os.path.join(self._venvDir, "stdlib", "lib", _PY_VERSION)
-
-        shutil.copytree(globalStdlib, privateStdLib, ignore=shutil.ignore_patterns(*self._config.stdlib_copy_block))
+        shutil.copytree(
+            globalStdlib,
+            self._venvLib,
+            ignore=shutil.ignore_patterns(*self._config.stdlib_copy_block),
+            dirs_exist_ok=True
+        )
 
         log("Cleaning environment")
         if _IS_WINDOWS:
             packageDir = os.path.join(self._venvDir, "Lib", "site-packages")
         else:
             packageDir = os.path.join(self._venvDir, "lib", _PY_VERSION, "site-packages")
 
@@ -168,110 +206,164 @@
             except IndexError:
                 return
             # remove the original file
             os.remove(filename)
             # rename the cached file
             shutil.move(cacheFile, os.path.join(folder, fname + ".pyc"))
 
+        if len(self._config.cache_block) > 0:
+            BL_RE = re.compile("|".join(self._config.cache_block))
+        else:
+            BL_RE = None
+
         for xxx in glob.glob(os.path.join(packageDir, "*/**.py"), recursive=True):
+            if BL_RE is not None and BL_RE.search(xxx) is not None:
+                continue
             keepCache(xxx)
 
         stdlibCacheBlacklist = ["encodings"]
         BL_RE = re.compile("|".join(stdlibCacheBlacklist))
 
-        for xxx in glob.glob(os.path.join(privateStdLib, "*/**.py"), recursive=True):
+        for xxx in glob.glob(os.path.join(self._venvLib, "*/**.py"), recursive=True):
             if BL_RE.search(xxx) is not None:
                 continue
             keepCache(xxx)
 
         shutil.copy(os.path.join(_TEMPLATE_DIR, "diamondpack-license.txt"), self._outputDir)
 
         log("Success - Virtual Environment")
 
-    def _get_cmd(self, script: DPScript) -> str:
-        if script.entry is not None:
-            return f'-c "from {script.path} import {script.entry}; exit({script.entry}())"'
+    def _get_cmd(self, app: App) -> str:
+        """
+        Returns the appropriate python cmd arguments depending on the app's entry point
+        :param app: The app
+        :return: The command string
+        """
+        if app.entry is not None:
+            # If the app has an entry point defined, run python in "command" mode
+            # import the func from the specified module, and execute it
+            return f'-c "from {app.path} import {app.entry}; exit({app.entry}())"'
         else:
-            return f'-m {script.path}'
-
-    def _make_script(self, script: DPScript):
+            # else just run the script as a module
+            return f'-m {app.path}'
 
-        cmd = self._get_cmd(script)
+    def _make_script(self, app: App):
+        """
+        Generate a .sh or .bat script for the given app
+        :param app: The app
+        :return: None
+        """
+        cmd = self._get_cmd(app)
 
+        # Select script extension
         if _IS_WINDOWS:
             extension = ".bat"
         else:
             extension = ".sh"
 
+        # generate filenames
         template = "app" + extension
-        outfile = os.path.join(self._outputDir, script.name + extension)
+        outfile = os.path.join(self._outputDir, app.name + extension)
 
+        # generate replacements
         replace = {
             _CMD_REPLACE: cmd,
             _PY_REPLACE: _PY_VERSION
         }
 
         _do_replace(template, outfile, replace)
 
+        # chmod
         if not _IS_WINDOWS:
             os.chmod(outfile, 0o755)
 
-        log(f'Success - {script.name}')
+        log(f'Success - {app.name}')
 
-    def _make_exec(self, script: DPScript):
+    def _make_exec(self, app: App):
+        """
+        Generate an executable for the given app
+        :param app: The app
+        :return: None
+        """
 
-        cmd = self._get_cmd(script)
+        cmd = self._get_cmd(app)
         # Escape quotes
         cmd = re.sub(r'"', '\\"', cmd)
 
+        # setup cmake dirs
         cmakeBuild = os.path.join(self._buildDir, "dp-cmake-build")
         cmakeSrc = os.path.join(self._buildDir, "dp-app-src-dir")
         os.makedirs(cmakeSrc, exist_ok=True)
 
         template = 'app.cpp'
         outfile = os.path.join(cmakeSrc, f'app.cpp')
 
         replace = {
             _CMD_REPLACE: cmd,
             _PY_REPLACE: _PY_VERSION
         }
 
         _do_replace(template, outfile, replace)
 
+        # Copy the build config
         shutil.copy(os.path.join(_TEMPLATE_DIR, "CMakeLists.txt"), cmakeSrc)
 
-        configureParams = ["cmake", "-S", cmakeSrc, "-B", cmakeBuild, f"-DEXEC_NAME={script.name}"]
+        configureParams = ["cmake", "-S", cmakeSrc, "-B", cmakeBuild, f"-DEXEC_NAME={app.name}"]
 
         buildParams = ["cmake", "--build", cmakeBuild]
 
         if _IS_WINDOWS:
             buildParams.append("--config=Release")
         else:
             configureParams.append("-DCMAKE_BUILD_TYPE=Release")
 
-        log(f"Building executable - {script.name}")
+        if self._config.debug_logs:
+            configureParams.append("-DDEBUG_LOGS=ON")
+
+        log(f"Building executable - {app.name}")
 
         log("Configuring CMake")
         ret = execute(configureParams)
         if ret != 0:
             raise RuntimeError(f"Unable to configure cmake: Return code ({ret})")
 
         log("Building app")
         ret = execute(buildParams)
         if ret != 0:
             raise RuntimeError(f"Unable to compile application: Return code ({ret})")
 
-        log(f"Copying executable - {script.name}")
+        log(f"Copying executable - {app.name}")
 
         if _IS_WINDOWS:
-            execName = f'{script.name}.exe'
+            execName = f'{app.name}.exe'
             execPath = os.path.join(cmakeBuild, "Release", execName)
         else:
-            execName = script.name
+            execName = app.name
             execPath = os.path.join(cmakeBuild, execName)
 
         if not os.path.isfile(execPath):
             raise RuntimeError(f"Cannot find built executable: {execPath}")
 
         shutil.copy(execPath, os.path.join(self._outputDir, execName))
 
-        log(f'Success - {script.name}')
+        if not _IS_WINDOWS:
+            #_copy_linux_required_libs(execPath, self._outputDir)
+            pass
+
+        log(f'Success - {app.name}')
+
+    def _copy_data(self):
+        if len(self._config.data_globs) == 0:
+            return
+        log("Copying Data")
+        print("  \u250C")
+        for globPath, dest in self._config.data_globs:
+            outDir = os.path.join(self._outputDir, dest)
+            if not os.path.exists(outDir):
+                os.makedirs(outDir, exist_ok=True)
+            for f in glob.iglob(globPath):
+                if not os.path.isfile(f):
+                    continue
+                print(f"  \u2502 {f} -> {outDir}\\{os.path.basename(f)}")
+                shutil.copy(f, outDir)
+        print("  \u2514")
+        log("Copying Data - Done")
```

### Comparing `diamondpack-1.4.1/diamondpack.egg-info/PKG-INFO` & `diamondpack-1.4.5/diamondpack.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondpack
-Version: 1.4.1
+Version: 1.4.5
 Summary: A simple packager for creating distributable python applications
 Author: Alagyn
 License: MIT License
         
         Copyright (c) 2023 Ben "Alagyn" Kimbrough
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,22 +70,45 @@
 `pip install diamondpack[app]`
 or
 `pip install cmake`
 
 ## Usage:
 
 ### 1. Configure DiamondPack via your `pyproject.toml`
+
 ```toml
 [project.scripts]
 # Each script named here will generate a new executable
 myScript = "examplePackage.myScript:main"
 
 [tool.diamondpack]
 mode = "app"
+
+# Prevents specific installed packages from being reduced to only .pyc files
+# Some packages complaing about this. This is a list of the MODULE's name, same as it is imported as
+# NOT the pip package name
+py-cache-blacklist = ["opencv"]
+
+# Prevents specific stdlib packages from being copied to reduce package size
+stdlib-blacklist = ["email", "turtle", "unittest"]
+
+# Flag to copy required tk/tcl files
+include-tk = false
+
+# Additional data files can be copied into your distribution like this
+# File globs are copied to the specified path in the dist.
+data-globs = [
+    ["myData/img*.jpg", "destinationDir"],
+    ["myData/data.dat", "data"]
+]
+
+# Enable some additional logging for the "app" mode
+debug-logs = true
 ```
+
 Mode can be `app` or `script`:
 - `app` will generate a compiled executable (requires CMake and a compiler installed)
 - `script` will generate a bash (Linux) or batch (Windows) script
 
 
 ### 2. Build your application into a wheel
 `python -m build --wheel`
```

### Comparing `diamondpack-1.4.1/diamondpack.egg-info/SOURCES.txt` & `diamondpack-1.4.5/diamondpack.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 diamondpack/__init__.py
 diamondpack/__main__.py
-diamondpack/dpconfig.py
-diamondpack/dplog.py
+diamondpack/config.py
+diamondpack/log.py
 diamondpack/pack.py
 diamondpack.egg-info/PKG-INFO
 diamondpack.egg-info/SOURCES.txt
 diamondpack.egg-info/dependency_links.txt
 diamondpack.egg-info/entry_points.txt
 diamondpack.egg-info/requires.txt
 diamondpack.egg-info/top_level.txt
```

### Comparing `diamondpack-1.4.1/pyproject.toml` & `diamondpack-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=58.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diamondpack"
 authors = [{ name = "Alagyn" }]
-version = "1.4.1"
+version = "1.4.5"
 description = "A simple packager for creating distributable python applications"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { file = "LICENSE" }
 keywords = ["package", "distribute"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

