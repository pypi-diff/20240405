# Comparing `tmp/richvalues-4.0.5.tar.gz` & `tmp/richvalues-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-4.0.5.tar", last modified: Tue Feb 27 09:06:53 2024, max compression
+gzip compressed data, was "richvalues-4.0.6.tar", last modified: Fri Apr  5 14:11:55 2024, max compression
```

## Comparing `richvalues-4.0.5.tar` & `richvalues-4.0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-02-27 09:06:53.090121 richvalues-4.0.5/
--rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-4.0.5/LICENSE
--rw-r--r--   0 andresmegias   (501) staff       (20)     1401 2024-02-27 09:06:53.089859 richvalues-4.0.5/PKG-INFO
--rw-rw-r--   0 andresmegias   (501) staff       (20)      835 2023-09-10 19:01:58.000000 richvalues-4.0.5/README.md
--rw-rw-r--   0 andresmegias   (501) staff       (20)      693 2024-02-27 09:04:37.000000 richvalues-4.0.5/pyproject.toml
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-02-27 09:06:53.086966 richvalues-4.0.5/richvalues/
--rw-rw-r--   0 andresmegias   (501) staff       (20)   201512 2024-02-27 09:03:44.000000 richvalues-4.0.5/richvalues/__init__.py
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-02-27 09:06:53.089533 richvalues-4.0.5/richvalues.egg-info/
--rw-r--r--   0 andresmegias   (501) staff       (20)     6148 2024-02-27 09:02:04.000000 richvalues-4.0.5/richvalues.egg-info/.DS_Store
--rw-r--r--   0 andresmegias   (501) staff       (20)     1401 2024-02-27 09:06:52.000000 richvalues-4.0.5/richvalues.egg-info/PKG-INFO
--rw-r--r--   0 andresmegias   (501) staff       (20)      263 2024-02-27 09:06:53.000000 richvalues-4.0.5/richvalues.egg-info/SOURCES.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)        1 2024-02-27 09:06:52.000000 richvalues-4.0.5/richvalues.egg-info/dependency_links.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       30 2024-02-27 09:06:52.000000 richvalues-4.0.5/richvalues.egg-info/requires.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       11 2024-02-27 09:06:52.000000 richvalues-4.0.5/richvalues.egg-info/top_level.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       38 2024-02-27 09:06:53.090239 richvalues-4.0.5/setup.cfg
--rw-rw-r--   0 andresmegias   (501) staff       (20)      869 2024-02-27 09:04:07.000000 richvalues-4.0.5/setup.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-04-05 14:11:55.135570 richvalues-4.0.6/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-4.0.6/LICENSE
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1407 2024-04-05 14:11:55.135310 richvalues-4.0.6/PKG-INFO
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      841 2024-04-02 13:16:34.000000 richvalues-4.0.6/README.md
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      693 2024-04-05 14:11:29.000000 richvalues-4.0.6/pyproject.toml
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-04-05 14:11:55.130948 richvalues-4.0.6/richvalues/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)   203292 2024-04-05 14:10:30.000000 richvalues-4.0.6/richvalues/__init__.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2024-04-05 14:11:55.134935 richvalues-4.0.6/richvalues.egg-info/
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1407 2024-04-05 14:11:55.000000 richvalues-4.0.6/richvalues.egg-info/PKG-INFO
+-rw-r--r--   0 andresmegias   (501) staff       (20)      233 2024-04-05 14:11:55.000000 richvalues-4.0.6/richvalues.egg-info/SOURCES.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)        1 2024-04-05 14:11:55.000000 richvalues-4.0.6/richvalues.egg-info/dependency_links.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       30 2024-04-05 14:11:55.000000 richvalues-4.0.6/richvalues.egg-info/requires.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       11 2024-04-05 14:11:55.000000 richvalues-4.0.6/richvalues.egg-info/top_level.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       38 2024-04-05 14:11:55.135683 richvalues-4.0.6/setup.cfg
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      869 2024-04-05 14:11:00.000000 richvalues-4.0.6/setup.py
```

### Comparing `richvalues-4.0.5/LICENSE` & `richvalues-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `richvalues-4.0.5/PKG-INFO` & `richvalues-4.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 4.0.5
+Version: 4.0.6
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/andresmegias/richvalues/blob/main/userguide.pdf
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
 
-With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/lower limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
 
 The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. A user guide and a quick tutorial are available on GitHub: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-4.0.5/README.md` & `richvalues-4.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
 
-With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/lower limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
 
 The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. A user guide and a quick tutorial are available on GitHub: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-4.0.5/pyproject.toml` & `richvalues-4.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "4.0.5"
+version = "4.0.6"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "description.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = ["Programming Language :: Python :: 3",
                "License :: OSI Approved :: BSD License",
```

### Comparing `richvalues-4.0.5/richvalues/__init__.py` & `richvalues-4.0.6/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '4.0.5'
+__version__ = '4.0.6'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import itertools
 import numpy as np
 import pandas as pd
@@ -234,15 +234,16 @@
             if m == 0:
                 num_digits_y = len(y)
                 num_digits_dy = len(dy)
                 m = n + int(num_digits_y - num_digits_dy)
                 num_digits_x = len(str(x).split('.')[0])
                 if num_digits_y > num_digits_x:
                     m -= 1
-                if float(dy[0]) <= extra_sf_lim:
+                base_dy = '{:e}'.format(float(dy)).split('e')[0]
+                if float(base_dy) <= extra_sf_lim:
                     m += 1
                 y = round_sf(x, m, min_exp, extra_sf_lim=1-1e-8)
         else:
             base_y, exp_y = '{:e}'.format(x).split('e')
             base_dy, exp_dy = '{:e}'.format(dx).split('e')
             exp_y, exp_dy = int(exp_y), int(exp_dy)
             d = exp_dy - exp_y
@@ -335,16 +336,18 @@
         diff = num_dec_2 - num_dec_1
         y1, dy1 = round_sf_unc(x, dx1, n+diff, min_exp, extra_sf_lim)
         y2, dy2 = round_sf_unc(x, dx2, n, min_exp, extra_sf_lim)
     else:
         diff = num_dec_1 - num_dec_2
         off1, off2 = 0, 0
         if num_dec_1 == 0 == num_dec_2:
-            b1 = float(str(dy1)[0]) if np.isfinite(dx1) else 10.
-            b2 = float(str(dy2)[0]) if np.isfinite(dx2) else 10.
+            base_dy1 = '{:e}'.format(dx1).split('e')[0]
+            base_dy2 = '{:e}'.format(dx2).split('e')[0]
+            b1 = float(base_dy1) if np.isfinite(dx1) else 10.
+            b2 = float(base_dy2) if np.isfinite(dx2) else 10.
             if dx2 > dx1 and b1 <= extra_sf_lim and b2 > extra_sf_lim:
                 off2 = 1
             if dx1 > dx2 and b2 <= extra_sf_lim and b1 > extra_sf_lim:
                 off1 = 1
         y1, dy1 = round_sf_unc(x, dx1, n+off1, min_exp, extra_sf_lim)
         y2, dy2 = round_sf_unc(x, dx2, n+diff+off2, min_exp, extra_sf_lim)
     y = y1 if dx2 > dx1 else y2
@@ -941,32 +944,33 @@
                 else:
                     if is_lolim:
                         symbol = '>'
                         y = int(np.floor(x)) if is_int else x  
                     elif is_uplim:
                         symbol = '<'
                         y = int(np.ceil(x)) if is_int else x  
-                    min_exp = 0
                     y = round_sf(y, n, min_exp, extra_sf_lim)
-                    y, a = y.split('e')
-                    a = str(int(a))
+                    if 'e' in y:
+                        y, a = y.split('e')
+                    else:
+                        a = '0'
                     text = ('${} {} {}'.format(symbol, y, mult_symbol)
                             + ' 10^{'+a+'}$')
-                text = text.replace('e-0', 'e-').replace('e+','e')
                 a = int(text.split('10^{')[1].split('}')[0])
                 if abs(a) < min_exp:
                     y = RichValue(x, dx, is_lolim, is_uplim,
                                   is_range, domain, is_int)
                     y.num_sf = n
                     y.min_exp = np.inf
                     y.extra_sf_lim = extra_sf_lim
                     text = y.latex(*kwargs)
                 if (not use_extra_sf_in_exacts and omit_ones_in_sci_notation
                      and dx[0] == dx[1] and dx[0] == 0 or np.isnan(dx[0])):
-                    text = text.replace('1 {} '.format(mult_symbol), '')
+                    if '.' not in text:
+                        text = text.replace('1 {} '.format(mult_symbol), '')
             else:
                 x1 = RichValue(main - unc[0], domain=domain)
                 x2 = RichValue(main + unc[1], domain=domain)
                 x1.min_exp = min_exp
                 x2.min_exp = min_exp
                 x1.range_bound = True
                 x2.range_bound = True
@@ -2659,15 +2663,15 @@
     """Sum two rich values to get a new one."""
     num_sf = min(x.num_sf, y.num_sf)
     min_exp = round(np.mean([x.min_exp, y.min_exp]))
     extra_sf_lim = max(x.extra_sf_lim, y.extra_sf_lim)
     is_int = x.is_int and y.is_int
     domain = [x.domain[0] + y.domain[0], x.domain[1] + y.domain[1]]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if x.is_exact or y.is_exact:
+    if (x.is_exact or y.is_exact) and (x.is_interv or y.is_interv):
         z = list(np.array(x.interval()) + np.array(y.interval()))
         z = RichValue(z, domain=domain, is_int=is_int)
     elif (not (x.is_interv or y.is_interv)
             and min(x.rel_ampl) > sigmas and min(y.rel_ampl) > sigmas):
         z = x.main + y.main
         dz = (np.array(x.unc)**2 + np.array(y.unc)**2)**0.5
         z = RichValue(z, dz, domain=domain, is_int=is_int)
@@ -2683,15 +2687,15 @@
     """Multiply two rich values to get a new one."""
     num_sf = min(x.num_sf, y.num_sf)
     min_exp = round(np.mean([x.min_exp, y.min_exp]))
     extra_sf_lim = max(x.extra_sf_lim, y.extra_sf_lim)
     is_int = x.is_int and y.is_int
     domain = propagate_domain(x.domain, y.domain, lambda a,b: a*b)
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if x.is_exact or y.is_exact:
+    if (x.is_exact or y.is_exact) and (x.is_interv or y.is_interv):
         z = list(np.array(x.interval()) * np.array(y.interval()))
         z = RichValue(z, domain=domain, is_int=is_int)
     elif (not (x.is_interv or y.is_interv)
          and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main * y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
         dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5 if z != 0. else 0.
@@ -3066,15 +3070,15 @@
             text1, text2 = text.split('--')
             x1, _, _, _, _, _, me1, el1 = parse_as_rich_value(text1)
             x2, _, _, _, _, _, me2, el2 = parse_as_rich_value(text2)
             main = [x1, x2]
             unc = 0
             is_lolim, is_uplim, is_range = False, False, True
             min_exp = round(np.mean([me1, me2]))
-            extra_sf_lim = min(el1, el2)
+            extra_sf_lim = max(el1, el2)
         return (main, unc, is_lolim, is_uplim, is_range, domain,
                 min_exp, extra_sf_lim)
     
     if pdf is None:
         text = str(text)
         is_complex = 'j' in text
         if not is_complex:
@@ -3199,15 +3203,15 @@
     domains = (np.array([domains[:,0].reshape(shape).tolist(),
                          domains[:,1].reshape(shape).tolist()])
                .transpose().reshape((*shape, 2)))
     are_ints = np.array(are_ints).reshape(shape)
     rarray = RichArray(mains, uncs, are_lolims, are_uplims, are_ranges,
                        domains, are_ints, variables, expressions)
     min_exp = round(np.mean(min_exps))
-    extra_sf_lim = min(extra_sf_lims)
+    extra_sf_lim = max(extra_sf_lims)
     rarray.set_params({'min_exp': min_exp, 'extra_sf_lim': extra_sf_lim})
     return rarray
 
 def rich_dataframe(df, domains=None, are_ints=None,
                    use_default_extra_sf_lim=False, **kwargs):
     """
     Convert the values of the input dataframe of text strings to rich values.
@@ -3578,15 +3582,15 @@
         np.random.shuffle(distr)
         if len(distr) != N:
             distr = distr[:N-2]
             distr = np.append(distr, [x1, x2])
     return distr
 
 def distr_with_rich_values(function, args, len_samples=None,
-                           is_vectorizable=False):
+                           is_vectorizable=False, **kwargs):
     """
     Same as function_with_rich_values, but just returns the final distribution.
     """
     if type(args) not in (tuple, list):
         args = [args]
     args = [rich_value(arg) if type(arg) not in (RichValue, ComplexRichValue)
             else arg for arg in args]
@@ -3684,15 +3688,15 @@
         x2 = np.sign(x2) * 10**zero_log
     elif x2 > 0 and x2 > 10**inf_log:
         x2 = 10**inf_log
     new_interval = [x1, x2]
     return new_interval
 
 def evaluate_distr(distr, domain=None, function=None, args=None,
-            len_samples=None, is_vectorizable=False, consider_intervs=True,
+            len_samples=None, is_vectorizable=False, consider_intervs=None,
             is_domain_cyclic=False, lims_fraction=None, num_reps_lims=None,
             save_pdf=None, **kwargs):
     """
     Interpret the given distribution as a rich value.
 
     Parameters
     ----------
@@ -3772,16 +3776,21 @@
             for j in range(num_vars):
                 all_vars[j] += [functions[j](distr)]
         return tuple(all_vars)
     
     if args is not None:
         if type(args) not in (tuple, list):
             args = [args]
-        args = [rich_value(arg) if type(arg) not in
-                (RichValue, ComplexRichValue) else arg for arg in args]
+        if type(args[0]) is not RichArray:
+            args = [rich_value(arg) if type(arg) not in
+                    (RichValue, ComplexRichValue) else arg for arg in args]
+    if consider_intervs is None:
+        consider_intervs = True
+        if args is not None and all([arg.is_centr for arg in args]):
+            consider_intervs = False
         
     distr = np.array(distr)
     
     is_complex = 'complex' in str(distr.dtype)
     if is_complex:
         if type(input_function) is str:
             function_real = 'np.real({})'.format(input_function)
@@ -4072,14 +4081,15 @@
         domain = add_zero_infs(domain, zero_log+6, inf_log-6)
         return domain
     
     if type(args) not in (tuple, list):
         args = [args]
     args = [rich_value(arg) if type(arg) not in (RichValue, ComplexRichValue)
             else arg for arg in args]
+    args_copy = copy.copy(args)
     
     input_function = copy.copy(function)
     if type(function) is str:
         variables = (list(np.concatenate(tuple(arg.variables for arg in args)))
                      if len(args) > 0 else [])
         variables = list(dict.fromkeys(variables).keys())
         vars_str = ','.join(variables)
@@ -4115,15 +4125,15 @@
             output = tuple(output)
         elif output_type is RichArray:
             output = np.array(output).view(RichArray)
         return output
             
     if len_samples is None:
         len_samples = int(len(args)**0.5 * defaultparams['size of samples'])
-    num_sf = min([arg.num_sf for arg in args])
+    num_sf = int(np.median([arg.num_sf for arg in args]))
     min_exp = round(np.mean([arg.min_exp for arg in args]))
     extra_sf_lim = max([arg.extra_sf_lim for arg in args])
     
     if consider_intervs is None:
         consider_intervs = (False if all([arg.is_centr for arg in args])
                             else True)
     use_analytic_propagation = (not any([arg.is_interv for arg in args])
@@ -4132,17 +4142,14 @@
         if (unc_function is None and (((unc_function is None and len(args) > 5))
                  or any([arg.prop_score < sigmas for arg in args]))):
             use_analytic_propagation = False
     elif unc_function is None:
             use_analytic_propagation = False
     
     args_main = np.array([arg.main for arg in args])
-    # print()
-    # print(args)
-    # print(args[0].expression)
     with np.errstate(divide='ignore', invalid='ignore'):
         main = function(*args_main)
     output_size = np.array(main).size
     output_type = RichArray if type(main) is np.ndarray else type(main)
     if is_vectorizable and output_size > 1:
         print("Warning: The argument 'is_vectorizable' only works with"
               "functions that return only one output.")
@@ -4220,24 +4227,22 @@
                 domain_k = [domain_k[0] - period, domain_k[1] + period]
         domains[k] = domain_k
     
     if use_analytic_propagation:
         
         mains = [main] if output_size == 1 else main
         if unc_function is not None:
-            args_unc = [np.array(arg.unc) for arg in args]
-            uncs = unc_function(*args_main, *args_unc)
+            uncs = []
+            args_main = np.array([arg.main for arg in args_copy])
+            for i in (0,1):
+                args_unc = [arg.unc[i] for arg in args_copy]
+                uncs += [unc_function(*args_main, *args_unc)]
             uncs = [uncs] if output_size == 1 else uncs
-            if output_size > 1:
-                for k in range(output_size):
-                    if not hasattr(uncs[k], '__iter__'):
-                        uncs[k] = [uncs[k]]*2
-                    uncs[k][1] = abs(uncs[k][1])
-            if not hasattr(uncs,'__iter__'):
-                uncs = [uncs]*output_size
+            for k in range(output_size):
+                uncs[k][1] = abs(uncs[k][1])
         else:
             inds_combs = list(itertools.product(*[[0,1,2]]*len(args)))
             comb_main = tuple([1]*len(args))
             inds_combs.remove(comb_main)
             args_combs = []
             args_all_vals = [[arg.main - arg.unc[0], arg.main,
                               arg.main + arg.unc[1]] for arg in args]
@@ -4257,14 +4262,17 @@
             domain_k = domains[k]
             if is_real:
                 rval_k = RichValue(main_k, unc_k, domain=domain_k)
             else:
                 real_k = RichValue(main_k.real, unc_k.real, domain=domain_k)
                 imag_k = RichValue(main_k.imag, unc_k.imag, domain=domain_k)
                 rval_k = ComplexRichValue(real_k, imag_k)
+            rval_k.num_sf = num_sf
+            rval_k.min_exp = min_exp
+            rval_k.extra_sf_lim = extra_sf_lim
             output += [rval_k]
             
     else:
         
         if optimize_len_samples:
             prop_score = min([arg.prop_score for arg in args])
             lim1, lim2 = 4., 20.
@@ -4332,14 +4340,45 @@
     * The rest of the arguments are the same as in 'function_with_rich_values'.
     
     Returns
     -------
     output : rich array / rich value
         Result of the function.
     """
+    if 'domain' in kwargs:
+        domain = kwargs['domain']
+        del kwargs['domain']
+    else:
+        domain = None
+    distr = distr_with_rich_arrays(function, args, elementwise, **kwargs)
+    if len(distr.shape) == 1:
+        output = evaluate_distr(distr, domain, function, args, **kwargs)
+    else:
+        output_size = distr.shape[1]
+        output = []
+        for k in range(output_size):
+            function_k = lambda *args: function(args)[k]
+            rval_k = evaluate_distr(distr[:,k], domain, function_k, args,
+                                    **kwargs)
+            output += [rval_k]
+        args_main = np.array([arg.main for arg in args])
+        with np.errstate(divide='ignore', invalid='ignore'):
+            main = function(*args_main)
+        output_size = np.array(main).size
+        output_type = RichArray if type(main) is np.ndarray else type(main)
+        if output_type is tuple and output_size > 1:
+            output = tuple(output)
+        elif output_type is RichArray:
+            output = np.array(output).view(RichArray)
+    return output
+
+def distr_with_rich_arrays(function, args, elementwise=False, **kwargs):
+    """
+    Same as function_with_rich_arrays, but just returns the final distribution.
+    """
     if type(args) not in (tuple, list):
         args = [args]
     args = [rich_array(arg) if type(arg) != RichArray else arg
             for arg in args]
     if elementwise and (len(args) > 0
             and type(args[0]) is str or not hasattr(args[0], '__iter__')):
         args = [rich_array(args)]
@@ -4347,31 +4386,32 @@
     else:
         args = [rich_array(arg) if type(arg) != RichArray else arg
                 for arg in args]
         shape = args[0].shape
     if 'len_samples' not in kwargs:
         kwargs['len_samples'] = int(len(args)**0.5
                                     * defaultparams['size of samples'])
+    if 'consider_intervs' in kwargs:
+        del kwargs['consider_intervs']
     if elementwise:
         same_shapes = True
         for arg in args[1:]:
             if arg.shape != shape:
                 same_shapes = False
                 break
         if not same_shapes:
             raise Exception('Input arrays have different shapes.')
-        array = np.empty(0, RichValue)
+        array = np.empty(0, float)
         args_flat = np.array([arg.flatten() for arg in args])
         for i in range(args[0].size):
             args_i = np.array(args_flat)[:,i].tolist()
-            rvalue = function_with_rich_values(function, args_i, **kwargs)
+            rvalue = distr_with_rich_values(function, args_i, **kwargs)
             array = np.append(array, rvalue)
         if shape == ():
             array = np.array(array[0])
-        array = array.view(RichArray)
         output = array
     else:
         if type(function) is str:
             variables = list(np.concatenate(tuple(arg.variables for arg in args)))
             variables = list(set(variables))
             expressions = [arg.expression for arg in args]
             function = function.replace('{}','({})')
@@ -4406,15 +4446,15 @@
                     arg_i = np.array(arg_i).reshape(arg_shapes[i])
                     rec_args += [arg_i]
                 y = function(*rec_args)
                 return y
             alt_args = []
             for arg in args:
                 alt_args += list(arg.flat)
-        output = function_with_rich_values(alt_function, alt_args, **kwargs)
+        output = distr_with_rich_values(alt_function, alt_args, **kwargs)
     return output
 
 def fmean(array, function='None', inverse_function='None',
           weights=None, weight_function=None, **kwargs):
     """
     Compute the generalized f-mean of the input values.
 
@@ -4520,20 +4560,20 @@
         else:
             r = 0
         factor = 2. + 12.*r**8
         return factor
     xa, ya = rich_array(x), rich_array(y)
     xc = rich_array([x]) if len(xa.shape) == 0 else xa
     yc = rich_array([y]) if len(ya.shape) == 0 else ya
-    if lims_factor is None:
-        lims_factor_x, lims_factor_y = None, None
-    elif type(lims_factor) in (float, int):
+    if type(lims_factor) in (float, int):
         lims_factor_x, lims_factor_y = [lims_factor]*2
     elif type(lims_factor) in (list, tuple):
         lims_factor_x, lims_factor_y = lims_factor
+    else:
+        lims_factor_x, lims_factor_y = None, None
     if lims_factor_x is None:
         lims_factor_x = lim_factor(xc)
     if lims_factor_y is None:
         lims_factor_y = lim_factor(yc)
     xc.set_lims_uncs(lims_factor_x)
     yc.set_lims_uncs(lims_factor_y)
     plt.plot()
@@ -4975,12 +5015,13 @@
 # Function acronyms.
 rval = rich_value
 rarray = rich_array
 rich_df = rdataframe = rich_dataframe
 function = function_with_rich_values
 array_function = function_with_rich_arrays
 distribution = distr_with_rich_values
+array_distribution = distr_with_rich_arrays
 evaluate_distribution = evaluate_distr
 center_and_uncertainties = center_and_uncs
 is_not_a_number = is_nan = isnan
 is_infinite = is_inf = isinf
 is_finite = is_finite = isfinite
```

### Comparing `richvalues-4.0.5/richvalues.egg-info/PKG-INFO` & `richvalues-4.0.6/richvalues.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 4.0.5
+Version: 4.0.6
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/andresmegias/richvalues/blob/main/userguide.pdf
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
 
-With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/lower limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
 
 The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. A user guide and a quick tutorial are available on GitHub: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-4.0.5/setup.py` & `richvalues-4.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '4.0.5',
+    version = '4.0.6',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues/',
```

