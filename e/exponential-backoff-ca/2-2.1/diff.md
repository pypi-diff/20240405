# Comparing `tmp/exponential_backoff_ca-2.tar.gz` & `tmp/exponential_backoff_ca-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponential_backoff_ca-2.tar", last modified: Wed Apr  3 20:30:16 2024, max compression
+gzip compressed data, was "exponential_backoff_ca-2.1.tar", last modified: Thu Apr  4 23:00:14 2024, max compression
```

## Comparing `exponential_backoff_ca-2.tar` & `exponential_backoff_ca-2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:30:16.212189 exponential_backoff_ca-2/
--rw-r--r--   0 root         (0) root         (0)     1006 2024-04-03 20:30:16.212189 exponential_backoff_ca-2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      617 2024-04-03 20:30:03.000000 exponential_backoff_ca-2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:30:16.208189 exponential_backoff_ca-2/exponential_backoff_ca/
--rw-r--r--   0 root         (0) root         (0)     3986 2024-04-03 20:30:03.000000 exponential_backoff_ca-2/exponential_backoff_ca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:30:16.212189 exponential_backoff_ca-2/exponential_backoff_ca.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1006 2024-04-03 20:30:16.000000 exponential_backoff_ca-2/exponential_backoff_ca.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-03 20:30:16.000000 exponential_backoff_ca-2/exponential_backoff_ca.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:30:16.000000 exponential_backoff_ca-2/exponential_backoff_ca.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-03 20:30:16.000000 exponential_backoff_ca-2/exponential_backoff_ca.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      624 2024-04-03 20:30:03.000000 exponential_backoff_ca-2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 20:30:16.212189 exponential_backoff_ca-2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:00:14.073246 exponential_backoff_ca-2.1/
+-rw-r--r--   0 root         (0) root         (0)     5233 2024-04-04 23:00:14.073246 exponential_backoff_ca-2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4842 2024-04-04 23:00:01.000000 exponential_backoff_ca-2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:00:14.073246 exponential_backoff_ca-2.1/exponential_backoff_ca/
+-rw-r--r--   0 root         (0) root         (0)     4026 2024-04-04 23:00:01.000000 exponential_backoff_ca-2.1/exponential_backoff_ca/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 23:00:14.073246 exponential_backoff_ca-2.1/exponential_backoff_ca.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5233 2024-04-04 23:00:14.000000 exponential_backoff_ca-2.1/exponential_backoff_ca.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-04 23:00:14.000000 exponential_backoff_ca-2.1/exponential_backoff_ca.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 23:00:14.000000 exponential_backoff_ca-2.1/exponential_backoff_ca.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 23:00:14.000000 exponential_backoff_ca-2.1/exponential_backoff_ca.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      626 2024-04-04 23:00:01.000000 exponential_backoff_ca-2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 23:00:14.073246 exponential_backoff_ca-2.1/setup.cfg
```

### Comparing `exponential_backoff_ca-2/exponential_backoff_ca/__init__.py` & `exponential_backoff_ca-2.1/exponential_backoff_ca/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,25 +90,25 @@
         """What to do on the next iteration
         """
         if self.counter < self.number_of_iterations:
             self.counter += 1
 
             self.progress(f"counter is: {self.counter}")
 
-            # Calculate how many slots. This will be
+            # Calculate how many available slots. This will be
             # a random integer in [0, (self.multiplier)**(self.counter) - 1].
-            max_slots = int(self.multiplier**(self.counter) - 1)
-            if ((self.max_slots is not None) and (max_slots > self.max_slots)):
+            available_slots = int(self.multiplier**(self.counter) - 1)
+            if ((self.max_slots is not None) and (available_slots > self.max_slots)):
                 self.progress(f"max slots limit of {self.max_slots} reached")
-                max_slots = self.max_slots
+                available_slots = self.max_slots
 
-            msg = f"will choose number of slots randomly from [0, {max_slots}]"
+            msg = f"will choose number of slots randomly from [0, {available_slots}]"
             self.progress(msg)
 
-            number_slots = random.randint(0, max_slots)
+            number_slots = random.randint(0, available_slots)
             self.progress(f"number of slots chosen: {number_slots}")
 
             wait_time = number_slots * self.slot_time
 
             if ((self.limit_value is not None) and (wait_time > self.limit_value)):
                 msg =f"limit value exceeded; returning limit of {self.limit_value}"
                 self.progress(msg)
```

### Comparing `exponential_backoff_ca-2/pyproject.toml` & `exponential_backoff_ca-2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exponential_backoff_ca"
-version = "2"
+version = "2.1"
 description = "An exponential backoff iterator with collision avoidance."
 readme = "README.md"
 requires-python = ">= 3.9"
 authors = [
   {name = "IEDO Team"},
 ]
 classifiers = [
```

