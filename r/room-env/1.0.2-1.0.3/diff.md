# Comparing `tmp/room_env-1.0.2.tar.gz` & `tmp/room_env-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "room_env-1.0.2.tar", last modified: Wed Mar 15 13:01:05 2023, max compression
+gzip compressed data, was "room_env-1.0.3.tar", last modified: Fri Apr  5 15:08:21 2024, max compression
```

## Comparing `room_env-1.0.2.tar` & `room_env-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,50 @@
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.053951 room_env-1.0.2/
--rw-rw-r--   0 tk        (1000) tk        (1000)     1068 2022-08-16 11:57:17.000000 room_env-1.0.2/LICENSE
--rw-rw-r--   0 tk        (1000) tk        (1000)     6472 2023-03-15 13:01:05.053951 room_env-1.0.2/PKG-INFO
--rw-rw-r--   0 tk        (1000) tk        (1000)     5993 2023-03-15 12:53:21.000000 room_env-1.0.2/README.md
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.049951 room_env-1.0.2/room_env/
--rw-rw-r--   0 tk        (1000) tk        (1000)      201 2023-03-15 12:53:21.000000 room_env-1.0.2/room_env/__init__.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.053951 room_env-1.0.2/room_env/data/
--rw-rw-r--   0 tk        (1000) tk        (1000)   429221 2022-08-16 11:57:17.000000 room_env-1.0.2/room_env/data/conceptnet-data.json
--rw-rw-r--   0 tk        (1000) tk        (1000)    47857 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/des-config-l-v1.json
--rw-rw-r--   0 tk        (1000) tk        (1000)    17989 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/des-config-m-v1.json
--rw-rw-r--   0 tk        (1000) tk        (1000)    10403 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/des-config-s-v1.json
--rw-rw-r--   0 tk        (1000) tk        (1000)     4789 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/des-config-xs-v1.json
--rw-rw-r--   0 tk        (1000) tk        (1000)     1545 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/des-config-xxs-v1.json
--rw-rw-r--   0 tk        (1000) tk        (1000)       19 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/human-locations
--rw-rw-r--   0 tk        (1000) tk        (1000)     1585 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/human-names
--rw-rw-r--   0 tk        (1000) tk        (1000)      620 2022-08-16 11:57:17.000000 room_env-1.0.2/room_env/data/ms-coco-80-categories
--rw-rw-r--   0 tk        (1000) tk        (1000)     1447 2022-08-16 11:57:17.000000 room_env-1.0.2/room_env/data/semantic-knowledge-small.json
--rw-rw-r--   0 tk        (1000) tk        (1000)     9801 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/semantic-knowledge.json
--rw-rw-r--   0 tk        (1000) tk        (1000)      142 2022-08-16 11:57:17.000000 room_env-1.0.2/room_env/data/top-human-names
--rw-rw-r--   0 tk        (1000) tk        (1000)       69 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/data/top-human-names-small
--rw-rw-r--   0 tk        (1000) tk        (1000)     7555 2022-11-30 15:21:44.000000 room_env-1.0.2/room_env/des.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.053951 room_env-1.0.2/room_env/envs/
--rw-rw-r--   0 tk        (1000) tk        (1000)       82 2023-03-15 12:28:38.000000 room_env-1.0.2/room_env/envs/__init__.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    17029 2023-03-15 12:53:21.000000 room_env-1.0.2/room_env/envs/room0.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    18228 2023-03-15 12:53:21.000000 room_env-1.0.2/room_env/envs/room1.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    32152 2022-09-28 09:49:14.000000 room_env-1.0.2/room_env/memory.py
--rw-rw-r--   0 tk        (1000) tk        (1000)     4386 2022-11-30 15:22:56.000000 room_env-1.0.2/room_env/policy.py
--rw-rw-r--   0 tk        (1000) tk        (1000)    18311 2023-03-15 12:53:21.000000 room_env-1.0.2/room_env/utils.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.049951 room_env-1.0.2/room_env.egg-info/
--rw-rw-r--   0 tk        (1000) tk        (1000)     6472 2023-03-15 13:01:05.000000 room_env-1.0.2/room_env.egg-info/PKG-INFO
--rw-rw-r--   0 tk        (1000) tk        (1000)      939 2023-03-15 13:01:05.000000 room_env-1.0.2/room_env.egg-info/SOURCES.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)        1 2023-03-15 13:01:05.000000 room_env-1.0.2/room_env.egg-info/dependency_links.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)       49 2023-03-15 13:01:05.000000 room_env-1.0.2/room_env.egg-info/requires.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)        9 2023-03-15 13:01:05.000000 room_env-1.0.2/room_env.egg-info/top_level.txt
--rw-rw-r--   0 tk        (1000) tk        (1000)      653 2023-03-15 13:01:05.053951 room_env-1.0.2/setup.cfg
--rw-rw-r--   0 tk        (1000) tk        (1000)       69 2023-03-15 10:46:48.000000 room_env-1.0.2/setup.py
-drwxrwxr-x   0 tk        (1000) tk        (1000)        0 2023-03-15 13:01:05.053951 room_env-1.0.2/test/
--rw-rw-r--   0 tk        (1000) tk        (1000)      239 2022-09-28 09:49:14.000000 room_env-1.0.2/test/test_des.py
--rw-rw-r--   0 tk        (1000) tk        (1000)      361 2022-09-28 09:49:14.000000 room_env-1.0.2/test/test_memory.py
--rw-rw-r--   0 tk        (1000) tk        (1000)     1193 2022-09-28 09:49:14.000000 room_env-1.0.2/test/test_policy.py
--rw-rw-r--   0 tk        (1000) tk        (1000)      434 2023-03-15 12:53:21.000000 room_env-1.0.2/test/test_room_env_v0.py
--rw-rw-r--   0 tk        (1000) tk        (1000)     6357 2023-03-15 12:53:21.000000 room_env-1.0.2/test/test_room_env_v1.py
--rw-rw-r--   0 tk        (1000) tk        (1000)      589 2022-09-28 09:49:14.000000 room_env-1.0.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 15:08:11.000000 room_env-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-05 15:08:21.236081 room_env-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-05 15:08:11.000000 room_env-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.224081 room_env-1.0.3/room_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/create_room2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/room_env/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   429221 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/conceptnet-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47857 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-l-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-m-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-s-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-xs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/des-config-xxs-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/human-locations
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/human-names
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/ms-coco-80-categories
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/names-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   108782 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-dev-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3908646 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-foo-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30841 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-l-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    57836 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-l2-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-m-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-s-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110453 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3912948 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xxl-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/room-config-xxs-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/semantic-knowledge-small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/semantic-knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/top-human-names
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/data/top-human-names-small
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/room_env/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35816 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/envs/room2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-05 15:08:11.000000 room_env-1.0.3/room_env/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.224081 room_env-1.0.3/room_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:08:21.000000 room_env-1.0.3/room_env.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-05 15:08:21.240081 room_env-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 15:08:11.000000 room_env-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:08:21.236081 room_env-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 15:08:11.000000 room_env-1.0.3/test/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 15:08:11.000000 room_env-1.0.3/test/test_utils.py
```

### Comparing `room_env-1.0.2/LICENSE` & `room_env-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `room_env-1.0.2/room_env/data/conceptnet-data.json` & `room_env-1.0.3/room_env/data/conceptnet-data.json`

 * *Files identical despite different names*

### Comparing `room_env-1.0.2/room_env/data/des-config-l-v1.json` & `room_env-1.0.3/room_env/data/des-config-l-v1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'components'": "{replace: OrderedDict([('barbara', [['donut', 'lap'], ['donut', 'lap'], "*

 * *                 "['donut', 'lap'], ['donut', 'lap']]), ('jennifer', [['keyboard', 'kennel'], "*

 * *                 "['keyboard', 'kennel'], ['sandwich', 'lunchbox'], ['sandwich', 'lunchbox'], "*

 * *                 "['sandwich', 'kitchen'], ['sandwich', 'lunchbox'], ['sandwich', 'lunchbox'], "*

 * *                 "['sandwich', 'lunchbox'], ['sandwich', 'kitchen']]), ('lauren', [['bird', "*

 * *                 "'tree'], ['bird', ' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "complexity": 73728,
     "components": {
-        "Alexander": [
+        "alexander": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "house"
@@ -59,15 +59,15 @@
                 "nursery"
             ],
             [
                 "train",
                 "nursery"
             ]
         ],
-        "Amanda": [
+        "amanda": [
             [
                 "bicycle",
                 "countryside"
             ],
             [
                 "bicycle",
                 "countryside"
@@ -97,15 +97,15 @@
                 "farm"
             ],
             [
                 "sheep",
                 "garage"
             ]
         ],
-        "Ann": [
+        "ann": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -147,21 +147,21 @@
                 "water"
             ],
             [
                 "boat",
                 "bathroom"
             ]
         ],
-        "Anthony": [
+        "anthony": [
             [
                 "sheep",
                 "farm"
             ]
         ],
-        "Arthur": [
+        "arthur": [
             [
                 "donut",
                 "bakery"
             ],
             [
                 "donut",
                 "bakery"
@@ -175,15 +175,15 @@
                 "bakery"
             ],
             [
                 "donut",
                 "bakery"
             ]
         ],
-        "Barbara": [
+        "barbara": [
             [
                 "donut",
                 "lap"
             ],
             [
                 "donut",
                 "lap"
@@ -193,15 +193,15 @@
                 "lap"
             ],
             [
                 "donut",
                 "lap"
             ]
         ],
-        "Beverly": [
+        "beverly": [
             [
                 "train",
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
@@ -211,15 +211,15 @@
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
             ]
         ],
-        "Billy": [
+        "billy": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "tree"
@@ -261,15 +261,15 @@
                 "water"
             ],
             [
                 "boat",
                 "farm"
             ]
         ],
-        "Brenda": [
+        "brenda": [
             [
                 "bicycle",
                 "garage"
             ],
             [
                 "bicycle",
                 "garage"
@@ -319,15 +319,15 @@
                 "farm"
             ],
             [
                 "bowl",
                 "nursery"
             ]
         ],
-        "Brittany": [
+        "brittany": [
             [
                 "kite",
                 "office"
             ],
             [
                 "kite",
                 "air"
@@ -361,15 +361,15 @@
                 "cupboard"
             ],
             [
                 "keyboard",
                 "cupboard"
             ]
         ],
-        "Carl": [
+        "carl": [
             [
                 "airplane",
                 "circus"
             ],
             [
                 "airplane",
                 "lap"
@@ -403,15 +403,15 @@
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
             ]
         ],
-        "Carol": [
+        "carol": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "tree"
@@ -433,25 +433,25 @@
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
             ]
         ],
-        "Catherine": [
+        "catherine": [
             [
                 "bicycle",
                 "home"
             ],
             [
                 "bicycle",
                 "garage"
             ]
         ],
-        "Christina": [
+        "christina": [
             [
                 "oven",
                 "bathroom"
             ],
             [
                 "oven",
                 "air"
@@ -509,15 +509,15 @@
                 "zoo"
             ],
             [
                 "bicycle",
                 "garage"
             ]
         ],
-        "Christopher": [
+        "christopher": [
             [
                 "sheep",
                 "movie"
             ],
             [
                 "sheep",
                 "farm"
@@ -539,15 +539,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "David": [
+        "david": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "tree"
@@ -581,21 +581,21 @@
                 "water"
             ],
             [
                 "boat",
                 "water"
             ]
         ],
-        "Diana": [
+        "diana": [
             [
                 "oven",
                 "home"
             ]
         ],
-        "Donald": [
+        "donald": [
             [
                 "car",
                 "home"
             ],
             [
                 "car",
                 "home"
@@ -625,15 +625,15 @@
                 "city"
             ],
             [
                 "dog",
                 "kitchen"
             ]
         ],
-        "Dylan": [
+        "dylan": [
             [
                 "elephant",
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
@@ -651,15 +651,15 @@
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Elijah": [
+        "elijah": [
             [
                 "train",
                 "farm"
             ],
             [
                 "train",
                 "zoo"
@@ -721,15 +721,15 @@
                 "home"
             ],
             [
                 "oven",
                 "home"
             ]
         ],
-        "Ethan": [
+        "ethan": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -751,15 +751,15 @@
                 "sky"
             ],
             [
                 "kite",
                 "air"
             ]
         ],
-        "Evelyn": [
+        "evelyn": [
             [
                 "elephant",
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
@@ -793,15 +793,15 @@
                 "home"
             ],
             [
                 "donut",
                 "bakery"
             ]
         ],
-        "Frank": [
+        "frank": [
             [
                 "train",
                 "circus"
             ],
             [
                 "train",
                 "circus"
@@ -815,15 +815,15 @@
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
             ]
         ],
-        "Gloria": [
+        "gloria": [
             [
                 "sheep",
                 "kitchen"
             ],
             [
                 "sheep",
                 "farm"
@@ -853,15 +853,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "kennel"
             ]
         ],
-        "Gregory": [
+        "gregory": [
             [
                 "oven",
                 "home"
             ],
             [
                 "oven",
                 "home"
@@ -907,15 +907,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "Isabella": [
+        "isabella": [
             [
                 "train",
                 "kitchen"
             ],
             [
                 "bird",
                 "tree"
@@ -929,15 +929,15 @@
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Jack": [
+        "jack": [
             [
                 "sandwich",
                 "lunchbox"
             ],
             [
                 "sandwich",
                 "lunchbox"
@@ -987,15 +987,15 @@
                 "home"
             ],
             [
                 "oven",
                 "home"
             ]
         ],
-        "Jacob": [
+        "jacob": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -1041,15 +1041,15 @@
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "James": [
+        "james": [
             [
                 "sheep",
                 "nursery"
             ],
             [
                 "sheep",
                 "nursery"
@@ -1087,15 +1087,15 @@
                 "air"
             ],
             [
                 "bicycle",
                 "air"
             ]
         ],
-        "Jean": [
+        "jean": [
             [
                 "sandwich",
                 "lunchbox"
             ],
             [
                 "sandwich",
                 "lunchbox"
@@ -1125,15 +1125,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Jennifer": [
+        "jennifer": [
             [
                 "keyboard",
                 "kennel"
             ],
             [
                 "keyboard",
                 "kennel"
@@ -1163,15 +1163,15 @@
                 "lunchbox"
             ],
             [
                 "sandwich",
                 "kitchen"
             ]
         ],
-        "Joan": [
+        "joan": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -1185,35 +1185,35 @@
                 "lap"
             ],
             [
                 "donut",
                 "movie"
             ]
         ],
-        "John": [
+        "john": [
             [
                 "kite",
                 "air"
             ]
         ],
-        "Jose": [
+        "jose": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Judith": [
+        "judith": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "park"
@@ -1235,15 +1235,15 @@
                 "tree"
             ],
             [
                 "bird",
                 "kitchen"
             ]
         ],
-        "Julie": [
+        "julie": [
             [
                 "car",
                 "city"
             ],
             [
                 "car",
                 "city"
@@ -1297,15 +1297,15 @@
                 "nursery"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Justin": [
+        "justin": [
             [
                 "car",
                 "city"
             ],
             [
                 "car",
                 "city"
@@ -1327,15 +1327,15 @@
                 "city"
             ],
             [
                 "car",
                 "city"
             ]
         ],
-        "Kathleen": [
+        "kathleen": [
             [
                 "kite",
                 "air"
             ],
             [
                 "kite",
                 "air"
@@ -1365,15 +1365,15 @@
                 "bathroom"
             ],
             [
                 "elephant",
                 "lap"
             ]
         ],
-        "Keith": [
+        "keith": [
             [
                 "car",
                 "city"
             ],
             [
                 "car",
                 "city"
@@ -1399,15 +1399,15 @@
                 "cupboard"
             ],
             [
                 "sheep",
                 "farm"
             ]
         ],
-        "Larry": [
+        "larry": [
             [
                 "airplane",
                 "cupboard"
             ],
             [
                 "airplane",
                 "sky"
@@ -1449,15 +1449,15 @@
                 "home"
             ],
             [
                 "oven",
                 "bathroom"
             ]
         ],
-        "Laura": [
+        "laura": [
             [
                 "handbag",
                 "store"
             ],
             [
                 "handbag",
                 "store"
@@ -1503,15 +1503,15 @@
                 "cupboard"
             ],
             [
                 "airplane",
                 "nursery"
             ]
         ],
-        "Lauren": [
+        "lauren": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "countryside"
@@ -1521,15 +1521,15 @@
                 "countryside"
             ],
             [
                 "bird",
                 "countryside"
             ]
         ],
-        "Linda": [
+        "linda": [
             [
                 "handbag",
                 "store"
             ],
             [
                 "handbag",
                 "store"
@@ -1539,15 +1539,15 @@
                 "store"
             ],
             [
                 "sheep",
                 "farm"
             ]
         ],
-        "Lisa": [
+        "lisa": [
             [
                 "car",
                 "city"
             ],
             [
                 "car",
                 "lunchbox"
@@ -1569,29 +1569,29 @@
                 "lunchbox"
             ],
             [
                 "boat",
                 "water"
             ]
         ],
-        "Margaret": [
+        "margaret": [
             [
                 "airplane",
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "Marilyn": [
+        "marilyn": [
             [
                 "train",
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
@@ -1613,15 +1613,15 @@
                 "zoo"
             ],
             [
                 "train",
                 "zoo"
             ]
         ],
-        "Martha": [
+        "martha": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "cupboard"
@@ -1655,15 +1655,15 @@
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
             ]
         ],
-        "Matthew": [
+        "matthew": [
             [
                 "oven",
                 "home"
             ],
             [
                 "oven",
                 "home"
@@ -1721,15 +1721,15 @@
                 "classroom"
             ],
             [
                 "car",
                 "apartment"
             ]
         ],
-        "Michael": [
+        "michael": [
             [
                 "elephant",
                 "circus"
             ],
             [
                 "elephant",
                 "water"
@@ -1803,15 +1803,15 @@
                 "bakery"
             ],
             [
                 "donut",
                 "garage"
             ]
         ],
-        "Nancy": [
+        "nancy": [
             [
                 "bicycle",
                 "movie"
             ],
             [
                 "kite",
                 "air"
@@ -1865,15 +1865,15 @@
                 "park"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Natalie": [
+        "natalie": [
             [
                 "bird",
                 "tree"
             ],
             [
                 "bird",
                 "tree"
@@ -1923,15 +1923,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Nicholas": [
+        "nicholas": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "park"
@@ -1965,15 +1965,15 @@
                 "farm"
             ],
             [
                 "sheep",
                 "farm"
             ]
         ],
-        "Olivia": [
+        "olivia": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -2031,15 +2031,15 @@
                 "movie"
             ],
             [
                 "sheep",
                 "farm"
             ]
         ],
-        "Patricia": [
+        "patricia": [
             [
                 "sheep",
                 "zoo"
             ],
             [
                 "sheep",
                 "zoo"
@@ -2065,15 +2065,15 @@
                 "city"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Rachel": [
+        "rachel": [
             [
                 "train",
                 "store"
             ],
             [
                 "bicycle",
                 "garage"
@@ -2087,15 +2087,15 @@
                 "garage"
             ],
             [
                 "bicycle",
                 "garage"
             ]
         ],
-        "Raymond": [
+        "raymond": [
             [
                 "handbag",
                 "store"
             ],
             [
                 "handbag",
                 "store"
@@ -2141,15 +2141,15 @@
                 "garage"
             ],
             [
                 "keyboard",
                 "garage"
             ]
         ],
-        "Rebecca": [
+        "rebecca": [
             [
                 "boat",
                 "water"
             ],
             [
                 "boat",
                 "water"
@@ -2191,15 +2191,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Roger": [
+        "roger": [
             [
                 "train",
                 "farm"
             ],
             [
                 "train",
                 "farm"
@@ -2225,15 +2225,15 @@
                 "zoo"
             ],
             [
                 "train",
                 "farm"
             ]
         ],
-        "Scott": [
+        "scott": [
             [
                 "boat",
                 "water"
             ],
             [
                 "boat",
                 "store"
@@ -2259,15 +2259,15 @@
                 "store"
             ],
             [
                 "boat",
                 "store"
             ]
         ],
-        "Stephanie": [
+        "stephanie": [
             [
                 "donut",
                 "apartment"
             ],
             [
                 "donut",
                 "bakery"
@@ -2317,15 +2317,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Steven": [
+        "steven": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
@@ -2363,43 +2363,43 @@
                 "city"
             ],
             [
                 "bird",
                 "city"
             ]
         ],
-        "Susan": [
+        "susan": [
             [
                 "airplane",
                 "house"
             ],
             [
                 "airplane",
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Teresa": [
+        "teresa": [
             [
                 "donut",
                 "bakery"
             ],
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Walter": [
+        "walter": [
             [
                 "car",
                 "city"
             ],
             [
                 "car",
                 "cupboard"
```

### Comparing `room_env-1.0.2/room_env/data/des-config-m-v1.json` & `room_env-1.0.3/room_env/data/des-config-m-v1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'components'": "{replace: OrderedDict([('gregory', [['handbag', 'store'], ['handbag', 'store'], "*

 * *                 "['handbag', 'store'], ['handbag', 'store'], ['handbag', 'store'], ['handbag', "*

 * *                 "'store'], ['handbag', 'store'], ['handbag', 'store']]), ('roger', [['bowl', "*

 * *                 "'cupboard'], ['bowl', 'cupboard'], ['bowl', 'cupboard'], ['bowl', 'cupboard'], "*

 * *                 "['bowl', 'cupboard'], ['bowl', 'cupboard'], ['bowl', 'cupboard']]), ('dylan', "*

 * *                 "[[' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "complexity": 12288,
     "components": {
-        "Alexander": [
+        "alexander": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -15,15 +15,15 @@
                 "cupboard"
             ],
             [
                 "keyboard",
                 "lap"
             ]
         ],
-        "Amanda": [
+        "amanda": [
             [
                 "airplane",
                 "bakery"
             ],
             [
                 "airplane",
                 "circus"
@@ -41,15 +41,15 @@
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Anthony": [
+        "anthony": [
             [
                 "dog",
                 "table"
             ],
             [
                 "dog",
                 "table"
@@ -95,25 +95,25 @@
                 "bakery"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Beverly": [
+        "beverly": [
             [
                 "airplane",
                 "sky"
             ],
             [
                 "handbag",
                 "office"
             ]
         ],
-        "Brenda": [
+        "brenda": [
             [
                 "bowl",
                 "nursery"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -159,15 +159,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "office"
             ]
         ],
-        "Brittany": [
+        "brittany": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "park"
@@ -177,15 +177,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Carol": [
+        "carol": [
             [
                 "sandwich",
                 "circus"
             ],
             [
                 "sandwich",
                 "circus"
@@ -199,15 +199,15 @@
                 "circus"
             ],
             [
                 "sandwich",
                 "circus"
             ]
         ],
-        "Christina": [
+        "christina": [
             [
                 "handbag",
                 "office"
             ],
             [
                 "handbag",
                 "store"
@@ -221,15 +221,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "office"
             ]
         ],
-        "David": [
+        "david": [
             [
                 "boat",
                 "water"
             ],
             [
                 "boat",
                 "water"
@@ -251,15 +251,15 @@
                 "water"
             ],
             [
                 "elephant",
                 "circus"
             ]
         ],
-        "Donald": [
+        "donald": [
             [
                 "bowl",
                 "bathroom"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -273,15 +273,15 @@
                 "cupboard"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Dylan": [
+        "dylan": [
             [
                 "boat",
                 "water"
             ],
             [
                 "keyboard",
                 "desk"
@@ -291,15 +291,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Gloria": [
+        "gloria": [
             [
                 "airplane",
                 "sky"
             ],
             [
                 "airplane",
                 "city"
@@ -321,15 +321,15 @@
                 "city"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Gregory": [
+        "gregory": [
             [
                 "handbag",
                 "store"
             ],
             [
                 "handbag",
                 "store"
@@ -355,15 +355,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "Jack": [
+        "jack": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "countryside"
@@ -373,25 +373,25 @@
                 "countryside"
             ],
             [
                 "dog",
                 "countryside"
             ]
         ],
-        "Jacob": [
+        "jacob": [
             [
                 "sandwich",
                 "bakery"
             ],
             [
                 "sandwich",
                 "bakery"
             ]
         ],
-        "John": [
+        "john": [
             [
                 "elephant",
                 "circus"
             ],
             [
                 "elephant",
                 "desk"
@@ -405,25 +405,25 @@
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
             ]
         ],
-        "Judith": [
+        "judith": [
             [
                 "sandwich",
                 "lunchbox"
             ],
             [
                 "sandwich",
                 "table"
             ]
         ],
-        "Justin": [
+        "justin": [
             [
                 "bowl",
                 "kennel"
             ],
             [
                 "bowl",
                 "kennel"
@@ -437,15 +437,15 @@
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Kathleen": [
+        "kathleen": [
             [
                 "elephant",
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
@@ -467,39 +467,39 @@
                 "office"
             ],
             [
                 "elephant",
                 "circus"
             ]
         ],
-        "Keith": [
+        "keith": [
             [
                 "boat",
                 "zoo"
             ],
             [
                 "boat",
                 "zoo"
             ],
             [
                 "boat",
                 "zoo"
             ]
         ],
-        "Laura": [
+        "laura": [
             [
                 "airplane",
                 "nursery"
             ],
             [
                 "airplane",
                 "nursery"
             ]
         ],
-        "Lauren": [
+        "lauren": [
             [
                 "boat",
                 "water"
             ],
             [
                 "boat",
                 "water"
@@ -553,15 +553,15 @@
                 "circus"
             ],
             [
                 "elephant",
                 "circus"
             ]
         ],
-        "Lisa": [
+        "lisa": [
             [
                 "boat",
                 "farm"
             ],
             [
                 "boat",
                 "farm"
@@ -587,15 +587,15 @@
                 "water"
             ],
             [
                 "boat",
                 "farm"
             ]
         ],
-        "Marilyn": [
+        "marilyn": [
             [
                 "airplane",
                 "table"
             ],
             [
                 "airplane",
                 "sky"
@@ -609,15 +609,15 @@
                 "table"
             ],
             [
                 "airplane",
                 "table"
             ]
         ],
-        "Martha": [
+        "martha": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -643,15 +643,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Michael": [
+        "michael": [
             [
                 "boat",
                 "water"
             ],
             [
                 "boat",
                 "water"
@@ -697,15 +697,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "Nancy": [
+        "nancy": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -731,15 +731,15 @@
                 "water"
             ],
             [
                 "boat",
                 "water"
             ]
         ],
-        "Natalie": [
+        "natalie": [
             [
                 "handbag",
                 "store"
             ],
             [
                 "handbag",
                 "store"
@@ -761,15 +761,15 @@
                 "store"
             ],
             [
                 "handbag",
                 "store"
             ]
         ],
-        "Patricia": [
+        "patricia": [
             [
                 "bowl",
                 "countryside"
             ],
             [
                 "bowl",
                 "countryside"
@@ -811,15 +811,15 @@
                 "bakery"
             ],
             [
                 "sandwich",
                 "lunchbox"
             ]
         ],
-        "Raymond": [
+        "raymond": [
             [
                 "boat",
                 "lunchbox"
             ],
             [
                 "boat",
                 "water"
@@ -841,21 +841,21 @@
                 "lunchbox"
             ],
             [
                 "boat",
                 "lunchbox"
             ]
         ],
-        "Rebecca": [
+        "rebecca": [
             [
                 "boat",
                 "water"
             ]
         ],
-        "Roger": [
+        "roger": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
```

### Comparing `room_env-1.0.2/room_env/data/des-config-s-v1.json` & `room_env-1.0.3/room_env/data/des-config-s-v1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'components'": "{replace: OrderedDict([('patricia', [['dog', 'store'], ['dog', 'store'], ['dog', "*

 * *                 "'kennel'], ['dog', 'store'], ['dog', 'store'], ['dog', 'kennel'], ['dog', "*

 * *                 "'store']]), ('laura', [['airplane', 'sky'], ['airplane', 'sky'], ['airplane', "*

 * *                 "'sky'], ['airplane', 'sky'], ['airplane', 'sky'], ['airplane', 'sky'], "*

 * *                 "['airplane', 'sky'], ['airplane', 'sky']]), ('dylan', [['bowl', 'cupboard'], "*

 * *                 "['bowl', 'air […]*

```diff
@@ -1,11 +1,11 @@
 {
     "complexity": 2048,
     "components": {
-        "Alexander": [
+        "alexander": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -15,25 +15,25 @@
                 "cupboard"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Anthony": [
+        "anthony": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Beverly": [
+        "beverly": [
             [
                 "keyboard",
                 "bakery"
             ],
             [
                 "keyboard",
                 "bakery"
@@ -47,21 +47,21 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "bakery"
             ]
         ],
-        "Brenda": [
+        "brenda": [
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Brittany": [
+        "brittany": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -103,15 +103,15 @@
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Carol": [
+        "carol": [
             [
                 "keyboard",
                 "park"
             ],
             [
                 "keyboard",
                 "park"
@@ -137,15 +137,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Christina": [
+        "christina": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -167,15 +167,15 @@
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Dylan": [
+        "dylan": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "air"
@@ -197,15 +197,15 @@
                 "cupboard"
             ],
             [
                 "bowl",
                 "air"
             ]
         ],
-        "Gloria": [
+        "gloria": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "closet"
@@ -223,15 +223,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "John": [
+        "john": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -285,15 +285,15 @@
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
             ]
         ],
-        "Keith": [
+        "keith": [
             [
                 "airplane",
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
@@ -339,15 +339,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Laura": [
+        "laura": [
             [
                 "airplane",
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
@@ -373,15 +373,15 @@
                 "sky"
             ],
             [
                 "airplane",
                 "sky"
             ]
         ],
-        "Lisa": [
+        "lisa": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "cupboard"
@@ -395,15 +395,15 @@
                 "cupboard"
             ],
             [
                 "dog",
                 "cupboard"
             ]
         ],
-        "Martha": [
+        "martha": [
             [
                 "keyboard",
                 "desk"
             ],
             [
                 "keyboard",
                 "desk"
@@ -441,15 +441,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "cupboard"
             ]
         ],
-        "Patricia": [
+        "patricia": [
             [
                 "dog",
                 "store"
             ],
             [
                 "dog",
                 "store"
@@ -471,15 +471,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "store"
             ]
         ],
-        "Roger": [
+        "roger": [
             [
                 "keyboard",
                 "classroom"
             ],
             [
                 "keyboard",
                 "desk"
```

### Comparing `room_env-1.0.2/room_env/data/des-config-xs-v1.json` & `room_env-1.0.3/room_env/data/des-config-xs-v1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'components'": "{replace: OrderedDict([('beverly', [['bowl', 'cupboard'], ['bowl', 'cupboard'], "*

 * *                 "['bowl', 'cupboard'], ['bowl', 'cupboard'], ['dog', 'kennel'], ['dog', 'lap'], "*

 * *                 "['dog', 'kennel'], ['dog', 'kennel'], ['dog', 'lap'], ['dog', 'kennel'], ['dog', "*

 * *                 "'lap'], ['dog', 'lap']]), ('john', [['dog', 'kennel'], ['dog', 'kennel'], "*

 * *                 "['dog', 'kennel'], ['dog', 'kennel'], ['dog', 'kennel'], ['dog', 'kennel'], "*

 * *                 "['bo […]*

```diff
@@ -1,21 +1,21 @@
 {
     "complexity": 512,
     "components": {
-        "Anthony": [
+        "anthony": [
             [
                 "dog",
                 "bakery"
             ],
             [
                 "dog",
                 "bakery"
             ]
         ],
-        "Beverly": [
+        "beverly": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -57,15 +57,15 @@
                 "lap"
             ],
             [
                 "dog",
                 "lap"
             ]
         ],
-        "Brittany": [
+        "brittany": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -79,15 +79,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Carol": [
+        "carol": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "bowl",
                 "desk"
@@ -113,15 +113,15 @@
                 "desk"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "John": [
+        "john": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
@@ -147,25 +147,25 @@
                 "desk"
             ],
             [
                 "bowl",
                 "desk"
             ]
         ],
-        "Lisa": [
+        "lisa": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Patricia": [
+        "patricia": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -207,15 +207,15 @@
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
             ]
         ],
-        "Roger": [
+        "roger": [
             [
                 "dog",
                 "kennel"
             ],
             [
                 "dog",
                 "kennel"
```

### Comparing `room_env-1.0.2/room_env/data/des-config-xxs-v1.json` & `room_env-1.0.3/room_env/data/des-config-xxs-v1.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'components'": "{replace: OrderedDict([('brittany', [['bowl', 'cupboard'], ['bowl', "*

 * *                 "'cupboard']]), ('patricia', [['bowl', 'cupboard'], ['bowl', 'cupboard'], "*

 * *                 "['bowl', 'cupboard'], ['bowl', 'cupboard'], ['bowl', 'cupboard'], ['bowl', "*

 * *                 "'cupboard'], ['bowl', 'desk'], ['bowl', 'cupboard']]), ('roger', [['bowl', "*

 * *                 "'circus']]), ('beverly', [['bowl', 'cupboard'], ['bowl', 'cupboard'], ['bowl', "*

 * *                 "'cupboard'], ['bowl', 'c […]*

```diff
@@ -1,11 +1,11 @@
 {
     "complexity": 128,
     "components": {
-        "Beverly": [
+        "beverly": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -15,25 +15,25 @@
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Brittany": [
+        "brittany": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Patricia": [
+        "patricia": [
             [
                 "bowl",
                 "cupboard"
             ],
             [
                 "bowl",
                 "cupboard"
@@ -59,15 +59,15 @@
                 "desk"
             ],
             [
                 "bowl",
                 "cupboard"
             ]
         ],
-        "Roger": [
+        "roger": [
             [
                 "bowl",
                 "circus"
             ]
         ]
     },
     "last_timestep": 128,
```

### Comparing `room_env-1.0.2/room_env/data/ms-coco-80-categories` & `room_env-1.0.3/room_env/data/ms-coco-80-categories`

 * *Files identical despite different names*

### Comparing `room_env-1.0.2/room_env/data/semantic-knowledge-small.json` & `room_env-1.0.3/room_env/data/semantic-knowledge-small.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'bicycle'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'garage'), ('weight', "*

 * *              '1)])])])}',*

 * * "'bird'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'tree'), ('weight', "*

 * *           '4)])])])}',*

 * * "'car'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'city'), ('weight', "*

 * *          '1)])])])}',*

 * * "'cat'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'lap'), ('weight', "*

 * *          '10)])])])}',*

 * * "'chair'": "{replace: OrderedDi […]*

```diff
@@ -1,82 +1,82 @@
 {
     "bicycle": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "bird": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "tree",
                 "weight": 4
             }
         ]
     },
     "car": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "city",
                 "weight": 1
             }
         ]
     },
     "cat": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "lap",
                 "weight": 10
             }
         ]
     },
     "chair": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "office",
                 "weight": 8
             }
         ]
     },
     "couch": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "house",
                 "weight": 5
             }
         ]
     },
     "cup": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "table",
                 "weight": 4
             }
         ]
     },
     "dog": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "park",
                 "weight": 1
             }
         ]
     },
     "laptop": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "desk",
                 "weight": 1
             }
         ]
     },
     "person": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "building",
                 "weight": 1
             }
         ]
     }
 }
```

### Comparing `room_env-1.0.2/room_env/data/semantic-knowledge.json` & `room_env-1.0.3/room_env/data/semantic-knowledge.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'airplane'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'sky'), ('weight', "*

 * *               '1)])])])}',*

 * * "'apple'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'apple_tree'), "*

 * *            "('weight', 1)])])])}",*

 * * "'banana'": '{replace: OrderedDict([(\'atlocation\', [OrderedDict([(\'tail\', "monkey\'s_hand"), '*

 * *             "('weight', 1)])])])}",*

 * * "'bear'": "{replace: OrderedDict([('atlocation', [OrderedDict([('tail', 'park'), ('weight', "*

 * *           '1)])])])}',*

 * * "' […]*

```diff
@@ -1,530 +1,530 @@
 {
     "airplane": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "sky",
                 "weight": 1
             }
         ]
     },
     "apple": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "apple_tree",
                 "weight": 1
             }
         ]
     },
     "banana": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "monkey's_hand",
                 "weight": 1
             }
         ]
     },
     "bear": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "park",
                 "weight": 1
             }
         ]
     },
     "bed": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "house",
                 "weight": 1
             }
         ]
     },
     "bench": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bus_stop",
                 "weight": 1
             }
         ]
     },
     "bicycle": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "bird": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "tree",
                 "weight": 1
             }
         ]
     },
     "boat": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "water",
                 "weight": 1
             }
         ]
     },
     "book": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "classroom",
                 "weight": 1
             }
         ]
     },
     "bottle": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "nursery",
                 "weight": 1
             }
         ]
     },
     "bowl": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "cupboard",
                 "weight": 1
             }
         ]
     },
     "broccoli": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "farmer's_market",
                 "weight": 1
             }
         ]
     },
     "bus": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bus_stop",
                 "weight": 1
             }
         ]
     },
     "cake": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bakery",
                 "weight": 1
             }
         ]
     },
     "car": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "city",
                 "weight": 1
             }
         ]
     },
     "cat": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "lap",
                 "weight": 1
             }
         ]
     },
     "cell_phone": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "backpack",
                 "weight": 1
             }
         ]
     },
     "chair": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "office",
                 "weight": 1
             }
         ]
     },
     "clock": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "desk",
                 "weight": 1
             }
         ]
     },
     "couch": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "house",
                 "weight": 1
             }
         ]
     },
     "cow": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "countryside",
                 "weight": 1
             }
         ]
     },
     "cup": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "table",
                 "weight": 1
             }
         ]
     },
     "dining_table": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "house",
                 "weight": 1
             }
         ]
     },
     "dog": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "kennel",
                 "weight": 1
             }
         ]
     },
     "donut": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bakery",
                 "weight": 1
             }
         ]
     },
     "elephant": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "circus",
                 "weight": 1
             }
         ]
     },
     "fire_hydrant": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "corner_of_two_streets",
                 "weight": 1
             }
         ]
     },
     "fork": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "kitchen",
                 "weight": 1
             }
         ]
     },
     "frisbee": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "park",
                 "weight": 1
             }
         ]
     },
     "giraffe": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "zoo",
                 "weight": 1
             }
         ]
     },
     "handbag": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "store",
                 "weight": 1
             }
         ]
     },
     "horse": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "race_track",
                 "weight": 1
             }
         ]
     },
     "hot_dog": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "soccer_game",
                 "weight": 1
             }
         ]
     },
     "keyboard": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "desk",
                 "weight": 1
             }
         ]
     },
     "kite": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "air",
                 "weight": 1
             }
         ]
     },
     "knife": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "kitchen",
                 "weight": 1
             }
         ]
     },
     "laptop": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "internet_cafe",
                 "weight": 1
             }
         ]
     },
     "microwave": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "apartment",
                 "weight": 1
             }
         ]
     },
     "motorcycle": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "mouse": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "hole_in_wall",
                 "weight": 1
             }
         ]
     },
     "oven": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "home",
                 "weight": 1
             }
         ]
     },
     "person": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bus_stop",
                 "weight": 1
             }
         ]
     },
     "pizza": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "oven",
                 "weight": 1
             }
         ]
     },
     "potted_plant": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "windowsill",
                 "weight": 1
             }
         ]
     },
     "refrigerator": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "sandwich": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "lunchbox",
                 "weight": 1
             }
         ]
     },
     "scissors": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "desk",
                 "weight": 1
             }
         ]
     },
     "sheep": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "farm",
                 "weight": 1
             }
         ]
     },
     "sink": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "kitchen",
                 "weight": 1
             }
         ]
     },
     "skis": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "spoon": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bowl",
                 "weight": 1
             }
         ]
     },
     "sports_ball": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "school",
                 "weight": 1
             }
         ]
     },
     "stop_sign": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "corner_of_two_streets",
                 "weight": 1
             }
         ]
     },
     "suitcase": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "movie",
                 "weight": 1
             }
         ]
     },
     "teddy_bear": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "toy_store",
                 "weight": 1
             }
         ]
     },
     "toilet": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "bathroom",
                 "weight": 1
             }
         ]
     },
     "toothbrush": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "suitcase",
                 "weight": 1
             }
         ]
     },
     "traffic_light": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "corner_of_two_streets",
                 "weight": 1
             }
         ]
     },
     "train": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "zoo",
                 "weight": 1
             }
         ]
     },
     "truck": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "garage",
                 "weight": 1
             }
         ]
     },
     "tv": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "house",
                 "weight": 1
             }
         ]
     },
     "umbrella": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "closet",
                 "weight": 1
             }
         ]
     },
     "vase": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "table",
                 "weight": 1
             }
         ]
     },
     "wine_glass": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "cupboard",
                 "weight": 1
             }
         ]
     },
     "zebra": {
-        "AtLocation": [
+        "atlocation": [
             {
                 "tail": "zoo",
                 "weight": 1
             }
         ]
     }
 }
```

### Comparing `room_env-1.0.2/room_env/des.py` & `room_env-1.0.3/room_env/des.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,89 @@
 """Discrete Event Simlator (RoomDes) for the Room."""
-import json
-import os
+
 from copy import deepcopy
 from pprint import pprint
 
+from .utils import read_json_prod as read_json
+from .utils import write_json
 
-def read_json(fname: str) -> dict:
-    """Read json.
 
-    There is some path magic going on here. This is to account for both the production
-    and development mode. Don't use this function for a general purpose.
+def fill_des_resources(des_size: str) -> None:
+    """Fill resources
 
-    """
-    fullpath = os.path.join(os.path.dirname(__file__), fname)
+    Args:
+        des_size
 
-    with open(fullpath, "r") as stream:
-        return json.load(stream)
+    """
+    des = RoomDes(des_size=des_size, check_resources=False)
+    des.run()
+    resources = {
+        foo: 9999
+        for foo in set(
+            [bar["object_location"] for foo in des.states for bar in foo.values()]
+        )
+    }
+    des.config["resources"] = deepcopy(resources)
+    write_json(des.config, f"./room_env/data/des-config-{des_size}.json")
+    resources = []
+    des = RoomDes(des_size=des_size, check_resources=True)
+    resources.append(deepcopy(des.resources))
+    while des.until > 0:
+        des.step()
+        des.until -= 1
+        resources.append(deepcopy(des.resources))
+
+    object_locations = deepcopy(list(des.resources.keys()))
+    resources = {
+        object_location: 9999
+        - min([resource[object_location] for resource in resources])
+        for object_location in object_locations
+    }
+
+    des.config["resources"] = deepcopy(resources)
+    write_json(des.config, f"./room_env/data/des-config-{des_size}.json")
+    des = RoomDes(des_size=des_size, check_resources=True)
 
 
 class RoomDes:
-
     """RoomDes Class.
 
     This class is very simple at the moment. When it's initialized, it places N_{humans}
     in the room. They periodically move to other locations. They also periodically
     change the location of their objects they are holding. At the moment,
     everything is deterministic.
 
     """
 
     def __init__(self, des_size: str = "l", check_resources: bool = True) -> None:
         """Instantiate the class.
 
-        Args
-        ----
-        des_size: configuartion for the RoomDes simulation. It should be either size or
-            dict. size can be "xxs (extra extra small", "xs (extra small)", "s (small)",
-            "m (medium)", or "l (large)".
+        Args:
+            des_size: configuartion for the RoomDes simulation. It should be either size or
+                dict. size can be "xxs (extra extra small", "xs (extra small)", "s (small)",
+                "m (medium)", or "l (large)".
 
-            {"components": <COMPONENTS>, "resources": <RESOURCES>,
-            "last_timestep": <LAST_TIMESTEP>,
-            "semantic_knowledge": <SEMANTIC_KNOWLEDGE>, "complexity", <COMPLEXITY>}
+                {"components": <COMPONENTS>, "resources": <RESOURCES>,
+                "last_timestep": <LAST_TIMESTEP>,
+                "semantic_knowledge": <SEMANTIC_KNOWLEDGE>, "complexity", <COMPLEXITY>}
 
-            <COMPONENTS> should look like this:
+                <COMPONENTS> should look like this:
 
-            <RESOURCES> should look like this:
+                <RESOURCES> should look like this:
 
-            {'desk': 2, 'A': 10000, 'lap': 10000}
+                {'desk': 2, 'A': 10000, 'lap': 10000}
 
-            <LAST_TIMESTEP> is a number where the DES terminates.
+                <LAST_TIMESTEP> is a number where the DES terminates.
 
-            <SEMANTIC_KNOWLEDGE> is a dictionary of semantic knowledge.
+                <SEMANTIC_KNOWLEDGE> is a dictionary of semantic knowledge.
 
-            <COMPLEXITY> is defined as num_humans * num_total_objects
-            * maximum_num_objects_per_human * maximum_num_locations_per_object
+                <COMPLEXITY> is defined as num_humans * num_total_objects
+                * maximum_num_objects_per_human * maximum_num_locations_per_object
 
-        check_resources: whether to check if the resources are depleted or not.
+            check_resources: whether to check if the resources are depleted or not.
 
         """
         if isinstance(des_size, str):
             assert des_size.lower() in [
                 "dev",
                 "xxs",
                 "xs",
@@ -73,15 +97,18 @@
         self.check_resources = check_resources
         self._initialize()
 
     def _initialize(self) -> None:
         """Initialize the simulator."""
         self.components = deepcopy(self.config["components"])
         self.resources = deepcopy(self.config["resources"])
-        self.semantic_knowledge = deepcopy(self.config["semantic_knowledge"])
+        self.semantic_knowledge = [
+            [key, "atlocation", val]
+            for key, val in self.config["semantic_knowledge"].items()
+        ]
 
         self.humans = []
         self.objects = []
         self.object_locations = []
 
         for human, obj_locs in self.components.items():
             self.humans.append(human)
@@ -159,24 +186,22 @@
         previous_state: dict,
         previous_resources: dict,
         current_state: dict,
         current_resources: dict,
     ) -> dict:
         """Check if any events have occured between the two consecutive states.
 
-        Args
-        ----
-        previous_state
-        previous_resources
-        current_state
-        current_resources
-
-        Returns
-        -------
-        event
+        Args:
+            previous_state
+            previous_resources
+            current_state
+            current_resources
+
+        Returns:
+            event
 
         """
         assert len(previous_state) == len(current_state)
         assert len(previous_resources) == len(current_resources)
 
         state_changes = {}
         resource_changes = {}
```

### Comparing `room_env-1.0.2/room_env/envs/room0.py` & `room_env-1.0.3/room_env/envs/room0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,29 @@
-"""Room environment compatible with gym.
-I advise you to check out room1.py, as it's more general.
-"""
-import json
+"""RoomEnv0 environment compatible with gym."""
+
 import logging
 import os
 import random
-from copy import deepcopy
 from itertools import cycle
-from typing import Tuple
 
 import gymnasium as gym
 
-from ..utils import read_lines, remove_name, split_name_entity
+from ..utils import read_json_prod as read_json
+from ..utils import read_lines, split_by_possessive
 
 CORRECT = 1
 WRONG = 0
 
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO").upper(),
     format="%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
-def read_json(fname: str) -> dict:
-    """Read json.
-
-    There is some path magic going on here. This is to account for both the production
-    and development mode. Don't use this function for a general purpose.
-
-    """
-    fullpath = os.path.join(os.path.dirname(__file__), "../", fname)
-
-    with open(fullpath, "r") as stream:
-        return json.load(stream)
-
-
 class RoomEnv0(gym.Env):
     """The Room environment version 0.
 
     In this big room, N_{agents} move around and observe N_{humans} placing objects.
     Every time the agents move around (i.e., take a step), they observe one human_{i}
     placing an object somewhere. Each agent can only observe one human at a time.
     Every time the agents takes a step, the environment also asks them where an object
@@ -55,50 +39,49 @@
 
     (2) The room environment changes every time. The humans can switch their locations,
     change their objects, and place them at different locations. These changes are
     not completely random. A decent portion of them come from commmon-sense knowledge.
     This means that an agent with both episodic and semantic memory systems will perform
     better than an agent with only one memory system.
 
+    Every string value is lower-cased to avoid confusion!!!
+
     """
 
     metadata = {"render.modes": ["console"]}
 
     def __init__(
         self,
         room_size: str = "small",
-        weighting_mode: str = "highest",
         probs: dict = {
             "commonsense": 0.7,
             "new_location": 0.1,
             "new_object": 0.1,
             "switch_person": 0.5,
         },
         limits: dict = {
             "heads": None,
             "tails": None,
             "names": None,
-            "allow_spaces": False,
+            "allow_spaces": True,
         },
         max_step: int = 1000,
         disjoint_entities: bool = True,
         num_agents: int = 1,
     ) -> None:
         """Initialize the environment.
 
-        Args
-        ----
-        room_size: small or big
-        weighting_mode: Either "weighted" or "highest"
-        probs: the probabilities that govern the room environment changes.
-        limits: Limitation on the triples.
-        max_step: maximum step an agent can take. The environment will terminate when
-            the number reaches this value.
-        disjoint_entities: Assure that the heads and the tails don't overlap.
-        num_agents: number of agents in the room.
+        Args:
+            room_size: small or big
+            probs: the probabilities that govern the room environment changes.
+            limits: Limitation on the triples.
+            max_step: maximum step an agent can take. The environment will terminate when
+                the number reaches this value.
+            disjoint_entities: Assure that the heads and the tails don't overlap.
+            num_agents: number of agents in the room.
 
         """
         super().__init__()
         self.room_size = room_size
         if self.room_size.lower() == "small":
             semantic_knowledge_path = "./data/semantic-knowledge-small.json"
             names_path = "./data/top-human-names-small"
@@ -141,40 +124,39 @@
                 + len(self.names)
                 + len(self.heads)
                 + len(self.tails)
             )
 
             assert lhs == rhs
 
-        self.weighting_mode = weighting_mode
         self.probs = probs
         self.max_step = max_step
         self.num_agents = num_agents
         # Our state / action space is quite complex. Here we just make a dummy
         # observation space to bypass the sanity check.
         self.observation_space = gym.spaces.Discrete(1)
         self.action_space = gym.spaces.Discrete(1)
 
-    def reset(self) -> Tuple:
+    def reset(self) -> tuple:
         """Reset the environment.
 
         This will place N_{humans} humans in the room. Each human only has one object,
         which will be placed by the human in a random location.
 
         """
-        self.step_counter = 0
+        self.current_time = 0
         random.shuffle(self.names)
         random.shuffle(self.heads)
         self.room = []
 
         for name, head in zip(self.names, self.heads):
             relation = self.relations[0]  # At the moment there is only one relation.
             tail = self.generate_tail(head, relation)
             if tail is not None:
-                self.room.append([f"{name}'s {head}", relation, f"{name}'s {tail}"])
+                self.room.append([f"{name}'s {head}", relation, f"{tail}"])
 
         navigate = [[i for i in range(len(self.room))] for _ in range(self.num_agents)]
         for navigate_ in navigate:
             random.shuffle(navigate_)
 
         self.navigate = [cycle(navigate_) for navigate_ in navigate]
 
@@ -184,73 +166,62 @@
         info = {}
 
         return (observations, question), info
 
     def generate_observations(self) -> list:
         """Generate a random obseration.
 
-        Returns
-        -------
-        observations: e.g., ["Tae's laptop, "AtLocation", "Tae's desk", 10]
-
-        The last element in the list accounts for the timestamp.
+        Returns:
+            observations: e.g., ["tae's laptop, "atlocation", "tae's desk", 10]
+                The last element in the list accounts for the timestamp.
 
         """
         observations = {
-            i: deepcopy([*self.room[next(navigate_)], self.step_counter])
+            i: [*self.room[next(navigate_)], self.current_time]
             for i, navigate_ in enumerate(self.navigate)
         }
 
         return observations
 
-    def generate_qa(self) -> Tuple[list, str]:
+    def generate_qa(self) -> tuple[list, str]:
         """Generate a question and the answer.
 
-        Returns
-        -------
-        question: e.g., ["Tae's laptop", "AtLocation"]
-        answer: e.g., "Tae's desk"
+        Returns:
+            question: e.g., ["tae's laptop", "atlocation", "?", 10]
+            answer: e.g., desk
 
         """
         random_choice = random.choice(self.room)
-        question = random_choice[:2]
-        answer = remove_name(random_choice[-1])
+        question = random_choice[:2] + ["?"] + [self.current_time]
+        answer = random_choice[2]
 
         return question, answer
 
     def generate_tail(self, head: str, relation: str) -> str:
         """This simulates humans placing their objects in their desired locations.
 
         Note that "head" shouldn't include a human name.
 
         """
+        relevant_tails = [
+            triple[2]
+            for triple in self.semantic_knowledge
+            if triple[0] == head and triple[1] == relation
+        ]
+        assert len(relevant_tails) == 1
+
         if random.random() < self.probs["commonsense"]:
             logging.debug(f"Generating a common location for {head} ...")
-            tails = self.semantic_knowledge[head][relation]
-
-            if len(tails) == 0:
-                return None
-
-            if self.weighting_mode == "weighted":
-                tail = random.choices(
-                    [tail["tail"] for tail in tails],
-                    weights=[tail["weight"] for tail in tails],
-                    k=1,
-                )[0]
-            elif self.weighting_mode == "highest":
-                tail = sorted(
-                    self.semantic_knowledge[head][relation], key=lambda x: x["weight"]
-                )[-1]["tail"]
-            else:
-                raise ValueError
+            tail = relevant_tails[0]
         else:
             logging.debug(f"Generating a NON common location for {head} ...")
             while True:
                 tail = random.choice(self.tails)
-                if tail not in self.semantic_knowledge[head][relation]:
+
+                if tail not in relevant_tails:
                     break
 
         return tail
 
     def renew(self) -> None:
         """Renew the room.
 
@@ -269,18 +240,18 @@
         a new random object.
 
         With the chance of probs["switch_person"], two persons switch their spots.
 
         """
         room = []
         for head, relation, tail in self.room:
-            name1, head = split_name_entity(head)
-            name2, tail = split_name_entity(tail)
+            name1, head = split_by_possessive(head)
+            # name2, tail = split_by_possessive(tail)
 
-            assert name1 == name2, "we don't do name mixing at this moment."
+            # assert name1 == name2, "we don't do name mixing at this moment."
 
             if random.random() < self.probs["new_object"]:
                 while True:
                     new_head = random.choice(self.heads)
                     if new_head != head:
                         head = new_head
                         tail = self.generate_tail(head, relation)
@@ -290,19 +261,15 @@
                     while True:
                         new_tail = self.generate_tail(head, relation)
                         if new_tail != tail:
                             tail = new_tail
                             break
 
             room.append(
-                [
-                    f"{name1}'s {deepcopy(head)}",
-                    deepcopy(relation),
-                    f"{name2}'s {deepcopy(tail)}",
-                ],
+                [f"{name1}'s {head}", relation, f"{tail}"],
             )
 
         if random.random() < self.probs["switch_person"]:
             i, j = random.sample(
                 range(
                     0,
                     len(
@@ -311,45 +278,52 @@
                 ),
                 2,
             )
             room[i], room[j] = room[j], room[i]
 
         self.room = room
 
-    def step(self, action: str) -> Tuple[Tuple, int, bool, bool, dict]:
+    def step(self, action: str) -> tuple[tuple, int, bool, bool, dict]:
         """An agent takes an action.
 
-        Args
-        ----
-        action: This is the agent's answer to the previous question.
+        Args:
+            action: This is the agent's answer to the previous question.
+
+        Returns:
+            observations: e.g., ["tae's laptop, "atlocation", "tae's desk", 10]
+            question: e.g., ["tae's laptop", "atlocation", "?", 10]
+            answer: e.g., desk
+            reward: +1 for correct answer, 0 for wrong answer.
+            done: True if the current_time reaches the max_step.
+            truncated: False
 
         """
         if str(action).lower() == self.answer.lower():
             logging.info(
                 f"The prediction ({action}) matches the answer ({self.answer})!"
             )
             reward = CORRECT
 
         else:
             logging.info(
                 f"The prediction ({action}) does NOT match the answer ({self.answer})!"
             )
             reward = WRONG
 
-        self.step_counter += 1
+        self.current_time += 1
 
         # Things will change in the room!
         self.renew()
 
         observations = self.generate_observations()
         question, self.answer = self.generate_qa()
 
         info = {}
 
-        if self.step_counter >= self.max_step:
+        if self.current_time >= self.max_step:
             done = True
         else:
             done = False
 
         truncated = False
 
         return (observations, question), reward, done, truncated, info
@@ -367,24 +341,22 @@
     def read_names(
         path: str = "./data/top-human-names",
         limit_names: int = None,
         allow_spaces: bool = False,
     ) -> list:
         """Read 20 most common names.
 
-        Args
-        ----
-        path: The path to the top 20 human name list.
-        limit_names: Limit the number of names
-        allow_spaces: Whether to include words that have spaces
-            (e.g., corner of two streets)
-
-        Returns
-        -------
-        names: human names (e.g., James)
+        Args:
+            path: The path to the top 20 human name list.
+            limit_names: Limit the number of names
+            allow_spaces: Whether to include words that have spaces
+                (e.g., corner of two streets)
+
+        Returns:
+            names: human names (e.g., james)
 
         """
         names = read_lines(path)
 
         if not allow_spaces:
             names = [name for name in names if len(name.split("_")) == 1]
 
@@ -400,33 +372,31 @@
     @staticmethod
     def load_semantic_knowledge(
         path: str,
         limit_heads: int = None,
         limit_tails: int = None,
         allow_spaces: bool = False,
         disjoint_entities: bool = True,
-    ) -> Tuple[list, list, list, list]:
+    ) -> tuple[list, list, list, list]:
         """Load saved semantic knowledge.
 
-        Args
-        ----
-        path: the path to the pretrained semantic memory.
-        limit_heads: Limit the number of heads (e.g., 10)
-        limit_tails: Limit the number of tails per heads (e.g., 1)
-        allow_spaces: Whether to include words that have spaces
-            (e.g., corner of two streets)
-        disjoint_entities: Whether to force that there are no common elements between
-            entities.
-
-        Returns
-        -------
-        semantic_knowledge
-        heads
-        relations
-        tails
+        Args:
+            path: the path to the pretrained semantic memory.
+            limit_heads: Limit the number of heads (e.g., 10)
+            limit_tails: Limit the number of tails per heads (e.g., 1)
+            allow_spaces: Whether to include words that have spaces
+                (e.g., corner of two streets)
+            disjoint_entities: Whether to force that there are no common elements between
+                entities.
+
+        Returns:
+            semantic_knowledge
+            heads
+            relations
+            tails
 
         """
         logging.debug(f"loading the semantic knowledge from {path}...")
         semantic_knowledge = read_json(path)
 
         heads = sorted(list(set(semantic_knowledge.keys())))
         if disjoint_entities:
@@ -510,8 +480,13 @@
                         for key_, val_ in val.items()
                     ]
                 )
             )
         )
         logging.info(f"semantic knowledge successfully loaded from {path}!")
 
-        return semantic_knowledge, heads, relations, tails
+        semantic_knowledge_list = []
+        for key, val in semantic_knowledge.items():
+            for k, v in val.items():
+                semantic_knowledge_list.append([key, k, v[0]["tail"]])
+
+        return semantic_knowledge_list, heads, relations, tails
```

### Comparing `room_env-1.0.2/room_env/utils.py` & `room_env-1.0.3/room_env/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 """Utility functions"""
+
 import json
 import logging
 import os
 import random
 import subprocess
 from copy import deepcopy
-from typing import List, Tuple
+from typing import Any
 
 import gymnasium as gym
 import numpy as np
 import torch
 import yaml
 
-import room_env
-
-from .des import RoomDes
-
 logging.basicConfig(
     level=os.environ.get("LOGLEVEL", "INFO").upper(),
     format="%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
+def sample_max_value_key(
+    prob_dict: dict[Any, float], keys_to_exclude: list = None
+) -> Any:
+    """Sample the key with the maximum value.
+
+    Args:
+        prob_dict: dict of probabilities
+        keys_to_exclude: keys to exclude
+
+    """
+    if keys_to_exclude is not None:
+        prob_dict = {k: v for k, v in prob_dict.items() if k not in keys_to_exclude}
+    else:
+        prob_dict = prob_dict
+    max_key = max(prob_dict, key=prob_dict.get)
+
+    return max_key
+
+
 def seed_everything(seed: int) -> None:
     """Seed every randomness to seed"""
     random.seed(seed)
     os.environ["PYTHONHASHSEED"] = str(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
@@ -50,29 +66,55 @@
     with open(fullpath, "r") as stream:
         names = stream.readlines()
     names = [line.strip() for line in names]
 
     return names
 
 
-def read_json(fname: str) -> dict:
+def read_json(fname: str) -> None:
     """Read json"""
     logging.debug(f"reading json {fname} ...")
     with open(fname, "r") as stream:
         return json.load(stream)
 
 
 def write_json(content: dict, fname: str) -> None:
     """Write json"""
     logging.debug(f"writing json {fname} ...")
     with open(fname, "w") as stream:
         json.dump(content, stream, indent=4, sort_keys=False)
 
 
-def read_yaml(fname: str) -> dict:
+def read_json_prod(fname: str) -> None:
+    """Read json.
+
+    There is some path magic going on here. This is to account for both the production
+    and development mode. Don't use this function for a general purpose.
+
+    """
+    fullpath = os.path.join(os.path.dirname(__file__), fname)
+
+    with open(fullpath, "r") as stream:
+        return json.load(stream)
+
+
+def write_json_prod(content: dict, fname: str) -> None:
+    """Write json.
+
+    There is some path magic going on here. This is to account for both the production
+    and development mode. Don't use this function for a general purpose.
+
+    """
+    fullpath = os.path.join(os.path.dirname(__file__), fname)
+
+    with open(fullpath, "w") as stream:
+        json.dump(content, stream, indent=4, sort_keys=False)
+
+
+def read_yaml(fname: str) -> None:
     """Read yaml.
 
     There is some path magic going on here. This is to account for both the production
     and development mode. Don't use this function for a general purpose.
 
     """
     if fname.startswith("/"):
@@ -90,84 +132,77 @@
     with open(fname, "w") as stream:
         yaml.dump(content, stream, indent=2, sort_keys=False)
 
 
 def read_data(data_path: str) -> dict:
     """Read train, val, test spilts.
 
-    Args
-    ----
-    data_path: path to data.
-
-    Returns
-    -------
-    data: {'train': list of training obs,
-           'val': list of val obs,
-           'test': list of test obs}
+    Args:
+        data_path: path to data.
+
+    Returns:
+        data: {'train': list of training obs,
+            'val': list of val obs,
+            'test': list of test obs}
+
     """
     logging.debug(f"reading data from {data_path} ...")
     data = read_json(data_path)
     logging.info(f"Succesfully read data {data_path}")
 
     return data
 
 
-def argmax(iterable):
+def argmax(iterable) -> int:
     """argmax"""
     return max(enumerate(iterable), key=lambda x: x[1])[0]
 
 
-def remove_name(entity: str) -> str:
+def remove_posession(entity: str) -> str:
     """Remove name from the entity.
 
-    Args
-    ----
-    entity: e.g., Bob's laptop
+    Args:
+        entity: e.g., bob's laptop
 
-    Returns
-    -------
-    e.g., laptop
+    Returns:
+        e.g., laptop
 
     """
-    return entity.split()[-1]
+    return entity.split("'s ")[-1]
 
 
-def split_name_entity(name_entity: str) -> Tuple[str, str]:
+def split_by_possessive(name_entity: str) -> tuple[str, str]:
     """Separate name and entity from the given string.
 
-    Args
-    ----
-    name_entity: e.g., "Bob's laptop"
-
-    Returns
-    -------
-    name: e.g., Bob
-    entity: e.g., laptop
+    Args:
+        name_entity: e.g., "tae's laptop"
+
+    Returns:
+        name: e.g., tae
+        entity: e.g., laptop
 
     """
     logging.debug(f"spliting name and entity from {name_entity}")
-    splitted = name_entity.split()
-    assert len(splitted) == 2 and "'" in splitted[0]
-    name = splitted[0].split("'")[0]
-    entity = splitted[1]
+    if "'s " in name_entity:
+        name, entity = name_entity.split("'s ")
+    else:
+        name, entity = None, None
 
     return name, entity
 
 
-def get_duplicate_dicts(search: dict, target: list) -> List:
+def get_duplicate_dicts(search: dict, target: list) -> list:
     """Find if there are duplicate dicts.
 
-    Args
-    ----
-    search: dict
-    target: target list to look up.
-
-    Returns
-    -------
-    duplicates: a list of dicts or None
+    Args:
+        search: dict
+        target: target list to look up.
+
+    Returns:
+        duplicates: a list of dicts or None
 
     """
     assert isinstance(search, dict)
     logging.debug("finding if duplicate dicts exist ...")
     duplicates = []
 
     for candidate in target:
@@ -177,15 +212,15 @@
                 duplicates.append(candidate)
 
     logging.info(f"{len(duplicates)} duplicates were found!")
 
     return duplicates
 
 
-def list_duplicates_of(seq, item) -> List:
+def list_duplicates_of(seq, item) -> list:
     # https://stackoverflow.com/questions/5419204/index-of-duplicates-items-in-a-python-list
     start_at = -1
     locs = []
     while True:
         try:
             loc = seq.index(item, start_at + 1)
         except ValueError:
@@ -204,28 +239,26 @@
     maximum_num_locations_per_object: int,
     maxiumum_days_period: int,
     des_size: str,
     last_timestep: int = 128,
 ) -> dict:
     """Make a des config.
 
-    Args
-    ----
-    commonsense_prob: commonsense probability
-    num_humans: number of humans
-    num_total_objects: number of total objects
-    maximum_num_objects_per_human: maximum number of objects per human
-    maximum_num_locations_per_object: maximum number of locations per object
-    maxiumum_days_period: maxiumum number of days period
-    des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
-    last_timestep: last time step where the DES terminates.
-
-    Returns
-    -------
-    des config
+    Args:
+        commonsense_prob: commonsense probability
+        num_humans: number of humans
+        num_total_objects: number of total objects
+        maximum_num_objects_per_human: maximum number of objects per human
+        maximum_num_locations_per_object: maximum number of locations per object
+        maxiumum_days_period: maxiumum number of days period
+        des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
+        last_timestep: last time step where the DES terminates.
+
+    Returns:
+        des config
 
     """
     des_config = {
         "human_names_path": "./room_env/data/human-names",
         "last_timestep": last_timestep,
         "maxiumum_days_period": maxiumum_days_period,
         "save_path": f"./room_env/data/des-config-{des_size}.json",
@@ -238,24 +271,22 @@
     des_config["num_total_objects"] = num_total_objects
     des_config["maximum_num_objects_per_human"] = maximum_num_objects_per_human
     des_config["maximum_num_locations_per_object"] = maximum_num_locations_per_object
 
     return des_config
 
 
-def get_des_variables(des_size: str = "l") -> Tuple[int, int, int]:
+def get_des_variables(des_size: str = "l") -> tuple[int, int, int]:
     """Get the des variables.
 
-    Args
-    ----
-    des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
-
-    Returns
-    -------
-    capacity, num_humans, num_total_objects
+    Args:
+        des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
+
+    Returns:
+        capacity, num_humans, num_total_objects
 
     """
     if des_size == "dev":
         capacity = 16
 
     elif des_size == "xxs":
         capacity = 2
@@ -287,33 +318,30 @@
     des_size: str = "l",
     allow_random_human: bool = True,
     allow_random_question: bool = True,
     question_prob: float = 0.1,
 ) -> dict:
     """Run the RoomEnv-v1 with multiple different seeds.
 
-    Args
-    ----
-    seeds:
-    capacity:
-    des_size:
-    allow_random_human:
-    allow_random_question:
-    question_prob:
-
-    Returns
-    -------
-    results
+    Args:
+        seeds:
+        capacity:
+        des_size:
+        allow_random_human:
+        allow_random_question:
+        question_prob:
+
+    Returns:
+        results
 
     """
     results = {}
     how_to_forget = ["episodic", "semantic", "random", "pre_sem"]
 
     for forget_short in how_to_forget:
-
         if forget_short == "random":
             pretrain_semantic = False
             capacity_ = {
                 "episodic": capacity // 2,
                 "semantic": capacity // 2,
                 "short": 1,
             }
@@ -332,20 +360,20 @@
             }
         else:
             raise ValueError
 
         results_ = []
         for seed in seeds:
             env = gym.make(
-                "RoomEnv-v1",
+                "room_env:RoomEnv-v1",
                 des_size=des_size,
                 seed=seed,
                 policies={
                     "memory_management": "rl",
-                    "question_answer": "episodic_semantic",
+                    "answer_question": "episodic_semantic",
                     "encoding": "argmax",
                 },
                 capacity=capacity_,
                 question_prob=question_prob,
                 observation_params="perfect",
                 allow_random_human=allow_random_human,
                 allow_random_question=allow_random_question,
@@ -390,33 +418,31 @@
     allow_random_human: bool,
     allow_random_question: bool,
     last_timestep: int,
     question_prob: float,
 ) -> dict:
     """Run the RoomEnv-v1 with different des configs, with multiple different seeds.
 
-    Args
-    ----
-    des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
-    capacity: int,
-    maximum_num_objects_per_human: maximum number of objects per human
-    maximum_num_locations_per_object: maximum number of locations per object
-    maxiumum_days_period: maxiumum number of days period
-    commonsense_prob: commonsense probability
-    num_humans: number of humans
-    num_total_objects: number of total objects
-    seeds: list,
-    allow_random_human: bool,
-    allow_random_question: bool,
-    last_timestep: int,
-    question_prob: float,
+    Args:
+        des_size: The size of DES (i.e., "xxs", "xs", "s", "m", "l", "dev")
+        capacity: int,
+        maximum_num_objects_per_human: maximum number of objects per human
+        maximum_num_locations_per_object: maximum number of locations per object
+        maxiumum_days_period: maxiumum number of days period
+        commonsense_prob: commonsense probability
+        num_humans: number of humans
+        num_total_objects: number of total objects
+        seeds: list,
+        allow_random_human: bool,
+        allow_random_question: bool,
+        last_timestep: int,
+        question_prob: float,
 
-    Returns
-    -------
-    results
+    Returns:
+        results
 
     """
     des_config = make_des_config(
         commonsense_prob=commonsense_prob,
         num_humans=num_humans,
         num_total_objects=num_total_objects,
         maximum_num_objects_per_human=maximum_num_objects_per_human,
@@ -469,106 +495,65 @@
         "num_humans": num_humans,
         "num_total_objects": num_total_objects,
         "maxiumum_days_period": maxiumum_days_period,
         "allow_random_human": allow_random_human,
         "allow_random_question": allow_random_question,
         "question_prob": question_prob,
     }
-    return deepcopy(results)
-
-
-def fill_des_resources(des_size: str) -> None:
-    """Fill resources
-
-    Args
-    ----
-    des_size
-
-    """
-    des = RoomDes(des_size=des_size, check_resources=False)
-    des.run()
-    resources = {
-        foo: 9999
-        for foo in set(
-            [bar["object_location"] for foo in des.states for bar in foo.values()]
-        )
-    }
-    des.config["resources"] = deepcopy(resources)
-    write_json(des.config, f"./room_env/data/des-config-{des_size}.json")
-    resources = []
-    des = RoomDes(des_size=des_size, check_resources=True)
-    resources.append(deepcopy(des.resources))
-    while des.until > 0:
-        des.step()
-        des.until -= 1
-        resources.append(deepcopy(des.resources))
-
-    object_locations = deepcopy(list(des.resources.keys()))
-    resources = {
-        object_location: 9999
-        - min([resource[object_location] for resource in resources])
-        for object_location in object_locations
-    }
-
-    des.config["resources"] = deepcopy(resources)
-    write_json(des.config, f"./room_env/data/des-config-{des_size}.json")
-    des = RoomDes(des_size=des_size, check_resources=True)
+    return results
 
 
 def get_handcrafted(
-    env: str = "RoomEnv-v1",
+    env: str = "room_env:RoomEnv-v1",
     des_size: str = "l",
     seeds: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
     question_prob: float = 0.1,
     observation_params: str = "perfect",
     policies: dict = {
         "memory_management": "rl",
-        "question_answer": "episodic_semantic",
+        "answer_question": "episodic_semantic",
         "encoding": "argmax",
     },
     capacities: list = [2, 4, 8, 16, 32, 64],
     allow_random_human: bool = False,
     allow_random_question: bool = True,
     varying_rewards: bool = False,
     check_resources: bool = True,
 ) -> None:
     """Get the env results with handcrafted policies.
 
     At the moment only {"memory_management": "rl"} is supported.
 
-    Args
-    ----
-    env: str = "RoomEnv-v1",
-    des_size: str = "l",
-    seeds: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
-    question_prob: float = 0.1,
-    policies: dict = {
-        "memory_management": "rl",
-        "question_answer": "episodic_semantic",
-        "encoding": "argmax",
-    },
-    capacities: list = [2, 4, 8, 16, 32, 64],
-    allow_random_human: whether to allow random humans to be observed.
-    allow_random_question: whether to allow random questions to be asked.
-    varying_rewards: If true, then the rewards are scaled in every episode so that
-            total_episode_rewards is 128.
-
-    Returns
-    -------
-    handcrafted_results
+    Args:
+        env: str = "RoomEnv-v1",
+        des_size: str = "l",
+        seeds: list = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+        question_prob: float = 0.1,
+        policies: dict = {
+            "memory_management": "rl",
+            "answer_question": "episodic_semantic",
+            "encoding": "argmax",
+        },
+        capacities: list = [2, 4, 8, 16, 32, 64],
+        allow_random_human: whether to allow random humans to be observed.
+        allow_random_question: whether to allow random questions to be asked.
+        varying_rewards: If true, then the rewards are scaled in every episode so that
+                total_maximum_episode_rewards is 128.
+
+    Returns:
+        handcrafted_results
 
     """
     how_to_forget = ["episodic", "semantic", "random", "pre_sem"]
     env_ = env
     handcrafted_results = {}
 
     for capacity in capacities:
         handcrafted_results[capacity] = {}
         for forget_short in how_to_forget:
-
             if forget_short == "random":
                 pretrain_semantic = False
                 capacity_ = {
                     "episodic": capacity // 2,
                     "semantic": capacity // 2,
                     "short": 1,
                 }
@@ -624,7 +609,55 @@
                 results.append(rewards)
 
             mean_ = np.mean(results).round(3).item()
             std_ = np.std(results).round(3).item()
             handcrafted_results[capacity][forget_short] = {"mean": mean_, "std": std_}
 
     return handcrafted_results
+
+
+def find_connected_nodes(graph_):
+    graph = deepcopy(graph_)
+
+    def dfs(node, row, col):
+        if (
+            row < 0
+            or col < 0
+            or row >= len(graph)
+            or col >= len(graph[0])
+            or graph[row][col] == 0
+        ):
+            return
+
+        connected_nodes.append((row, col))
+        graph[row][col] = 0  # Mark the node as visited
+
+        # Check the neighbors
+        dfs(node, row - 1, col)  # Up
+        dfs(node, row + 1, col)  # Down
+        dfs(node, row, col - 1)  # Left
+        dfs(node, row, col + 1)  # Right
+
+    connected_components = []
+    for row in range(len(graph)):
+        for col in range(len(graph[row])):
+            if graph[row][col] == 1:
+                connected_nodes = []
+                dfs(1, row, col)
+                if connected_nodes:
+                    connected_components.append(connected_nodes)
+
+    return connected_components
+
+
+def is_running_notebook() -> bool:
+    """See if the code is running in a notebook or not."""
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == "ZMQInteractiveShell":
+            return True  # Jupyter notebook or qtconsole
+        elif shell == "TerminalInteractiveShell":
+            return False  # Terminal running IPython
+        else:
+            return False  # Other type (?)
+    except NameError:
+        return False  # Probably standard Python interpreter
```

### Comparing `room_env-1.0.2/room_env.egg-info/SOURCES.txt` & `room_env-1.0.3/room_env.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 room_env/__init__.py
+room_env/create_room2.py
 room_env/des.py
-room_env/memory.py
-room_env/policy.py
 room_env/utils.py
 room_env.egg-info/PKG-INFO
 room_env.egg-info/SOURCES.txt
 room_env.egg-info/dependency_links.txt
 room_env.egg-info/requires.txt
 room_env.egg-info/top_level.txt
 room_env/data/conceptnet-data.json
@@ -17,20 +16,28 @@
 room_env/data/des-config-m-v1.json
 room_env/data/des-config-s-v1.json
 room_env/data/des-config-xs-v1.json
 room_env/data/des-config-xxs-v1.json
 room_env/data/human-locations
 room_env/data/human-names
 room_env/data/ms-coco-80-categories
+room_env/data/names-v2.json
+room_env/data/room-config-dev-v2.json
+room_env/data/room-config-foo-v2.json
+room_env/data/room-config-l-v2.json
+room_env/data/room-config-l2-v2.json
+room_env/data/room-config-m-v2.json
+room_env/data/room-config-s-v2.json
+room_env/data/room-config-xl-v2.json
+room_env/data/room-config-xs-v2.json
+room_env/data/room-config-xxl-v2.json
+room_env/data/room-config-xxs-v2.json
 room_env/data/semantic-knowledge-small.json
 room_env/data/semantic-knowledge.json
 room_env/data/top-human-names
 room_env/data/top-human-names-small
 room_env/envs/__init__.py
 room_env/envs/room0.py
 room_env/envs/room1.py
+room_env/envs/room2.py
 test/test_des.py
-test/test_memory.py
-test/test_policy.py
-test/test_room_env_v0.py
-test/test_room_env_v1.py
 test/test_utils.py
```

### Comparing `room_env-1.0.2/test/test_utils.py` & `room_env-1.0.3/test/test_utils.py`

 * *Files identical despite different names*

