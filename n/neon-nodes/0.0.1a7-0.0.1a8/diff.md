# Comparing `tmp/neon-nodes-0.0.1a7.tar.gz` & `tmp/neon-nodes-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-nodes-0.0.1a7.tar", last modified: Wed Feb 28 23:05:10 2024, max compression
+gzip compressed data, was "neon-nodes-0.0.1a8.tar", last modified: Fri Apr  5 01:46:59 2024, max compression
```

## Comparing `neon-nodes-0.0.1a7.tar` & `neon-nodes-0.0.1a8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:05:10.929127 neon-nodes-0.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-28 23:05:10.929127 neon-nodes-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:05:10.925127 neon-nodes-0.0.1a7/neon_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/neon_nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:05:10.929127 neon-nodes-0.0.1a7/neon_nodes/res/
--rw-r--r--   0 runner    (1001) docker     (127)   189942 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/neon_nodes/res/error.wav
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/neon_nodes/res/start_listening.wav
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/neon_nodes/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/neon_nodes/voice_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:05:10.929127 neon-nodes-0.0.1a7/neon_nodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 23:05:10.000000 neon-nodes-0.0.1a7/neon_nodes.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 23:05:10.929127 neon-nodes-0.0.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-02-28 23:05:07.000000 neon-nodes-0.0.1a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes/res/
+-rw-r--r--   0 runner    (1001) docker     (127)   189942 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/res/error.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/res/start_listening.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/neon_nodes/voice_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/neon_nodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 01:46:59.000000 neon-nodes-0.0.1a8/neon_nodes.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 01:46:59.952230 neon-nodes-0.0.1a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-05 01:46:54.000000 neon-nodes-0.0.1a8/setup.py
```

### Comparing `neon-nodes-0.0.1a7/LICENSE.md` & `neon-nodes-0.0.1a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a7/PKG-INFO` & `neon-nodes-0.0.1a8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-nodes
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Neon node clients for Hana
 Home-page: https://github.com/NeonGeckoCom/neon-nodes
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-nodes-0.0.1a7/neon_nodes/__init__.py` & `neon-nodes-0.0.1a8/neon_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a7/neon_nodes/res/error.wav` & `neon-nodes-0.0.1a8/neon_nodes/res/error.wav`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a7/neon_nodes/res/start_listening.wav` & `neon-nodes-0.0.1a8/neon_nodes/res/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a7/neon_nodes/version.py` & `neon-nodes-0.0.1a8/neon_nodes/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.1a7"
+__version__ = "0.0.1a8"
```

### Comparing `neon-nodes-0.0.1a7/neon_nodes/voice_client.py` & `neon-nodes-0.0.1a8/neon_nodes/voice_client.py`

 * *Files identical despite different names*

### Comparing `neon-nodes-0.0.1a7/neon_nodes.egg-info/PKG-INFO` & `neon-nodes-0.0.1a8/neon_nodes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-nodes
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Neon node clients for Hana
 Home-page: https://github.com/NeonGeckoCom/neon-nodes
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-nodes-0.0.1a7/setup.py` & `neon-nodes-0.0.1a8/setup.py`

 * *Files identical despite different names*

