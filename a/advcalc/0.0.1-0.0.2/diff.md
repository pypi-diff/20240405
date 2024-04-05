# Comparing `tmp/advcalc-0.0.1.tar.gz` & `tmp/advcalc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.0.1.tar", last modified: Wed Apr  3 02:33:06 2024, max compression
+gzip compressed data, was "advcalc-0.0.2.tar", last modified: Fri Apr  5 02:14:23 2024, max compression
```

## Comparing `advcalc-0.0.1.tar` & `advcalc-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 02:33:06.194702 advcalc-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-03 02:33:06.120489 advcalc-0.0.1/ADVCALC/
--rw-rw-rw-   0        0        0      317 2024-04-03 02:17:17.000000 advcalc-0.0.1/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0      897 2024-04-03 01:35:56.000000 advcalc-0.0.1/ADVCALC/calc.py
--rw-rw-rw-   0        0        0        0 2024-04-03 02:17:15.000000 advcalc-0.0.1/ADVCALC/test.py
--rw-rw-rw-   0        0        0      188 2024-04-03 02:33:06.194702 advcalc-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 02:33:06.193131 advcalc-0.0.1/advcalc.egg-info/
--rw-rw-rw-   0        0        0      188 2024-04-03 02:33:05.000000 advcalc-0.0.1/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-03 02:33:05.000000 advcalc-0.0.1/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 02:33:05.000000 advcalc-0.0.1/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 02:33:05.000000 advcalc-0.0.1/advcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 02:33:05.000000 advcalc-0.0.1/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 02:33:06.194702 advcalc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-03 02:20:45.000000 advcalc-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 02:14:23.719759 advcalc-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-05 02:14:23.673443 advcalc-0.0.2/ADVCALC/
+-rw-rw-rw-   0        0        0      317 2024-04-03 02:17:17.000000 advcalc-0.0.2/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0      878 2024-04-05 02:02:00.000000 advcalc-0.0.2/ADVCALC/calc.py
+-rw-rw-rw-   0        0        0      167 2024-04-05 02:14:23.716750 advcalc-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 02:14:23.712727 advcalc-0.0.2/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-04-05 02:14:23.000000 advcalc-0.0.2/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2024-04-05 02:14:23.000000 advcalc-0.0.2/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 02:14:23.000000 advcalc-0.0.2/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 02:14:23.000000 advcalc-0.0.2/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 02:14:23.719759 advcalc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      486 2024-04-05 02:05:14.000000 advcalc-0.0.2/setup.py
```

### Comparing `advcalc-0.0.1/ADVCALC/calc.py` & `advcalc-0.0.2/ADVCALC/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math as m
 def advcalc(equation):
     print(eval(equation))
     
 def add(num1, num2):
     sum = float(num1) + float(num2)
     print(sum)
 
@@ -15,15 +14,15 @@
     print(sum)
     
 def mul(num1, num2):
     sum = float(num1) * float(num2)
     print(sum)
 
 def sqrt(num):
-    sum = float(m.sqrt(num))
+    sum = float(num ** 0.5)
     print(sum)
 
 def square(num):
     sum = float(num * num)
     print(sum)
     
 def round_without_decimal_place(num):
```

