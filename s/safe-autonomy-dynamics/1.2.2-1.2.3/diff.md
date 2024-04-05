# Comparing `tmp/safe_autonomy_dynamics-1.2.2.tar.gz` & `tmp/safe_autonomy_dynamics-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_autonomy_dynamics-1.2.2.tar", max compression
+gzip compressed data, was "safe_autonomy_dynamics-1.2.3.tar", max compression
```

## Comparing `safe_autonomy_dynamics-1.2.2.tar` & `safe_autonomy_dynamics-1.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       34 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/LICENSE
--rw-r--r--   0        0        0     3158 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/README.md
--rw-r--r--   0        0        0      207 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/docs/api/cwh/index.md
--rw-r--r--   0        0        0      379 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/docs/api/external/aerobench/index.md
--rw-r--r--   0        0        0       68 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/docs/api/external/aerobench/lowlevel/index.md
--rw-r--r--   0        0        0       98 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/docs/api/external/index.md
--rw-r--r--   0        0        0      185 2024-03-18 19:07:29.485242 safe_autonomy_dynamics-1.2.2/docs/api/index.md
--rw-r--r--   0        0        0       90 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/css/material.css
--rw-r--r--   0        0        0      263 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      895 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/css/style.css
--rw-r--r--   0        0        0     2509 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/developer-guide.md
--rw-r--r--   0        0        0      678 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/gen_ref_nav.py
--rw-r--r--   0        0        0       48 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/index.md
--rw-r--r--   0        0        0     2045 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/install.md
--rw-r--r--   0        0        0      300 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0     1390 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/docs/user-guide.md
--rw-r--r--   0        0        0     1909 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/__init__.py
--rw-r--r--   0        0        0    25887 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/base_models.py
--rw-r--r--   0        0        0      547 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/__init__.py
--rw-r--r--   0        0        0    10026 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/point_model.py
--rw-r--r--   0        0        0    15568 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/rotational_model.py
--rw-r--r--   0        0        0    21360 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/sixdof_model.py
--rw-r--r--   0        0        0     3922 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/sun_model.py
--rw-r--r--   0        0        0    21092 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/dubins.py
--rw-r--r--   0        0        0        0 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/__init__.py
--rw-r--r--   0        0        0     2391 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/controlled_f16.py
--rw-r--r--   0        0        0        0 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/__init__.py
--rw-r--r--   0        0        0     1367 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/adc.py
--rw-r--r--   0        0        0     1935 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cl.py
--rw-r--r--   0        0        0     2450 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/clf16.py
--rw-r--r--   0        0        0     1725 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cm.py
--rw-r--r--   0        0        0     1883 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cn.py
--rw-r--r--   0        0        0     1812 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/conf16.py
--rw-r--r--   0        0        0     1729 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cx.py
--rw-r--r--   0        0        0      620 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cy.py
--rw-r--r--   0        0        0     1092 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cz.py
--rw-r--r--   0        0        0     1917 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dampp.py
--rw-r--r--   0        0        0     1975 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dlda.py
--rw-r--r--   0        0        0     1897 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dldr.py
--rw-r--r--   0        0        0     1937 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dnda.py
--rw-r--r--   0        0        0     1977 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dndr.py
--rw-r--r--   0        0        0     4053 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/low_level_controller.py
--rw-r--r--   0        0        0     6091 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/morellif16.py
--rw-r--r--   0        0        0      958 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/pdot.py
--rw-r--r--   0        0        0      681 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/rtau.py
--rw-r--r--   0        0        0     6616 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/subf16_model.py
--rw-r--r--   0        0        0      664 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/tgear.py
--rw-r--r--   0        0        0     2567 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/thrust.py
--rw-r--r--   0        0        0     9295 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/util.py
--rw-r--r--   0        0        0    12140 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/integrators.py
--rw-r--r--   0        0        0     1845 2024-03-18 19:07:29.489242 safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/utils.py
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 safe_autonomy_dynamics-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/LICENSE
+-rw-r--r--   0        0        0     3158 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/README.md
+-rw-r--r--   0        0        0      207 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/api/cwh/index.md
+-rw-r--r--   0        0        0      379 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/api/external/aerobench/index.md
+-rw-r--r--   0        0        0       68 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/api/external/aerobench/lowlevel/index.md
+-rw-r--r--   0        0        0       98 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/api/external/index.md
+-rw-r--r--   0        0        0      185 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/api/index.md
+-rw-r--r--   0        0        0       90 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/css/material.css
+-rw-r--r--   0        0        0      263 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      895 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/css/style.css
+-rw-r--r--   0        0        0     2509 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/developer-guide.md
+-rw-r--r--   0        0        0      678 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0       48 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/index.md
+-rw-r--r--   0        0        0     2045 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/install.md
+-rw-r--r--   0        0        0      300 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0     1390 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/docs/user-guide.md
+-rw-r--r--   0        0        0     1910 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/__init__.py
+-rw-r--r--   0        0        0    25887 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/base_models.py
+-rw-r--r--   0        0        0      547 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/__init__.py
+-rw-r--r--   0        0        0    10026 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/point_model.py
+-rw-r--r--   0        0        0    15568 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/rotational_model.py
+-rw-r--r--   0        0        0    21360 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/sixdof_model.py
+-rw-r--r--   0        0        0     3922 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/sun_model.py
+-rw-r--r--   0        0        0    21092 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/dubins.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/__init__.py
+-rw-r--r--   0        0        0     2391 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/controlled_f16.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/__init__.py
+-rw-r--r--   0        0        0     1367 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/adc.py
+-rw-r--r--   0        0        0     1935 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cl.py
+-rw-r--r--   0        0        0     2450 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/clf16.py
+-rw-r--r--   0        0        0     1725 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cm.py
+-rw-r--r--   0        0        0     1883 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cn.py
+-rw-r--r--   0        0        0     1812 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/conf16.py
+-rw-r--r--   0        0        0     1729 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cx.py
+-rw-r--r--   0        0        0      620 2024-04-05 17:26:30.562127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cy.py
+-rw-r--r--   0        0        0     1092 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cz.py
+-rw-r--r--   0        0        0     1917 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dampp.py
+-rw-r--r--   0        0        0     1975 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dlda.py
+-rw-r--r--   0        0        0     1897 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dldr.py
+-rw-r--r--   0        0        0     1937 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dnda.py
+-rw-r--r--   0        0        0     1977 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dndr.py
+-rw-r--r--   0        0        0     4053 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/low_level_controller.py
+-rw-r--r--   0        0        0     6091 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/morellif16.py
+-rw-r--r--   0        0        0      958 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/pdot.py
+-rw-r--r--   0        0        0      681 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/rtau.py
+-rw-r--r--   0        0        0     6616 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/subf16_model.py
+-rw-r--r--   0        0        0      664 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/tgear.py
+-rw-r--r--   0        0        0     2567 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/thrust.py
+-rw-r--r--   0        0        0     9295 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/util.py
+-rw-r--r--   0        0        0    12140 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/integrators.py
+-rw-r--r--   0        0        0     1845 2024-04-05 17:26:30.566127 safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/utils.py
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 safe_autonomy_dynamics-1.2.3/PKG-INFO
```

### Comparing `safe_autonomy_dynamics-1.2.2/README.md` & `safe_autonomy_dynamics-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/docs/css/style.css` & `safe_autonomy_dynamics-1.2.3/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/docs/developer-guide.md` & `safe_autonomy_dynamics-1.2.3/docs/developer-guide.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/docs/gen_ref_nav.py` & `safe_autonomy_dynamics-1.2.3/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/docs/install.md` & `safe_autonomy_dynamics-1.2.3/docs/install.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/docs/user-guide.md` & `safe_autonomy_dynamics-1.2.3/docs/user-guide.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/pyproject.toml` & `safe_autonomy_dynamics-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-autonomy-dynamics"
-version = "1.2.2"
+version = "1.2.3"
 description = "The safe-autonomy-dynamics package provides an API for dynamic systems supported by a library of common functions used to access and update system dynamics."
 authors = [
     "Charles Keating <Charles.Keating@udri.udayton.edu>",
 ]
 license = ""
 readme = "README.md"
 homepage = "https://github.com/act3-ace/safe-autonomy-dynamics.git"
@@ -19,15 +19,15 @@
 packages = [
         {include = "safe_autonomy_dynamics"},
     ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 numpy = "^1.23.5"
-jax = { version = "0.4.3", extras = ["cpu"], optional = true }
+jax = { version = "0.4.26", extras = ["cpu"], optional = true }
 scipy = ">=1.10.0"
 pydantic = "^2.6.2"
 pint = "^0.22"
 
 [tool.poetry.extras]
 jax = ["jax"]
```

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/base_models.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/base_models.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/__init__.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/point_model.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/point_model.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/rotational_model.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/rotational_model.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/sixdof_model.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/sixdof_model.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/cwh/sun_model.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/cwh/sun_model.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/dubins.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/dubins.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/controlled_f16.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/controlled_f16.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/adc.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/adc.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cl.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cl.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/clf16.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/clf16.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cm.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cm.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cn.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cn.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/conf16.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/conf16.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cx.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cx.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cy.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cy.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/cz.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/cz.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dampp.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dampp.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dlda.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dlda.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dldr.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dldr.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dnda.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dnda.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/dndr.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/dndr.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/low_level_controller.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/low_level_controller.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/morellif16.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/morellif16.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/pdot.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/pdot.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/rtau.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/rtau.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/subf16_model.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/subf16_model.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/tgear.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/tgear.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/lowlevel/thrust.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/lowlevel/thrust.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/external/aerobench/util.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/external/aerobench/util.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/integrators.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/integrators.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/safe_autonomy_dynamics/utils.py` & `safe_autonomy_dynamics-1.2.3/safe_autonomy_dynamics/utils.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_dynamics-1.2.2/PKG-INFO` & `safe_autonomy_dynamics-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: safe-autonomy-dynamics
-Version: 1.2.2
+Version: 1.2.3
 Summary: The safe-autonomy-dynamics package provides an API for dynamic systems supported by a library of common functions used to access and update system dynamics.
 Home-page: https://github.com/act3-ace/safe-autonomy-dynamics.git
 Author: Charles Keating
 Author-email: Charles.Keating@udri.udayton.edu
 Requires-Python: >=3.9,<3.13
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: jax
-Requires-Dist: jax[cpu] (==0.4.3) ; extra == "jax"
+Requires-Dist: jax[cpu] (==0.4.26) ; extra == "jax"
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pint (>=0.22,<0.23)
 Requires-Dist: pydantic (>=2.6.2,<3.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Project-URL: Documentation, https://github.com/act3-ace/safe-autonomy-dynamics/docs
 Project-URL: Repository, https://github.com/act3-ace/safe-autonomy-dynamics.git
 Description-Content-Type: text/markdown
```

