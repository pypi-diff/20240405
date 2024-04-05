# Comparing `tmp/math-spec-mapping-0.2.8.tar.gz` & `tmp/math-spec-mapping-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math-spec-mapping-0.2.8.tar", last modified: Sun Mar 31 21:57:24 2024, max compression
+gzip compressed data, was "math-spec-mapping-0.3.0.tar", last modified: Fri Apr  5 19:01:33 2024, max compression
```

## Comparing `math-spec-mapping-0.2.8.tar` & `math-spec-mapping-0.3.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.932754 math-spec-mapping-0.2.8/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math-spec-mapping-0.2.8/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-03-31 21:57:24.932453 math-spec-mapping-0.2.8/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-03-28 13:52:56.000000 math-spec-mapping-0.2.8/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-03-31 21:57:24.932805 math-spec-mapping-0.2.8/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.920824 math-spec-mapping-0.2.8/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.922106 math-spec-mapping-0.2.8/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.925723 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    22244 2024-03-31 19:34:38.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1497 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-28 19:23:03.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.926166 math-spec-mapping-0.2.8/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       60 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1607 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)        0 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.929560 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3273 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1334 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1223 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4217 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.931919 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     8882 2024-03-28 12:55:01.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    21113 2024-03-31 19:36:07.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2203 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      907 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    29208 2024-03-28 16:18:11.000000 math-spec-mapping-0.2.8/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-03-31 21:57:24.932172 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-03-31 21:57:24.000000 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-03-31 21:57:24.000000 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-03-31 21:57:24.000000 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-03-31 21:57:24.000000 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-03-31 21:57:24.000000 math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710893 math-spec-mapping-0.3.0/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math-spec-mapping-0.3.0/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-05 19:01:33.710661 math-spec-mapping-0.3.0/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-03-31 22:10:56.000000 math-spec-mapping-0.3.0/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-04-05 19:01:33.710941 math-spec-mapping-0.3.0/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.699591 math-spec-mapping-0.3.0/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.701063 math-spec-mapping-0.3.0/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.704423 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    27443 2024-04-05 17:59:27.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1497 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.704861 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       60 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1607 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        0 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.708056 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3273 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1334 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1223 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4217 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710188 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     8882 2024-03-28 12:55:01.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    21113 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2203 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      907 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    29208 2024-03-31 21:59:52.000000 math-spec-mapping-0.3.0/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-04-05 19:01:33.710429 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-04-05 19:01:33.000000 math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math-spec-mapping-0.2.8/LICENSE` & `math-spec-mapping-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/PKG-INFO` & `math-spec-mapping-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.2.8
+Version: 0.3.0
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math-spec-mapping-0.2.8/README.md` & `math-spec-mapping-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/pyproject.toml` & `math-spec-mapping-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.2.8"
+version = "0.3.0"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Block.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Block.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/ControlAction.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Entity.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/MathSpec.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files 18% similar despite different names*

```diff
@@ -352,32 +352,39 @@
     def get_all_stateful_metric_names(self):
         sm = []
         for metrics in self.stateful_metrics.values():
             sm.extend([x.name for x in metrics.metrics])
         return sm
 
     def _build_functional_parameters(self):
-        opts = [x for x in self.policies.values() if len(x.policy_options) > 1]
+        opts = [
+            (x, x.policy_options)
+            for x in self.policies.values()
+            if len(x.policy_options) > 1
+        ]
         opts.extend(
             [
-                x
+                (x, x.boundary_actions)
                 for x in self.boundary_actions.values()
                 if len(x.boundary_action_options) > 1
             ]
         )
         opts.extend(
             [
-                x
+                (x, x.control_actions)
                 for x in self.control_actions.values()
                 if len(x.control_action_options) > 1
             ]
         )
         self.functional_parameters = {}
         for x in opts:
-            self.functional_parameters["FP {}".format(x.name)] = x
+            x, y = x
+            self.functional_parameters["FP {}".format(x.name)] = {}
+            for y1 in y:
+                self.functional_parameters["FP {}".format(x.name)][y1.name] = y1
 
     def _build_parameter_types(self):
         system_parameters_types = {}
         behavioral_parameters_types = {}
         functional_parameters_types = {}
 
         for x in self.parameters.all_parameters:
@@ -592,11 +599,149 @@
         out += "\n\n"
 
         out += "parameters: Parameters = {**behavioral_parameters, **functional_parameters, **system_parameters}"
 
         with open(path, "w") as f:
             f.write(out)
 
+    def build_implementation(self, params):
+        return MathSpecImplementation(self, params)
+
 
 class MathSpecImplementation:
     def __init__(self, ms: MathSpec, params):
         self.ms = deepcopy(ms)
+        self.params = params
+        self.control_actions = self.load_control_actions()
+        self.boundary_actions = {}
+        self.policies = self.load_policies()
+        self.mechanisms = self.load_mechanisms()
+        self.load_wiring()
+
+    def load_control_actions(self):
+        control_actions = {}
+        for ca in self.ms.control_actions:
+            ca = self.ms.control_actions[ca]
+            opts = ca.control_action_options
+            if len(opts) == 0:
+                print("{} has no control action options".format(ca.name))
+            else:
+                if len(opts) == 1:
+                    opt = opts[0]
+                else:
+                    assert (
+                        "FP {}".format(ca.name) in self.params
+                    ), "No functional parameterization for {}".format(ca.name)
+                    opt = self.ms.functional_parameters["FP {}".format(ca.name)][
+                        self.params["FP {}".format(ca.name)]
+                    ]
+
+                assert (
+                    "python" in opt.implementations
+                ), "No python implementation for {} / {}".format(ca.name, opt.name)
+
+                control_actions[ca.name] = opt.implementations["python"]
+        return control_actions
+
+    def load_mechanisms(self):
+        mechanisms = {}
+        for m in self.ms.mechanisms:
+            m = self.ms.mechanisms[m]
+            if "python" not in m.implementations:
+                print("No python implementation for {}".format(m.name))
+            else:
+                mechanisms[m.name] = m.implementations["python"]
+        return mechanisms
+
+    def load_single_wiring(self, wiring):
+        components = [x.name for x in wiring.components]
+        if wiring.block_type == "Stack Block":
+
+            def wiring(state, params, spaces):
+                for component in components:
+                    spaces = self.blocks[component](state, params, spaces)
+                return spaces
+
+        elif wiring.block_type == "Parallel Block":
+
+            spaces_mapping = {}
+            for x in wiring.components:
+                spaces_mapping[x.name] = []
+
+            for i, x in enumerate([x.name for x in wiring.domain_blocks]):
+                spaces_mapping[x].append(i)
+
+            def wiring(state, params, spaces):
+                codomain = []
+                for component in components:
+                    spaces_i = [spaces[i] for i in spaces_mapping[component]]
+                    spaces_i = self.blocks[component](state, params, spaces_i)
+                    if spaces_i:
+                        codomain.extend(spaces_i)
+                return codomain
+
+        else:
+            assert False
+
+        return wiring
+
+    def load_policies(self):
+        policies = {}
+        for p in self.ms.policies:
+            p = self.ms.policies[p]
+            opts = p.policy_options
+            if len(opts) == 0:
+                print("{} has no policy options".format(p.name))
+            else:
+                if len(opts) == 1:
+                    opt = opts[0]
+                else:
+                    assert (
+                        "FP {}".format(p.name) in self.params
+                    ), "No functional parameterization for {}".format(p.name)
+                    opt = self.ms.functional_parameters["FP {}".format(p.name)][
+                        self.params["FP {}".format(p.name)]
+                    ]
+
+                if "python" not in opt.implementations:
+                    print(
+                        "No python implementation for {} / {}".format(p.name, opt.name)
+                    )
+                else:
+                    policies[p.name] = opt.implementations["python"]
+        return policies
+
+    def load_wiring(
+        self,
+    ):
+        self.blocks = {}
+        self.blocks.update(self.boundary_actions)
+        self.blocks.update(self.control_actions)
+        self.blocks.update(self.policies)
+        self.blocks.update(self.mechanisms)
+
+        self.wiring = {}
+
+        wiring = [x for x in self.ms.wiring.values()]
+
+        i = 1
+        while i > 0:
+            i = 0
+            hold = []
+            for w in wiring:
+                components = [x.name for x in w.components]
+                if all([x in self.blocks for x in components]):
+                    i += 1
+                    w2 = self.load_single_wiring(w)
+                    assert w.name not in self.blocks, "{} was a repeated block".format(
+                        w.name
+                    )
+                    if w2:
+                        self.blocks[w.name] = w2
+                        self.wiring[w.name] = w2
+
+                else:
+                    hold.append(w)
+            wiring = hold
+        if len(wiring) > 0:
+            wiring = [x.name for x in wiring]
+            print("The following wirings were not loading: {}".format(wiring))
```

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Metric.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Parameter.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/Policy.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/State.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/State.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/StatefulMetric.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Classes/__init__.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Convenience/documentation.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Convenience/documentation.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/action_transmission_channel.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/boundary_actions.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/control_actions.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/entities.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/entities.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/general.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/load.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/mechanism.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/metrics.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/metrics.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/parameters.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/parameters.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/policy.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/spaces.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/stateful_metrics.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/states.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/states.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/type.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/type.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Load/wiring.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/__init__.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/boundary_actions.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/control_actions.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/general.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/html.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/html.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/markdown.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/markdown.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/mechanisms.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/node_map.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/parameters.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/policies.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/spaces.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/state.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/state.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/tables.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/Reports/wiring.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/__init__.py` & `math-spec-mapping-0.3.0/src/math_spec_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping/schema.schema.json` & `math-spec-mapping-0.3.0/src/math_spec_mapping/schema.schema.json`

 * *Files identical despite different names*

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/PKG-INFO` & `math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.2.8
+Version: 0.3.0
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math-spec-mapping-0.2.8/src/math_spec_mapping.egg-info/SOURCES.txt` & `math-spec-mapping-0.3.0/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

