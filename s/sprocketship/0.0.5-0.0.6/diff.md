# Comparing `tmp/sprocketship-0.0.5.tar.gz` & `tmp/sprocketship-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.0.5.tar", last modified: Fri Apr  5 16:23:42 2024, max compression
+gzip compressed data, was "sprocketship-0.0.6.tar", last modified: Fri Apr  5 16:46:43 2024, max compression
```

## Comparing `sprocketship-0.0.5.tar` & `sprocketship-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:23:42.936117 sprocketship-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:23:35.000000 sprocketship-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:23:42.936117 sprocketship-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-05 16:23:35.000000 sprocketship-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:23:35.000000 sprocketship-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:23:42.936117 sprocketship-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:23:42.932117 sprocketship-0.0.5/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-05 16:23:35.000000 sprocketship-0.0.5/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:23:42.936117 sprocketship-0.0.5/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:23:42.000000 sprocketship-0.0.5/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 16:46:36.000000 sprocketship-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:46:43.510169 sprocketship-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-05 16:46:36.000000 sprocketship-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 16:46:36.000000 sprocketship-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:46:43.510169 sprocketship-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-05 16:46:36.000000 sprocketship-0.0.6/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:43.510169 sprocketship-0.0.6/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 16:46:43.000000 sprocketship-0.0.6/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.0.5/LICENSE` & `sprocketship-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.5/PKG-INFO` & `sprocketship-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.5 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.6 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

### Comparing `sprocketship-0.0.5/README.md` & `sprocketship-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.0.5/pyproject.toml` & `sprocketship-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "click",
     "snowflake",
```

### Comparing `sprocketship-0.0.5/sprocketship/cli.py` & `sprocketship-0.0.6/sprocketship/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 def get_file_contents(fpath):
     with open(fpath, 'r') as file:
         return file.read()
 
 
 def create_javascript_stored_procedure(**kwargs):
-  path = get_full_file_path(kwargs)
+  path = os.path.join(kwargs['project_dir'], get_full_file_path(kwargs))
   procedure_def_dict = {'procedure_definition': get_file_contents(path)}
   create_proc_text = '''
 CREATE {%if replace_if_exists %}OR REPLACE{% endif %} PROCEDURE {{database}}.{{schema}}.{{name}} (
 {%- for arg_name, arg_data_type in args.items() %}
 "{{arg_name.upper()}}" {{arg_data_type.upper()}}{%if not loop.last %},{% endif %}
 {%- endfor -%}
 )
@@ -71,15 +71,15 @@
 
         # Get the configurations for each procedure and attach relative path to file directory
         configs_with_paths = extract_configs(data["procedures"])
         procs = list(itertools.chain(*configs_with_paths.values()))
 
         for proc in procs:
             try:
-                rendered_proc = create_javascript_stored_procedure(**proc)
+                rendered_proc = create_javascript_stored_procedure(**proc, **{'project_dir': dir})
                 con.cursor().execute(rendered_proc)
                 msg = click.style(f"{proc['name']} ", fg='green', bold=True)
                 msg += click.style(f"launched into schema ", fg='white', bold=True)
                 msg += click.style(f"{proc['database']}.{proc['schema']}", fg='blue', bold=True)
                 click.echo(msg)
             except Exception as e:
                 msg = click.style(f"{proc['name']} ", fg='red', bold=True)
```

### Comparing `sprocketship-0.0.5/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.0.6/sprocketship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.0.5 Author-email: Nicklaus
+Metadata-Version: 2.1 Name: sprocketship Version: 0.0.6 Author-email: Nicklaus
 Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

