# Comparing `tmp/praklib-0.0.8.tar.gz` & `tmp/praklib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.0.8.tar", last modified: Thu Apr  4 15:06:11 2024, max compression
+gzip compressed data, was "praklib-0.0.9.tar", last modified: Thu Apr  4 15:15:29 2024, max compression
```

## Comparing `praklib-0.0.8.tar` & `praklib-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.316893 praklib-0.0.8/
--rw-rw-rw-   0        0        0      261 2024-04-04 15:06:11.315880 praklib-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.300974 praklib-0.0.8/praklib/
--rw-rw-rw-   0        0        0     4268 2024-04-04 15:05:36.000000 praklib-0.0.8/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.8/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:06:11.314563 praklib-0.0.8/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 15:06:11.000000 praklib-0.0.8/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 15:06:11.316893 praklib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-04 15:06:10.000000 praklib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.137068 praklib-0.0.9/
+-rw-rw-rw-   0        0        0      261 2024-04-04 15:15:29.136053 praklib-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.122730 praklib-0.0.9/praklib/
+-rw-rw-rw-   0        0        0     4277 2024-04-04 15:15:16.000000 praklib-0.0.9/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.9/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.135046 praklib-0.0.9/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:15:29.137068 praklib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-04 15:15:28.000000 praklib-0.0.9/setup.py
```

### Comparing `praklib-0.0.8/praklib/Praktika.py` & `praklib-0.0.9/praklib/Praktika.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     latex_table += "\\centering\n"
     latex_table += "\\begin{tabular}{|" + "|".join(["c"] * (num_cols)) + "|}\n"
     latex_table += "\\hline\n"
     latex_table += " & " + " & ".join(col_names) + " \\\\\n"
     latex_table += "\\hline\n"
 
     for i in range(num_rows):
-        latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\\n"
+        latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
 
     latex_table += "\\hline\n"
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
```

