# Comparing `tmp/Drumpler-1.0.5.tar.gz` & `tmp/Drumpler-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.5.tar", last modified: Thu Apr  4 18:34:21 2024, max compression
+gzip compressed data, was "Drumpler-1.0.6.tar", last modified: Fri Apr  5 21:42:23 2024, max compression
```

## Comparing `Drumpler-1.0.5.tar` & `Drumpler-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:34:21.528881 Drumpler-1.0.5/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:34:21.527551 Drumpler-1.0.5/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4161 2024-04-04 18:34:21.000000 Drumpler-1.0.5/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-04 18:34:21.000000 Drumpler-1.0.5/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-04 18:34:21.000000 Drumpler-1.0.5/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-04 18:34:21.000000 Drumpler-1.0.5/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-04 18:34:21.000000 Drumpler-1.0.5/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.5/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4161 2024-04-04 18:34:21.528277 Drumpler-1.0.5/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3498 2024-04-04 18:33:48.000000 Drumpler-1.0.5/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:34:21.522171 Drumpler-1.0.5/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.5/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      599 2024-04-03 21:23:08.000000 Drumpler-1.0.5/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     6474 2024-04-03 21:38:26.000000 Drumpler-1.0.5/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.5/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.5/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-04 18:34:21.529043 Drumpler-1.0.5/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-04 18:33:55.000000 Drumpler-1.0.5/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-04 18:34:21.526797 Drumpler-1.0.5/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.5/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.340773 Drumpler-1.0.6/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.339115 Drumpler-1.0.6/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-05 21:42:23.000000 Drumpler-1.0.6/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.6/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-05 21:42:23.339941 Drumpler-1.0.6/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.6/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.333449 Drumpler-1.0.6/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.6/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.6/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6976 2024-04-05 21:39:26.000000 Drumpler-1.0.6/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.6/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.6/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-05 21:42:23.340953 Drumpler-1.0.6/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-05 21:39:34.000000 Drumpler-1.0.6/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-05 21:42:23.338052 Drumpler-1.0.6/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.6/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.5/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: Drumpler
-Version: 1.0.5
-Summary: Framework for rapidly developing a restful API that requires post processing
-Home-page: https://github.com/KarelOmab/Drumpler
-Author: Karel Tutsu
-Author-email: karel.tutsu@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Flask
-Requires-Dist: python-dotenv
-Requires-Dist: SQLAlchemy
-Requires-Dist: Flask_SQLAlchemy
-Requires-Dist: requests
-Requires-Dist: schedule
-Requires-Dist: psycopg2-binary
-
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
 
@@ -47,19 +26,22 @@
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
 
 Create a `.env` file in the root directory of the application with the following contents:
 ```
-DATABASE_URI=your_database_uri_here 
-AUTHORIZATION_KEY=your_authorization_key_here 
-Drumpler_HOST=0.0.0.0 
-Drumpler_PORT=5000 
-Drumpler_DEBUG=True
+AUTHORIZATION_KEY=AUTH_KEY_HERE
+DRUMPLER_HOST=IP_HERE
+DRUMPLER_PORT=PORT_HERE
+DRUMPLER_DEBUG=BOOL_FLAG
+DB_NAME=DB_NAME_HERE
+DB_HOST=DB_HOST_HERE
+DB_USER=DB_USER_HERE
+DB_PASS=DB_PASS_HERE
 ```
 
 Replace `your_database_uri_here` and `your_authorization_key_here` with your actual database URI and desired authorization key.
 
 ## Using the Application - Drumpler
 
 To create a `Drumpler` RESTful server, the following is a sample implementation:
@@ -106,8 +88,8 @@
 
 ## Contributing
 
 Contributions to `Drumpler` are welcome! Please follow the standard fork-branch-PR workflow.
 
 ## License
 
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `Drumpler-1.0.5/LICENSE` & `Drumpler-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.5/PKG-INFO` & `Drumpler-1.0.6/Drumpler.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.5
+Version: 1.0.6
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,19 +47,22 @@
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
 
 Create a `.env` file in the root directory of the application with the following contents:
 ```
-DATABASE_URI=your_database_uri_here 
-AUTHORIZATION_KEY=your_authorization_key_here 
-Drumpler_HOST=0.0.0.0 
-Drumpler_PORT=5000 
-Drumpler_DEBUG=True
+AUTHORIZATION_KEY=AUTH_KEY_HERE
+DRUMPLER_HOST=IP_HERE
+DRUMPLER_PORT=PORT_HERE
+DRUMPLER_DEBUG=BOOL_FLAG
+DB_NAME=DB_NAME_HERE
+DB_HOST=DB_HOST_HERE
+DB_USER=DB_USER_HERE
+DB_PASS=DB_PASS_HERE
 ```
 
 Replace `your_database_uri_here` and `your_authorization_key_here` with your actual database URI and desired authorization key.
 
 ## Using the Application - Drumpler
 
 To create a `Drumpler` RESTful server, the following is a sample implementation:
```

### Comparing `Drumpler-1.0.5/README.md` & `Drumpler-1.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: Drumpler
+Version: 1.0.6
+Summary: Framework for rapidly developing a restful API that requires post processing
+Home-page: https://github.com/KarelOmab/Drumpler
+Author: Karel Tutsu
+Author-email: karel.tutsu@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Flask
+Requires-Dist: python-dotenv
+Requires-Dist: SQLAlchemy
+Requires-Dist: Flask_SQLAlchemy
+Requires-Dist: requests
+Requires-Dist: schedule
+Requires-Dist: psycopg2-binary
+
 
 # `Drumpler`
 
 `Drumpler` is a general-purpose application designed to facilitate efficient workflow automation through RESTful API interactions and job processing. Built on Flask and SQLAlchemy, this application serves as a robust backend for capturing, storing, and processing HTTP requests in a scalable manner. The application is split into two main components: `drumpler.py` for handling RESTful API requests and `mammoth.py` for querying the API and processing jobs asynchronously.
 
 # High Level Overview
 
@@ -26,19 +47,22 @@
 Install Drumpler via pip:
 `pip install Drumpler`
 
 ## Configuration
 
 Create a `.env` file in the root directory of the application with the following contents:
 ```
-DATABASE_URI=your_database_uri_here 
-AUTHORIZATION_KEY=your_authorization_key_here 
-Drumpler_HOST=0.0.0.0 
-Drumpler_PORT=5000 
-Drumpler_DEBUG=True
+AUTHORIZATION_KEY=AUTH_KEY_HERE
+DRUMPLER_HOST=IP_HERE
+DRUMPLER_PORT=PORT_HERE
+DRUMPLER_DEBUG=BOOL_FLAG
+DB_NAME=DB_NAME_HERE
+DB_HOST=DB_HOST_HERE
+DB_USER=DB_USER_HERE
+DB_PASS=DB_PASS_HERE
 ```
 
 Replace `your_database_uri_here` and `your_authorization_key_here` with your actual database URI and desired authorization key.
 
 ## Using the Application - Drumpler
 
 To create a `Drumpler` RESTful server, the following is a sample implementation:
@@ -85,8 +109,8 @@
 
 ## Contributing
 
 Contributions to `Drumpler` are welcome! Please follow the standard fork-branch-PR workflow.
 
 ## License
 
-This project is licensed under the MIT License - see the LICENSE file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `Drumpler-1.0.5/drumpler/constants.py` & `Drumpler-1.0.6/drumpler/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from dotenv import load_dotenv
 
 load_dotenv()  # Load environment variables from .env file
 
 AUTHORIZATION_KEY = os.getenv('AUTHORIZATION_KEY')
 
 # Load environment variables
-DRUMPLER_HOST = "http://127.0.0.1"
-DRUMPLER_PORT = 5000  # Adjust the URL/port as necessary
+DRUMPLER_HOST = os.getenv('DRUMPLER_HOST', "http://127.0.0.1")
+DRUMPLER_PORT = int(os.getenv('DRUMPLER_PORT', "5000"))
 DRUMPLER_URL = f"{DRUMPLER_HOST}:{DRUMPLER_PORT}"  # Adjust the URL/port as necessary
-DRUMPLER_DEBUG = True
+DRUMPLER_DEBUG = bool(os.getenv('DRUMPLER_DEBUG', "True"))
 MAMMOTH_WORKERS = 1
 
 DB_NAME = os.getenv('DB_NAME')
 DB_HOST = os.getenv('DB_HOST')
 DB_USER = os.getenv('DB_USER')
 DB_PASS = os.getenv('DB_PASS')
 DATABASE_URI = f'postgresql://{DB_USER}:{DB_PASS}@{DB_HOST}/{DB_NAME}'
```

### Comparing `Drumpler-1.0.5/drumpler/drumpler.py` & `Drumpler-1.0.6/drumpler/drumpler.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from flask import Flask, request, jsonify
 from .constants import DRUMPLER_HOST, DRUMPLER_PORT, DRUMPLER_DEBUG, DATABASE_URI, AUTHORIZATION_KEY
 import json
 from flask_sqlalchemy import SQLAlchemy
 from .request import Request as BaseRequest
 
 app = Flask(__name__)
-
 app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 
 class Request(db.Model, BaseRequest):
     id = db.Column(db.Integer, primary_key=True)
     timestamp = db.Column(db.DateTime, default=db.func.current_timestamp())
@@ -20,39 +19,52 @@
     method = db.Column(db.String(8))
     request_url = db.Column(db.String(256))
     request_raw = db.Column(db.Text)
     is_handled = db.Column(db.Integer, default=0)
     is_being_processed = db.Column(db.Boolean, default=False)
 
 class Drumpler:
-    def __init__(self, host=DRUMPLER_HOST, port=DRUMPLER_PORT, debug=DRUMPLER_DEBUG):
+    def __init__(self):
         self.__init_env()
         self.app = Flask(__name__)
         self.DATABASE = 'requests.db'
         self.AUTHORIZATION_KEY = AUTHORIZATION_KEY
-        self.host = host
-        self.port = port
-        self.debug = debug
+
+        # Fetching environment variables or using defaults
+        host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
+        port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
+        debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
+        
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
+        self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
+
+        # Initialize SQLAlchemy with the current Flask app
+        db.init_app(self.app)
+
         self.__setup_routes()
 
     def __setup_routes(self):
-        app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
-        app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
-        app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
-        app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
-        app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
+        self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
+        self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
+        self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
+        self.app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
+        self.app.add_url_rule('/request/<int:request_id>', view_func=self.__update_request, methods=['PUT'])
+        self.app.add_url_rule('/request/<int:request_id>', view_func=self.__delete_request, methods=['DELETE'])
 
     def __init_env(self):
         if not os.path.exists(".env"):
             sys.exit("ERROR! You must create a .env file that contains a single line 'AUTHORIZATION_KEY=YourAuthorizationKeyHere'")
 
     def __authorize_request(self):
         authorization = request.headers.get('Authorization')
         return authorization and authorization == f"Bearer {self.AUTHORIZATION_KEY}"
-            
+    
+    def hello_world(self):
+        return "Hello World"
+
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
         data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
         new_request = Request(
             source_ip=request.remote_addr,
@@ -141,12 +153,13 @@
             return jsonify({"message": "Request not found"}), 404
 
     def run(self):
         with app.app_context():
             db.create_all()  # Initialize the database tables within an application context
             db.session.commit()
             
+        
         app.run(host=self.host, port=self.port, debug=self.debug)
 
 if __name__ == '__main__':
     drumpler = Drumpler()
-    drumpler.run()
+    drumpler.run()
```

### Comparing `Drumpler-1.0.5/drumpler/mammoth.py` & `Drumpler-1.0.6/drumpler/mammoth.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.5/drumpler/request.py` & `Drumpler-1.0.6/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.5/setup.py` & `Drumpler-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.5',
+    version='1.0.6',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.5/test/test_drumpler.py` & `Drumpler-1.0.6/test/test_drumpler.py`

 * *Files identical despite different names*

