# Comparing `tmp/netsome-0.1.1.tar.gz` & `tmp/netsome-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.1.1.tar", max compression
+gzip compressed data, was "netsome-0.2.0.tar", max compression
```

## Comparing `netsome-0.1.1.tar` & `netsome-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1076 2024-03-27 09:32:36.724182 netsome-0.1.1/LICENSE
--rw-r--r--   0        0        0      144 2024-03-27 19:59:27.452194 netsome-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:13:03.131810 netsome-0.1.1/netsome/__init__.py
--rw-r--r--   0        0        0      115 2024-03-29 07:09:10.475947 netsome-0.1.1/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-03-31 17:48:55.416820 netsome-0.1.1/netsome/converters/__init__.py
--rw-r--r--   0        0        0      665 2024-03-31 18:26:56.511844 netsome-0.1.1/netsome/converters/bgp.py
--rw-r--r--   0        0        0        0 2024-03-29 07:02:52.497218 netsome-0.1.1/netsome/types/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-31 18:07:25.705804 netsome-0.1.1/netsome/types/bgp.py
--rw-r--r--   0        0        0      442 2024-03-29 07:10:04.563924 netsome-0.1.1/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-03-29 07:03:11.197676 netsome-0.1.1/netsome/validators/__init__.py
--rw-r--r--   0        0        0      949 2024-03-31 18:00:28.448394 netsome-0.1.1/netsome/validators/bgp.py
--rw-r--r--   0        0        0      288 2024-03-29 07:09:10.484949 netsome-0.1.1/netsome/validators/vlans.py
--rw-r--r--   0        0        0      950 2024-03-31 18:34:25.738130 netsome-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 netsome-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-27 09:32:36.724182 netsome-0.2.0/LICENSE
+-rw-r--r--   0        0        0      216 2024-04-05 20:13:03.123602 netsome-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 19:13:03.131810 netsome-0.2.0/netsome/__init__.py
+-rw-r--r--   0        0        0      254 2024-04-05 20:12:51.694562 netsome-0.2.0/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-03-29 07:02:52.497218 netsome-0.2.0/netsome/types/__init__.py
+-rw-r--r--   0        0        0     1606 2024-04-05 20:12:51.695230 netsome-0.2.0/netsome/types/bgp.py
+-rw-r--r--   0        0        0     4041 2024-04-05 20:12:51.695776 netsome-0.2.0/netsome/types/ipv4.py
+-rw-r--r--   0        0        0      429 2024-04-05 20:12:51.696340 netsome-0.2.0/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-03-29 07:03:11.197676 netsome-0.2.0/netsome/validators/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-05 20:12:51.697184 netsome-0.2.0/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     1838 2024-04-05 20:12:51.697727 netsome-0.2.0/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      288 2024-03-29 07:09:10.484949 netsome-0.2.0/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1017 2024-04-05 20:12:58.589978 netsome-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 netsome-0.2.0/PKG-INFO
```

### Comparing `netsome-0.1.1/LICENSE` & `netsome-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.1.1/netsome/validators/bgp.py` & `netsome-0.2.0/netsome/validators/bgp.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 def validate_asdotplus(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid asdot+ type, must be str")
 
     if c.DOT not in string:
         raise ValueError("Invalid asdot+ format, must be HIGH_ORDER.LOW_ORDER")
 
+    # FIXME
     validate_asplain(converters.asdotplus_to_asplain(string))
 
 
 def validate_asdot(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid asdot type, must be str")
```

### Comparing `netsome-0.1.1/pyproject.toml` & `netsome-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poe.env]
-DIRS = "netsome"
+DIRS = "netsome tests"
 
 [tool.poe.tasks.pretty]
 default_item_type = "cmd"
 sequence = [
   "poetry run autoflake --in-place --verbose --recursive $DIRS",
   "poetry run black $DIRS",
   "poetry run isort $DIRS",
@@ -15,27 +15,27 @@
 ]
 
 [tool.poe.tasks.tests]
 cmd = "poetry run pytest -vvv"
 
 [tool.poetry]
 authors = ["kuderr <dakudryavcev@gmail.com>"]
-description = ""
+classifiers = [
+  "Development Status :: 1 - Planning",
+  "Topic :: Software Development :: Libraries",
+  "Topic :: System :: Networking"
+]
+description = "The one and only library to make your network business code handsome"
+keywords = ["library", "network"]
 license = "MIT License"
 name = "netsome"
 readme = "README.md"
-version = "0.1.1"
 repository = "https://github.com/kuderr/netsome"
-keywords = ["library", "network"]
-classifiers = [
-    "Development Status :: 1 - Planning",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: System :: Networking",
-]
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
-toml-sort = "^0.23.1"
 pytest = "^8.1.1"
+toml-sort = "^0.23.1"
```

### Comparing `netsome-0.1.1/PKG-INFO` & `netsome-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.1.1
-Summary: 
+Version: 0.2.0
+Summary: The one and only library to make your network business code handsome
 Home-page: https://github.com/kuderr/netsome
 License: MIT
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -17,25 +17,31 @@
 Project-URL: Repository, https://github.com/kuderr/netsome
 Description-Content-Type: text/markdown
 
 TODO:
 
 types/validators:
 
-- asn
-- community
-- ipv4 address
-- ipv4 subnet
-- vlan
-- dns
-- mac
+- [x] asn
+- [ ] community
+- [x] ipv4 address
+- [x] ipv4 subnet
+- [x] vlan
+- [ ] dns
+- [ ] mac
 
 parsing:
 
 - ports
 
 utils:
 
 - resolve
 
 ranges/pools
 
+OTHER:
+
+- errors message
+- docs
+- comments
+
```

