# Comparing `tmp/localconfig-1.1.3.tar.gz` & `tmp/localconfig-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/localconfig-1.1.3.tar", last modified: Tue May 14 21:44:05 2019, max compression
+gzip compressed data, was "localconfig-1.1.4.tar", last modified: Fri Apr  5 01:59:37 2024, max compression
```

## Comparing `localconfig-1.1.3.tar` & `localconfig-1.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mzheng    (1000) root         (0)        0 2019-05-14 21:44:05.000000 localconfig-1.1.3/
-drwxr-xr-x   0 mzheng    (1000) root         (0)        0 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig/
--rw-r--r--   0 mzheng    (1000) root         (0)    14595 2018-07-19 05:58:32.000000 localconfig-1.1.3/localconfig/manager.py
--rw-r--r--   0 mzheng    (1000) root         (0)       68 2018-06-19 05:57:53.000000 localconfig-1.1.3/localconfig/__init__.py
--rw-r--r--   0 mzheng    (1000) root         (0)      873 2018-06-19 05:57:53.000000 localconfig-1.1.3/localconfig/utils.py
-drwxr-xr-x   0 mzheng    (1000) root         (0)        0 2019-05-14 21:44:05.000000 localconfig-1.1.3/test/
--rw-r--r--   0 mzheng    (1000) root         (0)       25 2018-06-19 05:57:53.000000 localconfig-1.1.3/test/last_source.cfg
--rw-r--r--   0 mzheng    (1000) root         (0)     6902 2018-06-19 06:51:59.000000 localconfig-1.1.3/test/test_manager.py
--rw-r--r--   0 mzheng    (1000) root         (0)       48 2018-06-19 05:57:53.000000 localconfig-1.1.3/test/third_source.cfg
-drwxr-xr-x   0 mzheng    (1000) root         (0)        0 2019-05-14 21:44:05.000000 localconfig-1.1.3/docs/
--rw-r--r--   0 mzheng    (1000) root         (0)      602 2018-06-19 05:57:53.000000 localconfig-1.1.3/docs/index.rst
--rw-r--r--   0 mzheng    (1000) root         (0)     7068 2018-06-19 05:57:53.000000 localconfig-1.1.3/docs/Makefile
--rw-r--r--   0 mzheng    (1000) root         (0)     5298 2019-05-14 21:43:07.000000 localconfig-1.1.3/docs/README.rst
--rw-r--r--   0 mzheng    (1000) root         (0)     9020 2018-06-19 05:57:53.000000 localconfig-1.1.3/docs/conf.py
--rw-r--r--   0 mzheng    (1000) root         (0)     2523 2019-05-14 21:44:04.000000 localconfig-1.1.3/docs/CHANGELOG.rst
--rw-r--r--   0 mzheng    (1000) root         (0)       74 2018-06-19 05:57:53.000000 localconfig-1.1.3/docs/localconfig.rst
--rw-r--r--   0 mzheng    (1000) root         (0)       72 2018-06-19 05:57:53.000000 localconfig-1.1.3/docs/utils.rst
--rw-r--r--   0 mzheng    (1000) root         (0)      915 2018-06-19 06:46:50.000000 localconfig-1.1.3/setup.py
--rw-r--r--   0 mzheng    (1000) root         (0)       82 2018-07-20 10:33:54.000000 localconfig-1.1.3/.coveragerc
--rw-r--r--   0 mzheng    (1000) root         (0)     5298 2019-05-14 21:43:07.000000 localconfig-1.1.3/README.rst
--rw-r--r--   0 mzheng    (1000) root         (0)     1362 2018-07-20 10:48:30.000000 localconfig-1.1.3/tox.ini
--rw-r--r--   0 mzheng    (1000) root         (0)       38 2019-05-14 21:44:05.000000 localconfig-1.1.3/setup.cfg
--rw-r--r--   0 mzheng    (1000) root         (0)     1076 2018-06-19 05:57:53.000000 localconfig-1.1.3/LICENSE
--rw-r--r--   0 mzheng    (1000) root         (0)     7445 2019-05-14 21:44:05.000000 localconfig-1.1.3/PKG-INFO
--rw-r--r--   0 mzheng    (1000) root         (0)     1212 2018-07-20 10:33:54.000000 localconfig-1.1.3/.gitignore
-drwxr-xr-x   0 mzheng    (1000) root         (0)        0 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig.egg-info/
--rw-r--r--   0 mzheng    (1000) root         (0)      443 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig.egg-info/SOURCES.txt
--rw-r--r--   0 mzheng    (1000) root         (0)       12 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig.egg-info/top_level.txt
--rw-r--r--   0 mzheng    (1000) root         (0)        1 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig.egg-info/dependency_links.txt
--rw-r--r--   0 mzheng    (1000) root         (0)     7445 2019-05-14 21:44:05.000000 localconfig-1.1.3/localconfig.egg-info/PKG-INFO
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-04-05 01:59:37.880890 localconfig-1.1.4/
+-rw-r--r--   0 max        (501) staff       (20)       82 2024-01-07 16:50:19.000000 localconfig-1.1.4/.coveragerc
+-rw-r--r--   0 max        (501) staff       (20)     1212 2024-01-07 16:50:19.000000 localconfig-1.1.4/.gitignore
+-rw-r--r--   0 max        (501) staff       (20)     1076 2024-01-07 16:50:19.000000 localconfig-1.1.4/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5989 2024-04-05 01:59:37.880683 localconfig-1.1.4/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     5315 2024-04-05 01:59:31.000000 localconfig-1.1.4/README.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-04-05 01:59:37.879191 localconfig-1.1.4/docs/
+-rw-r--r--   0 max        (501) staff       (20)     2857 2024-04-05 01:59:36.000000 localconfig-1.1.4/docs/CHANGELOG.rst
+-rw-r--r--   0 max        (501) staff       (20)     7068 2024-01-07 16:50:19.000000 localconfig-1.1.4/docs/Makefile
+-rw-r--r--   0 max        (501) staff       (20)     5315 2024-04-05 01:59:31.000000 localconfig-1.1.4/docs/README.rst
+-rw-r--r--   0 max        (501) staff       (20)     9020 2024-01-07 16:50:19.000000 localconfig-1.1.4/docs/conf.py
+-rw-r--r--   0 max        (501) staff       (20)      602 2024-01-07 16:50:19.000000 localconfig-1.1.4/docs/index.rst
+-rw-r--r--   0 max        (501) staff       (20)       74 2024-01-07 16:50:19.000000 localconfig-1.1.4/docs/localconfig.rst
+-rw-r--r--   0 max        (501) staff       (20)       72 2024-01-07 16:50:19.000000 localconfig-1.1.4/docs/utils.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-04-05 01:59:37.879593 localconfig-1.1.4/localconfig/
+-rw-r--r--   0 max        (501) staff       (20)       68 2024-01-07 16:50:19.000000 localconfig-1.1.4/localconfig/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    14691 2024-04-05 01:59:31.000000 localconfig-1.1.4/localconfig/manager.py
+-rw-r--r--   0 max        (501) staff       (20)     1122 2024-04-05 01:59:31.000000 localconfig-1.1.4/localconfig/utils.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-04-05 01:59:37.880055 localconfig-1.1.4/localconfig.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5989 2024-04-05 01:59:37.000000 localconfig-1.1.4/localconfig.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      443 2024-04-05 01:59:37.000000 localconfig-1.1.4/localconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2024-04-05 01:59:37.000000 localconfig-1.1.4/localconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       12 2024-04-05 01:59:37.000000 localconfig-1.1.4/localconfig.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2024-04-05 01:59:37.880943 localconfig-1.1.4/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      915 2024-01-07 16:50:19.000000 localconfig-1.1.4/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2024-04-05 01:59:37.880430 localconfig-1.1.4/test/
+-rw-r--r--   0 max        (501) staff       (20)       25 2024-01-07 16:50:19.000000 localconfig-1.1.4/test/last_source.cfg
+-rw-r--r--   0 max        (501) staff       (20)     7618 2024-04-05 01:59:31.000000 localconfig-1.1.4/test/test_manager.py
+-rw-r--r--   0 max        (501) staff       (20)       48 2024-01-07 16:50:19.000000 localconfig-1.1.4/test/third_source.cfg
+-rw-r--r--   0 max        (501) staff       (20)     1262 2024-01-07 17:16:18.000000 localconfig-1.1.4/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `localconfig-1.1.3/localconfig/manager.py` & `localconfig-1.1.4/localconfig/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from configparser import ConfigParser, BasicInterpolation, DuplicateSectionError, DEFAULTSECT
 from io import StringIO, IOBase
 import os
 import re
 import sys
 
-from localconfig.utils import is_float, is_int, is_bool, is_none, is_config, CONFIG_KEY_RE, to_bool
+from localconfig.utils import is_float, is_int, is_int_base_n, is_bool, is_none, is_config, CONFIG_KEY_RE, to_bool
 
 NON_ALPHA_NUM = re.compile('[^A-Za-z0-9]')
 NO_DEFAULT_VALUE = 'NO-DEFAULT-VALUE'
 
 
 class LocalConfig(object):
     """
@@ -330,14 +330,16 @@
     def _typed_value(self, value):
         """ Transform string value to an actual data type of the same value. """
 
         if value not in self._value_cache:
             new_value = value
             if is_int(value):
                 new_value = int(value)
+            elif is_int_base_n(value):
+                new_value = int(value, 0)
             elif is_float(value):
                 new_value = float(value)
             elif is_bool(value):
                 new_value = to_bool(value)
             elif is_none(value):
                 new_value = None
             self._value_cache[value] = new_value
```

### Comparing `localconfig-1.1.3/localconfig/utils.py` & `localconfig-1.1.4/localconfig/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import re
 
-CONFIG_KEY_RE = re.compile('[A-Za-z0-9\-\_\.]+\s*=')
+CONFIG_KEY_RE = re.compile(r'[A-Za-z0-9\-\_\.]+\s*=')
 
 
 def is_float(value):
     """ Checks if the value is a float """
     return _is_type(value, float)
 
 
 def is_int(value):
     """ Checks if the value is an int """
     return _is_type(value, int)
 
 
+def is_int_base_n(value):
+    """ Checks if the value is an int """
+    try:
+        # int(value, 0) will autodetect the presence of a base-n prefix in a string
+        int(value, 0)
+        return True
+    except Exception:
+        return False
+
+
 def is_bool(value):
     """ Checks if the value is a bool """
     return value.lower() in ['true', 'false', 'yes', 'no', 'on', 'off']
 
 
 def is_none(value):
     """ Checks if the value is a None """
```

### Comparing `localconfig-1.1.3/test/test_manager.py` & `localconfig-1.1.4/test/test_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 TEST_CONFIG = """\
 # Section used for type testing
 [types]
 
 # An int value
 int = 1
 
+# A binary int value
+int_binary = 0b11
+
+# An octal int value
+int_octal = 0o77
+
+# A hexadecimal int value
+int_hex = 0xabcd
+
 # A float value
 float = 2.0
 
 # A mid-commented out
 # comment = value
 
 # A bool value
@@ -51,14 +60,20 @@
 # Comment at the end
 """
 COMPACT_TEST_CONFIG = """\
 # Section used for type testing
 [types]
 # An int value
 int: 1
+# A binary int value
+int_binary: 0b11
+# An octal int value
+int_octal: 0o77
+# A hexadecimal int value
+int_hex: 0xabcd
 # A float value
 float: 2.0
 # A mid-commented out
 # comment = value
 
 # A bool value
 true: True
@@ -89,30 +104,35 @@
     config = LocalConfig()
     config.read(TEST_CONFIG)
     return config
 
 
 def test_read(config):
     assert config.types.int == 1
+    assert config.types.int_binary == 0b11
+    assert config.types.int_octal == 0o77
+    assert config.types.int_hex == 0xabcd
     assert config.types.float == 2.0
     assert config.types.true is True
     assert config.types.false is False
     assert config.types.none is None
     assert config.types.string_value == 'Value'
 
-    assert (config.another_section.multi_line ==
-            'This line spans multiple lines and\nwill be written out as such. '
-            'It will wrap\nwhere it originally wrapped.')
+    assert (config.another_section.multi_line == 'This line spans multiple lines and\nwill be written out as such. '
+                                                 'It will wrap\nwhere it originally wrapped.')
 
     assert config.no_section is None
     assert config.types.no_key is None
 
     assert {
       ('types', 'string-value'): '# A string value',
       ('types', 'int'): '# An int value',
+      ('types', 'int_binary'): '# A binary int value',
+      ('types', 'int_octal'): '# An octal int value',
+      ('types', 'int_hex'): '# A hexadecimal int value',
       ('types', 'float'): '# A float value',
       ('types', 'true'): '# A mid-commented out\n# comment = value\n\n# A bool value',
       ('types', 'false'): '# A false bool value',
       ('types', 'none'): '# A None value',
       'another-section': '# A commented out value\n# comment = value\n\n\n'
                          '####################################################\n'
                          '# Another section\n# with multiline comments\n'
@@ -209,24 +229,30 @@
     assert 'int: 1' in str(config)
 
 
 def test_iter(config):
     assert list(config) == ['types', 'another-section']
     assert [
       ('int', 1),
+      ('int_binary', 0b11),
+      ('int_octal', 0o77),
+      ('int_hex', 0xabcd),
       ('float', 2.0),
       ('true', True),
       ('false', False),
       ('none', None),
       ('string-value', 'Value')] == list(config.types)
     assert {
       'false': False,
       'none': None,
       'string-value': 'Value',
       'int': 1,
+      'int_binary': 0b11,
+      'int_octal': 0o77,
+      'int_hex': 0xabcd,
       'float': 2.0,
       'true': True} == dict(list(config.types))
 
 
 def test_add_section(config):
     config.add_section('New Section', comment='Comment for\n  new section')
     config.new_section.value = 1
```

### Comparing `localconfig-1.1.3/docs/index.rst` & `localconfig-1.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `localconfig-1.1.3/docs/Makefile` & `localconfig-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `localconfig-1.1.3/docs/README.rst` & `localconfig-1.1.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 Data type is guessed based on the value and converted on read.
 
 The following types are supported:
 
 ======= ===========================================
 Type    Example Value
 ======= ===========================================
-int     1
+int     1 0b1101 0o70 0xFF
 float   2.0
 bool    true false yes no on off (case insensitive)
 None    none (case insensitive)
 str     Any other value not matched by above
 ======= ===========================================
 
 Remote Config
```

### Comparing `localconfig-1.1.3/docs/conf.py` & `localconfig-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `localconfig-1.1.3/docs/CHANGELOG.rst` & `localconfig-1.1.4/docs/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,22 @@
-Version 1.1.3
+Version 1.1.4
 ================================================================================
 
+* Merge pull request #6 from ilario/int-non_decimal
+  
+  Add support for non-decimal integers
+* README added int_base_n to int examples
+* test_manager test int_base_n
+* manage: use is_int_base_n
+* utils: added is_int_base_n
+* Update tox
+
+Version 1.1.3
+--------------------------------------------------------------------------------
+
 * Fix RST doc format
 * Add note about config read order
 * Test py37
 * Skip setting last source if run by pytest
 * Fix typo
 
 Version 1.1.2
```

### Comparing `localconfig-1.1.3/setup.py` & `localconfig-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 
 setuptools.setup(
   name='localconfig',
-  version='1.1.3',
+  version='1.1.4',
 
   author='Max Zheng',
   author_email='maxzheng.os @t gmail.com',
 
   description='A simplified interface to ConfigParser using dot notion with data type / comment support.',
   long_description=open('README.rst').read(),
```

### Comparing `localconfig-1.1.3/README.rst` & `localconfig-1.1.4/docs/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 Data type is guessed based on the value and converted on read.
 
 The following types are supported:
 
 ======= ===========================================
 Type    Example Value
 ======= ===========================================
-int     1
+int     1 0b1101 0o70 0xFF
 float   2.0
 bool    true false yes no on off (case insensitive)
 None    none (case insensitive)
 str     Any other value not matched by above
 ======= ===========================================
 
 Remote Config
```

### Comparing `localconfig-1.1.3/tox.ini` & `localconfig-1.1.4/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = cover, py37, style
+envlist = py38, cover, style
 
 [testenv]
 # Consolidate all deps here instead of separately in test/style/cover so we
 # have a single env to work with, which makes debugging easier (like which env?).
 # Not as clean but easier to work with during development, which is better.
 deps =
     flake8
@@ -18,30 +18,27 @@
 recreate = False
 skipsdist = True
 usedevelop = True
 setenv =
     PIP_PROCESS_DEPENDENCY_LINKS=1
     PIP_DEFAULT_TIMEOUT=60
     ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future
-envdir = {homedir}/.virtualenvs/localconfig_{envname}
+envdir = {work_dir}/localconfig_{envname}
 commands =
     pytest {env:PYTESTARGS:}
 
-[testenv:py36]
-envdir = {homedir}/.virtualenvs/localconfig
-
 [testenv:style]
-basepython = python3.6
-envdir = {homedir}/.virtualenvs/localconfig
+basepython = python3
+envdir = {work_dir}/localconfig
 commands =
     flake8 --config tox.ini
 
 [testenv:cover]
-basepython = python3.6
-envdir = {homedir}/.virtualenvs/localconfig
+basepython = python3
+envdir = {work_dir}/localconfig
 commands =
     pytest {env:PYTESTARGS:} --cov . --cov-report=xml --cov-report=html --cov-report=term --cov-report=annotate:textcov \
                              --cov-fail-under=80
 
 [flake8]
 exclude = .git,.tox,.eggs,__pycache__,docs,build,dist
 ignore = E111,E121,W292,E123,E226
```

### Comparing `localconfig-1.1.3/LICENSE` & `localconfig-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `localconfig-1.1.3/PKG-INFO` & `localconfig-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: localconfig
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simplified interface to ConfigParser using dot notion with data type / comment support.
 Home-page: https://github.com/maxzheng/localconfig
 Author: Max Zheng
 Author-email: maxzheng.os @t gmail.com
 License: MIT
-Description: localconfig
-        ===========
-        
-        A simplified interface to `ConfigParser`_ using dot notion with data type / comment support.
-        
-        Feature Summary
-        ===============
-        
-        * Simple access to config using dot notion and iterators
-        * Full compatibility with `ConfigParser`_ ini formats (as that is used as the backend)
-        * Data type support by intelligently guessing the data types based on value on read.
-        * Multiple config source input (read from string, file pointer, file, or list of them)
-        * Full comment support / retention on save
-        * Lazy reading of config sources for performance (only read when a config value is accessed)
-        
-        .. _ConfigParser: https://docs.python.org/3/library/configparser.html
-        
-        Quick Start Tutorial
-        ====================
-        
-        To install::
-        
-            pip install localconfig
-        
-        Let's say we have a script named `program` with the following config in `~/.config/program`:
-        
-        .. code-block:: ini
-        
-            [Web Server]
-            # Server host
-            host = 0.0.0.0
-        
-            # Server port
-            port = 8080
-        
-            # Debug logging
-            debug = off
-        
-        To read the config, simply do:
-        
-        .. code-block:: python
-        
-            from localconfig import config
-        
-            start_server(config.web_server.host, config.web_server.port, config.web_server.debug)
-        
-            # Or use get method:
-            # start_server(config.get('Web Server', 'host'),
-            #              config.get('Web Server', 'port'),
-            #              config.get('web_server', 'debug'))  # Yes, 'web_server' also works here!
-            #
-            # Or if the config is in docstring, read from it:
-            # config.read(__doc__)
-            #
-            # Or if the config file is elsewhere:
-            # config.read('/etc/path/to/config.ini')  # Non-existing file is ignored
-            #
-            # Or read from a list of sources
-            # config.read(['string config', file_path, file_pointer, io.StringIO('config')])
-            #
-            # Or create another instance for another config:
-            # from localconfig import LocalConfig
-            # config2 = LocalConfig('/etc/path/to/another/config.ini')
-        
-        Configs are read in the order they are called using `config.read()`, but the config file passed to the `LocalConfig()`
-        constructor (defaults to `~/.config/$script_name`) will be read last before the first access to config values, which
-        allows us to read configs from various locations, like default configs from a string that is checked in with the code,
-        while allowing them to be overrriden from the config file that is passed to the constructor.
-        
-        Now, let's do some inspection:
-        
-        .. code-block:: python
-        
-            # Iterate over sections and their keys/values
-            for section in config:
-              print(section)                   # Web Server
-        
-              for key, value in config.items(section):
-                print(key, value, type(value)) # host 0.0.0.0 <type 'str'>
-                                               # port 8080 <type 'int'>
-                                               # debug False <type 'bool'>
-        
-            sections = list(config)            # ['Web Server']
-        
-            # Iterate over keys/values
-            for key, value in config.web_server:
-              print(key, value, type(value))    # Same output as above config.items()
-        
-            items = list(config.web_server)    # [('host', '0.0.0.0'), ('port', 8080), ('debug', False)]
-            items = dict(config.web_server)    # {'host': '0.0.0.0', 'port': 8080, 'debug': False}
-        
-            # Check if a section or key is set - any non-existing section or key defaults to None.
-            if config.web_server or config.no_such_section:
-              pass
-        
-            if config.web_server and (config.web_server.port or config.web_server.no_such_key):
-              pass
-        
-        To add a section and set a value:
-        
-        .. code-block:: python
-        
-            config.add_section('App Server', comment='Settings for application server')
-            config.app_server.host = 'localhost'
-        
-            # Use `set` if you want to set a comment
-            config.set('App Server', 'port', 9090, comment='App server port')
-        
-            # Set value for the DEFAULT section (default value for all other sections)
-            config.env = 'prod'
-        
-        To write the config:
-        
-        .. code-block:: python
-        
-            config.save()
-        
-            # Or simply get the config as a string:
-            # config_str = str(config)
-            #
-            # Or save to a different location:
-            # config.save('/path/to/save/to.ini')
-        
-        If we open `~/.config/program` now, we would see::
-        
-            [DEFAULT]
-        
-            env = prod
-        
-        
-            [Web Server]
-        
-            # Server host
-            host = 0.0.0.0
-        
-            # Server port
-            port = 8080
-        
-            # Debug logging
-            debug = off
-        
-        
-            # Settings for application server
-            [App Server]
-        
-            host = localhost
-        
-            # App server port
-            port = 9090
-        
-        Supported Data Types
-        ====================
-        
-        Data type is guessed based on the value and converted on read.
-        
-        The following types are supported:
-        
-        ======= ===========================================
-        Type    Example Value
-        ======= ===========================================
-        int     1
-        float   2.0
-        bool    true false yes no on off (case insensitive)
-        None    none (case insensitive)
-        str     Any other value not matched by above
-        ======= ===========================================
-        
-        Remote Config
-        =============
-        
-        Check out: https://pypi.python.org/pypi/remoteconfig
-        
-        More
-        ====
-        
-        | Documentation: http://localconfig.readthedocs.org/
-        |
-        | PyPI Package: https://pypi.python.org/pypi/localconfig
-        | GitHub Source: https://github.com/maxzheng/localconfig
-        | Report Issues/Bugs: https://github.com/maxzheng/localconfig/issues
-        |
-        | Connect: https://www.linkedin.com/in/maxzheng
-        | Contact: maxzheng.os @t gmail.com
-        
 Keywords: configuration config ConfigParser data type support
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
+License-File: LICENSE
+
+localconfig
+===========
+
+A simplified interface to `ConfigParser`_ using dot notion with data type / comment support.
+
+Feature Summary
+===============
+
+* Simple access to config using dot notion and iterators
+* Full compatibility with `ConfigParser`_ ini formats (as that is used as the backend)
+* Data type support by intelligently guessing the data types based on value on read.
+* Multiple config source input (read from string, file pointer, file, or list of them)
+* Full comment support / retention on save
+* Lazy reading of config sources for performance (only read when a config value is accessed)
+
+.. _ConfigParser: https://docs.python.org/3/library/configparser.html
+
+Quick Start Tutorial
+====================
+
+To install::
+
+    pip install localconfig
+
+Let's say we have a script named `program` with the following config in `~/.config/program`:
+
+.. code-block:: ini
+
+    [Web Server]
+    # Server host
+    host = 0.0.0.0
+
+    # Server port
+    port = 8080
+
+    # Debug logging
+    debug = off
+
+To read the config, simply do:
+
+.. code-block:: python
+
+    from localconfig import config
+
+    start_server(config.web_server.host, config.web_server.port, config.web_server.debug)
+
+    # Or use get method:
+    # start_server(config.get('Web Server', 'host'),
+    #              config.get('Web Server', 'port'),
+    #              config.get('web_server', 'debug'))  # Yes, 'web_server' also works here!
+    #
+    # Or if the config is in docstring, read from it:
+    # config.read(__doc__)
+    #
+    # Or if the config file is elsewhere:
+    # config.read('/etc/path/to/config.ini')  # Non-existing file is ignored
+    #
+    # Or read from a list of sources
+    # config.read(['string config', file_path, file_pointer, io.StringIO('config')])
+    #
+    # Or create another instance for another config:
+    # from localconfig import LocalConfig
+    # config2 = LocalConfig('/etc/path/to/another/config.ini')
+
+Configs are read in the order they are called using `config.read()`, but the config file passed to the `LocalConfig()`
+constructor (defaults to `~/.config/$script_name`) will be read last before the first access to config values, which
+allows us to read configs from various locations, like default configs from a string that is checked in with the code,
+while allowing them to be overrriden from the config file that is passed to the constructor.
+
+Now, let's do some inspection:
+
+.. code-block:: python
+
+    # Iterate over sections and their keys/values
+    for section in config:
+      print(section)                   # Web Server
+
+      for key, value in config.items(section):
+        print(key, value, type(value)) # host 0.0.0.0 <type 'str'>
+                                       # port 8080 <type 'int'>
+                                       # debug False <type 'bool'>
+
+    sections = list(config)            # ['Web Server']
+
+    # Iterate over keys/values
+    for key, value in config.web_server:
+      print(key, value, type(value))    # Same output as above config.items()
+
+    items = list(config.web_server)    # [('host', '0.0.0.0'), ('port', 8080), ('debug', False)]
+    items = dict(config.web_server)    # {'host': '0.0.0.0', 'port': 8080, 'debug': False}
+
+    # Check if a section or key is set - any non-existing section or key defaults to None.
+    if config.web_server or config.no_such_section:
+      pass
+
+    if config.web_server and (config.web_server.port or config.web_server.no_such_key):
+      pass
+
+To add a section and set a value:
+
+.. code-block:: python
+
+    config.add_section('App Server', comment='Settings for application server')
+    config.app_server.host = 'localhost'
+
+    # Use `set` if you want to set a comment
+    config.set('App Server', 'port', 9090, comment='App server port')
+
+    # Set value for the DEFAULT section (default value for all other sections)
+    config.env = 'prod'
+
+To write the config:
+
+.. code-block:: python
+
+    config.save()
+
+    # Or simply get the config as a string:
+    # config_str = str(config)
+    #
+    # Or save to a different location:
+    # config.save('/path/to/save/to.ini')
+
+If we open `~/.config/program` now, we would see::
+
+    [DEFAULT]
+
+    env = prod
+
+
+    [Web Server]
+
+    # Server host
+    host = 0.0.0.0
+
+    # Server port
+    port = 8080
+
+    # Debug logging
+    debug = off
+
+
+    # Settings for application server
+    [App Server]
+
+    host = localhost
+
+    # App server port
+    port = 9090
+
+Supported Data Types
+====================
+
+Data type is guessed based on the value and converted on read.
+
+The following types are supported:
+
+======= ===========================================
+Type    Example Value
+======= ===========================================
+int     1 0b1101 0o70 0xFF
+float   2.0
+bool    true false yes no on off (case insensitive)
+None    none (case insensitive)
+str     Any other value not matched by above
+======= ===========================================
+
+Remote Config
+=============
+
+Check out: https://pypi.python.org/pypi/remoteconfig
+
+More
+====
+
+| Documentation: http://localconfig.readthedocs.org/
+|
+| PyPI Package: https://pypi.python.org/pypi/localconfig
+| GitHub Source: https://github.com/maxzheng/localconfig
+| Report Issues/Bugs: https://github.com/maxzheng/localconfig/issues
+|
+| Connect: https://www.linkedin.com/in/maxzheng
+| Contact: maxzheng.os @t gmail.com
```

### Comparing `localconfig-1.1.3/.gitignore` & `localconfig-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `localconfig-1.1.3/localconfig.egg-info/PKG-INFO` & `localconfig-1.1.4/localconfig.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: localconfig
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simplified interface to ConfigParser using dot notion with data type / comment support.
 Home-page: https://github.com/maxzheng/localconfig
 Author: Max Zheng
 Author-email: maxzheng.os @t gmail.com
 License: MIT
-Description: localconfig
-        ===========
-        
-        A simplified interface to `ConfigParser`_ using dot notion with data type / comment support.
-        
-        Feature Summary
-        ===============
-        
-        * Simple access to config using dot notion and iterators
-        * Full compatibility with `ConfigParser`_ ini formats (as that is used as the backend)
-        * Data type support by intelligently guessing the data types based on value on read.
-        * Multiple config source input (read from string, file pointer, file, or list of them)
-        * Full comment support / retention on save
-        * Lazy reading of config sources for performance (only read when a config value is accessed)
-        
-        .. _ConfigParser: https://docs.python.org/3/library/configparser.html
-        
-        Quick Start Tutorial
-        ====================
-        
-        To install::
-        
-            pip install localconfig
-        
-        Let's say we have a script named `program` with the following config in `~/.config/program`:
-        
-        .. code-block:: ini
-        
-            [Web Server]
-            # Server host
-            host = 0.0.0.0
-        
-            # Server port
-            port = 8080
-        
-            # Debug logging
-            debug = off
-        
-        To read the config, simply do:
-        
-        .. code-block:: python
-        
-            from localconfig import config
-        
-            start_server(config.web_server.host, config.web_server.port, config.web_server.debug)
-        
-            # Or use get method:
-            # start_server(config.get('Web Server', 'host'),
-            #              config.get('Web Server', 'port'),
-            #              config.get('web_server', 'debug'))  # Yes, 'web_server' also works here!
-            #
-            # Or if the config is in docstring, read from it:
-            # config.read(__doc__)
-            #
-            # Or if the config file is elsewhere:
-            # config.read('/etc/path/to/config.ini')  # Non-existing file is ignored
-            #
-            # Or read from a list of sources
-            # config.read(['string config', file_path, file_pointer, io.StringIO('config')])
-            #
-            # Or create another instance for another config:
-            # from localconfig import LocalConfig
-            # config2 = LocalConfig('/etc/path/to/another/config.ini')
-        
-        Configs are read in the order they are called using `config.read()`, but the config file passed to the `LocalConfig()`
-        constructor (defaults to `~/.config/$script_name`) will be read last before the first access to config values, which
-        allows us to read configs from various locations, like default configs from a string that is checked in with the code,
-        while allowing them to be overrriden from the config file that is passed to the constructor.
-        
-        Now, let's do some inspection:
-        
-        .. code-block:: python
-        
-            # Iterate over sections and their keys/values
-            for section in config:
-              print(section)                   # Web Server
-        
-              for key, value in config.items(section):
-                print(key, value, type(value)) # host 0.0.0.0 <type 'str'>
-                                               # port 8080 <type 'int'>
-                                               # debug False <type 'bool'>
-        
-            sections = list(config)            # ['Web Server']
-        
-            # Iterate over keys/values
-            for key, value in config.web_server:
-              print(key, value, type(value))    # Same output as above config.items()
-        
-            items = list(config.web_server)    # [('host', '0.0.0.0'), ('port', 8080), ('debug', False)]
-            items = dict(config.web_server)    # {'host': '0.0.0.0', 'port': 8080, 'debug': False}
-        
-            # Check if a section or key is set - any non-existing section or key defaults to None.
-            if config.web_server or config.no_such_section:
-              pass
-        
-            if config.web_server and (config.web_server.port or config.web_server.no_such_key):
-              pass
-        
-        To add a section and set a value:
-        
-        .. code-block:: python
-        
-            config.add_section('App Server', comment='Settings for application server')
-            config.app_server.host = 'localhost'
-        
-            # Use `set` if you want to set a comment
-            config.set('App Server', 'port', 9090, comment='App server port')
-        
-            # Set value for the DEFAULT section (default value for all other sections)
-            config.env = 'prod'
-        
-        To write the config:
-        
-        .. code-block:: python
-        
-            config.save()
-        
-            # Or simply get the config as a string:
-            # config_str = str(config)
-            #
-            # Or save to a different location:
-            # config.save('/path/to/save/to.ini')
-        
-        If we open `~/.config/program` now, we would see::
-        
-            [DEFAULT]
-        
-            env = prod
-        
-        
-            [Web Server]
-        
-            # Server host
-            host = 0.0.0.0
-        
-            # Server port
-            port = 8080
-        
-            # Debug logging
-            debug = off
-        
-        
-            # Settings for application server
-            [App Server]
-        
-            host = localhost
-        
-            # App server port
-            port = 9090
-        
-        Supported Data Types
-        ====================
-        
-        Data type is guessed based on the value and converted on read.
-        
-        The following types are supported:
-        
-        ======= ===========================================
-        Type    Example Value
-        ======= ===========================================
-        int     1
-        float   2.0
-        bool    true false yes no on off (case insensitive)
-        None    none (case insensitive)
-        str     Any other value not matched by above
-        ======= ===========================================
-        
-        Remote Config
-        =============
-        
-        Check out: https://pypi.python.org/pypi/remoteconfig
-        
-        More
-        ====
-        
-        | Documentation: http://localconfig.readthedocs.org/
-        |
-        | PyPI Package: https://pypi.python.org/pypi/localconfig
-        | GitHub Source: https://github.com/maxzheng/localconfig
-        | Report Issues/Bugs: https://github.com/maxzheng/localconfig/issues
-        |
-        | Connect: https://www.linkedin.com/in/maxzheng
-        | Contact: maxzheng.os @t gmail.com
-        
 Keywords: configuration config ConfigParser data type support
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
+License-File: LICENSE
+
+localconfig
+===========
+
+A simplified interface to `ConfigParser`_ using dot notion with data type / comment support.
+
+Feature Summary
+===============
+
+* Simple access to config using dot notion and iterators
+* Full compatibility with `ConfigParser`_ ini formats (as that is used as the backend)
+* Data type support by intelligently guessing the data types based on value on read.
+* Multiple config source input (read from string, file pointer, file, or list of them)
+* Full comment support / retention on save
+* Lazy reading of config sources for performance (only read when a config value is accessed)
+
+.. _ConfigParser: https://docs.python.org/3/library/configparser.html
+
+Quick Start Tutorial
+====================
+
+To install::
+
+    pip install localconfig
+
+Let's say we have a script named `program` with the following config in `~/.config/program`:
+
+.. code-block:: ini
+
+    [Web Server]
+    # Server host
+    host = 0.0.0.0
+
+    # Server port
+    port = 8080
+
+    # Debug logging
+    debug = off
+
+To read the config, simply do:
+
+.. code-block:: python
+
+    from localconfig import config
+
+    start_server(config.web_server.host, config.web_server.port, config.web_server.debug)
+
+    # Or use get method:
+    # start_server(config.get('Web Server', 'host'),
+    #              config.get('Web Server', 'port'),
+    #              config.get('web_server', 'debug'))  # Yes, 'web_server' also works here!
+    #
+    # Or if the config is in docstring, read from it:
+    # config.read(__doc__)
+    #
+    # Or if the config file is elsewhere:
+    # config.read('/etc/path/to/config.ini')  # Non-existing file is ignored
+    #
+    # Or read from a list of sources
+    # config.read(['string config', file_path, file_pointer, io.StringIO('config')])
+    #
+    # Or create another instance for another config:
+    # from localconfig import LocalConfig
+    # config2 = LocalConfig('/etc/path/to/another/config.ini')
+
+Configs are read in the order they are called using `config.read()`, but the config file passed to the `LocalConfig()`
+constructor (defaults to `~/.config/$script_name`) will be read last before the first access to config values, which
+allows us to read configs from various locations, like default configs from a string that is checked in with the code,
+while allowing them to be overrriden from the config file that is passed to the constructor.
+
+Now, let's do some inspection:
+
+.. code-block:: python
+
+    # Iterate over sections and their keys/values
+    for section in config:
+      print(section)                   # Web Server
+
+      for key, value in config.items(section):
+        print(key, value, type(value)) # host 0.0.0.0 <type 'str'>
+                                       # port 8080 <type 'int'>
+                                       # debug False <type 'bool'>
+
+    sections = list(config)            # ['Web Server']
+
+    # Iterate over keys/values
+    for key, value in config.web_server:
+      print(key, value, type(value))    # Same output as above config.items()
+
+    items = list(config.web_server)    # [('host', '0.0.0.0'), ('port', 8080), ('debug', False)]
+    items = dict(config.web_server)    # {'host': '0.0.0.0', 'port': 8080, 'debug': False}
+
+    # Check if a section or key is set - any non-existing section or key defaults to None.
+    if config.web_server or config.no_such_section:
+      pass
+
+    if config.web_server and (config.web_server.port or config.web_server.no_such_key):
+      pass
+
+To add a section and set a value:
+
+.. code-block:: python
+
+    config.add_section('App Server', comment='Settings for application server')
+    config.app_server.host = 'localhost'
+
+    # Use `set` if you want to set a comment
+    config.set('App Server', 'port', 9090, comment='App server port')
+
+    # Set value for the DEFAULT section (default value for all other sections)
+    config.env = 'prod'
+
+To write the config:
+
+.. code-block:: python
+
+    config.save()
+
+    # Or simply get the config as a string:
+    # config_str = str(config)
+    #
+    # Or save to a different location:
+    # config.save('/path/to/save/to.ini')
+
+If we open `~/.config/program` now, we would see::
+
+    [DEFAULT]
+
+    env = prod
+
+
+    [Web Server]
+
+    # Server host
+    host = 0.0.0.0
+
+    # Server port
+    port = 8080
+
+    # Debug logging
+    debug = off
+
+
+    # Settings for application server
+    [App Server]
+
+    host = localhost
+
+    # App server port
+    port = 9090
+
+Supported Data Types
+====================
+
+Data type is guessed based on the value and converted on read.
+
+The following types are supported:
+
+======= ===========================================
+Type    Example Value
+======= ===========================================
+int     1 0b1101 0o70 0xFF
+float   2.0
+bool    true false yes no on off (case insensitive)
+None    none (case insensitive)
+str     Any other value not matched by above
+======= ===========================================
+
+Remote Config
+=============
+
+Check out: https://pypi.python.org/pypi/remoteconfig
+
+More
+====
+
+| Documentation: http://localconfig.readthedocs.org/
+|
+| PyPI Package: https://pypi.python.org/pypi/localconfig
+| GitHub Source: https://github.com/maxzheng/localconfig
+| Report Issues/Bugs: https://github.com/maxzheng/localconfig/issues
+|
+| Connect: https://www.linkedin.com/in/maxzheng
+| Contact: maxzheng.os @t gmail.com
```

