# Comparing `tmp/flask_shopify_utils-0.1.2.tar.gz` & `tmp/flask_shopify_utils-0.1.3.tar.gz`

## Comparing `flask_shopify_utils-0.1.2.tar` & `flask_shopify_utils-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/test_alpha.py
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/test_default_routes.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/test_graphql_cli.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/tests/test_ui_routes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/LICENSE
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/README.md
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34768 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_alpha.py
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_ui_routes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/PKG-INFO
```

### Comparing `flask_shopify_utils-0.1.2/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.1.3/src/flask_shopify_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
@@ -656,15 +656,16 @@
             if not scopes:
                 resp = self.proxy_response(500, 'Something went wrong while fetching installation data!')
                 resp.status_code = 500
                 return resp
             record.scopes = ','.join(list(map(lambda x: x['handle'], scopes['accessScopes'])))
             self.db.commit()
             # Register GDPR mandatory webhook @todo
-            return redirect('https://{}/admin/app/{}'.format(
+            # https://shopify.dev/docs/apps/auth/get-access-tokens/authorization-code-grant/getting-started
+            return redirect('https://{}/apps/{}'.format(
                 g.store_key,
                 self.config.get('SHOPIFY_API_KEY'))
             )
 
         # Register the `install` route
         @default_routes.route('/install', methods=['GET'], endpoint='install')
         def install():
```

### Comparing `flask_shopify_utils-0.1.2/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.1.3/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.1.3/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/tests/conftest.py` & `flask_shopify_utils-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/tests/test_alpha.py` & `flask_shopify_utils-0.1.3/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/tests/test_default_routes.py` & `flask_shopify_utils-0.1.3/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.1.3/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/tests/test_ui_routes.py` & `flask_shopify_utils-0.1.3/tests/test_ui_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/LICENSE` & `flask_shopify_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/README.md` & `flask_shopify_utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.2/pyproject.toml` & `flask_shopify_utils-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,28 @@
     "Framework :: Flask"
 ]
 dependencies = [
     "Flask < 4",
     "Flask-SQLAlchemy < 4",
     "ShopifyAPI == 12.4.0",
     "sgqlc < 17",
-    "psutil == 5.9.5",
-    "pytz == 2023.3",
+    "psutil < 6",
+    "pytz == 2024.1",
     "requests < 3",
     "Cerberus == 1.3.5",
     "PyJWT == 2.8.0",
     "simplejson < 4"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "pytest == 7.4.2"
+    "pytest == 8.1.1",
+    "twine == 5.0.0",
+    "build == 1.2.1"
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = '-vs'
 testpaths = ["tests"]
 python_files = ["test_*.py"]
```

### Comparing `flask_shopify_utils-0.1.2/PKG-INFO` & `flask_shopify_utils-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: flask-shopify-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
@@ -16,23 +16,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: cerberus==1.3.5
 Requires-Dist: flask-sqlalchemy<4
 Requires-Dist: flask<4
-Requires-Dist: psutil==5.9.5
+Requires-Dist: psutil<6
 Requires-Dist: pyjwt==2.8.0
-Requires-Dist: pytz==2023.3
+Requires-Dist: pytz==2024.1
 Requires-Dist: requests<3
 Requires-Dist: sgqlc<17
 Requires-Dist: shopifyapi==12.4.0
 Requires-Dist: simplejson<4
 Provides-Extra: dev
-Requires-Dist: pytest==7.4.2; extra == 'dev'
+Requires-Dist: build==1.2.1; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
+Requires-Dist: twine==5.0.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Flask-Shopify-Utils
 
 The utils for Flask Application that build for Shopify Custom App 
 
 ---
```

