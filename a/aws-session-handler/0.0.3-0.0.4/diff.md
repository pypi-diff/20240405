# Comparing `tmp/aws_session_handler-0.0.3.tar.gz` & `tmp/aws_session_handler-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws_session_handler-0.0.3.tar", last modified: Wed Aug  1 09:35:31 2018, max compression
+gzip compressed data, was "aws_session_handler-0.0.4.tar", last modified: Fri Apr  5 11:15:30 2024, max compression
```

## Comparing `aws_session_handler-0.0.3.tar` & `aws_session_handler-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/
--rw-rw-r--   0 mario     (1000) mario     (1000)      952 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/PKG-INFO
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler/
--rw-rw-r--   0 mario     (1000) mario     (1000)       71 2018-07-31 18:03:36.000000 aws_session_handler-0.0.3/aws_session_handler/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     9324 2018-08-01 09:29:08.000000 aws_session_handler-0.0.3/aws_session_handler/awssessionhandler.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler.egg-info/
--rw-rw-r--   0 mario     (1000) mario     (1000)      263 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)      952 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler.egg-info/PKG-INFO
--rw-rw-r--   0 mario     (1000) mario     (1000)       20 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler.egg-info/top_level.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)        1 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/aws_session_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)      663 2018-08-01 09:33:35.000000 aws_session_handler-0.0.3/setup.py
--rw-rw-r--   0 mario     (1000) mario     (1000)       38 2018-08-01 09:35:31.000000 aws_session_handler-0.0.3/setup.cfg
--rw-rw-r--   0 mario     (1000) mario     (1000)      382 2018-07-31 18:03:58.000000 aws_session_handler-0.0.3/README.md
+drwxr-xr-x   0 mario     (1000) mario     (1000)        0 2024-04-05 11:15:30.527107 aws_session_handler-0.0.4/
+-rw-r--r--   0 mario     (1000) mario     (1000)     1082 2024-04-05 10:41:22.000000 aws_session_handler-0.0.4/LICENSE
+-rw-r--r--   0 mario     (1000) mario     (1000)      799 2024-04-05 11:15:30.527107 aws_session_handler-0.0.4/PKG-INFO
+-rw-r--r--   0 mario     (1000) mario     (1000)      382 2024-04-05 10:41:22.000000 aws_session_handler-0.0.4/README.md
+drwxr-xr-x   0 mario     (1000) mario     (1000)        0 2024-04-05 11:15:30.527107 aws_session_handler-0.0.4/aws_session_handler/
+-rw-r--r--   0 mario     (1000) mario     (1000)       71 2024-04-05 10:41:22.000000 aws_session_handler-0.0.4/aws_session_handler/__init__.py
+-rw-r--r--   0 mario     (1000) mario     (1000)     9756 2024-04-05 10:41:22.000000 aws_session_handler-0.0.4/aws_session_handler/awssessionhandler.py
+drwxr-xr-x   0 mario     (1000) mario     (1000)        0 2024-04-05 11:15:30.527107 aws_session_handler-0.0.4/aws_session_handler.egg-info/
+-rw-r--r--   0 mario     (1000) mario     (1000)      799 2024-04-05 11:15:30.000000 aws_session_handler-0.0.4/aws_session_handler.egg-info/PKG-INFO
+-rw-r--r--   0 mario     (1000) mario     (1000)      271 2024-04-05 11:15:30.000000 aws_session_handler-0.0.4/aws_session_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 mario     (1000) mario     (1000)        1 2024-04-05 11:15:30.000000 aws_session_handler-0.0.4/aws_session_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 mario     (1000) mario     (1000)       20 2024-04-05 11:15:30.000000 aws_session_handler-0.0.4/aws_session_handler.egg-info/top_level.txt
+-rw-r--r--   0 mario     (1000) mario     (1000)       38 2024-04-05 11:15:30.527107 aws_session_handler-0.0.4/setup.cfg
+-rw-r--r--   0 mario     (1000) mario     (1000)      714 2024-04-05 11:15:25.000000 aws_session_handler-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aws_session_handler-0.0.3/aws_session_handler/awssessionhandler.py` & `aws_session_handler-0.0.4/aws_session_handler/awssessionhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,28 @@
         """
         if not self._profile and not self._region:
             raise Exception('ERROR: missing region and profile (use self.set(profile_name=None, region=None)')
 
         self._get_session()
         return self._session.client(*args, **kwargs)
 
+    def resource(self, *args, **kwargs):
+        """
+        Lookup credentials and give a boto3 resource in return
+        (check boto3 client for args, kwargs)
+        :param args:
+        :param kwargs:
+        :return: boto3 session client
+        """
+        if not self._profile and not self._region:
+            raise Exception('ERROR: missing region and profile (use self.set(profile_name=None, region=None)')
+
+        self._get_session()
+        return self._session.resource(*args, **kwargs)
+
     def get_session(self):
         self._get_session()
         return self._session
 
     def _config_lookup(self):
         self._lookup_session = session.get_session()
         self._lookup_session.set_config_variable('profile', self._profile)
@@ -154,15 +168,14 @@
                     'aws_access_key_id': cred['AccessKeyId'],
                     'aws_secret_access_key': cred['SecretAccessKey'],
                     'aws_session_token': cred['SessionToken'],
                     'expire': cred['Expiration'].isoformat(),
                     'source_profile': self._config['source_profile'],
                     'region': self._region,
                 }
-                # ToDo resolve username and append to RoleSessionName?
 
             if not self._short_session_token:
                 token_changed = True
                 assume_session = boto3.Session(
                     aws_access_key_id=self._long_session_token['aws_access_key_id'],
                     aws_secret_access_key=self._long_session_token['aws_secret_access_key'],
                     aws_session_token=self._long_session_token['aws_session_token'],
```

### Comparing `aws_session_handler-0.0.3/setup.py` & `aws_session_handler-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='aws_session_handler',
     packages=find_packages(),
     version=VERSION,
     description='AWS Session Handler',
+    long_description_content_type='text/markdown',
     long_description=long_description,
     keywords='boto3 amazon web services aws authentication',
     author='MarioVerbelen',
     author_email='mario@verbelen.org',
     url='https://github.com/MarioVerbelen/aws_session_handler',
     download_url='https://github.com/MarioVerbelen/aws_session_handler',
     license='MIT License',
```

