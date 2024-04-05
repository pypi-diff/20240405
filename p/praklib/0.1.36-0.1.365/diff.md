# Comparing `tmp/praklib-0.1.36.tar.gz` & `tmp/praklib-0.1.365.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.36.tar", last modified: Fri Apr  5 17:18:27 2024, max compression
+gzip compressed data, was "praklib-0.1.365.tar", last modified: Fri Apr  5 17:21:39 2024, max compression
```

## Comparing `praklib-0.1.36.tar` & `praklib-0.1.365.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.220511 praklib-0.1.36/
--rw-rw-rw-   0        0        0      262 2024-04-05 17:18:27.219467 praklib-0.1.36/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.205809 praklib-0.1.36/praklib/
--rw-rw-rw-   0        0        0     5821 2024-04-05 17:18:21.000000 praklib-0.1.36/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.36/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.218447 praklib-0.1.36/praklib.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 17:18:27.220511 praklib-0.1.36/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-04-05 17:18:26.000000 praklib-0.1.36/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.216297 praklib-0.1.365/
+-rw-rw-rw-   0        0        0      263 2024-04-05 17:21:39.216297 praklib-0.1.365/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.203430 praklib-0.1.365/praklib/
+-rw-rw-rw-   0        0        0     5969 2024-04-05 17:21:38.000000 praklib-0.1.365/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.365/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.214293 praklib-0.1.365/praklib.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:21:39.216297 praklib-0.1.365/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-04-05 17:21:38.000000 praklib-0.1.365/setup.py
```

### Comparing `praklib-0.1.36/praklib/Praktika.py` & `praklib-0.1.365/praklib/Praktika.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,19 +38,21 @@
     # Round the value and the error
     rounded_value = round(value, rounding_precision)
     rounded_error = round(error, rounding_precision)
 
     return rounded_value, rounded_error
 
 def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
-                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0), loc="upper right"):
+                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0), ylim =(0,0), loc="upper right"):
     if (xlim == (0,0)):
         plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     else:
         plt.xlim(xlim[0], xlim[1])
+    if (ylim != (0,0)):
+        plt.ylim(ylim[0], ylim[1])
     if (grid == True):
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
 
     if (line == True):
         f, = plt.plot(x, y, linewidth=0.8, c="teal",
@@ -75,19 +77,21 @@
     param_names = list(results.params.keys())
     param_values = [results.params[name].value for name in param_names]
     param_errors = [results.params[name].stderr if results.params[name].stderr else 0 for name in param_names]
 
     return param_names, param_values, param_errors
 
 def graf_fit(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
-                fit_function, grid=True, show=True, scatter=True, xlim=(0,0), loc="upper right"):
+                fit_function, grid=True, show=True, scatter=True, xlim=(0,0), ylim =(0,0), loc="upper right"):
     if (xlim == (0, 0)):
         plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     else:
         plt.xlim(xlim[0], xlim[1])
+    if (ylim != (0,0)):
+        plt.ylim(ylim[0], ylim[1])
     data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 500)
 
     param_names, param_values, param_errors = fit_data(fit_vstup, fit_vystup, params_fit, fit_function, show_results=False)
     funkcni_param = np.array(param_values) + 1j * np.array(param_errors)
     params = dict(zip(param_names, funkcni_param))
 
     data2 = fit_function(data1, **params)
```

