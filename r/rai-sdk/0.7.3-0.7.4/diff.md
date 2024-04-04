# Comparing `tmp/rai-sdk-0.7.3.tar.gz` & `tmp/rai-sdk-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai-sdk-0.7.3.tar", last modified: Thu Mar  7 14:02:14 2024, max compression
+gzip compressed data, was "rai-sdk-0.7.4.tar", last modified: Thu Apr  4 22:07:06 2024, max compression
```

## Comparing `rai-sdk-0.7.3.tar` & `rai-sdk-0.7.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/rai_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-07 14:02:14.000000 rai-sdk-0.7.3/rai_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-07 14:02:14.000000 rai-sdk-0.7.3/rai_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 14:02:14.000000 rai-sdk-0.7.3/rai_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-07 14:02:14.000000 rai-sdk-0.7.3/rai_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 14:02:14.000000 rai-sdk-0.7.3/rai_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/railib/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28474 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/railib/pb/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/pb/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/pb/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/railib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:02:14.301920 rai-sdk-0.7.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-07 14:02:08.000000 rai-sdk-0.7.3/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/rai_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 22:07:06.000000 rai-sdk-0.7.4/rai_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.508692 rai-sdk-0.7.4/railib/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/railib/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/pb/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/railib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:07:06.512693 rai-sdk-0.7.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-04 22:07:01.000000 rai-sdk-0.7.4/test/test_unit.py
```

### Comparing `rai-sdk-0.7.3/LICENSE` & `rai-sdk-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/PKG-INFO` & `rai-sdk-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.7.3
+Version: 0.7.4
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.7.3/README.md` & `rai-sdk-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/rai_sdk.egg-info/PKG-INFO` & `rai-sdk-0.7.4/rai_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-sdk
-Version: 0.7.3
+Version: 0.7.4
 Summary: The RelationalAI Software Development Kit for Python
 Home-page: http://github.com/RelationalAI/rai-sdk-python
 Author: RelationalAI, Inc.
 Author-email: support@relational.ai
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rai-sdk-0.7.3/railib/__init__.py` & `rai-sdk-0.7.4/railib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version_info__ = (0, 7, 3)
+__version_info__ = (0, 7, 4)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `rai-sdk-0.7.3/railib/api.py` & `rai-sdk-0.7.4/railib/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,16 @@
     "list_edbs",
     "list_engines",
     "list_models",
     "list_users",
     "list_oauth_clients",
     "load_csv",
     "update_user",
+    "suspend_engine",
+    "resume_engine",
 ]
 
 
 # Context contains the state required to make rAI API calls.
 class Context(rest.Context):
     def __init__(
         self,
@@ -368,14 +370,38 @@
     poll_with_specified_overhead(
         lambda: is_engine_term_state(get_engine(ctx, engine)["state"]),
         overhead_rate=0.2,
         timeout=30 * 60,
     )
     return get_engine(ctx, engine)
 
+
+def suspend_engine(ctx: Context, engine: str, **kwargs):
+    data = {"suspend": True}
+    url = _mkurl(ctx, f"{PATH_ENGINE}/{engine}")
+    rsp = rest.patch(ctx, url, data, **kwargs)
+    return json.loads(rsp.read())
+
+
+def resume_engine(ctx: Context, engine: str, **kwargs):
+    data = {"suspend": False}
+    url = _mkurl(ctx, f"{PATH_ENGINE}/{engine}")
+    rsp = rest.patch(ctx, url, data, **kwargs)
+    return json.loads(rsp.read())
+
+
+def resume_engine_wait(ctx: Context, engine: str, **kwargs):
+    resume_engine(ctx, engine, **kwargs)
+    poll_with_specified_overhead(
+        lambda: is_engine_term_state(get_engine(ctx, engine)["state"]),
+        overhead_rate=0.2,
+        timeout=30 * 60,
+    )
+    return get_engine(ctx, engine)
+
 
 def create_user(ctx: Context, email: str, roles: List[Role] = None, **kwargs):
     rs = roles or []
     data = {"email": email, "roles": [r.value for r in rs]}
     url = _mkurl(ctx, PATH_USER)
     rsp = rest.post(ctx, url, data, **kwargs)
     return json.loads(rsp.read())
```

### Comparing `rai-sdk-0.7.3/railib/config.py` & `rai-sdk-0.7.4/railib/config.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/railib/credentials.py` & `rai-sdk-0.7.4/railib/credentials.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/railib/pb/message_pb2.py` & `rai-sdk-0.7.4/railib/pb/message_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/railib/pb/schema_pb2.py` & `rai-sdk-0.7.4/railib/pb/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/railib/rest.py` & `rai-sdk-0.7.4/railib/rest.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/railib/show.py` & `rai-sdk-0.7.4/railib/show.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/setup.py` & `rai-sdk-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/test/test_integration.py` & `rai-sdk-0.7.4/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `rai-sdk-0.7.3/test/test_unit.py` & `rai-sdk-0.7.4/test/test_unit.py`

 * *Files identical despite different names*

