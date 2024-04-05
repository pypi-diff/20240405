# Comparing `tmp/flask-minijson-0.2.tar.gz` & `tmp/flask-minijson-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flask-minijson-0.2.tar", last modified: Wed Jun 30 15:08:24 2021, max compression
+gzip compressed data, was "flask-minijson-0.3.tar", last modified: Fri Apr  5 07:22:45 2024, max compression
```

## Comparing `flask-minijson-0.2.tar` & `flask-minijson-0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-06-30 15:08:24.298846 flask-minijson-0.2/
--rw-rw-rw-   0        0        0     1089 2021-06-30 12:38:24.000000 flask-minijson-0.2/LICENSE
--rw-rw-rw-   0        0        0       26 2021-06-30 12:41:13.000000 flask-minijson-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2827 2021-06-30 15:08:24.298846 flask-minijson-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2021-06-30 14:45:22.000000 flask-minijson-0.2/README.md
-drwxrwxrwx   0        0        0        0 2021-06-30 15:08:24.297843 flask-minijson-0.2/flask_minijson.egg-info/
--rw-rw-rw-   0        0        0     2827 2021-06-30 15:08:24.000000 flask-minijson-0.2/flask_minijson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2021-06-30 15:08:24.000000 flask-minijson-0.2/flask_minijson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-30 15:08:24.000000 flask-minijson-0.2/flask_minijson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2021-06-30 15:08:24.000000 flask-minijson-0.2/flask_minijson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1158 2021-06-30 15:08:02.000000 flask-minijson-0.2/flask_minijson.py
--rw-rw-rw-   0        0        0       29 2021-06-30 12:41:25.000000 flask-minijson-0.2/requirements.txt
--rw-rw-rw-   0        0        0     1306 2021-06-30 15:08:24.300847 flask-minijson-0.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-06-30 12:39:05.000000 flask-minijson-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:22:45.752144 flask-minijson-0.3/
+-rw-rw-rw-   0        0        0     1140 2024-04-05 07:20:09.000000 flask-minijson-0.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-04-05 07:11:20.000000 flask-minijson-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2811 2024-04-05 07:22:45.750190 flask-minijson-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2024-04-05 07:11:20.000000 flask-minijson-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 07:22:45.748325 flask-minijson-0.3/flask_minijson.egg-info/
+-rw-rw-rw-   0        0        0     2811 2024-04-05 07:22:45.000000 flask-minijson-0.3/flask_minijson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-05 07:22:45.000000 flask-minijson-0.3/flask_minijson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 07:22:45.000000 flask-minijson-0.3/flask_minijson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 07:22:45.000000 flask-minijson-0.3/flask_minijson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1310 2024-04-05 07:14:20.000000 flask-minijson-0.3/flask_minijson.py
+-rw-rw-rw-   0        0        0       29 2024-04-05 07:11:20.000000 flask-minijson-0.3/requirements.txt
+-rw-rw-rw-   0        0        0     1297 2024-04-05 07:22:45.753121 flask-minijson-0.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-05 07:11:20.000000 flask-minijson-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 07:22:45.745308 flask-minijson-0.3/tests/
+-rw-rw-rw-   0        0        0      529 2024-04-05 07:11:20.000000 flask-minijson-0.3/tests/test_minijson.py
```

### Comparing `flask-minijson-0.2/LICENSE` & `flask-minijson-0.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2021 dronehub.ai
+Copyright (c) 2021 Dronehub Group sp. z o. o.
+Copyright (c) 2024 Piotr Maślanka
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flask-minijson-0.2/PKG-INFO` & `flask-minijson-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: flask-minijson
-Version: 0.2
+Version: 0.3
 Summary: A Flask extension to allow client's to submit data using the MiniJSON codec
 Home-page: https://github.com/Dronehub/flask-minijson
 Author: Piotr Maślanka
-Author-email: piotr.maslanka@dronehub.ai
-License: UNKNOWN
+Author-email: pmaslanka@smok.co
 Project-URL: Code, https://github.com/Dronehub/flask-minijson
 Project-URL: Issue tracker, https://github.com/Dronehub/flask-minijson/issues
-Description: flask-minijson
-        ==============
-        
-        [![Build Status](https://travis-ci.com/Dronehub/flask-minijson.svg)](https://travis-ci.com/Dronehub/flask-minijson)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/flask-minijson/test_coverage)
-        [![Issue Count](https://codeclimate.com/github/Dronehub/flask-minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/flask-minijson)
-        [![PyPI](https://img.shields.io/pypi/pyversions/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
-        [![PyPI version](https://badge.fury.io/py/flask-minijson.svg)](https://badge.fury.io/py/flask-minijson)
-        [![PyPI](https://img.shields.io/pypi/implementation/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
-        
-        An extension for Flask to allow clients to submit data using the application/minijson codec
-        
-        flask-json is required to be initialized before `FlaskMiniJSON`, in such a way:
-        
-        ```python
-        from flask_minijson import FlaskMiniJSON
-        
-        app = Flask(__name__)
-        FlaskJSON(app)
-        FlaskMiniJSON(app)
-        ```
-        
-        And you use it like this:
-        
-        ```python
-        @app.route('/v1', methods=['POST'])
-        def endpoint():
-            json = request.get_json()
-        ```
-        if normal JSON is passed, it will be recognized. If
-        minijson is sent by the client, it will be recognized as well
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: !=2.7.*,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+flask-minijson
+==============
+
+[![Build Status](https://travis-ci.com/Dronehub/flask-minijson.svg)](https://travis-ci.com/Dronehub/flask-minijson)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/flask-minijson/test_coverage)
+[![Issue Count](https://codeclimate.com/github/Dronehub/flask-minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/pyversions/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
+[![PyPI version](https://badge.fury.io/py/flask-minijson.svg)](https://badge.fury.io/py/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/implementation/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/wheel/flask-minijson.svg)]()
+[![License](https://img.shields.io/pypi/l/flask-minijson)](https://github.com/Dronehub/flask-minijson)
+
+An extension for Flask to allow clients to submit data using the
+[minijson](https://github.com/Dronehub/minijson) codec by providing
+a `Content-Type` header of `application/minijson`.
+
+flask-json is required to be initialized before `FlaskMiniJSON`, in such a way:
+
+```python
+from flask_minijson import FlaskMiniJSON
+
+app = Flask(__name__)
+FlaskJSON(app)
+FlaskMiniJSON(app)
+```
+
+And you use it like this:
+
+```python
+@app.route('/v1', methods=['POST'])
+def endpoint():
+    json = request.get_json()
+```
+
+if normal JSON is passed, it will be recognized. If
+minijson is sent by the client, it will be recognized as well.
```

### Comparing `flask-minijson-0.2/README.md` & `flask-minijson-0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 
 [![Build Status](https://travis-ci.com/Dronehub/flask-minijson.svg)](https://travis-ci.com/Dronehub/flask-minijson)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/flask-minijson/test_coverage)
 [![Issue Count](https://codeclimate.com/github/Dronehub/flask-minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/flask-minijson)
 [![PyPI](https://img.shields.io/pypi/pyversions/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
 [![PyPI version](https://badge.fury.io/py/flask-minijson.svg)](https://badge.fury.io/py/flask-minijson)
 [![PyPI](https://img.shields.io/pypi/implementation/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/wheel/flask-minijson.svg)]()
+[![License](https://img.shields.io/pypi/l/flask-minijson)](https://github.com/Dronehub/flask-minijson)
 
-An extension for Flask to allow clients to submit data using the application/minijson codec
+An extension for Flask to allow clients to submit data using the
+[minijson](https://github.com/Dronehub/minijson) codec by providing
+a `Content-Type` header of `application/minijson`.
 
 flask-json is required to be initialized before `FlaskMiniJSON`, in such a way:
 
 ```python
 from flask_minijson import FlaskMiniJSON
 
 app = Flask(__name__)
@@ -23,9 +27,10 @@
 And you use it like this:
 
 ```python
 @app.route('/v1', methods=['POST'])
 def endpoint():
     json = request.get_json()
 ```
+
 if normal JSON is passed, it will be recognized. If
-minijson is sent by the client, it will be recognized as well
+minijson is sent by the client, it will be recognized as well.
```

### Comparing `flask-minijson-0.2/flask_minijson.egg-info/PKG-INFO` & `flask-minijson-0.3/flask_minijson.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: flask-minijson
-Version: 0.2
+Version: 0.3
 Summary: A Flask extension to allow client's to submit data using the MiniJSON codec
 Home-page: https://github.com/Dronehub/flask-minijson
 Author: Piotr Maślanka
-Author-email: piotr.maslanka@dronehub.ai
-License: UNKNOWN
+Author-email: pmaslanka@smok.co
 Project-URL: Code, https://github.com/Dronehub/flask-minijson
 Project-URL: Issue tracker, https://github.com/Dronehub/flask-minijson/issues
-Description: flask-minijson
-        ==============
-        
-        [![Build Status](https://travis-ci.com/Dronehub/flask-minijson.svg)](https://travis-ci.com/Dronehub/flask-minijson)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/flask-minijson/test_coverage)
-        [![Issue Count](https://codeclimate.com/github/Dronehub/flask-minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/flask-minijson)
-        [![PyPI](https://img.shields.io/pypi/pyversions/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
-        [![PyPI version](https://badge.fury.io/py/flask-minijson.svg)](https://badge.fury.io/py/flask-minijson)
-        [![PyPI](https://img.shields.io/pypi/implementation/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
-        
-        An extension for Flask to allow clients to submit data using the application/minijson codec
-        
-        flask-json is required to be initialized before `FlaskMiniJSON`, in such a way:
-        
-        ```python
-        from flask_minijson import FlaskMiniJSON
-        
-        app = Flask(__name__)
-        FlaskJSON(app)
-        FlaskMiniJSON(app)
-        ```
-        
-        And you use it like this:
-        
-        ```python
-        @app.route('/v1', methods=['POST'])
-        def endpoint():
-            json = request.get_json()
-        ```
-        if normal JSON is passed, it will be recognized. If
-        minijson is sent by the client, it will be recognized as well
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: !=2.7.*,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+
+flask-minijson
+==============
+
+[![Build Status](https://travis-ci.com/Dronehub/flask-minijson.svg)](https://travis-ci.com/Dronehub/flask-minijson)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/34b392b61482d98ad3f0/test_coverage)](https://codeclimate.com/github/Dronehub/flask-minijson/test_coverage)
+[![Issue Count](https://codeclimate.com/github/Dronehub/flask-minijson/badges/issue_count.svg)](https://codeclimate.com/github/Dronehub/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/pyversions/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
+[![PyPI version](https://badge.fury.io/py/flask-minijson.svg)](https://badge.fury.io/py/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/implementation/flask-minijson.svg)](https://pypi.python.org/pypi/flask-minijson)
+[![PyPI](https://img.shields.io/pypi/wheel/flask-minijson.svg)]()
+[![License](https://img.shields.io/pypi/l/flask-minijson)](https://github.com/Dronehub/flask-minijson)
+
+An extension for Flask to allow clients to submit data using the
+[minijson](https://github.com/Dronehub/minijson) codec by providing
+a `Content-Type` header of `application/minijson`.
+
+flask-json is required to be initialized before `FlaskMiniJSON`, in such a way:
+
+```python
+from flask_minijson import FlaskMiniJSON
+
+app = Flask(__name__)
+FlaskJSON(app)
+FlaskMiniJSON(app)
+```
+
+And you use it like this:
+
+```python
+@app.route('/v1', methods=['POST'])
+def endpoint():
+    json = request.get_json()
+```
+
+if normal JSON is passed, it will be recognized. If
+minijson is sent by the client, it will be recognized as well.
```

### Comparing `flask-minijson-0.2/setup.cfg` & `flask-minijson-0.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 320d 0a6e 616d 6520  ion = 0.2..name 
+00000010: 696f 6e20 3d20 302e 330d 0a6e 616d 6520  ion = 0.3..name 
 00000020: 3d20 666c 6173 6b2d 6d69 6e69 6a73 6f6e  = flask-minijson
 00000030: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 00000040: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
 00000050: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
 00000060: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
 00000070: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
 00000080: 6f77 6e3b 2063 6861 7273 6574 3d55 5446  own; charset=UTF
 00000090: 2d38 0d0a 6175 7468 6f72 203d 2050 696f  -8..author = Pio
 000000a0: 7472 204d 61c5 9b6c 616e 6b61 0d0a 6c69  tr Ma..lanka..li
 000000b0: 6365 6e73 655f 6669 6c65 7320 3d20 0d0a  cense_files = ..
 000000c0: 094c 4943 454e 5345 0d0a 6175 7468 6f72  .LICENSE..author
-000000d0: 5f65 6d61 696c 203d 2070 696f 7472 2e6d  _email = piotr.m
-000000e0: 6173 6c61 6e6b 6140 6472 6f6e 6568 7562  aslanka@dronehub
-000000f0: 2e61 690d 0a64 6573 6372 6970 7469 6f6e  .ai..description
-00000100: 203d 2041 2046 6c61 736b 2065 7874 656e   = A Flask exten
-00000110: 7369 6f6e 2074 6f20 616c 6c6f 7720 636c  sion to allow cl
-00000120: 6965 6e74 2773 2074 6f20 7375 626d 6974  ient's to submit
-00000130: 2064 6174 6120 7573 696e 6720 7468 6520   data using the 
-00000140: 4d69 6e69 4a53 4f4e 2063 6f64 6563 0d0a  MiniJSON codec..
-00000150: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000160: 7468 7562 2e63 6f6d 2f44 726f 6e65 6875  thub.com/Dronehu
-00000170: 622f 666c 6173 6b2d 6d69 6e69 6a73 6f6e  b/flask-minijson
-00000180: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
-00000190: 200d 0a09 436f 6465 203d 2068 7474 7073   ...Code = https
-000001a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4472  ://github.com/Dr
-000001b0: 6f6e 6568 7562 2f66 6c61 736b 2d6d 696e  onehub/flask-min
-000001c0: 696a 736f 6e0d 0a09 4973 7375 6520 7472  ijson...Issue tr
-000001d0: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
-000001e0: 6769 7468 7562 2e63 6f6d 2f44 726f 6e65  github.com/Drone
-000001f0: 6875 622f 666c 6173 6b2d 6d69 6e69 6a73  hub/flask-minijs
-00000200: 6f6e 2f69 7373 7565 730d 0a63 6c61 7373  on/issues..class
-00000210: 6966 6965 7220 3d20 0d0a 0944 6576 656c  ifier = ...Devel
-00000220: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000230: 2034 202d 2042 6574 610d 0a09 5072 6f67   4 - Beta...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 0d0a 0950 726f   :: Python...Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 2e35 0d0a 0950 726f 6772 616d 6d69 6e67  .5...Programming
-00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002a0: 686f 6e20 3a3a 2033 2e36 0d0a 0950 726f  hon :: 3.6...Pro
-000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002d0: 2e37 0d0a 0950 726f 6772 616d 6d69 6e67  .7...Programming
-000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002f0: 686f 6e20 3a3a 2033 2e38 0d0a 0950 726f  hon :: 3.8...Pro
-00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000320: 2e39 0d0a 0950 726f 6772 616d 6d69 6e67  .9...Programming
-00000330: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000340: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-00000350: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-00000360: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000370: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000380: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
-00000390: 696f 6e20 3a3a 2050 7950 790d 0a09 4f70  ion :: PyPy...Op
-000003a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000003b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000003c0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-000003d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000003e0: 5420 4c69 6365 6e73 650d 0a09 546f 7069  T License...Topi
-000003f0: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
-00000400: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
-00000410: 7261 7269 6573 0d0a 0d0a 5b70 7963 6f64  raries....[pycod
-00000420: 6573 7479 6c65 5d0d 0a6d 6178 2d6c 696e  estyle]..max-lin
-00000430: 652d 6c65 6e67 7468 203d 2031 3030 0d0a  e-length = 100..
-00000440: 0d0a 5b70 6570 385d 0d0a 6d61 782d 6c69  ..[pep8]..max-li
-00000450: 6e65 2d6c 656e 6774 6820 3d20 3130 300d  ne-length = 100.
-00000460: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
-00000470: 0d0a 756e 6976 6572 7361 6c20 3d20 300d  ..universal = 0.
-00000480: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
-00000490: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000004a0: 213d 322e 372e 2a2c 213d 332e 302e 2a2c  !=2.7.*,!=3.0.*,
-000004b0: 213d 332e 312e 2a2c 213d 332e 322e 2a2c  !=3.1.*,!=3.2.*,
-000004c0: 213d 332e 332e 2a2c 213d 332e 342e 2a0d  !=3.3.*,!=3.4.*.
-000004d0: 0a70 795f 6d6f 6475 6c65 7320 3d20 666c  .py_modules = fl
-000004e0: 6173 6b5f 6d69 6e69 6a73 6f6e 0d0a 0d0a  ask_minijson....
-000004f0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000500: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000510: 7465 203d 2030 0d0a 0d0a                 te = 0....
+000000d0: 5f65 6d61 696c 203d 2070 6d61 736c 616e  _email = pmaslan
+000000e0: 6b61 4073 6d6f 6b2e 636f 0d0a 6465 7363  ka@smok.co..desc
+000000f0: 7269 7074 696f 6e20 3d20 4120 466c 6173  ription = A Flas
+00000100: 6b20 6578 7465 6e73 696f 6e20 746f 2061  k extension to a
+00000110: 6c6c 6f77 2063 6c69 656e 7427 7320 746f  llow client's to
+00000120: 2073 7562 6d69 7420 6461 7461 2075 7369   submit data usi
+00000130: 6e67 2074 6865 204d 696e 694a 534f 4e20  ng the MiniJSON 
+00000140: 636f 6465 630d 0a75 726c 203d 2068 7474  codec..url = htt
+00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000160: 4472 6f6e 6568 7562 2f66 6c61 736b 2d6d  Dronehub/flask-m
+00000170: 696e 696a 736f 6e0d 0a70 726f 6a65 6374  inijson..project
+00000180: 5f75 726c 7320 3d20 0d0a 0943 6f64 6520  _urls = ...Code 
+00000190: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001a0: 2e63 6f6d 2f44 726f 6e65 6875 622f 666c  .com/Dronehub/fl
+000001b0: 6173 6b2d 6d69 6e69 6a73 6f6e 0d0a 0949  ask-minijson...I
+000001c0: 7373 7565 2074 7261 636b 6572 203d 2068  ssue tracker = h
+000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001e0: 6d2f 4472 6f6e 6568 7562 2f66 6c61 736b  m/Dronehub/flask
+000001f0: 2d6d 696e 696a 736f 6e2f 6973 7375 6573  -minijson/issues
+00000200: 0d0a 636c 6173 7369 6669 6572 203d 200d  ..classifier = .
+00000210: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+00000220: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
+00000230: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000240: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000250: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
+00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000270: 6f6e 203a 3a20 332e 350d 0a09 5072 6f67  on :: 3.5...Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002a0: 360d 0a09 5072 6f67 7261 6d6d 696e 6720  6...Programming 
+000002b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002c0: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002f0: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000310: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
+00000320: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000330: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
+00000340: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
+00000350: 4350 7974 686f 6e0d 0a09 5072 6f67 7261  CPython...Progra
+00000360: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000370: 3a20 5079 7468 6f6e 203a 3a20 496d 706c  : Python :: Impl
+00000380: 656d 656e 7461 7469 6f6e 203a 3a20 5079  ementation :: Py
+00000390: 5079 0d0a 094f 7065 7261 7469 6e67 2053  Py...Operating S
+000003a0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000003b0: 7065 6e64 656e 740d 0a09 4c69 6365 6e73  pendent...Licens
+000003c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000003d0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000003e0: 0d0a 0954 6f70 6963 203a 3a20 536f 6674  ...Topic :: Soft
+000003f0: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000400: 203a 3a20 4c69 6272 6172 6965 730d 0a0d   :: Libraries...
+00000410: 0a5b 7079 636f 6465 7374 796c 655d 0d0a  .[pycodestyle]..
+00000420: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
+00000430: 3d20 3130 300d 0a0d 0a5b 7065 7038 5d0d  = 100....[pep8].
+00000440: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+00000450: 203d 2031 3030 0d0a 0d0a 5b62 6469 7374   = 100....[bdist
+00000460: 5f77 6865 656c 5d0d 0a75 6e69 7665 7273  _wheel]..univers
+00000470: 616c 203d 2030 0d0a 0d0a 5b6f 7074 696f  al = 0....[optio
+00000480: 6e73 5d0d 0a70 7974 686f 6e5f 7265 7175  ns]..python_requ
+00000490: 6972 6573 203d 2021 3d32 2e37 2e2a 2c21  ires = !=2.7.*,!
+000004a0: 3d33 2e30 2e2a 2c21 3d33 2e31 2e2a 2c21  =3.0.*,!=3.1.*,!
+000004b0: 3d33 2e32 2e2a 2c21 3d33 2e33 2e2a 2c21  =3.2.*,!=3.3.*,!
+000004c0: 3d33 2e34 2e2a 0d0a 7079 5f6d 6f64 756c  =3.4.*..py_modul
+000004d0: 6573 203d 2066 6c61 736b 5f6d 696e 696a  es = flask_minij
+000004e0: 736f 6e0d 0a0d 0a5b 6567 675f 696e 666f  son....[egg_info
+000004f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000500: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000510: 0a                                       .
```

