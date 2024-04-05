# Comparing `tmp/praklib-0.1.2.tar.gz` & `tmp/praklib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.2.tar", last modified: Fri Apr  5 15:55:15 2024, max compression
+gzip compressed data, was "praklib-0.1.3.tar", last modified: Fri Apr  5 16:46:26 2024, max compression
```

## Comparing `praklib-0.1.2.tar` & `praklib-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.098560 praklib-0.1.2/
--rw-rw-rw-   0        0        0      261 2024-04-05 15:55:15.097433 praklib-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.076867 praklib-0.1.2/praklib/
--rw-rw-rw-   0        0        0     5720 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.2/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.095407 praklib-0.1.2/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:55:15.098560 praklib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-05 15:55:14.000000 praklib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.401805 praklib-0.1.3/
+-rw-rw-rw-   0        0        0      261 2024-04-05 16:46:26.400804 praklib-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.387245 praklib-0.1.3/praklib/
+-rw-rw-rw-   0        0        0     5636 2024-04-05 16:46:25.000000 praklib-0.1.3/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.3/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.399730 praklib-0.1.3/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:46:26.401805 praklib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-05 16:46:25.000000 praklib-0.1.3/setup.py
```

### Comparing `praklib-0.1.2/praklib/Praktika.py` & `praklib-0.1.3/praklib/Praktika.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,18 +38,19 @@
     # Round the value and the error
     rounded_value = round(value, rounding_precision)
     rounded_error = round(error, rounding_precision)
 
     return rounded_value, rounded_error
 
 def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
-                grid=True, show=True, scatter=True, line=False, err=True):
-    plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
-    data1 = np.arange(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1],
-                      (x[len(x) - 1] + errx[len(x) - 1] - x[0] - errx[0]) / 100, dtype=np.double)
+                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0)):
+    if (xlim == (0,0)):
+        plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
+    else:
+        plt.xlim(xlim[0], xlim[1])
     if (grid == True):
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
 
     if (line == True):
         f, = plt.plot(x, y, linewidth=0.8, c="teal",
```

