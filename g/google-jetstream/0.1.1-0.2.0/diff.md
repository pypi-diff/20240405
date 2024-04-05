# Comparing `tmp/google-jetstream-0.1.1.tar.gz` & `tmp/google-jetstream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-jetstream-0.1.1.tar", last modified: Fri Mar  1 03:20:10 2024, max compression
+gzip compressed data, was "google-jetstream-0.2.0.tar", last modified: Fri Apr  5 20:27:53 2024, max compression
```

## Comparing `google-jetstream-0.1.1.tar` & `google-jetstream-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.166956 google-jetstream-0.1.1/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-02-25 02:26:58.000000 google-jetstream-0.1.1/AUTHORS
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)    11358 2024-02-25 01:51:15.000000 google-jetstream-0.1.1/LICENSE
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1360 2024-03-01 03:20:10.166956 google-jetstream-0.1.1/PKG-INFO
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      843 2024-02-27 01:12:15.000000 google-jetstream-0.1.1/README.md
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/google_jetstream.egg-info/
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1360 2024-03-01 03:20:10.000000 google-jetstream-0.1.1/google_jetstream.egg-info/PKG-INFO
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1030 2024-03-01 03:20:10.000000 google-jetstream-0.1.1/google_jetstream.egg-info/SOURCES.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)        1 2024-03-01 03:20:10.000000 google-jetstream-0.1.1/google_jetstream.egg-info/dependency_links.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       54 2024-03-01 03:20:10.000000 google-jetstream-0.1.1/google_jetstream.egg-info/requires.txt
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-03-01 03:20:10.000000 google-jetstream-0.1.1/google_jetstream.egg-info/top_level.txt
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/__init__.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/core/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/core/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     5197 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/core/config_lib.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/core/implementations/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/core/implementations/__init__.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/core/implementations/mock/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/core/implementations/mock/__init__.py
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      992 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/core/implementations/mock/config.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1633 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/core/implementations/mock/server.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)    22410 2024-03-01 01:24:19.000000 google-jetstream-0.1.1/jetstream/core/orchestrator.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3231 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/core/orchestrator_test.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/core/proto/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/core/proto/__init__.py
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)     2233 2024-02-27 00:06:04.000000 google-jetstream-0.1.1/jetstream/core/proto/jetstream_pb2.py
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)     3311 2024-02-27 00:06:04.000000 google-jetstream-0.1.1/jetstream/core/proto/jetstream_pb2_grpc.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2428 2024-02-26 23:57:50.000000 google-jetstream-0.1.1/jetstream/core/server_lib.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2815 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/core/server_test.py
-drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-03-01 03:20:10.162956 google-jetstream-0.1.1/jetstream/engine/
--rw-r--r--   0 zijunzhou (868522) primarygroup (89939)      575 2024-02-25 02:08:13.000000 google-jetstream-0.1.1/jetstream/engine/__init__.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     7042 2024-02-26 23:57:50.000000 google-jetstream-0.1.1/jetstream/engine/engine_api.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     9190 2024-02-26 23:57:50.000000 google-jetstream-0.1.1/jetstream/engine/mock_engine.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3896 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/engine/mock_engine_test.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2604 2024-02-26 20:25:41.000000 google-jetstream-0.1.1/jetstream/engine/mock_utils.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     6227 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/engine/token_utils.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1805 2024-02-27 00:06:04.000000 google-jetstream-0.1.1/jetstream/engine/tokenizer_pb2.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)      734 2024-02-27 00:06:04.000000 google-jetstream-0.1.1/jetstream/engine/tokenizer_pb2_grpc.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2787 2024-02-26 23:57:02.000000 google-jetstream-0.1.1/jetstream/engine/utils_test.py
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)       38 2024-03-01 03:20:10.166956 google-jetstream-0.1.1/setup.cfg
--rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1535 2024-03-01 03:20:02.000000 google-jetstream-0.1.1/setup.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-02-25 02:26:58.000000 google-jetstream-0.2.0/AUTHORS
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)    11358 2024-02-25 01:51:15.000000 google-jetstream-0.2.0/LICENSE
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)       23 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/MANIFEST.in
+-rw-r--r--   0 zijunzhou (868522) primarygroup (89939)    12231 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/PKG-INFO
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)    11508 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/README.md
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/google_jetstream.egg-info/
+-rw-r--r--   0 zijunzhou (868522) primarygroup (89939)    12231 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/PKG-INFO
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1133 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/SOURCES.txt
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)        1 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/dependency_links.txt
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)       54 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/requires.txt
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)       10 2024-04-05 20:27:53.000000 google-jetstream-0.2.0/google_jetstream.egg-info/top_level.txt
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.943053 google-jetstream-0.2.0/jetstream/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/__init__.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/__init__.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     5185 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/config_lib.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/implementations/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/__init__.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/implementations/mock/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/__init__.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      993 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/config.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1512 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/implementations/mock/server.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)    25986 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/orchestrator.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3401 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/orchestrator_test.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.947053 google-jetstream-0.2.0/jetstream/core/proto/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/__init__.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2273 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3182 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2_grpc.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     4623 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/server_lib.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2857 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/server_test.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/jetstream/core/utils/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/utils/__init__.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3357 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/core/utils/async_multifuture.py
+drwxr-x---   0 zijunzhou (868522) primarygroup (89939)        0 2024-04-05 20:27:53.951054 google-jetstream-0.2.0/jetstream/engine/
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      574 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/__init__.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     7096 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/engine_api.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     9214 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_engine.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     3896 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_engine_test.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2792 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/mock_utils.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     6814 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/token_utils.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1840 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)      755 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2_grpc.py
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     2823 2024-04-04 18:58:15.000000 google-jetstream-0.2.0/jetstream/engine/utils_test.py
+-rw-r--r--   0 zijunzhou (868522) primarygroup (89939)       53 2024-04-05 19:41:14.000000 google-jetstream-0.2.0/requirements.in
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)       38 2024-04-05 20:27:53.955054 google-jetstream-0.2.0/setup.cfg
+-rw-r-----   0 zijunzhou (868522) primarygroup (89939)     1592 2024-04-05 20:24:22.000000 google-jetstream-0.2.0/setup.py
```

### Comparing `google-jetstream-0.1.1/LICENSE` & `google-jetstream-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-jetstream-0.1.1/google_jetstream.egg-info/SOURCES.txt` & `google-jetstream-0.2.0/google_jetstream.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 AUTHORS
 LICENSE
+MANIFEST.in
 README.md
+requirements.in
 setup.py
 google_jetstream.egg-info/PKG-INFO
 google_jetstream.egg-info/SOURCES.txt
 google_jetstream.egg-info/dependency_links.txt
 google_jetstream.egg-info/requires.txt
 google_jetstream.egg-info/top_level.txt
 jetstream/__init__.py
@@ -17,14 +19,16 @@
 jetstream/core/implementations/__init__.py
 jetstream/core/implementations/mock/__init__.py
 jetstream/core/implementations/mock/config.py
 jetstream/core/implementations/mock/server.py
 jetstream/core/proto/__init__.py
 jetstream/core/proto/jetstream_pb2.py
 jetstream/core/proto/jetstream_pb2_grpc.py
+jetstream/core/utils/__init__.py
+jetstream/core/utils/async_multifuture.py
 jetstream/engine/__init__.py
 jetstream/engine/engine_api.py
 jetstream/engine/mock_engine.py
 jetstream/engine/mock_engine_test.py
 jetstream/engine/mock_utils.py
 jetstream/engine/token_utils.py
 jetstream/engine/tokenizer_pb2.py
```

### Comparing `google-jetstream-0.1.1/jetstream/__init__.py` & `google-jetstream-0.2.0/jetstream/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/core/__init__.py` & `google-jetstream-0.2.0/jetstream/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/core/config_lib.py` & `google-jetstream-0.2.0/jetstream/core/config_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,72 +35,72 @@
   prefill_slices: Tuple[str, ...] = ()
   generate_slices: Tuple[str, ...] = ()
   interleaved_slices: Tuple[str, ...] = ()
   prefill_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
   generate_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
   interleaved_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
 
-  def get_slices_to_launch(self: 'ServerConfig') -> str:
+  def get_slices_to_launch(self: "ServerConfig") -> str:
     """Used when launching this config via xm config."""
-    return ','.join(
+    return ",".join(
         self.prefill_slices + self.generate_slices + self.interleaved_slices
     )
 
 
 @dataclasses.dataclass
 class InstantiatedEngines:
   prefill_engines: List[engine_api.Engine]
   generate_engines: List[engine_api.Engine]
   interleaved_engines: List[engine_api.Engine]
 
 
-# ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
+# ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
 
 
 def get_test_engine(devices: Devices, weight: int) -> engine_api.Engine:
   del devices
   return mock_engine.TestEngine(
       batch_size=8,
       cache_length=32,
       weight=weight,
   )
 
 
 @dataclasses.dataclass
 class CPUTestServer(ServerConfig):
-  prefill_slices = ('cpu=1',)
-  generate_slices = ('cpu=1',)
+  prefill_slices = ("cpu=1",)
+  generate_slices = ("cpu=1",)
   prefill_engine_create_fns = (functools.partial(get_test_engine, weight=2),)
   generate_engine_create_fns = (functools.partial(get_test_engine, weight=4),)
 
 
 @dataclasses.dataclass
 class InterleavedCPUTestServer(ServerConfig):
-  interleaved_slices = ('cpu=1',)
+  interleaved_slices = ("cpu=1",)
   interleaved_engine_create_fns = (
       functools.partial(get_test_engine, weight=2),
   )
 
 
-# ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
+# ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
 
 
 def slice_to_num_chips(s: str) -> int:
   """Converts a TPU spec like v5e=4x2 to the number of chips, 8."""
   # Account for the case where it is written 'v5e:4x2'.
-  delim = '=' if '=' in s else ':'
-  i = math.prod([int(c) for c in s.split(delim)[1].split('x')])
+  delim = "=" if "=" in s else ":"
+  i = math.prod([int(c) for c in s.split(delim)[1].split("x")])
   return i
 
 
 def _split_devices_by_slices(
     devices: list[Devices], slices: list[int]
 ) -> List[List[Devices]]:
   """Converts an ordered list of devices into slices."""
-  assert sum(slices) == len(devices), f'{sum(slices)} != {len(devices)}'
+  assert sum(slices) == len(devices), f"{sum(slices)} != {len(devices)}"
   cumsum = 0
   slice_split_devices = []
   for sl in slices:
     slice_split_devices.append(devices[cumsum : cumsum + sl])
     cumsum += sl
   return slice_split_devices
 
@@ -124,23 +124,23 @@
       slice_to_num_chips(s)
       for s in list(server_config.prefill_slices)
       + list(server_config.generate_slices)
       + list(server_config.interleaved_slices)
   ]
   if sum(slices) != len(devices):
     raise ValueError(
-        f'The number of available devices ({len(devices)}) do not match the '
-        f'expected number of devices on all the slices ({sum(slices)}) '
-        'specified in the server_config:\n'
-        f'{server_config.prefill_slices=}\n'
-        f'{server_config.generate_slices=}\n'
-        f'{server_config.interleaved_slices=}\n'
+        f"The number of available devices ({len(devices)}) do not match the "
+        f"expected number of devices on all the slices ({sum(slices)}) "
+        "specified in the server_config:\n"
+        f"{server_config.prefill_slices=}\n"
+        f"{server_config.generate_slices=}\n"
+        f"{server_config.interleaved_slices=}\n"
     )
   # e.g. [[tpu_0], [tpu_1]] corresponding to prefill: v5e=1x1
-  # generate = v5e=1x1; or [[tpu_0, tpu_1, tpu_2, tpu_3]] corresponding to 
+  # generate = v5e=1x1; or [[tpu_0, tpu_1, tpu_2, tpu_3]] corresponding to
   # interleaved: v5e=2x2
   split_devices = _split_devices_by_slices(devices, slices)
   prefill_engines = [
       e(split_devices.pop(0)) for e in server_config.prefill_engine_create_fns
   ]
   generate_engines = [
       e(split_devices.pop(0)) for e in server_config.generate_engine_create_fns
@@ -148,8 +148,8 @@
   # These share chips and weights for prefill and generation.
   interleaved_engines = [
       e(split_devices.pop(0))
       for e in server_config.interleaved_engine_create_fns
   ]
   return InstantiatedEngines(
       prefill_engines, generate_engines, interleaved_engines
-  )
+  )
```

### Comparing `google-jetstream-0.1.1/jetstream/core/implementations/__init__.py` & `google-jetstream-0.2.0/jetstream/core/implementations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/core/implementations/mock/__init__.py` & `google-jetstream-0.2.0/jetstream/core/implementations/mock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/core/implementations/mock/config.py` & `google-jetstream-0.2.0/jetstream/core/implementations/mock/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 """Config for mock."""
 
 from typing import Type
 
 
 from jetstream.core import config_lib
 
+
 def get_server_config(config_str: str) -> Type[config_lib.ServerConfig]:
   match config_str:
-    case 'InterleavedCPUTestServer':
+    case "InterleavedCPUTestServer":
       server_config = config_lib.InterleavedCPUTestServer
-    case 'CPUTestServer':
+    case "CPUTestServer":
       server_config = config_lib.CPUTestServer
     case _:
       raise NotImplementedError
   return server_config
```

### Comparing `google-jetstream-0.1.1/jetstream/core/implementations/mock/server.py` & `google-jetstream-0.2.0/jetstream/core/implementations/mock/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,35 +19,33 @@
 from absl import app
 from absl import flags
 
 from jetstream.core.implementations.mock import config as mock_config
 from jetstream.core import server_lib
 
 
-_PORT = flags.DEFINE_integer('port', 9000, 'port to listen on')
-_THREADS = flags.DEFINE_integer(
-    'threads', 64, 'number of worker threads in thread pool'
-)
+_PORT = flags.DEFINE_integer("port", 9000, "port to listen on")
 _CONFIG = flags.DEFINE_string(
-    'config',
-    'InterleavedCPUTestServer',
-    'available servers',
+    "config",
+    "InterleavedCPUTestServer",
+    "available servers",
 )
 
+
 def main(argv: Sequence[str]):
   del argv
   # No devices for local cpu test. A None for prefill and a None for generate.
   devices = server_lib.get_devices()
   server_config = mock_config.get_server_config(_CONFIG.value)
-  # We separate credential from run so that we can unit test it with local credentials.
+  # We separate credential from run so that we can unit test it with local
+  # credentials.
   # TODO: Add grpc credentials for OSS.
   jetstream_server = server_lib.run(
-      threads=_THREADS.value,
       port=_PORT.value,
       config=server_config,
       devices=devices,
   )
   jetstream_server.wait_for_termination()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
   app.run(main)
```

### Comparing `google-jetstream-0.1.1/jetstream/core/orchestrator.py` & `google-jetstream-0.2.0/jetstream/core/orchestrator.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Orchestrates the engines for the inference workflow with performance optimization.
+"""Orchestrates the engines with performance optimization for inference.
 
 1. A client sends a DecodeRequest via gRPC to the server, an 'LLMOrchestrator'.
 2. This gets wrapped as an 'ActiveRequest' inside the orchestrator, with a
     'return_channel' queue as a place that output tokens can be placed.
     - The ActiveRequest is placed on the 'prefill_queue'.
     - A while loop runs continuously, yielding any tokens placed on the return
       channel until an end condition is met (EOS token or max tokens).
@@ -57,467 +57,609 @@
 grpc.
 It is literally queues all the way down! :)
 The primary concern is GIL contention between threads, which is why we block
 on queues that don't have an ongoing activity (i.e. everything but the
 generation queue) because we don't control to go back to those queues until
 necessary. Blocking means that the GIL doesn't switch back to that thread,
 wheras continual queue get operations 'chop' control and mean that we do not
-achieve good throughput. This is okay on the prefill/transfer/detokenisation
+achieve good throughput. This is okay on the prefill/transfer/detokenization
 threads because we don't need to do anything other than react to the presence
 of items on these queues, wheras the generation thread needs to also run a
 step - so it cannot block until it has new things to insert.
 
 ## Testing
 This server is intended to be easy to locally test.
 
 Either use :orchestrator test, which tests the multi-threading components,
 :server_test, which extends this to test grpc_components, or run it locally
 to debug hangs due to bugs in threads (it is easier to debug with live logs).
 """
 
 import dataclasses
 import functools
+import itertools
 import logging
+import os
 import queue
+import signal
+import sys
 import threading
 import time
-from typing import Any, Iterable, Optional, Union
+import traceback
+from typing import Any, AsyncIterator, Optional, Union
 
 import grpc
 import jax
-import numpy as np
-
-from jetstream.engine import engine_api
-from jetstream.engine import token_utils
 from jetstream.core.proto import jetstream_pb2
 from jetstream.core.proto import jetstream_pb2_grpc
+from jetstream.core.utils import async_multifuture
+from jetstream.engine import engine_api
+from jetstream.engine import token_utils
+import numpy as np
+
+
+root = logging.getLogger()
+root.setLevel(logging.DEBUG)
+
+handler = logging.StreamHandler(sys.stdout)
+handler.setLevel(logging.DEBUG)
+formatter = logging.Formatter(
+    "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+)
+handler.setFormatter(formatter)
+root.addHandler(handler)
+
+
+def delete_pytree(p):
+  def delete_leaf(leaf):
+    if isinstance(leaf, jax.Array):
+      leaf.delete()
+    del leaf
+
+  jax.tree_map(delete_leaf, p)
 
 
 @dataclasses.dataclass
 class ActiveRequest:
   """Current state of the driver."""
+
   #################### Information relevant for generation #####################
   max_tokens: int
+  # We keep prefill and decode information together in the same object so that
+  # there is less indirection about where this return channel is.
+  # The return channel returns a list of strings, one per sample for that query.
+  return_channel: async_multifuture.AsyncMultifuture[list[str]]
   # [num_samples,] which corresponds to whether each sample is complete for the
   # requests.
   complete: Optional[np.ndarray] = None
   prefill_result: Any = None
   #################### Information relevant for prefill ########################
   history_path: Optional[str] = None
   prefill_text: Optional[str] = None
-  ################## Information relevant for detokenisation ###################
+  ################## Information relevant for detokenization ###################
   # Which generate step this was added at.
   generate_timestep_added: Optional[int] = None
-  # We keep prefill and decode information together in the same object so that
-  # there is less indirection about where this return channel is.
-  # The return channel returns a list of strings, one per sample for that query.
-  return_channel: queue.Queue[list[str]] = dataclasses.field(
-      default_factory=queue.Queue
-  )
-
-  def next(self: 'ActiveRequest'):
-    """Blocks until the next token is available, call from RPC threads."""
-    return self.return_channel.get()
 
   def enqueue_tokens(self, generated_tokens: list[str]):
     """Records information about the step.
 
     Args:
       generated_tokens: One token to put into the return channel
 
     This should be called only from within the Drivers background thread.
     """
-    self.return_channel.put(generated_tokens)
+    self.return_channel.add_result(generated_tokens)
+
+
+class JetThread(threading.Thread):
+  """Thread that kills the program if it fails.
+
+  If a driver thread goes down, we can't operate.
+  """
+
+  def run(self):
+    try:
+      super().run()
+    except Exception as e:  # pylint: disable=broad-exception-caught
+      print(f"Thread {self.name} encountered an error: {e}")
+      traceback.print_exc()
+      os.kill(os.getpid(), signal.SIGKILL)
+
+
+async def _abort_or_raise(
+    context: grpc.aio.ServicerContext | None,
+    code: grpc.StatusCode,
+    details: str,
+):
+  """Safely aborts a gRPC context if available, or raises an Exception."""
+  if context is None:
+    raise RuntimeError(details)
+
+  await context.abort(code, details)
 
 
 class Driver:
   """Drives the engines."""
 
   _prefill_engines: list[engine_api.Engine]
   _generate_engines: list[engine_api.Engine]
   # Allows us to pre-load the params, primarily so that we can iterate quickly
   # on the driver in colab without reloading weights.
-  _prefill_params: Optional[dict[int, Any]] = {}
-  _generate_params: Optional[dict[int, Any]] = {}
+  _prefill_params: list[Any]
+  _generate_params: list[Any]
   # Stage 1
-  _prefill_backlog: queue.Queue[ActiveRequest]
+  _prefill_backlog: queue.Queue[ActiveRequest | None]
   # Stage 2
-  _transfer_backlog: queue.Queue[ActiveRequest]
-  # Stage 3
   # We keep this as a dict to avoid a possibly expensive object comparison
   # when logging the index of the generate engine we send a prefill result
   # to, it allows us to natively have the index from the min operation, rather
   # than have to call .index()
-  _generate_backlogs: dict[int, queue.Queue[ActiveRequest]] = {}
-  # Stage 4
+  _generate_backlogs: dict[int, queue.Queue[ActiveRequest | None]] = {}
+  # Stage 3
   # This can be a list because we can pass it as an arg to generate and
   # detokenize threads. It is a list of tokens to be detokenized.
   _detokenize_backlogs: list[queue.Queue[engine_api.ResultTokens]] = []
   _generate_slots: list[queue.Queue[int]] = []
-  _active_requests: list[queue.Queue[tuple[int, ActiveRequest]]] = []
+  _active_requests: list[queue.Queue[tuple[int, ActiveRequest | None]]] = []
 
   def __init__(
       self,
-      prefill_engines=None,
-      generate_engines=None,
-      prefill_params=None,
-      generate_params=None,
+      prefill_engines: Optional[list[engine_api.Engine]] = None,
+      generate_engines: Optional[list[engine_api.Engine]] = None,
+      prefill_params: Optional[list[Any]] = None,
+      generate_params: Optional[list[Any]] = None,
   ):
+    if prefill_engines is None:
+      prefill_engines = []
+    if generate_engines is None:
+      generate_engines = []
+    if prefill_params is None:
+      prefill_params = []
+    if generate_params is None:
+      generate_params = []
+
     logging.info(
-        'Initialising driver with %d prefill engines and %d generate engines.',
+        "Initialising driver with %d prefill engines and %d generate engines.",
         len(prefill_engines),
         len(generate_engines),
     )
     self._prefill_engines = prefill_engines
     self._generate_engines = generate_engines
-    self._prefill_params = prefill_params if prefill_params else {}
-    self._generate_params = generate_params if generate_params else {}
+    self._prefill_params = prefill_params
+    self._generate_params = generate_params
     # Stages 1-4 represent the life cycle of a request.
     # Stage 1
     # At first, a request is placed here in order to get prefilled.
     self._prefill_backlog = queue.Queue()
+    # _ready_to_prefill event will block the prefill thread until there is
+    # available decode slot to insert the prefill result.
+    self._ready_to_prefill = threading.Event()
     # Stage 2
-    # After prefilling, it is placed here in order to get transferred to
-    # one of the generate backlogs.
-    self._transfer_backlog = queue.Queue()
-    # Stage 3
     # Each generate engine accesses its own generate backlog.
     self._generate_backlogs = {
-        idx: queue.Queue() for idx, _ in enumerate(generate_engines)
+        # Don't receive more than 1/3 the number of concurrent decodes to avoid
+        # OOM for single host.
+        idx: queue.Queue(engine.max_concurrent_decodes // 3)
+        for idx, engine in enumerate(self._generate_engines)
     }
-    # Stage 4
+    # Stage 3
     # After generation, ActiveRequests are placed on the detokenization backlog
     # for tokens to be sent into each ActiveRequest's return channel.
     # We have one of these per generate engine to simplify the logic keeping
     # track of which generation engine to replace slots on.
     # This is a queue of either - tuple[int, ActiveRequest] which represents our
     # active requests, or tuple[int, sample_tokens]. We combine these into one
     # queue because it allows us to be somewhat clever with how we do
     # detokenization.
     # If the detokenization receives an (int, ActiveRequest) this signifies
     # that slot int should from now be placing tokens in the return channel of
     # the ActiveRequest.
     # If it receives (int, sample_tokens) then it actually
-    # does a detokenisation for any slots which have previously been set active
+    # does a detokenization for any slots which have previously been set active
     # via the previous kind of object, and the int is used to log which step
     # the tokens were created at. By having them in one queue we prevent
     # the possibility of race conditions where a slot is made live before the
     # tokens are ready and it receives tokens from a different sequence,
     # or tokens detokenized before the relevant slot is live.
-    self._detokenize_backlogs = [queue.Queue() for _ in generate_engines]
-    # Finally we have a queue that doesn't represent a stage, but tracks the
-    # internal status of a request within the generation loop.
-    # a) A queue of integers representing available 'slots' in the decode
-    #   operation. I.e. potentially available rows in the batch and/or
-    #   microbatch. When we want to insert a prefill result, we pop an integer
-    #   to insert at. When this is empty, it means all slots are full.
-
-    # Construct a)
-    self._generate_slots = [queue.Queue() for _ in generate_engines]
-    _ = [[self._generate_slots[idx].put(i)
-          for i in range(engine.max_concurrent_decodes)]
-         for idx, engine in enumerate(generate_engines)]
+    self._detokenize_backlogs = [
+        # We don't let detokenization accumulate more than 8 steps to avoid
+        # synchronization issues.
+        queue.Queue(8)
+        for _ in self._generate_engines
+    ]
 
-    # Kick off all our threads
+    # A queue of integers representing available 'slots' in the decode
+    # operation. I.e. potentially available rows in the batch and/or microbatch.
+    # When we want to insert a prefill result, we pop an integer to insert at.
+    # When this is empty, it means all slots are full.
+    self._generate_slots = [
+        queue.Queue(engine.max_concurrent_decodes)
+        for engine in self._generate_engines
+    ]
+    _ = [
+        [
+            self._generate_slots[idx].put(i)
+            for i in range(engine.max_concurrent_decodes)
+        ]
+        for idx, engine in enumerate(self._generate_engines)
+    ]
+
+    # Create all threads
     self._prefill_threads = [
-        threading.Thread(
-            target=functools.partial(self._prefill_thread, idx, engine)
+        JetThread(
+            target=functools.partial(self._prefill_thread, idx),
+            name=f"prefill-{idx}",
         )
-        for idx, engine in enumerate(self._prefill_engines)
+        for idx in range(len(self._prefill_engines))
     ]
-    self._transfer_thread = threading.Thread(target=self._transfer_thread)
     self._generate_threads = [
-        threading.Thread(
+        JetThread(
             target=functools.partial(
                 self._generate_thread,
                 idx,
-                engine,
-                self._generate_slots[idx],
-                self._detokenize_backlogs[idx],
-            )
+            ),
+            name=f"generate-{idx}",
         )
-        for idx, engine in enumerate(self._generate_engines)
+        for idx in range(len(self._generate_engines))
     ]
-    # Construct b)
     self.detokenize_threads = [
-        threading.Thread(
+        JetThread(
             target=functools.partial(
                 self._detokenize_thread,
                 idx,
-                engine,
-                self._generate_slots[idx],
-                self._detokenize_backlogs[idx],
-            )
+            ),
+            name=f"detokenize-{idx}",
         )
-        for idx, engine in enumerate(self._generate_engines)
+        for idx in range(len(self._generate_engines))
     ]
+    self._all_threads = list(
+        itertools.chain(
+            self._prefill_threads,
+            self._generate_threads,
+            self.detokenize_threads,
+        )
+    )
     self.live = True
-    # Kick off all threads
-    _ = [f.start() for f in self._prefill_threads]
-    self._transfer_thread.start()
-    _ = [f.start() for f in self._generate_threads]
-    _ = [f.start() for f in self.detokenize_threads]
+    # Start all threads
+    for t in self._all_threads:
+      t.start()
+
+  def stop(self):
+    """Stops the driver and all background threads."""
+    # Signal to all threads that they should stop.
+    self.live = False
+
+    all_backlogs = list(
+        itertools.chain(
+            [self._prefill_backlog],
+            self._generate_backlogs.values(),
+            self._detokenize_backlogs,
+        )
+    )
+
+    while any(t.is_alive() for t in self._all_threads):
+      # Empty all backlogs and mark any remaining requests as cancelled.
+      for q in all_backlogs:
+        while True:
+          try:
+            r = q.get_nowait()
+            if r is None:
+              continue
+            elif isinstance(r, ActiveRequest):
+              r.return_channel = None
+            else:  # detokenize backlog
+              _, r = r
+              if isinstance(r, ActiveRequest):
+                r.return_channel = None
+          except queue.Empty:
+            break
+
+      # Put sentinels to unblock threads.
+      for q in all_backlogs:
+        try:
+          q.put_nowait(None)
+        except queue.Full:
+          pass
+
+    # Wait for all threads to stop.
+    for t in self._all_threads:
+      t.join()
+
+  def get_total_concurrent_requests(self) -> int:
+    """Gets the total number of concurrent requests the driver can handle."""
+    # We don't support filling all backlogs at once because it can cause GIL
+    # contention.
+    total_max_concurrent_decodes = sum(
+        [e.max_concurrent_decodes for e in self._generate_engines]
+    )
+    return total_max_concurrent_decodes
 
   def place_request_on_prefill_queue(self, request: ActiveRequest):
     """Used to place new requests for prefilling and generation."""
-    self._prefill_backlog.put(request)
+    # Don't block so we can fail and shed load when the queue is full.
+    self._prefill_backlog.put(request, block=False)
 
   def _load_cache_history(self, path: str) -> Union[None, Any]:
     """Loads previous kv cache for a longer conversation."""
     if path:
       raise NotImplementedError
     else:
       return None
 
-  def _prefill_thread(self, idx: int, prefill_engine: engine_api.Engine,
-                      transfer_backpressure: int = 8):
+  def _prefill_thread(self, idx: int):
     """Thread which runs in the background performing prefills."""
-    logging.info('---------Spinning up prefill thread %d.---------', idx)
+    logging.info("---------Spinning up prefill thread %d.---------", idx)
+    prefill_engine = self._prefill_engines[idx]
     prefill_params = self._prefill_params[idx]
     metadata = prefill_engine.get_tokenizer()
     vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
-    logging.info('---------Prefill params %d loaded.---------', idx)
-
-    while self.live:
-      # We don't want to keep lots of kv caches live in memory on the prefill
-      # slice that aren't about to be sent over to a generation slice.
-      if (self._transfer_backlog.qsize() < transfer_backpressure):
-        # Check if there is anything on the prefill backlog, pop if so.
-        try:
-          request = self._prefill_backlog.get(block=True)
-          # TODO: Implement hot/cold cache for history.
-          history = self._load_cache_history(request.history_path)  # pylint: disable = assignment-from-none
-          # Tokenize, and introduce a leading dimension
-          is_bos = not bool(request.history_path)
-          logging.info('Prefilling on prefill engine %d : "%s", prefill queue size, %d, is_bos: %s, history: %s', idx, request.prefill_text, self._prefill_backlog.qsize(), is_bos, request.history_path)  # pylint: disable = line-too-long
-          padded_tokens, true_length = token_utils.tokenize_and_pad(
-              request.prefill_text,
-              vocab,
-              is_bos=is_bos,
-              max_prefill_length=prefill_engine.max_prefill_length,
-          )
-          # Compute new kv cache for the prefill_text, conditional on
-          # history.
-          prefill_result = prefill_engine.prefill(
-              params=prefill_params,
-              existing_prefix=history,
-              padded_tokens=padded_tokens,
-              true_length=true_length,
-          )
-          jax.block_until_ready(prefill_result)
-          request.prefill_result = prefill_result
-          # Once prefill is complete, place it on the generation queue.
-          self._transfer_backlog.put(request)
-          logging.info(
-              'Placed request "%s" on the transfer queue.', request.prefill_text
-          )
-        except queue.Empty:
-          # Otherwise, don't do anything!
-          pass
+    logging.info("---------Prefill params %d loaded.---------", idx)
 
-  def _transfer_thread(self, generation_backpressure: int = 8):
-    """Transfers the kv cache on an active request to the least full generate backlog."""
     while self.live:
-      # We don't want to keep lots of kv caches live in memory on a generate
-      # slice that haven't been inserted
-      if (
-          sum([backlog.qsize() for backlog in self._generate_backlogs.values()])
-          < generation_backpressure
-      ):
-        try:
-          new_request = self._transfer_backlog.get(block=True)
-
-          # Get the index of the generate queue with the minimmum qsize.
-          idx = min(
-              self._generate_backlogs.items(), key=lambda q: q[1].qsize()
-          )[0]
-          logging.info(
-              'Transferring "%s" to generate engine %d.',
-              new_request.prefill_text,
-              idx,
-          )
-          # Transfer the info to the relevant generate backlog.
-          new_request.prefill_result = jax.device_put(
-              new_request.prefill_result,
-              self._generate_engines[idx].get_prefix_destination_sharding(),
-          )
-          # Place the request on the correct generate backlog.
-          self._generate_backlogs[idx].put(new_request)
-          logging.info(
-              'Request "%s" tsuccessfully transferrred to generate engine %d.',
-              new_request.prefill_text,
-              idx,
-          )
-        except queue.Empty:
-          pass
+      # The prefill thread can wait until there is available decode slot to
+      # insert.
+      if self._generate_slots[idx].qsize() == 0:
+        logging.info(
+            "Prefill waits for available slot; prefill queue size %d",
+            self._prefill_backlog.qsize(),
+        )
+        self._ready_to_prefill.wait()
+        logging.info(
+            "Prefill continues; prefill queue size %d",
+            self._prefill_backlog.qsize(),
+        )
+      # The prefill thread can just sleep until it has work to do.
+      request = self._prefill_backlog.get(block=True)
+      if request is None:
+        break
+      # TODO: Implement hot/cold cache for history.
+      history = self._load_cache_history(request.history_path)  # pylint: disable = assignment-from-none
+      # Tokenize, and introduce a leading dimension
+      is_bos = not bool(request.history_path)
+      logging.info(
+          "Prefilling on prefill engine %d : prefill queue size, %d,"
+          " is_bos: %s, history: %s",
+          idx,
+          self._prefill_backlog.qsize(),
+          is_bos,
+          request.history_path,
+      )
+      padded_tokens, true_length = token_utils.tokenize_and_pad(
+          request.prefill_text,
+          vocab,
+          is_bos=is_bos,
+          max_prefill_length=prefill_engine.max_prefill_length,
+      )
+      # Compute new kv cache for the prefill_text, conditional on
+      # history.
+      prefill_result = prefill_engine.prefill(
+          params=prefill_params,
+          existing_prefix=history,
+          padded_tokens=padded_tokens,
+          true_length=true_length,
+      )
+      request.prefill_result = prefill_result
+      # Once prefill is complete, place it on the generation queue and block if
+      # full.
+      self._generate_backlogs[idx].put(request, block=True)
+      logging.info(
+          "Placed request on the generate queue, generate_backlogs=%d",
+          self._generate_backlogs[idx].qsize(),
+      )
 
-  def _generate_thread(
-      self,
-      idx: int,
-      generate_engine: engine_api.Engine,
-      my_slots: queue.Queue[int],
-      my_detokenize_backlog: queue.Queue[tuple[int, engine_api.ResultTokens]],
-      backpressure: int = 3,
-  ):
-    """Step token generation and insert prefills from backlog.
+  def _generate_thread(self, idx: int):
+    """Step token generation and insert prefills from backlog."""
+    logging.info("---------Spinning up generate thread %d.---------", idx)
+    generate_engine = self._generate_engines[idx]
+    my_slots = self._generate_slots[idx]
+    my_generate_backlog = self._generate_backlogs[idx]
+    my_detokenize_backlog = self._detokenize_backlogs[idx]
 
-    Args:
-      idx: Idx corresponding to which generation engine idx this is.
-      generate_engine: The generate engine corresponding to this thread.
-      my_slots: Integers representing free my_slots.
-      my_detokenize_backlog: Detokenize backlog for this generate engine.
-      backpressure: How many steps we can queue up before pausing, allows us to
-        hide dispatch times because jit calls are dispatched one after another.
-        We have this in the first place because we don't want to enqueue
-        thousands of steps.
-    """
-    logging.info('---------Spinning up generate thread %d.---------', idx)
     # Keep track of what step tokens were generated at.
     generate_timestep = 0
     # State to store things like running kv cache in.
     decode_state = generate_engine.init_decode_state()
     generate_params = self._generate_params[idx]
-    logging.info('---------Generate params %d loaded.---------', idx)
+    logging.info("---------Generate params %d loaded.---------", idx)
     time_of_last_generate = time.time()
+    time_of_last_print = time.time()
     while self.live:
-      # Check if there are any free my_slots.
-      if not my_slots.empty() and not self._generate_backlogs[idx].empty():
-        # Only get requests from the backlog corresponding to this engine.
-        new_request = self._generate_backlogs[idx].get()
-        slot = my_slots.get()
+      if (time.time() - time_of_last_print) > 1:
         logging.info(
-            'Generate slice %d slot %d step %d,'
-            ' generating for : "%s"', idx, slot, generate_timestep,
-            new_request.prefill_text,
+            "Generate thread making a decision with:"
+            " prefill_backlog=%d"
+            " generate_free_slots=%d",
+            self._prefill_backlog.qsize(),
+            my_slots.qsize(),
+        )
+        time_of_last_print = time.time()
+
+      max_concurrent_decodes = generate_engine.max_concurrent_decodes
+
+      # TODO: Move insert to prefill thread.
+      # Check if there are any free my_slots. We don't want to block here since
+      # we can still generate if we can't insert. We do this in a while loop to
+      # insert as many sequences as possible.
+      while True:
+        my_slots_size = my_slots.qsize()
+
+        try:
+          slot = my_slots.get(block=False)
+          # Found a slot, now see if we can fill it.
+        except queue.Empty:
+          # Exit this while loop as we have no free slots to insert into.
+          break
+
+        # We block when the decode slots are all free since we need to get a
+        # prefilled request to insert. We add timeout for the block to handle
+        # the case when the prefill backlog is cancelled and we end up with no
+        # more useful prefill work to do.
+        block = my_slots_size == max_concurrent_decodes
+        try:
+          new_request = my_generate_backlog.get(block=block, timeout=1.0)
+          # Got free slot and new request, use them.
+        except queue.Empty:
+          # No new requests, we can't insert, so put back slot.
+          my_slots.put(slot, block=False)
+          # If we were blocking and hit the timeout, then retry the loop.
+          # Otherwise, we can exit and proceed to generation.
+          if block:
+            continue
+          else:
+            break
+
+        # Signal to kill the thread.
+        if new_request is None:
+          return
+
+        logging.info(
+            "Generate slice %d filling slot %d at step %d.",
+            idx,
+            slot,
+            generate_timestep,
         )
         decode_state = generate_engine.insert(
-            new_request.prefill_result, decode_state,
-            slot=slot
+            new_request.prefill_result, decode_state, slot=slot
         )
+        delete_pytree(new_request.prefill_result)
         new_request.generate_timestep_added = generate_timestep
         new_request.complete = np.zeros(
             (generate_engine.samples_per_slot,), dtype=np.bool_
         )
-        my_detokenize_backlog.put((slot, new_request))
+        # Respond to detokenization backpressure.
+        my_detokenize_backlog.put((slot, new_request), block=True)
 
-      if my_detokenize_backlog.qsize() < backpressure:
-        decode_state, sampled_tokens = generate_engine.generate(
-            generate_params, decode_state
-        )
-        sampled_tokens.copy_to_host_async()
-        my_detokenize_backlog.put((generate_timestep, sampled_tokens))
-        generate_timestep += 1
-        logging.info(
-            'Generate engine %d step %d - slots free : %d / %d, took %.2fms',
-            idx,
-            generate_timestep,
-            my_slots.qsize(),
-            generate_engine.max_concurrent_decodes,
-            (time.time() - time_of_last_generate)*10**3,
-        )
-        time_of_last_generate = time.time()
+      # At this point, we know that we have at least some slots filled.
+      assert (
+          my_slots.qsize() < max_concurrent_decodes
+      ), "At this point we must have some requests inserted into the slots."
+
+      # Now we actually take a generate step on requests in the slots.
+      decode_state, sampled_tokens = generate_engine.generate(
+          generate_params, decode_state
+      )
+      sampled_tokens.copy_to_host_async()
+      # Respond to detokenization backpressure.
+      my_detokenize_backlog.put((generate_timestep, sampled_tokens), block=True)
+      generate_timestep += 1
+      logging.info(
+          "Generate engine %d step %d - slots free : %d / %d, took %.2fms",
+          idx,
+          generate_timestep,
+          my_slots_size,
+          max_concurrent_decodes,
+          (time.time() - time_of_last_generate) * 10**3,
+      )
+      time_of_last_generate = time.time()
 
-  def _detokenize_thread(
-      self,
-      idx: int,
-      generate_engine: engine_api.Engine,
-      my_slots: queue.Queue[int],
-      my_detokenize_backlog: queue.Queue[
-          Union[tuple[int, engine_api.ResultTokens], tuple[int, ActiveRequest]]
-      ],
-  ):
+  def _detokenize_thread(self, idx: int):
     """Detokenize sampled tokens and returns them to the user."""
-    del idx
     # One of these per generate engine.
     # For all filled my_slots, pop the sampled token onto the relevant
     # requests return channel. If it done, place it back onto free slots.
-    metadata = generate_engine.get_tokenizer()
+    my_detokenize_backlog = self._detokenize_backlogs[idx]
+    my_generate_engine = self._generate_engines[idx]
+    my_slots = self._generate_slots[idx]
+
+    metadata = my_generate_engine.get_tokenizer()
     vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
 
     my_live_requests = {
-        i: None for i in range(generate_engine.max_concurrent_decodes)
+        i: None for i in range(my_generate_engine.max_concurrent_decodes)
     }
-
     while self.live:
-      try:
-        data = my_detokenize_backlog.get(block=True)
-        start_detokenise_time = time.time()
-        if isinstance(data[1], engine_api.ResultTokens):
-          # We want to detokenise them.
-          generate_timestep_added, result_tokens = data
-          # Disable attribute error because pytype doesn't know this
-          # is a result tokens, and we can't annotate the tuple.
-          result_tokens = result_tokens.convert_to_numpy()  # pytype: disable=attribute-error
-
-          for slot, request in my_live_requests.items():
-            if request is not None:
-              results, complete = token_utils.process_result_tokens(
-                  slot=slot,
-                  slot_max_length=request.max_tokens,
-                  result_tokens=result_tokens,
-                  vocab=vocab,
-                  complete=request.complete,
-              )
-              request.complete = complete
-              # Return some tokens.
-              request.enqueue_tokens(results)
-              if request.complete.all():
-                # Place the slot back on the free queue.
-                my_live_requests[slot] = None
-                my_slots.put(slot)
-          logging.info(
-              'Detokenising generate step %d took %.2fms',
-              generate_timestep_added,
-              (time.time() - start_detokenise_time) * 10**3,
-          )
-        else:
-          # We want to update a slot with the new channel.
-          slot, active_request = data
-          my_live_requests[slot] = active_request
-
-      except queue.Empty:
-        # Nothing to detokenize!
-        pass
+      data = my_detokenize_backlog.get(block=True)
+      if data is None:
+        break
+      start_detokenize_time = time.time()
+      if isinstance(data[1], engine_api.ResultTokens):
+        # We want to detokenize them.
+        generate_timestep_added, result_tokens = data
+        # Disable attribute error because pytype doesn't know this
+        # is a result tokens, and we can't annotate the tuple.
+        result_tokens = result_tokens.convert_to_numpy()
+
+        for slot, request in my_live_requests.items():
+          if request is not None:
+            results, complete = token_utils.process_result_tokens(
+                slot=slot,
+                slot_max_length=request.max_tokens,
+                result_tokens=result_tokens,
+                vocab=vocab,
+                complete=request.complete,
+            )
+            request.complete = complete
+            # Return some tokens.
+            request.enqueue_tokens(results)
+            if request.complete.all():
+              request.return_channel.close()
+              # Place the slot back on the free queue.
+              my_live_requests[slot] = None
+              my_slots.put(slot, block=False)  # This should always have space.
+              self._ready_to_prefill.set()
+        logging.info(
+            "Detokenizing generate step %d took %.2fms",
+            generate_timestep_added,
+            (time.time() - start_detokenize_time) * 10**3,
+        )
+      else:
+        # We want to update a slot with the new channel.
+        slot, active_request = data
+        my_live_requests[slot] = active_request
 
 
 class LLMOrchestrator(jetstream_pb2_grpc.OrchestratorServicer):
   """Coordinates a set of prefill and generate slices for LLM decoding."""
 
   _driver: Driver
 
   def __init__(self, driver: Driver):
     self._driver = driver
 
-  def Decode(
+  async def Decode(  # pylint: disable=invalid-overridden-method
       self,
       request: jetstream_pb2.DecodeRequest,
-      context: Optional[grpc.ServicerContext] = None,
-  ) -> Iterable[jetstream_pb2.DecodeResponse]:
+      context: Optional[grpc.aio.ServicerContext] = None,
+  ) -> AsyncIterator[jetstream_pb2.DecodeResponse]:
     """Decode."""
     if context is None:
       logging.warning(
-          'LLM orchestrator is being used in offline test mode, and will not'
-          ' respond to gRPC queries - only direct function calls.'
+          "LLM orchestrator is being used in offline test mode, and will not"
+          " respond to gRPC queries - only direct function calls."
       )
+    return_channel = async_multifuture.AsyncMultifuture()
+    if context:
+      context.add_done_callback(return_channel.cancel)
     # Wrap request as an ActiveRequest.
     active_request = ActiveRequest(
         max_tokens=request.max_tokens,
         history_path=request.session_cache,
         prefill_text=request.additional_text,
+        return_channel=return_channel,
     )
     # The first stage is being prefilled, all other stages are handled
     # inside the driver (transfer, generate*N, detokenize).
-    self._driver.place_request_on_prefill_queue(active_request)
+    try:
+      self._driver.place_request_on_prefill_queue(active_request)
+    except queue.Full:
+      # Safely abort the gRPC server thread with a retriable error.
+      await _abort_or_raise(
+          context=context,
+          code=grpc.StatusCode.RESOURCE_EXHAUSTED,
+          details=(
+              "The driver prefill queue is full and more requests cannot be"
+              " handled. You may retry this request."
+          ),
+      )
     logging.info(
-        'Placed request with text "%s" on the prefill queue.',
-        active_request.prefill_text,
+        "Placed request on the prefill queue.",
     )
-
-    while True:
+    async for response in active_request.return_channel:
       # When an active request is created a queue is instantiated. New tokens
       # are placed there during the decoding loop, we pop from that queue by
       # using the .next method on the active request.
       # Yielding allows for the response to be a streaming grpc call - which
       # can be called via iterating over a for loop on the other side.
-      yield jetstream_pb2.DecodeResponse(response=active_request.next())
-      if active_request.complete:
-        break
+      # The DecodeResponse stream should consume all generated tokens in
+      # return_channel when complete signal is received. It should check if
+      # return_channel is empty to decide if it should exit the while loop.
+      yield jetstream_pb2.DecodeResponse(response=response)
```

### Comparing `google-jetstream-0.1.1/jetstream/core/orchestrator_test.py` & `google-jetstream-0.2.0/jetstream/core/orchestrator_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 I.e. ['Ċ', 'Ō', 'Ɵ'] when converted back with chr().
 
 Therefore we should get back the character sequence '$lǔ' if we request 3 tokens
 decoded (these are the ascii chars at those indices which is what the test
 tokenizer returns).
 """
 
-from jetstream.engine import mock_engine
+from absl.testing import absltest
 from jetstream.core import orchestrator
 from jetstream.core.proto import jetstream_pb2
-from absl.testing import absltest
+from jetstream.engine import mock_engine
 
 
 class OrchestratorTest(absltest.TestCase):
 
   def _setup_driver(self):
     prefill_engine = mock_engine.TestEngine(
         batch_size=32, cache_length=256, weight=2.0
@@ -57,41 +57,47 @@
     # so that we can test that the right one is in use at a given time.
     generate_engine = mock_engine.TestEngine(
         batch_size=4, cache_length=32, weight=4.0
     )
     driver = orchestrator.Driver(
         prefill_engines=[prefill_engine],
         generate_engines=[generate_engine],
+        prefill_params=[prefill_engine.load_params()],
+        generate_params=[generate_engine.load_params()],
     )
     return driver
 
-  def test_orchestrator(self):
+  async def test_orchestrator(self):
     """Test the multithreaded orchestration."""
     driver = self._setup_driver()
     client = orchestrator.LLMOrchestrator(driver=driver)
 
     # The string representation of np.array([[65, 66]]), [2] will be prepend
     # as BOS.
-    text = 'AB'
+    text = "AB"
 
     request = jetstream_pb2.DecodeRequest(
-        session_cache='',
+        session_cache="",
         additional_text=text,
         priority=1,
         max_tokens=3,
     )
     iterator = client.Decode(request)
     # chr of [266, 332, 415].
-    expected_tokens = ['Ċ', 'Ō', 'Ɵ', '']
+    expected_tokens = ["Ċ", "Ō", "Ɵ", ""]
     counter = 0
-    for token in iterator:
+    async for token in iterator:
       # Tokens come through as bytes.
-      print('actual output: ' + bytes(token.response[0], encoding='utf-8').decode())
+      print(
+          "actual output: "
+          + bytes(token.response[0], encoding="utf-8").decode()
+      )
       assert (
-          bytes(token.response[0], encoding='utf-8').decode()
+          bytes(token.response[0], encoding="utf-8").decode()
           == expected_tokens[counter]
       )
       counter += 1
+    driver.stop()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.1.1/jetstream/core/proto/__init__.py` & `google-jetstream-0.2.0/jetstream/core/proto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/core/proto/jetstream_pb2.py` & `google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,33 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: jetstream/core/proto/jetstream.proto
 # Protobuf Python Version: 4.25.1
+# pylint: disable=all
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$jetstream/core/proto/jetstream.proto\x12\x0fjetstream_proto\"e\n\rDecodeRequest\x12\x15\n\rsession_cache\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64itional_text\x18\x02 \x01(\t\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x12\n\nmax_tokens\x18\x04 \x01(\x05\"\"\n\x0e\x44\x65\x63odeResponse\x12\x10\n\x08response\x18\x01 \x03(\t2]\n\x0cOrchestrator\x12M\n\x06\x44\x65\x63ode\x12\x1e.jetstream_proto.DecodeRequest\x1a\x1f.jetstream_proto.DecodeResponse\"\x00\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n$jetstream/core/proto/jetstream.proto\x12\x0fjetstream_proto"e\n\rDecodeRequest\x12\x15\n\rsession_cache\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64itional_text\x18\x02 \x01(\t\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x12\n\nmax_tokens\x18\x04 \x01(\x05""\n\x0e\x44\x65\x63odeResponse\x12\x10\n\x08response\x18\x01 \x03(\t2]\n\x0cOrchestrator\x12M\n\x06\x44\x65\x63ode\x12\x1e.jetstream_proto.DecodeRequest\x1a\x1f.jetstream_proto.DecodeResponse"\x00\x30\x01\x62\x06proto3'
+)
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'jetstream.core.proto.jetstream_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(
+    DESCRIPTOR, "jetstream.core.proto.jetstream_pb2", _globals
+)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_DECODEREQUEST']._serialized_start=57
-  _globals['_DECODEREQUEST']._serialized_end=158
-  _globals['_DECODERESPONSE']._serialized_start=160
-  _globals['_DECODERESPONSE']._serialized_end=194
-  _globals['_ORCHESTRATOR']._serialized_start=196
-  _globals['_ORCHESTRATOR']._serialized_end=289
+  _globals["_DECODEREQUEST"]._serialized_start = 57
+  _globals["_DECODEREQUEST"]._serialized_end = 158
+  _globals["_DECODERESPONSE"]._serialized_start = 160
+  _globals["_DECODERESPONSE"]._serialized_end = 194
+  _globals["_ORCHESTRATOR"]._serialized_start = 196
+  _globals["_ORCHESTRATOR"]._serialized_end = 289
 # @@protoc_insertion_point(module_scope)
```

### Comparing `google-jetstream-0.1.1/jetstream/core/proto/jetstream_pb2_grpc.py` & `google-jetstream-0.2.0/jetstream/core/proto/jetstream_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,79 +9,86 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+# pylint: disable=all
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from jetstream.core.proto import jetstream_pb2 as jetstream_dot_core_dot_proto_dot_jetstream__pb2
 
 
 class OrchestratorStub(object):
-    """TODO: Merge this with main JetStream core once we settle on an API.
+  """TODO: Merge this with main JetStream core once we settle on an API."""
 
-    """
-
-    def __init__(self, channel):
-        """Constructor.
+  def __init__(self, channel):
+    """Constructor.
 
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.Decode = channel.unary_stream(
-                '/jetstream_proto.Orchestrator/Decode',
-                request_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.SerializeToString,
-                response_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.FromString,
-                )
+    Args:
+        channel: A grpc.Channel.
+    """
+    self.Decode = channel.unary_stream(
+        "/jetstream_proto.Orchestrator/Decode",
+        request_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.SerializeToString,
+        response_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.FromString,
+    )
 
 
 class OrchestratorServicer(object):
-    """TODO: Merge this with main JetStream core once we settle on an API.
+  """TODO: Merge this with main JetStream core once we settle on an API."""
 
-    """
-
-    def Decode(self, request, context):
-        """Generate the next model tokens.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+  def Decode(self, request, context):
+    """Generate the next model tokens."""
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details("Method not implemented!")
+    raise NotImplementedError("Method not implemented!")
 
 
 def add_OrchestratorServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'Decode': grpc.unary_stream_rpc_method_handler(
-                    servicer.Decode,
-                    request_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.FromString,
-                    response_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'jetstream_proto.Orchestrator', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
+  rpc_method_handlers = {
+      "Decode": grpc.unary_stream_rpc_method_handler(
+          servicer.Decode,
+          request_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.FromString,
+          response_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.SerializeToString,
+      ),
+  }
+  generic_handler = grpc.method_handlers_generic_handler(
+      "jetstream_proto.Orchestrator", rpc_method_handlers
+  )
+  server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class Orchestrator(object):
-    """TODO: Merge this with main JetStream core once we settle on an API.
-
-    """
+  """TODO: Merge this with main JetStream core once we settle on an API."""
 
-    @staticmethod
-    def Decode(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/jetstream_proto.Orchestrator/Decode',
-            jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.SerializeToString,
-            jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+  @staticmethod
+  def Decode(
+      request,
+      target,
+      options=(),
+      channel_credentials=None,
+      call_credentials=None,
+      insecure=False,
+      compression=None,
+      wait_for_ready=None,
+      timeout=None,
+      metadata=None,
+  ):
+    return grpc.experimental.unary_stream(
+        request,
+        target,
+        "/jetstream_proto.Orchestrator/Decode",
+        jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.SerializeToString,
+        jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.FromString,
+        options,
+        channel_credentials,
+        insecure,
+        call_credentials,
+        compression,
+        wait_for_ready,
+        timeout,
+        metadata,
+    )
```

### Comparing `google-jetstream-0.1.1/jetstream/core/server_test.py` & `google-jetstream-0.2.0/jetstream/core/server_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,83 +14,85 @@
 
 """Tests gRPC server end-to-end.
 
 See orchestrator test for why these characters specifically will be the
 response.
 """
 
-from typing import Any
+from typing import Any, Type
 
+from absl.testing import absltest, parameterized
 import grpc
-import portpicker
-
 from jetstream.core import config_lib
 from jetstream.core import server_lib
 from jetstream.core.proto import jetstream_pb2
 from jetstream.core.proto import jetstream_pb2_grpc
-from absl.testing import absltest, parameterized
+import portpicker
 
 
 class ServerTest(parameterized.TestCase):
 
   @parameterized.parameters(
       # Uses weight 2 for prefill, 4 for decode.
       (
           config_lib.CPUTestServer,
-          ['Ċ', 'Ō', 'Ɵ', ''],
+          ["Ċ", "Ō", "Ɵ", ""],
           [None, None],
       ),
       # Uses the same prefill / generate weights (2).
       (
           config_lib.InterleavedCPUTestServer,
-          ['Ċ', 'Ə', 'ɖ', ''],
+          ["Ċ", "Ə", "ɖ", ""],
           [None],
       ),
   )
   def test_server(
       self,
-      config: config_lib.ServerConfig,
+      config: Type[config_lib.ServerConfig],
       expected_tokens: list[str],
       devices: list[Any],
   ):
     """Sets up a server and requests token responses."""
     ######################### Server side ######################################
     port = portpicker.pick_unused_port()
-    print('port: ' + str(port))
+    print("port: " + str(port))
     credentials = grpc.local_server_credentials()
 
-    _ = server_lib.run(
-        threads=25,
+    server = server_lib.run(
         port=port,
         config=config,
         devices=devices,
         credentials=credentials,
     )
     ###################### Requester side ######################################
     channel = grpc.secure_channel(
-        f'localhost:{port}', grpc.local_channel_credentials()
+        f"localhost:{port}", grpc.local_channel_credentials()
     )
     stub = jetstream_pb2_grpc.OrchestratorStub(channel)
 
     # The string representation of np.array([[65, 66]]), [2] will be prependd
     # as BOS
-    text = 'AB'
+    text = "AB"
     request = jetstream_pb2.DecodeRequest(
-        session_cache='',
+        session_cache="",
         additional_text=text,
         priority=1,
         max_tokens=3,
     )
     iterator = stub.Decode(request)
     counter = 0
     for token in iterator:
       # Tokens come through as bytes
-      print('actual output: ' + bytes(token.response[0], encoding='utf-8').decode())
+      print(
+          "actual output: "
+          + bytes(token.response[0], encoding="utf-8").decode()
+      )
       assert (
-          bytes(token.response[0], encoding='utf-8').decode()
+          bytes(token.response[0], encoding="utf-8").decode()
           == expected_tokens[counter]
       )
       counter += 1
+    server.stop()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/__init__.py` & `google-jetstream-0.2.0/jetstream/core/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/engine_api.py` & `google-jetstream-0.2.0/jetstream/engine/engine_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Defines the JetStream API.
 
 These functions are the accelerator functions which an outer sampling loop
-could want to call, enabling interleaved (continous batching) inference.
+could want to call, enabling interleaved (continuous batching) inference.
 """
 
 import abc
 from typing import Any, Optional, Tuple, Union
 
 from flax import struct
 import jax
@@ -40,18 +40,20 @@
 # Cpus asscociated with the mesh.
 CpuDevices = Any
 
 
 @struct.dataclass
 class SlotData:
   """Class to store slot data."""
+
   tokens: Union[jax.Array, np.ndarray]
   valid: Union[jax.Array, np.ndarray]
   lengths: Union[jax.Array, np.ndarray]
 
+
 # pylint: disable=g-doc-args
 @struct.dataclass
 class ResultTokens(abc.ABC):
   """Class to store returned tokens in.
 
   We store everything in one array, and keep indexes - because copying
   a single array to host is much faster.
@@ -74,48 +76,52 @@
   length_idx: tuple[int, int] = struct.field(
       pytree_node=False,
   )
   samples_per_slot: int = struct.field(
       pytree_node=False,
   )
 
-  def copy_to_host_async(self: 'ResultTokens') -> None:
+  def copy_to_host_async(self: "ResultTokens") -> None:
     """Copy to host asynchronously."""
     self.data.copy_to_host_async()
 
-  def convert_to_numpy(self: 'ResultTokens') -> 'ResultTokens':
+  def convert_to_numpy(self: "ResultTokens") -> "ResultTokens":
     """Converts to numpy."""
     return ResultTokens(
         np.array(self.data),
         self.tokens_idx,
         self.valid_idx,
         self.length_idx,
         self.samples_per_slot,
     )
 
-  def get_result_at_slot(
-      self, slot: int
-  ) -> SlotData:
+  def get_result_at_slot(self, slot: int) -> SlotData:
     """Returns the token at a given slot.
 
     Args:
       slot: An integer from [0, n) representing an index into the batch.
 
     Note: implementations of this method must correctly handle
     microbatches, if microbatches are used.
     """
     # Potentially get multiple beams for given slot.
     start_idx = slot * self.samples_per_slot
     end_idx = (slot + 1) * self.samples_per_slot
     # Mask out any non valid tokens.
     return SlotData(
-        tokens=self.data[start_idx:end_idx, self.tokens_idx[0]:self.tokens_idx[1]],
-        valid=self.data[start_idx:end_idx, self.valid_idx[0]:self.valid_idx[1]],
+        tokens=self.data[
+            start_idx:end_idx, self.tokens_idx[0] : self.tokens_idx[1]
+        ],
+        valid=self.data[
+            start_idx:end_idx, self.valid_idx[0] : self.valid_idx[1]
+        ],
         # Only get a 1D representation here
-        lengths=self.data[start_idx:end_idx, self.length_idx[0]:self.length_idx[1]][:, 0]
+        lengths=self.data[
+            start_idx:end_idx, self.length_idx[0] : self.length_idx[1]
+        ][:, 0],
     )
 
 
 class Engine(abc.ABC):
   """The computational core of the generative model server.
 
   Engine defines an API that models must adhere to as they plug into the
@@ -137,17 +143,15 @@
     processed by the underlying model. tokens is logically appended
     to the text represented by `existing_prefix`. This method returns a new
     kv_cache (typically) for the resulting text.
     """
 
   @abc.abstractmethod
   def generate(
-      self,
-      params: Params,
-      decode_state: DecodeState
+      self, params: Params, decode_state: DecodeState
   ) -> Tuple[DecodeState, ResultTokens]:
     """Generates tokens for each sequence being decoded in parallel.
 
     Generate takes a batch of pre-computed kv-caches, and computes:
       - the predicted next token for each of the sequences
       - an updated set of kv-caches
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/mock_engine.py` & `google-jetstream-0.2.0/jetstream/engine/mock_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 Params = jax.Array  # [1,].
 Prefix = jax.Array  # [batch,] of strings with different lengths.
 
 
 @struct.dataclass
 class DecodeState:
   """The inputs into a generation step."""
+
   prefill_cache: jax.Array
   generate_cache: jax.Array
   generate_cache_index: int
   generate_lengths: jax.Array
 
 
 class TestEngine(engine_api.Engine):
@@ -64,15 +65,15 @@
 
   def __init__(self, batch_size: int, cache_length: int, weight: float):
     self.prefill_cache_batch = batch_size
     self.generate_cache_batch = batch_size
     self.cache_length = cache_length
     self.weight = weight
     self._mesh = jax.sharding.Mesh(
-        mesh_utils.create_device_mesh((1, 1, 1), jax.devices()), ('x', 'y', 'z')
+        mesh_utils.create_device_mesh((1, 1, 1), jax.devices()), ("x", "y", "z")
     )
 
   def load_params(self) -> Params:
     """Loads model weights."""
     # An integer, used to multiply inputs.
     return jnp.array([self.weight], dtype=jnp.float32)
 
@@ -152,15 +153,16 @@
         (fake_size, fake_size)
     )
     # Do some fake work that isn't eliminated by dead code elimination (DCE).
     generate_cache = generate_cache + fake_work.mean() - fake_work.mean()
     new_lengths = generate_lengths + 1
     speculations = new_timestep.shape[1]
     # Concatenates the tokens, their validity and the lengths of each sequence
-    # into one tensor so that copy operations are faster on Cloud TPU infrastructure.
+    # into one tensor so that copy operations are faster on Cloud TPU
+    # infrastructure.
     token_data = jnp.concatenate(
         [new_timestep, jnp.ones_like(new_timestep), new_lengths[:, None]],
         axis=-1,
     )
     return DecodeState(
         prefill_cache=prefill_cache,
         generate_cache=generate_cache,
@@ -188,16 +190,18 @@
   ) -> DecodeState:
     """Adds `prefix` into `decode_state` at `slot`."""
     # [B, T], [T,] -> [B, T]
     prefill_cache = jax.lax.dynamic_update_slice_in_dim(
         decode_state.prefill_cache, prefix, slot, axis=0
     )
     generate_cache = jax.lax.dynamic_update_slice_in_dim(
-        decode_state.generate_cache, jnp.zeros((1, self.cache_length)),
-        slot, axis=0
+        decode_state.generate_cache,
+        jnp.zeros((1, self.cache_length)),
+        slot,
+        axis=0,
     )
     samples_per_slot = self.generate_cache_batch // self.prefill_cache_batch
     generate_lengths = jax.lax.dynamic_update_slice_in_dim(
         decode_state.generate_lengths,
         jnp.zeros((samples_per_slot), dtype=jnp.int32),
         slot * samples_per_slot,
         axis=0,
@@ -211,15 +215,15 @@
   def get_prefix_destination_sharding(self) -> Any:
     return jax.sharding.NamedSharding(
         mesh=self.mesh, spec=jax.sharding.PartitionSpec()
     )
 
   def get_tokenizer(self) -> tokenizer_pb2.TokenizerParameters:
     """Return a protobuf of tokenizer info, callable from Py or C++."""
-    return tokenizer_pb2.TokenizerParameters(path='test', extra_ids=0)
+    return tokenizer_pb2.TokenizerParameters(path="test", extra_ids=0)
 
   def init_decode_state(self) -> DecodeState:
     """Initialises any state which a generation step transforms."""
     return DecodeState(
         prefill_cache=jnp.zeros(
             (self.prefill_cache_batch, self.cache_length), dtype=jnp.float32
         ),
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/mock_engine_test.py` & `google-jetstream-0.2.0/jetstream/engine/mock_engine_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     params = engine.load_params()
     return engine, params
 
   def _prefill(self):
     """Performs prefill and returns a kv cache."""
     engine, params = self._setup()
     # A 2 will be pre-pended as 'bos' token from the vocab.
-    text = 'AB'
+    text = "AB"
     metadata = engine.get_tokenizer()
     vocab = token_utils.load_vocab(metadata.path, metadata.extra_ids)
     tokens, true_length = token_utils.tokenize_and_pad(text, vocab, is_bos=True)
     prefill_result = engine.prefill(
         params=params, padded_tokens=tokens, true_length=3
     )
     return engine, params, prefill_result, true_length
@@ -89,26 +89,26 @@
     metadata = engine.get_tokenizer()
     tokenizer = token_utils.load_vocab(
         metadata.path, metadata.extra_ids
     ).tokenizer
     # Char for 266
     token_data = sampled_tokens.get_result_at_slot(slot)
     tok = token_data.tokens
-    assert tokenizer.IdToPiece(int(tok.item())) == 'Ċ'
+    assert tokenizer.IdToPiece(int(tok.item())) == "Ċ"
     decode_state, sampled_tokens = engine.generate(
         params=params, decode_state=decode_state
     )
     # Char for 399
     token_data = sampled_tokens.get_result_at_slot(slot)
     tok = token_data.tokens
-    assert tokenizer.IdToPiece(int(tok.item())) == 'Ə'
+    assert tokenizer.IdToPiece(int(tok.item())) == "Ə"
     _, sampled_tokens = engine.generate(
         params=params, decode_state=decode_state
     )
     # Char for 598
     token_data = sampled_tokens.get_result_at_slot(slot)
     tok = token_data.tokens
-    assert tokenizer.IdToPiece(int(tok.item())) == 'ɖ'
+    assert tokenizer.IdToPiece(int(tok.item())) == "ɖ"
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/mock_utils.py` & `google-jetstream-0.2.0/jetstream/engine/mock_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,23 +21,33 @@
 
 
 @struct.dataclass
 class TestTokenizer:
   """Tokenizer used for testing purposes."""
 
   def IdToPiece(self, integer: int) -> str:  # pylint: disable=invalid-name
-    """In the real version, unlike encode_tf/decode_tf, doesn't strip trailing whitespace."""
+    """In the real version, unlike encode_tf/decode_tf, doesn't strip trailing
+
+    whitespace.
+    """
     return chr(integer)
 
+  def decode(self, tokens: np.ndarray):  # pylint: disable=invalid-name
+    """Converts a numpy array into a string.
+
+    Uses tokens[0] as we are doing streaming decode now
+    """
+    return chr(tokens[0])
+
 
 @struct.dataclass
 class TestVocab(Vocabulary):
   """Mock vocabulary used for tests.
 
-  These methods are duplicative on the test vocab, but required to fit 
+  These methods are duplicative on the test vocab, but required to fit
   the seqio.Vocabulary interface.
   """
 
   pad_id = 0
   eos_id = 1
   bos_id = 2
   unk_id = 3
@@ -46,32 +56,32 @@
 
   def _encode(self, s: str) -> Sequence[int]:
     """Converts a string into a integer sequenc."""
     # 'We use array methods, not python iterables so we don't
     # implement this method in the mock vocab.
     raise NotImplementedError
 
-  def _decode(self, tokens: np.ndarray):
+  def _decode(self, ids: np.ndarray):
     """Converts a numpy array into a string."""
     # 'We use array methods, not python iterables so we don't
     # implement this method in the mock vocab.
     raise NotImplementedError
 
-  def _encode_tf(self, text: str) -> np.ndarray:
+  def _encode_tf(self, s: str) -> np.ndarray:
     """Converts a string into a numpy array."""
     # We mock using numpy to avoid propagating tf dependencies.
-    chars = np.array([ord(c) for c in text]).astype(np.int32)
+    chars = np.array([ord(c) for c in s]).astype(np.int32)
     return chars
 
-  def _decode_tf(self, tokens: np.ndarray) -> List[str]:
+  def _decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
     # We mock using numpy to avoid propagating tf dependencies.
-    results = np.split(tokens, tokens.shape[0])
-    return [''.join([chr(r) for r in list(line[0])]) for line in results]
+    results = np.split(ids, ids.shape[0])
+    return ["".join([chr(r) for r in list(line[0])]) for line in results]
 
-  def encode_tf(self, text: str) -> np.ndarray:
+  def encode_tf(self, s: str) -> np.ndarray:
     """Converts a string into a numpy array."""
-    return self._encode_tf(text)
+    return self._encode_tf(s)
 
-  def decode_tf(self, tokens: np.ndarray) -> List[str]:
+  def decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
-    return self._decode_tf(tokens)
+    return self._decode_tf(ids)
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/token_utils.py` & `google-jetstream-0.2.0/jetstream/engine/token_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,29 @@
 from seqio.vocabularies import SentencePieceVocabulary
 from seqio.vocabularies import Vocabulary
 
 from jetstream.engine import engine_api
 from jetstream.engine import mock_utils
 
 
+def mix_decode(vocab: Vocabulary, tok_id: int):
+  """
+  The IdToPiece and decode results differ for 344 tokens in Llama2.
+  Use the decode function to generate the correct strings for these 344 tokens.
+  If IdToPiece returns a hex string (e.g., '<0x0A>') for a token within these
+    344, utilize IdToPiece to convert it into a string, likely with a space
+    placeholder (' ') for the corresponding tokens.
+  """
+  p_token = vocab.tokenizer.IdToPiece(tok_id)
+  # SentencePiece escapes the whitespace with a meta symbol "▁" (U+2581)
+  p_token = p_token.replace("▁", " ")
+  d_token = vocab.tokenizer.decode([tok_id])
+  return p_token if p_token.lstrip() == d_token else d_token
+
+
 def take_nearest_length(lengths: list[int], length: int) -> int:
   """Gets the nearest length to the right in a set of lengths."""
   pos = bisect_left(lengths, length)
   if pos == len(lengths):
     return lengths[-1]
   return lengths[pos]
 
@@ -79,27 +94,29 @@
         max_prefill_length,
     ]
   tokens = np.array(vocab.encode_tf(s))  # [Length]
   # Add a beginning of sequence token if this is the beginning.
   if is_bos:
     tokens = np.concatenate(
         [
-            np.array([
-                vocab.bos_id,
-            ]),
+            np.array(
+                [
+                    vocab.bos_id,
+                ]
+            ),
             tokens,
         ],
         axis=-1,
     )
   true_length = tokens.shape[-1]
   padded_length = take_nearest_length(prefill_lengths, true_length)
   padding = padded_length - true_length
-  assert vocab.pad_id == 0, 'Further logic required if pad_id not 0.'
+  assert vocab.pad_id == 0, "Further logic required if pad_id not 0."
   if padding < 0:
-    logging.warning('Provided sequence longer than available.')
+    logging.warning("Provided sequence longer than available.")
     # Take the last N tokens if we have too many.
     padded_tokens = tokens[-padded_length:]
   else:
     padded_tokens = np.pad(tokens, (0, padding))
   return jnp.array(padded_tokens), true_length
 
 
@@ -107,15 +124,16 @@
     slot: int,
     slot_max_length: int,
     result_tokens: engine_api.ResultTokens,
     vocab: Vocabulary,
     complete: np.ndarray,
     debug: bool = False,
 ) -> Tuple[List[str], np.ndarray]:
-  """Processes a result tokens into a list of strings, handling multiple samples.
+  """Processes a result tokens into a list of strings, handling multiple
+    samples.
 
   Args:
     slot: The slot at which to draw tokens from.
     slot_max_length: Max length for a sample in the slot.
     result_tokens: The tokens to access by slot.
     vocab: For the detokenizer.
     complete: Array representing the completion status of each sample in the
@@ -133,65 +151,63 @@
   slot_lengths = slot_data.lengths
   samples, speculations = slot_tokens.shape
   stop_tokens = [vocab.eos_id, vocab.pad_id]
   # Stop anything which has reached it's max length.
   complete = complete | (slot_lengths > slot_max_length)
   if debug:
     logging.info(
-        'Complete %s, slot_tokens: %s, slot_lengths: %s',
-        complete.__str__(),
-        slot_tokens.__str__(),
-        slot_lengths.__str__(),
+        "Complete %s, slot_tokens: %s, slot_lengths: %s",
+        str(complete),
+        str(slot_tokens),
+        str(slot_lengths),
     )
   sample_return = []
   for idx in range(samples):
-    string_so_far = ''
+    string_so_far = ""
     if not complete[idx].item():
       for spec_idx in range(speculations):
         tok_id = slot_tokens[idx, spec_idx].item()
         valid = slot_valid[idx, spec_idx].item()
         if debug:
           logging.info(
-              'Sample idx: %d Speculation idx: %d Token: %d',
+              "Sample idx: %d Speculation idx: %d Token: %d",
               idx,
               spec_idx,
               tok_id,
           )
         if tok_id in stop_tokens or not valid:
           complete[idx] = True
           break
         else:
           try:
-            token = vocab.tokenizer.IdToPiece(tok_id)  # pytype: disable=attribute-error
-            # ▁ or _ encodes a blank space.
-            token = token.replace('▁', ' ').replace('_', ' ')
+            token = mix_decode(vocab, tok_id)  # pytype: disable=attribute-error
           except ValueError:
             # This error only occurs when using tests where the vocab range is
             # computed via addition and int->char is computed using chr(). Real
             # models have vocab logits which are at max the size of the vocab.
-            logging.warning('%d exceeded vocab range', tok_id)
-            token = '<sampled_outside_vocab>'
+            logging.warning("%d exceeded vocab range", tok_id)
+            token = "<sampled_outside_vocab>"
           string_so_far += token
     sample_return.append(string_so_far)
     if debug:
-      logging.info('Sampled return %s', sample_return.__str__())
+      logging.info("Sampled return %s", str(sample_return))
   return sample_return, complete
 
 
 def load_vocab(path: str, extra_ids: int = 0) -> Vocabulary:
   """Eagerly loads a vocabulary.
 
   Args:
     path: Vocabulary file path.
     extra_ids: Number of extra IDs.
 
   Returns:
     A seqio Vocabulary.
   """
-  if path == 'test':
+  if path == "test":
     return mock_utils.TestVocab()
   else:
     vocab = SentencePieceVocabulary(
         path,
         extra_ids=extra_ids,
     )
     # SentencePieceVocabulary uses lazy loading. Request access to a property,
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/tokenizer_pb2.py` & `google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: jetstream/engine/tokenizer.proto
 # Protobuf Python Version: 4.25.1
+# pylint: disable=all
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n jetstream/engine/tokenizer.proto\x12\x06\x65ngine\"6\n\x13TokenizerParameters\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\textra_ids\x18\x02 \x01(\x05\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n jetstream/engine/tokenizer.proto\x12\x06\x65ngine"6\n\x13TokenizerParameters\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\textra_ids\x18\x02 \x01(\x05\x42\x02P\x01\x62\x06proto3'
+)
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'jetstream.engine.tokenizer_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(
+    DESCRIPTOR, "jetstream.engine.tokenizer_pb2", _globals
+)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_TOKENIZERPARAMETERS']._serialized_start=44
-  _globals['_TOKENIZERPARAMETERS']._serialized_end=98
+  _globals["DESCRIPTOR"]._options = None
+  _globals["DESCRIPTOR"]._serialized_options = b"P\001"
+  _globals["_TOKENIZERPARAMETERS"]._serialized_start = 44
+  _globals["_TOKENIZERPARAMETERS"]._serialized_end = 98
 # @@protoc_insertion_point(module_scope)
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/tokenizer_pb2_grpc.py` & `google-jetstream-0.2.0/jetstream/engine/tokenizer_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+# pylint: disable=all
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-
```

### Comparing `google-jetstream-0.1.1/jetstream/engine/utils_test.py` & `google-jetstream-0.2.0/jetstream/engine/utils_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 from absl.testing import absltest
 
 
 class UtilsTest(absltest.TestCase):
 
   def test_speculations_with_multi_sample_slots(self, samples_per_slot=2):
     # [4, 1]
-    mock_tokens = np.array([
-        [0, ord('A')],
-        [ord('A'), ord('D')],
-        [ord('T'), ord('3')],
-        [ord('A'), 1],
-    ]).astype(np.int32)
+    mock_tokens = np.array(
+        [
+            [0, ord("A")],
+            [ord("A"), ord("D")],
+            [ord("T"), ord("3")],
+            [ord("A"), 1],
+        ]
+    ).astype(np.int32)
     mock_valid_tokens = np.ones_like(mock_tokens, dtype=np.int32)
-    mock_lengths = np.ones(mock_tokens.shape[0], dtype=np.int32)*2
+    mock_lengths = np.ones(mock_tokens.shape[0], dtype=np.int32) * 2
     # completion is 'per slot' because we track it for a given request.
     mock_complete = np.zeros(
         (mock_tokens.shape[0] // samples_per_slot), dtype=np.int32
     )
     data = np.concatenate(
         [
             mock_tokens,
@@ -59,25 +61,25 @@
         result_tokens=result_tokens,
         vocab=mock_utils.TestVocab(),
         complete=mock_complete,
     )
     np.testing.assert_equal(complete, np.array([1, 0]))
 
     assert not per_channel[0]  # i.e. == '', because of the pad.
-    assert per_channel[1] == 'AD'
+    assert per_channel[1] == "AD"
     mock_complete = np.zeros(
         (mock_tokens.shape[0] // samples_per_slot), dtype=np.int32
     )
     per_channel, complete = token_utils.process_result_tokens(
         slot=1,
         slot_max_length=4,
         result_tokens=result_tokens,
         vocab=mock_utils.TestVocab(),
         complete=mock_complete,
     )
-    assert per_channel[0] == 'T3'
-    assert per_channel[1] == 'A'  # second token is padded.
+    assert per_channel[0] == "T3"
+    assert per_channel[1] == "A"  # second token is padded.
     np.testing.assert_equal(complete, np.array([0, 1]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
   absltest.main()
```

### Comparing `google-jetstream-0.1.1/setup.py` & `google-jetstream-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,31 +15,29 @@
 from setuptools import find_packages, setup
 
 
 def parse_requirements(filename):
   """load requirements from a pip requirements file."""
   with open(filename) as f:
     lineiter = (line.strip() for line in f)
-    return [line for line in lineiter if line and not line.startswith('#')]
+    return [line for line in lineiter if line and not line.startswith("#")]
 
 
 setup(
-    name='google-jetstream',
-    version='0.1.1',
+    name="google-jetstream",
+    version="0.2.0",
     description=(
-        'A throughput and memory optimized engine for LLM inference on TPU and'
-        ' GPU.'
+        "JetStream is a throughput and memory optimized engine for LLM inference on XLA devices, starting with TPUs (and GPUs in future -- PRs welcome)."
     ),
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    author='Google LLC',
-    url='https://github.com/google/JetStream',
-    packages=find_packages(exclude='benchmarks'),
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    author="Google LLC",
+    url="https://github.com/google/JetStream",
+    packages=find_packages(exclude="benchmarks"),
     classifiers=[
-        'Programming Language :: Python :: 3.10',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
     ],
-    python_requires='>=3.10',
-    install_requires=parse_requirements('requirements.in'),
+    python_requires=">=3.10",
+    install_requires=parse_requirements("requirements.in"),
 )
-
```

