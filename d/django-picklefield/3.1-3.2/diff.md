# Comparing `tmp/django-picklefield-3.1.tar.gz` & `tmp/django-picklefield-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-picklefield-3.1.tar", last modified: Sat Jun 18 20:20:49 2022, max compression
+gzip compressed data, was "django-picklefield-3.2.tar", last modified: Fri Apr  5 02:17:42 2024, max compression
```

## Comparing `django-picklefield-3.1.tar` & `django-picklefield-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 charettes   (501) staff       (20)        0 2022-06-18 20:20:49.533377 django-picklefield-3.1/
--rw-r--r--   0 charettes   (501) staff       (20)     1126 2022-06-18 15:34:24.000000 django-picklefield-3.1/LICENSE
--rw-r--r--   0 charettes   (501) staff       (20)       34 2022-06-18 15:34:24.000000 django-picklefield-3.1/MANIFEST.in
--rw-r--r--   0 charettes   (501) staff       (20)    11358 2022-06-18 20:20:49.533683 django-picklefield-3.1/PKG-INFO
--rw-r--r--   0 charettes   (501) staff       (20)    10152 2022-06-18 20:13:54.000000 django-picklefield-3.1/README.rst
-drwxr-xr-x   0 charettes   (501) staff       (20)        0 2022-06-18 20:20:49.530706 django-picklefield-3.1/django_picklefield.egg-info/
--rw-r--r--   0 charettes   (501) staff       (20)    11358 2022-06-18 20:20:49.000000 django-picklefield-3.1/django_picklefield.egg-info/PKG-INFO
--rw-r--r--   0 charettes   (501) staff       (20)      329 2022-06-18 20:20:49.000000 django-picklefield-3.1/django_picklefield.egg-info/SOURCES.txt
--rw-r--r--   0 charettes   (501) staff       (20)        1 2022-06-18 20:20:49.000000 django-picklefield-3.1/django_picklefield.egg-info/dependency_links.txt
--rw-r--r--   0 charettes   (501) staff       (20)       25 2022-06-18 20:20:49.000000 django-picklefield-3.1/django_picklefield.egg-info/requires.txt
--rw-r--r--   0 charettes   (501) staff       (20)       12 2022-06-18 20:20:49.000000 django-picklefield-3.1/django_picklefield.egg-info/top_level.txt
-drwxr-xr-x   0 charettes   (501) staff       (20)        0 2022-06-18 20:20:49.532691 django-picklefield-3.1/picklefield/
--rw-r--r--   0 charettes   (501) staff       (20)      276 2022-06-18 20:13:54.000000 django-picklefield-3.1/picklefield/__init__.py
--rw-r--r--   0 charettes   (501) staff       (20)       21 2022-06-18 15:34:24.000000 django-picklefield-3.1/picklefield/constants.py
--rw-r--r--   0 charettes   (501) staff       (20)     8264 2022-06-18 15:34:24.000000 django-picklefield-3.1/picklefield/fields.py
--rw-r--r--   0 charettes   (501) staff       (20)      322 2022-06-18 20:20:49.535288 django-picklefield-3.1/setup.cfg
--rw-r--r--   0 charettes   (501) staff       (20)     1545 2022-06-18 20:20:20.000000 django-picklefield-3.1/setup.py
+drwxr-xr-x   0 charettes   (501) staff       (20)        0 2024-04-05 02:17:42.632557 django-picklefield-3.2/
+-rw-r--r--   0 charettes   (501) staff       (20)     1126 2022-06-18 15:34:24.000000 django-picklefield-3.2/LICENSE
+-rw-r--r--   0 charettes   (501) staff       (20)       34 2022-06-18 15:34:24.000000 django-picklefield-3.2/MANIFEST.in
+-rw-r--r--   0 charettes   (501) staff       (20)    11770 2024-04-05 02:17:42.632881 django-picklefield-3.2/PKG-INFO
+-rw-r--r--   0 charettes   (501) staff       (20)    10344 2024-04-05 02:15:02.000000 django-picklefield-3.2/README.rst
+drwxr-xr-x   0 charettes   (501) staff       (20)        0 2024-04-05 02:17:42.627573 django-picklefield-3.2/django_picklefield.egg-info/
+-rw-r--r--   0 charettes   (501) staff       (20)    11770 2024-04-05 02:17:42.000000 django-picklefield-3.2/django_picklefield.egg-info/PKG-INFO
+-rw-r--r--   0 charettes   (501) staff       (20)      329 2024-04-05 02:17:42.000000 django-picklefield-3.2/django_picklefield.egg-info/SOURCES.txt
+-rw-r--r--   0 charettes   (501) staff       (20)        1 2024-04-05 02:17:42.000000 django-picklefield-3.2/django_picklefield.egg-info/dependency_links.txt
+-rw-r--r--   0 charettes   (501) staff       (20)       25 2024-04-05 02:17:42.000000 django-picklefield-3.2/django_picklefield.egg-info/requires.txt
+-rw-r--r--   0 charettes   (501) staff       (20)       12 2024-04-05 02:17:42.000000 django-picklefield-3.2/django_picklefield.egg-info/top_level.txt
+drwxr-xr-x   0 charettes   (501) staff       (20)        0 2024-04-05 02:17:42.631551 django-picklefield-3.2/picklefield/
+-rw-r--r--   0 charettes   (501) staff       (20)      276 2024-04-05 02:16:16.000000 django-picklefield-3.2/picklefield/__init__.py
+-rw-r--r--   0 charettes   (501) staff       (20)       21 2022-06-18 15:34:24.000000 django-picklefield-3.2/picklefield/constants.py
+-rw-r--r--   0 charettes   (501) staff       (20)     8264 2022-06-18 15:34:24.000000 django-picklefield-3.2/picklefield/fields.py
+-rw-r--r--   0 charettes   (501) staff       (20)      322 2024-04-05 02:17:42.634481 django-picklefield-3.2/setup.cfg
+-rw-r--r--   0 charettes   (501) staff       (20)     1760 2024-04-05 02:11:42.000000 django-picklefield-3.2/setup.py
```

### Comparing `django-picklefield-3.1/LICENSE` & `django-picklefield-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-picklefield-3.1/PKG-INFO` & `django-picklefield-3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: django-picklefield
-Version: 3.1
+Version: 3.2
 Summary: Pickled object field for Django
 Home-page: http://github.com/gintas/django-picklefield
 Author: Simon Charette
 Author-email: charette.s+django-picklefiel@gmail.com
 License: MIT
 Keywords: django pickle model field
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
@@ -189,18 +194,25 @@
 field editable=False by default (which I swear I already did once before!)
 since it is never a good idea to have a PickledObjectField be user editable.
 
 -------
 Changes
 -------
 
+Changes in version 3.2.0
+========================
+
+* Added tested support for Django 4.1, 4.2, 5.0.
+* Added tested support for Python 3.11, 3.12.
+* Dropped support for Python 3.6 and 3.7.
+
 Changes in version 3.1.0
 ========================
 
-* Added testing against Django 3.2 and 4.0.
+* Added tested support for Django 3.2 and 4.0.
 
 Changes in version 3.0.1
 ========================
 
 * None; addressed a packaging issue with 3.0.0
 
 Changes in version 3.0.0
```

### Comparing `django-picklefield-3.1/README.rst` & `django-picklefield-3.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -158,18 +158,25 @@
 field editable=False by default (which I swear I already did once before!)
 since it is never a good idea to have a PickledObjectField be user editable.
 
 -------
 Changes
 -------
 
+Changes in version 3.2.0
+========================
+
+* Added tested support for Django 4.1, 4.2, 5.0.
+* Added tested support for Python 3.11, 3.12.
+* Dropped support for Python 3.6 and 3.7.
+
 Changes in version 3.1.0
 ========================
 
-* Added testing against Django 3.2 and 4.0.
+* Added tested support for Django 3.2 and 4.0.
 
 Changes in version 3.0.1
 ========================
 
 * None; addressed a packaging issue with 3.0.0
 
 Changes in version 3.0.0
```

### Comparing `django-picklefield-3.1/django_picklefield.egg-info/PKG-INFO` & `django-picklefield-3.2/django_picklefield.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: django-picklefield
-Version: 3.1
+Version: 3.2
 Summary: Pickled object field for Django
 Home-page: http://github.com/gintas/django-picklefield
 Author: Simon Charette
 Author-email: charette.s+django-picklefiel@gmail.com
 License: MIT
 Keywords: django pickle model field
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
@@ -189,18 +194,25 @@
 field editable=False by default (which I swear I already did once before!)
 since it is never a good idea to have a PickledObjectField be user editable.
 
 -------
 Changes
 -------
 
+Changes in version 3.2.0
+========================
+
+* Added tested support for Django 4.1, 4.2, 5.0.
+* Added tested support for Python 3.11, 3.12.
+* Dropped support for Python 3.6 and 3.7.
+
 Changes in version 3.1.0
 ========================
 
-* Added testing against Django 3.2 and 4.0.
+* Added tested support for Django 3.2 and 4.0.
 
 Changes in version 3.0.1
 ========================
 
 * None; addressed a packaging issue with 3.0.0
 
 Changes in version 3.0.0
```

### Comparing `django-picklefield-3.1/picklefield/fields.py` & `django-picklefield-3.2/picklefield/fields.py`

 * *Files identical despite different names*

### Comparing `django-picklefield-3.1/setup.py` & `django-picklefield-3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,28 @@
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords=['django pickle model field'],
     packages=find_packages(exclude=['tests', 'tests.*']),
     python_requires='>=3',
     install_requires=['Django>=3.2'],
```

