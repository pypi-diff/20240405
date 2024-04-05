# Comparing `tmp/testimony-2.3.0.tar.gz` & `tmp/testimony-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testimony-2.3.0.tar", last modified: Wed Jun 21 14:29:31 2023, max compression
+gzip compressed data, was "testimony-2.4.0.tar", last modified: Fri Apr  5 20:52:20 2024, max compression
```

## Comparing `testimony-2.3.0.tar` & `testimony-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.382362 testimony-2.3.0/
--rwxr-xr-x   0 elyezer    (501) staff       (20)    35121 2023-06-21 13:43:31.000000 testimony-2.3.0/LICENSE
--rw-r--r--   0 elyezer    (501) staff       (20)       35 2023-06-21 13:43:31.000000 testimony-2.3.0/MANIFEST.in
--rw-r--r--   0 elyezer    (501) staff       (20)     1089 2023-06-21 14:29:31.382240 testimony-2.3.0/PKG-INFO
--rw-r--r--   0 elyezer    (501) staff       (20)      469 2023-06-21 13:43:31.000000 testimony-2.3.0/README.rst
--rw-r--r--   0 elyezer    (501) staff       (20)        6 2023-06-21 14:25:35.000000 testimony-2.3.0/VERSION
--rw-r--r--   0 elyezer    (501) staff       (20)       38 2023-06-21 14:29:31.382400 testimony-2.3.0/setup.cfg
--rw-r--r--   0 elyezer    (501) staff       (20)     1155 2023-06-21 14:24:11.000000 testimony-2.3.0/setup.py
-drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.381323 testimony-2.3.0/testimony/
--rwxr-xr-x   0 elyezer    (501) staff       (20)    20591 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/__init__.py
--rw-r--r--   0 elyezer    (501) staff       (20)     1174 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/cli.py
--rw-r--r--   0 elyezer    (501) staff       (20)     2536 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/config.py
--rw-r--r--   0 elyezer    (501) staff       (20)     1032 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/constants.py
--rw-r--r--   0 elyezer    (501) staff       (20)     5187 2023-06-21 13:43:31.000000 testimony-2.3.0/testimony/parser.py
-drwxr-xr-x   0 elyezer    (501) staff       (20)        0 2023-06-21 14:29:31.382068 testimony-2.3.0/testimony.egg-info/
--rw-r--r--   0 elyezer    (501) staff       (20)     1089 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/PKG-INFO
--rw-r--r--   0 elyezer    (501) staff       (20)      349 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/SOURCES.txt
--rw-r--r--   0 elyezer    (501) staff       (20)        1 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/dependency_links.txt
--rw-r--r--   0 elyezer    (501) staff       (20)       54 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/entry_points.txt
--rw-r--r--   0 elyezer    (501) staff       (20)       32 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/requires.txt
--rw-r--r--   0 elyezer    (501) staff       (20)       10 2023-06-21 14:29:31.000000 testimony-2.3.0/testimony.egg-info/top_level.txt
+drwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)        0 2024-04-05 20:52:20.771588 testimony-2.4.0/
+-rwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)    35121 2024-04-04 19:57:27.000000 testimony-2.4.0/LICENSE
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)       35 2024-04-04 19:57:27.000000 testimony-2.4.0/MANIFEST.in
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     1333 2024-04-05 20:52:20.771588 testimony-2.4.0/PKG-INFO
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)      469 2024-04-04 19:57:27.000000 testimony-2.4.0/README.rst
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)        6 2024-04-05 20:43:54.000000 testimony-2.4.0/VERSION
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)       38 2024-04-05 20:52:20.771588 testimony-2.4.0/setup.cfg
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     1304 2024-04-04 19:57:27.000000 testimony-2.4.0/setup.py
+drwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)        0 2024-04-05 20:52:20.770588 testimony-2.4.0/testimony/
+-rwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)    22093 2024-04-04 19:57:27.000000 testimony-2.4.0/testimony/__init__.py
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     1273 2024-04-04 19:57:27.000000 testimony-2.4.0/testimony/cli.py
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     2536 2024-04-04 19:57:27.000000 testimony-2.4.0/testimony/config.py
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     1032 2024-04-04 19:57:27.000000 testimony-2.4.0/testimony/constants.py
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     5187 2024-04-04 19:57:27.000000 testimony-2.4.0/testimony/parser.py
+drwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)        0 2024-04-05 20:52:20.771588 testimony-2.4.0/testimony.egg-info/
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     1333 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/PKG-INFO
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)      370 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/SOURCES.txt
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)        1 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/dependency_links.txt
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)       54 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/entry_points.txt
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)       32 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/requires.txt
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)       10 2024-04-05 20:52:20.000000 testimony-2.4.0/testimony.egg-info/top_level.txt
+drwxr-xr-x   0 ogajduse  (1000) ogajduse  (1000)        0 2024-04-05 20:52:20.771588 testimony-2.4.0/tests/
+-rw-r--r--   0 ogajduse  (1000) ogajduse  (1000)     6872 2024-04-04 19:57:27.000000 testimony-2.4.0/tests/test_sample.py
```

### Comparing `testimony-2.3.0/LICENSE` & `testimony-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testimony-2.3.0/PKG-INFO` & `testimony-2.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: testimony
-Version: 2.3.0
+Version: 2.4.0
 Summary: Testimony inspects and reports on the python test cases.
 Home-page: https://github.com/SatelliteQE/testimony/
 Author: Suresh Thirugn
 Author-email: sthirugn@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Click
+Requires-Dist: termcolor
+Requires-Dist: docutils
+Requires-Dist: pyyaml
 
 Testimony
 =========
 
 Are you tired of managing your test cases in a test case management tool and
 your test code in a python automation framework?  Testimony can help to use
 the python automation framework as a test case repository tool.
```

### Comparing `testimony-2.3.0/setup.py` & `testimony-2.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     entry_points="""
         [console_scripts]
         testimony=testimony.cli:testimony
     """,
     description='Testimony inspects and reports on the python test cases.',
     long_description=long_description,
```

### Comparing `testimony-2.3.0/testimony/__init__.py` & `testimony-2.4.0/testimony/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     import termcolor
     HAS_TERMCOLOR = True
 except ImportError:
     HAS_TERMCOLOR = False
 
 SETTINGS = {
     'json': False,
+    'markdown': False,
     'nocolor': False,
     'tokens': {},
 }
 
 
 def indent(text, prefix, predicate=None):
     """Add 'prefix' to the beginning of selected lines in 'text'.
@@ -264,32 +265,71 @@
                     )
                     for key, value in sorted(self.invalid_tokens.items())
                 ])
             )
         return '\n'.join(output)
 
 
-def main(report, paths, json_output, nocolor):
+def main(report, paths, json_output, markdown_output, nocolor):
     """Entry point for the testimony project.
 
     Expects a valid report type and valid directory paths, hopefully argparse
     is taking care of validation
     """
     SETTINGS['json'] = json_output
+    SETTINGS['markdown'] = markdown_output
     SETTINGS['nocolor'] = nocolor
 
     if report == SUMMARY_REPORT:
         report_function = summary_report
     elif report == PRINT_REPORT:
         report_function = print_report
     elif report == VALIDATE_DOCSTRING_REPORT:
         report_function = validate_docstring_report
     sys.exit(report_function(get_testcases(paths)))
 
 
+def print_markdown(testcases):
+    """Print markdown formatted list of test cases.
+
+    :param testcases: A dict where the key is a path and value is a list of
+        found testcases on that path.
+    """
+    result = {}
+    for path, tests in testcases.items():
+        result[path] = [test.to_dict() for test in tests]
+        print('# {0}\n\n'.format(
+            colored(path, attrs=['bold'])))
+        if len(tests) == 0:
+            print('No test cases found.\n')
+        for test in tests:
+            title = testcase_title(test)
+            print('## {0}\n\n'.format(
+                title))
+            for token, data in test.to_dict().items():
+                if token == 'tokens':
+                    for key, value in data.items():
+                        print(f'### {key}\n')
+                        print(value)
+                        print('\n')
+                elif token == 'invalid-tokens':
+                    print('### invalid tokens')
+                    for key, value in data.items():
+                        print(f'* {key}: {value}')
+                    print('\n')
+                elif token == 'rst-parse-messages':
+                    for val in data:
+                        print(val)
+                else:
+                    raise ValueError(f'Invalid token: {token}')
+            print('\n')
+
+    return 0
+
+
 def print_report(testcases):
     """Print the list of test cases.
 
     :param testcases: A dict where the key is a path and value is a list of
         found testcases on that path.
     """
     if SETTINGS['json']:
@@ -308,14 +348,17 @@
                     'rst-parse-messages']
                 test_data['_testimony'] = testimony_metadata
                 result.append(test_data)
 
         print(json.dumps(result))
         return 0
 
+    if SETTINGS['markdown']:
+        return print_markdown(testcases)
+
     result = {}
     for path, tests in testcases.items():
         result[path] = [test.to_dict() for test in tests]
         print('{0}\n{1}\n'.format(
             colored(path, attrs=['bold']), '=' * len(path)))
         if len(tests) == 0:
             print('No test cases found.\n')
```

### Comparing `testimony-2.3.0/testimony/cli.py` & `testimony-2.4.0/testimony/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 import click
 
 from testimony import SETTINGS, config, constants, main
 
 
 @click.command()
 @click.option('-j', '--json', help='JSON output', is_flag=True)
+@click.option('-m', '--markdown', help='mardown output', is_flag=True)
 @click.option('-n', '--nocolor', default=False, help='Color output',
               is_flag=True)
 @click.option('--tokens', help='Comma separated list of expected tokens')
 @click.option(
     '--minimum-tokens', help='Comma separated list of minimum expected tokens')
 @click.option(
     '-c', '--config', 'config_file', type=click.File(),
     help='Configuration file (YAML)')
 @click.argument('report', type=click.Choice(constants.REPORT_TAGS))
 @click.argument('path', nargs=-1, type=click.Path(exists=True))
 def testimony(
-        json, nocolor, tokens, minimum_tokens, config_file, report, path):
+        json, markdown, nocolor, tokens, minimum_tokens, config_file,
+        report, path):
     """Inspect and report on the Python test cases."""
     if config_file:
         SETTINGS['tokens'] = config.parse_config(config_file)
     if tokens:
         config.update_tokens_dict(SETTINGS['tokens'], tokens)
     if minimum_tokens:
         config.update_tokens_dict(
             SETTINGS['tokens'], minimum_tokens, {'required': True})
-    main(report, path, json, nocolor)
+    main(report, path, json, markdown, nocolor)
```

### Comparing `testimony-2.3.0/testimony/config.py` & `testimony-2.4.0/testimony/config.py`

 * *Files identical despite different names*

### Comparing `testimony-2.3.0/testimony/constants.py` & `testimony-2.4.0/testimony/constants.py`

 * *Files identical despite different names*

### Comparing `testimony-2.3.0/testimony/parser.py` & `testimony-2.4.0/testimony/parser.py`

 * *Files identical despite different names*

### Comparing `testimony-2.3.0/testimony.egg-info/PKG-INFO` & `testimony-2.4.0/testimony.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: testimony
-Version: 2.3.0
+Version: 2.4.0
 Summary: Testimony inspects and reports on the python test cases.
 Home-page: https://github.com/SatelliteQE/testimony/
 Author: Suresh Thirugn
 Author-email: sthirugn@redhat.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Click
+Requires-Dist: termcolor
+Requires-Dist: docutils
+Requires-Dist: pyyaml
 
 Testimony
 =========
 
 Are you tired of managing your test cases in a test case management tool and
 your test code in a python automation framework?  Testimony can help to use
 the python automation framework as a test case repository tool.
```

