# Comparing `tmp/tahutils-0.1.6.tar.gz` & `tmp/tahutils-0.1.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahutils-0.1.6.tar", max compression
+gzip compressed data, was "tahutils-0.1.7a1.tar", max compression
```

## Comparing `tahutils-0.1.6.tar` & `tahutils-0.1.7a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    14198 2024-04-04 21:19:25.127819 tahutils-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     1560 2024-04-04 21:19:25.127819 tahutils-0.1.6/README.md
--rw-r--r--   0        0        0      744 2024-04-04 21:19:25.127819 tahutils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      242 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/__init__.py
--rw-r--r--   0        0        0     2447 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/parse.py
--rw-r--r--   0        0        0     7782 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/spb.py
--rw-r--r--   0        0        0       84 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/__init__.py
--rw-r--r--   0        0        0     6178 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/array_packer.py
--rw-r--r--   0        0        0     3008 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/host_session_establishment.py
--rw-r--r--   0        0        0      140 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/readme.md
--rw-r--r--   0        0        0    15690 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/sparkplug_b.py
--rw-r--r--   0        0        0     8621 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu/sparkplug_b_pb2.py
--rw-r--r--   0        0        0        5 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/tahu_version.txt
--rw-r--r--   0        0        0      224 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/types.py
--rw-r--r--   0        0        0     1436 2024-04-04 21:19:25.127819 tahutils-0.1.6/tahutils/utils.py
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 tahutils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    14198 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/LICENSE.txt
+-rw-r--r--   0        0        0     1560 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/README.md
+-rw-r--r--   0        0        0      747 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/pyproject.toml
+-rw-r--r--   0        0        0      245 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/parse.py
+-rw-r--r--   0        0        0     8071 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/spb.py
+-rw-r--r--   0        0        0       84 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/array_packer.py
+-rw-r--r--   0        0        0     3008 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/host_session_establishment.py
+-rw-r--r--   0        0        0      140 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/readme.md
+-rw-r--r--   0        0        0    15690 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/sparkplug_b.py
+-rw-r--r--   0        0        0     8621 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/sparkplug_b_pb2.py
+-rw-r--r--   0        0        0        5 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu_version.txt
+-rw-r--r--   0        0        0      224 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/types.py
+-rw-r--r--   0        0        0     1436 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/utils.py
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 tahutils-0.1.7a1/PKG-INFO
```

### Comparing `tahutils-0.1.6/LICENSE.txt` & `tahutils-0.1.7a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/README.md` & `tahutils-0.1.7a1/README.md`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/pyproject.toml` & `tahutils-0.1.7a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahutils"
-version = "0.1.6"
+version = "0.1.7-a1"
 description = "Python utilities for Tahu & Sparkplug B."
 authors = ["Justin Dula <justin.dula@intellicintegration.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Operating System :: OS Independent",
```

### Comparing `tahutils-0.1.6/tahutils/parse.py` & `tahutils-0.1.7a1/tahutils/parse.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/tahutils/spb.py` & `tahutils-0.1.7a1/tahutils/spb.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,22 @@
 	
 	def getNodeDeathPayload(self):
 		"""Returns a death payload for the node. This must be requested and sent as part of the connection."""
 		self.node_death_requested = True
 		self._last_death = self._serialize(spb.getNodeDeathPayload())
 		return self._last_death
 	
-	def getNodeBirthPayload(self, state: MetricValues, times: MetricTimes = dict(), ignore_missing_node_death: bool = False):
+	def getNodeBirthPayload(self, state: MetricValues, times: MetricTimes = dict(), rebirth: bool = False, ignore_missing_node_death: bool = False):
 		"""Returns a birth payload for the given state. State must be set for all metrics. Times can be set for specific metrics, if desired."""
 		state = self._preprocess_dict(state)
 		times = self._preprocess_dict(times, is_time=True)
 		
 		if not ignore_missing_node_death and not self.node_death_requested:
 			raise ValueError("Must request death before requesting new birth")
-		if set(COMMAND_METRICS_SET | state.keys()) != set(self.all_metrics):
+		if not rebirth and set(COMMAND_METRICS_SET | state.keys()) != set(self.all_metrics):
 			raise ValueError("Node birth metrics must be the same as the model's metrics")
 
 		payload = spb.getNodeBirthPayload()
 
 		for metric in COMMAND_METRICS_SET:
 			if metric not in state:
 				state[metric] = False
@@ -116,14 +116,21 @@
 			self.current_values[metric] = value
 
 			if metric in times:
 				spb.addMetric(payload, metric, self._metric_to_alias[metric], mt, value, metric[times])
 			else:
 				spb.addMetric(payload, metric, self._metric_to_alias[metric], mt, value)
 
+		if rebirth:
+			for metric in set(self.current_values.keys()).difference(state.keys()):
+				value = self.current_values[metric]
+				mt = self.metric_types[metric]
+
+				spb.addMetric(payload, metric, self._metric_to_alias[metric], mt, value)
+
 		return self._serialize(payload)
 	
 	def getDataPayload(self, state: MetricValues, times: MetricTimes = dict()):
 		"""Returns a data payload for the given state. Times can be set for specific metrics, if desired."""
 		state = self._preprocess_dict(state)
 		times = self._preprocess_dict(times, is_time=True)
```

### Comparing `tahutils-0.1.6/tahutils/tahu/array_packer.py` & `tahutils-0.1.7a1/tahutils/tahu/array_packer.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/tahutils/tahu/host_session_establishment.py` & `tahutils-0.1.7a1/tahutils/tahu/host_session_establishment.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/tahutils/tahu/sparkplug_b.py` & `tahutils-0.1.7a1/tahutils/tahu/sparkplug_b.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/tahutils/tahu/sparkplug_b_pb2.py` & `tahutils-0.1.7a1/tahutils/tahu/sparkplug_b_pb2.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/tahutils/utils.py` & `tahutils-0.1.7a1/tahutils/utils.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.6/PKG-INFO` & `tahutils-0.1.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahutils
-Version: 0.1.6
+Version: 0.1.7a1
 Summary: Python utilities for Tahu & Sparkplug B.
 Author: Justin Dula
 Author-email: justin.dula@intellicintegration.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

