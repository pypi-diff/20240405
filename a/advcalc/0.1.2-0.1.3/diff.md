# Comparing `tmp/advcalc-0.1.2.tar.gz` & `tmp/advcalc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.2.tar", last modified: Fri Apr  5 03:40:05 2024, max compression
+gzip compressed data, was "advcalc-0.1.3.tar", last modified: Fri Apr  5 03:57:22 2024, max compression
```

## Comparing `advcalc-0.1.2.tar` & `advcalc-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.284151 advcalc-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.222454 advcalc-0.1.2/ADVCALC/
--rw-rw-rw-   0        0        0      894 2024-04-05 03:38:57.000000 advcalc-0.1.2/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      702 2024-04-05 03:40:05.279919 advcalc-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-04-05 03:32:25.000000 advcalc-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:40:05.279919 advcalc-0.1.2/advcalc.egg-info/
--rw-rw-rw-   0        0        0      702 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:40:05.000000 advcalc-0.1.2/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:40:05.284151 advcalc-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      589 2024-04-05 03:39:01.000000 advcalc-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.528325 advcalc-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.495987 advcalc-0.1.3/ADVCALC/
+-rw-rw-rw-   0        0        0     2126 2024-04-05 03:56:50.000000 advcalc-0.1.3/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      754 2024-04-05 03:57:22.524043 advcalc-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-05 03:56:07.000000 advcalc-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.523634 advcalc-0.1.3/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      754 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:57:22.528325 advcalc-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-05 03:57:16.000000 advcalc-0.1.3/setup.py
```

### Comparing `advcalc-0.1.2/ADVCALC/__init__.py` & `advcalc-0.1.3/ADVCALC/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+apiKey = "advcalc-oisdf8asdiufj9iuejisdfuj48ieujkassdfh834iuer84ue6479ureidjfhjiherjfug8ireuufh"
 def advcalc(equation):
     print(eval(equation))
     
 def add(num1, num2):
     sum = float(num1) + float(num2)
     print(sum)
 
@@ -39,8 +40,65 @@
     
 def cbrt(num):
     sum = float(num) ** (1. / 3)
     print(sum)
 
 def pow(num1, num2):
     sum = float(num1) ** float(num2)
-    print(sum)
+    print(sum)
+    
+def getAPIKey():
+    print("Your API Key is:\n")
+    print(f'{apiKey}')
+    
+def getCode(ApiKey):
+    if str(ApiKey) == str(apiKey):
+        print("""
+def advcalc(equation):
+    print(eval(equation))
+    
+def add(num1, num2):
+    sum = float(num1) + float(num2)
+    print(sum)
+
+def sub(num1, num2):
+    sum = float(num1) - float(num2)
+    print(sum)
+    
+def div(num1, num2):
+    sum = float(num1) / float(num2)
+    print(sum)
+    
+def mul(num1, num2):
+    sum = float(num1) * float(num2)
+    print(sum)
+
+def sqrt(num):
+    sum = float(num ** 0.5)
+    print(sum)
+
+def square(num):
+    sum = float(num * num)
+    print(sum)
+    
+def round_without_decimal_place(num):
+    sum = float(round(num))
+    print(sum)
+
+def round_with_decimal_place(num,decimal):
+    sum = float(round(num,decimal))
+    print(sum)
+
+def cube(num):
+    sum = float(num**3)
+    print(sum)
+    
+def cbrt(num):
+    sum = float(num) ** (1. / 3)
+    print(sum)
+
+def pow(num1, num2):
+    sum = float(num1) ** float(num2)
+    print(sum)""")
+        
+    else:
+        print("Error: API Key does not exist.")
```

### Comparing `advcalc-0.1.2/LICENSE` & `advcalc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.2/PKG-INFO` & `advcalc-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: advcalc
-Version: 0.1.2
-Summary: Advanced Python Calculator
-Author: Zack
-License: MIT
-Keywords: python,calculator
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ADVCALC
 
 ## How to use it
 ##### First use:
 `pip instal advcalc`
 ##### Then, import it in your python file by using:
 `import ADVCALC` 
@@ -42,7 +32,11 @@
 `cube`
 
 `cbrt`
 
 `and`
 
 `pow`
+
+`getAPIKey`
+
+`getCode` **Requires an API Key**
```

### Comparing `advcalc-0.1.2/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Advanced Python Calculator
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -42,7 +42,11 @@
 `cube`
 
 `cbrt`
 
 `and`
 
 `pow`
+
+`getAPIKey`
+
+`getCode` **Requires an API Key**
```

