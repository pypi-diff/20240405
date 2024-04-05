# Comparing `tmp/Drumpler-1.0.6.tar.gz` & `tmp/Drumpler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.6.tar", last modified: Fri Apr  5 21:42:23 2024, max compression
+gzip compressed data, was "Drumpler-1.0.7.tar", last modified: Fri Apr  5 21:43:29 2024, max compression
```

## Comparing `Drumpler-1.0.6.tar` & `Drumpler-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.340773 Drumpler-1.0.6/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.339115 Drumpler-1.0.6/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.6/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:42:23.339941 Drumpler-1.0.6/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.6/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.333449 Drumpler-1.0.6/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.6/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.6/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6976 2024-04-05 21:39:26.000000 Drumpler-1.0.6/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.6/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.6/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-05 21:42:23.340953 Drumpler-1.0.6/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-05 21:39:34.000000 Drumpler-1.0.6/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.338052 Drumpler-1.0.6/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.6/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.533457 Drumpler-1.0.7/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.531896 Drumpler-1.0.7/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-05 21:43:29.000000 Drumpler-1.0.7/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.7/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:43:29.532624 Drumpler-1.0.7/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.7/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.526579 Drumpler-1.0.7/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.7/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.7/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6982 2024-04-05 21:43:17.000000 Drumpler-1.0.7/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.7/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.7/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-05 21:43:29.533637 Drumpler-1.0.7/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-05 21:43:22.000000 Drumpler-1.0.7/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:43:29.530959 Drumpler-1.0.7/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.7/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.6/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.7/Drumpler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.6/LICENSE` & `Drumpler-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.6/PKG-INFO` & `Drumpler-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.6/README.md` & `Drumpler-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.6/drumpler/constants.py` & `Drumpler-1.0.7/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.6/drumpler/drumpler.py` & `Drumpler-1.0.7/drumpler/drumpler.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     def __init__(self):
         self.__init_env()
         self.app = Flask(__name__)
         self.DATABASE = 'requests.db'
         self.AUTHORIZATION_KEY = AUTHORIZATION_KEY
 
         # Fetching environment variables or using defaults
-        host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
-        port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
-        debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
+        self.host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
+        self.port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
+        self.debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
         
         self.app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
         # Initialize SQLAlchemy with the current Flask app
         db.init_app(self.app)
 
@@ -153,13 +153,12 @@
             return jsonify({"message": "Request not found"}), 404
 
     def run(self):
         with app.app_context():
             db.create_all()  # Initialize the database tables within an application context
             db.session.commit()
             
-        
         app.run(host=self.host, port=self.port, debug=self.debug)
 
 if __name__ == '__main__':
     drumpler = Drumpler()
     drumpler.run()
```

### Comparing `Drumpler-1.0.6/drumpler/mammoth.py` & `Drumpler-1.0.7/drumpler/mammoth.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.6/drumpler/request.py` & `Drumpler-1.0.7/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.6/setup.py` & `Drumpler-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.6',
+    version='1.0.7',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.6/test/test_drumpler.py` & `Drumpler-1.0.7/test/test_drumpler.py`

 * *Files identical despite different names*

