# Comparing `tmp/praklib-0.1.tar.gz` & `tmp/praklib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.tar", last modified: Fri Apr  5 15:02:07 2024, max compression
+gzip compressed data, was "praklib-0.1.1.tar", last modified: Fri Apr  5 15:08:12 2024, max compression
```

## Comparing `praklib-0.1.tar` & `praklib-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.167827 praklib-0.1/
--rw-rw-rw-   0        0        0      259 2024-04-05 15:02:07.166804 praklib-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.154420 praklib-0.1/praklib/
--rw-rw-rw-   0        0        0     4473 2024-04-05 15:01:47.000000 praklib-0.1/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.165793 praklib-0.1/praklib.egg-info/
--rw-rw-rw-   0        0        0      259 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:02:07.167827 praklib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      378 2024-04-05 15:02:06.000000 praklib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.998795 praklib-0.1.1/
+-rw-rw-rw-   0        0        0      261 2024-04-05 15:08:11.997780 praklib-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.981156 praklib-0.1.1/praklib/
+-rw-rw-rw-   0        0        0     4470 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.1/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.995765 praklib-0.1.1/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:08:11.998795 praklib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-05 15:08:11.000000 praklib-0.1.1/setup.py
```

### Comparing `praklib-0.1/praklib/Praktika.py` & `praklib-0.1.1/praklib/Praktika.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     latex_table += "\\hline\n"
 
     if err==True:
         for i in range(num_rows):
             latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
     if err==False:
         for i in range(num_rows):
-            latex_table += " & " + " & ".join([f"${val[0]}$" for val in data[i]]) + " \\\\ \\hline \n"
+            latex_table += " & " + " & ".join([f"${val}$" for val in data[i]]) + " \\\\ \\hline \n"
 
     latex_table += "\\hline\n"
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
```

