# Comparing `tmp/smart_parallelize-1.0.7.tar.gz` & `tmp/smart_parallelize-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-1.0.7.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.0.tar", max compression
```

## Comparing `smart_parallelize-1.0.7.tar` & `smart_parallelize-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.128520 smart_parallelize-1.0.7/README.md
--rw-r--r--   0        0        0      316 2024-03-30 17:36:51.236388 smart_parallelize-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.946987 smart_parallelize-1.0.7/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     3992 2024-03-30 17:36:37.062634 smart_parallelize-1.0.7/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 smart_parallelize-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.0/README.md
+-rw-r--r--   0        0        0      316 2024-04-05 16:29:58.539934 smart_parallelize-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.0/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4178 2024-04-05 16:56:11.231984 smart_parallelize-2.0.0/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 smart_parallelize-2.0.0/PKG-INFO
```

### Comparing `smart_parallelize-1.0.7/README.md` & `smart_parallelize-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-1.0.7/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.0/smart_parallelize/parallelize.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,103 +25,106 @@
     return MEMORY, CPUS, MEM_PER_WORKER
 
 try:
 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
 except RaySystemError:
 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
 
-def smart_parallelize(func, n_vars2parallelize=1): 
+def smart_parallelize(func): 
     '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
 
     def wrap(**kwargs): 
         def f2(**kwargs):
-            kwargs2       = kwargs.copy()
-            kw1_name      = list(kwargs.keys())[0]
-            kw1_vals      = kwargs[kw1_name]
-            kwargs2[kw1_name] = kw1_vals[0]
-            r0 = func(**kwargs2)
-            if isinstance(r0, tuple):
-                results = ()
-                for i, r in enumerate(r0):
-                    r = np.atleast_1d(r)
-                    results += (np.zeros((len(kw1_vals), *r.shape)),)
-                    tup = True
-            else:
-                results = np.zeros((len(kw1_vals), *r0.shape))
-                tup = False
-
-            for i, kw1_val in enumerate(kw1_vals):
-                kwargs2[kw1_name] = kw1_val
-                r_all = func(**kwargs2)
-                if tup:
-                    for j, r in enumerate(r_all):
-                        results[j][i] = r
-                else:
-                    results[i] = r_all
+            par_args = list(kwargs.keys())[:n_args2parallelize]
+            data_par_args = [kwargs[i] for i in par_args]
+            results = []
+            for i, _ in enumerate(data_par_args[0]):
+                kwargs_0 = kwargs.copy()
+                for j, _ in enumerate(data_par_args):
+                    kwargs_0[par_args[j]] = data_par_args[j][i]
+                r = func(**kwargs_0)
+                results.append(r)
             return results
         @ray.remote(memory=MEM_PER_WORKER)
         def get_results(**kwargs):
             try:
                 args_names = ray.get(args_names_put)
                 args_vals  = ray.get(args_vals_put)
                 kwargs2 = dict(zip(args_names, args_vals))
                 kwargs.update(kwargs2)
             except NameError:
                 pass
-            return f2(**kwargs)
+            results = f2(**kwargs)
+            return results
         
-        arg2parallelize = kwargs[list(kwargs.keys())[0]]
+        try:
+            n_args2parallelize = kwargs['n_args2parallelize']
+            # delete n_args2parallelize from kwargs
+            del kwargs['n_args2parallelize']
+        except KeyError:
+            n_args2parallelize = 1
+
+        par_args = list(kwargs.keys())[:n_args2parallelize]
+        arg2parallelize_unsplit = [kwargs[i] for i in par_args]
+
         # split into CPUS chunks
-        arg2parallelize = np.array_split(arg2parallelize, CPUS)
+        arg2parallelize = [np.array_split(i, CPUS) for i in arg2parallelize_unsplit]
 
-        arg_names = list(kwargs.keys())[1:]
-        arg_vals  = list(kwargs.values())[1:]
+        arg_names = list(kwargs.keys())[n_args2parallelize:]
+        arg_vals  = list(kwargs.values())[n_args2parallelize:]
 
         if len(arg_names) != 0:
             args_names_put = ray.put(arg_names)
             args_vals_put  = ray.put(arg_vals)
 
         workers = []
-        for i in range(len(arg2parallelize)):
-            if len(arg2parallelize[i]) == 0:
+        for i in range(len(arg2parallelize[0])):
+            if len(arg2parallelize[0][i]) == 0:
                 continue
-            par_arg    = {list(kwargs.keys())[0]:arg2parallelize[i]}
+            # par_arg    = {list(kwargs.keys())[0]:arg2parallelize[i]}
+            par_arg = {}
+            for j in range(len(par_args)):
+                par_arg[par_args[j]] = arg2parallelize[j][i]
             workers.append(get_results.remote(**par_arg))
         result = ray.get(workers)
 
-        if isinstance(result[0], tuple):
-            result = [list(r) for r in result]
-            r2 = list(result[0])
-            for i,r in enumerate(result):
-                if i == 0:
-                    continue
-                for j, r2i in enumerate(r):
-                    r2[j] = np.append(r2[j], r2i, axis=0)
-            for i, r2i in enumerate(r2):
-                r2[i] = np.concatenate(r2i)
-            result = tuple(r2)
-        else:
-            result = np.concatenate(result)
-
-        return result 
+        r_test = result[0][0]
+        try:
+            n_outputs = len(r_test)
+        except TypeError:
+            n_outputs = 1
+
+        results = []
+        for i in range(n_outputs):
+            results.append([])
+        for i in range(len(result)):
+            for j in range(len(result[i])):
+                for k in range(n_outputs):
+                    try:
+                        results[k].append(result[i][j][k])
+                    except TypeError:
+                        results[k].append(result[i][j])
+        return results
     return wrap 
 
 
 if __name__ == "__main__":
     import timeit
+    from scipy.integrate import quad
 
     @smart_parallelize
     def func(x, y):
-        sleep(1)
-        return x,y
+        fnc = lambda x: np.exp(-x*y)
+        return quad(fnc, 0, x)[0]
     
-    x = np.ones((15,6))
-    y = 64
+    x = np.ones((25,))
+    y = np.ones((25,))*2
+    # y = 2
     start  = timeit.default_timer()
-    answer = func(x=x, y=y)
+    answer = func(x=x, y=y, n_args2parallelize=2)
     stop  = timeit.default_timer()
     print(stop - start)
     print(answer)
 
 
     start  = timeit.default_timer()
     answer = []
```

### Comparing `smart_parallelize-1.0.7/PKG-INFO` & `smart_parallelize-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 1.0.7
+Version: 2.0.0
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

