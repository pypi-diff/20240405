# Comparing `tmp/Paste-3.7.1.tar.gz` & `tmp/Paste-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Paste-3.7.1.tar", last modified: Thu Oct 19 10:27:48 2023, max compression
+gzip compressed data, was "Paste-3.8.0.tar", last modified: Sat Mar 16 14:50:51 2024, max compression
```

## Comparing `Paste-3.7.1.tar` & `Paste-3.8.0.tar`

### file list

```diff
@@ -1,274 +1,273 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.041615 Paste-3.7.1/
--rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.7.1/MANIFEST.in
--rw-r--r--   0 cdent      (503) staff       (20)     4779 2023-10-19 10:27:48.041696 Paste-3.7.1/PKG-INFO
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.979779 Paste-3.7.1/Paste.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     4779 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     6439 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1900 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/namespace_packages.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/not-zip-safe
--rw-r--r--   0 cdent      (503) staff       (20)       93 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2023-10-19 10:27:47.000000 Paste-3.7.1/Paste.egg-info/top_level.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3454 2023-10-19 10:24:33.000000 Paste-3.7.1/README.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.983163 Paste-3.7.1/docs/
--rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/DeveloperGuidelines.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/StyleGuide.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.983612 Paste-3.7.1/docs/_static/
--rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/_static/default.css
--rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/_static/paste.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.984201 Paste-3.7.1/docs/community/
--rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/community/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/community/mailing-list.txt
--rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/community/repository.txt
--rw-r--r--   0 cdent      (503) staff       (20)     4078 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/developer-features.txt
--rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/do-it-yourself-framework.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.984401 Paste-3.7.1/docs/download/
--rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/download/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/future.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:47.984842 Paste-3.7.1/docs/include/
--rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/include/contact.txt
--rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/include/reference_header.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/license.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.001850 Paste-3.7.1/docs/modules/
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.auth_tkt.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.basic.txt
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.cas.txt
--rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.cookie.txt
--rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.digest.txt
--rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.form.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.grantip.txt
--rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/auth.multi.txt
--rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/cascade.txt
--rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/cgiapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/cgitb_catcher.txt
--rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.debugapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.fsdiff.txt
--rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.prints.txt
--rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.profile.txt
--rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.watchthreads.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/debug.wdg_validate.txt
--rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/errordocument.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/evalexception.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/exceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/fileapp.txt
--rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/fixture.txt
--rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/gzipper.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/httpexceptions.txt
--rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/httpheaders.txt
--rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/httpserver.txt
--rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/lint.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/pony.txt
--rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/progress.txt
--rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/proxy.txt
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/recursive.txt
--rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/registry.txt
--rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/reloader.txt
--rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/request.txt
--rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/response.txt
--rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/session.txt
--rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/transaction.txt
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/translogger.txt
--rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/url.txt
--rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/urlmap.txt
--rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/urlparser.txt
--rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/util.import_string.txt
--rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/util.multidict.txt
--rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/wsgilib.txt
--rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/modules/wsgiwrappers.txt
--rw-r--r--   0 cdent      (503) staff       (20)    41218 2023-10-19 10:24:33.000000 Paste-3.7.1/docs/news.txt
--rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/paste-httpserver-threadpool.txt
--rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/test_server.ini
--rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/testing-applications.txt
--rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/url-parsing-with-wsgi.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.002602 Paste-3.7.1/docs/web/
--rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/web/default-site.css
--rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/web/site.js
--rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.7.1/docs/web/style.css
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.010140 Paste-3.7.1/paste/
--rw-r--r--   0 cdent      (503) staff       (20)      551 2023-10-15 13:05:17.000000 Paste-3.7.1/paste/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.012422 Paste-3.7.1/paste/auth/
--rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    16601 2020-07-22 15:14:09.000000 Paste-3.7.1/paste/auth/auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     4136 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/auth/basic.py
--rw-r--r--   0 cdent      (503) staff       (20)     4006 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/cas.py
--rw-r--r--   0 cdent      (503) staff       (20)    16588 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     9304 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/form.py
--rw-r--r--   0 cdent      (503) staff       (20)     4021 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/multi.py
--rw-r--r--   0 cdent      (503) staff       (20)    16276 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/auth/open_id.py
--rw-r--r--   0 cdent      (503) staff       (20)     4475 2020-01-28 15:54:01.000000 Paste-3.7.1/paste/cascade.py
--rw-r--r--   0 cdent      (503) staff       (20)     9742 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     3903 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/config.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.013612 Paste-3.7.1/paste/cowbell/
--rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/cowbell/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/cowbell/bell-ascending.png
--rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/cowbell/bell-descending.png
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.015756 Paste-3.7.1/paste/debug/
--rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/__init__.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/debugapp.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    14923 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/doctest_webapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/fsdiff.py
--rw-r--r--   0 cdent      (503) staff       (20)     5574 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/prints.py
--rw-r--r--   0 cdent      (503) staff       (20)     7607 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/profile.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     3396 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/testserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    10839 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/watchthreads.py
--rw-r--r--   0 cdent      (503) staff       (20)     4268 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/debug/wdg_validate.py
--rw-r--r--   0 cdent      (503) staff       (20)    13904 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.016358 Paste-3.7.1/paste/evalexception/
--rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     2155 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/evalcontext.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.017812 Paste-3.7.1/paste/evalexception/media/
--rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/media/MochiKit.packed.js
--rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/media/debug.js
--rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/media/minus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/evalexception/media/plus.jpg
--rw-r--r--   0 cdent      (503) staff       (20)    22254 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/evalexception/middleware.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.020478 Paste-3.7.1/paste/exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    19681 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/exceptions/collector.py
--rw-r--r--   0 cdent      (503) staff       (20)    17045 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/exceptions/errormiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)    19504 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/exceptions/formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4576 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/exceptions/reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4127 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/exceptions/serial_number_generator.py
--rw-r--r--   0 cdent      (503) staff       (20)    13698 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)    59616 2020-09-24 15:58:29.000000 Paste-3.7.1/paste/fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/flup_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     3819 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)    24522 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)    43615 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/httpheaders.py
--rwxr-xr-x   0 cdent      (503) staff       (20)    57237 2022-06-22 10:14:29.000000 Paste-3.7.1/paste/httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    14988 2020-10-12 12:27:11.000000 Paste-3.7.1/paste/lint.py
--rw-r--r--   0 cdent      (503) staff       (20)     7830 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/modpython.py
--rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/pony.py
--rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/progress.py
--rw-r--r--   0 cdent      (503) staff       (20)    10192 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)    14708 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    22275 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     6038 2022-06-22 10:14:29.000000 Paste-3.7.1/paste/reloader.py
--rw-r--r--   0 cdent      (503) staff       (20)    14123 2023-10-19 10:03:40.000000 Paste-3.7.1/paste/request.py
--rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/response.py
--rw-r--r--   0 cdent      (503) staff       (20)    11554 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/session.py
--rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/transaction.py
--rw-r--r--   0 cdent      (503) staff       (20)     5218 2023-10-02 19:24:33.000000 Paste-3.7.1/paste/translogger.py
--rw-r--r--   0 cdent      (503) staff       (20)    14738 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/url.py
--rw-r--r--   0 cdent      (503) staff       (20)     9369 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)    26865 2023-04-30 11:31:00.000000 Paste-3.7.1/paste/urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.028013 Paste-3.7.1/paste/util/
--rw-r--r--   0 cdent      (503) staff       (20)    83623 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/PySourceColor.py
--rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/classinit.py
--rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/classinstance.py
--rw-r--r--   0 cdent      (503) staff       (20)      913 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/converters.py
--rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/dateinterval.py
--rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/filemixin.py
--rw-r--r--   0 cdent      (503) staff       (20)     3846 2023-10-19 10:03:40.000000 Paste-3.7.1/paste/util/finddata.py
--rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/findpackage.py
--rw-r--r--   0 cdent      (503) staff       (20)      802 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/html.py
--rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)    19262 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/intset.py
--rw-r--r--   0 cdent      (503) staff       (20)     9320 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/ip4.py
--rw-r--r--   0 cdent      (503) staff       (20)     1227 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/killthread.py
--rw-r--r--   0 cdent      (503) staff       (20)     4036 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/looper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)    12682 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)     2351 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)     5612 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/scgiserver.py
--rw-r--r--   0 cdent      (503) staff       (20)    24403 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/template.py
--rw-r--r--   0 cdent      (503) staff       (20)     8175 2022-06-22 10:14:29.000000 Paste-3.7.1/paste/util/threadedprint.py
--rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/util/threadinglocal.py
--rw-r--r--   0 cdent      (503) staff       (20)    20470 2022-08-18 20:32:03.000000 Paste-3.7.1/paste/wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)    22299 2020-01-26 15:30:37.000000 Paste-3.7.1/paste/wsgiwrappers.py
--rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.7.1/regen-docs
--rw-r--r--   0 cdent      (503) staff       (20)      162 2023-10-19 10:27:48.042003 Paste-3.7.1/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)     4612 2023-10-19 10:26:55.000000 Paste-3.7.1/setup.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.033545 Paste-3.7.1/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.034359 Paste-3.7.1/tests/cgiapp_data/
--rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/cgiapp_data/error.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)     2039 2023-04-30 11:31:00.000000 Paste-3.7.1/tests/cgiapp_data/form.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/cgiapp_data/ok.cgi
--rwxr-xr-x   0 cdent      (503) staff       (20)      223 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/cgiapp_data/stderr.cgi
--rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/template.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.035148 Paste-3.7.1/tests/test_auth/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_auth/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     1527 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_auth/test_auth_cookie.py
--rw-r--r--   0 cdent      (503) staff       (20)     3077 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_auth/test_auth_digest.py
--rw-r--r--   0 cdent      (503) staff       (20)     3832 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_auth/test_auth_tkt.py
--rw-r--r--   0 cdent      (503) staff       (20)     2053 2020-10-12 12:27:11.000000 Paste-3.7.1/tests/test_cgiapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2249 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_cgitb_catcher.py
--rw-r--r--   0 cdent      (503) staff       (20)     2901 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_config.py
--rw-r--r--   0 cdent      (503) staff       (20)     1533 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_doctests.py
--rw-r--r--   0 cdent      (503) staff       (20)     3461 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_errordocument.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.036128 Paste-3.7.1/tests/test_exceptions/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_exceptions/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     3389 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_exceptions/test_error_middleware.py
--rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_exceptions/test_formatter.py
--rw-r--r--   0 cdent      (503) staff       (20)     4055 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_exceptions/test_httpexceptions.py
--rw-r--r--   0 cdent      (503) staff       (20)     1280 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_exceptions/test_reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)     9766 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_fileapp.py
--rw-r--r--   0 cdent      (503) staff       (20)     2489 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     1264 2023-04-30 11:31:00.000000 Paste-3.7.1/tests/test_grantip.py
--rw-r--r--   0 cdent      (503) staff       (20)      888 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_gzipper.py
--rw-r--r--   0 cdent      (503) staff       (20)     6505 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_httpheaders.py
--rw-r--r--   0 cdent      (503) staff       (20)     3447 2020-02-12 10:40:19.000000 Paste-3.7.1/tests/test_httpserver.py
--rw-r--r--   0 cdent      (503) staff       (20)      477 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_import_string.py
--rw-r--r--   0 cdent      (503) staff       (20)     5255 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_multidict.py
--rw-r--r--   0 cdent      (503) staff       (20)      721 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_profilemiddleware.py
--rw-r--r--   0 cdent      (503) staff       (20)      624 2023-04-30 11:31:00.000000 Paste-3.7.1/tests/test_proxy.py
--rw-r--r--   0 cdent      (503) staff       (20)     4178 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_recursive.py
--rw-r--r--   0 cdent      (503) staff       (20)    11149 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_registry.py
--rw-r--r--   0 cdent      (503) staff       (20)     2354 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_request.py
--rw-r--r--   0 cdent      (503) staff       (20)     1465 2023-10-19 10:03:40.000000 Paste-3.7.1/tests/test_request_form.py
--rw-r--r--   0 cdent      (503) staff       (20)      369 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_response.py
--rw-r--r--   0 cdent      (503) staff       (20)     1587 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_session.py
--rw-r--r--   0 cdent      (503) staff       (20)     1810 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_urlmap.py
--rw-r--r--   0 cdent      (503) staff       (20)     6944 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_urlparser.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.036857 Paste-3.7.1/tests/test_util/
--rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_util/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     6026 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_util/test_datetimeutil.py
--rw-r--r--   0 cdent      (503) staff       (20)    11873 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_util/test_mimeparse.py
--rw-r--r--   0 cdent      (503) staff       (20)     1171 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_util/test_quoting.py
--rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_wsgilib.py
--rw-r--r--   0 cdent      (503) staff       (20)     6441 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/test_wsgiwrappers.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.037338 Paste-3.7.1/tests/urlparser_data/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.037527 Paste-3.7.1/tests/urlparser_data/deep/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/deep/index.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.037721 Paste-3.7.1/tests/urlparser_data/deep/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/deep/sub/Main.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.038300 Paste-3.7.1/tests/urlparser_data/find_file/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.038498 Paste-3.7.1/tests/urlparser_data/find_file/dir with spaces/
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/find_file/dir with spaces/test 4.html
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/find_file/index.txt
--rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/find_file/test 3.html
--rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/find_file/test2.html
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.039078 Paste-3.7.1/tests/urlparser_data/hook/
--rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/hook/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      231 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/hook/app.py
--rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/hook/index.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.039266 Paste-3.7.1/tests/urlparser_data/not_found/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/__init__.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.039648 Paste-3.7.1/tests/urlparser_data/not_found/recur/
--rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/recur/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/recur/isfound.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.040051 Paste-3.7.1/tests/urlparser_data/not_found/simple/
--rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/simple/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/simple/found.txt
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.040463 Paste-3.7.1/tests/urlparser_data/not_found/user/
--rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/user/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      235 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/not_found/user/list.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.041054 Paste-3.7.1/tests/urlparser_data/python/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/python/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/python/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/python/stream.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-10-19 10:27:48.041459 Paste-3.7.1/tests/urlparser_data/python/sub/
--rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/python/sub/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/python/sub/simpleapp.py
--rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.7.1/tests/urlparser_data/secured.txt
--rw-r--r--   0 cdent      (503) staff       (20)      365 2023-10-19 10:24:33.000000 Paste-3.7.1/tox.ini
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.022458 Paste-3.8.0/
+-rw-r--r--   0 cdent      (503) staff       (20)      323 2020-01-26 15:30:37.000000 Paste-3.8.0/MANIFEST.in
+-rw-r--r--   0 cdent      (503) staff       (20)     4908 2024-03-16 14:50:51.022296 Paste-3.8.0/PKG-INFO
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.021642 Paste-3.8.0/Paste.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     4908 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     6420 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1900 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/namespace_packages.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/not-zip-safe
+-rw-r--r--   0 cdent      (503) staff       (20)       93 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2024-03-16 14:50:50.000000 Paste-3.8.0/Paste.egg-info/top_level.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3446 2024-03-16 14:39:27.000000 Paste-3.8.0/README.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.939221 Paste-3.8.0/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)     4608 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/DeveloperGuidelines.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3170 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/StyleGuide.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.939777 Paste-3.8.0/docs/_static/
+-rw-r--r--   0 cdent      (503) staff       (20)     5988 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/_static/default.css
+-rw-r--r--   0 cdent      (503) staff       (20)      194 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/_static/paste.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.940601 Paste-3.8.0/docs/community/
+-rw-r--r--   0 cdent      (503) staff       (20)      571 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      759 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/mailing-list.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      141 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/community/repository.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3886 2024-03-16 14:46:49.000000 Paste-3.8.0/docs/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4500 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/developer-features.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    19254 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/do-it-yourself-framework.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.940863 Paste-3.8.0/docs/download/
+-rw-r--r--   0 cdent      (503) staff       (20)     1383 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/download/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     3184 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/future.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.941431 Paste-3.8.0/docs/include/
+-rw-r--r--   0 cdent      (503) staff       (20)      338 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/include/contact.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       66 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/include/reference_header.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1985 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1077 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/license.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.961550 Paste-3.8.0/docs/modules/
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.auth_tkt.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.basic.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.cas.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      314 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.cookie.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      297 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.digest.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      242 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.form.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.grantip.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      238 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/auth.multi.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      273 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cascade.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      281 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cgiapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/cgitb_catcher.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      280 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.debugapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      354 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.fsdiff.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      207 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.prints.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      312 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.profile.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      325 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.watchthreads.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/debug.wdg_validate.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      288 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/errordocument.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/evalexception.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1259 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/exceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      248 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/fileapp.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      633 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/fixture.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      226 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/gzipper.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1604 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpexceptions.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      216 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpheaders.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      202 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/httpserver.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      272 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/lint.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/pony.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      246 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/progress.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      306 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/proxy.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      232 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/recursive.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      372 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/registry.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      293 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/reloader.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      501 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/request.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      353 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/response.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      243 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/session.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      284 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/transaction.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/translogger.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      185 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/url.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      224 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/urlmap.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      392 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/urlparser.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      332 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/util.import_string.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      260 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/util.multidict.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      520 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/wsgilib.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      279 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/modules/wsgiwrappers.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    41287 2024-03-16 14:42:52.000000 Paste-3.8.0/docs/news.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     6405 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/paste-httpserver-threadpool.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      933 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/test_server.ini
+-rw-r--r--   0 cdent      (503) staff       (20)     5073 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/testing-applications.txt
+-rw-r--r--   0 cdent      (503) staff       (20)    12875 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/url-parsing-with-wsgi.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.962515 Paste-3.8.0/docs/web/
+-rw-r--r--   0 cdent      (503) staff       (20)     5756 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/default-site.css
+-rw-r--r--   0 cdent      (503) staff       (20)     1653 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/site.js
+-rw-r--r--   0 cdent      (503) staff       (20)     1241 2020-01-26 15:30:37.000000 Paste-3.8.0/docs/web/style.css
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.972219 Paste-3.8.0/paste/
+-rw-r--r--   0 cdent      (503) staff       (20)      551 2023-10-15 13:05:17.000000 Paste-3.8.0/paste/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.975432 Paste-3.8.0/paste/auth/
+-rw-r--r--   0 cdent      (503) staff       (20)      444 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16187 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4213 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/basic.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3996 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/cas.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16273 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9272 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5444 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/form.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3989 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3042 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/auth/multi.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16244 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/auth/open_id.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4474 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cascade.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9688 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3803 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4312 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/config.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.977026 Paste-3.8.0/paste/cowbell/
+-rw-r--r--   0 cdent      (503) staff       (20)     3727 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)   132993 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/bell-ascending.png
+-rw-r--r--   0 cdent      (503) staff       (20)   124917 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/cowbell/bell-descending.png
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.979998 Paste-3.8.0/paste/debug/
+-rw-r--r--   0 cdent      (503) staff       (20)      221 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/__init__.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2855 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/debugapp.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    14916 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/doctest_webapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12902 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/debug/fsdiff.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5444 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/prints.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7553 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/profile.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     3395 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/testserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10832 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/watchthreads.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4261 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/debug/wdg_validate.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13855 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.980806 Paste-3.8.0/paste/evalexception/
+-rw-r--r--   0 cdent      (503) staff       (20)      282 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2111 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/evalexception/evalcontext.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.982667 Paste-3.8.0/paste/evalexception/media/
+-rw-r--r--   0 cdent      (503) staff       (20)   202262 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/MochiKit.packed.js
+-rw-r--r--   0 cdent      (503) staff       (20)     4257 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/debug.js
+-rw-r--r--   0 cdent      (503) staff       (20)      359 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/minus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)      361 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/evalexception/media/plus.jpg
+-rw-r--r--   0 cdent      (503) staff       (20)    22142 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/evalexception/middleware.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.984450 Paste-3.8.0/paste/exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)      252 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19661 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/collector.py
+-rw-r--r--   0 cdent      (503) staff       (20)    16954 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/errormiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19464 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4565 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4069 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/exceptions/serial_number_generator.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13698 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)    59245 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3923 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/flup_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3818 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)    24244 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)    43120 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpheaders.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)    57052 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14920 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/lint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7783 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/modpython.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2279 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/pony.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)     8162 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/progress.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9200 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14605 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22250 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6000 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/reloader.py
+-rw-r--r--   0 cdent      (503) staff       (20)    13883 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7659 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/response.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11396 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4363 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/transaction.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5159 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/translogger.py
+-rw-r--r--   0 cdent      (503) staff       (20)    14440 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/url.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9248 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)    26451 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:50.991961 Paste-3.8.0/paste/util/
+-rw-r--r--   0 cdent      (503) staff       (20)    83603 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/PySourceColor.py
+-rw-r--r--   0 cdent      (503) staff       (20)       86 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1849 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/classinit.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1361 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/classinstance.py
+-rw-r--r--   0 cdent      (503) staff       (20)      861 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/converters.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2412 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/dateinterval.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10796 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1427 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/filemixin.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3808 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/finddata.py
+-rw-r--r--   0 cdent      (503) staff       (20)      782 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/findpackage.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3114 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)    19071 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/intset.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9267 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/ip4.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1197 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/killthread.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3988 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/looper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6604 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12405 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2011 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5565 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/scgiserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)    23670 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/util/template.py
+-rw-r--r--   0 cdent      (503) staff       (20)     8175 2022-06-22 10:14:29.000000 Paste-3.8.0/paste/util/threadedprint.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1484 2020-01-26 15:30:37.000000 Paste-3.8.0/paste/util/threadinglocal.py
+-rw-r--r--   0 cdent      (503) staff       (20)    20260 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)    22173 2024-03-16 14:39:27.000000 Paste-3.8.0/paste/wsgiwrappers.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)      234 2020-01-26 15:30:37.000000 Paste-3.8.0/regen-docs
+-rw-r--r--   0 cdent      (503) staff       (20)      162 2024-03-16 14:50:51.022824 Paste-3.8.0/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)     4612 2024-03-16 14:43:51.000000 Paste-3.8.0/setup.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.001687 Paste-3.8.0/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      138 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.002833 Paste-3.8.0/tests/cgiapp_data/
+-rwxr-xr-x   0 cdent      (503) staff       (20)       41 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/cgiapp_data/error.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)     2000 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/cgiapp_data/form.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      132 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/cgiapp_data/ok.cgi
+-rwxr-xr-x   0 cdent      (503) staff       (20)      185 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/cgiapp_data/stderr.cgi
+-rw-r--r--   0 cdent      (503) staff       (20)     4132 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/template.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.004180 Paste-3.8.0/tests/test_auth/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_auth/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1465 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_cookie.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3026 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_digest.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3598 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_auth/test_auth_tkt.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2053 2020-10-12 12:27:11.000000 Paste-3.8.0/tests/test_cgiapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2157 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_cgitb_catcher.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2846 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_config.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1506 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_doctests.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3461 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_errordocument.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.005552 Paste-3.8.0/tests/test_exceptions/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3286 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_exceptions/test_error_middleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4985 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/test_formatter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4263 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_exceptions/test_httpexceptions.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1280 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_exceptions/test_reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9589 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_fileapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2489 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1240 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_grantip.py
+-rw-r--r--   0 cdent      (503) staff       (20)      886 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_gzipper.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6843 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_httpheaders.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3229 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_httpserver.py
+-rw-r--r--   0 cdent      (503) staff       (20)      477 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_import_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5116 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_multidict.py
+-rw-r--r--   0 cdent      (503) staff       (20)      721 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_profilemiddleware.py
+-rw-r--r--   0 cdent      (503) staff       (20)      624 2023-04-30 11:31:00.000000 Paste-3.8.0/tests/test_proxy.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4178 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_recursive.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11013 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_registry.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2323 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_request.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1463 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_request_form.py
+-rw-r--r--   0 cdent      (503) staff       (20)      369 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_response.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1548 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_session.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1786 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_urlmap.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6944 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_urlparser.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.006936 Paste-3.8.0/tests/test_util/
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_util/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6109 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_util/test_datetimeutil.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11873 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_util/test_mimeparse.py
+-rw-r--r--   0 cdent      (503) staff       (20)      997 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_util/test_quoting.py
+-rw-r--r--   0 cdent      (503) staff       (20)      842 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/test_wsgilib.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6380 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/test_wsgiwrappers.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.007724 Paste-3.8.0/tests/urlparser_data/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.008021 Paste-3.8.0/tests/urlparser_data/deep/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/deep/index.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.008348 Paste-3.8.0/tests/urlparser_data/deep/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/deep/sub/Main.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.009469 Paste-3.8.0/tests/urlparser_data/find_file/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.009896 Paste-3.8.0/tests/urlparser_data/find_file/dir with spaces/
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/dir with spaces/test 4.html
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/index.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        7 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/test 3.html
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/find_file/test2.html
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.011002 Paste-3.8.0/tests/urlparser_data/hook/
+-rw-r--r--   0 cdent      (503) staff       (20)      289 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/hook/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      200 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/hook/app.py
+-rw-r--r--   0 cdent      (503) staff       (20)      201 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/hook/index.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.011263 Paste-3.8.0/tests/urlparser_data/not_found/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/__init__.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.017973 Paste-3.8.0/tests/urlparser_data/not_found/recur/
+-rw-r--r--   0 cdent      (503) staff       (20)      374 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/recur/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/recur/isfound.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.018946 Paste-3.8.0/tests/urlparser_data/not_found/simple/
+-rw-r--r--   0 cdent      (503) staff       (20)      134 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/simple/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)        9 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/simple/found.txt
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.019567 Paste-3.8.0/tests/urlparser_data/not_found/user/
+-rw-r--r--   0 cdent      (503) staff       (20)      411 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/not_found/user/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      204 2024-03-16 14:39:27.000000 Paste-3.8.0/tests/urlparser_data/not_found/user/list.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.020483 Paste-3.8.0/tests/urlparser_data/python/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      183 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)      208 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/stream.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2024-03-16 14:50:51.021177 Paste-3.8.0/tests/urlparser_data/python/sub/
+-rw-r--r--   0 cdent      (503) staff       (20)        2 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/sub/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      186 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/python/sub/simpleapp.py
+-rw-r--r--   0 cdent      (503) staff       (20)        8 2020-01-26 15:30:37.000000 Paste-3.8.0/tests/urlparser_data/secured.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      365 2023-10-19 10:24:33.000000 Paste-3.8.0/tox.ini
```

### Comparing `Paste-3.7.1/PKG-INFO` & `Paste-3.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.7.1
+Version: 3.8.0
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/cdent/paste
 Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
@@ -21,26 +21,30 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Framework :: Paste
 Requires-Python: >=3
+Requires-Dist: setuptools
+Requires-Dist: six>=1.4.0
 Provides-Extra: subprocess
 Provides-Extra: hotshot
-Provides-Extra: Flup
-Provides-Extra: Paste
+Provides-Extra: flup
+Requires-Dist: flup; extra == "flup"
+Provides-Extra: paste
 Provides-Extra: openid
+Requires-Dist: python-openid; extra == "openid"
 
 
 *Paste is in maintenance mode and recently moved from bitbucket to github.
 Patches are accepted to keep it on life support, but for the most part, please
 consider using other options.*
 
-**As of release 3.7.0 Paste no longer tries to support Python 2. If you are
+**As of release 3.7.0 Paste no longer supports Python 2. If you are
 required to continue using Python 2 please pin an earlier version of Paste.**
 
 Paste provides several pieces of "middleware" (or filters) that can be nested
 to build web applications.  Each piece of middleware uses the WSGI (`PEP 333`_)
 interface, and should be compatible with other middleware based on those
 interfaces.
```

### Comparing `Paste-3.7.1/Paste.egg-info/PKG-INFO` & `Paste-3.8.0/Paste.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paste
-Version: 3.7.1
+Version: 3.8.0
 Summary: Tools for using a Web Server Gateway Interface stack
 Home-page: https://pythonpaste.readthedocs.io/
 Author: Chris Dent
 Author-email: chris.dent@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/cdent/paste
 Project-URL: Bug Tracker, https://github.com/cdent/paste/issues
@@ -21,26 +21,30 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Framework :: Paste
 Requires-Python: >=3
+Requires-Dist: setuptools
+Requires-Dist: six>=1.4.0
 Provides-Extra: subprocess
 Provides-Extra: hotshot
-Provides-Extra: Flup
-Provides-Extra: Paste
+Provides-Extra: flup
+Requires-Dist: flup; extra == "flup"
+Provides-Extra: paste
 Provides-Extra: openid
+Requires-Dist: python-openid; extra == "openid"
 
 
 *Paste is in maintenance mode and recently moved from bitbucket to github.
 Patches are accepted to keep it on life support, but for the most part, please
 consider using other options.*
 
-**As of release 3.7.0 Paste no longer tries to support Python 2. If you are
+**As of release 3.7.0 Paste no longer supports Python 2. If you are
 required to continue using Python 2 please pin an earlier version of Paste.**
 
 Paste provides several pieces of "middleware" (or filters) that can be nested
 to build web applications.  Each piece of middleware uses the WSGI (`PEP 333`_)
 interface, and should be compatible with other middleware based on those
 interfaces.
```

### Comparing `Paste-3.7.1/Paste.egg-info/SOURCES.txt` & `Paste-3.8.0/Paste.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,14 @@
 paste/util/classinstance.py
 paste/util/converters.py
 paste/util/dateinterval.py
 paste/util/datetimeutil.py
 paste/util/filemixin.py
 paste/util/finddata.py
 paste/util/findpackage.py
-paste/util/html.py
 paste/util/import_string.py
 paste/util/intset.py
 paste/util/ip4.py
 paste/util/killthread.py
 paste/util/looper.py
 paste/util/mimeparse.py
 paste/util/multidict.py
```

### Comparing `Paste-3.7.1/Paste.egg-info/entry_points.txt` & `Paste-3.8.0/Paste.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/README.rst` & `Paste-3.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 *Paste is in maintenance mode and recently moved from bitbucket to github.
 Patches are accepted to keep it on life support, but for the most part, please
 consider using other options.*
 
-**As of release 3.7.0 Paste no longer tries to support Python 2. If you are
+**As of release 3.7.0 Paste no longer supports Python 2. If you are
 required to continue using Python 2 please pin an earlier version of Paste.**
 
 Paste provides several pieces of "middleware" (or filters) that can be nested
 to build web applications.  Each piece of middleware uses the WSGI (`PEP 333`_)
 interface, and should be compatible with other middleware based on those
 interfaces.
```

### Comparing `Paste-3.7.1/docs/DeveloperGuidelines.txt` & `Paste-3.8.0/docs/DeveloperGuidelines.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/StyleGuide.txt` & `Paste-3.8.0/docs/StyleGuide.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/_static/default.css` & `Paste-3.8.0/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/community/index.txt` & `Paste-3.8.0/docs/community/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/community/mailing-list.txt` & `Paste-3.8.0/docs/community/mailing-list.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/conf.py` & `Paste-3.8.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 project = 'Paste'
 copyright = '2008, Ian Bicking'
 
 # The default replacements for |version| and |release|, also used in various
 # other places throughout the built documents.
 #
 # The short X.Y version.
-version = '3.0'
+version = ''
 # The full version, including alpha/beta/rc tags.
-release = '3.0.0'
+release = ''
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 today_fmt = '%B %d, %Y'
 
@@ -67,18 +67,15 @@
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 
 # Options for HTML output
 # -----------------------
 
-# The style sheet to use for HTML and HTML Help pages. A file of that name
-# must exist either in Sphinx' static/ path, or in one of the custom paths
-# given in html_static_path.
-html_style = 'default.css'
+html_theme = 'nature'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `Paste-3.7.1/docs/developer-features.txt` & `Paste-3.8.0/docs/developer-features.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/do-it-yourself-framework.txt` & `Paste-3.8.0/docs/do-it-yourself-framework.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/download/index.txt` & `Paste-3.8.0/docs/download/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/future.txt` & `Paste-3.8.0/docs/future.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/index.txt` & `Paste-3.8.0/docs/index.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/license.txt` & `Paste-3.8.0/docs/license.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/modules/exceptions.txt` & `Paste-3.8.0/docs/modules/exceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/modules/fixture.txt` & `Paste-3.8.0/docs/modules/fixture.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/modules/httpexceptions.txt` & `Paste-3.8.0/docs/modules/httpexceptions.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/modules/wsgilib.txt` & `Paste-3.8.0/docs/modules/wsgilib.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/news.txt` & `Paste-3.8.0/docs/news.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 News
 ====
 
 .. contents::
 
+3.8.0
+-----
+
+* Remove remainder of Python 2 code. Thanks a-detiste.
+
 3.7.0
 -----
 
 * End Python 2 support.
 * Remove use of distutils.
 * Fix double query processing in parse_formvars.
```

### Comparing `Paste-3.7.1/docs/paste-httpserver-threadpool.txt` & `Paste-3.8.0/docs/paste-httpserver-threadpool.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/test_server.ini` & `Paste-3.8.0/docs/test_server.ini`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/testing-applications.txt` & `Paste-3.8.0/docs/testing-applications.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/url-parsing-with-wsgi.txt` & `Paste-3.8.0/docs/url-parsing-with-wsgi.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/web/default-site.css` & `Paste-3.8.0/docs/web/default-site.css`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/web/site.js` & `Paste-3.8.0/docs/web/site.js`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/docs/web/style.css` & `Paste-3.8.0/docs/web/style.css`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/__init__.py` & `Paste-3.8.0/paste/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/auth/auth_tkt.py` & `Paste-3.8.0/paste/auth/auth_tkt.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,27 +39,20 @@
 import six
 import time as time_mod
 try:
     import hashlib
 except ImportError:
     # mimic hashlib (will work for md5, fail for secure hashes)
     import md5 as hashlib
-try:
-    from http.cookies import SimpleCookie
-except ImportError:
-    # Python 2
-    from Cookie import SimpleCookie
+from http.cookies import SimpleCookie
+from urllib.parse import quote as url_quote
+from urllib.parse import unquote as url_unquote
+
 from paste import request
 
-try:
-    from urllib import quote as url_quote # Python 2.X
-    from urllib import unquote as url_unquote
-except ImportError:
-    from urllib.parse import quote as url_quote  # Python 3+
-    from urllib.parse import unquote as url_unquote
 
 DEFAULT_DIGEST = hashlib.md5
 
 
 class AuthTicket(object):
 
     """
@@ -99,25 +92,25 @@
 
     def __init__(self, secret, userid, ip, tokens=(), user_data='',
                  time=None, cookie_name='auth_tkt',
                  secure=False, digest_algo=DEFAULT_DIGEST):
         self.secret = secret
         self.userid = userid
         self.ip = ip
-        if not isinstance(tokens, six.string_types):
+        if not isinstance(tokens, str):
             tokens = ','.join(tokens)
         self.tokens = tokens
         self.user_data = user_data
         if time is None:
             self.time = time_mod.time()
         else:
             self.time = time
         self.cookie_name = cookie_name
         self.secure = secure
-        if isinstance(digest_algo, six.binary_type):
+        if isinstance(digest_algo, bytes):
             # correct specification of digest from hashlib or fail
             self.digest_algo = getattr(hashlib, digest_algo)
         else:
             self.digest_algo = digest_algo
 
     def digest(self):
         return calculate_digest(
@@ -129,19 +122,16 @@
         if self.tokens:
             v += maybe_encode(self.tokens) + b'!'
         v += maybe_encode(self.user_data)
         return v
 
     def cookie(self):
         c = SimpleCookie()
-        if six.PY3:
-            import base64
-            cookie_value = base64.b64encode(self.cookie_value())
-        else:
-            cookie_value = self.cookie_value().encode('base64').strip().replace('\n', '')
+        import base64
+        cookie_value = base64.b64encode(self.cookie_value())
         c[self.cookie_name] = cookie_value
         c[self.cookie_name]['path'] = '/'
         if self.secure:
             c[self.cookie_name]['secure'] = 'true'
         return c
 
 
@@ -160,15 +150,15 @@
 def parse_ticket(secret, ticket, ip, digest_algo=DEFAULT_DIGEST):
     """
     Parse the ticket, returning (timestamp, userid, tokens, user_data).
 
     If the ticket cannot be parsed, ``BadTicket`` will be raised with
     an explanation.
     """
-    if isinstance(digest_algo, six.binary_type):
+    if isinstance(digest_algo, bytes):
         # correct specification of digest from hashlib or fail
         digest_algo = getattr(hashlib, digest_algo)
     digest_hexa_size = digest_algo().digest_size * 2
     ticket = ticket.strip(b'"')
     digest = ticket[:digest_hexa_size]
     try:
         timestamp = int(ticket[digest_hexa_size:digest_hexa_size + 8], 16)
@@ -221,15 +211,15 @@
           (t & 0xff00) >> 8,
           t & 0xff)
     ts_chars = b''.join(map(six.int2byte, ts))
     return (ip_chars + ts_chars)
 
 
 def maybe_encode(s, encoding='utf8'):
-    if isinstance(s, six.text_type):
+    if isinstance(s, str):
         s = s.encode(encoding)
     return s
 
 
 class AuthTKTMiddleware(object):
 
     """
@@ -355,15 +345,15 @@
         def cookie_setting_start_response(status, headers, exc_info=None):
             headers.extend(set_cookies)
             return start_response(status, headers, exc_info)
 
         return self.app(environ, cookie_setting_start_response)
 
     def set_user_cookie(self, environ, userid, tokens, user_data):
-        if not isinstance(tokens, six.string_types):
+        if not isinstance(tokens, str):
             tokens = ','.join(tokens)
         if self.include_ip:
             remote_addr = environ['REMOTE_ADDR']
         else:
             remote_addr = '0.0.0.0'
         ticket = AuthTicket(
             self.secret,
```

### Comparing `Paste-3.7.1/paste/auth/basic.py` & `Paste-3.8.0/paste/auth/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,24 @@
 ...     return username == password
 >>> serve(AuthBasicHandler(dump_environ, realm, authfunc))
 serving on...
 
 .. [1] http://www.w3.org/Protocols/HTTP/1.0/draft-ietf-http-spec.html#BasicAA
 """
 from base64 import b64decode
+
 import six
+
 from paste.httpexceptions import HTTPUnauthorized
-from paste.httpheaders import *
+from paste.httpheaders import (
+    AUTHORIZATION,
+    AUTH_TYPE,
+    REMOTE_USER,
+    WWW_AUTHENTICATE,
+)
 
 class AuthBasicAuthenticator(object):
     """
     implements ``Basic`` authentication details
     """
     type = 'basic'
     def __init__(self, realm, authfunc):
```

### Comparing `Paste-3.7.1/paste/auth/cas.py` & `Paste-3.8.0/paste/auth/cas.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     http://www.yale.edu/tp/auth/usingcasatyale.html
 
 This implementation has the goal of maintaining current path arguments
 passed to the system so that it can be used as middleware at any stage
 of processing.  It has the secondary goal of allowing for other
 authentication methods to be used concurrently.
 """
-from six.moves.urllib.parse import urlencode
+from urllib.parse import urlencode
 from paste.request import construct_url
 from paste.httpexceptions import HTTPSeeOther, HTTPForbidden
 
 class CASLoginFailure(HTTPForbidden):
     """ The exception raised if the authority returns 'no' """
 
 class CASAuthenticate(HTTPSeeOther):
```

### Comparing `Paste-3.7.1/paste/auth/cookie.py` & `Paste-3.8.0/paste/auth/cookie.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,15 @@
         self.content = content
         self.cookie = cookie
 
 _all_chars = ''.join([chr(x) for x in range(0, 255)])
 def new_secret():
     """ returns a 64 byte secret """
     secret = ''.join(random.sample(_all_chars, 64))
-    if six.PY3:
-        secret = secret.encode('utf8')
+    secret = secret.encode('utf8')
     return secret
 
 class AuthCookieSigner(object):
     """
     save/restore ``environ`` entries via digially signed cookie
 
     This class converts content into a timed and digitally signed
@@ -123,42 +122,35 @@
             raised so that unexpected handling of cookies on the client
             side are avoided.  By default this is set at 4k (4096 bytes),
             which is the standard cookie size limit.
 
     """
     def __init__(self, secret = None, timeout = None, maxlen = None):
         self.timeout = timeout or 30
-        if isinstance(timeout, six.string_types):
+        if isinstance(timeout, str):
             raise ValueError(
                 "Timeout must be a number (minutes), not a string (%r)"
                 % timeout)
         self.maxlen  = maxlen or 4096
         self.secret = secret or new_secret()
 
     def sign(self, content):
         """
         Sign the content returning a valid cookie (that does not
         need to be escaped and quoted).  The expiration of this
         cookie is handled server-side in the auth() function.
         """
         timestamp = make_time(time.time() + 60*self.timeout)
-        if six.PY3:
-            content = content.encode('utf8')
-            timestamp = timestamp.encode('utf8')
-
-        if six.PY3:
-            cookie = base64.encodebytes(
-                hmac.new(self.secret, content, sha1).digest() +
-                timestamp +
-                content)
-        else:
-            cookie = base64.encodestring(
-                hmac.new(self.secret, content, sha1).digest() +
-                timestamp +
-                content)
+        content = content.encode('utf8')
+        timestamp = timestamp.encode('utf8')
+
+        cookie = base64.encodebytes(
+            hmac.new(self.secret, content, sha1).digest() +
+            timestamp +
+            content)
         cookie = cookie.replace(b"/", b"_").replace(b"=", b"~")
         cookie = cookie.replace(b'\n', b'').replace(b'\r', b'')
         if len(cookie) > self.maxlen:
             raise CookieTooLarge(content, cookie)
         return cookie
 
     def auth(self, cookie):
@@ -308,16 +300,15 @@
                             "The value of the environmental variable %r "
                             "is not a str (only str is allowed; got %r)"
                             % (k, v))
                     content.append("%s=%s" % (encode(k), encode(v)))
             if content:
                 content = ";".join(content)
                 content = self.signer.sign(content)
-                if six.PY3:
-                    content = content.decode('utf8')
+                content = content.decode('utf8')
                 cookie = '%s=%s; Path=/;' % (self.cookie_name, content)
                 if 'https' == environ['wsgi.url_scheme']:
                     cookie += ' secure;'
                 response_headers.append(('Set-Cookie', cookie))
             return start_response(status, response_headers, exc_info)
         return self.application(environ, response_hook)
 
@@ -382,15 +373,15 @@
 
         ``maxlen``
 
             The maximum length of the cookie that is sent (default 4k,
             which is a typical browser maximum)
 
     """
-    if isinstance(scanlist, six.string_types):
+    if isinstance(scanlist, str):
         scanlist = scanlist.split()
     if secret is None and global_conf.get('secret'):
         secret = global_conf['secret']
     try:
         timeout = int(timeout)
     except ValueError:
         raise ValueError('Bad value for timeout (must be int): %r'
```

### Comparing `Paste-3.7.1/paste/auth/digest.py` & `Paste-3.8.0/paste/auth/digest.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,28 @@
 implementation does not provide for further challenges, nor does it
 support Authentication-Info header.  It also uses md5, and an option
 to use sha would be a good thing.
 
 .. [1] http://www.faqs.org/rfcs/rfc2617.html
 """
 from paste.httpexceptions import HTTPUnauthorized
-from paste.httpheaders import *
+from paste.httpheaders import (
+    AUTHORIZATION,
+    AUTH_TYPE,
+    PATH_INFO,
+    REMOTE_USER,
+    REQUEST_METHOD,
+    SCRIPT_NAME,
+)
 try:
     from hashlib import md5
 except ImportError:
     from md5 import md5
 import time, random
-from six.moves.urllib.parse import quote as url_quote
-import six
+from urllib.parse import quote as url_quote
 
 def _split_auth_string(auth_string):
     """ split a digest auth string into individual key=value strings """
     prev = None
     for item in auth_string.split(","):
         try:
             if prev.count('"') == 1:
@@ -65,35 +71,32 @@
         if v.startswith('"') and len(v) > 1 and v.endswith('"'):
             v = v[1:-1]
         yield (k, v)
 
 def digest_password(realm, username, password):
     """ construct the appropriate hashcode needed for HTTP digest """
     content = "%s:%s:%s" % (username, realm, password)
-    if six.PY3:
-        content = content.encode('utf8')
+    content = content.encode('utf8')
     return md5(content).hexdigest()
 
 class AuthDigestAuthenticator(object):
     """ implementation of RFC 2617 - HTTP Digest Authentication """
     def __init__(self, realm, authfunc):
         self.nonce    = {} # list to prevent replay attacks
         self.authfunc = authfunc
         self.realm    = realm
 
     def build_authentication(self, stale = ''):
         """ builds the authentication error """
         content = "%s:%s" % (time.time(), random.random())
-        if six.PY3:
-            content = content.encode('utf-8')
+        content = content.encode('utf-8')
         nonce  = md5(content).hexdigest()
 
         content = "%s:%s" % (time.time(), random.random())
-        if six.PY3:
-            content = content.encode('utf-8')
+        content = content.encode('utf-8')
         opaque = md5(content).hexdigest()
 
         self.nonce[nonce] = None
         parts = {'realm': self.realm, 'qop': 'auth',
                  'nonce': nonce, 'opaque': opaque }
         if stale:
             parts['stale'] = 'true'
@@ -103,23 +106,21 @@
 
     def compute(self, ha1, username, response, method,
                       path, nonce, nc, cnonce, qop):
         """ computes the authentication, raises error if unsuccessful """
         if not ha1:
             return self.build_authentication()
         content = '%s:%s' % (method, path)
-        if six.PY3:
-            content = content.encode('utf8')
+        content = content.encode('utf8')
         ha2 = md5(content).hexdigest()
         if qop:
             chk = "%s:%s:%s:%s:%s:%s" % (ha1, nonce, nc, cnonce, qop, ha2)
         else:
             chk = "%s:%s:%s" % (ha1, nonce, ha2)
-        if six.PY3:
-            chk = chk.encode('utf8')
+        chk = chk.encode('utf8')
         if response != md5(chk).hexdigest():
             if nonce in self.nonce:
                 del self.nonce[nonce]
             return self.build_authentication()
         pnc = self.nonce.get(nonce,'00000000')
         if pnc is not None and nc <= pnc:
             if nonce in self.nonce:
```

### Comparing `Paste-3.7.1/paste/auth/form.py` & `Paste-3.8.0/paste/auth/form.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/auth/grantip.py` & `Paste-3.8.0/paste/auth/grantip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Grant roles and logins based on IP address.
 """
-import six
 from paste.util import ip4
 
-class GrantIPMiddleware(object):
+class GrantIPMiddleware:
 
     """
     On each request, ``ip_map`` is checked against ``REMOTE_ADDR``
     and logins and roles are assigned based on that.
 
     ``ip_map`` is a map of {ip_mask: (username, roles)}.  Either
     ``username`` or ``roles`` may be None.  Roles may also be prefixed
@@ -31,15 +30,15 @@
         self.ip_map = []
         for key, value in ip_map.items():
             self.ip_map.append((ip4.IP4Range(key),
                                 self._convert_user_role(value[0], value[1])))
         self.clobber_username = clobber_username
 
     def _convert_user_role(self, username, roles):
-        if roles and isinstance(roles, six.string_types):
+        if roles and isinstance(roles, str):
             roles = roles.split(',')
         return (username, roles)
 
     def __call__(self, environ, start_response):
         addr = ip4.ip2int(environ['REMOTE_ADDR'], False)
         remove_user = False
         add_roles = []
```

### Comparing `Paste-3.7.1/paste/auth/multi.py` & `Paste-3.8.0/paste/auth/multi.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/auth/open_id.py` & `Paste-3.8.0/paste/auth/open_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 """
 
 __all__ = ['AuthOpenIDHandler']
 
 import cgi
 import urlparse
 import re
-import six
 
 import paste.request
 from paste import httpexceptions
 
 def quoteattr(s):
     qs = cgi.escape(s, 1)
     return '"%s"' % (qs,)
@@ -73,15 +72,15 @@
 # Python-OpenID.
 # sys.path.append('/path/to/openid/')
 
 from openid.store import filestore
 from openid.consumer import consumer
 from openid.oidutil import appendArgs
 
-class AuthOpenIDHandler(object):
+class AuthOpenIDHandler:
     """
     This middleware implements OpenID Consumer behavior to authenticate a
     URL against an OpenID Server.
     """
 
     def __init__(self, app, data_store_path, auth_prefix='/oid',
                  login_redirect=None, catch_401=False,
@@ -395,15 +394,15 @@
     catch_401=False,
     url_to_username=None,
     apply_auth_tkt=False,
     auth_tkt_logout_path=None):
     from paste.deploy.converters import asbool
     from paste.util import import_string
     catch_401 = asbool(catch_401)
-    if url_to_username and isinstance(url_to_username, six.string_types):
+    if url_to_username and isinstance(url_to_username, str):
         url_to_username = import_string.eval_import(url_to_username)
     apply_auth_tkt = asbool(apply_auth_tkt)
     new_app = AuthOpenIDHandler(
         app, data_store_path=data_store_path, auth_prefix=auth_prefix,
         login_redirect=login_redirect, catch_401=catch_401,
         url_to_username=url_to_username or None)
     if apply_auth_tkt:
```

### Comparing `Paste-3.7.1/paste/cascade.py` & `Paste-3.8.0/paste/cascade.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 Cascades through several applications, so long as applications
 return ``404 Not Found``.
 """
 from paste import httpexceptions
 from paste.util import converters
 import tempfile
-from six import BytesIO
+from io import BytesIO
 
 __all__ = ['Cascade']
 
 def make_cascade(loader, global_conf, catch='404', **local_conf):
     """
     Entry point for Paste Deploy configuration
```

### Comparing `Paste-3.7.1/paste/cgiapp.py` & `Paste-3.8.0/paste/cgiapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 Application that runs a CGI script.
 """
 import os
 import sys
 import subprocess
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 try:
     import select
 except ImportError:
     select = None
 import six
 
 from paste.util import converters
@@ -20,15 +20,15 @@
 
 class CGIError(Exception):
     """
     Raised when the CGI script can't be found or doesn't
     act like a proper CGI script.
     """
 
-class CGIApplication(object):
+class CGIApplication:
 
     """
     This object acts as a proxy to a CGI application.  You pass in the
     script path (``script``), an optional path to search for the
     script (if the name isn't absolute) (``path``).  If you don't give
     a path, then ``$PATH`` will be used.
     """
@@ -144,17 +144,16 @@
             elif b':' not in line1:
                 raise CGIError(
                     "Bad header line: %r" % line1)
             else:
                 name, value = line1.split(b':', 1)
                 value = value.lstrip()
                 name = name.strip()
-                if six.PY3:
-                    name = name.decode('utf8')
-                    value = value.decode('utf8')
+                name = name.decode('utf8')
+                value = value.decode('utf8')
                 if name.lower() == 'status':
                     if ' ' not in value:
                         # WSGI requires this space, sometimes CGI scripts don't set it:
                         value = '%s General' % value
                     self.status = value
                 else:
                     self.headers.append((name, value))
```

### Comparing `Paste-3.7.1/paste/cgitb_catcher.py` & `Paste-3.8.0/paste/cgitb_catcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 Captures any exceptions and prints a pretty report.  See the `cgitb
 documentation <http://python.org/doc/current/lib/module-cgitb.html>`_
 for more.
 """
 
 import cgitb
-import six
-from six.moves import cStringIO as StringIO
+from io import StringIO
 import sys
 
 from paste.util import converters
 
 class NoDefault(object):
     pass
 
@@ -28,15 +27,15 @@
                  context=5,
                  format="html"):
         self.app = app
         if global_conf is None:
             global_conf = {}
         if display is NoDefault:
             display = global_conf.get('debug')
-        if isinstance(display, six.string_types):
+        if isinstance(display, str):
             display = converters.asbool(display)
         self.display = display
         self.logdir = logdir
         self.context = int(context)
         self.format = format
 
     def __call__(self, environ, start_response):
@@ -45,16 +44,15 @@
             return self.catching_iter(app_iter, environ)
         except:
             exc_info = sys.exc_info()
             start_response('500 Internal Server Error',
                            [('content-type', 'text/html')],
                            exc_info)
             response = self.exception_handler(exc_info, environ)
-            if six.PY3:
-                response = response.encode('utf8')
+            response = response.encode('utf8')
             return [response]
 
     def catching_iter(self, app_iter, environ):
         if not app_iter:
             return
         error_on_close = False
         try:
@@ -70,16 +68,15 @@
                     app_iter.close()
                 except:
                     close_response = self.exception_handler(
                         sys.exc_info(), environ)
                     response += (
                         '<hr noshade>Error in .close():<br>%s'
                         % close_response)
-            if six.PY3:
-                response = response.encode('utf8')
+            response = response.encode('utf8')
             yield response
 
     def exception_handler(self, exc_info, environ):
         dummy_file = StringIO()
         hook = cgitb.Hook(file=dummy_file,
                           display=self.display,
                           logdir=self.logdir,
```

### Comparing `Paste-3.7.1/paste/config.py` & `Paste-3.8.0/paste/config.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/cowbell/__init__.py` & `Paste-3.8.0/paste/cowbell/__init__.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/cowbell/bell-ascending.png` & `Paste-3.8.0/paste/cowbell/bell-ascending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/cowbell/bell-descending.png` & `Paste-3.8.0/paste/cowbell/bell-descending.png`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/debug/debugapp.py` & `Paste-3.8.0/paste/debug/debugapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/debug/doctest_webapp.py` & `Paste-3.8.0/paste/debug/doctest_webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import doctest
 import os
 import sys
 import shutil
 import re
 import cgi
 import rfc822
-from cStringIO import StringIO
+from io import StringIO
 from paste.util import PySourceColor
 
 
 here = os.path.abspath(__file__)
 paste_parent = os.path.dirname(
     os.path.dirname(os.path.dirname(here)))
```

### Comparing `Paste-3.7.1/paste/debug/fsdiff.py` & `Paste-3.8.0/paste/debug/fsdiff.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/debug/prints.py` & `Paste-3.8.0/paste/debug/prints.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,36 +13,32 @@
 
 You might want to include ``style="white-space: normal"``, as all the
 whitespace will be quoted, and this allows the text to wrap if
 necessary.
 
 """
 
-from cStringIO import StringIO
+from io import StringIO
 import re
 import cgi
 from paste.util import threadedprint
 from paste import wsgilib
 from paste import response
-import six
 import sys
 
 _threadedprint_installed = False
 
 __all__ = ['PrintDebugMiddleware']
 
 class TeeFile(object):
 
     def __init__(self, files):
         self.files = files
 
     def write(self, v):
-        if isinstance(v, unicode):
-            # WSGI is picky in this case
-            v = str(v)
         for file in self.files:
             file.write(v)
 
 class PrintDebugMiddleware(object):
 
     """
     This middleware captures all the printed statements, and inlines
@@ -68,15 +64,15 @@
 
     def __init__(self, app, global_conf=None, force_content_type=False,
                  print_wsgi_errors=True, replace_stdout=False):
         # @@: global_conf should be handled separately and only for
         # the entry point
         self.app = app
         self.force_content_type = force_content_type
-        if isinstance(print_wsgi_errors, six.string_types):
+        if isinstance(print_wsgi_errors, str):
             from paste.deploy.converters import asbool
             print_wsgi_errors = asbool(print_wsgi_errors)
         self.print_wsgi_errors = print_wsgi_errors
         self.replace_stdout = replace_stdout
         self._threaded_print_stdout = None
 
     def __call__(self, environ, start_response):
```

### Comparing `Paste-3.7.1/paste/debug/profile.py` & `Paste-3.8.0/paste/debug/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 import sys
 import os
 import hotshot
 import hotshot.stats
 import threading
 import cgi
-import six
 import time
-from cStringIO import StringIO
+from io import StringIO
 from paste import response
 
 __all__ = ['ProfileMiddleware', 'profile_decorator']
 
 class ProfileMiddleware(object):
 
     """
@@ -197,15 +196,15 @@
                 % (end_time - start_time))
         f.write(output)
         f.write(output_callers)
         if output_file not in (None, '-', 'stdout', 'stderr'):
             f.close()
         if exc_info:
             # We captured an exception earlier, now we re-raise it
-            six.reraise(exc_info[0], exc_info[1], exc_info[2])
+            raise exc_info
         return result
 
     def format_function(self, func, *args, **kw):
         args = map(repr, args)
         args.extend(
             ['%s=%r' % (k, v) for k, v in kw.items()])
         return '%s(%s)' % (func.__name__, ', '.join(args))
```

### Comparing `Paste-3.7.1/paste/debug/testserver.py` & `Paste-3.8.0/paste/debug/testserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 This builds upon paste.util.baseserver to customize it for regressions
 where using raw_interactive won't do.
 
 
 """
 import time
-from paste.httpserver import *
+from paste.httpserver import WSGIServer
 
 class WSGIRegressionServer(WSGIServer):
     """
     A threaded WSGIServer for use in regression testing.  To use this
     module, call serve(application, regression=True), and then call
     server.accept() to let it handle one request.  When finished, use
     server.stop() to shutdown the server. Note that all pending requests
@@ -63,15 +63,15 @@
 def serve(application, host=None, port=None, handler=None):
     server = WSGIRegressionServer(application, host, port, handler)
     print("serving on %s:%s" % server.server_address)
     server.serve_forever()
     return server
 
 if __name__ == '__main__':
-    from six.moves.urllib.request import urlopen
+    from urllib.request import urlopen
     from paste.wsgilib import dump_environ
     server = serve(dump_environ)
     baseuri = ("http://%s:%s" % server.server_address)
 
     def fetch(path):
         # tell the server to humor exactly one more request
         server.accept(1)
```

### Comparing `Paste-3.7.1/paste/debug/watchthreads.py` & `Paste-3.8.0/paste/debug/watchthreads.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Watches the key ``paste.httpserver.thread_pool`` to see how many
 threads there are and report on any wedged threads.
 """
 import sys
 import cgi
 import time
 import traceback
-from cStringIO import StringIO
+from io import StringIO
 from thread import get_ident
 from paste import httpexceptions
 from paste.request import construct_url, parse_formvars
 from paste.util.template import HTMLTemplate, bunch
 
 page_template = HTMLTemplate('''
 <html>
```

### Comparing `Paste-3.7.1/paste/debug/wdg_validate.py` & `Paste-3.8.0/paste/debug/wdg_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Middleware that tests the validity of all generated HTML using the
 `WDG HTML Validator <http://www.htmlhelp.com/tools/validator/>`_
 """
 
-from cStringIO import StringIO
+from io import StringIO
 import subprocess
 from paste.response import header_value
 import re
 import cgi
 
 __all__ = ['WDGValidateMiddleware']
```

### Comparing `Paste-3.7.1/paste/errordocument.py` & `Paste-3.8.0/paste/errordocument.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 The middleware in this module can be used to intercept responses with
 specified status codes and internally forward the request to an appropriate
 URL where the content can be displayed to the user as an error document.
 """
 
 import warnings
 import sys
-from six.moves.urllib import parse as urlparse
+from urllib import parse as urlparse
 from paste.recursive import ForwardRequestException, RecursiveMiddleware, RecursionLoop
 from paste.util import converters
 from paste.response import replace_header
-import six
 
 def forward(app, codes):
     """
     Intercepts a response with a particular status code and returns the
     content from a specified URL instead.
 
     The arguments are:
@@ -87,16 +86,15 @@
             return self.app(environ, keep_status_start_response)
         except RecursionLoop as e:
             line = 'Recursion error getting error page: %s\n' % e
             environ['wsgi.errors'].write(line)
             keep_status_start_response('500 Server Error', [('Content-type', 'text/plain')], sys.exc_info())
             body = ('Error: %s.  (Error page could not be fetched)'
                     % self.status)
-            if six.PY3:
-                body = body.encode('utf8')
+            body = body.encode('utf8')
             return [body]
 
 
 class StatusBasedForward(object):
     """
     Middleware that lets you test a response against a custom mapper object to
     programatically determine whether to internally forward to another URL and
```

### Comparing `Paste-3.7.1/paste/evalexception/evalcontext.py` & `Paste-3.8.0/paste/evalexception/evalcontext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
-from six.moves import cStringIO as StringIO
+from io import StringIO
 import traceback
 import threading
 import pdb
-import six
 import sys
 
 exec_lock = threading.Lock()
 
-class EvalContext(object):
+class EvalContext:
 
     """
     Class that represents a interactive interface.  It has its own
     namespace.  Use eval_context.exec_expr(expr) to run commands; the
     output of those commands is returned, as are print statements.
 
     This is essentially what doctest does, and is taken directly from
@@ -31,15 +30,15 @@
         try:
             debugger = _OutputRedirectingPdb(save_stdout)
             debugger.reset()
             pdb.set_trace = debugger.set_trace
             sys.stdout = out
             try:
                 code = compile(s, '<web>', "single", 0, 1)
-                six.exec_(code, self.globs, self.namespace)
+                exec(code, self.globs, self.namespace)
                 debugger.set_continue()
             except KeyboardInterrupt:
                 raise
             except:
                 traceback.print_exc(file=out)
                 debugger.set_continue()
         finally:
```

### Comparing `Paste-3.7.1/paste/evalexception/media/MochiKit.packed.js` & `Paste-3.8.0/paste/evalexception/media/MochiKit.packed.js`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/evalexception/media/debug.js` & `Paste-3.8.0/paste/evalexception/media/debug.js`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/evalexception/middleware.py` & `Paste-3.8.0/paste/evalexception/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,31 @@
 given then it will make the response more compact (and less
 Javascripty), since if you use innerHTML it'll kill your browser.  You
 can look for the header X-Debug-URL in your 500 responses if you want
 to see the full debuggable traceback.  Also, this URL is printed to
 ``wsgi.errors``, so you can open it up in another browser window.
 """
 
-from __future__ import print_function
-
+import html
 import sys
 import os
 import traceback
-import six
-from six.moves import cStringIO as StringIO
+from io import StringIO
 import pprint
 import itertools
 import time
 import re
 from paste.exceptions import errormiddleware, formatter, collector
 from paste import wsgilib
 from paste import urlparser
 from paste import httpexceptions
 from paste import registry
 from paste import request
 from paste import response
 from paste.evalexception import evalcontext
-from paste.util import html
 
 limit = 200
 
 def html_quote(v):
     """
     Escape HTML characters, plus translate None to ''
     """
@@ -159,16 +156,16 @@
 def get_debug_count(environ):
     """
     Return the unique debug count for the current request
     """
     if 'paste.evalexception.debug_count' in environ:
         return environ['paste.evalexception.debug_count']
     else:
-        environ['paste.evalexception.debug_count'] = next = six.next(debug_counter)
-        return next
+        environ['paste.evalexception.debug_count'] = _next = next(debug_counter)
+        return _next
 
 class EvalException(object):
 
     def __init__(self, application, global_conf=None,
                  xmlhttp_key=None):
         self.application = application
         self.debug_infos = {}
@@ -414,16 +411,15 @@
         head_html = (formatter.error_css + formatter.hide_display_js)
         head_html += self.eval_javascript()
         repost_button = make_repost_button(self.environ)
         page = error_template % {
             'repost_button': repost_button or '',
             'head_html': head_html,
             'body': html}
-        if six.PY3:
-            page = page.encode('utf8')
+        page = page.encode('utf8')
         return [page]
 
     def eval_javascript(self):
         base_path = self.base_path + '/_debug'
         return (
             '<script type="text/javascript" src="%s/media/MochiKit.packed.js">'
             '</script>\n'
```

### Comparing `Paste-3.7.1/paste/exceptions/collector.py` & `Paste-3.8.0/paste/exceptions/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 An exception collector that finds traceback information plus
 supplements
 """
 
 import sys
 import traceback
 import time
-from six.moves import cStringIO as StringIO
+from io import StringIO
 import linecache
 from paste.exceptions import serial_number_generator
 import warnings
 
 DEBUG_EXCEPTION_FORMATTER = True
 DEBUG_IDENT_PREFIX = 'E-'
 FALLBACK_ENCODING = 'UTF-8'
```

### Comparing `Paste-3.7.1/paste/exceptions/errormiddleware.py` & `Paste-3.8.0/paste/exceptions/errormiddleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 """
 Error handler middleware
 """
 import sys
 import traceback
 import cgi
-from six.moves import cStringIO as StringIO
+from io import StringIO
 from paste.exceptions import formatter, collector, reporter
 from paste import wsgilib
 from paste import request
-import six
 
 __all__ = ['ErrorMiddleware', 'handle_exception']
 
 class _NoDefault(object):
     def __repr__(self):
         return '<NoDefault>'
 NoDefault = _NoDefault()
@@ -148,16 +147,15 @@
                     if isinstance(exc_info[1], expect):
                         raise
                 start_response('500 Internal Server Error',
                                [('content-type', 'text/html')],
                                exc_info)
                 # @@: it would be nice to deal with bad content types here
                 response = self.exception_handler(exc_info, environ)
-                if six.PY3:
-                    response = response.encode('utf8')
+                response = response.encode('utf8')
                 return [response]
             finally:
                 # clean up locals...
                 exc_info = None
 
     def make_catching_iter(self, app_iter, environ, sr_checker):
         if isinstance(app_iter, (list, tuple)):
@@ -241,16 +239,15 @@
                     % close_response)
 
             if not self.start_checker.response_started:
                 self.start_checker('500 Internal Server Error',
                                [('content-type', 'text/html')],
                                exc_info)
 
-            if six.PY3:
-                response = response.encode('utf8')
+            response = response.encode('utf8')
             return response
     __next__ = next
 
     def close(self):
         # This should at least print something to stderr if the
         # close method fails at this point
         if not self.closed:
```

### Comparing `Paste-3.7.1/paste/exceptions/formatter.py` & `Paste-3.8.0/paste/exceptions/formatter.py`

 * *Files identical despite different names*

```diff
@@ -3,17 +3,16 @@
 
 """
 Formatters for the exception data that comes from ExceptionCollector.
 """
 # @@: TODO:
 # Use this: http://www.zope.org/Members/tino/VisualTraceback/VisualTracebackNews
 
-import six
 import re
-from paste.util import html
+import html
 from paste.util import PySourceColor
 
 def html_quote(s):
     return html.escape(str(s), True)
 
 class AbstractFormatter(object):
 
@@ -73,15 +72,15 @@
             lines.append(self.format_source_line(filename or '?', frame))
             source = frame.get_source_line()
             long_source = frame.get_source_line(2)
             if source:
                 lines.append(self.format_long_source(
                     source, long_source))
         etype = exc_data.exception_type
-        if not isinstance(etype, six.string_types):
+        if not isinstance(etype, str):
             etype = etype.__name__
         exc_info = self.format_exception_info(
             etype,
             exc_data.exception_value)
         data_by_importance = {'important': [], 'normal': [],
                               'supplemental': [], 'extra': []}
         for (importance, name), value in general_data.items():
```

### Comparing `Paste-3.7.1/paste/exceptions/reporter.py` & `Paste-3.8.0/paste/exceptions/reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             pass
 
     def check_params(self):
         if not self.to_addresses:
             raise ValueError("You must set to_addresses")
         if not self.from_address:
             raise ValueError("You must set from_address")
-        if isinstance(self.to_addresses, (str, unicode)):
+        if isinstance(self.to_addresses, str):
             self.to_addresses = [self.to_addresses]
 
     def assemble_email(self, exc_data):
         short_html_version = self.format_html(
             exc_data, show_hidden_frames=False)
         long_html_version = self.format_html(
             exc_data, show_hidden_frames=True)
```

### Comparing `Paste-3.7.1/paste/exceptions/serial_number_generator.py` & `Paste-3.8.0/paste/exceptions/serial_number_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 base = len(good_characters)
 
 def make_identifier(number):
     """
     Encodes a number as an identifier.
     """
-    if not isinstance(number, six.integer_types):
+    if not isinstance(number, int):
         raise ValueError(
             "You can only make identifiers out of integers (not %r)"
             % number)
     if number < 0:
         raise ValueError(
             "You cannot make identifiers out of negative numbers: %r"
             % number)
@@ -57,20 +57,19 @@
     if not callable(hasher):
         # Accept sha/md5 modules as well as callables
         hasher = hasher.new
     if length > 26 and hasher is md5:
         raise ValueError(
             "md5 cannot create hashes longer than 26 characters in "
             "length (you gave %s)" % length)
-    if isinstance(s, six.text_type):
+    if isinstance(s, str):
         s = s.encode('utf-8')
-    elif not isinstance(s, six.binary_type):
+    elif not isinstance(s, bytes):
         s = str(s)
-        if six.PY3:
-            s = s.encode('utf-8')
+        s = s.encode('utf-8')
     h = hasher(s)
     bin_hash = h.digest()
     modulo = base ** length
     number = 0
     for c in list(bin_hash):
         number = (number * 256 + six.byte2int([c])) % modulo
     ident = make_identifier(number)
```

### Comparing `Paste-3.7.1/paste/fileapp.py` & `Paste-3.8.0/paste/fileapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/fixture.py` & `Paste-3.8.0/paste/fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 
 Most interesting is the `TestApp <class-paste.fixture.TestApp.html>`_
 for testing WSGI applications, and the `TestFileEnvironment
 <class-paste.fixture.TestFileEnvironment.html>`_ class for testing the
 effects of command-line scripts.
 """
 
-from __future__ import print_function
-
 import sys
+import io
 import random
 import mimetypes
 import time
 import os
 import shutil
 import smtplib
 import shlex
 import re
-import six
 import subprocess
-from six.moves import cStringIO as StringIO
-from six.moves.urllib.parse import urlencode
-from six.moves.urllib import parse as urlparse
+from urllib.parse import urlencode
+from urllib import parse as urlparse
 from six.moves.http_cookies import BaseCookie
+import six
 
 from paste import wsgilib
 from paste import lint
 from paste.response import HeaderDict
 
 def tempnam_no_warning(*args):
     """
@@ -118,15 +116,15 @@
         ``pre_request_hook`` is a function to be called prior to
         making requests (such as ``post`` or ``get``). This function
         must take one argument (the instance of the TestApp).
 
         ``post_request_hook`` is a function, similar to
         ``pre_request_hook``, to be called after requests are made.
         """
-        if isinstance(app, (six.binary_type, six.text_type)):
+        if isinstance(app, (bytes, str)):
             from paste.deploy import loadapp
             # @@: Should pick up relative_to from calling module's
             # __file__
             app = loadapp(app, relative_to=relative_to)
         self.app = app
         self.namespace = namespace
         self.relative_to = relative_to
@@ -181,15 +179,15 @@
         Returns a `response object
         <class-paste.fixture.TestResponse.html>`_
         """
         if extra_environ is None:
             extra_environ = {}
         __tracebackhide__ = True  # Hide from pytest:
         if params:
-            if not isinstance(params, (six.binary_type, six.text_type)):
+            if not isinstance(params, (bytes, str)):
                 params = urlencode(params, doseq=True)
             if '?' in url:
                 url += '&'
             else:
                 url += '?'
             url += params
         environ = self._make_environ()
@@ -215,15 +213,15 @@
         environ = self._make_environ()
         # @@: Should this be all non-strings?
         if isinstance(params, (list, tuple, dict)):
             params = urlencode(params)
         if hasattr(params, 'items'):
             # Some other multi-dict like format
             params = urlencode(params.items())
-        if six.PY3 and isinstance(params, six.text_type):
+        if isinstance(params, str):
             params = params.encode('utf8')
         if upload_files:
             params = urlparse.parse_qsl(params, keep_blank_values=True)
             content_type, params = self.encode_multipart(
                 params, upload_files)
             environ['CONTENT_TYPE'] = content_type
         elif params:
@@ -231,15 +229,15 @@
         url = str(url)
         if '?' in url:
             url, environ['QUERY_STRING'] = url.split('?', 1)
         else:
             environ['QUERY_STRING'] = ''
         environ['CONTENT_LENGTH'] = str(len(params))
         environ['REQUEST_METHOD'] = method
-        environ['wsgi.input'] = six.BytesIO(params)
+        environ['wsgi.input'] = io.BytesIO(params)
         self._set_headers(headers, environ)
         environ.update(extra_environ)
         req = TestRequest(url, environ, expect_errors)
         return self.do_request(req, status=status)
 
     def post(self, url, params=b'', headers=None, extra_environ=None,
              status=None, upload_files=None, expect_errors=False):
@@ -326,16 +324,15 @@
         """
         Encodes a set of parameters (typically a name/value list) and
         a set of files (a list of (name, filename, file_body)) into a
         typical POST body, returning the (content_type, body).
         """
         boundary = '----------a_BoUnDaRy%s$' % random.random()
         content_type = 'multipart/form-data; boundary=%s' % boundary
-        if six.PY3:
-            boundary = boundary.encode('ascii')
+        boundary = boundary.encode('ascii')
 
         lines = []
         for key, value in params:
             lines.append(b'--'+boundary)
             line = b'Content-Disposition: form-data; name="%s"' % six.ensure_binary(key)
             lines.append(line)
             lines.append(b'')
@@ -448,16 +445,15 @@
                     % (res.full_status, ', '.join(map(str, status)),
                        res.request.url, res.body))
             return
         if status is None:
             if res.status >= 200 and res.status < 400:
                 return
             body = res.body
-            if six.PY3:
-                body = body.decode('utf8', 'xmlcharrefreplace')
+            body = body.decode('utf8', 'xmlcharrefreplace')
             raise AppError(
                 "Bad response: %s (not 200 OK or 3xx redirect for %s)\n%s"
                 % (res.full_status, res.request.url,
                    body))
         if status != res.status:
             raise AppError(
                 "Bad response: %s (not %s)" % (res.full_status, status))
@@ -471,15 +467,15 @@
         status, headers, body, errors = resp
         return TestResponse(self, status, headers, body, errors,
                             total_time)
 
 class CaptureStdout(object):
 
     def __init__(self, actual):
-        self.captured = StringIO()
+        self.captured = io.StringIO()
         self.actual = actual
 
     def write(self, s):
         self.captured.write(s)
         self.actual.write(s)
 
     def flush(self):
@@ -552,16 +548,15 @@
     _tag_re = re.compile(r'<(/?)([:a-z0-9_\-]*)(.*?)>', re.S|re.I)
 
     def _parse_forms(self):
         forms = self._forms_indexed = {}
         form_texts = []
         started = None
         body = self.body
-        if not six.PY2:
-            body = body.decode('utf8', 'xmlcharrefreplace')
+        body = body.decode('utf8', 'xmlcharrefreplace')
         for match in self._tag_re.finditer(body):
             end = match.group(1) == '/'
             tag = match.group(2).lower()
             if tag != 'form':
                 continue
             if end:
                 assert started, (
@@ -809,17 +804,17 @@
 
     def __contains__(self, s):
         """
         A response 'contains' a string if it is present in the body
         of the response.  Whitespace is normalized when searching
         for a string.
         """
-        if not isinstance(s, (six.binary_type, six.text_type)):
+        if not isinstance(s, (bytes, str)):
             s = str(s)
-        if isinstance(s, six.text_type):
+        if isinstance(s, str):
             ## FIXME: we don't know that this response uses utf8:
             s = s.encode('utf8')
         return (self.body.find(s) != -1
                 or self.normal_body.find(s) != -1)
 
     def mustcontain(self, *strings, **kw):
         """
@@ -829,15 +824,15 @@
         Equivalent to::
 
             assert string in res
         """
         if 'no' in kw:
             no = kw['no']
             del kw['no']
-            if isinstance(no, (six.binary_type, six.text_type)):
+            if isinstance(no, (bytes, str)):
                 no = [no]
         else:
             no = []
         if kw:
             raise TypeError(
                 "The only keyword argument allowed is 'no'")
         for s in strings:
@@ -851,24 +846,22 @@
                 print("Actual response (has %r)" % no_s, file=sys.stderr)
                 print(self, file=sys.stderr)
                 raise IndexError(
                     "Body contains string %r" % no_s)
 
     def __repr__(self):
         body = self.body
-        if six.PY3:
-            body = body.decode('utf8', 'xmlcharrefreplace')
+        body = body.decode('utf8', 'xmlcharrefreplace')
         body = body[:20]
         return '<Response %s %r>' % (self.full_status, body)
 
     def __str__(self):
         simple_body = b'\n'.join([l for l in self.body.splitlines()
                                  if l.strip()])
-        if six.PY3:
-            simple_body = simple_body.decode('utf8', 'xmlcharrefreplace')
+        simple_body = simple_body.decode('utf8', 'xmlcharrefreplace')
         return 'Response: %s\n%s\n%s' % (
             self.status,
             '\n'.join(['%s: %s' % (n, v) for n, v in self.headers]),
             simple_body)
 
     def showbrowser(self):
         """
@@ -1709,15 +1702,15 @@
             return ''.join(padding) + sep.join(full)
     else:
         return sep.join(full)
 
 def _make_pattern(pat):
     if pat is None:
         return None
-    if isinstance(pat, (six.binary_type, six.text_type)):
+    if isinstance(pat, (bytes, str)):
         pat = re.compile(pat)
     if hasattr(pat, 'search'):
         return pat.search
     if callable(pat):
         return pat
     assert 0, (
         "Cannot make callable pattern object out of %r" % pat)
@@ -1736,15 +1729,15 @@
     import warnings
     warnings.warn(
         'setup_module is deprecated',
         DeprecationWarning, 2)
     if module is None:
         # The module we were called from must be the module...
         module = sys._getframe().f_back.f_globals['__name__']
-    if isinstance(module, (six.binary_type, six.text_type)):
+    if isinstance(module, (bytes, str)):
         module = sys.modules[module]
     if hasattr(module, 'reset_state'):
         module.reset_state()
 
 def html_unquote(v):
     """
     Unquote (some) entities in HTML.  (incomplete)
```

### Comparing `Paste-3.7.1/paste/flup_session.py` & `Paste-3.8.0/paste/flup_session.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/gzipper.py` & `Paste-3.8.0/paste/gzipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 """
 WSGI middleware
 
 Gzip-encodes the response.
 """
 
 import gzip
+import io
+
 from paste.response import header_value, remove_header
 from paste.httpheaders import CONTENT_LENGTH
-import six
 
 class GzipOutput(object):
     pass
 
 class middleware(object):
 
     def __init__(self, application, compress_level=6):
@@ -41,15 +42,15 @@
         return response.write()
 
 class GzipResponse(object):
 
     def __init__(self, start_response, compress_level):
         self.start_response = start_response
         self.compress_level = compress_level
-        self.buffer = six.BytesIO()
+        self.buffer = io.BytesIO()
         self.compressible = False
         self.content_length = None
 
     def gzip_start_response(self, status, headers, exc_info=None):
         self.headers = headers
         ct = header_value(headers,'content-type')
         ce = header_value(headers,'content-encoding')
```

### Comparing `Paste-3.7.1/paste/httpexceptions.py` & `Paste-3.8.0/paste/httpexceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 References:
 
 .. [1] http://www.python.org/peps/pep-0333.html#error-handling
 .. [2] http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html#sec10.5
 
 """
 
-import six
 from paste.wsgilib import catch_errors_app
 from paste.response import has_header, header_value, replace_header
 from paste.request import resolve_relative_url
 from paste.util.quoting import strip_html, html_quote, no_quote, comment_quote
 
 SERVER_NAME = 'WSGI Server'
 TEMPLATE = """\
@@ -174,17 +173,17 @@
     required_headers = ()
 
     def __init__(self, detail=None, headers=None, comment=None):
         assert self.code, "Do not directly instantiate abstract exceptions."
         assert isinstance(headers, (type(None), list)), (
             "headers must be None or a list: %r"
             % headers)
-        assert isinstance(detail, (type(None), six.binary_type, six.text_type)), (
+        assert isinstance(detail, (type(None), bytes, str)), (
             "detail must be None or a string: %r" % detail)
-        assert isinstance(comment, (type(None), six.binary_type, six.text_type)), (
+        assert isinstance(comment, (type(None), bytes, str)), (
             "comment must be None or a string: %r" % comment)
         self.headers = headers or tuple()
         for req in self.required_headers:
             assert headers and has_header(headers, req), (
                 "Exception %s must be passed the header %r "
                 "(got headers: %r)"
                 % (self.__class__.__name__, req, headers))
@@ -202,18 +201,14 @@
                 'comment': comment_escfunc(self.comment)}
         if HTTPException.template != self.template:
             for (k, v) in environ.items():
                 args[k] = escfunc(v)
             if self.headers:
                 for (k, v) in self.headers:
                     args[k.lower()] = escfunc(v)
-        if six.PY2:
-            for key, value in args.items():
-                if isinstance(value, six.text_type):
-                    args[key] = value.encode('utf8', 'xmlcharrefreplace')
         return template % args
 
     def plain(self, environ):
         """ text/plain representation of the exception """
         body = self.make_body(environ, strip_html(self.template), no_quote, comment_quote)
         return ('%s %s\r\n%s\r\n' % (self.code, self.title, body))
 
@@ -234,15 +229,15 @@
         if 'html' in environ.get('HTTP_ACCEPT','') or \
             '*/*' in environ.get('HTTP_ACCEPT',''):
             replace_header(headers, 'content-type', 'text/html')
             content = self.html(environ)
         else:
             replace_header(headers, 'content-type', 'text/plain')
             content = self.plain(environ)
-        if isinstance(content, six.text_type):
+        if isinstance(content, str):
             content = content.encode('utf8')
             cur_content_type = (
                 header_value(headers, 'content-type')
                 or 'text/html')
             replace_header(
                 headers, 'content-type',
                 cur_content_type + '; charset=utf8')
@@ -590,16 +585,16 @@
     title = 'HTTP Version Not Supported'
     explanation = ('The HTTP version is not supported.')
 
 # abstract HTTP related exceptions
 __all__ = ['HTTPException', 'HTTPRedirection', 'HTTPError' ]
 
 _exceptions = {}
-for name, value in six.iteritems(dict(globals())):
-    if (isinstance(value, (type, six.class_types)) and
+for name, value in dict(globals()).items():
+    if (isinstance(value, type) and
         issubclass(value, HTTPException) and
         value.code):
         _exceptions[value.code] = value
         __all__.append(name)
 
 def get_exception(code):
     return _exceptions[code]
```

### Comparing `Paste-3.7.1/paste/httpheaders.py` & `Paste-3.8.0/paste/httpheaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,24 +131,17 @@
 
 .. [1] http://www.w3.org/Protocols/rfc2616/rfc2616-sec4.html#sec4.2
 .. [2] http://www.python.org/peps/pep-0333.html#environ-variables
 .. [3] http://www.python.org/peps/pep-0333.html#the-start-response-callable
 
 """
 import mimetypes
-import six
 from time import time as now
-try:
-    # Python 3
-    from email.utils import formatdate, parsedate_tz, mktime_tz
-    from urllib.request import AbstractDigestAuthHandler, parse_keqv_list, parse_http_list
-except ImportError:
-    # Python 2
-    from rfc822 import formatdate, parsedate_tz, mktime_tz
-    from urllib2 import AbstractDigestAuthHandler, parse_keqv_list, parse_http_list
+from email.utils import formatdate, parsedate_tz, mktime_tz
+from urllib.request import AbstractDigestAuthHandler, parse_keqv_list, parse_http_list
 
 from .httpexceptions import HTTPBadRequest
 
 __all__ = ['get_header', 'list_headers', 'normalize_headers',
            'HTTPHeader', 'EnvironVariable' ]
 
 class EnvironVariable(str):
@@ -167,15 +160,15 @@
 REMOTE_USER    = EnvironVariable("REMOTE_USER")
 REMOTE_SESSION = EnvironVariable("REMOTE_SESSION")
 AUTH_TYPE      = EnvironVariable("AUTH_TYPE")
 REQUEST_METHOD = EnvironVariable("REQUEST_METHOD")
 SCRIPT_NAME    = EnvironVariable("SCRIPT_NAME")
 PATH_INFO      = EnvironVariable("PATH_INFO")
 
-for _name, _obj in six.iteritems(dict(globals())):
+for _name, _obj in dict(globals()).items():
     if isinstance(_obj, EnvironVariable):
         __all__.append(_name)
 
 _headers = {}
 
 class HTTPHeader(object):
     """
@@ -733,15 +726,15 @@
             result.append('no-store')
         if no_transform:
             result.append('no-transform')
         if max_age is not None:
             result.append('max-age=%d' % max_age)
         if s_maxage is not None:
             result.append('s-maxage=%d' % s_maxage)
-        for (k, v) in six.iteritems(extensions):
+        for (k, v) in extensions.items():
             if k not in self.extensions:
                 raise AssertionError("unexpected extension used: '%s'" % k)
             result.append('%s="%s"' % (k.replace("_", "-"), v))
         return (result, expires)
 
     def compose(self, **kwargs):
         (result, expires) = self._compose(**kwargs)
@@ -1012,32 +1005,23 @@
         (_, realm) = challenge.split('realm="')
         (realm, _) = realm.split('"', 1)
         auth = AbstractDigestAuthHandler()
         auth.add_password(realm, path, username, password)
         (token, challenge) = challenge.split(' ', 1)
         chal = parse_keqv_list(parse_http_list(challenge))
         class FakeRequest(object):
-            if six.PY3:
-                @property
-                def full_url(self):
-                    return path
-
-                selector = full_url
-
-                @property
-                def data(self):
-                    return None
-            else:
-                def get_full_url(self):
-                    return path
-
-                get_selector = get_full_url
-
-                def has_data(self):
-                    return False
+            @property
+            def full_url(self):
+                return path
+
+            selector = full_url
+
+            @property
+            def data(self):
+                return None
 
             def get_method(self):
                 return method or "GET"
 
         retval = "Digest %s" % auth.get_authorization(FakeRequest(), chal)
         return (retval,)
 _Authorization('Authorization', 'request', 'RFC 2617')
@@ -1107,10 +1091,10 @@
 
 for head in _headers.values():
     headname = head.name.replace("-","_").upper()
     locals()[headname] = head
     __all__.append(headname)
 
 __pudge_all__ = __all__[:]
-for _name, _obj in six.iteritems(dict(globals())):
+for _name, _obj in dict(globals()).items():
     if isinstance(_obj, type) and issubclass(_obj, HTTPHeader):
         __pudge_all__.append(_name)
```

### Comparing `Paste-3.7.1/paste/httpserver.py` & `Paste-3.8.0/paste/httpserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 
 # @@: add in protection against HTTP/1.0 clients who claim to
 #     be 1.1 but do not send a Content-Length
 
 # @@: add support for chunked encoding, this is not a 1.1 server
 #     till this is completed.
 
-from __future__ import print_function
 import atexit
 import traceback
 import io
 import socket, sys, threading
 import posixpath
-import six
 import time
 import os
 from itertools import count
 from six.moves import _thread
 from six.moves import queue
 from six.moves.BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer
 from six.moves.socketserver import ThreadingMixIn
-from six.moves.urllib.parse import unquote, urlsplit
+from urllib.parse import unquote, urlsplit
 from paste.util import converters
 import logging
 try:
     from paste.util import killthread
 except ImportError:
     # Not available, probably no ctypes
     killthread = None
@@ -167,15 +165,15 @@
             self.end_headers()
         self.wfile.write(chunk)
 
     def wsgi_start_response(self, status, response_headers, exc_info=None):
         if exc_info:
             try:
                 if self.wsgi_headers_sent:
-                    six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                    raise exc_info
                 else:
                     # In this case, we're going to assume that the
                     # higher-level code is currently handling the
                     # issue and returning a resonable response.
                     # self.log_error(repr(exc_info))
                     pass
             finally:
@@ -598,15 +596,15 @@
         self.max_requests = max_requests
         self.name = name
         self.queue = queue.Queue()
         self.workers = []
         self.daemon = daemon
         if logger is None:
             logger = logging.getLogger('paste.httpserver.ThreadPool')
-        if isinstance(logger, six.string_types):
+        if isinstance(logger, str):
             logger = logging.getLogger(logger)
         self.logger = logger
         self.error_email = error_email
         self._worker_count = count()
 
         assert (not kill_thread_limit
                 or kill_thread_limit >= hung_thread_limit), (
@@ -756,15 +754,15 @@
     def thread_exists(self, thread_id):
         """
         Returns true if a thread with this id is still running
         """
         return thread_id in threading._active
 
     def add_worker_thread(self, *args, **kwargs):
-        index = six.next(self._worker_count)
+        index = next(self._worker_count)
         worker = threading.Thread(target=self.worker_thread_callback,
                                   args=args, kwargs=kwargs,
                                   name=("worker %d" % index))
         worker.daemon = self.daemon
         worker.start()
 
     def kill_hung_threads(self):
@@ -799,15 +797,15 @@
                 self.logger.warning(
                     'Thread %s hung (working on task for %i seconds)',
                     worker.thread_id, now - time_started)
                 try:
                     import pprint
                     info_desc = pprint.pformat(info)
                 except:
-                    out = six.StringIO()
+                    out = io.StringIO()
                     traceback.print_exc(file=out)
                     info_desc = 'Error:\n%s' % out.getvalue()
                 self.notify_problem(
                     "Killing worker thread (id=%(thread_id)s) because it has been \n"
                     "working on task for %(time)s seconds (limit is %(limit)s)\n"
                     "Info on task:\n"
                     "%(info)s"
@@ -913,16 +911,14 @@
                         # That last exception was intended to kill me
                         break
                 finally:
                     try:
                         del self.worker_tracker[thread_id]
                     except KeyError:
                         pass
-                    if six.PY2:
-                        sys.exc_clear()
                 self.idle_workers.append(thread_id)
         finally:
             try:
                 del self.worker_tracker[thread_id]
             except KeyError:
                 pass
             try:
```

### Comparing `Paste-3.7.1/paste/lint.py` & `Paste-3.8.0/paste/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,14 @@
 
   - That .close() is called (doesn't raise exception, only prints to
     sys.stderr, because we only know it isn't called when the object
     is garbage collected).
 """
 
 import re
-import six
 import sys
 import warnings
 
 header_re = re.compile(r'^[a-zA-Z][a-zA-Z0-9\-_]*$')
 bad_header_value_re = re.compile(r'[\000-\037]')
 
 class WSGIWarning(Warning):
@@ -181,28 +180,28 @@
 
     def __init__(self, wsgi_input):
         self.input = wsgi_input
 
     def read(self, *args):
         assert len(args) <= 1
         v = self.input.read(*args)
-        assert isinstance(v, six.binary_type)
+        assert isinstance(v, bytes)
         return v
 
     def readline(self, *args):
         v = self.input.readline(*args)
-        assert isinstance(v, six.binary_type)
+        assert isinstance(v, bytes)
         return v
 
     def readlines(self, *args):
         assert len(args) <= 1
         lines = self.input.readlines(*args)
         assert isinstance(lines, list)
         for line in lines:
-            assert isinstance(line, six.binary_type)
+            assert isinstance(line, bytes)
         return lines
 
     def __iter__(self):
         while 1:
             line = self.readline()
             if not line:
                 return
@@ -213,15 +212,15 @@
 
 class ErrorWrapper(object):
 
     def __init__(self, wsgi_errors):
         self.errors = wsgi_errors
 
     def write(self, s):
-        assert isinstance(s, six.string_types)
+        assert isinstance(s, str)
         self.errors.write(s)
 
     def flush(self):
         self.errors.flush()
 
     def writelines(self, seq):
         for line in seq:
@@ -232,15 +231,15 @@
 
 class WriteWrapper(object):
 
     def __init__(self, wsgi_writer):
         self.writer = wsgi_writer
 
     def __call__(self, s):
-        assert isinstance(s, six.binary_type)
+        assert isinstance(s, bytes)
         self.writer(s)
 
 class PartialIteratorWrapper(object):
 
     def __init__(self, wsgi_iterator):
         self.iterator = wsgi_iterator
 
@@ -258,15 +257,15 @@
 
     def __iter__(self):
         return self
 
     def next(self):
         assert not self.closed, (
             "Iterator read after closed")
-        v = six.next(self.iterator)
+        v = next(self.iterator)
         if self.check_start_response is not None:
             assert self.check_start_response, (
                 "The application returns and we started iterating over its body, but start_response has not yet been called")
             self.check_start_response = None
         return v
 
     __next__ = next
```

### Comparing `Paste-3.7.1/paste/modpython.py` & `Paste-3.8.0/paste/modpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 The module.function will be called with no arguments on server shutdown,
 once for each child process or thread.
 
 This module highly based on Robert Brewer's, here:
 http://projects.amor.org/misc/svn/modpython_gateway.py
 """
 
-import six
 import traceback
 
 try:
     from mod_python import apache
 except:
     pass
 from paste.deploy import loadapp
@@ -173,15 +172,15 @@
                 self.request.set_content_length(len(data))
                 self.request.write(data)
 
     def start_response(self, status, headers, exc_info=None):
         if exc_info:
             try:
                 if self.started:
-                    six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                    raise exc_info
             finally:
                 exc_info = None
 
         self.request.status = int(status[:3])
 
         for key, val in headers:
             if key.lower() == 'content-length':
```

### Comparing `Paste-3.7.1/paste/pony.py` & `Paste-3.8.0/paste/pony.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/progress.py` & `Paste-3.8.0/paste/progress.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/proxy.py` & `Paste-3.8.0/paste/proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,16 @@
     use = egg:Paste#proxy
     address = http://server3:8680/exist/rest/db/orgs/sch/config/
     allowed_request_methods = GET
 
 """
 
 from six.moves import http_client as httplib
-from six.moves.urllib import parse as urlparse
-from six.moves.urllib.parse import quote
-import six
+from urllib import parse as urlparse
+from urllib.parse import quote
 
 from paste import httpexceptions
 from paste.util.converters import aslist
 
 # Remove these headers from response (specify lower case header
 # names):
 filtered_headers = (
@@ -248,39 +247,17 @@
         return [body]
 
 def parse_headers(message):
     """
     Turn a Message object into a list of WSGI-style headers.
     """
     headers_out = []
-    if six.PY3:
-        for header, value in message.items():
-            if header.lower() not in filtered_headers:
-                headers_out.append((header, value))
-    else:
-        for full_header in message.headers:
-            if not full_header:
-                # Shouldn't happen, but we'll just ignore
-                continue
-            if full_header[0].isspace():
-                # Continuation line, add to the last header
-                if not headers_out:
-                    raise ValueError(
-                        "First header starts with a space (%r)" % full_header)
-                last_header, last_value = headers_out.pop()
-                value = last_value + ' ' + full_header.strip()
-                headers_out.append((last_header, value))
-                continue
-            try:
-                header, value = full_header.split(':', 1)
-            except:
-                raise ValueError("Invalid header: %r" % full_header)
-            value = value.strip()
-            if header.lower() not in filtered_headers:
-                headers_out.append((header, value))
+    for header, value in message.items():
+        if header.lower() not in filtered_headers:
+            headers_out.append((header, value))
     return headers_out
 
 def make_transparent_proxy(
     global_conf, force_host=None, force_scheme='http'):
     """
     Create a proxy that connects to a specific host, but does
     absolutely no other filtering, including the Host header.
```

### Comparing `Paste-3.7.1/paste/recursive.py` & `Paste-3.8.0/paste/recursive.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,16 @@
   paste.recursive.old_path_info:
       A list of previous ``PATH_INFO`` values from previous redirects.
 
 Raise ``ForwardRequestException(new_path_info)`` to do a forward
 (aborting the current request).
 """
 
-import six
 import warnings
-from six.moves import cStringIO as StringIO
+from io import StringIO
 
 __all__ = ['RecursiveMiddleware']
 __pudge_all__ =  ['RecursiveMiddleware', 'ForwardRequestException']
 
 class RecursionLoop(AssertionError):
     # Subclasses AssertionError for legacy reasons
     """Raised when a recursion enters into a loop"""
@@ -316,15 +315,15 @@
     Returns an IncludeResponse object.
     """
 
     def activate(self, environ):
         response = IncludedResponse()
         def start_response(status, headers, exc_info=None):
             if exc_info:
-                six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                raise exc_info
             response.status = status
             response.headers = headers
             return response.write
         app_iter = self.application(environ, start_response)
         try:
             for s in app_iter:
                 response.write(s)
@@ -370,15 +369,15 @@
     (be sure to call close on the response!)
     """
 
     def activate(self, environ):
         response = IncludedAppIterResponse()
         def start_response(status, headers, exc_info=None):
             if exc_info:
-                six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                raise exc_info
             response.status = status
             response.headers = headers
             return response.write
         app_iter = self.application(environ, start_response)
         response.app_iter = app_iter
         return response
```

### Comparing `Paste-3.7.1/paste/registry.py` & `Paste-3.8.0/paste/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 **NOTE:** This is *highly* unlikely to be an issue in the vast majority of
 cases, and requires incredibly large amounts of proxy object access before
 one should consider the proxy object to be causing slow-downs. This section
 is provided solely in the extremely rare case that it is an issue so that a
 quick way to work around it is documented.
 
 """
-import six
 import paste.util.threadinglocal as threadinglocal
 
 __all__ = ['StackedObjectProxy', 'RegistryManager', 'StackedObjectRestorer',
            'restorer']
 
 class NoDefault(object): pass
 
@@ -344,15 +343,15 @@
 
     # Replace now does the same thing as register
     replace = register
 
     def cleanup(self):
         """Remove all objects from all StackedObjectProxy instances that
         were tracked at this Registry context"""
-        for stacked, obj in six.itervalues(self.reglist[-1]):
+        for stacked, obj in self.reglist[-1].values():
             stacked._pop_object(obj)
         self.reglist.pop()
 
 class RegistryManager(object):
     """Creates and maintains a Registry context
 
     RegistryManager creates a new registry context for the registration of
@@ -497,15 +496,15 @@
         self.saved_registry_states[self.get_request_id(environ)] = \
             (registry, registry.reglist[:])
 
         # Tweak the StackedObjectProxies we want to save state for -- change
         # their methods to act differently when a restoration context is active
         # in the current thread
         for reglist in registry.reglist:
-            for stacked, obj in six.itervalues(reglist):
+            for stacked, obj in reglist.values():
                 self.enable_restoration(stacked)
 
     def get_saved_proxied_obj(self, stacked, request_id):
         """Retrieve the saved object proxied by the specified
         StackedObjectProxy for the request identified by request_id"""
         # All state for the request identified by request_id
         reglist = self.saved_registry_states[request_id][1]
```

### Comparing `Paste-3.7.1/paste/reloader.py` & `Paste-3.8.0/paste/reloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         return CONFIG_FILE_CACHE.keys()
     paste.reloader.add_file_callback(watch_config_files)
 
 Then every time the reloader polls files it will call
 ``watch_config_files`` and check all the filenames it returns.
 """
 
-from __future__ import print_function
 import os
 import sys
 import time
 import threading
 import traceback
 from paste.util.classinstance import classinstancemethod
```

### Comparing `Paste-3.7.1/paste/request.py` & `Paste-3.8.0/paste/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,18 @@
                    script_name=None, path_info=None, querystring=None)
    * path_info_split(path_info)
    * path_info_pop(environ)
    * resolve_relative_url(url, environ)
 
 """
 import cgi
-from six.moves.urllib import parse as urlparse
-from six.moves.urllib.parse import quote, parse_qsl
-try:
-    # Python 3
-    from http.cookies import SimpleCookie, CookieError
-except ImportError:
-    # Python 2
-    from Cookie import SimpleCookie, CookieError
-
-try:
-    from UserDict import DictMixin
-except ImportError:
-    from collections.abc import MutableMapping as DictMixin
-import six
+from collections.abc import MutableMapping as DictMixin
+from urllib import parse as urlparse
+from urllib.parse import quote, parse_qsl
+from http.cookies import SimpleCookie, CookieError
 
 from paste.util.multidict import MultiDict
 
 __all__ = ['get_cookies', 'get_cookie_dict', 'parse_querystring',
            'parse_formvars', 'construct_url', 'path_info_split',
            'path_info_pop', 'resolve_relative_url', 'EnvironHeaders']
 
@@ -170,19 +160,18 @@
     if use_cgi:
         # Prevent FieldStorage from parsing QUERY_STRING during GET/HEAD
         # requests
         old_query_string = environ.get('QUERY_STRING','')
         environ['QUERY_STRING'] = ''
         inp = environ['wsgi.input']
         kwparms = {}
-        if six.PY3:
-            if encoding:
-                kwparms['encoding'] = encoding
-            if errors:
-                kwparms['errors'] = errors
+        if encoding:
+            kwparms['encoding'] = encoding
+        if errors:
+            kwparms['errors'] = errors
         fs = cgi.FieldStorage(fp=inp,
                               environ=environ,
                               keep_blank_values=True,
                               **kwparms)
         environ['QUERY_STRING'] = old_query_string
         if isinstance(fs.value, list):
             for name in fs.keys():
```

### Comparing `Paste-3.7.1/paste/response.py` & `Paste-3.8.0/paste/response.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/session.py` & `Paste-3.8.0/paste/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,40 +19,34 @@
 
 @@: This doesn't do any locking, and may cause problems when a single
 session is accessed concurrently.  Also, it loads and saves the
 session for each request, with no caching.  Also, sessions aren't
 expired.
 """
 
-try:
-    # Python 3
-    from http.cookies import SimpleCookie
-except ImportError:
-    # Python 2
-    from Cookie import SimpleCookie
+from http.cookies import SimpleCookie
 import time
 import random
 import os
 import datetime
-import six
 import threading
 import tempfile
 
 try:
     import cPickle
 except ImportError:
     import pickle as cPickle
 try:
     from hashlib import md5
 except ImportError:
     from md5 import md5
 from paste import wsgilib
 from paste import request
 
-class SessionMiddleware(object):
+class SessionMiddleware:
 
     def __init__(self, application, global_conf=None, **factory_kw):
         self.application = application
         self.factory_kw = factory_kw
 
     def __call__(self, environ, start_response):
         session_factory = SessionFactory(environ, **self.factory_kw)
@@ -145,16 +139,15 @@
         """
         r = [time.time(), random.random()]
         if hasattr(os, 'times'):
             r.append(os.times())
         if for_object is not None:
             r.append(id(for_object))
         content = str(r)
-        if six.PY3:
-            content = content.encode('utf8')
+        content = content.encode('utf8')
         md5_hash = md5(content)
         try:
             return md5_hash.hexdigest()
         except AttributeError:
             # Older versions of Python didn't have hexdigest, so we'll
             # do it manually
             hexdigest = []
@@ -184,15 +177,15 @@
 
 class FileSession(object):
 
     def __init__(self, sid, create=False, session_file_path=tempfile.gettempdir(),
                  chmod=None,
                  expiration=2880, # in minutes: 48 hours
                  ):
-        if chmod and isinstance(chmod, (six.binary_type, six.text_type)):
+        if chmod and isinstance(chmod, (bytes, str)):
             chmod = int(chmod, 8)
         self.chmod = chmod
         if not sid:
             # Invalid...
             raise KeyError
         self.session_file_path = session_file_path
         self.sid = sid
```

### Comparing `Paste-3.7.1/paste/transaction.py` & `Paste-3.8.0/paste/transaction.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/translogger.py` & `Paste-3.8.0/paste/translogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Middleware for logging requests, using Apache combined log format
 """
 
 import logging
-import six
 import time
 from six.moves.urllib.parse import quote
 
-class TransLogger(object):
+class TransLogger:
     """
     This logging middleware will log all requests as they go through.
     They are, by default, sent to a logger named ``'wsgi'`` at the
     INFO level.
 
     If ``setup_console_handler`` is true, then messages for the named
     logger will be sent to the console.
@@ -111,17 +110,17 @@
     app, global_conf,
     logger_name='wsgi',
     format=None,
     logging_level=logging.INFO,
     setup_console_handler=True,
     set_logger_level=logging.DEBUG):
     from paste.util.converters import asbool
-    if isinstance(logging_level, (six.binary_type, six.text_type)):
+    if isinstance(logging_level, (bytes, str)):
         logging_level = logging._levelNames[logging_level]
-    if isinstance(set_logger_level, (six.binary_type, six.text_type)):
+    if isinstance(set_logger_level, (bytes, str)):
         set_logger_level = logging._levelNames[set_logger_level]
     return TransLogger(
         app,
         format=format or None,
         logging_level=logging_level,
         logger_name=logger_name,
         setup_console_handler=asbool(setup_console_handler),
```

### Comparing `Paste-3.7.1/paste/url.py` & `Paste-3.8.0/paste/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 
 """
 This module implements a class for handling URLs.
 """
-from six.moves.urllib.parse import parse_qsl, quote, unquote, urlencode
+import html
+from urllib.parse import parse_qsl, quote, unquote, urlencode
 from paste import request
-import six
-from paste.util import html
 
 # Imported lazily from FormEncode:
 variabledecode = None
 
 __all__ = ["URL", "Image"]
 
 def html_quote(v):
@@ -35,29 +34,24 @@
         return '[%s]' % ', '.join(map(js_repr, v))
     elif isinstance(v, dict):
         return '{%s}' % ', '.join(
             ['%s: %s' % (js_repr(key), js_repr(value))
              for key, value in v])
     elif isinstance(v, str):
         return repr(v)
-    elif isinstance(v, unicode):
-        # @@: how do you do Unicode literals in Javascript?
-        return repr(v.encode('UTF-8'))
     elif isinstance(v, (float, int)):
         return repr(v)
-    elif isinstance(v, long):
-        return repr(v).lstrip('L')
     elif hasattr(v, '__js_repr__'):
         return v.__js_repr__()
     else:
         raise ValueError(
             "I don't know how to turn %r into a Javascript representation"
             % v)
 
-class URLResource(object):
+class URLResource:
 
     """
     This is an abstract superclass for different kinds of URLs
     """
 
     default_params = {}
 
@@ -180,18 +174,15 @@
             if not new_url.endswith('/'):
                 new_url += '/'
             u = u.__class__(new_url+path, vars=u.vars,
                             attrs=u.attrs,
                             params=u.original_params)
         return u
 
-    if six.PY3:
-        __truediv__ = addpath
-    else:
-        __div__ = addpath
+    __truediv__ = addpath
 
     def become(self, OtherClass):
         return OtherClass(self.url, vars=self.vars,
                           attrs=self.attrs,
                           params=self.original_params)
 
     def href__get(self):
```

### Comparing `Paste-3.7.1/paste/urlmap.py` & `Paste-3.8.0/paste/urlmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 Map URL prefixes to WSGI applications.  See ``URLMap``
 """
 
+import html
 import re
 import os
-from paste.util import html
-try:
-    # Python 3
-    from collections.abc import MutableMapping as DictMixin
-except ImportError:
-    # Python 2
-    from UserDict import DictMixin
+from collections.abc import MutableMapping as DictMixin
 
 from paste import httpexceptions
 
 __all__ = ['URLMap', 'PathProxyURLMap']
 
 def urlmap_factory(loader, global_conf, **local_conf):
     if 'not_found_app' in local_conf:
@@ -237,15 +232,15 @@
     def __init__(self, map, base_paste_url, base_path, builder):
         self.map = map
         self.base_paste_url = self.map.normalize_url(base_paste_url)
         self.base_path = base_path
         self.builder = builder
 
     def __setitem__(self, url, app):
-        if isinstance(app, (str, unicode)):
+        if isinstance(app, str):
             app_fn = os.path.join(self.base_path, app)
             app = self.builder(app_fn)
         url = self.map.normalize_url(url)
         # @@: This means http://foo.com/bar will potentially
         # match foo.com, but /base_paste_url/bar, which is unintuitive
         url = (url[0] or self.base_paste_url[0],
                self.base_paste_url[1] + url[1])
```

### Comparing `Paste-3.7.1/paste/urlparser.py` & `Paste-3.8.0/paste/urlparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 """
 WSGI applications that parse the URL and dispatch to on-disk resources
 """
 
 import os
-import six
 import sys
-
-if six.PY2:
-    import imp
-else:
-    import importlib.util as imputil
+import importlib.util as imputil
 
 import mimetypes
 try:
     import pkg_resources
 except ImportError:
     pkg_resources = None
 from paste import request
@@ -135,15 +130,15 @@
         for name, value in constructor_conf.items():
             if not name.startswith('constructor '):
                 raise ValueError(
                     "Only extra configuration keys allowed are "
                     "'constructor .ext = import_expr'; you gave %r "
                     "(=%r)" % (name, value))
             ext = name[len('constructor '):].strip()
-            if isinstance(value, (str, unicode)):
+            if isinstance(value, str):
                 value = import_string.eval_import(value)
             self.constructors[ext] = value
 
     def __call__(self, environ, start_response):
         environ['paste.urlparser.base_python_name'] = self.base_python_name
         if self.init_module is NoDefault:
             self.init_module = self.find_init_module(environ)
@@ -388,30 +383,20 @@
         base_name = module_name.split('.')[-1]
         parent = load_module_from_name(environ, os.path.dirname(filename),
                                        parent_name, errors)
     else:
         base_name = module_name
     module = None
 
-    if six.PY2:
-        fp = None
-        try:
-            fp, pathname, stuff = imp.find_module(
-                base_name, [os.path.dirname(filename)])
-            module = imp.load_module(module_name, fp, pathname, stuff)
-        finally:
-            if fp is not None:
-                fp.close()
-    else:
-        # imp is deprecated and will be removed in Python 3.12
-        spec = imputil.spec_from_file_location(base_name, filename)
-        if spec is not None:
-            module = imputil.module_from_spec(spec)
-            sys.modules[base_name] = module
-            spec.loader.exec_module(module)
+    # imp is deprecated and will be removed in Python 3.12
+    spec = imputil.spec_from_file_location(base_name, filename)
+    if spec is not None:
+        module = imputil.module_from_spec(spec)
+        sys.modules[base_name] = module
+        spec.loader.exec_module(module)
 
     return module
 
 def make_py(parser, environ, filename):
     module = load_module(environ, filename)
     if not module:
         return None
@@ -537,15 +522,15 @@
         document_root, cache_max_age=cache_max_age)
 
 class PkgResourcesParser(StaticURLParser):
 
     def __init__(self, egg_or_spec, resource_name, manager=None, root_resource=None):
         if pkg_resources is None:
             raise NotImplementedError("This class requires pkg_resources.")
-        if isinstance(egg_or_spec, (six.binary_type, six.text_type)):
+        if isinstance(egg_or_spec, (bytes, str)):
             self.egg = pkg_resources.get_distribution(egg_or_spec)
         else:
             self.egg = egg_or_spec
         self.resource_name = resource_name
         if manager is None:
             manager = pkg_resources.ResourceManager()
         self.manager = manager
```

### Comparing `Paste-3.7.1/paste/util/PySourceColor.py` & `Paste-3.8.0/paste/util/PySourceColor.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 import time
 import glob
 import getopt
 import keyword
 import token
 import tokenize
 import traceback
-from six.moves import cStringIO as StringIO
+from io import StringIO
 # Do not edit
 NAME = token.NAME
 NUMBER = token.NUMBER
 COMMENT = tokenize.COMMENT
 OPERATOR = token.OP
 ERRORTOKEN = token.ERRORTOKEN
 ARGS = token.NT_OFFSET + 1
```

### Comparing `Paste-3.7.1/paste/util/classinit.py` & `Paste-3.8.0/paste/util/classinit.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/classinstance.py` & `Paste-3.8.0/paste/util/classinstance.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/dateinterval.py` & `Paste-3.8.0/paste/util/dateinterval.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/datetimeutil.py` & `Paste-3.8.0/paste/util/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/filemixin.py` & `Paste-3.8.0/paste/util/filemixin.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/finddata.py` & `Paste-3.8.0/paste/util/finddata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 # Note: you may want to copy this into your setup.py file verbatim, as
 # you can't import this from another package, when you don't know if
 # that package is installed yet.
 
-from __future__ import print_function
 import sys
 from fnmatch import fnmatchcase
 from pathlib import Path
 
 # Provided as an attribute, so you can append to these instead
 # of replicating them:
 standard_exclude = ('*.py', '*.pyc', '*$py.class', '*~', '.*', '*.bak')
```

### Comparing `Paste-3.7.1/paste/util/findpackage.py` & `Paste-3.8.0/paste/util/findpackage.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/import_string.py` & `Paste-3.8.0/paste/util/import_string.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/intset.py` & `Paste-3.8.0/paste/util/intset.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 """Immutable integer set type.
 
 Integer set class.
 
 Copyright (C) 2006, Heiko Wundram.
 Released under the MIT license.
 """
-import six
 
 # Version information
 # -------------------
 
 __author__ = "Heiko Wundram <me@modelnine.org>"
 __version__ = "0.2"
 __revision__ = "6"
 __date__ = "2006-01-20"
 
 
 # Utility classes
 # ---------------
 
-class _Infinity(object):
+class _Infinity:
     """Internal type used to represent infinity values."""
 
     __slots__ = ["_neg"]
 
     def __init__(self,neg):
         self._neg = neg
 
@@ -59,15 +58,15 @@
         if not isinstance(value, _VALID_TYPES):
             return NotImplemented
         return not isinstance(value,_Infinity) or self._neg != value._neg
 
     def __repr__(self):
         return "None"
 
-_VALID_TYPES = six.integer_types + (_Infinity,)
+_VALID_TYPES = (int, _Infinity)
 
 
 
 # Constants
 # ---------
 
 _MININF = _Infinity(True)
@@ -117,48 +116,48 @@
             self._min = _MININF
         if self._max is None:
             self._max = _MAXINF
 
         # Check keyword arguments.
         if kwargs:
             raise ValueError("Invalid keyword argument.")
-        if not ( isinstance(self._min, six.integer_types) or self._min is _MININF ):
+        if not ( isinstance(self._min, int) or self._min is _MININF ):
             raise TypeError("Invalid type of min argument.")
-        if not ( isinstance(self._max, six.integer_types) or self._max is _MAXINF ):
+        if not ( isinstance(self._max, int) or self._max is _MAXINF ):
             raise TypeError("Invalid type of max argument.")
         if ( self._min is not _MININF and self._max is not _MAXINF and
              self._min > self._max ):
             raise ValueError("Minimum is not smaller than maximum.")
-        if isinstance(self._max, six.integer_types):
+        if isinstance(self._max, int):
             self._max += 1
 
         # Process arguments.
         for arg in args:
-            if isinstance(arg, six.integer_types):
+            if isinstance(arg, int):
                 start, stop = arg, arg+1
             elif isinstance(arg,tuple):
                 if len(arg) != 2:
                     raise ValueError("Invalid tuple, must be (start,stop).")
 
                 # Process argument.
                 start, stop = arg
                 if start is None:
                     start = self._min
                 if stop is None:
                     stop = self._max
 
                 # Check arguments.
-                if not ( isinstance(start, six.integer_types) or start is _MININF ):
+                if not ( isinstance(start, int) or start is _MININF ):
                     raise TypeError("Invalid type of tuple start.")
-                if not ( isinstance(stop, six.integer_types) or stop is _MAXINF ):
+                if not ( isinstance(stop, int) or stop is _MAXINF ):
                     raise TypeError("Invalid type of tuple stop.")
                 if ( start is not _MININF and stop is not _MAXINF and
                      start > stop ):
                     continue
-                if isinstance(stop, six.integer_types):
+                if isinstance(stop, int):
                     stop += 1
             else:
                 raise TypeError("Invalid argument.")
 
             if start > self._max:
                 continue
             elif start < self._min:
@@ -211,15 +210,15 @@
                 i += 1
         self._ranges = tuple(self._ranges)
         self._hash = hash(self._ranges)
 
     def __coerce__(self,other):
         if isinstance(other,IntSet):
             return self, other
-        elif isinstance(other, six.integer_types + (tuple,)):
+        elif isinstance(other, (int, tuple,)):
             try:
                 return self, self.__class__(other)
             except TypeError:
                 # Catch a type error, in that case the structure specified by
                 # other is something we can't coerce, return NotImplemented.
                 # ValueErrors are not caught, they signal that the data was
                 # invalid for the constructor. This is appropriate to signal
@@ -454,15 +453,15 @@
                 if r[1] is _MAXINF:
                     ubranges.extend(([0,1],[-1,-1]))
                 else:
                     ubranges.append([r[1]-1,-1])
             elif r[1] is _MAXINF:
                 ubranges.append([r[0],1])
             else:
-                for val in xrange(r[0],r[1]):
+                for val in range(r[0],r[1]):
                     yield val
         if ubranges:
             while True:
                 for ubrange in ubranges:
                     yield ubrange[0]
                     ubrange[0] += ubrange[1]
 
@@ -471,18 +470,18 @@
 
     def __repr__(self):
         """Return a representation of this integer set. The representation is
         executable to get an equal integer set."""
 
         rv = []
         for start, stop in self._ranges:
-            if ( isinstance(start, six.integer_types) and isinstance(stop, six.integer_types)
+            if ( isinstance(start, int) and isinstance(stop, int)
                  and stop-start == 1 ):
                 rv.append("%r" % start)
-            elif isinstance(stop, six.integer_types):
+            elif isinstance(stop, int):
                 rv.append("(%r,%r)" % (start,stop-1))
             else:
                 rv.append("(%r,%r)" % (start,stop))
         if self._min is not _MININF:
             rv.append("min=%r" % self._min)
         if self._max is not _MAXINF:
             rv.append("max=%r" % self._max)
```

### Comparing `Paste-3.7.1/paste/util/ip4.py` & `Paste-3.8.0/paste/util/ip4.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 # Imports
 # -------
 
 from paste.util import intset
 import socket
-import six
 
 
 # IP4Range class
 # --------------
 
 class IP4Range(intset.IntSet):
     """IP4 address range class with efficient storage of address ranges.
@@ -84,22 +83,22 @@
                     args[i] = self._parseAddrRange(argval)
             elif isinstance(argval,tuple):
                 if len(tuple) != 2:
                     raise ValueError("Tuple is of invalid length.")
                 addr1, addr2 = argval
                 if isinstance(addr1,str):
                     addr1 = self._parseAddrRange(addr1)[0]
-                elif not isinstance(addr1, six.integer_types):
+                elif not isinstance(addr1, int):
                     raise TypeError("Invalid argument.")
                 if isinstance(addr2,str):
                     addr2 = self._parseAddrRange(addr2)[1]
-                elif not isinstance(addr2, six.integer_types):
+                elif not isinstance(addr2, int):
                     raise TypeError("Invalid argument.")
                 args[i] = (addr1,addr2)
-            elif not isinstance(argval, six.integer_types):
+            elif not isinstance(argval, int):
                 raise TypeError("Invalid argument.")
 
         # Initialize the integer set.
         super(IP4Range,self).__init__(min=self._MINIP4,max=self._MAXIP4,*args)
 
     # Parsing functions
     # -----------------
```

### Comparing `Paste-3.7.1/paste/util/killthread.py` & `Paste-3.8.0/paste/util/killthread.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Kill a thread, from http://sebulba.wikispaces.com/recipe+thread2
 """
-import six
 try:
     import ctypes
 except ImportError:
     raise ImportError(
         "You cannot use paste.util.killthread without ctypes installed")
 if not hasattr(ctypes, 'pythonapi'):
     raise ImportError(
         "You cannot use paste.util.killthread without ctypes.pythonapi")
 
 def async_raise(tid, exctype):
     """raises the exception, performs cleanup if needed.
 
     tid is the value given by thread.get_ident() (an integer).
     Raise SystemExit to kill a thread."""
-    if not isinstance(exctype, (six.class_types, type)):
+    if not isinstance(exctype, type):
         raise TypeError("Only types can be raised (not instances)")
     if not isinstance(tid, int):
         raise TypeError("tid must be an integer")
     res = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(tid), ctypes.py_object(exctype))
     if res == 0:
         raise ValueError("invalid thread id")
     elif res != 1:
```

### Comparing `Paste-3.7.1/paste/util/looper.py` & `Paste-3.8.0/paste/util/looper.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,16 @@
     ---
     3 c
 
 """
 
 __all__ = ['looper']
 
-import six
 
-
-class looper(object):
+class looper:
     """
     Helper for looping (particularly in templates)
 
     Use this like::
 
         for loop, item in looper(seq):
             if loop.first:
@@ -40,15 +38,15 @@
     def __iter__(self):
         return looper_iter(self.seq)
 
     def __repr__(self):
         return '<%s for %r>' % (
             self.__class__.__name__, self.seq)
 
-class looper_iter(object):
+class looper_iter:
 
     def __init__(self, seq):
         self.seq = list(seq)
         self.pos = 0
 
     def __iter__(self):
         return self
@@ -137,15 +135,15 @@
         if self.last:
             return True
         return self._compare_group(self.item, self.next, getter)
 
     def _compare_group(self, item, other, getter):
         if getter is None:
             return item != other
-        elif (isinstance(getter, (six.binary_type, six.text_type))
+        elif (isinstance(getter, (bytes, str))
               and getter.startswith('.')):
             getter = getter[1:]
             if getter.endswith('()'):
                 getter = getter[:-2]
                 return getattr(item, getter)() != getattr(other, getter)()
             else:
                 return getattr(item, getter) != getattr(other, getter)
```

### Comparing `Paste-3.7.1/paste/util/mimeparse.py` & `Paste-3.8.0/paste/util/mimeparse.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/multidict.py` & `Paste-3.8.0/paste/util/multidict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 import cgi
 import copy
-import six
 import sys
-
-try:
-    # Python 3
-    from collections.abc import MutableMapping as DictMixin
-except ImportError:
-    # Python 2
-    from UserDict import DictMixin
+from collections.abc import MutableMapping as DictMixin
 
 class MultiDict(DictMixin):
 
     """
     An ordered dictionary that can have multiple values for each key.
     Adds the methods getall, getone, mixed, and add to the normal
     dictionary interface.
@@ -30,15 +23,15 @@
             elif hasattr(args[0], 'items'):
                 items = args[0].items()
             else:
                 items = args[0]
             self._items = list(items)
         else:
             self._items = []
-        self._items.extend(six.iteritems(kw))
+        self._items.extend(kw.items())
 
     def __getitem__(self, key):
         for k, v in self._items:
             if k == key:
                 return v
         raise KeyError(repr(key))
 
@@ -261,21 +254,19 @@
         Decode the specified value to unicode. Assumes value is a ``str`` or
         `FieldStorage`` object.
 
         ``FieldStorage`` objects are specially handled.
         """
         if isinstance(value, cgi.FieldStorage):
             # decode FieldStorage's field name and filename
-            decode_name = self.decode_keys and isinstance(value.name, six.binary_type)
-            if six.PY2 or decode_name:
+            decode_name = self.decode_keys and isinstance(value.name, bytes)
+            if decode_name:
                 value = copy.copy(value)
                 if decode_name:
                     value.name = value.name.decode(self.encoding, self.errors)
-                if six.PY2:
-                    value.filename = value.filename.decode(self.encoding, self.errors)
         else:
             try:
                 value = value.decode(self.encoding, self.errors)
             except AttributeError:
                 pass
         return value
 
@@ -314,29 +305,29 @@
         Returns a dictionary where the values are either single
         values, or a list of values when a key/value appears more than
         once in this dictionary.  This is similar to the kind of
         dictionary often used to represent the variables in a web
         request.
         """
         unicode_mixed = {}
-        for key, value in six.iteritems(self.multi.mixed()):
+        for key, value in self.multi.mixed().items():
             if isinstance(value, list):
                 value = [self._decode_value(value) for value in value]
             else:
                 value = self._decode_value(value)
             unicode_mixed[self._decode_key(key)] = value
         return unicode_mixed
 
     def dict_of_lists(self):
         """
         Returns a dictionary where each key is associated with a
         list of values.
         """
         unicode_dict = {}
-        for key, value in six.iteritems(self.multi.dict_of_lists()):
+        for key, value in self.multi.dict_of_lists().items():
             value = [self._decode_value(value) for value in value]
             unicode_dict[self._decode_key(key)] = value
         return unicode_dict
 
     def __delitem__(self, key):
         key = self._encode_key(key)
         self.multi.__delitem__(key)
@@ -384,18 +375,18 @@
         for k in self.multi.iterkeys():
             yield self._decode_key(k)
 
     __iter__ = iterkeys
 
     def items(self):
         return [(self._decode_key(k), self._decode_value(v)) for \
-                    k, v in six.iteritems(self.multi)]
+                    k, v in self.multi.items()]
 
     def iteritems(self):
-        for k, v in six.iteritems(self.multi):
+        for k, v in self.multi.items():
             yield (self._decode_key(k), self._decode_value(v))
 
     def values(self):
         return [self._decode_value(v) for v in self.multi.itervalues()]
 
     def itervalues(self):
         for v in self.multi.itervalues():
```

### Comparing `Paste-3.7.1/paste/util/quoting.py` & `Paste-3.8.0/paste/util/quoting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 
-import six
 import re
 from six.moves import html_entities
-from six.moves.urllib.parse import quote, unquote
+from urllib.parse import quote, unquote
+import six
 
-from paste.util import html
+import html
 
 
 __all__ = ['html_quote', 'html_unquote', 'url_quote', 'url_unquote',
            'strip_html']
 
 default_encoding = 'UTF-8'
 
@@ -18,44 +18,35 @@
     r"""
     Quote the value (turned to a string) as HTML.  This quotes <, >,
     and quotes:
     """
     encoding = encoding or default_encoding
     if v is None:
         return ''
-    elif isinstance(v, six.binary_type):
-        if six.PY3:
-            return html.escape(v.decode(encoding), 1).encode(encoding)
-        else:
-            return html.escape(v, 1)
-    elif isinstance(v, six.text_type):
-        if six.PY3:
-            return html.escape(v, 1)
-        else:
-            return html.escape(v.encode(encoding), 1)
+    elif isinstance(v, bytes):
+        return html.escape(v.decode(encoding), 1).encode(encoding)
+    elif isinstance(v, str):
+        return html.escape(v, 1)
     else:
-        if six.PY3:
-            return html.escape(six.text_type(v), 1)
-        else:
-            return html.escape(six.text_type(v).encode(encoding), 1)
+        return html.escape(str(v), 1)
 
 _unquote_re = re.compile(r'&([a-zA-Z]+);')
 def _entity_subber(match, name2c=html_entities.name2codepoint):
     code = name2c.get(match.group(1))
     if code:
         return six.unichr(code)
     else:
         return match.group(0)
 
 def html_unquote(s, encoding=None):
     r"""
     Decode the value.
 
     """
-    if isinstance(s, six.binary_type):
+    if isinstance(s, bytes):
         s = s.decode(encoding or default_encoding)
     return _unquote_re.sub(_entity_subber, s)
 
 def strip_html(s):
     # should this use html_unquote?
     s = re.sub('<.*?>', '', s)
     s = html_unquote(s)
```

### Comparing `Paste-3.7.1/paste/util/scgiserver.py` & `Paste-3.8.0/paste/util/scgiserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 and point mod_scgi (or whatever your SCGI front end is) at port 4000.
 
 Kudos to the WSGI folk for writing a nice PEP & the Quixote folk for
 writing a nice extensible SCGI server for Python!
 """
 
-import six
 import sys
 import time
 from scgi import scgi_server
 
 def debug(msg):
     timestamp = time.strftime("%Y-%m-%d %H:%M:%S",
                               time.localtime(time.time()))
@@ -87,15 +86,15 @@
             chunks.append(data)
 
         def start_response(status, response_headers, exc_info=None):
             if exc_info:
                 try:
                     if headers_sent:
                         # Re-raise original exception if headers sent
-                        six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                        raise exc_info
                 finally:
                     exc_info = None     # avoid dangling circular ref
             elif headers_set:
                 raise AssertionError("Headers already set!")
 
             headers_set[:] = [status, response_headers]
             return write
```

### Comparing `Paste-3.7.1/paste/util/template.py` & `Paste-3.8.0/paste/util/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 If there are syntax errors ``TemplateError`` will be raised.
 """
 
 import re
 import six
 import sys
 from html import escape
-from six.moves.urllib.parse import quote
+from urllib.parse import quote
 from paste.util.looper import looper
 
 __all__ = ['TemplateError', 'Template', 'sub', 'HTMLTemplate',
            'sub_html', 'html', 'bunch']
 
 token_re = re.compile(r'\{\{|\}\}')
 in_re = re.compile(r'\s+in\s+')
@@ -74,15 +74,15 @@
         'looper': looper,
         }
 
     default_encoding = 'utf8'
 
     def __init__(self, content, name=None, namespace=None):
         self.content = content
-        self._unicode = isinstance(content, six.text_type)
+        self._unicode = isinstance(content, str)
         self.name = name
         self._parsed = parse(content, name=name)
         if namespace is None:
             namespace = {}
         self.namespace = namespace
 
     def from_filename(cls, filename, namespace=None, encoding=None):
@@ -120,15 +120,15 @@
         parts = []
         self._interpret_codes(self._parsed, ns, out=parts)
         return ''.join(parts)
 
     def _interpret_codes(self, codes, ns, out):
         __traceback_hide__ = True
         for item in codes:
-            if isinstance(item, six.string_types):
+            if isinstance(item, str):
                 out.append(item)
             else:
                 self._interpret_code(item, ns, out)
 
     def _interpret_code(self, code, ns, out):
         __traceback_hide__ = True
         name, pos = code[0], code[1]
@@ -181,15 +181,15 @@
             except _TemplateBreak:
                 break
 
     def _interpret_if(self, parts, ns, out):
         __traceback_hide__ = True
         # @@: if/else/else gets through
         for part in parts:
-            assert not isinstance(part, six.string_types)
+            assert not isinstance(part, str)
             name, pos = part[0], part[1]
             if name == 'else':
                 result = True
             else:
                 result = self._eval(part[2], ns, pos)
             if result:
                 self._interpret_codes(part[3], ns, out)
@@ -209,46 +209,40 @@
                 arg0 = str(e)
             e.args = (self._add_line_info(arg0, pos),)
             six.reraise(exc_info[0], e, exc_info[2])
 
     def _exec(self, code, ns, pos):
         __traceback_hide__ = True
         try:
-            six.exec_(code, ns)
+            exec(code, ns)
         except:
             exc_info = sys.exc_info()
             e = exc_info[1]
             e.args = (self._add_line_info(e.args[0], pos),)
             six.reraise(exc_info[0], e, exc_info[2])
 
     def _repr(self, value, pos):
         __traceback_hide__ = True
         try:
             if value is None:
                 return ''
-            if self._unicode:
-                try:
-                    value = six.text_type(value)
-                except UnicodeDecodeError:
-                    value = str(value)
-            else:
-                value = str(value)
+            value = str(value)
         except:
             exc_info = sys.exc_info()
             e = exc_info[1]
             e.args = (self._add_line_info(e.args[0], pos),)
             six.reraise(exc_info[0], e, exc_info[2])
         else:
-            if self._unicode and isinstance(value, six.binary_type):
+            if self._unicode and isinstance(value, bytes):
                 if not self.decode_encoding:
                     raise UnicodeDecodeError(
                         'Cannot decode str value %r into unicode '
                         '(no default_encoding provided)' % value)
                 value = value.decode(self.default_encoding)
-            elif not self._unicode and isinstance(value, six.text_type):
+            elif not self._unicode and isinstance(value, str):
                 if not self.decode_encoding:
                     raise UnicodeEncodeError(
                         'Cannot encode unicode value %r into str '
                         '(no default_encoding provided)' % value)
                 value = value.encode(self.default_encoding)
             return value
 
@@ -313,32 +307,22 @@
     def __repr__(self):
         return '<%s %r>' % (
             self.__class__.__name__, self.value)
 
 def html_quote(value):
     if value is None:
         return ''
-    if not isinstance(value, six.string_types):
-        if six.PY2 and hasattr(value, '__unicode__'):
-            value = unicode(value)
-        else:
-            value = str(value)
+    if not isinstance(value, str):
+        value = str(value)
     value = escape(value, 1)
-    if six.PY2 and isinstance(value, unicode):
-        value = value.encode('ascii', 'xmlcharrefreplace')
     return value
 
 def url(v):
-    if not isinstance(v, six.string_types):
-        if six.PY2 and hasattr(v, '__unicode__'):
-            v = unicode(v)
-        else:
-            v = str(v)
-    if six.PY2 and isinstance(v, unicode):
-        v = v.encode('utf8')
+    if not isinstance(v, str):
+        v = str(v)
     return quote(v)
 
 def attr(**kw):
     kw = sorted(kw.items())
     parts = []
     for name, value in kw:
         if value is None:
@@ -443,30 +427,30 @@
        >>> tokens
        [('if x', (1, 3)), '\nx\n', ('endif', (3, 3)), '\ny']
        >>> trim_lex(tokens)
        [('if x', (1, 3)), 'x\n', ('endif', (3, 3)), 'y']
     """
     for i in range(len(tokens)):
         current = tokens[i]
-        if isinstance(tokens[i], six.string_types):
+        if isinstance(tokens[i], str):
             # we don't trim this
             continue
         item = current[0]
         if not statement_re.search(item) and item not in single_statements:
             continue
         if not i:
             prev = ''
         else:
             prev = tokens[i-1]
         if i+1 >= len(tokens):
             next = ''
         else:
             next = tokens[i+1]
-        if (not isinstance(next, six.string_types)
-            or not isinstance(prev, six.string_types)):
+        if (not isinstance(next, str)
+            or not isinstance(prev, str)):
             continue
         if ((not prev or trail_whitespace_re.search(prev))
             and (not next or lead_whitespace_re.search(next))):
             if prev:
                 m = trail_whitespace_re.search(prev)
                 # +1 to leave the leading \n on:
                 prev = prev[:m.start()+1]
@@ -537,15 +521,15 @@
     result = []
     while tokens:
         next, tokens = parse_expr(tokens, name)
         result.append(next)
     return result
 
 def parse_expr(tokens, name, context=()):
-    if isinstance(tokens[0], six.string_types):
+    if isinstance(tokens[0], str):
         return tokens[0], tokens[1:]
     expr, pos = tokens[0]
     expr = expr.strip()
     if expr.startswith('py:'):
         expr = expr[3:].lstrip(' \t')
         if expr.startswith('\n'):
             expr = expr[1:]
```

### Comparing `Paste-3.7.1/paste/util/threadedprint.py` & `Paste-3.8.0/paste/util/threadedprint.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/util/threadinglocal.py` & `Paste-3.8.0/paste/util/threadinglocal.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/paste/wsgilib.py` & `Paste-3.8.0/paste/wsgilib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 
 """
 A module of many disparate routines.
 """
 
-from __future__ import print_function
-
 # functions which moved to paste.request and paste.response
 # Deprecated around 15 Dec 2005
+import io
+import sys
+import warnings
+from traceback import print_exception
+from io import StringIO
+from urllib.parse import unquote, urlsplit
+
 from paste.request import get_cookies, parse_querystring, parse_formvars
 from paste.request import construct_url, path_info_split, path_info_pop
 from paste.response import HeaderDict, has_header, header_value, remove_header
 from paste.response import error_body_response, error_response, error_response_app
 
-from traceback import print_exception
-import six
-import sys
-from six.moves import cStringIO as StringIO
-from six.moves.urllib.parse import unquote, urlsplit
-import warnings
 
 __all__ = ['add_close', 'add_start_close', 'capture_output', 'catch_errors',
            'catch_errors_app', 'chained_app_iters', 'construct_url',
            'dump_environ', 'encode_unicode_app_iter', 'error_body_response',
            'error_response', 'get_cookies', 'has_header', 'header_value',
            'interactive', 'intercept_output', 'path_info_pop',
            'path_info_split', 'raw_interactive', 'send_file']
 
-class add_close(object):
+class add_close:
     """
     An an iterable that iterates over app_iter, then calls
     close_func.
     """
 
     def __init__(self, app_iterable, close_func):
         self.app_iterable = app_iterable
@@ -115,18 +114,18 @@
         self._closed = False
 
     def __iter__(self):
         return self
 
     def next(self):
         if len(self.chained) == 1:
-            return six.next(self.chained[0])
+            return next(self.chained[0])
         else:
             try:
-                return six.next(self.chained[0])
+                return next(self.chained[0])
             except StopIteration:
                 self.chained.pop(0)
                 return self.next()
     __next__ = next
 
     def close(self):
         self._closed = True
@@ -134,15 +133,15 @@
         for app_iter in self.app_iters:
             try:
                 if hasattr(app_iter, 'close'):
                     app_iter.close()
             except:
                 got_exc = sys.exc_info()
         if got_exc:
-            six.reraise(got_exc[0], got_exc[1], got_exc[2])
+            raise got_exc
 
     def __del__(self):
         if not self._closed:
             # We can't raise an error or anything at this stage
             print("Error: app_iter.close() was not called when finishing "
                 "WSGI request. finalization function %s not called"
                   % self.close_func, file=sys.stderr)
@@ -160,15 +159,15 @@
         self.errors = errors
 
     def __iter__(self):
         return self
 
     def next(self):
         content = next(self.app_iter)
-        if isinstance(content, six.text_type):
+        if isinstance(content, str):
             content = content.encode(self.encoding, self.errors)
         return content
     __next__ = next
 
     def close(self):
         if hasattr(self.app_iterable, 'close'):
             self.app_iterable.close()
@@ -205,15 +204,15 @@
             self.close = self.app_iterable.close
 
     def __iter__(self):
         return self
 
     def next(self):
         try:
-            return six.next(self.app_iter)
+            return next(self.app_iter)
         except StopIteration:
             if self.ok_callback:
                 self.ok_callback()
             raise
         except:
             self.error_callback(sys.exc_info())
             raise
@@ -257,15 +256,15 @@
             self.close = self.app_iterable.close
 
     def __iter__(self):
         return self
 
     def next(self):
         try:
-            return six.next(self.app_iter)
+            return next(self.app_iter)
         except StopIteration:
             if self.ok_callback:
                 self.ok_callback()
             raise
         except self.catch:
             if hasattr(self.app_iterable, 'close'):
                 try:
@@ -274,40 +273,40 @@
                     # @@: Print to wsgi.errors?
                     pass
             new_app_iterable = self.error_callback_app(
                 self.environ, self.start_response, sys.exc_info())
             app_iter = iter(new_app_iterable)
             if hasattr(new_app_iterable, 'close'):
                 self.close = new_app_iterable.close
-            self.next = lambda: six.next(app_iter)
+            self.next = lambda: next(app_iter)
             return self.next()
     __next__ = next
 
 def raw_interactive(application, path='', raise_on_wsgi_error=False,
                     **environ):
     """
     Runs the application in a fake environment.
     """
     assert "path_info" not in environ, "argument list changed"
     if raise_on_wsgi_error:
         errors = ErrorRaiser()
     else:
-        errors = six.StringIO()
+        errors = io.StringIO()
     basic_environ = {
         # mandatory CGI variables
         'REQUEST_METHOD': 'GET',     # always mandatory
         'SCRIPT_NAME': '',           # may be empty if app is at the root
         'PATH_INFO': '',             # may be empty if at root of app
         'SERVER_NAME': 'localhost',  # always mandatory
         'SERVER_PORT': '80',         # always mandatory
         'SERVER_PROTOCOL': 'HTTP/1.0',
         # mandatory wsgi variables
         'wsgi.version': (1, 0),
         'wsgi.url_scheme': 'http',
-        'wsgi.input': six.BytesIO(),
+        'wsgi.input': io.BytesIO(),
         'wsgi.errors': errors,
         'wsgi.multithread': False,
         'wsgi.multiprocess': False,
         'wsgi.run_once': False,
         }
     if path:
         (_, _, path_info, query, fragment) = urlsplit(str(path))
@@ -321,26 +320,26 @@
         name = name.replace('__', '.')
         basic_environ[name] = value
     if ('SERVER_NAME' in basic_environ
         and 'HTTP_HOST' not in basic_environ):
         basic_environ['HTTP_HOST'] = basic_environ['SERVER_NAME']
     istream = basic_environ['wsgi.input']
     if isinstance(istream, bytes):
-        basic_environ['wsgi.input'] = six.BytesIO(istream)
+        basic_environ['wsgi.input'] = io.BytesIO(istream)
         basic_environ['CONTENT_LENGTH'] = len(istream)
     data = {}
     output = []
     headers_set = []
     headers_sent = []
     def start_response(status, headers, exc_info=None):
         if exc_info:
             try:
                 if headers_sent:
                     # Re-raise original exception only if headers sent
-                    six.reraise(exc_info[0], exc_info[1], exc_info[2])
+                    raise exc_info
             finally:
                 # avoid dangling circular reference
                 exc_info = None
         elif headers_set:
             # You cannot set the headers more than once, unless the
             # exc_info is provided.
             raise AssertionError("Headers already set and no exc_info!")
@@ -348,15 +347,15 @@
         data['status'] = status
         data['headers'] = headers
         return output.append
     app_iter = application(basic_environ, start_response)
     try:
         try:
             for s in app_iter:
-                if not isinstance(s, six.binary_type):
+                if not isinstance(s, bytes):
                     raise ValueError(
                         "The app_iter response can only contain bytes (not "
                         "unicode); got: %r" % s)
                 headers_sent.append(True)
                 if not headers_set:
                     raise AssertionError("Content sent w/o headers!")
                 output.append(s)
@@ -421,16 +420,15 @@
         output.append("%s: %s\n" % (k, v))
     output.append("\n")
     content_length = environ.get("CONTENT_LENGTH", '')
     if content_length:
         output.append(environ['wsgi.input'].read(int(content_length)))
         output.append("\n")
     output = "".join(output)
-    if six.PY3:
-        output = output.encode('utf8')
+    output = output.encode('utf8')
     headers = [('Content-Type', 'text/plain'),
                ('Content-Length', str(len(output)))]
     start_response("200 OK", headers)
     return [output]
 
 def send_file(filename):
     warnings.warn(
```

### Comparing `Paste-3.7.1/paste/wsgiwrappers.py` & `Paste-3.8.0/paste/wsgiwrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 
 The WSGIRequest and WSGIResponse objects are light wrappers to make it easier
 to deal with an incoming request and sending a response.
 """
 import re
 import warnings
 from pprint import pformat
-try:
-    # Python 3
-    from http.cookies import SimpleCookie
-except ImportError:
-    # Python 2
-    from Cookie import SimpleCookie
-import six
+from http.cookies import SimpleCookie
 
 from paste.request import EnvironHeaders, get_cookie_dict, \
     parse_dict_querystring, parse_formvars
 from paste.util.multidict import MultiDict, UnicodeMultiDict
 from paste.registry import StackedObjectProxy
 from paste.response import HeaderDict
 from paste.wsgilib import encode_unicode_app_iter
@@ -407,15 +401,15 @@
             self.cookies[key]['path'] = path
         if domain is not None:
             self.cookies[key]['domain'] = domain
         self.cookies[key]['expires'] = 0
         self.cookies[key]['max-age'] = 0
 
     def _set_content(self, content):
-        if not isinstance(content, (six.binary_type, six.text_type)):
+        if not isinstance(content, (bytes, str)):
             self._iter = content
             if isinstance(content, list):
                 self._is_str_iter = True
             else:
                 self._is_str_iter = False
         else:
             self._iter = [content]
```

### Comparing `Paste-3.7.1/setup.py` & `Paste-3.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # - update version in setup.py (__version__)
 # - update changelog: docs/news.txt
 # - commit and push to git
 # - make release
 #
 # The final step will release to pypi and to Github
 
-__version__ = '3.7.1'
+__version__ = '3.8.0'
 
 from setuptools import setup, find_packages
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__),
                                 'paste', 'util'))
 import finddata
```

### Comparing `Paste-3.7.1/tests/cgiapp_data/form.cgi` & `Paste-3.8.0/tests/cgiapp_data/form.cgi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python
 
-from __future__ import print_function
-
 import sys
 
 # Quiet warnings in this CGI so that it does not upset tests.
 if not sys.warnoptions:
     import warnings
     warnings.simplefilter("ignore")
```

### Comparing `Paste-3.7.1/tests/template.txt` & `Paste-3.8.0/tests/template.txt`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_auth/test_auth_cookie.py` & `Paste-3.8.0/tests/test_auth/test_auth_cookie.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # (c) 2005 Clark C. Evans
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
-from six.moves import xrange
-import six
-
 from paste.auth import cookie
 from paste.wsgilib import raw_interactive, dump_environ
 from paste.response import header_value
 from paste.httpexceptions import *
 
 def build(application,setenv, *args, **kwargs):
     def setter(environ, start_response):
@@ -32,15 +29,14 @@
     value = header_value(headers,'Set-Cookie')
     assert "Path=/;" in value
     assert "expires=" not in value
     cookie = value.split(";")[0]
     (status,headers,content,errors) = \
             raw_interactive(app,{'HTTP_COOKIE': cookie})
     expected = ("%s: %s" % (key,val.replace("\n","\n    ")))
-    if six.PY3:
-        expected = expected.encode('utf8')
+    expected = expected.encode('utf8')
     assert expected in content
 
 def test_roundtrip():
-    roundtrip = str('').join(map(chr, xrange(256)))
+    roundtrip = str('').join(map(chr, range(256)))
     test_basic(roundtrip,roundtrip)
```

### Comparing `Paste-3.7.1/tests/test_auth/test_auth_digest.py` & `Paste-3.8.0/tests/test_auth/test_auth_digest.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 
 from paste.auth.digest import *
 from paste.wsgilib import raw_interactive
 from paste.httpexceptions import *
 from paste.httpheaders import AUTHORIZATION, WWW_AUTHENTICATE, REMOTE_USER
 import os
-import six
 
 def application(environ, start_response):
     content = REMOTE_USER(environ)
     start_response("200 OK",(('Content-Type', 'text/plain'),
                              ('Content-Length', len(content))))
 
-    if six.PY3:
-        content = content.encode('utf8')
+    content = content.encode('utf8')
     return [content]
 
 realm = "tag:clarkevans.com,2005:testing"
 
 def backwords(environ, realm, username):
     """ dummy password hash, where user password is just reverse """
     password = list(username)
@@ -56,16 +54,16 @@
 # The following code uses sockets to test the functionality,
 # to enable use:
 #
 # $ TEST_SOCKET=1 pytest
 
 
 if os.environ.get("TEST_SOCKET", ""):
-    from six.moves.urllib.error import HTTPError
-    from six.moves.urllib.request import build_opener, HTTPDigestAuthHandler
+    from urllib.error import HTTPError
+    from urllib.request import build_opener, HTTPDigestAuthHandler
     from paste.debug.testserver import serve
     server = serve(application)
 
     def authfetch(username,password,path="/",realm=realm):
         server.accept(2)
         import socket
         socket.setdefaulttimeout(5)
```

### Comparing `Paste-3.7.1/tests/test_auth/test_auth_tkt.py` & `Paste-3.8.0/tests/test_auth/test_auth_tkt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import hashlib
-import six
-if six.PY3:
-    import base64
+import base64
+from http.cookies import SimpleCookie
 from paste.auth.auth_tkt import AuthTicket
-try:
-    from http.cookies import SimpleCookie
-except ImportError:
-    # Python 2
-    from Cookie import SimpleCookie
 
 
 def test_auth_ticket_digest_and_cookie_value():
     test_parameters = [
         (
             (
                 'shared_secret',
@@ -104,17 +98,14 @@
             }
         ),
     ]
 
     for test_args, test_kwargs, expected_values in test_parameters:
         token = AuthTicket(*test_args, **test_kwargs)
         expected_cookie = SimpleCookie()
-        if six.PY3:
-            # import pdb; pdb.set_trace()
-            expected_cookie_value = base64.b64encode(expected_values['cookie_value'])
-        else:
-            expected_cookie_value = expected_values['cookie_value'].encode('base64')
+        # import pdb; pdb.set_trace()
+        expected_cookie_value = base64.b64encode(expected_values['cookie_value'])
 
         expected_cookie[expected_values['name']] = expected_cookie_value
         expected_cookie[expected_values['name']]['path'] = expected_values['path']
         expected_cookie[expected_values['name']]['secure'] = expected_values['secure']
         assert expected_cookie == token.cookie()
```

### Comparing `Paste-3.7.1/tests/test_cgiapp.py` & `Paste-3.8.0/tests/test_cgiapp.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_cgitb_catcher.py` & `Paste-3.8.0/tests/test_cgitb_catcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,15 @@
 ############################################################
 ## Tests
 ############################################################
 
 def test_makes_exception():
     res = do_request(bad_app)
     print(res)
-    if six.PY3:
-        assert 'bad_app() takes 0 positional arguments but 2 were given' in res
-    else:
-        assert 'bad_app() takes no arguments (2 given' in res
+    assert 'bad_app() takes 0 positional arguments but 2 were given' in res
     assert 'iterator = application(environ, start_response_wrapper)' in res
     assert 'lint.py' in res
     assert 'cgitb_catcher.py' in res
 
 def test_start_res():
     res = do_request(start_response_app)
     print(res)
```

### Comparing `Paste-3.7.1/tests/test_config.py` & `Paste-3.8.0/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # (c) 2007 Philip Jenvey; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 
 import pytest
-import six
 
 from paste.config import CONFIG, ConfigMiddleware
 from paste.fixture import TestApp
 
 test_key = 'test key'
 
 def reset_config():
@@ -16,30 +15,28 @@
         except IndexError:
             break
 
 def app_with_config(environ, start_response):
     start_response('200 OK', [('Content-type','text/plain')])
     lines = ['Variable is: %s\n' % CONFIG[test_key],
             'Variable is (in environ): %s' % environ['paste.config'][test_key]]
-    if six.PY3:
-        lines = [line.encode('utf8') for line in lines]
+    lines = [line.encode('utf8') for line in lines]
     return lines
 
 class NestingAppWithConfig(object):
     def __init__(self, app):
         self.app = app
 
     def __call__(self, environ, start_response):
         response = self.app(environ, start_response)
         assert isinstance(response, list)
         supplement = ['Nesting variable is: %s' % CONFIG[test_key],
                       'Nesting variable is (in environ): %s' % \
                           environ['paste.config'][test_key]]
-        if six.PY3:
-            supplement = [line.encode('utf8') for line in supplement]
+        supplement = [line.encode('utf8') for line in supplement]
         response.extend(supplement)
         return response
 
 def test_request_config():
     try:
         config = {test_key: 'test value'}
         app = ConfigMiddleware(app_with_config, config)
```

### Comparing `Paste-3.7.1/tests/test_doctests.py` & `Paste-3.8.0/tests/test_doctests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import doctest
 import os
 
 import pytest
-import six
 
 from paste.util.import_string import simple_import
 
 filenames = [
     'tests/template.txt',
     ]
 
@@ -26,16 +25,15 @@
     'paste.util.quoting',
     'paste.wsgilib',
     'paste.url',
     'paste.request',
     ]
 
 options = doctest.ELLIPSIS | doctest.REPORT_ONLY_FIRST_FAILURE
-if six.PY3:
-    options |= doctest.IGNORE_EXCEPTION_DETAIL
+options |= doctest.IGNORE_EXCEPTION_DETAIL
 
 
 @pytest.mark.parametrize('filename', filenames)
 def test_doctests(filename):
     filename = os.path.join(
         os.path.dirname(os.path.dirname(__file__)),
         filename)
```

### Comparing `Paste-3.7.1/tests/test_errordocument.py` & `Paste-3.8.0/tests/test_errordocument.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_exceptions/test_error_middleware.py` & `Paste-3.8.0/tests/test_exceptions/test_error_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,18 +69,15 @@
 ## Tests
 ############################################################
 
 def test_makes_exception():
     res = do_request(bad_app)
     assert '<html' in res
     res = strip_html(str(res))
-    if six.PY3:
-        assert 'bad_app() takes 0 positional arguments but 2 were given' in res
-    else:
-        assert 'bad_app() takes no arguments (2 given' in res, repr(res)
+    assert 'bad_app() takes 0 positional arguments but 2 were given' in res
     assert 'iterator = application(environ, start_response_wrapper)' in res
     assert 'paste.lint' in res
     assert 'paste.exceptions.errormiddleware' in res
 
 def test_unicode_exception():
     res = do_request(unicode_bad_app)
```

### Comparing `Paste-3.7.1/tests/test_exceptions/test_formatter.py` & `Paste-3.8.0/tests/test_exceptions/test_formatter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_exceptions/test_httpexceptions.py` & `Paste-3.8.0/tests/test_exceptions/test_httpexceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,32 @@
 """
 WSGI Exception Middleware
 
 Regression Test Suite
 """
 
 import pytest
-import six
 
-from paste.httpexceptions import *
+from paste.httpexceptions import (
+    get_exception,
+    HTTPBadRequest,
+    HTTPClientError,
+    HTTPError,
+    HTTPException,
+    HTTPExceptionHandler,
+    HTTPFound,
+    HTTPInternalServerError,
+    HTTPMovedPermanently,
+    HTTPNotFound,
+    HTTPNotImplemented,
+    HTTPRedirection,
+    HTTPServerError,
+    HTTPTemporaryRedirect,
+    HTTPUseProxy,
+)
 from paste.response import header_value
 
 
 def test_HTTPMove():
     """ make sure that location is a mandatory attribute of Redirects """
     pytest.raises(AssertionError, HTTPFound)
     pytest.raises(AssertionError, HTTPTemporaryRedirect,
@@ -67,18 +82,15 @@
         saved.append((status,headers))
     def redapp(environ, start_response):
         raise HTTPFound("/bing/foo")
     app = HTTPExceptionHandler(redapp)
     result = list(app({'HTTP_ACCEPT': 'text/html'},saveit))
     assert b'<a href="/bing/foo">' in result[0]
     assert "302 Found" == saved[0][0]
-    if six.PY3:
-        assert "text/html; charset=utf8" == header_value(saved[0][1], 'content-type')
-    else:
-        assert "text/html" == header_value(saved[0][1], 'content-type')
+    assert "text/html; charset=utf8" == header_value(saved[0][1], 'content-type')
     assert "/bing/foo" == header_value(saved[0][1],'location')
     result = list(app({'HTTP_ACCEPT': 'text/plain'},saveit))
     assert "text/plain; charset=utf8" == header_value(saved[1][1],'content-type')
     assert "/bing/foo" == header_value(saved[1][1],'location')
 
 def test_misc():
     assert get_exception(301) == HTTPMovedPermanently
```

### Comparing `Paste-3.7.1/tests/test_exceptions/test_reporter.py` & `Paste-3.8.0/tests/test_exceptions/test_reporter.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_fileapp.py` & `Paste-3.8.0/tests/test_fileapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # (c) 2005 Ian Bicking, Clark C. Evans and contributors
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 import time
 import random
 import os
 import tempfile
-try:
-    # Python 3
-    from email.utils import parsedate_tz, mktime_tz
-except ImportError:
-    # Python 2
-    from rfc822 import parsedate_tz, mktime_tz
-import six
+from email.utils import parsedate_tz, mktime_tz
 
 from paste import fileapp
 from paste.fileapp import *
 from paste.fixture import *
 
 # NOTE(haypo): don't use string.letters because the order of lower and upper
 # case letters changes when locale.setlocale() is called for the first time
@@ -97,16 +91,15 @@
             headers={'if-modified-since':
                 'Thu, 22 Dec 3030 01:01:01 GMT'})
     assert 400 == res.status and b"check your system clock" in res.body
 
 def test_file():
     tempfile = "test_fileapp.%s.txt" % (random.random())
     content = LETTERS * 20
-    if six.PY3:
-        content = content.encode('utf8')
+    content = content.encode('utf8')
     with open(tempfile, "wb") as fp:
         fp.write(content)
     try:
         app = fileapp.FileApp(tempfile)
         res = TestApp(app).get("/")
         assert len(content) == int(res.header('content-length'))
         assert 'text/plain' == res.header('content-type')
@@ -178,27 +171,25 @@
     assert res.header('content-length') == '1'
     res = build("bytes=%d-%d" % (3,17), status=206)
     assert res.body == content[3:18]
     assert res.header('content-length') == '15'
 
 def test_range():
     content = LETTERS * 5
-    if six.PY3:
-        content = content.encode('utf8')
+    content = content.encode('utf8')
     def build(range, status=206):
         app = DataApp(content)
         return TestApp(app).get("/",headers={'Range': range}, status=status)
     _excercize_range(build,content)
     build('bytes=0-%d' % (len(content)+1), 416)
 
 def test_file_range():
     tempfile = "test_fileapp.%s.txt" % (random.random())
     content = LETTERS * (1+(fileapp.CACHE_SIZE // len(LETTERS)))
-    if six.PY3:
-        content = content.encode('utf8')
+    content = content.encode('utf8')
     assert len(content) > fileapp.CACHE_SIZE
     with open(tempfile, "wb") as fp:
         fp.write(content)
     try:
         def build(range, status=206):
             app = fileapp.FileApp(tempfile)
             return TestApp(app).get("/",headers={'Range': range},
```

### Comparing `Paste-3.7.1/tests/test_fixture.py` & `Paste-3.8.0/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_grantip.py` & `Paste-3.8.0/tests/test_grantip.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
     def application(environ, start_response):
         start_response('200 OK', [('content-type', 'text/plain')])
         lines = [
             str(environ.get('REMOTE_USER')),
             ':',
             str(environ.get('REMOTE_USER_TOKENS')),
             ]
-        if six.PY3:
-            lines = [line.encode('utf8') for line in lines]
+        lines = [line.encode('utf8') for line in lines]
         return lines
     ip_map = {
         '127.0.0.1': (None, 'system'),
         '192.168.0.0/16': (None, 'worker'),
         '192.168.0.5<->192.168.0.8': ('bob', 'editor'),
         '192.168.0.8': ('__remove__', '-worker'),
         }
```

### Comparing `Paste-3.7.1/tests/test_gzipper.py` & `Paste-3.8.0/tests/test_gzipper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from paste.fixture import TestApp
 from paste.gzipper import middleware
 import gzip
-import six
+import io
 
 def simple_app(environ, start_response):
     start_response('200 OK',
                    [('content-type', 'text/plain'),
                     ('content-length', '0')])
     return [b'this is a test'] if environ['REQUEST_METHOD'] != 'HEAD' else []
 
@@ -13,15 +13,15 @@
 app = TestApp(wsgi_app)
 
 def test_gzip():
     res = app.get(
         '/', extra_environ=dict(HTTP_ACCEPT_ENCODING='gzip'))
     assert int(res.header('content-length')) == len(res.body)
     assert res.body != b'this is a test'
-    actual = gzip.GzipFile(fileobj=six.BytesIO(res.body)).read()
+    actual = gzip.GzipFile(fileobj=io.BytesIO(res.body)).read()
     assert actual == b'this is a test'
 
 def test_gzip_head():
     res = app.head(
         '/', extra_environ=dict(HTTP_ACCEPT_ENCODING='gzip'))
     assert int(res.header('content-length')) == 0
     assert res.body == b''
```

### Comparing `Paste-3.7.1/tests/test_httpheaders.py` & `Paste-3.8.0/tests/test_httpheaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,34 @@
-from paste.httpheaders import *
 import time
 
+from paste.httpheaders import (
+    normalize_headers,
+    ACCEPT,
+    ACCEPT_CHARSET,
+    AGE,
+    ALLOW,
+    CACHE_CONTROL,
+    CONTENT_DISPOSITION,
+    CONTENT_ENCODING,
+    CONTENT_LENGTH,
+    CONTENT_TYPE,
+    DATE,
+    EXPIRES,
+    ETAG,
+    FROM,
+    IF_MODIFIED_SINCE,
+    PRAGMA,
+    RANGE,
+    REFERER,
+    UPGRADE,
+    VIA,
+    VARY,
+    WWW_AUTHENTICATE,
+)
+
 def _test_generic(collection):
     assert 'bing' == VIA(collection)
     REFERER.update(collection,'internal:/some/path')
     assert 'internal:/some/path' == REFERER(collection)
     CACHE_CONTROL.update(collection,max_age=1234)
     CONTENT_DISPOSITION.update(collection,filename="bingles.txt")
     PRAGMA.update(collection,"test","multi",'valued="items"')
```

### Comparing `Paste-3.7.1/tests/test_httpserver.py` & `Paste-3.8.0/tests/test_httpserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import email
 import io
 import socket
 
-import six
-
 from paste.httpserver import LimitedLengthFile, WSGIHandler, serve
-from six.moves import StringIO
 
 
 class MockServer(object):
     server_address = ('127.0.0.1', 80)
 
 
 class MockSocket(object):
     def makefile(self, mode, bufsize):
-        return StringIO()
+        return io.StringIO()
 
 
 def test_environ():
     mock_socket = MockSocket()
     mock_client_address = '1.2.3.4'
     mock_server = MockServer()
 
@@ -55,18 +52,14 @@
     assert f.tell() == 0
     assert f.read() == b'012345678'
     assert f.tell() == 9
     assert f.read() == b''
 
 def test_limited_length_file_tell_on_socket():
     backing_read, backing_write = socket.socketpair()
-    if six.PY2:
-        # On Python 2, socketpair() returns an internal socket type rather than
-        # the public one.
-        backing_read = socket.socket(_sock=backing_read)
     f = LimitedLengthFile(backing_read.makefile('rb'), 10)
     backing_write.send(b'0123456789')
     backing_write.close()
     assert f.tell() == 0
     assert f.read(1) == b'0'
     assert f.tell() == 1
     assert f.read() == b'123456789'
@@ -126,8 +119,8 @@
         svr.server_close()
         
         assert (af == socket.AF_INET6)
         assert (addr[0] == '::1')
         assert (str(p) == port)
     except (socket.error, OSError) as err:
         # v6 support not available in this OS, pass the test
-        assert True
+        assert True
```

### Comparing `Paste-3.7.1/tests/test_multidict.py` & `Paste-3.8.0/tests/test_multidict.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # (c) 2007 Ian Bicking and Philip Jenvey; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 import cgi
 import gc
 import io
 
 import pytest
-import six
 
 from paste.util.multidict import MultiDict, UnicodeMultiDict
 
 def test_dict():
     d = MultiDict({'a': 1})
     assert d.items() == [('a', 1)]
 
@@ -59,31 +58,31 @@
 
 def _test_unicode_dict(decode_param_names=False):
     d = UnicodeMultiDict(MultiDict({b'a': 'a test'}))
     d.encoding = 'utf-8'
     d.errors = 'ignore'
 
     if decode_param_names:
-        key_str = six.text_type
+        key_str = str
         k = lambda key: key
         d.decode_keys = True
     else:
-        key_str = six.binary_type
+        key_str = bytes
         k = lambda key: key.encode()
 
     def assert_unicode(obj):
-        assert isinstance(obj, six.text_type)
+        assert isinstance(obj, str)
 
     def assert_key_str(obj):
         assert isinstance(obj, key_str)
 
     def assert_unicode_item(obj):
         key, value = obj
         assert isinstance(key, key_str)
-        assert isinstance(value, six.text_type)
+        assert isinstance(value, str)
 
     assert d.items() == [(k('a'), u'a test')]
     map(assert_key_str, d.keys())
     map(assert_unicode, d.values())
 
     d[b'b'] = b'2 test'
     d[b'c'] = b'3 test'
@@ -102,40 +101,40 @@
                          (k('b'), u'5 test')]
     list(map(assert_unicode_item, d.items()))
 
     del d[k('b')]
     assert d.items() == [(k('a'), u'a test'), (k('c'), u'3 test')]
     list(map(assert_unicode_item, d.items()))
     assert d.pop('xxx', u'5 test') == u'5 test'
-    assert isinstance(d.pop('xxx', u'5 test'), six.text_type)
+    assert isinstance(d.pop('xxx', u'5 test'), str)
     assert d.getone(k('a')) == u'a test'
-    assert isinstance(d.getone(k('a')), six.text_type)
+    assert isinstance(d.getone(k('a')), str)
     assert d.popitem() == (k('c'), u'3 test')
     d[k('c')] = b'3 test'
     assert_unicode_item(d.popitem())
     assert d.items() == [(k('a'), u'a test')]
     list(map(assert_unicode_item, d.items()))
 
     item = []
     assert d.setdefault(k('z'), item) is item
     items = d.items()
     assert items == [(k('a'), u'a test'), (k('z'), item)]
     assert isinstance(items[1][0], key_str)
     assert isinstance(items[1][1], list)
 
-    assert isinstance(d.setdefault(k('y'), b'y test'), six.text_type)
-    assert isinstance(d[k('y')], six.text_type)
+    assert isinstance(d.setdefault(k('y'), b'y test'), str)
+    assert isinstance(d[k('y')], str)
 
     assert d.mixed() == {k('a'): u'a test', k('y'): u'y test', k('z'): item}
     assert d.dict_of_lists() == {k('a'): [u'a test'], k('y'): [u'y test'],
                                  k('z'): [item]}
     del d[k('z')]
-    list(map(assert_unicode_item, six.iteritems(d.mixed())))
+    list(map(assert_unicode_item, d.mixed().items()))
     list(map(assert_unicode_item, [(key, value[0]) for \
-                                   key, value in six.iteritems(d.dict_of_lists())]))
+                                   key, value in d.dict_of_lists().items()]))
 
     assert k('a') in d
     dcopy = d.copy()
     assert dcopy is not d
     assert dcopy == d
     d[k('x')] = 'x test'
     assert dcopy != d
@@ -151,15 +150,15 @@
     fs.name = 'thefile'
     fs.filename = 'hello.txt'
     fs.file = io.BytesIO(b'hello')
     d[k('f')] = fs
     ufs = d[k('f')]
     assert isinstance(ufs, cgi.FieldStorage)
     assert ufs.name == fs.name
-    assert isinstance(ufs.name, str if six.PY3 else key_str)
+    assert isinstance(ufs.name, str)
     assert ufs.filename == fs.filename
-    assert isinstance(ufs.filename, six.text_type)
+    assert isinstance(ufs.filename, str)
     assert isinstance(ufs.value, bytes)
     assert ufs.value == b'hello'
     ufs = None
     gc.collect()
     assert not fs.file.closed
```

### Comparing `Paste-3.7.1/tests/test_profilemiddleware.py` & `Paste-3.8.0/tests/test_profilemiddleware.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_proxy.py` & `Paste-3.8.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_recursive.py` & `Paste-3.8.0/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_registry.py` & `Paste-3.8.0/tests/test_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,23 @@
     return [b'Hello world!\n']
 
 def simpleapp_withregistry(environ, start_response):
     status = '200 OK'
     response_headers = [('Content-type','text/plain')]
     start_response(status, response_headers)
     body = 'Hello world!Value is %s\n' % regobj.keys()
-    if six.PY3:
-        body = body.encode('utf8')
+    body = body.encode('utf8')
     return [body]
 
 def simpleapp_withregistry_default(environ, start_response):
     status = '200 OK'
     response_headers = [('Content-type','text/plain')]
     start_response(status, response_headers)
     body = 'Hello world!Value is %s\n' % secondobj
-    if six.PY3:
-        body = body.encode('utf8')
+    body = body.encode('utf8')
     return [body]
 
 
 class RegistryUsingApp(object):
     def __init__(self, var, value, raise_exc=False):
         self.var = var
         self.value = value
@@ -48,64 +46,60 @@
             environ['paste.registry'].register(self.var, self.value)
         if self.raise_exc:
             raise self.raise_exc
         status = '200 OK'
         response_headers = [('Content-type','text/plain')]
         start_response(status, response_headers)
         body = 'Hello world!\nThe variable is %s' % str(regobj)
-        if six.PY3:
-            body = body.encode('utf8')
+        body = body.encode('utf8')
         return [body]
 
 class RegistryUsingIteratorApp(object):
     def __init__(self, var, value):
         self.var = var
         self.value = value
 
     def __call__(self, environ, start_response):
         if 'paste.registry' in environ:
             environ['paste.registry'].register(self.var, self.value)
         status = '200 OK'
         response_headers = [('Content-type','text/plain')]
         start_response(status, response_headers)
         body = 'Hello world!\nThe variable is %s' % str(regobj)
-        if six.PY3:
-            body = body.encode('utf8')
+        body = body.encode('utf8')
         return iter([body])
 
 class RegistryMiddleMan(object):
     def __init__(self, app, var, value, depth):
         self.app = app
         self.var = var
         self.value = value
         self.depth = depth
 
     def __call__(self, environ, start_response):
         if 'paste.registry' in environ:
             environ['paste.registry'].register(self.var, self.value)
         line = ('\nInserted by middleware!\nInsertValue at depth %s is %s'
                 % (self.depth, str(regobj)))
-        if six.PY3:
-            line = line.encode('utf8')
+        line = line.encode('utf8')
         app_response = [line]
         app_iter = None
         app_iter = self.app(environ, start_response)
         if type(app_iter) in (list, tuple):
             app_response.extend(app_iter)
         else:
             response = []
             for line in app_iter:
                 response.append(line)
             if hasattr(app_iter, 'close'):
                 app_iter.close()
             app_response.extend(response)
         line = ('\nAppended by middleware!\nAppendValue at \
                 depth %s is %s' % (self.depth, str(regobj)))
-        if six.PY3:
-            line = line.encode('utf8')
+        line = line.encode('utf8')
         app_response.append(line)
         return app_response
 
 
 def test_simple():
     app = TestApp(simpleapp)
     response = app.get('/')
```

### Comparing `Paste-3.7.1/tests/test_request.py` & `Paste-3.8.0/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # (c) 2005 Ben Bangert
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 from paste.fixture import *
 from paste.request import *
 from paste.wsgiwrappers import WSGIRequest
-import six
 
 def simpleapp(environ, start_response):
     status = '200 OK'
     response_headers = [('Content-type','text/plain')]
     start_response(status, response_headers)
     request = WSGIRequest(environ)
     body = [
         'Hello world!\n', 'The get is %s' % str(request.GET),
         ' and Val is %s\n' % request.GET.get('name'),
         'The languages are: %s\n' % request.languages,
         'The accepttypes is: %s\n' % request.match_accept(['text/html', 'application/xml'])]
-    if six.PY3:
-        body = [line.encode('utf8')  for line in body]
+    body = [line.encode('utf8')  for line in body]
     return body
 
 def test_gets():
     app = TestApp(simpleapp)
     res = app.get('/')
     assert 'Hello' in res
     assert "get is MultiDict([])" in res
```

### Comparing `Paste-3.7.1/tests/test_request_form.py` & `Paste-3.8.0/tests/test_request_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import six
+import io
 
 from paste.request import *
 from paste.util.multidict import MultiDict
 
 def test_parse_querystring():
     e = {'QUERY_STRING': 'a=1&b=2&c=3&b=4'}
     d = parse_querystring(e)
@@ -14,15 +14,15 @@
     assert d == [('a', ''), ('b', ''), ('c', ''), ('d', '1')]
 
 def make_post(body):
     e = {
         'CONTENT_TYPE': 'application/x-www-form-urlencoded',
         'CONTENT_LENGTH': str(len(body)),
         'REQUEST_METHOD': 'POST',
-        'wsgi.input': six.BytesIO(body),
+        'wsgi.input': io.BytesIO(body),
         }
     return e
 
 def test_parse_formvars_nodup():
     """GH85: Test that parse_formvars can be called twice."""
     e = {'QUERY_STRING': 'a=1&b=2&c=3&b=4', 'wsgi.input': ""}
     d1 = parse_formvars(e)
```

### Comparing `Paste-3.7.1/tests/test_session.py` & `Paste-3.8.0/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from paste.session import SessionMiddleware
 from paste.fixture import TestApp
-import six
 
 info = []
 
 def wsgi_app(environ, start_response):
     pi = environ.get('PATH_INFO', '')
     if pi in ('/get1', '/get2'):
         if pi == '/get1':
             sess = environ['paste.session.factory']()
         start_response('200 OK', [('content-type', 'text/plain')])
         if pi == '/get2':
             sess = environ['paste.session.factory']()
         if 'info' in sess:
             body = str(sess['info'])
-            if six.PY3:
-                body = body.encode('utf8')
+            body = body.encode('utf8')
             return [body]
         else:
             return [b'no-info']
     if pi in ('/put1', '/put2'):
         if pi == '/put1':
             sess = environ['paste.session.factory']()
             sess['info']  = info[0]
```

### Comparing `Paste-3.7.1/tests/test_urlmap.py` & `Paste-3.8.0/tests/test_urlmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from paste.urlmap import *
-from paste.fixture import *
-import six
+from paste.urlmap import URLMap
+from paste.fixture import TestApp
 
 def make_app(response_text):
     def app(environ, start_response):
         headers = [('Content-type', 'text/html')]
         start_response('200 OK', headers)
         body = response_text % environ
-        if six.PY3:
-            body = body.encode('ascii')
+        body = body.encode('ascii')
         return [body]
     return app
 
 def test_map():
     mapper = URLMap({})
     app = TestApp(mapper)
     text = '%s script_name="%%(SCRIPT_NAME)s" path_info="%%(PATH_INFO)s"'
```

### Comparing `Paste-3.7.1/tests/test_urlparser.py` & `Paste-3.8.0/tests/test_urlparser.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_util/test_datetimeutil.py` & `Paste-3.8.0/tests/test_util/test_datetimeutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # (c) 2005 Clark C. Evans and contributors
 # This module is part of the Python Paste Project and is released under
 # the MIT License: http://www.opensource.org/licenses/mit-license.php
 # Some of this code was funded by: http://prometheusresearch.com
 from time import localtime
 from datetime import date
-from paste.util.datetimeutil import *
+from paste.util.datetimeutil import (
+    normalize_date,
+    normalize_time,
+    normalize_timedelta,
+    parse_date,
+)
 
 def test_timedelta():
     assert('' == normalize_timedelta(""))
     assert('0.10' == normalize_timedelta("6m"))
     assert('0.50' == normalize_timedelta("30m"))
     assert('0.75' == normalize_timedelta("45m"))
     assert('1.00' == normalize_timedelta("60 min"))
```

### Comparing `Paste-3.7.1/tests/test_util/test_mimeparse.py` & `Paste-3.8.0/tests/test_util/test_mimeparse.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_util/test_quoting.py` & `Paste-3.8.0/tests/test_util/test_quoting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from paste.util import quoting
-import six
 import unittest
 
 class TestQuoting(unittest.TestCase):
     def test_html_unquote(self):
         self.assertEqual(quoting.html_unquote(b'&lt;hey&nbsp;you&gt;'),
-                         u'<hey\xa0you>')
+                         '<hey\xa0you>')
         self.assertEqual(quoting.html_unquote(b''),
-                         u'')
+                         '')
         self.assertEqual(quoting.html_unquote(b'&blahblah;'),
-                         u'&blahblah;')
+                         '&blahblah;')
         self.assertEqual(quoting.html_unquote(b'\xe1\x80\xa9'),
-                         u'\u1029')
+                         '\u1029')
 
     def test_html_quote(self):
         self.assertEqual(quoting.html_quote(1),
                          '1')
         self.assertEqual(quoting.html_quote(None),
                          '')
         self.assertEqual(quoting.html_quote('<hey!>'),
                          '&lt;hey!&gt;')
         self.assertEqual(quoting.html_quote(b'<hey!>'),
                          b'&lt;hey!&gt;')
-        if six.PY3:
-            self.assertEqual(quoting.html_quote(u'<\u1029>'),
-                             u'&lt;\u1029&gt;')
-        else:
-            self.assertEqual(quoting.html_quote(u'<\u1029>'),
-                             '&lt;\xe1\x80\xa9&gt;')
+        self.assertEqual(quoting.html_quote('<\u1029>'),
+                         '&lt;\u1029&gt;')
```

### Comparing `Paste-3.7.1/tests/test_wsgilib.py` & `Paste-3.8.0/tests/test_wsgilib.py`

 * *Files identical despite different names*

### Comparing `Paste-3.7.1/tests/test_wsgiwrappers.py` & `Paste-3.8.0/tests/test_wsgiwrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # (c) 2007 Philip Jenvey; written for Paste (http://pythonpaste.org)
 # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
 import cgi
 import io
 from paste.fixture import TestApp
 from paste.wsgiwrappers import WSGIRequest, WSGIResponse
-import six
 
 class AssertApp(object):
     def __init__(self, assertfunc):
         self.assertfunc = assertfunc
 
     def __call__(self, environ, start_response):
         start_response('200 OK', [('Content-type','text/plain')])
@@ -83,15 +82,15 @@
         assert fs.value == b'Sushi'
 
         request.charset = 'UTF-8'
         assert len(request.POST) == 1
         assert isinstance(request.POST.keys()[0], str)
         fs = request.POST['thefile']
         assert isinstance(fs, cgi.FieldStorage)
-        assert isinstance(fs.filename, six.text_type)
+        assert isinstance(fs.filename, str)
         assert fs.filename == u'寿司.txt'
         assert fs.value == b'Sushi'
 
         request.charset = None
         assert fs.value == b'Sushi'
         return []
 
@@ -103,50 +102,50 @@
     assert response.content_type == 'text/html'
     assert response.charset == 'UTF-8'
     response.write(u'test')
     response.write(u'test2')
     response.write('test3')
     status, headers, content = response.wsgi_response()
     for data in content:
-        assert isinstance(data, six.binary_type)
+        assert isinstance(data, bytes)
 
     WSGIResponse.defaults._push_object(dict(content_type='text/html',
                                             charset='iso-8859-1'))
     try:
         response = WSGIResponse()
         response.write(u'test')
         response.write(u'test2')
         response.write('test3')
         status, headers, content = response.wsgi_response()
         for data in content:
-            assert isinstance(data, six.binary_type)
+            assert isinstance(data, bytes)
     finally:
         WSGIResponse.defaults._pop_object()
 
     # WSGIResponse will allow unicode to pass through when no charset is
     # set
     WSGIResponse.defaults._push_object(dict(content_type='text/html',
                                             charset=None))
     try:
         response = WSGIResponse(u'test')
         response.write(u'test1')
         status, headers, content = response.wsgi_response()
         for data in content:
-            assert isinstance(data, six.text_type)
+            assert isinstance(data, str)
     finally:
         WSGIResponse.defaults._pop_object()
 
     WSGIResponse.defaults._push_object(dict(content_type='text/html',
                                             charset=''))
     try:
         response = WSGIResponse(u'test')
         response.write(u'test1')
         status, headers, content = response.wsgi_response()
         for data in content:
-            assert isinstance(data, six.text_type)
+            assert isinstance(data, str)
     finally:
         WSGIResponse.defaults._pop_object()
 
 def test_call_wsgiresponse():
     resp = WSGIResponse(b'some content', 'application/octet-stream')
     def sp(status, response_headers):
         assert status == '200 OK'
```

