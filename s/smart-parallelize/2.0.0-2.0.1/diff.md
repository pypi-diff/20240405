# Comparing `tmp/smart_parallelize-2.0.0.tar.gz` & `tmp/smart_parallelize-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.0.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.1.tar", max compression
```

## Comparing `smart_parallelize-2.0.0.tar` & `smart_parallelize-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.0/README.md
--rw-r--r--   0        0        0      316 2024-04-05 16:29:58.539934 smart_parallelize-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.0/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4178 2024-04-05 16:56:11.231984 smart_parallelize-2.0.0/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 smart_parallelize-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.1/README.md
+-rw-r--r--   0        0        0      316 2024-04-05 18:17:41.204659 smart_parallelize-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.1/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4285 2024-04-05 18:16:25.834211 smart_parallelize-2.0.1/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 smart_parallelize-2.0.1/PKG-INFO
```

### Comparing `smart_parallelize-2.0.0/README.md` & `smart_parallelize-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.0/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.1/smart_parallelize/parallelize.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 	MEMORY, CPUS, MEM_PER_WORKER = get_mem_func()
 
 def smart_parallelize(func): 
     '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
 
     def wrap(**kwargs): 
         def f2(**kwargs):
+            print(kwargs)
             par_args = list(kwargs.keys())[:n_args2parallelize]
             data_par_args = [kwargs[i] for i in par_args]
             results = []
             for i, _ in enumerate(data_par_args[0]):
                 kwargs_0 = kwargs.copy()
                 for j, _ in enumerate(data_par_args):
                     kwargs_0[par_args[j]] = data_par_args[j][i]
+                print('kwargs_0', kwargs_0)
                 r = func(**kwargs_0)
                 results.append(r)
             return results
         @ray.remote(memory=MEM_PER_WORKER)
         def get_results(**kwargs):
             try:
                 args_names = ray.get(args_names_put)
@@ -97,31 +99,32 @@
         for i in range(n_outputs):
             results.append([])
         for i in range(len(result)):
             for j in range(len(result[i])):
                 for k in range(n_outputs):
                     try:
                         results[k].append(result[i][j][k])
-                    except TypeError:
+                    except (TypeError, IndexError):
                         results[k].append(result[i][j])
         return results
     return wrap 
 
 
 if __name__ == "__main__":
     import timeit
     from scipy.integrate import quad
 
     @smart_parallelize
     def func(x, y):
+        x = np.sum(x)
         fnc = lambda x: np.exp(-x*y)
         return quad(fnc, 0, x)[0]
     
-    x = np.ones((25,))
-    y = np.ones((25,))*2
+    x = np.ones((30,2))
+    y = np.ones((30,))*2
     # y = 2
     start  = timeit.default_timer()
     answer = func(x=x, y=y, n_args2parallelize=2)
     stop  = timeit.default_timer()
     print(stop - start)
     print(answer)
```

### Comparing `smart_parallelize-2.0.0/PKG-INFO` & `smart_parallelize-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

