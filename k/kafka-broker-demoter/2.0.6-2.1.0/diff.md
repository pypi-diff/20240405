# Comparing `tmp/kafka_broker_demoter-2.0.6.tar.gz` & `tmp/kafka_broker_demoter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_broker_demoter-2.0.6.tar", last modified: Thu Jan 18 16:17:31 2024, max compression
+gzip compressed data, was "kafka_broker_demoter-2.1.0.tar", last modified: Fri Apr  5 11:26:15 2024, max compression
```

## Comparing `kafka_broker_demoter-2.0.6.tar` & `kafka_broker_demoter-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/kafka_broker_demoter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter/configure_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    32012 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter/demoter.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:17:20.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 16:17:31.000000 kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:17:31.218832 kafka_broker_demoter-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-18 16:17:07.000000 kafka_broker_demoter-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:26:15.120780 kafka_broker_demoter-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 11:26:15.120780 kafka_broker_demoter-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:26:15.116780 kafka_broker_demoter-2.1.0/kafka_broker_demoter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter/configure_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32642 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter/demoter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:26:15.120780 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:26:07.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 11:26:15.000000 kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:26:15.116780 kafka_broker_demoter-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:26:15.120780 kafka_broker_demoter-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-05 11:25:56.000000 kafka_broker_demoter-2.1.0/setup.py
```

### Comparing `kafka_broker_demoter-2.0.6/LICENSE` & `kafka_broker_demoter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_broker_demoter-2.0.6/PKG-INFO` & `kafka_broker_demoter-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka_broker_demoter
-Version: 2.0.6
+Version: 2.1.0
 Summary: Tool for safely demote a broker from a kafka cluster
 Author: Sergio Troiano
 Author-email: sergio_troiano@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kafka-python==2.0.2
@@ -63,14 +63,15 @@
 
 The demote rollback action will revert the changes made by the demote action, restoring the original state of the broker.
 
 ## Configuration Options
 
 - `--bootstrap-servers`: The list of Kafka brokers to connect to. Required for both actions.
 - `--kafka-path`: The path to the Kafka installation directory. Default: /opt/kafka.
+- `--concurrent-leader-movements`: The number of concurrent leadership movements beetween brokers.
 - `--kafka-heap-opts`: The heap options to use when starting Kafka. Default: -Xmx512M.
 - `--topic-tracker`: The topic tracker to use. Default: `default`.
 - `--log-file`: The path to the log file. Default: kafka_broker_demoter.log.
 - `--log-level`: The log level. Available options: INFO, DEBUG. Default: INFO.
 
 ## License
```

### Comparing `kafka_broker_demoter-2.0.6/README.md` & `kafka_broker_demoter-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 The demote rollback action will revert the changes made by the demote action, restoring the original state of the broker.
 
 ## Configuration Options
 
 - `--bootstrap-servers`: The list of Kafka brokers to connect to. Required for both actions.
 - `--kafka-path`: The path to the Kafka installation directory. Default: /opt/kafka.
+- `--concurrent-leader-movements`: The number of concurrent leadership movements beetween brokers.
 - `--kafka-heap-opts`: The heap options to use when starting Kafka. Default: -Xmx512M.
 - `--topic-tracker`: The topic tracker to use. Default: `default`.
 - `--log-file`: The path to the log file. Default: kafka_broker_demoter.log.
 - `--log-level`: The log level. Available options: INFO, DEBUG. Default: INFO.
 
 ## License
```

### Comparing `kafka_broker_demoter-2.0.6/kafka_broker_demoter/cli.py` & `kafka_broker_demoter-2.1.0/kafka_broker_demoter/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,21 @@
         required=(
             "demote" in sys.argv
             or "demote_rollback" in sys.argv
             or "update_throttle" in sys.argv
         ),
     )
     parser.add_argument(
+        "--concurrent-leader-movements",
+        type=int,
+        help="The max nº of leader movements that will be carried out at the same time.",
+        default=1,
+        required=False,
+    )
+    parser.add_argument(
         "--kafka-path",
         type=str,
         default="/opt/kafka",
         help="Sets the Kafka installation path",
         required=False,
     )
     parser.add_argument(
@@ -115,17 +122,17 @@
         args.bootstrap_servers,
         args.kafka_path,
         args.kafka_heap_opts,
         args.topic_tracker,
     )
 
     if args.demotion_action == "demote":
-        demoter.demote(args.broker_id, args.throttle_bytes)
+        demoter.demote(args.broker_id, args.throttle_bytes, args.concurrent_leader_movements)
     elif args.demotion_action == "demote_rollback":
-        demoter.demote_rollback(args.broker_id, args.remove_throttle)
+        demoter.demote_rollback(args.broker_id, args.remove_throttle, args.concurrent_leader_movements)
     elif args.demotion_action == "update_throttle":
         # Convert broker_ids to a list of integers
         if args.broker_ids:
             args.broker_ids = [int(broker_id) for broker_id in args.broker_ids]
         demoter.update_throttle(
             args.broker_id, args.update_throttle_bytes, args.broker_ids
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kafka_broker_demoter-2.0.6/kafka_broker_demoter/configure_logging.py` & `kafka_broker_demoter-2.1.0/kafka_broker_demoter/configure_logging.py`

 * *Files identical despite different names*

### Comparing `kafka_broker_demoter-2.0.6/kafka_broker_demoter/demoter.py` & `kafka_broker_demoter-2.1.0/kafka_broker_demoter/demoter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import os
 import random
 import re
 import string
 import subprocess
 import tempfile
+import time
 
 from kafka import KafkaAdminClient, KafkaConsumer, KafkaProducer
 from kafka.admin import NewTopic
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 from kafka_broker_demoter.exceptions import (
     BrokerStatusError,
@@ -36,18 +37,18 @@
         self.bootstrap_servers = bootstrap_servers
         self.kafka_path = kafka_path
         self.kafka_heap_opts = kafka_heap_opts
         self.topic_tracker = topic_tracker
 
         self.admin_client = None
         self.partitions_temp_filepath = None
-        self.admin_config_tmp_file = None
         self.admin_config_content = (
             "default.api.timeout.ms=240000\nrequest.timeout.ms=120000"
         )
+        self.admin_config_tmp_file = self._generate_tmpfile_with_admin_configs()
 
     @property
     def _get_admin_client(self):
         if self.admin_client is None:
             self.admin_client = KafkaAdminClient(
                 bootstrap_servers=self.bootstrap_servers
             )
@@ -260,15 +261,15 @@
                 replication_factor=3,
                 topic_configs={"cleanup.policy": "compact"},
             )
             self._get_admin_client.create_topics(
                 new_topics=[topic], validate_only=False
             )
 
-    def demote(self, broker_id, throttle):
+    def demote(self, broker_id, throttle, num_concurrent_leader_movements):
         """
         Demotes a broker by reassigning the partition leaders from the specified broker to other brokers.
         If an ongoing or unfinished demote operation is found for the broker, a BrokerStatusError is raised.
         If a RecordNotFoundError occurs while checking for ongoing demote operations, the broker is considered ready for demotion.
 
         Args:
             broker_id (int): The ID of the broker to be demoted.
@@ -305,15 +306,16 @@
             )
             logger.info(
                 "Moving leaderships away from broker: {}, it may take a while...".format(
                     broker_id
                 )
             )
             self._change_replica_assignment(demoted_partitions_state)
-            self._trigger_leader_election(demoted_partitions_state)
+            self._trigger_leader_election(demoted_partitions_state, num_concurrent_leader_movements)
+
             self._save_rollback_plan(broker_id, current_partitions_state)
             if throttle > 0:
                 self._set_throttles(broker_id, throttle)
 
         logger.info("Broker {} was successfully demoted".format(broker_id))
 
     def _unset_throttles(self, broker_id):
@@ -687,15 +689,15 @@
             if broker_id_match and throttled_rate_match:
                 broker_id = int(broker_id_match.group(1))
                 throttled_rate = int(throttled_rate_match.group(1))
                 broker_configs[broker_id] = throttled_rate
 
         print(json.dumps(broker_configs))
 
-    def demote_rollback(self, broker_id, remove_throttle):
+    def demote_rollback(self, broker_id, remove_throttle, num_concurrent_leader_movements):
         """
         Perform a rollback for the previous demote operation on a specific broker.
 
         Args:
             broker_id: The ID of the broker to rollback the demotion for.
 
         Raises:
@@ -713,15 +715,15 @@
             )
         logger.info(
             "Executing demote rollback operation for broker: {}, it may take a while...".format(
                 broker_id
             )
         )
         self._change_replica_assignment(previous_partitions_state)
-        self._trigger_leader_election(previous_partitions_state)
+        self._trigger_leader_election(previous_partitions_state, num_concurrent_leader_movements)
         self._produce_record(broker_id, None)
         if remove_throttle:
             self._unset_throttles(broker_id)
         logger.info(
             "Rollback plan for broker {} was successfully executed".format(broker_id)
         )
 
@@ -735,30 +737,28 @@
         Returns:
             str: The filepath of the generated temporary file.
 
         Raises:
             None.
 
         Notes:
-            - If `self.partitions_temp_filepath` is already set, a new temporary file will not be generated.
             - The generated filepath will have a random filename consisting of lowercase letters and digits.
             - The generated filepath will have the '.json' extension.
 
         """
-        if self.partitions_temp_filepath is None:
-            filename = "".join(
-                random.choices(string.ascii_lowercase + string.digits, k=10)
-            )
-            self.partitions_temp_filepath = tempfile.mktemp(
-                suffix=".json", prefix=filename
-            )
-
-        with open(self.partitions_temp_filepath, "w") as temp_file:
+        filename = "".join(
+            random.choices(string.ascii_lowercase + string.digits, k=10)
+        )
+        partitions_temp_filepath = tempfile.mktemp(
+            suffix=".json", prefix=filename
+        )
+        self.partitions_temp_filepath = partitions_temp_filepath
+        with open(partitions_temp_filepath, "w") as temp_file:
             json.dump(data, temp_file)
-            return self.partitions_temp_filepath
+            return partitions_temp_filepath
 
     def _change_replica_assignment(self, demoting_plan):
         """
         Change the replica assignment of partitions based on the provided demoting plan.
 
         Args:
             demoting_plan (dict): A dictionary containing the demoting plan.
@@ -779,54 +779,61 @@
         env_vars = os.environ.copy()
         env_vars["KAFKA_HEAP_OPTS"] = self.kafka_heap_opts
         self._execute_subprocess(command, env_vars)
 
     def _generate_tmpfile_with_admin_configs(self):
         """
         Generate a temporary file containing the admin configurations.
-
-        If the temporary file doesn't already exist, it will be created. The admin configurations
-        are written to the file, and the file is closed before returning its name.
+        The admin configurations are written to the file, and the file
+        is closed before returning its name.
 
         Returns:
             str: The path/name of the temporary file.
 
         """
-        if self.admin_config_tmp_file is None:
-            self.admin_config_tmp_file = tempfile.NamedTemporaryFile(delete=False)
+        admin_config_tmp_file = tempfile.NamedTemporaryFile(delete=False)
 
-        self.admin_config_tmp_file.write(self.admin_config_content.encode())
-        self.admin_config_tmp_file.close()
-        return self.admin_config_tmp_file.name
+        admin_config_tmp_file.write(self.admin_config_content.encode())
+        admin_config_tmp_file.close()
+        return admin_config_tmp_file.name
 
-    def _trigger_leader_election(self, demoting_plan):
+    def _trigger_leader_election(self, demoting_plan, concurrent_leader_movements):
         """
         Trigger a leader election using the demoting plan.
 
         This method runs the `kafka-leader-election.sh` script with the provided demoting plan.
         The command is executed using the provided Kafka installation's path, the generated admin
         configurations, the bootstrap servers, and the path to the temporary file containing
-        the demoting plan in JSON format.
+        the demoting plan in JSON format. The number of leadership movements is limited to concurrent_leader_movements
+        to avoid stressing the brokers.
 
         Args:
             demoting_plan (dict or list): A dictionary or list representation of the demoting plan.
-
+            concurrent_leader_movements (int): Nº of concurrent leader movements between brokers.
         Raises:
             TriggerLeaderElectionError: If the leader election fails.
 
         """
-        demoting_plan_filepath = self._generate_tempfile_with_json_content(
-            demoting_plan
-        )
-        command = "{}/bin/kafka-leader-election.sh --admin.config {} --bootstrap-server {} --election-type PREFERRED --path-to-json-file {}".format(
-            self.kafka_path,
-            self._generate_tmpfile_with_admin_configs(),
-            self.bootstrap_servers,
-            demoting_plan_filepath,
-        )
-        env_vars = os.environ.copy()
-        env_vars["KAFKA_HEAP_OPTS"] = self.kafka_heap_opts
-        self._execute_subprocess(command, env_vars)
+        # Split entry items into groups of N=concurrent_leader_movements
+        grouped_entries = [demoting_plan["partitions"][i:i + concurrent_leader_movements] for i in range(0, len(demoting_plan["partitions"]), concurrent_leader_movements)]
+
+        # Iterate over each group
+        for group in grouped_entries:
+            logger.info("Running kafka-leader-election on partitions: {}".format(group))
+            demoting_plan_filepath = self._generate_tempfile_with_json_content(
+                {"partitions": group}
+            )
+
+            command = "{}/bin/kafka-leader-election.sh --admin.config {} --bootstrap-server {} --election-type PREFERRED --path-to-json-file {}".format(
+                self.kafka_path,
+                self.admin_config_tmp_file,
+                self.bootstrap_servers,
+                demoting_plan_filepath,
+            )
+            env_vars = os.environ.copy()
+            env_vars["KAFKA_HEAP_OPTS"] = self.kafka_heap_opts
+            self._execute_subprocess(command, env_vars)
+            time.sleep(1)
 
     def _save_rollback_plan(self, broker_id, current_partitions_state):
         logger.info("Saving rollback plan for broker {}".format(broker_id))
         self._produce_record(broker_id, current_partitions_state)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/PKG-INFO` & `kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka_broker_demoter
-Version: 2.0.6
+Version: 2.1.0
 Summary: Tool for safely demote a broker from a kafka cluster
 Author: Sergio Troiano
 Author-email: sergio_troiano@hotmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: kafka-python==2.0.2
@@ -63,14 +63,15 @@
 
 The demote rollback action will revert the changes made by the demote action, restoring the original state of the broker.
 
 ## Configuration Options
 
 - `--bootstrap-servers`: The list of Kafka brokers to connect to. Required for both actions.
 - `--kafka-path`: The path to the Kafka installation directory. Default: /opt/kafka.
+- `--concurrent-leader-movements`: The number of concurrent leadership movements beetween brokers.
 - `--kafka-heap-opts`: The heap options to use when starting Kafka. Default: -Xmx512M.
 - `--topic-tracker`: The topic tracker to use. Default: `default`.
 - `--log-file`: The path to the log file. Default: kafka_broker_demoter.log.
 - `--log-level`: The log level. Available options: INFO, DEBUG. Default: INFO.
 
 ## License
```

### Comparing `kafka_broker_demoter-2.0.6/kafka_broker_demoter.egg-info/SOURCES.txt` & `kafka_broker_demoter-2.1.0/kafka_broker_demoter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafka_broker_demoter-2.0.6/setup.py` & `kafka_broker_demoter-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import Extension, find_packages, setup
 from setuptools.command.test import test as TestCommand
 
 __location__ = os.path.join(
     os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe()))
 )
 
-version = "2.0.6"
+version = "2.1.0"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 def get_install_requirements(path):
     content = open(os.path.join(__location__, path)).read()
```

