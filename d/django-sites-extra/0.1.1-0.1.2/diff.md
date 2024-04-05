# Comparing `tmp/django-sites-extra-0.1.1.tar.gz` & `tmp/django-sites-extra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sites-extra-0.1.1.tar", last modified: Sat Mar 30 21:37:29 2024, max compression
+gzip compressed data, was "django-sites-extra-0.1.2.tar", last modified: Fri Apr  5 21:11:33 2024, max compression
```

## Comparing `django-sites-extra-0.1.1.tar` & `django-sites-extra-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.097574 django-sites-extra-0.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44607 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44178 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44917 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16622 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44629 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.093574 django-sites-extra-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 21:37:29.000000 django-sites-extra-0.1.1/src/django_sites_extra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/src/sites_extra/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/src/sites_extra/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/src/sites_extra/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:29.101574 django-sites-extra-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-30 21:37:19.000000 django-sites-extra-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.439829 django-sites-extra-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-05 21:11:33.439829 django-sites-extra-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.435829 django-sites-extra-0.1.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22177 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21977 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22389 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23592 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22389 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22189 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-05 21:11:33.439829 django-sites-extra-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.431829 django-sites-extra-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.439829 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 21:11:33.000000 django-sites-extra-0.1.2/src/django_sites_extra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.435829 django-sites-extra-0.1.2/src/sites_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.435829 django-sites-extra-0.1.2/src/sites_extra/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/src/sites_extra/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:33.439829 django-sites-extra-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 21:11:18.000000 django-sites-extra-0.1.2/tox.ini
```

### Comparing `django-sites-extra-0.1.1/.pre-commit-config.yaml` & `django-sites-extra-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/LICENSE` & `django-sites-extra-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/PKG-INFO` & `django-sites-extra-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sites-extra
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django application to extend the standard "sites" framework with extra utils.
 Home-page: https://github.com/DLRSP/django-sites-extra
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-sites-extra-0.1.1/README.md` & `django-sites-extra-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/mkdocs.yml` & `django-sites-extra-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/pyproject.toml` & `django-sites-extra-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     --strict-markers
     --ds=tests.settings
     """
 django_find_project = false
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "0.1.1"
+current_version = "0.1.2"
 commit = true
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
```

### Comparing `django-sites-extra-0.1.1/requirements/docs.txt` & `django-sites-extra-0.1.2/requirements/py38-django42.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,459 +1,315 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/docs.txt requirements/docs.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
 #
-babel==2.14.0 \
-    --hash=sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363 \
-    --hash=sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287
-    # via mkdocs-material
-certifi==2024.2.2 \
-    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
-    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
-    # via requests
-charset-normalizer==3.3.2 \
-    --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
-    --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
-    --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
-    --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
-    --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
-    --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
-    --hash=sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574 \
-    --hash=sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e \
-    --hash=sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519 \
-    --hash=sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898 \
-    --hash=sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269 \
-    --hash=sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3 \
-    --hash=sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f \
-    --hash=sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6 \
-    --hash=sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8 \
-    --hash=sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a \
-    --hash=sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73 \
-    --hash=sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc \
-    --hash=sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714 \
-    --hash=sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2 \
-    --hash=sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc \
-    --hash=sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce \
-    --hash=sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d \
-    --hash=sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e \
-    --hash=sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6 \
-    --hash=sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269 \
-    --hash=sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96 \
-    --hash=sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d \
-    --hash=sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a \
-    --hash=sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4 \
-    --hash=sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77 \
-    --hash=sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d \
-    --hash=sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0 \
-    --hash=sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed \
-    --hash=sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068 \
-    --hash=sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac \
-    --hash=sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25 \
-    --hash=sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8 \
-    --hash=sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab \
-    --hash=sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26 \
-    --hash=sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2 \
-    --hash=sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db \
-    --hash=sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f \
-    --hash=sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5 \
-    --hash=sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99 \
-    --hash=sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c \
-    --hash=sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d \
-    --hash=sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811 \
-    --hash=sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa \
-    --hash=sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a \
-    --hash=sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03 \
-    --hash=sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b \
-    --hash=sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04 \
-    --hash=sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c \
-    --hash=sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001 \
-    --hash=sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458 \
-    --hash=sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389 \
-    --hash=sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99 \
-    --hash=sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985 \
-    --hash=sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537 \
-    --hash=sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238 \
-    --hash=sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f \
-    --hash=sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d \
-    --hash=sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796 \
-    --hash=sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a \
-    --hash=sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143 \
-    --hash=sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8 \
-    --hash=sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c \
-    --hash=sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5 \
-    --hash=sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5 \
-    --hash=sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711 \
-    --hash=sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4 \
-    --hash=sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6 \
-    --hash=sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c \
-    --hash=sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7 \
-    --hash=sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4 \
-    --hash=sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b \
-    --hash=sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae \
-    --hash=sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12 \
-    --hash=sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c \
-    --hash=sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae \
-    --hash=sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8 \
-    --hash=sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887 \
-    --hash=sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b \
-    --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
-    --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
-    --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
-    --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
-    --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
-    --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
-    # via requests
-click==8.1.7 \
-    --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
-    --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
-    # via mkdocs
-colorama==0.4.6 \
-    --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
-    --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-    # via mkdocs-material
-ghp-import==2.1.0 \
-    --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
-    --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
-    # via mkdocs
-gitdb==4.0.11 \
-    --hash=sha256:81a3407ddd2ee8df444cbacea00e2d038e40150acfa3001696fe0dcf1d3adfa4 \
-    --hash=sha256:bf5421126136d6d0af55bc1e7c1af1c397a34f5b7bd79e776cd3e89785c2b04b
-    # via gitpython
-gitpython==3.1.42 \
-    --hash=sha256:1bf9cd7c9e7255f77778ea54359e54ac22a72a5b51288c457c881057b7bb9ecd \
-    --hash=sha256:2d99869e0fef71a73cbd242528105af1d6c1b108c60dfabd994bf292f76c3ceb
-    # via mkdocs-git-revision-date-plugin
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
-    # via requests
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
+    # via django
+backports-zoneinfo==0.2.1 \
+    --hash=sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf \
+    --hash=sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328 \
+    --hash=sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546 \
+    --hash=sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6 \
+    --hash=sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570 \
+    --hash=sha256:7b0a64cda4145548fed9efc10322770f929b944ce5cee6c0dfe0c87bf4c0c8c9 \
+    --hash=sha256:8439c030a11780786a2002261569bdf362264f605dfa4d65090b64b05c9f79a7 \
+    --hash=sha256:8961c0f32cd0336fb8e8ead11a1f8cd99ec07145ec2931122faaac1c8f7fd987 \
+    --hash=sha256:89a48c0d158a3cc3f654da4c2de1ceba85263fafb861b98b59040a5086259722 \
+    --hash=sha256:a76b38c52400b762e48131494ba26be363491ac4f9a04c1b7e92483d169f6582 \
+    --hash=sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc \
+    --hash=sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b \
+    --hash=sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1 \
+    --hash=sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08 \
+    --hash=sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac \
+    --hash=sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2
+    # via django
+chardet==5.2.0 \
+    --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
+    --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
+    # via reportlab
+cssselect2==0.7.0 \
+    --hash=sha256:1ccd984dab89fc68955043aca4e1b03e0cf29cad9880f6e28e3ba7a74b14aa5a \
+    --hash=sha256:fd23a65bfd444595913f02fc71f6b286c29261e354c41d722ca7a261a49b5969
+    # via svglib
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via
-    #   mkdocs
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-markdown==3.6 \
-    --hash=sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f \
-    --hash=sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224
+    #   -r requirements/requirements.in
+    #   django-filer
+    #   django-polymorphic
+    #   easy-thumbnails
+django-filer==3.1.1 \
+    --hash=sha256:126026a15a160561097e0c486839c4cf3076f4363065e287e692c9316d197a86 \
+    --hash=sha256:c58628155ace4bb9f10f6ea9cdf92049b5961bd2ef82c5a3b76f09091f8af50d
+    # via -r requirements/requirements.in
+django-polymorphic==3.1.0 \
+    --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
+    --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
+    # via django-filer
+easy-thumbnails[svg]==2.8.5 \
+    --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
+    --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
+    # via django-filer
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
+    # via svglib
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
-    #   mkdocs
-    #   mkdocs-material
-    #   pymdown-extensions
-markupsafe==2.1.5 \
-    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
-    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
-    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
-    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
-    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
-    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
-    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
-    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
-    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
-    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
-    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
-    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
-    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
-    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
-    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
-    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
-    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
-    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
-    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
-    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
-    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
-    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
-    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
-    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
-    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
-    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
-    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
-    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
-    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
-    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
-    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
-    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
-    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
-    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
-    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
-    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
-    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
-    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
-    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
-    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
-    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
-    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
-    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
-    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
-    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
-    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
-    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
-    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
-    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
-    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
-    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
-    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
-    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
-    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
-    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
-    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
-    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
-    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
-    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
-    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
+    #   easy-thumbnails
+    #   reportlab
+reportlab==4.1.0 \
+    --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
+    --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
-    #   jinja2
-    #   mkdocs
-mergedeep==1.3.4 \
-    --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
-    --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-    # via mkdocs
-mkdocs==1.5.3 \
-    --hash=sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1 \
-    --hash=sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2
+    #   easy-thumbnails
+    #   svglib
+sqlparse==0.4.4 \
+    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
+    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+    # via django
+svglib==1.5.1 \
+    --hash=sha256:3ae765d3a9409ee60c0fb4d24c2deb6a80617aa927054f5bcd7fc98f0695e587
+    # via easy-thumbnails
+tinycss2==1.2.1 \
+    --hash=sha256:2b80a96d41e7c3914b8cda8bc7f705a4d9c49275616e886103dd839dfc847847 \
+    --hash=sha256:8cff3a8f066c2ec677c06dbc7b45619804a6938478d9d73c284b29d14ecb0627
     # via
-    #   -r requirements/docs.in
-    #   mkdocs-git-revision-date-plugin
-    #   mkdocs-material
-mkdocs-git-revision-date-plugin==0.3.2 \
-    --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
-    # via -r requirements/docs.in
-mkdocs-material==9.5.15 \
-    --hash=sha256:39f03cca45e82bf54eb7456b5a18bd252eabfdd67f237a229471484a0a4d4635 \
-    --hash=sha256:e5c96dec3d19491de49ca643fc1dbb92b278e43cdb816c775bc47db77d9b62fb
-    # via -r requirements/docs.in
-mkdocs-material-extensions==1.3.1 \
-    --hash=sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443 \
-    --hash=sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31
-    # via mkdocs-material
-packaging==24.0 \
-    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
-    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
-    # via mkdocs
-paginate==0.5.6 \
-    --hash=sha256:5e6007b6a9398177a7e1648d04fdd9f8c9766a1a945bceac82f1929e8c78af2d
-    # via mkdocs-material
-pathspec==0.12.1 \
-    --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
-    --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
-    # via mkdocs
-platformdirs==4.2.0 \
-    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
-    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
-    # via mkdocs
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-    # via mkdocs-material
-pymdown-extensions==10.7.1 \
-    --hash=sha256:c70e146bdd83c744ffc766b4671999796aba18842b268510a329f7f64700d584 \
-    --hash=sha256:f5cc7000d7ff0d1ce9395d216017fa4df3dde800afb1fb72d1c7d3fd35e710f4
-    # via mkdocs-material
-python-dateutil==2.9.0.post0 \
-    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
-    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
-    # via ghp-import
-pyyaml==6.0.1 \
-    --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
-    --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
-    --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
-    --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
-    --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
-    --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
-    --hash=sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595 \
-    --hash=sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62 \
-    --hash=sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98 \
-    --hash=sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696 \
-    --hash=sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290 \
-    --hash=sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9 \
-    --hash=sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d \
-    --hash=sha256:49a183be227561de579b4a36efbb21b3eab9651dd81b1858589f796549873dd6 \
-    --hash=sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867 \
-    --hash=sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47 \
-    --hash=sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486 \
-    --hash=sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6 \
-    --hash=sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3 \
-    --hash=sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007 \
-    --hash=sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938 \
-    --hash=sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0 \
-    --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
-    --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
-    --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
-    --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
-    --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
-    --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
-    --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
-    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
-    --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
-    --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
-    --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
-    --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
-    --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
-    --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
-    --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
-    --hash=sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924 \
-    --hash=sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34 \
-    --hash=sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43 \
-    --hash=sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859 \
-    --hash=sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673 \
-    --hash=sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54 \
-    --hash=sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a \
-    --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
-    --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
-    --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
-    --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
-    --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
-    --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
-    --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
+    #   cssselect2
+    #   svglib
+typing-extensions==4.10.0 \
+    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
+    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+    # via asgiref
+webencodings==0.5.1 \
+    --hash=sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78 \
+    --hash=sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923
     # via
-    #   mkdocs
-    #   pymdown-extensions
-    #   pyyaml-env-tag
-pyyaml-env-tag==0.1 \
-    --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
-    --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
-    # via mkdocs
-regex==2023.12.25 \
-    --hash=sha256:0694219a1d54336fd0445ea382d49d36882415c0134ee1e8332afd1529f0baa5 \
-    --hash=sha256:086dd15e9435b393ae06f96ab69ab2d333f5d65cbe65ca5a3ef0ec9564dfe770 \
-    --hash=sha256:094ba386bb5c01e54e14434d4caabf6583334090865b23ef58e0424a6286d3dc \
-    --hash=sha256:09da66917262d9481c719599116c7dc0c321ffcec4b1f510c4f8a066f8768105 \
-    --hash=sha256:0ecf44ddf9171cd7566ef1768047f6e66975788258b1c6c6ca78098b95cf9a3d \
-    --hash=sha256:0fda75704357805eb953a3ee15a2b240694a9a514548cd49b3c5124b4e2ad01b \
-    --hash=sha256:11a963f8e25ab5c61348d090bf1b07f1953929c13bd2309a0662e9ff680763c9 \
-    --hash=sha256:150c39f5b964e4d7dba46a7962a088fbc91f06e606f023ce57bb347a3b2d4630 \
-    --hash=sha256:1b9d811f72210fa9306aeb88385b8f8bcef0dfbf3873410413c00aa94c56c2b6 \
-    --hash=sha256:1e0eabac536b4cc7f57a5f3d095bfa557860ab912f25965e08fe1545e2ed8b4c \
-    --hash=sha256:22a86d9fff2009302c440b9d799ef2fe322416d2d58fc124b926aa89365ec482 \
-    --hash=sha256:22f3470f7524b6da61e2020672df2f3063676aff444db1daa283c2ea4ed259d6 \
-    --hash=sha256:263ef5cc10979837f243950637fffb06e8daed7f1ac1e39d5910fd29929e489a \
-    --hash=sha256:283fc8eed679758de38fe493b7d7d84a198b558942b03f017b1f94dda8efae80 \
-    --hash=sha256:29171aa128da69afdf4bde412d5bedc335f2ca8fcfe4489038577d05f16181e5 \
-    --hash=sha256:298dc6354d414bc921581be85695d18912bea163a8b23cac9a2562bbcd5088b1 \
-    --hash=sha256:2aae8101919e8aa05ecfe6322b278f41ce2994c4a430303c4cd163fef746e04f \
-    --hash=sha256:2f4e475a80ecbd15896a976aa0b386c5525d0ed34d5c600b6d3ebac0a67c7ddf \
-    --hash=sha256:34e4af5b27232f68042aa40a91c3b9bb4da0eeb31b7632e0091afc4310afe6cb \
-    --hash=sha256:37f8e93a81fc5e5bd8db7e10e62dc64261bcd88f8d7e6640aaebe9bc180d9ce2 \
-    --hash=sha256:3a17d3ede18f9cedcbe23d2daa8a2cd6f59fe2bf082c567e43083bba3fb00347 \
-    --hash=sha256:3b1de218d5375cd6ac4b5493e0b9f3df2be331e86520f23382f216c137913d20 \
-    --hash=sha256:43f7cd5754d02a56ae4ebb91b33461dc67be8e3e0153f593c509e21d219c5060 \
-    --hash=sha256:4558410b7a5607a645e9804a3e9dd509af12fb72b9825b13791a37cd417d73a5 \
-    --hash=sha256:4719bb05094d7d8563a450cf8738d2e1061420f79cfcc1fa7f0a44744c4d8f73 \
-    --hash=sha256:4bfc2b16e3ba8850e0e262467275dd4d62f0d045e0e9eda2bc65078c0110a11f \
-    --hash=sha256:518440c991f514331f4850a63560321f833979d145d7d81186dbe2f19e27ae3d \
-    --hash=sha256:51f4b32f793812714fd5307222a7f77e739b9bc566dc94a18126aba3b92b98a3 \
-    --hash=sha256:531ac6cf22b53e0696f8e1d56ce2396311254eb806111ddd3922c9d937151dae \
-    --hash=sha256:5cd05d0f57846d8ba4b71d9c00f6f37d6b97d5e5ef8b3c3840426a475c8f70f4 \
-    --hash=sha256:5dd58946bce44b53b06d94aa95560d0b243eb2fe64227cba50017a8d8b3cd3e2 \
-    --hash=sha256:60080bb3d8617d96f0fb7e19796384cc2467447ef1c491694850ebd3670bc457 \
-    --hash=sha256:636ba0a77de609d6510235b7f0e77ec494d2657108f777e8765efc060094c98c \
-    --hash=sha256:67d3ccfc590e5e7197750fcb3a2915b416a53e2de847a728cfa60141054123d4 \
-    --hash=sha256:68191f80a9bad283432385961d9efe09d783bcd36ed35a60fb1ff3f1ec2efe87 \
-    --hash=sha256:7502534e55c7c36c0978c91ba6f61703faf7ce733715ca48f499d3dbbd7657e0 \
-    --hash=sha256:7aa47c2e9ea33a4a2a05f40fcd3ea36d73853a2aae7b4feab6fc85f8bf2c9704 \
-    --hash=sha256:7d2af3f6b8419661a0c421584cfe8aaec1c0e435ce7e47ee2a97e344b98f794f \
-    --hash=sha256:7e316026cc1095f2a3e8cc012822c99f413b702eaa2ca5408a513609488cb62f \
-    --hash=sha256:88ad44e220e22b63b0f8f81f007e8abbb92874d8ced66f32571ef8beb0643b2b \
-    --hash=sha256:88d1f7bef20c721359d8675f7d9f8e414ec5003d8f642fdfd8087777ff7f94b5 \
-    --hash=sha256:89723d2112697feaa320c9d351e5f5e7b841e83f8b143dba8e2d2b5f04e10923 \
-    --hash=sha256:8a0ccf52bb37d1a700375a6b395bff5dd15c50acb745f7db30415bae3c2b0715 \
-    --hash=sha256:8c2c19dae8a3eb0ea45a8448356ed561be843b13cbc34b840922ddf565498c1c \
-    --hash=sha256:905466ad1702ed4acfd67a902af50b8db1feeb9781436372261808df7a2a7bca \
-    --hash=sha256:9852b76ab558e45b20bf1893b59af64a28bd3820b0c2efc80e0a70a4a3ea51c1 \
-    --hash=sha256:98a2636994f943b871786c9e82bfe7883ecdaba2ef5df54e1450fa9869d1f756 \
-    --hash=sha256:9aa1a67bbf0f957bbe096375887b2505f5d8ae16bf04488e8b0f334c36e31360 \
-    --hash=sha256:9eda5f7a50141291beda3edd00abc2d4a5b16c29c92daf8d5bd76934150f3edc \
-    --hash=sha256:a6d1047952c0b8104a1d371f88f4ab62e6275567d4458c1e26e9627ad489b445 \
-    --hash=sha256:a9b6d73353f777630626f403b0652055ebfe8ff142a44ec2cf18ae470395766e \
-    --hash=sha256:a9cc99d6946d750eb75827cb53c4371b8b0fe89c733a94b1573c9dd16ea6c9e4 \
-    --hash=sha256:ad83e7545b4ab69216cef4cc47e344d19622e28aabec61574b20257c65466d6a \
-    --hash=sha256:b014333bd0217ad3d54c143de9d4b9a3ca1c5a29a6d0d554952ea071cff0f1f8 \
-    --hash=sha256:b43523d7bc2abd757119dbfb38af91b5735eea45537ec6ec3a5ec3f9562a1c53 \
-    --hash=sha256:b521dcecebc5b978b447f0f69b5b7f3840eac454862270406a39837ffae4e697 \
-    --hash=sha256:b77e27b79448e34c2c51c09836033056a0547aa360c45eeeb67803da7b0eedaf \
-    --hash=sha256:b7a635871143661feccce3979e1727c4e094f2bdfd3ec4b90dfd4f16f571a87a \
-    --hash=sha256:b7fca9205b59c1a3d5031f7e64ed627a1074730a51c2a80e97653e3e9fa0d415 \
-    --hash=sha256:ba1b30765a55acf15dce3f364e4928b80858fa8f979ad41f862358939bdd1f2f \
-    --hash=sha256:ba99d8077424501b9616b43a2d208095746fb1284fc5ba490139651f971d39d9 \
-    --hash=sha256:c25a8ad70e716f96e13a637802813f65d8a6760ef48672aa3502f4c24ea8b400 \
-    --hash=sha256:c3c4a78615b7762740531c27cf46e2f388d8d727d0c0c739e72048beb26c8a9d \
-    --hash=sha256:c40281f7d70baf6e0db0c2f7472b31609f5bc2748fe7275ea65a0b4601d9b392 \
-    --hash=sha256:c7ad32824b7f02bb3c9f80306d405a1d9b7bb89362d68b3c5a9be53836caebdb \
-    --hash=sha256:cb3fe77aec8f1995611f966d0c656fdce398317f850d0e6e7aebdfe61f40e1cd \
-    --hash=sha256:cc038b2d8b1470364b1888a98fd22d616fba2b6309c5b5f181ad4483e0017861 \
-    --hash=sha256:cc37b9aeebab425f11f27e5e9e6cf580be7206c6582a64467a14dda211abc232 \
-    --hash=sha256:cc6bb9aa69aacf0f6032c307da718f61a40cf970849e471254e0e91c56ffca95 \
-    --hash=sha256:d126361607b33c4eb7b36debc173bf25d7805847346dd4d99b5499e1fef52bc7 \
-    --hash=sha256:d15b274f9e15b1a0b7a45d2ac86d1f634d983ca40d6b886721626c47a400bf39 \
-    --hash=sha256:d166eafc19f4718df38887b2bbe1467a4f74a9830e8605089ea7a30dd4da8887 \
-    --hash=sha256:d498eea3f581fbe1b34b59c697512a8baef88212f92e4c7830fcc1499f5b45a5 \
-    --hash=sha256:d6f7e255e5fa94642a0724e35406e6cb7001c09d476ab5fce002f652b36d0c39 \
-    --hash=sha256:d78bd484930c1da2b9679290a41cdb25cc127d783768a0369d6b449e72f88beb \
-    --hash=sha256:d865984b3f71f6d0af64d0d88f5733521698f6c16f445bb09ce746c92c97c586 \
-    --hash=sha256:d902a43085a308cef32c0d3aea962524b725403fd9373dea18110904003bac97 \
-    --hash=sha256:d94a1db462d5690ebf6ae86d11c5e420042b9898af5dcf278bd97d6bda065423 \
-    --hash=sha256:da695d75ac97cb1cd725adac136d25ca687da4536154cdc2815f576e4da11c69 \
-    --hash=sha256:db2a0b1857f18b11e3b0e54ddfefc96af46b0896fb678c85f63fb8c37518b3e7 \
-    --hash=sha256:df26481f0c7a3f8739fecb3e81bc9da3fcfae34d6c094563b9d4670b047312e1 \
-    --hash=sha256:e14b73607d6231f3cc4622809c196b540a6a44e903bcfad940779c80dffa7be7 \
-    --hash=sha256:e2610e9406d3b0073636a3a2e80db05a02f0c3169b5632022b4e81c0364bcda5 \
-    --hash=sha256:e692296c4cc2873967771345a876bcfc1c547e8dd695c6b89342488b0ea55cd8 \
-    --hash=sha256:e693e233ac92ba83a87024e1d32b5f9ab15ca55ddd916d878146f4e3406b5c91 \
-    --hash=sha256:e81469f7d01efed9b53740aedd26085f20d49da65f9c1f41e822a33992cb1590 \
-    --hash=sha256:e8c7e08bb566de4faaf11984af13f6bcf6a08f327b13631d41d62592681d24fe \
-    --hash=sha256:ed19b3a05ae0c97dd8f75a5d8f21f7723a8c33bbc555da6bbe1f96c470139d3c \
-    --hash=sha256:efb2d82f33b2212898f1659fb1c2e9ac30493ac41e4d53123da374c3b5541e64 \
-    --hash=sha256:f44dd4d68697559d007462b0a3a1d9acd61d97072b71f6d1968daef26bc744bd \
-    --hash=sha256:f72cbae7f6b01591f90814250e636065850c5926751af02bb48da94dfced7baa \
-    --hash=sha256:f7bc09bc9c29ebead055bcba136a67378f03d66bf359e87d0f7c759d6d4ffa31 \
-    --hash=sha256:ff100b203092af77d1a5a7abe085b3506b7eaaf9abf65b73b7d6905b6cb76988
-    # via mkdocs-material
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
-    # via mkdocs-material
-six==1.16.0 \
-    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
-    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-    # via python-dateutil
-smmap==5.0.1 \
-    --hash=sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62 \
-    --hash=sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da
-    # via gitdb
-urllib3==2.2.1 \
-    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
-    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
-    # via requests
-watchdog==4.0.0 \
-    --hash=sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257 \
-    --hash=sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca \
-    --hash=sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b \
-    --hash=sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85 \
-    --hash=sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b \
-    --hash=sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19 \
-    --hash=sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50 \
-    --hash=sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92 \
-    --hash=sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269 \
-    --hash=sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f \
-    --hash=sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c \
-    --hash=sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b \
-    --hash=sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87 \
-    --hash=sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b \
-    --hash=sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b \
-    --hash=sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8 \
-    --hash=sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c \
-    --hash=sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3 \
-    --hash=sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7 \
-    --hash=sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605 \
-    --hash=sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935 \
-    --hash=sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b \
-    --hash=sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927 \
-    --hash=sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101 \
-    --hash=sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07 \
-    --hash=sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec \
-    --hash=sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4 \
-    --hash=sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245 \
-    --hash=sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d
-    # via mkdocs
+    #   cssselect2
+    #   tinycss2
```

### Comparing `django-sites-extra-0.1.1/requirements/py310-django32.txt` & `django-sites-extra-0.1.2/requirements/py310-django42.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
     --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via reportlab
 cssselect2==0.7.0 \
     --hash=sha256:1ccd984dab89fc68955043aca4e1b03e0cf29cad9880f6e28e3ba7a74b14aa5a \
     --hash=sha256:fd23a65bfd444595913f02fc71f6b286c29261e354c41d722ca7a261a49b5969
     # via svglib
-django==3.2.25 \
-    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
-    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via
     #   -r requirements/requirements.in
     #   django-filer
     #   django-polymorphic
     #   easy-thumbnails
 django-filer==3.1.1 \
     --hash=sha256:126026a15a160561097e0c486839c4cf3076f4363065e287e692c9316d197a86 \
@@ -32,166 +32,244 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
-pytz==2024.1 \
-    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
-    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
-    # via django
 reportlab==4.1.0 \
     --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
     --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
     #   easy-thumbnails
     #   svglib
 sqlparse==0.4.4 \
```

### Comparing `django-sites-extra-0.1.1/requirements/py310-django42.txt` & `django-sites-extra-0.1.2/requirements/py39-django42.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
@@ -32,159 +32,241 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
 reportlab==4.1.0 \
     --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
     --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
```

### Comparing `django-sites-extra-0.1.1/requirements/py311-django32.txt` & `django-sites-extra-0.1.2/requirements/py311-django42.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
     --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via reportlab
 cssselect2==0.7.0 \
     --hash=sha256:1ccd984dab89fc68955043aca4e1b03e0cf29cad9880f6e28e3ba7a74b14aa5a \
     --hash=sha256:fd23a65bfd444595913f02fc71f6b286c29261e354c41d722ca7a261a49b5969
     # via svglib
-django==3.2.25 \
-    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
-    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via
     #   -r requirements/requirements.in
     #   django-filer
     #   django-polymorphic
     #   easy-thumbnails
 django-filer==3.1.1 \
     --hash=sha256:126026a15a160561097e0c486839c4cf3076f4363065e287e692c9316d197a86 \
@@ -32,166 +32,244 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
-pytz==2024.1 \
-    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
-    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
-    # via django
 reportlab==4.1.0 \
     --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
     --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
     #   easy-thumbnails
     #   svglib
 sqlparse==0.4.4 \
```

### Comparing `django-sites-extra-0.1.1/requirements/py311-django42.txt` & `django-sites-extra-0.1.2/requirements/py311-django32.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
     --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via reportlab
 cssselect2==0.7.0 \
     --hash=sha256:1ccd984dab89fc68955043aca4e1b03e0cf29cad9880f6e28e3ba7a74b14aa5a \
     --hash=sha256:fd23a65bfd444595913f02fc71f6b286c29261e354c41d722ca7a261a49b5969
     # via svglib
-django==4.2.11 \
-    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
-    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
+django==3.2.25 \
+    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
+    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
     # via
     #   -r requirements/requirements.in
     #   django-filer
     #   django-polymorphic
     #   easy-thumbnails
 django-filer==3.1.1 \
     --hash=sha256:126026a15a160561097e0c486839c4cf3076f4363065e287e692c9316d197a86 \
@@ -32,162 +32,248 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
+pytz==2024.1 \
+    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
+    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
+    # via django
 reportlab==4.1.0 \
     --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
     --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
     #   easy-thumbnails
     #   svglib
 sqlparse==0.4.4 \
```

### Comparing `django-sites-extra-0.1.1/requirements/py38-django32.txt` & `django-sites-extra-0.1.2/requirements/py310-django32.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
@@ -32,159 +32,241 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
```

### Comparing `django-sites-extra-0.1.1/requirements/py38-django42.txt` & `django-sites-extra-0.1.2/requirements/py39-django32.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,28 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-backports-zoneinfo==0.2.1 \
-    --hash=sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf \
-    --hash=sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328 \
-    --hash=sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546 \
-    --hash=sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6 \
-    --hash=sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570 \
-    --hash=sha256:7b0a64cda4145548fed9efc10322770f929b944ce5cee6c0dfe0c87bf4c0c8c9 \
-    --hash=sha256:8439c030a11780786a2002261569bdf362264f605dfa4d65090b64b05c9f79a7 \
-    --hash=sha256:8961c0f32cd0336fb8e8ead11a1f8cd99ec07145ec2931122faaac1c8f7fd987 \
-    --hash=sha256:89a48c0d158a3cc3f654da4c2de1ceba85263fafb861b98b59040a5086259722 \
-    --hash=sha256:a76b38c52400b762e48131494ba26be363491ac4f9a04c1b7e92483d169f6582 \
-    --hash=sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc \
-    --hash=sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b \
-    --hash=sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1 \
-    --hash=sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08 \
-    --hash=sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac \
-    --hash=sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2
-    # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
     --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via reportlab
 cssselect2==0.7.0 \
     --hash=sha256:1ccd984dab89fc68955043aca4e1b03e0cf29cad9880f6e28e3ba7a74b14aa5a \
     --hash=sha256:fd23a65bfd444595913f02fc71f6b286c29261e354c41d722ca7a261a49b5969
     # via svglib
-django==4.2.11 \
-    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
-    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
+django==3.2.25 \
+    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
+    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
     # via
     #   -r requirements/requirements.in
     #   django-filer
     #   django-polymorphic
     #   easy-thumbnails
 django-filer==3.1.1 \
     --hash=sha256:126026a15a160561097e0c486839c4cf3076f4363065e287e692c9316d197a86 \
@@ -50,162 +32,248 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
+pytz==2024.1 \
+    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
+    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
+    # via django
 reportlab==4.1.0 \
     --hash=sha256:28a40d5000afbd8ccae15a47f7abe2841768461354bede1a9d42841132997c98 \
     --hash=sha256:3a99faf412691159c068b3ff01c15307ce2fd2cf6b860199434874e002040a84
     # via
     #   easy-thumbnails
     #   svglib
 sqlparse==0.4.4 \
```

### Comparing `django-sites-extra-0.1.1/requirements/py39-django32.txt` & `django-sites-extra-0.1.2/requirements/py38-django32.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
@@ -32,159 +32,241 @@
     --hash=sha256:08bc4f4f4a773a19b2deced5a56deddd1ef56ebd15207bf4052e2901c25ef57e \
     --hash=sha256:d6955b5308bf6e41dcb22ba7c96f00b51dfa497a8a5ab1e9c06c7951bf417bf8
     # via django-filer
 easy-thumbnails[svg]==2.8.5 \
     --hash=sha256:7e4e912609fc9b60b3a1fef6557ec15ddf9c4f946267a92e6920dfd4dd765e35 \
     --hash=sha256:97f5a5278d8b6c1f5b1b7473f3737d29b18f5c1159cbdf0ab28674fdac2f8c87
     # via django-filer
-lxml==5.1.1 \
-    --hash=sha256:036b36c48cd775e4fd2084b34ae62ffeefa7a01f955f5a5b816f9257c308cfc0 \
-    --hash=sha256:04ef231dde88294a5499f61a74cdc42af97d8d5ecec1b0a645d1c7d436942789 \
-    --hash=sha256:071e5123d1eca861708c4be5b54e4d88923fa33fab3aa02722e907518b07071c \
-    --hash=sha256:0e46181d15fae102c53621bed9356b7a599a1e837b978c934a350dd00842b1d9 \
-    --hash=sha256:13b73d78a8023203722cf98e9ea0b222da83110d1d5ef437ef8782a7755b4586 \
-    --hash=sha256:1528b37e83c3aeecb438e76e5be6279b353275560125a9c3f4d74642c5f110f9 \
-    --hash=sha256:161838cb95c97e8d76d01e544a3570b52ab6b863f4897a90e1f073bb110a75ba \
-    --hash=sha256:19c6bc7476eeac4598ff925ae98597610109e21af4cd7ab1e060efcfc4b1c6e2 \
-    --hash=sha256:1b0611bba10d6f5467b86673e8f6bba4de0d00f7d111eea843bc872abfe11b5c \
-    --hash=sha256:1d0270d33fbde6e1c6758ff58e2e284144f5331aa05dfe7f44ceafdf4e9d31aa \
-    --hash=sha256:1d380f183bd03ab827899753ea96dabe27d2025eb0bfd4f2ac0eee4afa0f351d \
-    --hash=sha256:20cd17eb21f5ae54da96791c49e1fbd3327bf66b2c00556cdf8d0552c2270f92 \
-    --hash=sha256:26974096654241df08a30dc2eb0e139c1ad5653660aa4b2ced66000230e96c14 \
-    --hash=sha256:2992480a25434d2df31413136ef87effab14d43b07f1f54c5012c4f6c7530144 \
-    --hash=sha256:29b2771b4eec4e85063f10294facdd9829d010e6cc9668040d0cf936dc56733a \
-    --hash=sha256:2de00750318ae6869b9dfa6429a4f82b8ecad043049414547474d09db549c2ee \
-    --hash=sha256:318847c165063549c8fda6b162a0d068689b10deb825cb3859caef69fddaaaff \
-    --hash=sha256:3641bc124b037921de4220538a5ebb52354fd2799fc2bbfb335d28096063c7d6 \
-    --hash=sha256:3a6e9b34f59c9755aa279c652e1c48c333c665d05a88afcd8e5ff0bde86f3b14 \
-    --hash=sha256:3c5940f188189956ccb3d1adb413001ada79f2d2b81087d2612a0cc4a1197eed \
-    --hash=sha256:3da8db291568c27b2bb248dcfc8838ca3149f373a24e204bcd1c2c89e2813d14 \
-    --hash=sha256:42a8aa957e98bd8b884a8142175ec24ce4ef0a57760e8879f193bfe64b757ca9 \
-    --hash=sha256:43f21b5929185fa4560836942020bb00a0fcdec9f67be98cac1a4b99501757c1 \
-    --hash=sha256:48dd28b9f410329de709a4bb6169c58f2cd8bff25f5a48d647678ec9b8a40c65 \
-    --hash=sha256:4958c378d9387c45ef8c4859495cf6be76f863e4e3b31494f6ec7f2c48d3b8e3 \
-    --hash=sha256:50007f4e94dc4e38030487a8b6c4af87a2d51ed059c7b74b29e3dd937cb1dfe1 \
-    --hash=sha256:5020b3081030b5cfc8149eee231167aea4ff68df73a610e1d542809e1f11fde7 \
-    --hash=sha256:52358249292bc155af681a9240ec3d944c1195f0124aa10ec4e3635adc1e10a1 \
-    --hash=sha256:55e13a19829dcdbf0c5233062977aeb6daf72e65124909128045976f659164e8 \
-    --hash=sha256:56f1e813ff660d031c77edba90a068d57e47ae93a9e811330fc88946fa68af9a \
-    --hash=sha256:59ca75cfcf646ff64aa19ca4e7fd2a0fde77268d5a87856525d9e0b69b77d0c4 \
-    --hash=sha256:5bd2595ebe95214446e00a1ab94571f778b126e17736ea222c07505c4e092289 \
-    --hash=sha256:5dcb373720b70aa05419e508265dd86f06886ca0388967f6f024fbc4d551379f \
-    --hash=sha256:60ceffdca5d637fe8ee95c7f06733a6c9646e07da80997efe3af2d4b4f366e36 \
-    --hash=sha256:666432274881cb2535e71dbe745e08ef10fe25c81fbb1a6b1e3c973177823b0c \
-    --hash=sha256:68eed33377a9925aed7ba56c8611d50aaa1e45638c07a92b4b4b0a0436cc2dd2 \
-    --hash=sha256:6c49eb5deaed1990fde5b5d80d6800aec1b5fd6113346b5f11068d988f68f2c4 \
-    --hash=sha256:74d0967c6f91eec6fe91159f9e8ccb3720fa0fbf9f462109c7bef62550df397c \
-    --hash=sha256:77425482e4311d1cff119a2b5ab26c52ec209d2a3d728a54db3223ab91995e20 \
-    --hash=sha256:77842b79b63c83c04dcfe2f045c78e15e4d97c86838eabd2e6518c1ed97e3900 \
-    --hash=sha256:81107c8de3e463052ae8fd05fd31b97c371c7a9ce4a189b8bb5f45b0b3545fb9 \
-    --hash=sha256:87b67d8620c2725d666e5d88ddba56bcdb1f52211a2e7d22f951b67c35f7f627 \
-    --hash=sha256:8a943826e7a9254eed661a7134fcde3c832a9fecd989d0f47c6e08c7b769cb2c \
-    --hash=sha256:906966babd374fdfe46e130fc656488003f0d0d63b7cba612aa5a796c8804283 \
-    --hash=sha256:9113fe65a62f834b8e994c8f48e7b2179bf81878c0ec80ad7feba51ab9417663 \
-    --hash=sha256:95a51324a55000c55f4ab79e1f7f1e0bc42b7a24e39633f79542753023a9d4b7 \
-    --hash=sha256:99bcdf665576a26b44c7ce767d76b769a4418b0a13cda8300b26fb7b2647bd5b \
-    --hash=sha256:9c03f3715c68fc707d9383d56e482d95d198ba07cb3dad4aee9e5a5ca06b2536 \
-    --hash=sha256:9cc30dc3c49ea914fa62ea73b57198b541cf2cd522fcf2b9559f99a24df769bb \
-    --hash=sha256:a02ed1ebc469734dbfed5b688f709334de19e7a333cba7ae187b17d2b2c1d4ff \
-    --hash=sha256:a103426e809640a2d985062d2f4b28db2f0fe4469ff72a67cb31fa70613158f1 \
-    --hash=sha256:a305d0469177fd78a0a9aa2231c60218266bb85d4b7955f9b67dab628c9267fd \
-    --hash=sha256:a76a7b35e7660c74eb3f943c19f5f78c882dceab890cf8017027b6100b79ad8e \
-    --hash=sha256:a94a97380ad689d751eb0a1e1ccd2a0622c5141771a31abe9a16075f80027e95 \
-    --hash=sha256:acff17e0cd5344677757a152631d8411efac6a84e4476d60123a9b33f5d6c511 \
-    --hash=sha256:adedfb61be862f48907218e3a24bf051fd2ecca53358f3958b0bdb17d7881c20 \
-    --hash=sha256:adff469b7dbfe9f3babc9e4479449ee97085ba70ac492fbe5f0f7217940c6731 \
-    --hash=sha256:aff34295a6c87638a1f1905355cf3a97e4026c45c0cf3bb6ed6bc35b885b4a33 \
-    --hash=sha256:b174885fd2cabd1ad48585296f495e25d607f02db99668c08b2afaceb668e21b \
-    --hash=sha256:bc6904519dd1f92eb82f7d49814a33bbc444d0b66b1438e76daf3f79ef4aa38f \
-    --hash=sha256:bd46b5b19ac969de8e87fb3d04414641d12ee489e2ea6cc75344087829b31c63 \
-    --hash=sha256:bf7e57dbe7b3c605e63849d9c8dae246a6ab9002223c57cd3f3dec7c3a0a8e6d \
-    --hash=sha256:bfbdadc3cfe552331ecb0bbdcabf148d1697c73aa4321151e0e6c1704eeb76a7 \
-    --hash=sha256:c7c1d2f6e9c7a1c4478146ee38d16dbe0eb3be998424bc0f01346c671c38b86d \
-    --hash=sha256:d1abbf2249467a37da45fb2d7ff37e578dfc9813f142800e58db9da761cb7899 \
-    --hash=sha256:d1f4d37b3f8d2d44493edce3d65ac987127bababd8ae208a6f0d7d260852346e \
-    --hash=sha256:d26243d994d4077a50056e9008848e5b421be0c6f0fd4e932a9463e1d89fc42b \
-    --hash=sha256:d55ddc73dec971277b181a6d1a6abdd34f50e4511e1e60f6b4ebe22cbaad05bb \
-    --hash=sha256:d9358f7268c161dc0a1c3216018f26c04954b5dd47ba6dead79da6598f4725d4 \
-    --hash=sha256:d94a28c16cc430b68c374b37b8bb536ba5f0a4a080be0e1daa8310c44a00a75c \
-    --hash=sha256:dec3491aa69a91ed07f5e6bc033e2b1a9424447ad5312ee69ac973e94d79083a \
-    --hash=sha256:f05ab8cea65363d0cc7ce818f42407504b6d94ca885b4cde0270f021e2f4ef61 \
-    --hash=sha256:f1d0824e3ddb969fe1337b1bc45cf0bec8095b342f36903f41a74b7769cc8c73 \
-    --hash=sha256:f8682af96b5ad5093aab9eee5e4ff24cb7a9796c78699d914dd456ebfe7484a6
+lxml==5.2.1 \
+    --hash=sha256:04ab5415bf6c86e0518d57240a96c4d1fcfc3cb370bb2ac2a732b67f579e5a04 \
+    --hash=sha256:057cdc6b86ab732cf361f8b4d8af87cf195a1f6dc5b0ff3de2dced242c2015e0 \
+    --hash=sha256:058a1308914f20784c9f4674036527e7c04f7be6fb60f5d61353545aa7fcb739 \
+    --hash=sha256:08802f0c56ed150cc6885ae0788a321b73505d2263ee56dad84d200cab11c07a \
+    --hash=sha256:0a15438253b34e6362b2dc41475e7f80de76320f335e70c5528b7148cac253a1 \
+    --hash=sha256:0c3f67e2aeda739d1cc0b1102c9a9129f7dc83901226cc24dd72ba275ced4218 \
+    --hash=sha256:0e7259016bc4345a31af861fdce942b77c99049d6c2107ca07dc2bba2435c1d9 \
+    --hash=sha256:0ed777c1e8c99b63037b91f9d73a6aad20fd035d77ac84afcc205225f8f41188 \
+    --hash=sha256:0f5d65c39f16717a47c36c756af0fb36144069c4718824b7533f803ecdf91138 \
+    --hash=sha256:0f8c09ed18ecb4ebf23e02b8e7a22a05d6411911e6fabef3a36e4f371f4f2585 \
+    --hash=sha256:11a04306fcba10cd9637e669fd73aa274c1c09ca64af79c041aa820ea992b637 \
+    --hash=sha256:1ae67b4e737cddc96c99461d2f75d218bdf7a0c3d3ad5604d1f5e7464a2f9ffe \
+    --hash=sha256:1c5bb205e9212d0ebddf946bc07e73fa245c864a5f90f341d11ce7b0b854475d \
+    --hash=sha256:1f7785f4f789fdb522729ae465adcaa099e2a3441519df750ebdccc481d961a1 \
+    --hash=sha256:200e63525948e325d6a13a76ba2911f927ad399ef64f57898cf7c74e69b71095 \
+    --hash=sha256:21c2e6b09565ba5b45ae161b438e033a86ad1736b8c838c766146eff8ceffff9 \
+    --hash=sha256:2213afee476546a7f37c7a9b4ad4d74b1e112a6fafffc9185d6d21f043128c81 \
+    --hash=sha256:27aa20d45c2e0b8cd05da6d4759649170e8dfc4f4e5ef33a34d06f2d79075d57 \
+    --hash=sha256:2a66bf12fbd4666dd023b6f51223aed3d9f3b40fef06ce404cb75bafd3d89536 \
+    --hash=sha256:2c9d147f754b1b0e723e6afb7ba1566ecb162fe4ea657f53d2139bbf894d050a \
+    --hash=sha256:2ddfe41ddc81f29a4c44c8ce239eda5ade4e7fc305fb7311759dd6229a080052 \
+    --hash=sha256:31e9a882013c2f6bd2f2c974241bf4ba68c85eba943648ce88936d23209a2e01 \
+    --hash=sha256:3249cc2989d9090eeac5467e50e9ec2d40704fea9ab72f36b034ea34ee65ca98 \
+    --hash=sha256:3545039fa4779be2df51d6395e91a810f57122290864918b172d5dc7ca5bb433 \
+    --hash=sha256:394ed3924d7a01b5bd9a0d9d946136e1c2f7b3dc337196d99e61740ed4bc6fe1 \
+    --hash=sha256:3a6b45da02336895da82b9d472cd274b22dc27a5cea1d4b793874eead23dd14f \
+    --hash=sha256:3a74c4f27167cb95c1d4af1c0b59e88b7f3e0182138db2501c353555f7ec57f4 \
+    --hash=sha256:3d0c3dd24bb4605439bf91068598d00c6370684f8de4a67c2992683f6c309d6b \
+    --hash=sha256:3dbe858ee582cbb2c6294dc85f55b5f19c918c2597855e950f34b660f1a5ede6 \
+    --hash=sha256:3dc773b2861b37b41a6136e0b72a1a44689a9c4c101e0cddb6b854016acc0aa8 \
+    --hash=sha256:3e183c6e3298a2ed5af9d7a356ea823bccaab4ec2349dc9ed83999fd289d14d5 \
+    --hash=sha256:3f7765e69bbce0906a7c74d5fe46d2c7a7596147318dbc08e4a2431f3060e306 \
+    --hash=sha256:417d14450f06d51f363e41cace6488519038f940676ce9664b34ebf5653433a5 \
+    --hash=sha256:44f6c7caff88d988db017b9b0e4ab04934f11e3e72d478031efc7edcac6c622f \
+    --hash=sha256:491755202eb21a5e350dae00c6d9a17247769c64dcf62d8c788b5c135e179dc4 \
+    --hash=sha256:4951e4f7a5680a2db62f7f4ab2f84617674d36d2d76a729b9a8be4b59b3659be \
+    --hash=sha256:52421b41ac99e9d91934e4d0d0fe7da9f02bfa7536bb4431b4c05c906c8c6919 \
+    --hash=sha256:530e7c04f72002d2f334d5257c8a51bf409db0316feee7c87e4385043be136af \
+    --hash=sha256:533658f8fbf056b70e434dff7e7aa611bcacb33e01f75de7f821810e48d1bb66 \
+    --hash=sha256:5670fb70a828663cc37552a2a85bf2ac38475572b0e9b91283dc09efb52c41d1 \
+    --hash=sha256:56c22432809085b3f3ae04e6e7bdd36883d7258fcd90e53ba7b2e463efc7a6af \
+    --hash=sha256:58278b29cb89f3e43ff3e0c756abbd1518f3ee6adad9e35b51fb101c1c1daaec \
+    --hash=sha256:588008b8497667f1ddca7c99f2f85ce8511f8f7871b4a06ceede68ab62dff64b \
+    --hash=sha256:59565f10607c244bc4c05c0c5fa0c190c990996e0c719d05deec7030c2aa8289 \
+    --hash=sha256:59689a75ba8d7ffca577aefd017d08d659d86ad4585ccc73e43edbfc7476781a \
+    --hash=sha256:5aea8212fb823e006b995c4dda533edcf98a893d941f173f6c9506126188860d \
+    --hash=sha256:5c670c0406bdc845b474b680b9a5456c561c65cf366f8db5a60154088c92d102 \
+    --hash=sha256:5ca1e8188b26a819387b29c3895c47a5e618708fe6f787f3b1a471de2c4a94d9 \
+    --hash=sha256:5d077bc40a1fe984e1a9931e801e42959a1e6598edc8a3223b061d30fbd26bbc \
+    --hash=sha256:5d5792e9b3fb8d16a19f46aa8208987cfeafe082363ee2745ea8b643d9cc5b45 \
+    --hash=sha256:5dd1537e7cc06efd81371f5d1a992bd5ab156b2b4f88834ca852de4a8ea523fa \
+    --hash=sha256:5ea7b6766ac2dfe4bcac8b8595107665a18ef01f8c8343f00710b85096d1b53a \
+    --hash=sha256:622020d4521e22fb371e15f580d153134bfb68d6a429d1342a25f051ec72df1c \
+    --hash=sha256:627402ad8dea044dde2eccde4370560a2b750ef894c9578e1d4f8ffd54000461 \
+    --hash=sha256:644df54d729ef810dcd0f7732e50e5ad1bd0a135278ed8d6bcb06f33b6b6f708 \
+    --hash=sha256:64641a6068a16201366476731301441ce93457eb8452056f570133a6ceb15fca \
+    --hash=sha256:64c2baa7774bc22dd4474248ba16fe1a7f611c13ac6123408694d4cc93d66dbd \
+    --hash=sha256:6588c459c5627fefa30139be4d2e28a2c2a1d0d1c265aad2ba1935a7863a4913 \
+    --hash=sha256:66bc5eb8a323ed9894f8fa0ee6cb3e3fb2403d99aee635078fd19a8bc7a5a5da \
+    --hash=sha256:68a2610dbe138fa8c5826b3f6d98a7cfc29707b850ddcc3e21910a6fe51f6ca0 \
+    --hash=sha256:6935bbf153f9a965f1e07c2649c0849d29832487c52bb4a5c5066031d8b44fd5 \
+    --hash=sha256:6992030d43b916407c9aa52e9673612ff39a575523c5f4cf72cdef75365709a5 \
+    --hash=sha256:6a014510830df1475176466b6087fc0c08b47a36714823e58d8b8d7709132a96 \
+    --hash=sha256:6ab833e4735a7e5533711a6ea2df26459b96f9eec36d23f74cafe03631647c41 \
+    --hash=sha256:6cc6ee342fb7fa2471bd9b6d6fdfc78925a697bf5c2bcd0a302e98b0d35bfad3 \
+    --hash=sha256:6cf58416653c5901e12624e4013708b6e11142956e7f35e7a83f1ab02f3fe456 \
+    --hash=sha256:70a9768e1b9d79edca17890175ba915654ee1725975d69ab64813dd785a2bd5c \
+    --hash=sha256:70ac664a48aa64e5e635ae5566f5227f2ab7f66a3990d67566d9907edcbbf867 \
+    --hash=sha256:71e97313406ccf55d32cc98a533ee05c61e15d11b99215b237346171c179c0b0 \
+    --hash=sha256:7221d49259aa1e5a8f00d3d28b1e0b76031655ca74bb287123ef56c3db92f213 \
+    --hash=sha256:74b28c6334cca4dd704e8004cba1955af0b778cf449142e581e404bd211fb619 \
+    --hash=sha256:764b521b75701f60683500d8621841bec41a65eb739b8466000c6fdbc256c240 \
+    --hash=sha256:78bfa756eab503673991bdcf464917ef7845a964903d3302c5f68417ecdc948c \
+    --hash=sha256:794f04eec78f1d0e35d9e0c36cbbb22e42d370dda1609fb03bcd7aeb458c6377 \
+    --hash=sha256:79bd05260359170f78b181b59ce871673ed01ba048deef4bf49a36ab3e72e80b \
+    --hash=sha256:7a7efd5b6d3e30d81ec68ab8a88252d7c7c6f13aaa875009fe3097eb4e30b84c \
+    --hash=sha256:7c17b64b0a6ef4e5affae6a3724010a7a66bda48a62cfe0674dabd46642e8b54 \
+    --hash=sha256:804f74efe22b6a227306dd890eecc4f8c59ff25ca35f1f14e7482bbce96ef10b \
+    --hash=sha256:853e074d4931dbcba7480d4dcab23d5c56bd9607f92825ab80ee2bd916edea53 \
+    --hash=sha256:857500f88b17a6479202ff5fe5f580fc3404922cd02ab3716197adf1ef628029 \
+    --hash=sha256:865bad62df277c04beed9478fe665b9ef63eb28fe026d5dedcb89b537d2e2ea6 \
+    --hash=sha256:88e22fc0a6684337d25c994381ed8a1580a6f5ebebd5ad41f89f663ff4ec2885 \
+    --hash=sha256:8b9c07e7a45bb64e21df4b6aa623cb8ba214dfb47d2027d90eac197329bb5e94 \
+    --hash=sha256:8de8f9d6caa7f25b204fc861718815d41cbcf27ee8f028c89c882a0cf4ae4134 \
+    --hash=sha256:8e77c69d5892cb5ba71703c4057091e31ccf534bd7f129307a4d084d90d014b8 \
+    --hash=sha256:9123716666e25b7b71c4e1789ec829ed18663152008b58544d95b008ed9e21e9 \
+    --hash=sha256:958244ad566c3ffc385f47dddde4145088a0ab893504b54b52c041987a8c1863 \
+    --hash=sha256:96323338e6c14e958d775700ec8a88346014a85e5de73ac7967db0367582049b \
+    --hash=sha256:9676bfc686fa6a3fa10cd4ae6b76cae8be26eb5ec6811d2a325636c460da1806 \
+    --hash=sha256:9b0ff53900566bc6325ecde9181d89afadc59c5ffa39bddf084aaedfe3b06a11 \
+    --hash=sha256:9b9ec9c9978b708d488bec36b9e4c94d88fd12ccac3e62134a9d17ddba910ea9 \
+    --hash=sha256:9c6ad0fbf105f6bcc9300c00010a2ffa44ea6f555df1a2ad95c88f5656104817 \
+    --hash=sha256:9ca66b8e90daca431b7ca1408cae085d025326570e57749695d6a01454790e95 \
+    --hash=sha256:9e2addd2d1866fe112bc6f80117bcc6bc25191c5ed1bfbcf9f1386a884252ae8 \
+    --hash=sha256:a0af35bd8ebf84888373630f73f24e86bf016642fb8576fba49d3d6b560b7cbc \
+    --hash=sha256:a2b44bec7adf3e9305ce6cbfa47a4395667e744097faed97abb4728748ba7d47 \
+    --hash=sha256:a2dfe7e2473f9b59496247aad6e23b405ddf2e12ef0765677b0081c02d6c2c0b \
+    --hash=sha256:a55ee573116ba208932e2d1a037cc4b10d2c1cb264ced2184d00b18ce585b2c0 \
+    --hash=sha256:a7baf9ffc238e4bf401299f50e971a45bfcc10a785522541a6e3179c83eabf0a \
+    --hash=sha256:a8d5c70e04aac1eda5c829a26d1f75c6e5286c74743133d9f742cda8e53b9c2f \
+    --hash=sha256:a91481dbcddf1736c98a80b122afa0f7296eeb80b72344d7f45dc9f781551f56 \
+    --hash=sha256:ab31a88a651039a07a3ae327d68ebdd8bc589b16938c09ef3f32a4b809dc96ef \
+    --hash=sha256:abc25c3cab9ec7fcd299b9bcb3b8d4a1231877e425c650fa1c7576c5107ab851 \
+    --hash=sha256:adfb84ca6b87e06bc6b146dc7da7623395db1e31621c4785ad0658c5028b37d7 \
+    --hash=sha256:afbbdb120d1e78d2ba8064a68058001b871154cc57787031b645c9142b937a62 \
+    --hash=sha256:afd5562927cdef7c4f5550374acbc117fd4ecc05b5007bdfa57cc5355864e0a4 \
+    --hash=sha256:b070bbe8d3f0f6147689bed981d19bbb33070225373338df755a46893528104a \
+    --hash=sha256:b0b58fbfa1bf7367dde8a557994e3b1637294be6cf2169810375caf8571a085c \
+    --hash=sha256:b560e3aa4b1d49e0e6c847d72665384db35b2f5d45f8e6a5c0072e0283430533 \
+    --hash=sha256:b6241d4eee5f89453307c2f2bfa03b50362052ca0af1efecf9fef9a41a22bb4f \
+    --hash=sha256:b6787b643356111dfd4032b5bffe26d2f8331556ecb79e15dacb9275da02866e \
+    --hash=sha256:bcbf4af004f98793a95355980764b3d80d47117678118a44a80b721c9913436a \
+    --hash=sha256:beb72935a941965c52990f3a32d7f07ce869fe21c6af8b34bf6a277b33a345d3 \
+    --hash=sha256:bf2e2458345d9bffb0d9ec16557d8858c9c88d2d11fed53998512504cd9df49b \
+    --hash=sha256:c2d35a1d047efd68027817b32ab1586c1169e60ca02c65d428ae815b593e65d4 \
+    --hash=sha256:c38d7b9a690b090de999835f0443d8aa93ce5f2064035dfc48f27f02b4afc3d0 \
+    --hash=sha256:c6f2c8372b98208ce609c9e1d707f6918cc118fea4e2c754c9f0812c04ca116d \
+    --hash=sha256:c817d420c60a5183953c783b0547d9eb43b7b344a2c46f69513d5952a78cddf3 \
+    --hash=sha256:c8ba129e6d3b0136a0f50345b2cb3db53f6bda5dd8c7f5d83fbccba97fb5dcb5 \
+    --hash=sha256:c94e75445b00319c1fad60f3c98b09cd63fe1134a8a953dcd48989ef42318534 \
+    --hash=sha256:cc4691d60512798304acb9207987e7b2b7c44627ea88b9d77489bbe3e6cc3bd4 \
+    --hash=sha256:cc518cea79fd1e2f6c90baafa28906d4309d24f3a63e801d855e7424c5b34144 \
+    --hash=sha256:cd53553ddad4a9c2f1f022756ae64abe16da1feb497edf4d9f87f99ec7cf86bd \
+    --hash=sha256:cf22b41fdae514ee2f1691b6c3cdeae666d8b7fa9434de445f12bbeee0cf48dd \
+    --hash=sha256:d38c8f50ecf57f0463399569aa388b232cf1a2ffb8f0a9a5412d0db57e054860 \
+    --hash=sha256:d3be9b2076112e51b323bdf6d5a7f8a798de55fb8d95fcb64bd179460cdc0704 \
+    --hash=sha256:d4f2cc7060dc3646632d7f15fe68e2fa98f58e35dd5666cd525f3b35d3fed7f8 \
+    --hash=sha256:d7520db34088c96cc0e0a3ad51a4fd5b401f279ee112aa2b7f8f976d8582606d \
+    --hash=sha256:d793bebb202a6000390a5390078e945bbb49855c29c7e4d56a85901326c3b5d9 \
+    --hash=sha256:da052e7962ea2d5e5ef5bc0355d55007407087392cf465b7ad84ce5f3e25fe0f \
+    --hash=sha256:dae0ed02f6b075426accbf6b2863c3d0a7eacc1b41fb40f2251d931e50188dad \
+    --hash=sha256:ddc678fb4c7e30cf830a2b5a8d869538bc55b28d6c68544d09c7d0d8f17694dc \
+    --hash=sha256:df2e6f546c4df14bc81f9498bbc007fbb87669f1bb707c6138878c46b06f6510 \
+    --hash=sha256:e02c5175f63effbd7c5e590399c118d5db6183bbfe8e0d118bdb5c2d1b48d937 \
+    --hash=sha256:e196a4ff48310ba62e53a8e0f97ca2bca83cdd2fe2934d8b5cb0df0a841b193a \
+    --hash=sha256:e233db59c8f76630c512ab4a4daf5a5986da5c3d5b44b8e9fc742f2a24dbd460 \
+    --hash=sha256:e32be23d538753a8adb6c85bd539f5fd3b15cb987404327c569dfc5fd8366e85 \
+    --hash=sha256:e3d30321949861404323c50aebeb1943461a67cd51d4200ab02babc58bd06a86 \
+    --hash=sha256:e89580a581bf478d8dcb97d9cd011d567768e8bc4095f8557b21c4d4c5fea7d0 \
+    --hash=sha256:e998e304036198b4f6914e6a1e2b6f925208a20e2042563d9734881150c6c246 \
+    --hash=sha256:ec42088248c596dbd61d4ae8a5b004f97a4d91a9fd286f632e42e60b706718d7 \
+    --hash=sha256:efa7b51824aa0ee957ccd5a741c73e6851de55f40d807f08069eb4c5a26b2baa \
+    --hash=sha256:f0a1bc63a465b6d72569a9bba9f2ef0334c4e03958e043da1920299100bc7c08 \
+    --hash=sha256:f18a5a84e16886898e51ab4b1d43acb3083c39b14c8caeb3589aabff0ee0b270 \
+    --hash=sha256:f2a9efc53d5b714b8df2b4b3e992accf8ce5bbdfe544d74d5c6766c9e1146a3a \
+    --hash=sha256:f3bbbc998d42f8e561f347e798b85513ba4da324c2b3f9b7969e9c45b10f6169 \
+    --hash=sha256:f42038016852ae51b4088b2862126535cc4fc85802bfe30dea3500fdfaf1864e \
+    --hash=sha256:f443cdef978430887ed55112b491f670bba6462cea7a7742ff8f14b7abb98d75 \
+    --hash=sha256:f51969bac61441fd31f028d7b3b45962f3ecebf691a510495e5d2cd8c8092dbd \
+    --hash=sha256:f8aca2e3a72f37bfc7b14ba96d4056244001ddcc18382bd0daa087fd2e68a354 \
+    --hash=sha256:f9737bf36262046213a28e789cc82d82c6ef19c85a0cf05e75c670a33342ac2c \
+    --hash=sha256:fd6037392f2d57793ab98d9e26798f44b8b4da2f2464388588f48ac52c489ea1 \
+    --hash=sha256:feaa45c0eae424d3e90d78823f3828e7dc42a42f21ed420db98da2c4ecf0a2cb \
+    --hash=sha256:ff097ae562e637409b429a7ac958a20aab237a0378c42dabaa1e3abf2f896e5f \
+    --hash=sha256:ff46d772d5f6f73564979cd77a4fffe55c916a05f3cb70e7c9c0590059fb29ef
     # via svglib
-pillow==10.2.0 \
-    --hash=sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8 \
-    --hash=sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39 \
-    --hash=sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac \
-    --hash=sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869 \
-    --hash=sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e \
-    --hash=sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04 \
-    --hash=sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9 \
-    --hash=sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e \
-    --hash=sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe \
-    --hash=sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef \
-    --hash=sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56 \
-    --hash=sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa \
-    --hash=sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f \
-    --hash=sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f \
-    --hash=sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e \
-    --hash=sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a \
-    --hash=sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2 \
-    --hash=sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2 \
-    --hash=sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5 \
-    --hash=sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a \
-    --hash=sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2 \
-    --hash=sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213 \
-    --hash=sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563 \
-    --hash=sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591 \
-    --hash=sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c \
-    --hash=sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2 \
-    --hash=sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb \
-    --hash=sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757 \
-    --hash=sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0 \
-    --hash=sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452 \
-    --hash=sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad \
-    --hash=sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01 \
-    --hash=sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f \
-    --hash=sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5 \
-    --hash=sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61 \
-    --hash=sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e \
-    --hash=sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b \
-    --hash=sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068 \
-    --hash=sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9 \
-    --hash=sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588 \
-    --hash=sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483 \
-    --hash=sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f \
-    --hash=sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67 \
-    --hash=sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7 \
-    --hash=sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311 \
-    --hash=sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6 \
-    --hash=sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72 \
-    --hash=sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6 \
-    --hash=sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129 \
-    --hash=sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13 \
-    --hash=sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67 \
-    --hash=sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c \
-    --hash=sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516 \
-    --hash=sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e \
-    --hash=sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e \
-    --hash=sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364 \
-    --hash=sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023 \
-    --hash=sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1 \
-    --hash=sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04 \
-    --hash=sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d \
-    --hash=sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a \
-    --hash=sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7 \
-    --hash=sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb \
-    --hash=sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4 \
-    --hash=sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e \
-    --hash=sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1 \
-    --hash=sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48 \
-    --hash=sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868
+pillow==10.3.0 \
+    --hash=sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c \
+    --hash=sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2 \
+    --hash=sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb \
+    --hash=sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d \
+    --hash=sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa \
+    --hash=sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3 \
+    --hash=sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1 \
+    --hash=sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a \
+    --hash=sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd \
+    --hash=sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8 \
+    --hash=sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999 \
+    --hash=sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599 \
+    --hash=sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936 \
+    --hash=sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375 \
+    --hash=sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d \
+    --hash=sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b \
+    --hash=sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60 \
+    --hash=sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572 \
+    --hash=sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3 \
+    --hash=sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced \
+    --hash=sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f \
+    --hash=sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b \
+    --hash=sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19 \
+    --hash=sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f \
+    --hash=sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d \
+    --hash=sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383 \
+    --hash=sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795 \
+    --hash=sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355 \
+    --hash=sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57 \
+    --hash=sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09 \
+    --hash=sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b \
+    --hash=sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462 \
+    --hash=sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf \
+    --hash=sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f \
+    --hash=sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a \
+    --hash=sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad \
+    --hash=sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9 \
+    --hash=sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d \
+    --hash=sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45 \
+    --hash=sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994 \
+    --hash=sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d \
+    --hash=sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338 \
+    --hash=sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463 \
+    --hash=sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451 \
+    --hash=sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591 \
+    --hash=sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c \
+    --hash=sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd \
+    --hash=sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32 \
+    --hash=sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9 \
+    --hash=sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf \
+    --hash=sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5 \
+    --hash=sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828 \
+    --hash=sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3 \
+    --hash=sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5 \
+    --hash=sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2 \
+    --hash=sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b \
+    --hash=sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2 \
+    --hash=sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475 \
+    --hash=sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3 \
+    --hash=sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb \
+    --hash=sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef \
+    --hash=sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015 \
+    --hash=sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002 \
+    --hash=sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170 \
+    --hash=sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84 \
+    --hash=sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57 \
+    --hash=sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f \
+    --hash=sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27 \
+    --hash=sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a
     # via
     #   easy-thumbnails
     #   reportlab
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
```

### Comparing `django-sites-extra-0.1.1/runtests.py` & `django-sites-extra-0.1.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/setup.cfg` & `django-sites-extra-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-sites-extra
-version = 0.1.1
+version = 0.1.2
 url = https://github.com/DLRSP/django-sites-extra
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application to extend the standard "sites" framework with extra utils.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-sites-extra-0.1.1/setup.py` & `django-sites-extra-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/src/django_sites_extra.egg-info/PKG-INFO` & `django-sites-extra-0.1.2/src/django_sites_extra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sites-extra
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django application to extend the standard "sites" framework with extra utils.
 Home-page: https://github.com/DLRSP/django-sites-extra
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-sites-extra-0.1.1/src/django_sites_extra.egg-info/SOURCES.txt` & `django-sites-extra-0.1.2/src/django_sites_extra.egg-info/SOURCES.txt`

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
 src/django_sites_extra.egg-info/PKG-INFO
 src/django_sites_extra.egg-info/SOURCES.txt
 src/django_sites_extra.egg-info/dependency_links.txt
 src/django_sites_extra.egg-info/not-zip-safe
```

### Comparing `django-sites-extra-0.1.1/src/sites_extra/admin.py` & `django-sites-extra-0.1.2/src/sites_extra/admin.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/src/sites_extra/context_processors.py` & `django-sites-extra-0.1.2/src/sites_extra/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/src/sites_extra/migrations/0001_initial.py` & `django-sites-extra-0.1.2/src/sites_extra/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/tests/settings.py` & `django-sites-extra-0.1.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-sites-extra-0.1.1/tests/test_fake.py` & `django-sites-extra-0.1.2/tests/test_fake.py`

 * *Files identical despite different names*

