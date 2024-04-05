# Comparing `tmp/pyramid_beaker-0.8.tar.gz` & `tmp/pyramid_beaker-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_beaker-0.8.tar", last modified: Fri Jun 28 07:46:25 2013, max compression
+gzip compressed data, was "pyramid_beaker-0.9.tar", last modified: Fri Mar 29 10:57:38 2024, max compression
```

## Comparing `pyramid_beaker-0.8.tar` & `pyramid_beaker-0.9.tar`

### file list

```diff
@@ -1,31 +1,16 @@
-drwxrwxr-x   0 chrism    (1000) chrism    (1000)        0 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     4102 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/PKG-INFO
-drwxrwxr-x   0 chrism    (1000) chrism    (1000)        0 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/pyramid_beaker/
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     6118 2012-09-09 04:29:45.000000 pyramid_beaker-0.8/pyramid_beaker/__init__.py
--rw-rw-r--   0 chrism    (1000) chrism    (1000)    13810 2012-09-09 04:29:45.000000 pyramid_beaker-0.8/pyramid_beaker/tests.py
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      109 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/COPYRIGHT.txt
-drwxrwxr-x   0 chrism    (1000) chrism    (1000)        0 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/docs/
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     5821 2012-09-09 04:29:45.000000 pyramid_beaker-0.8/docs/index.rst
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      399 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/docs/glossary.rst
-drwxrwxr-x   0 chrism    (1000) chrism    (1000)        0 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/docs/.static/
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     3924 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/docs/.static/logo_hi.gif
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      378 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/docs/.static/repoze.css
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     6953 2013-06-28 07:45:31.000000 pyramid_beaker-0.8/docs/conf.py
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      216 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/docs/api.rst
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     2566 2012-07-10 21:18:08.000000 pyramid_beaker-0.8/docs/Makefile
--rw-rw-r--   0 chrism    (1000) chrism    (1000)       17 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/docs/.gitignore
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      312 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/setup.cfg
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     5200 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/CONTRIBUTORS.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     2385 2013-06-28 07:45:37.000000 pyramid_beaker-0.8/setup.py
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      576 2012-07-10 21:01:47.000000 pyramid_beaker-0.8/tox.ini
-drwxrwxr-x   0 chrism    (1000) chrism    (1000)        0 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     4102 2013-06-28 07:46:22.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/PKG-INFO
--rw-rw-r--   0 chrism    (1000) chrism    (1000)        1 2012-07-10 17:51:58.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/not-zip-safe
--rw-rw-r--   0 chrism    (1000) chrism    (1000)        1 2013-06-28 07:46:22.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/dependency_links.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)       15 2013-06-28 07:46:22.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/top_level.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      518 2013-06-28 07:46:25.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/SOURCES.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)       63 2013-06-28 07:46:22.000000 pyramid_beaker-0.8/pyramid_beaker.egg-info/requires.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     2201 2013-06-28 07:45:24.000000 pyramid_beaker-0.8/CHANGES.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)      290 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/README.txt
--rw-rw-r--   0 chrism    (1000) chrism    (1000)       96 2012-07-10 21:11:35.000000 pyramid_beaker-0.8/.gitignore
--rw-rw-r--   0 chrism    (1000) chrism    (1000)     1791 2012-07-10 17:51:30.000000 pyramid_beaker-0.8/LICENSE.txt
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-03-29 10:57:38.566779 pyramid_beaker-0.9/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1791 2024-02-27 10:38:44.000000 pyramid_beaker-0.9/LICENSE.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4012 2024-03-29 10:57:38.566586 pyramid_beaker-0.9/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      238 2024-02-28 16:48:45.000000 pyramid_beaker-0.9/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-03-29 10:57:38.562214 pyramid_beaker-0.9/pyramid_beaker/
+-rw-r--r--   0 fschulze   (501) staff       (20)     6158 2024-02-27 10:38:44.000000 pyramid_beaker-0.9/pyramid_beaker/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    14021 2024-02-28 16:48:45.000000 pyramid_beaker-0.9/pyramid_beaker/tests.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-03-29 10:57:38.565342 pyramid_beaker-0.9/pyramid_beaker.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     4012 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      318 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)       85 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       15 2024-03-29 10:57:38.000000 pyramid_beaker-0.9/pyramid_beaker.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      291 2024-03-29 10:57:38.567364 pyramid_beaker-0.9/setup.cfg
+-rw-r--r--   0 fschulze   (501) staff       (20)     2614 2024-03-29 10:54:26.000000 pyramid_beaker-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_beaker-0.8/pyramid_beaker/__init__.py` & `pyramid_beaker-0.9/pyramid_beaker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,18 @@
         _cookie_on_exception = _options.pop('cookie_on_exception', True)
         _constant_csrf_token = _options.pop('constant_csrf_token', False)
 
         def __init__(self, request):
             SessionObject.__init__(self, request.environ, **self._options)
             def session_callback(request, response):
                 exception = getattr(request, 'exception', None)
-                if (exception is None or self._cookie_on_exception
-                    and self.accessed()):
+                if (
+                    (exception is None or self._cookie_on_exception)
+                    and self.accessed()
+                ):
                     self.persist()
                     headers = self.__dict__['_headers']
                     if headers['set_cookie'] and headers['cookie_out']:
                         response.headerlist.append(
                             ('Set-Cookie', headers['cookie_out']))
             request.add_response_callback(session_callback)
```

### Comparing `pyramid_beaker-0.8/pyramid_beaker/tests.py` & `pyramid_beaker-0.9/pyramid_beaker/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,16 +341,24 @@
         set_cache_regions_from_settings(settings)
         default_term = beaker.cache.cache_regions.get('default_term')
         short_term = beaker.cache.cache_regions.get('short_term')
         self.assertFalse(short_term.get('enabled'))
         self.assertFalse(default_term.get('enabled'))
 
 class TestIncludeMe(unittest.TestCase):
-    def test_includeme(self):
-        from pyramid.interfaces import ISessionFactory
+    def setUp(self):
         from pyramid import testing
+        self.config = testing.setUp()
+    
+    def _callFUT(self, config):
         from pyramid_beaker import includeme
-        config = testing.setUp(settings={})
-        includeme(config)
-        session_factory = config.registry.queryUtility(ISessionFactory)
-        self.assertEqual(str(session_factory),
-                "<class 'pyramid_beaker.PyramidBeakerSessionObject'>")
+        return includeme(self.config)
+
+    def test_it(self):
+        from pyramid.interfaces import ISessionFactory
+        from pyramid_beaker import BeakerSessionFactoryConfig
+        self._callFUT(self.config)
+        session_factory = self.config.registry.queryUtility(ISessionFactory)
+        self.assertEqual(
+                            str(session_factory), 
+                            str(BeakerSessionFactoryConfig())
+                            )
```

### Comparing `pyramid_beaker-0.8/setup.py` & `pyramid_beaker-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,58 +15,62 @@
 import os
 
 from setuptools import setup
 from setuptools import find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
-    README = open(os.path.join(here, 'README.txt')).read()
+    README = open(os.path.join(here, 'README.rst')).read()
     CHANGES = open(os.path.join(here, 'CHANGES.txt')).read()
 except:
     README = ''
     CHANGES = ''
 
 requires = ['pyramid', 'beaker']
 
 docs_extras = [
     'Sphinx',
     'docutils',
+    'pylons-sphinx-themes',
     ]
 
 testing_extras = [
     'nose',
     'coverage',
     ]
 
 setup(name='pyramid_beaker',
-      version='0.8',
+      version='0.9',
       description='Beaker session factory backend for Pyramid',
       long_description=README + '\n\n' +  CHANGES,
       classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.2",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Pyramid",
         ],
       keywords='web wsgi pylons pyramid',
       author="Chris McDonough, Agendaless Consulting",
-      author_email="pylons-devel@googlegroups.com",
-      url="http://docs.pylonsproject.org/projects/pyramid_beaker/en/latest/",
+      author_email="pylons-discuss@googlegroups.com",
+      url="https://docs.pylonsproject.org/projects/pyramid_beaker/en/latest/",
       license="BSD-derived (http://www.repoze.org/LICENSE.txt)",
       packages=find_packages(),
       include_package_data=True,
       zip_safe=False,
       tests_require = requires,
       install_requires = requires,
       extras_require = {
           'testing':testing_extras,
           'docs':docs_extras,
           },
       test_suite="pyramid_beaker",
       )
-
```

### Comparing `pyramid_beaker-0.8/LICENSE.txt` & `pyramid_beaker-0.9/LICENSE.txt`

 * *Files identical despite different names*

