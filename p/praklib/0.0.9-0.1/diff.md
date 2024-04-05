# Comparing `tmp/praklib-0.0.9.tar.gz` & `tmp/praklib-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.0.9.tar", last modified: Thu Apr  4 15:15:29 2024, max compression
+gzip compressed data, was "praklib-0.1.tar", last modified: Fri Apr  5 15:02:07 2024, max compression
```

## Comparing `praklib-0.0.9.tar` & `praklib-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.137068 praklib-0.0.9/
--rw-rw-rw-   0        0        0      261 2024-04-04 15:15:29.136053 praklib-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.122730 praklib-0.0.9/praklib/
--rw-rw-rw-   0        0        0     4277 2024-04-04 15:15:16.000000 praklib-0.0.9/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.9/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:15:29.135046 praklib-0.0.9/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 15:15:29.000000 praklib-0.0.9/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 15:15:29.137068 praklib-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-04 15:15:28.000000 praklib-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.167827 praklib-0.1/
+-rw-rw-rw-   0        0        0      259 2024-04-05 15:02:07.166804 praklib-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.154420 praklib-0.1/praklib/
+-rw-rw-rw-   0        0        0     4473 2024-04-05 15:01:47.000000 praklib-0.1/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:02:07.165793 praklib-0.1/praklib.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 15:02:07.000000 praklib-0.1/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:02:07.167827 praklib-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      378 2024-04-05 15:02:06.000000 praklib-0.1/setup.py
```

### Comparing `praklib-0.0.9/praklib/Praktika.py` & `praklib-0.1/praklib/Praktika.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,27 +59,31 @@
         plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
     plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
                  ecolor="red", linewidth=1.0)
     plt.legend()
     plt.show()
 
 
-def latex_table(data, col_names):
+def latex_table(data, col_names, err=True):
     num_rows = len(data)
     num_cols = len(data[0])
 
     latex_table = "\\begin{table}[h!]\n"
     latex_table += "\\centering\n"
     latex_table += "\\begin{tabular}{|" + "|".join(["c"] * (num_cols)) + "|}\n"
     latex_table += "\\hline\n"
     latex_table += " & " + " & ".join(col_names) + " \\\\\n"
     latex_table += "\\hline\n"
 
-    for i in range(num_rows):
-        latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
+    if err==True:
+        for i in range(num_rows):
+            latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
+    if err==False:
+        for i in range(num_rows):
+            latex_table += " & " + " & ".join([f"${val[0]}$" for val in data[i]]) + " \\\\ \\hline \n"
 
     latex_table += "\\hline\n"
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
```

