# Comparing `tmp/praklib-0.1.1.tar.gz` & `tmp/praklib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.1.tar", last modified: Fri Apr  5 15:08:12 2024, max compression
+gzip compressed data, was "praklib-0.1.2.tar", last modified: Fri Apr  5 15:55:15 2024, max compression
```

## Comparing `praklib-0.1.1.tar` & `praklib-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.998795 praklib-0.1.1/
--rw-rw-rw-   0        0        0      261 2024-04-05 15:08:11.997780 praklib-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.981156 praklib-0.1.1/praklib/
--rw-rw-rw-   0        0        0     4470 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.1/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:08:11.995765 praklib-0.1.1/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 15:08:11.000000 praklib-0.1.1/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:08:11.998795 praklib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-05 15:08:11.000000 praklib-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.098560 praklib-0.1.2/
+-rw-rw-rw-   0        0        0      261 2024-04-05 15:55:15.097433 praklib-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.076867 praklib-0.1.2/praklib/
+-rw-rw-rw-   0        0        0     5720 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.2/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:55:15.095407 praklib-0.1.2/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 15:55:14.000000 praklib-0.1.2/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 15:55:15.098560 praklib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-05 15:55:14.000000 praklib-0.1.2/setup.py
```

### Comparing `praklib-0.1.1/praklib/Praktika.py` & `praklib-0.1.2/praklib/Praktika.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,49 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from lmfit import Model
+import uncertainties.unumpy as unp
+
+
+def round_uncertainties(array):
+    rounded_values = []
+    rounded_errors = []
+    for x in array:
+        rounded_value, rounded_error = custom_round(x.nominal_value, x.std_dev)
+        rounded_values.append(rounded_value)
+        rounded_errors.append(rounded_error)
+    return unp.uarray(rounded_values, rounded_errors)
+
+def custom_round(value, error):
+    # Define a threshold for treating the error as effectively zero
+    epsilon = 1e-10
+
+    # Check if the error is effectively zero
+    if error < epsilon:
+        return 0.0, 0.0
+
+    # Calculate the magnitude of the error
+    error_magnitude = int(np.floor(np.log10(error)))
+
+    # Determine the rounding precision based on the first decimal digit of the error
+    if error_magnitude < 0:
+        rounding_precision = -error_magnitude
+    elif error_magnitude == 0:
+        if int(error * 10) % 10 == 1:
+            rounding_precision = 2
+        else:
+            rounding_precision = 1
+    else:
+        rounding_precision = 0
+
+    # Round the value and the error
+    rounded_value = round(value, rounding_precision)
+    rounded_error = round(error, rounding_precision)
+
+    return rounded_value, rounded_error
 
 def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
                 grid=True, show=True, scatter=True, line=False, err=True):
     plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     data1 = np.arange(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1],
                       (x[len(x) - 1] + errx[len(x) - 1] - x[0] - errx[0]) / 100, dtype=np.double)
     if (grid == True):
```

