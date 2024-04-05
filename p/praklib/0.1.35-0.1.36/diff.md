# Comparing `tmp/praklib-0.1.35.tar.gz` & `tmp/praklib-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.35.tar", last modified: Fri Apr  5 17:15:01 2024, max compression
+gzip compressed data, was "praklib-0.1.36.tar", last modified: Fri Apr  5 17:18:27 2024, max compression
```

## Comparing `praklib-0.1.35.tar` & `praklib-0.1.36.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.800145 praklib-0.1.35/
--rw-rw-rw-   0        0        0      262 2024-04-05 17:15:01.799144 praklib-0.1.35/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.785459 praklib-0.1.35/praklib/
--rw-rw-rw-   0        0        0     5636 2024-04-05 17:14:52.000000 praklib-0.1.35/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.35/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.797721 praklib-0.1.35/praklib.egg-info/
--rw-rw-rw-   0        0        0      262 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 17:15:01.800145 praklib-0.1.35/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-04-05 17:15:01.000000 praklib-0.1.35/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.220511 praklib-0.1.36/
+-rw-rw-rw-   0        0        0      262 2024-04-05 17:18:27.219467 praklib-0.1.36/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.205809 praklib-0.1.36/praklib/
+-rw-rw-rw-   0        0        0     5821 2024-04-05 17:18:21.000000 praklib-0.1.36/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.36/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:18:27.218447 praklib-0.1.36/praklib.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 17:18:27.000000 praklib-0.1.36/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:18:27.220511 praklib-0.1.36/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-04-05 17:18:26.000000 praklib-0.1.36/setup.py
```

### Comparing `praklib-0.1.35/praklib/Praktika.py` & `praklib-0.1.36/praklib/Praktika.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # Round the value and the error
     rounded_value = round(value, rounding_precision)
     rounded_error = round(error, rounding_precision)
 
     return rounded_value, rounded_error
 
 def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
-                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0)):
+                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0), loc="upper right"):
     if (xlim == (0,0)):
         plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     else:
         plt.xlim(xlim[0], xlim[1])
     if (grid == True):
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
@@ -56,15 +56,15 @@
         f, = plt.plot(x, y, linewidth=0.8, c="teal",
                   label=linelabel, marker="none")
     if (scatter == True):
         g = plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
     if (err == True):
         plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
                  ecolor="red", linewidth=1.0)
-    plt.legend()
+    plt.legend(loc=loc)
     if (show == True):
         plt.show()
 def fit_data(y, z, initial_params, fit_function, show_results=True):
     model = Model(fit_function)
     params = model.make_params()
     for param_name in initial_params.keys():
         params.add(param_name, value=initial_params[param_name])
@@ -75,16 +75,19 @@
     param_names = list(results.params.keys())
     param_values = [results.params[name].value for name in param_names]
     param_errors = [results.params[name].stderr if results.params[name].stderr else 0 for name in param_names]
 
     return param_names, param_values, param_errors
 
 def graf_fit(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
-                fit_function, grid=True, show=True, scatter=True):
-    plt.xlim(x[0]-errx[0], x[-1]+errx[-1])
+                fit_function, grid=True, show=True, scatter=True, xlim=(0,0), loc="upper right"):
+    if (xlim == (0, 0)):
+        plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
+    else:
+        plt.xlim(xlim[0], xlim[1])
     data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 500)
 
     param_names, param_values, param_errors = fit_data(fit_vstup, fit_vystup, params_fit, fit_function, show_results=False)
     funkcni_param = np.array(param_values) + 1j * np.array(param_errors)
     params = dict(zip(param_names, funkcni_param))
 
     data2 = fit_function(data1, **params)
@@ -95,16 +98,17 @@
     plt.ylabel(ylabel)
 
     plt.plot(data1, data2.real, linewidth=0.8, c="teal", label=linelabel)
     if scatter:
         plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
     plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
                  ecolor="red", linewidth=1.0)
-    plt.legend()
-    plt.show()
+    plt.legend(loc=loc)
+    if show==True:
+        plt.show()
 
 
 def latex_table(data, col_names, err=True):
     num_rows = len(data)
     num_cols = len(data[0])
 
     latex_table = "\\begin{table}[h!]\n"
```

