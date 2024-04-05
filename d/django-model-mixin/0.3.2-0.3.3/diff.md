# Comparing `tmp/django-model-mixin-0.3.2.tar.gz` & `tmp/django-model-mixin-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-mixin-0.3.2.tar", last modified: Sun Oct  8 17:35:12 2023, max compression
+gzip compressed data, was "django-model-mixin-0.3.3.tar", last modified: Fri Apr  5 21:51:25 2024, max compression
```

## Comparing `django-model-mixin-0.3.2.tar` & `django-model-mixin-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.063447 django-model-mixin-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-08 17:35:12.063447 django-model-mixin-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.059446 django-model-mixin-0.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    32974 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44937 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44508 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    45247 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44959 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2023-10-08 17:35:12.063447 django-model-mixin-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.051447 django-model-mixin-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.059446 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-08 17:35:12.000000 django-model-mixin-0.3.2/src/django_model_mixin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.059446 django-model-mixin-0.3.2/src/model_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/src/model_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/src/model_mixin/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.051447 django-model-mixin-0.3.2/src/model_mixin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.051447 django-model-mixin-0.3.2/src/model_mixin/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.059446 django-model-mixin-0.3.2/src/model_mixin/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/src/model_mixin/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/src/model_mixin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 17:35:12.059446 django-model-mixin-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-10-08 17:34:51.000000 django-model-mixin-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.314747 django-model-mixin-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-05 21:51:25.314747 django-model-mixin-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.310747 django-model-mixin-0.3.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-05 21:51:25.314747 django-model-mixin-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.306748 django-model-mixin-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.310747 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 21:51:25.000000 django-model-mixin-0.3.3/src/django_model_mixin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.310747 django-model-mixin-0.3.3/src/model_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/src/model_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/src/model_mixin/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.306748 django-model-mixin-0.3.3/src/model_mixin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.306748 django-model-mixin-0.3.3/src/model_mixin/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.310747 django-model-mixin-0.3.3/src/model_mixin/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/src/model_mixin/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/src/model_mixin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:25.310747 django-model-mixin-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 21:51:14.000000 django-model-mixin-0.3.3/tox.ini
```

### Comparing `django-model-mixin-0.3.2/.pre-commit-config.yaml` & `django-model-mixin-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/LICENSE` & `django-model-mixin-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/PKG-INFO` & `django-model-mixin-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-mixin
-Version: 0.3.2
+Version: 0.3.3
 Summary: Django application provide simple model's mixins to add common reusable attributes.
 Home-page: https://github.com/DLRSP/django-model-mixin
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-model-mixin-0.3.2/README.md` & `django-model-mixin-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/mkdocs.yml` & `django-model-mixin-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/pyproject.toml` & `django-model-mixin-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     --strict-markers
     --ds=tests.settings
     """
 django_find_project = false
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "0.3.2"
+current_version = "0.3.3"
 commit = true
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
```

### Comparing `django-model-mixin-0.3.2/requirements/py310-django32.txt` & `django-model-mixin-0.3.3/requirements/py310-django42.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==3.2.22 \
-    --hash=sha256:83b6d66b06e484807d778263fdc7f9186d4dc1862fcfa6507830446ac6b060ba \
-    --hash=sha256:c5e7b668025a6e06cad9ba6d4de1fd1a21212acebb51ea34abb400c6e4d33430
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via -r requirements/requirements.in
-pytz==2023.3.post1 \
-    --hash=sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b \
-    --hash=sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7
-    # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.8.0 \
-    --hash=sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0 \
-    --hash=sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef
+typing-extensions==4.10.0 \
+    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
+    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
     # via asgiref
```

### Comparing `django-model-mixin-0.3.2/requirements/py310-django42.txt` & `django-model-mixin-0.3.3/requirements/py311-django42.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django42.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==4.2.6 \
-    --hash=sha256:08f41f468b63335aea0d904c5729e0250300f6a1907bf293a65499496cdbc68f \
-    --hash=sha256:a64d2487cdb00ad7461434320ccc38e60af9c404773a2f95ab0093b4453a3215
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.8.0 \
-    --hash=sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0 \
-    --hash=sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef
-    # via asgiref
```

### Comparing `django-model-mixin-0.3.2/requirements/py311-django32.txt` & `django-model-mixin-0.3.3/requirements/py311-django32.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
-django==3.2.22 \
-    --hash=sha256:83b6d66b06e484807d778263fdc7f9186d4dc1862fcfa6507830446ac6b060ba \
-    --hash=sha256:c5e7b668025a6e06cad9ba6d4de1fd1a21212acebb51ea34abb400c6e4d33430
+django==3.2.25 \
+    --hash=sha256:7ca38a78654aee72378594d63e51636c04b8e28574f5505dff630895b5472777 \
+    --hash=sha256:a52ea7fcf280b16f7b739cec38fa6d3f8953a5456986944c3ca97e79882b4e38
     # via -r requirements/requirements.in
-pytz==2023.3.post1 \
-    --hash=sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b \
-    --hash=sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7
+pytz==2024.1 \
+    --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
+    --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
```

### Comparing `django-model-mixin-0.3.2/requirements/py38-django42.txt` & `django-model-mixin-0.3.3/requirements/py38-django42.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django42.txt requirements/requirements.in
 #
-asgiref==3.7.2 \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
+asgiref==3.8.1 \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 backports-zoneinfo==0.2.1 \
     --hash=sha256:17746bd546106fa389c51dbea67c8b7c8f0d14b5526a579ca6ccf5ed72c526cf \
     --hash=sha256:1b13e654a55cd45672cb54ed12148cd33628f672548f373963b0bff67b217328 \
     --hash=sha256:1c5742112073a563c81f786e77514969acb58649bcdf6cdf0b4ed31a348d4546 \
     --hash=sha256:4a0f800587060bf8880f954dbef70de6c11bbe59c673c3d818921f042f9954a6 \
     --hash=sha256:5c144945a7752ca544b4b78c8c41544cdfaf9786f25fe5ffb10e838e19a27570 \
@@ -22,19 +22,19 @@
     --hash=sha256:da6013fd84a690242c310d77ddb8441a559e9cb3d3d59ebac9aca1a57b2e18bc \
     --hash=sha256:e55b384612d93be96506932a786bbcde5a2db7a9e6a4bb4bffe8b733f5b9036b \
     --hash=sha256:e81b76cace8eda1fca50e345242ba977f9be6ae3945af8d46326d776b4cf78d1 \
     --hash=sha256:e8236383a20872c0cdf5a62b554b27538db7fa1bbec52429d8d106effbaeca08 \
     --hash=sha256:f04e857b59d9d1ccc39ce2da1021d196e47234873820cbeaad210724b1ee28ac \
     --hash=sha256:fadbfe37f74051d024037f223b8e001611eac868b5c5b06144ef4d8b799862f2
     # via django
-django==4.2.6 \
-    --hash=sha256:08f41f468b63335aea0d904c5729e0250300f6a1907bf293a65499496cdbc68f \
-    --hash=sha256:a64d2487cdb00ad7461434320ccc38e60af9c404773a2f95ab0093b4453a3215
+django==4.2.11 \
+    --hash=sha256:6e6ff3db2d8dd0c986b4eec8554c8e4f919b5c1ff62a5b4390c17aff2ed6e5c4 \
+    --hash=sha256:ddc24a0a8280a0430baa37aff11f28574720af05888c62b7cfe71d219f4599d3
     # via -r requirements/requirements.in
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.8.0 \
-    --hash=sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0 \
-    --hash=sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef
+typing-extensions==4.10.0 \
+    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
+    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
     # via asgiref
```

### Comparing `django-model-mixin-0.3.2/runtests.py` & `django-model-mixin-0.3.3/runtests.py`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/setup.cfg` & `django-model-mixin-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-model-mixin
-version = 0.3.2
+version = 0.3.3
 url = https://github.com/DLRSP/django-model-mixin
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application provide simple model's mixins to add common reusable attributes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-model-mixin-0.3.2/setup.py` & `django-model-mixin-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/src/django_model_mixin.egg-info/PKG-INFO` & `django-model-mixin-0.3.3/src/django_model_mixin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-mixin
-Version: 0.3.2
+Version: 0.3.3
 Summary: Django application provide simple model's mixins to add common reusable attributes.
 Home-page: https://github.com/DLRSP/django-model-mixin
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-model-mixin-0.3.2/src/django_model_mixin.egg-info/SOURCES.txt` & `django-model-mixin-0.3.3/src/django_model_mixin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

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
 src/django_model_mixin.egg-info/PKG-INFO
 src/django_model_mixin.egg-info/SOURCES.txt
 src/django_model_mixin.egg-info/dependency_links.txt
 src/django_model_mixin.egg-info/not-zip-safe
```

### Comparing `django-model-mixin-0.3.2/src/model_mixin/admin.py` & `django-model-mixin-0.3.3/src/model_mixin/admin.py`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/src/model_mixin/locale/it/LC_MESSAGES/django.po` & `django-model-mixin-0.3.3/src/model_mixin/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/src/model_mixin/models.py` & `django-model-mixin-0.3.3/src/model_mixin/models.py`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/tests/settings.py` & `django-model-mixin-0.3.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-model-mixin-0.3.2/tests/test_fake.py` & `django-model-mixin-0.3.3/tests/test_fake.py`

 * *Files identical despite different names*

