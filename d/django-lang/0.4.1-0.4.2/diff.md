# Comparing `tmp/django-lang-0.4.1.tar.gz` & `tmp/django-lang-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lang-0.4.1.tar", last modified: Sun Mar 31 22:09:35 2024, max compression
+gzip compressed data, was "django-lang-0.4.2.tar", last modified: Fri Apr  5 20:25:58 2024, max compression
```

## Comparing `django-lang-0.4.1.tar` & `django-lang-0.4.2.tar`

### file list

```diff
@@ -1,58 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-31 22:09:25.000000 django-lang-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-31 22:09:25.000000 django-lang-0.4.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-31 22:09:25.000000 django-lang-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-31 22:09:25.000000 django-lang-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-31 22:09:25.000000 django-lang-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-31 22:09:35.008990 django-lang-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-31 22:09:25.000000 django-lang-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-31 22:09:25.000000 django-lang-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-31 22:09:25.000000 django-lang-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.004990 django-lang-0.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44607 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44178 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44917 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44629 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-31 22:09:25.000000 django-lang-0.4.1/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-31 22:09:25.000000 django-lang-0.4.1/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-31 22:09:35.008990 django-lang-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-31 22:09:25.000000 django-lang-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.000990 django-lang-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/src/django_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 22:09:34.000000 django-lang-0.4.1/src/django_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/src/lang/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.000990 django-lang-0.4.1/src/lang/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.000990 django-lang-0.4.1/src/lang/static/lang/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/src/lang/static/lang/css/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/static/lang/css/nav-link.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/src/lang/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/templates/hreflang.html
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/templates/nav-link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/src/lang/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/templatetags/languages_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-31 22:09:25.000000 django-lang-0.4.1/src/lang/templatetags/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:35.008990 django-lang-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 22:09:25.000000 django-lang-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-31 22:09:25.000000 django-lang-0.4.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-31 22:09:25.000000 django-lang-0.4.1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-31 22:09:25.000000 django-lang-0.4.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-31 22:09:25.000000 django-lang-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.834766 django-lang-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 20:25:48.000000 django-lang-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 20:25:48.000000 django-lang-0.4.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 20:25:48.000000 django-lang-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 20:25:48.000000 django-lang-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 20:25:48.000000 django-lang-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-05 20:25:58.834766 django-lang-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-05 20:25:48.000000 django-lang-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 20:25:48.000000 django-lang-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-05 20:25:48.000000 django-lang-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 20:25:48.000000 django-lang-0.4.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 20:25:48.000000 django-lang-0.4.2/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-05 20:25:58.834766 django-lang-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 20:25:48.000000 django-lang-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.822766 django-lang-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/src/django_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 20:25:58.000000 django-lang-0.4.2/src/django_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/src/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.826766 django-lang-0.4.2/src/lang/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.826766 django-lang-0.4.2/src/lang/static/lang/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/src/lang/static/lang/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/static/lang/css/nav-link.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/src/lang/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/templates/hreflang.html
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/templates/nav-link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/src/lang/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/templatetags/languages_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-05 20:25:48.000000 django-lang-0.4.2/src/lang/templatetags/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:58.830766 django-lang-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:25:48.000000 django-lang-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-05 20:25:48.000000 django-lang-0.4.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 20:25:48.000000 django-lang-0.4.2/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-05 20:25:48.000000 django-lang-0.4.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 20:25:48.000000 django-lang-0.4.2/tox.ini
```

### Comparing `django-lang-0.4.1/.pre-commit-config.yaml` & `django-lang-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/LICENSE` & `django-lang-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/PKG-INFO` & `django-lang-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lang
-Version: 0.4.1
+Version: 0.4.2
 Summary: Django application to provide useful utils and reusable parts of code for multi-languages sites.
 Home-page: https://github.com/DLRSP/django-lang
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-lang-0.4.1/README.md` & `django-lang-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/mkdocs.yml` & `django-lang-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/pyproject.toml` & `django-lang-0.4.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     --strict-markers
     --ds=tests.settings
     """
 django_find_project = false
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "0.4.1"
+current_version = "0.4.2"
 commit = true
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
```

### Comparing `django-lang-0.4.1/requirements/py310-django32.txt` & `django-lang-0.4.2/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py310-django42.txt` & `django-lang-0.4.2/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py311-django32.txt` & `django-lang-0.4.2/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py311-django42.txt` & `django-lang-0.4.2/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py38-django32.txt` & `django-lang-0.4.2/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py38-django42.txt` & `django-lang-0.4.2/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py39-django32.txt` & `django-lang-0.4.2/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/requirements/py39-django42.txt` & `django-lang-0.4.2/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/runtests.py` & `django-lang-0.4.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/setup.cfg` & `django-lang-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-lang
-version = 0.4.1
+version = 0.4.2
 url = https://github.com/DLRSP/django-lang
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application to provide useful utils and reusable parts of code for multi-languages sites.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-lang-0.4.1/setup.py` & `django-lang-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/src/django_lang.egg-info/PKG-INFO` & `django-lang-0.4.2/src/django_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lang
-Version: 0.4.1
+Version: 0.4.2
 Summary: Django application to provide useful utils and reusable parts of code for multi-languages sites.
 Home-page: https://github.com/DLRSP/django-lang
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-lang-0.4.1/src/django_lang.egg-info/SOURCES.txt` & `django-lang-0.4.2/src/django_lang.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 README.md
 mkdocs.yml
 pyproject.toml
 runtests.py
 setup.cfg
 setup.py
 tox.ini
-requirements/dev.in
-requirements/docs.in
-requirements/docs.txt
-requirements/py310-dev.txt
 requirements/py310-django32.txt
 requirements/py310-django42.txt
-requirements/py311-dev.txt
 requirements/py311-django32.txt
 requirements/py311-django42.txt
-requirements/py38-dev.txt
 requirements/py38-django32.txt
 requirements/py38-django42.txt
-requirements/py39-dev.txt
 requirements/py39-django32.txt
 requirements/py39-django42.txt
 requirements/requirements.in
 src/django_lang.egg-info/PKG-INFO
 src/django_lang.egg-info/SOURCES.txt
 src/django_lang.egg-info/dependency_links.txt
 src/django_lang.egg-info/not-zip-safe
```

### Comparing `django-lang-0.4.1/src/lang/templates/nav-link.html` & `django-lang-0.4.2/src/lang/templates/nav-link.html`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/src/lang/templatetags/languages_helpers.py` & `django-lang-0.4.2/src/lang/templatetags/languages_helpers.py`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/src/lang/templatetags/urls.py` & `django-lang-0.4.2/src/lang/templatetags/urls.py`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/tests/settings.py` & `django-lang-0.4.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-lang-0.4.1/tests/test_fake.py` & `django-lang-0.4.2/tests/test_fake.py`

 * *Files identical despite different names*

