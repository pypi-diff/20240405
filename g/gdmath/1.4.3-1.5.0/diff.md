# Comparing `tmp/gdmath-1.4.3.tar.gz` & `tmp/gdmath-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmath-1.4.3.tar", last modified: Thu Apr  4 12:05:49 2024, max compression
+gzip compressed data, was "gdmath-1.5.0.tar", last modified: Fri Apr  5 14:16:46 2024, max compression
```

## Comparing `gdmath-1.4.3.tar` & `gdmath-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:49.642386 gdmath-1.4.3/
--rw-rw-rw-   0        0        0     1091 2024-04-04 12:05:29.000000 gdmath-1.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0      150 2024-04-04 12:05:29.000000 gdmath-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4604 2024-04-04 12:05:49.642386 gdmath-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2185 2024-04-04 12:05:29.000000 gdmath-1.4.3/README.md
--rw-rw-rw-   0        0        0     1437 2024-04-04 12:05:29.000000 gdmath-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 12:05:49.642386 gdmath-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-04-04 12:05:29.000000 gdmath-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:49.626761 gdmath-1.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:49.626761 gdmath-1.4.3/src/gdmath/
--rw-rw-rw-   0        0        0      225 2024-04-04 12:05:29.000000 gdmath-1.4.3/src/gdmath/__init__.py
--rw-rw-rw-   0        0        0      225 2024-04-04 12:05:29.000000 gdmath-1.4.3/src/gdmath/__init__.pyi
--rw-rw-rw-   0        0        0   279870 2024-04-04 12:05:30.000000 gdmath-1.4.3/src/gdmath/_gdmath.pyi
--rw-rw-rw-   0        0        0  1184016 2024-04-04 12:05:30.000000 gdmath-1.4.3/src/gdmath/_gdmath.pyx
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:49.642386 gdmath-1.4.3/src/gdmath.egg-info/
--rw-rw-rw-   0        0        0     4604 2024-04-04 12:05:49.000000 gdmath-1.4.3/src/gdmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-04 12:05:49.000000 gdmath-1.4.3/src/gdmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:05:49.000000 gdmath-1.4.3/src/gdmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 12:05:49.000000 gdmath-1.4.3/src/gdmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 14:16:46.372503 gdmath-1.5.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 14:16:15.000000 gdmath-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      180 2024-04-05 14:16:15.000000 gdmath-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4669 2024-04-05 14:16:46.372503 gdmath-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2250 2024-04-05 14:16:15.000000 gdmath-1.5.0/README.md
+-rw-rw-rw-   0        0        0     1437 2024-04-05 14:16:15.000000 gdmath-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 14:16:46.372503 gdmath-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-04-05 14:16:15.000000 gdmath-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 14:16:46.356882 gdmath-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 14:16:46.372503 gdmath-1.5.0/src/gdmath/
+-rw-rw-rw-   0        0        0      225 2024-04-05 14:16:15.000000 gdmath-1.5.0/src/gdmath/__init__.py
+-rw-rw-rw-   0        0        0      225 2024-04-05 14:16:15.000000 gdmath-1.5.0/src/gdmath/__init__.pyi
+-rw-rw-rw-   0        0        0  1108012 2024-04-05 14:16:17.000000 gdmath-1.5.0/src/gdmath/_gdmath.pyi
+-rw-rw-rw-   0        0        0  1951229 2024-04-05 14:16:17.000000 gdmath-1.5.0/src/gdmath/_gdmath.pyx
+drwxrwxrwx   0        0        0        0 2024-04-05 14:16:46.372503 gdmath-1.5.0/src/gdmath.egg-info/
+-rw-rw-rw-   0        0        0     4669 2024-04-05 14:16:46.000000 gdmath-1.5.0/src/gdmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-05 14:16:46.000000 gdmath-1.5.0/src/gdmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 14:16:46.000000 gdmath-1.5.0/src/gdmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 14:16:46.000000 gdmath-1.5.0/src/gdmath.egg-info/top_level.txt
```

### Comparing `gdmath-1.4.3/LICENSE.txt` & `gdmath-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gdmath-1.4.3/PKG-INFO` & `gdmath-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmath
-Version: 1.4.3
+Version: 1.5.0
 Summary: GdMath: a fast math library for game development
 Author-email: shBLOCK <sh@shblock.xyz>
 License: MIT License
         
         Copyright (c) 2019 Federico Stra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,39 +41,45 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# GdMath: a fast math library for game development
+# GdMath: a lightning fast spatial math library for gamedev
 
 [![Codegen](https://github.com/shBLOCK/GdMath/actions/workflows/codegen.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/codegen.yml)
 [![Tests](https://github.com/shBLOCK/GdMath/actions/workflows/tests.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/tests.yml)
 [![Release](https://github.com/shBLOCK/GdMath/actions/workflows/release.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/release.yml)
 
 ## Main features
-- 100% Cython implementation (~30x speedup from pure python on average)
-  - Codegen based
-- Linear Algebra
+- Fast Pure Cython Implementation
+  - ~20x speedup from pure python(3.12) impl on average
+  - Based on custom code generation
+- Spatial Math
   - [Vector](https://github.com/shBLOCK/GdMath/wiki#vectors)
-    - Pythonic and GLSL-like
     - Operators +, -, *, /, @(dot), ^(cross), |(distance) ...
-    - Fast swizzling (e.g. `Vec3(1, 2, 3).zxy`)
+    - Fast (compile time) swizzling (e.g. `Vec3(1, 2, 3).zxy`)
     - Flexible constructor (e.g. `Vec3(Vec2(1, 2), 3)`)
     - Iterating and unpacking (e.g. `x, y, z = Vec3(1, 2, 3)`)
+    - Works with other libraries (pygame, numpy, ...)
   - Transform
     - [Transform2D](https://github.com/shBLOCK/GdMath/wiki#transform2d) & [Transform3D](https://github.com/shBLOCK/GdMath/wiki#transform3d)
-    - Godot and GLSL like api
+- All floats are double-precision
+- Full pythonic interface & GLSL-like API
 - Stubs for better IDE support
 
 Please refer to the [wiki](https://github.com/shBLOCK/GdMath/wiki) for more details
 
+## Benchmark
+[![Benchmark Results](https://github.com/shBLOCK/GdMath/raw/master/benchmark/chart.png)](https://github.com/shBLOCK/GdMath/tree/master/benchmark/chart.png)
+
 ## Implementation details
-**This library uses code generation.**   
-Every swizzle pattern and constructor are implemented as individual methods and properties (For performance reasons).   
-As a result, code generation is required so that I don't have to maintain 50,000+ lines of code by hand...   
-Besides, it also has the convenience that vector classes of every dimension and type (e.g. Vec2 Vec3 Vec2i Vec3i) are generated from the same template, so a lot of repetitive code is avoided.
+- **Codegen!**  
+  Custom code generation is used throughout this library.  
+  Every swizzle pattern and constructor are implemented as individual methods and properties (For performance reasons).   
+  As a result, code generation is required so that I don't have to maintain 50,000+ lines of code by hand...   
+  Besides, it also handles vector classes of every dimension and type (e.g. Vec2 Vec3 Vec2i Vec3i) are generated from the same template, so a lot of repetitive code is avoided.
+  There's also a stub generator.
 
 ## Notes
-- This library was initially inspired by [Godot](https://godotengine.org/)'s math library. (pun intended)   
-- FYI, when I was coding this, I didn't know about `Cython.Tempita` until it's too late. It'd probably be a lot easier if I knew it from the beginning and don't have to write as much codegen by myself... But I'd still need to do things like overloading by myself anyway, so it's not a big deal.
+- This library was initially inspired by [Godot](https://godotengine.org/)'s math library. Pun intended :)
```

### Comparing `gdmath-1.4.3/pyproject.toml` & `gdmath-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "cython"]
 
 [project]
 name = "gdmath"
-version = "1.4.3"
+version = "1.5.0"
 description = "GdMath: a fast math library for game development"
 readme = "README.md"
 requires-python = ">= 3.9"
 license = {file = "LICENSE.txt"}
 authors = [{name = "shBLOCK", email = "sh@shblock.xyz"}]
 keywords = ["vector", "gamedev", "linear algebra", "math library", "math", "game development"]
 classifiers = [
```

### Comparing `gdmath-1.4.3/src/gdmath.egg-info/PKG-INFO` & `gdmath-1.5.0/src/gdmath.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmath
-Version: 1.4.3
+Version: 1.5.0
 Summary: GdMath: a fast math library for game development
 Author-email: shBLOCK <sh@shblock.xyz>
 License: MIT License
         
         Copyright (c) 2019 Federico Stra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,39 +41,45 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# GdMath: a fast math library for game development
+# GdMath: a lightning fast spatial math library for gamedev
 
 [![Codegen](https://github.com/shBLOCK/GdMath/actions/workflows/codegen.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/codegen.yml)
 [![Tests](https://github.com/shBLOCK/GdMath/actions/workflows/tests.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/tests.yml)
 [![Release](https://github.com/shBLOCK/GdMath/actions/workflows/release.yml/badge.svg)](https://github.com/shBLOCK/GdMath/actions/workflows/release.yml)
 
 ## Main features
-- 100% Cython implementation (~30x speedup from pure python on average)
-  - Codegen based
-- Linear Algebra
+- Fast Pure Cython Implementation
+  - ~20x speedup from pure python(3.12) impl on average
+  - Based on custom code generation
+- Spatial Math
   - [Vector](https://github.com/shBLOCK/GdMath/wiki#vectors)
-    - Pythonic and GLSL-like
     - Operators +, -, *, /, @(dot), ^(cross), |(distance) ...
-    - Fast swizzling (e.g. `Vec3(1, 2, 3).zxy`)
+    - Fast (compile time) swizzling (e.g. `Vec3(1, 2, 3).zxy`)
     - Flexible constructor (e.g. `Vec3(Vec2(1, 2), 3)`)
     - Iterating and unpacking (e.g. `x, y, z = Vec3(1, 2, 3)`)
+    - Works with other libraries (pygame, numpy, ...)
   - Transform
     - [Transform2D](https://github.com/shBLOCK/GdMath/wiki#transform2d) & [Transform3D](https://github.com/shBLOCK/GdMath/wiki#transform3d)
-    - Godot and GLSL like api
+- All floats are double-precision
+- Full pythonic interface & GLSL-like API
 - Stubs for better IDE support
 
 Please refer to the [wiki](https://github.com/shBLOCK/GdMath/wiki) for more details
 
+## Benchmark
+[![Benchmark Results](https://github.com/shBLOCK/GdMath/raw/master/benchmark/chart.png)](https://github.com/shBLOCK/GdMath/tree/master/benchmark/chart.png)
+
 ## Implementation details
-**This library uses code generation.**   
-Every swizzle pattern and constructor are implemented as individual methods and properties (For performance reasons).   
-As a result, code generation is required so that I don't have to maintain 50,000+ lines of code by hand...   
-Besides, it also has the convenience that vector classes of every dimension and type (e.g. Vec2 Vec3 Vec2i Vec3i) are generated from the same template, so a lot of repetitive code is avoided.
+- **Codegen!**  
+  Custom code generation is used throughout this library.  
+  Every swizzle pattern and constructor are implemented as individual methods and properties (For performance reasons).   
+  As a result, code generation is required so that I don't have to maintain 50,000+ lines of code by hand...   
+  Besides, it also handles vector classes of every dimension and type (e.g. Vec2 Vec3 Vec2i Vec3i) are generated from the same template, so a lot of repetitive code is avoided.
+  There's also a stub generator.
 
 ## Notes
-- This library was initially inspired by [Godot](https://godotengine.org/)'s math library. (pun intended)   
-- FYI, when I was coding this, I didn't know about `Cython.Tempita` until it's too late. It'd probably be a lot easier if I knew it from the beginning and don't have to write as much codegen by myself... But I'd still need to do things like overloading by myself anyway, so it's not a big deal.
+- This library was initially inspired by [Godot](https://godotengine.org/)'s math library. Pun intended :)
```

