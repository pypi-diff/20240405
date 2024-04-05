# Comparing `tmp/messages-local-0.0.47.tar.gz` & `tmp/messages-local-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages-local-0.0.47.tar", last modified: Thu Mar 14 20:40:40 2024, max compression
+gzip compressed data, was "messages-local-0.0.48.tar", last modified: Fri Apr  5 09:47:49 2024, max compression
```

## Comparing `messages-local-0.0.47.tar` & `messages-local-0.0.48.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:40:40.756119 messages-local-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-14 20:40:40.756119 messages-local-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-14 20:40:02.000000 messages-local-0.0.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:40:40.752119 messages-local-0.0.47/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:40:40.756119 messages-local-0.0.47/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-03-14 20:40:02.000000 messages-local-0.0.47/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 20:40:02.000000 messages-local-0.0.47/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:40:40.756119 messages-local-0.0.47/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-14 20:40:40.000000 messages-local-0.0.47/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-14 20:40:40.000000 messages-local-0.0.47/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 20:40:40.000000 messages-local-0.0.47/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-14 20:40:40.000000 messages-local-0.0.47/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-14 20:40:40.000000 messages-local-0.0.47/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-14 20:40:02.000000 messages-local-0.0.47/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 20:40:40.756119 messages-local-0.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-14 20:40:02.000000 messages-local-0.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 09:47:49.289157 messages-local-0.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 09:47:09.000000 messages-local-0.0.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.285157 messages-local-0.0.48/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-05 09:47:09.000000 messages-local-0.0.48/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:09.000000 messages-local-0.0.48/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:47:49.289157 messages-local-0.0.48/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 09:47:49.000000 messages-local-0.0.48/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 09:47:09.000000 messages-local-0.0.48/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:47:49.289157 messages-local-0.0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-05 09:47:09.000000 messages-local-0.0.48/setup.py
```

### Comparing `messages-local-0.0.47/PKG-INFO` & `messages-local-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.47
+Version: 0.0.48
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages-local-0.0.47/README.md` & `messages-local-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `messages-local-0.0.47/messages_local/src/MessagesLocal.py` & `messages-local-0.0.48/messages_local/src/MessagesLocal.py`

 * *Files identical despite different names*

### Comparing `messages-local-0.0.47/messages_local.egg-info/PKG-INFO` & `messages-local-0.0.48/messages_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.47
+Version: 0.0.48
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages-local-0.0.47/setup.py` & `messages-local-0.0.48/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.47', # https://pypi.org/project/messages-local
+    version='0.0.48', # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/messages-local-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
@@ -25,9 +25,8 @@
                       "queue-worker-local>=0.0.12",  # https://pypi.org/project/queue-worker-local/
                       "variable-local>=0.0.45",  # https://pypi.org/project/variable-local/
                       "label-message-local>=0.0.2",
                       "whatsapp-message-vonage-local",
                       "whataspp-inforu-local",
                       "email-message-aws-ses-local"
                       ]
-
 )
```

