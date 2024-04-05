# Comparing `tmp/pydqt-1.3.7.tar.gz` & `tmp/pydqt-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydqt-1.3.7.tar", max compression
+gzip compressed data, was "pydqt-1.3.8.tar", max compression
```

## Comparing `pydqt-1.3.7.tar` & `pydqt-1.3.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    17476 2024-04-05 11:55:14.501674 pydqt-1.3.7/README.md
--rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.7/pydqt/__init__.py
--rw-r--r--   0        0        0    35253 2024-04-05 11:01:13.511539 pydqt-1.3.7/pydqt/pydqt.py
--rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.7/pydqt/sql/templates/macros/macros.jinja
--rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.7/pydqt/test.csv
--rw-r--r--   0        0        0     6687 2024-04-05 11:52:33.920281 pydqt-1.3.7/pydqt/tests/test_querying.py
--rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.7/pydqt/utils/__init__.py
--rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.7/pydqt/utils/custom_filters.py
--rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.7/pydqt/workspaces/main/templates/base.sql
--rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.7/pydqt/workspaces/main/templates/example.sql
--rw-r--r--   0        0        0      684 2024-04-05 11:56:23.240091 pydqt-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    18372 1970-01-01 00:00:00.000000 pydqt-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    17476 2024-04-05 11:55:14.501674 pydqt-1.3.8/README.md
+-rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.8/pydqt/__init__.py
+-rw-r--r--   0        0        0    35531 2024-04-05 12:19:47.521897 pydqt-1.3.8/pydqt/pydqt.py
+-rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.8/pydqt/sql/templates/macros/macros.jinja
+-rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.8/pydqt/test.csv
+-rw-r--r--   0        0        0     6687 2024-04-05 11:52:33.920281 pydqt-1.3.8/pydqt/tests/test_querying.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.8/pydqt/utils/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.8/pydqt/utils/custom_filters.py
+-rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.8/pydqt/workspaces/main/templates/base.sql
+-rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.8/pydqt/workspaces/main/templates/example.sql
+-rw-r--r--   0        0        0      684 2024-04-05 12:20:32.656522 pydqt-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0    18372 1970-01-01 00:00:00.000000 pydqt-1.3.8/PKG-INFO
```

### Comparing `pydqt-1.3.7/README.md` & `pydqt-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.7/pydqt/__init__.py` & `pydqt-1.3.8/pydqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.7/pydqt/pydqt.py` & `pydqt-1.3.8/pydqt/pydqt.py`

 * *Files 1% similar despite different names*

```diff
@@ -934,25 +934,29 @@
             os.remove(full_filename)
 
             rendered_str = template.render(kwargs)
             pattern = '\'[A-Za-z0-9_.-\/]+\.csv\''
             m=re.findall(pattern, rendered_str)
             if len(m)>0:
                 rendered_str=rendered_str.replace(m[0],f'read_csv_auto({m[0]}, header=true)')    
+            # handle ':language' lower case issue
+            rendered_str = rendered_str.replace(':LANGUAGE',':language')     
             return (False,rendered_str)
         else:
             for key,val in kwargs.items():
                 s=s.replace('{{' + key + '}}',val)
             rendered_str=s                
             pattern = '\'[A-Za-z0-9_.-\/]+\.csv\''
             m=re.findall(pattern, rendered_str)
             if len(m)>0:
                 rendered_str=rendered_str.replace(m[0],f'read_csv_auto({m[0]}, header=true)')    
+            rendered_str = rendered_str.replace(':LANGUAGE',':language')    
             return (False,rendered_str)            
     else:
         template = environment.get_template(template)
         rendered_str = template.render(kwargs)
         pattern = '\'[A-Za-z0-9_.-\/]+\.csv\''
         m=re.findall(pattern, rendered_str)
         if len(m)>0:
             rendered_str=rendered_str.replace(m[0],f'read_csv_auto({m[0]}, header=true)')    
+        rendered_str = rendered_str.replace(':LANGUAGE',':language')    
         return (True,rendered_str)
```

### Comparing `pydqt-1.3.7/pydqt/sql/templates/macros/macros.jinja` & `pydqt-1.3.8/pydqt/sql/templates/macros/macros.jinja`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.7/pydqt/test.csv` & `pydqt-1.3.8/pydqt/test.csv`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.7/pydqt/tests/test_querying.py` & `pydqt-1.3.8/pydqt/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.7/pyproject.toml` & `pydqt-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydqt"
-version = "1.3.7"
+version = "1.3.8"
 description = "A package to help parameterise and macrofy sql queries"
 authors = ["Mark Ingham <mark.ingham@ly.st>"]
 readme = "README.md"
 repository = "https://github.com/markingham77/dqt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `pydqt-1.3.7/PKG-INFO` & `pydqt-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydqt
-Version: 1.3.7
+Version: 1.3.8
 Summary: A package to help parameterise and macrofy sql queries
 Home-page: https://github.com/markingham77/dqt
 License: MIT
 Author: Mark Ingham
 Author-email: mark.ingham@ly.st
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

