# Comparing `tmp/praklib-0.1.3.tar.gz` & `tmp/praklib-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.3.tar", last modified: Fri Apr  5 16:46:26 2024, max compression
+gzip compressed data, was "praklib-0.1.35.tar", last modified: Fri Apr  5 17:15:01 2024, max compression
```

## Comparing `praklib-0.1.3.tar` & `praklib-0.1.35.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.401805 praklib-0.1.3/
--rw-rw-rw-   0        0        0      261 2024-04-05 16:46:26.400804 praklib-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.387245 praklib-0.1.3/praklib/
--rw-rw-rw-   0        0        0     5636 2024-04-05 16:46:25.000000 praklib-0.1.3/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.3/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:46:26.399730 praklib-0.1.3/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 16:46:26.000000 praklib-0.1.3/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 16:46:26.401805 praklib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-05 16:46:25.000000 praklib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.800145 praklib-0.1.35/
+-rw-rw-rw-   0        0        0      262 2024-04-05 17:15:01.799144 praklib-0.1.35/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.785459 praklib-0.1.35/praklib/
+-rw-rw-rw-   0        0        0     5636 2024-04-05 17:14:52.000000 praklib-0.1.35/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.35/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 17:15:01.797721 praklib-0.1.35/praklib.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 17:15:01.000000 praklib-0.1.35/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 17:15:01.800145 praklib-0.1.35/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-04-05 17:15:01.000000 praklib-0.1.35/setup.py
```

### Comparing `praklib-0.1.3/praklib/Praktika.py` & `praklib-0.1.35/praklib/Praktika.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     param_errors = [results.params[name].stderr if results.params[name].stderr else 0 for name in param_names]
 
     return param_names, param_values, param_errors
 
 def graf_fit(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
                 fit_function, grid=True, show=True, scatter=True):
     plt.xlim(x[0]-errx[0], x[-1]+errx[-1])
-    data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 100)
+    data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 500)
 
     param_names, param_values, param_errors = fit_data(fit_vstup, fit_vystup, params_fit, fit_function, show_results=False)
     funkcni_param = np.array(param_values) + 1j * np.array(param_errors)
     params = dict(zip(param_names, funkcni_param))
 
     data2 = fit_function(data1, **params)
```

