# Comparing `tmp/zen-toolbox-0.1.65.tar.gz` & `tmp/zen-toolbox-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen-toolbox-0.1.65.tar", last modified: Wed Mar 27 13:18:44 2024, max compression
+gzip compressed data, was "zen-toolbox-0.1.70.tar", last modified: Fri Apr  5 17:04:36 2024, max compression
```

## Comparing `zen-toolbox-0.1.65.tar` & `zen-toolbox-0.1.70.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:18:44.432455 zen-toolbox-0.1.65/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-27 13:18:44.432455 zen-toolbox-0.1.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:18:44.432455 zen-toolbox-0.1.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:18:44.432455 zen-toolbox-0.1.65/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/toolbox/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/toolbox/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28436 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-27 13:18:36.000000 zen-toolbox-0.1.65/toolbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:18:44.432455 zen-toolbox-0.1.65/zen_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 13:18:44.000000 zen-toolbox-0.1.65/zen_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:04:36.968197 zen-toolbox-0.1.70/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-05 17:04:36.968197 zen-toolbox-0.1.70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:04:36.968197 zen-toolbox-0.1.70/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:04:36.964197 zen-toolbox-0.1.70/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/toolbox/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/toolbox/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28427 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 17:04:30.000000 zen-toolbox-0.1.70/toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:04:36.964197 zen-toolbox-0.1.70/zen_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 17:04:36.000000 zen-toolbox-0.1.70/zen_toolbox.egg-info/top_level.txt
```

### Comparing `zen-toolbox-0.1.65/setup.py` & `zen-toolbox-0.1.70/setup.py`

 * *Files identical despite different names*

### Comparing `zen-toolbox-0.1.65/toolbox/portfolio.py` & `zen-toolbox-0.1.70/toolbox/portfolio.py`

 * *Files identical despite different names*

### Comparing `zen-toolbox-0.1.65/toolbox/stats.py` & `zen-toolbox-0.1.70/toolbox/stats.py`

 * *Files identical despite different names*

### Comparing `zen-toolbox-0.1.65/toolbox/utils.py` & `zen-toolbox-0.1.70/toolbox/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         extra_prob_ex (float, optional): The probability of extra expenses. Defaults to 0.0.
         extra (list, optional): The list of extra values. Defaults to [].
 
     Returns:
         dict: A dictionary containing the final patrimonio, the patrimonio trajectory, and other related information.
     """
     extra = pd.DataFrame(
-        np.array(extra), columns=["months", "aportes", "despesas", "index"]
+        np.array(extra), columns=["months", "aportes", "despesas"]
     )
     df = pd.DataFrame(np.arange(1, months + 1, 1), columns=["months"])
     df["years"] = df["months"] / 12
     df["aportes"] = np.minimum(
         max_ap,
         (
             (df["months"] % freq_ap == 0)
```

