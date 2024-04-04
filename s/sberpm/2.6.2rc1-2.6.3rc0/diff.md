# Comparing `tmp/sberpm-2.6.2rc1.tar.gz` & `tmp/sberpm-2.6.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sberpm-2.6.2rc1.tar", last modified: Thu Nov  9 23:09:11 2023, max compression
+gzip compressed data, was "sberpm-2.6.3rc0.tar", last modified: Thu Apr  4 21:33:48 2024, max compression
```

## Comparing `sberpm-2.6.2rc1.tar` & `sberpm-2.6.3rc0.tar`

### file list

```diff
@@ -1,120 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.164161 sberpm-2.6.2rc1/
--rw-rw-rw-   0        0        0      274 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/.gitignore
--rw-rw-rw-   0        0        0    29507 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/LICENSE
--rw-rw-rw-   0        0        0    62148 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/LICENSE_RUS
--rw-rw-rw-   0        0        0      273 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/MANIFEST.in
--rw-rw-rw-   0        0        0     3784 2023-11-09 23:09:11.163196 sberpm-2.6.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0     2213 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/README.md
--rw-rw-rw-   0        0        0      610 2023-11-09 22:40:13.000000 sberpm-2.6.2rc1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.762098 sberpm-2.6.2rc1/sberpm/
--rw-rw-rw-   0        0        0      542 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/__init__.py
--rw-rw-rw-   0        0        0    31800 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/_holder.py
--rw-rw-rw-   0        0        0      947 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/_utils.py
--rw-rw-rw-   0        0        0       26 2023-11-09 23:08:09.000000 sberpm-2.6.2rc1/sberpm/_version.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.803988 sberpm-2.6.2rc1/sberpm/autoinsights/
--rw-rw-rw-   0        0        0      120 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/autoinsights/__init__.py
--rw-rw-rw-   0        0        0    22755 2023-11-09 20:11:15.000000 sberpm-2.6.2rc1/sberpm/autoinsights/_influencing_activities.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.811745 sberpm-2.6.2rc1/sberpm/bpmn/
--rw-rw-rw-   0        0        0      177 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/__init__.py
--rw-rw-rw-   0        0        0    26484 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_file_to_graph.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.868080 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/
--rw-rw-rw-   0        0        0      103 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
--rw-rw-rw-   0        0        0     4093 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
--rw-rw-rw-   0        0        0     6642 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
--rw-rw-rw-   0        0        0     4680 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
--rw-rw-rw-   0        0        0     1545 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
--rw-rw-rw-   0        0        0     5350 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.875081 sberpm-2.6.2rc1/sberpm/column_matching/
--rw-rw-rw-   0        0        0      102 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/column_matching/__init__.py
--rw-rw-rw-   0        0        0      182 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/column_matching/_column_matching.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.879104 sberpm-2.6.2rc1/sberpm/column_matching/file_obf/
--rw-rw-rw-   0        0        0     5849 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/column_matching/file_obf/_column_matching_.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.888083 sberpm-2.6.2rc1/sberpm/conformance_checking/
--rw-rw-rw-   0        0        0      202 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/conformance_checking/__init__.py
--rw-rw-rw-   0        0        0     6061 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/conformance_checking/_conformance_checking.py
--rw-rw-rw-   0        0        0     9883 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/conformance_checking/_token_replay.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.897082 sberpm-2.6.2rc1/sberpm/decision_mining/
--rw-rw-rw-   0        0        0      100 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    33758 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/decision_mining/_decision_mining.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.907095 sberpm-2.6.2rc1/sberpm/graph_stats/
--rw-rw-rw-   0        0        0      146 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/graph_stats/__init__.py
--rw-rw-rw-   0        0        0     3336 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/graph_stats/centrality.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.913101 sberpm-2.6.2rc1/sberpm/imitation/
--rw-rw-rw-   0        0        0       78 2023-08-31 17:57:22.000000 sberpm-2.6.2rc1/sberpm/imitation/__init__.py
--rw-rw-rw-   0        0        0      177 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/imitation/_simulation.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.922669 sberpm-2.6.2rc1/sberpm/imitation/file_obf/
--rw-rw-rw-   0        0        0    21989 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/imitation/file_obf/_simulation_.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.958088 sberpm-2.6.2rc1/sberpm/metrics/
--rw-rw-rw-   0        0        0      371 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/__init__.py
--rw-rw-rw-   0        0        0     5524 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_activity_metric.py
--rw-rw-rw-   0        0        0     6918 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_base_metric.py
--rw-rw-rw-   0        0        0     4077 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_id_metric.py
--rw-rw-rw-   0        0        0     5173 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_trace_metric.py
--rw-rw-rw-   0        0        0     6093 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_transition_metric.py
--rw-rw-rw-   0        0        0     3995 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_user_metric.py
--rw-rw-rw-   0        0        0      389 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/metrics/_utils.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.015238 sberpm-2.6.2rc1/sberpm/miners/
--rw-rw-rw-   0        0        0     1374 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/__init__.py
--rw-rw-rw-   0        0        0     9571 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_abstract_miner.py
--rw-rw-rw-   0        0        0    19774 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_alpha_miner.py
--rw-rw-rw-   0        0        0    10578 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_alpha_plus_miner.py
--rw-rw-rw-   0        0        0      177 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/_auto_miner.py
--rw-rw-rw-   0        0        0     3153 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_causal_miner.py
--rw-rw-rw-   0        0        0    18462 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_correlation_miner.py
--rw-rw-rw-   0        0        0     9122 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_heu_miner.py
--rw-rw-rw-   0        0        0     3896 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_inductive_miner.py
--rw-rw-rw-   0        0        0     8354 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_inductive_utils.py
--rw-rw-rw-   0        0        0      175 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/_ml_miner.py
--rw-rw-rw-   0        0        0      181 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/_parallel_miner.py
--rw-rw-rw-   0        0        0     2678 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/_simple_miner.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.030239 sberpm-2.6.2rc1/sberpm/miners/file_obf/
--rw-rw-rw-   0        0        0     3296 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/file_obf/_auto_miner_.obfsbpm
--rw-rw-rw-   0        0        0     5140 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/file_obf/_ml_miner_.obfsbpm
--rw-rw-rw-   0        0        0     6021 2023-11-09 22:54:01.000000 sberpm-2.6.2rc1/sberpm/miners/file_obf/_parallel_miner_.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.042277 sberpm-2.6.2rc1/sberpm/miners/mining_utils/
--rw-rw-rw-   0        0        0       62 2023-08-31 17:57:22.000000 sberpm-2.6.2rc1/sberpm/miners/mining_utils/__init__.py
--rw-rw-rw-   0        0        0     8347 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/mining_utils/_inductive_utils.py
--rw-rw-rw-   0        0        0    25893 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/miners/mining_utils/_node_utils.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.046240 sberpm-2.6.2rc1/sberpm/ml/
--rw-rw-rw-   0        0        0      114 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.077220 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/
--rw-rw-rw-   0        0        0      571 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0    11459 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlier_detector.py
--rw-rw-rw-   0        0        0     4669 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
--rw-rw-rw-   0        0        0     5295 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outliercblof.py
--rw-rw-rw-   0        0        0     2404 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outliercustom.py
--rw-rw-rw-   0        0        0     4911 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierforest.py
--rw-rw-rw-   0        0        0     6340 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierlof.py
--rw-rw-rw-   0        0        0     4804 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierocsvm.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.084196 sberpm-2.6.2rc1/sberpm/ml/chronometrage/
--rw-rw-rw-   0        0        0       76 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/chronometrage/__init__.py
--rw-rw-rw-   0        0        0     6531 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/chronometrage/_chronometrage.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.092197 sberpm-2.6.2rc1/sberpm/ml/utils/
--rw-rw-rw-   0        0        0      107 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/utils/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/ml/utils/_perm_importance.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.100198 sberpm-2.6.2rc1/sberpm/models/
--rw-rw-rw-   0        0        0      300 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/models/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/models/_check_models.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.129200 sberpm-2.6.2rc1/sberpm/visual/
--rw-rw-rw-   0        0        0      608 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/visual/__init__.py
--rw-rw-rw-   0        0        0    79418 2023-11-09 21:59:51.000000 sberpm-2.6.2rc1/sberpm/visual/_chart_painter.py
--rw-rw-rw-   0        0        0    18529 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/visual/_graph.py
--rw-rw-rw-   0        0        0    12329 2023-11-09 20:47:15.000000 sberpm-2.6.2rc1/sberpm/visual/_graphviz_painter.py
--rw-rw-rw-   0        0        0    25598 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/visual/_matplotlib_painter.py
--rw-rw-rw-   0        0        0      594 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/visual/_types.py
--rw-rw-rw-   0        0        0     6935 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/sberpm/visual/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:10.796996 sberpm-2.6.2rc1/sberpm.egg-info/
--rw-rw-rw-   0        0        0     3784 2023-11-09 23:09:09.000000 sberpm-2.6.2rc1/sberpm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3106 2023-11-09 23:09:10.000000 sberpm-2.6.2rc1/sberpm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 23:09:09.000000 sberpm-2.6.2rc1/sberpm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      446 2023-11-09 23:09:09.000000 sberpm-2.6.2rc1/sberpm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-09 23:09:09.000000 sberpm-2.6.2rc1/sberpm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-09 23:09:11.179665 sberpm-2.6.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     2606 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.151166 sberpm-2.6.2rc1/tutorials/
--rw-rw-rw-   0        0        0    19319 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/tutorials/chrono_data.xlsx
--rw-rw-rw-   0        0        0   132942 2023-11-09 22:01:42.000000 sberpm-2.6.2rc1/tutorials/example.xlsx
-drwxrwxrwx   0        0        0        0 2023-11-09 23:09:11.155143 sberpm-2.6.2rc1/tutorials/poster_PM/
--rw-rw-rw-   0        0        0    48006 2023-11-09 18:02:34.000000 sberpm-2.6.2rc1/tutorials/poster_PM/poster.png
--rw-rw-rw-   0        0        0    93609 2023-11-09 23:05:24.000000 sberpm-2.6.2rc1/tutorials/tutorial_en.ipynb
--rw-rw-rw-   0        0        0   126171 2023-11-09 23:04:23.000000 sberpm-2.6.2rc1/tutorials/tutorial_ru.ipynb
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.973203 sberpm-2.6.3rc0/
+-rw-rw-rw-   0        0        0      274 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/.gitignore
+-rw-rw-rw-   0        0        0    29507 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/LICENSE
+-rw-rw-rw-   0        0        0    62148 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/LICENSE_RUS
+-rw-rw-rw-   0        0        0      261 2024-04-04 19:49:56.000000 sberpm-2.6.3rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3654 2024-04-04 21:33:48.972237 sberpm-2.6.3rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     2240 2024-04-04 19:56:36.000000 sberpm-2.6.3rc0/README.md
+-rw-rw-rw-   0        0        0      610 2023-11-09 22:40:13.000000 sberpm-2.6.3rc0/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.748196 sberpm-2.6.3rc0/sberpm/
+-rw-rw-rw-   0        0        0      504 2024-04-04 21:17:27.000000 sberpm-2.6.3rc0/sberpm/__init__.py
+-rw-rw-rw-   0        0        0    31800 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/_holder.py
+-rw-rw-rw-   0        0        0      947 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/_utils.py
+-rw-rw-rw-   0        0        0       26 2024-04-04 20:04:32.000000 sberpm-2.6.3rc0/sberpm/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.775189 sberpm-2.6.3rc0/sberpm/bpmn/
+-rw-rw-rw-   0        0        0      177 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/__init__.py
+-rw-rw-rw-   0        0        0    26484 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_file_to_graph.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.794191 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/
+-rw-rw-rw-   0        0        0      103 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
+-rw-rw-rw-   0        0        0     4093 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
+-rw-rw-rw-   0        0        0     6642 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
+-rw-rw-rw-   0        0        0     4680 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
+-rw-rw-rw-   0        0        0     1545 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
+-rw-rw-rw-   0        0        0     5350 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.803192 sberpm-2.6.3rc0/sberpm/conformance_checking/
+-rw-rw-rw-   0        0        0      202 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/conformance_checking/__init__.py
+-rw-rw-rw-   0        0        0     6061 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/conformance_checking/_conformance_checking.py
+-rw-rw-rw-   0        0        0     9883 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/conformance_checking/_token_replay.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.807211 sberpm-2.6.3rc0/sberpm/decision_mining/
+-rw-rw-rw-   0        0        0      100 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    33758 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/decision_mining/_decision_mining.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.813192 sberpm-2.6.3rc0/sberpm/graph_stats/
+-rw-rw-rw-   0        0        0      146 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/graph_stats/__init__.py
+-rw-rw-rw-   0        0        0     3336 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/graph_stats/centrality.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.818211 sberpm-2.6.3rc0/sberpm/imitation/
+-rw-rw-rw-   0        0        0       78 2023-08-31 17:57:22.000000 sberpm-2.6.3rc0/sberpm/imitation/__init__.py
+-rw-rw-rw-   0        0        0    28528 2024-04-04 21:27:23.000000 sberpm-2.6.3rc0/sberpm/imitation/_simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.839216 sberpm-2.6.3rc0/sberpm/metrics/
+-rw-rw-rw-   0        0        0      371 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5524 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_activity_metric.py
+-rw-rw-rw-   0        0        0     6918 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_base_metric.py
+-rw-rw-rw-   0        0        0     4077 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_id_metric.py
+-rw-rw-rw-   0        0        0     5173 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_trace_metric.py
+-rw-rw-rw-   0        0        0     6093 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_transition_metric.py
+-rw-rw-rw-   0        0        0     3995 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_user_metric.py
+-rw-rw-rw-   0        0        0      389 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/metrics/_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.884216 sberpm-2.6.3rc0/sberpm/miners/
+-rw-rw-rw-   0        0        0     1152 2024-04-04 19:52:28.000000 sberpm-2.6.3rc0/sberpm/miners/__init__.py
+-rw-rw-rw-   0        0        0     9571 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_abstract_miner.py
+-rw-rw-rw-   0        0        0    19774 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_alpha_miner.py
+-rw-rw-rw-   0        0        0    10578 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_alpha_plus_miner.py
+-rw-rw-rw-   0        0        0     3153 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_causal_miner.py
+-rw-rw-rw-   0        0        0    18462 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_correlation_miner.py
+-rw-rw-rw-   0        0        0     9122 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_heu_miner.py
+-rw-rw-rw-   0        0        0     3896 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_inductive_miner.py
+-rw-rw-rw-   0        0        0     8354 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_inductive_utils.py
+-rw-rw-rw-   0        0        0     2678 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/_simple_miner.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.894198 sberpm-2.6.3rc0/sberpm/miners/mining_utils/
+-rw-rw-rw-   0        0        0       62 2023-08-31 17:57:22.000000 sberpm-2.6.3rc0/sberpm/miners/mining_utils/__init__.py
+-rw-rw-rw-   0        0        0     8347 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/mining_utils/_inductive_utils.py
+-rw-rw-rw-   0        0        0    25893 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/miners/mining_utils/_node_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.896215 sberpm-2.6.3rc0/sberpm/ml/
+-rw-rw-rw-   0        0        0      114 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.919210 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/
+-rw-rw-rw-   0        0        0      571 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0    11459 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlier_detector.py
+-rw-rw-rw-   0        0        0     4669 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
+-rw-rw-rw-   0        0        0     5295 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outliercblof.py
+-rw-rw-rw-   0        0        0     2404 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outliercustom.py
+-rw-rw-rw-   0        0        0     4911 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierforest.py
+-rw-rw-rw-   0        0        0     6340 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierlof.py
+-rw-rw-rw-   0        0        0     4804 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierocsvm.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.924217 sberpm-2.6.3rc0/sberpm/ml/chronometrage/
+-rw-rw-rw-   0        0        0       76 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/chronometrage/__init__.py
+-rw-rw-rw-   0        0        0     6531 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/chronometrage/_chronometrage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.929223 sberpm-2.6.3rc0/sberpm/ml/utils/
+-rw-rw-rw-   0        0        0      107 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/utils/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/ml/utils/_perm_importance.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.935200 sberpm-2.6.3rc0/sberpm/models/
+-rw-rw-rw-   0        0        0      300 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/models/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/models/_check_models.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.955203 sberpm-2.6.3rc0/sberpm/visual/
+-rw-rw-rw-   0        0        0      608 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/visual/__init__.py
+-rw-rw-rw-   0        0        0    79418 2023-11-09 21:59:51.000000 sberpm-2.6.3rc0/sberpm/visual/_chart_painter.py
+-rw-rw-rw-   0        0        0    18529 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/visual/_graph.py
+-rw-rw-rw-   0        0        0    12329 2023-11-09 20:47:15.000000 sberpm-2.6.3rc0/sberpm/visual/_graphviz_painter.py
+-rw-rw-rw-   0        0        0    25598 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/visual/_matplotlib_painter.py
+-rw-rw-rw-   0        0        0      594 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/visual/_types.py
+-rw-rw-rw-   0        0        0     6935 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/sberpm/visual/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.770213 sberpm-2.6.3rc0/sberpm.egg-info/
+-rw-rw-rw-   0        0        0     3654 2024-04-04 21:33:48.000000 sberpm-2.6.3rc0/sberpm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2024-04-04 21:33:48.000000 sberpm-2.6.3rc0/sberpm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 21:33:48.000000 sberpm-2.6.3rc0/sberpm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      446 2024-04-04 21:33:48.000000 sberpm-2.6.3rc0/sberpm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 21:33:48.000000 sberpm-2.6.3rc0/sberpm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 21:33:48.984241 sberpm-2.6.3rc0/setup.cfg
+-rw-rw-rw-   0        0        0     2494 2024-04-04 19:56:49.000000 sberpm-2.6.3rc0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.966205 sberpm-2.6.3rc0/tutorials/
+-rw-rw-rw-   0        0        0    19319 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/tutorials/chrono_data.xlsx
+-rw-rw-rw-   0        0        0   132942 2023-11-09 22:01:42.000000 sberpm-2.6.3rc0/tutorials/example.xlsx
+drwxrwxrwx   0        0        0        0 2024-04-04 21:33:48.969225 sberpm-2.6.3rc0/tutorials/poster_PM/
+-rw-rw-rw-   0        0        0    48006 2023-11-09 18:02:34.000000 sberpm-2.6.3rc0/tutorials/poster_PM/poster.png
+-rw-rw-rw-   0        0        0    89606 2024-04-04 20:38:37.000000 sberpm-2.6.3rc0/tutorials/tutorial_en.ipynb
+-rw-rw-rw-   0        0        0   120789 2024-04-04 20:16:02.000000 sberpm-2.6.3rc0/tutorials/tutorial_ru.ipynb
```

### Comparing `sberpm-2.6.2rc1/LICENSE` & `sberpm-2.6.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/LICENSE_RUS` & `sberpm-2.6.3rc0/LICENSE_RUS`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/PKG-INFO` & `sberpm-2.6.3rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: sberpm
-Version: 2.6.2rc1
+Version: 2.6.3rc0
 Summary: Library that is intended to operate with various process mining tasks.
-Author: Sberbank Process Mining Team
-Author-email: AABugaenko@sberbank.ru
+Author: Sber Process Mining Team
+Author-email: SberPM_lib@sberbank.ru
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_RUS
 Requires-Dist: dataclassy==1.*
 Requires-Dist: dataenforce==0.1.2
@@ -65,9 +62,9 @@
 Additionally, you might need to install graphviz executables and add the path to the executables to PATH variable: https://graphviz.org/download/
 
 # Examples
 To find out how to work with SberPM, see [tutorials](https://pypi.org/project/sberpm/#files) in files tar.gz.
 
 # Contacts
 If you have any questions or suggestions, feel free to contact us!
-- Andrey Bugaenko (aabugaenko@sberbank.ru)
+- Библиотека Sber Process Mining ("SberPM_lib@sberbank.ru")
```

### Comparing `sberpm-2.6.2rc1/README.md` & `sberpm-2.6.3rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 Additionally, you might need to install graphviz executables and add the path to the executables to PATH variable: https://graphviz.org/download/
 
 # Examples
 To find out how to work with SberPM, see [tutorials](https://pypi.org/project/sberpm/#files) in files tar.gz.
 
 # Contacts
 If you have any questions or suggestions, feel free to contact us!
-- Andrey Bugaenko (aabugaenko@sberbank.ru)
+- Библиотека Sber Process Mining ("SberPM_lib@sberbank.ru")
```

### Comparing `sberpm-2.6.2rc1/requirements.txt` & `sberpm-2.6.3rc0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/_holder.py` & `sberpm-2.6.3rc0/sberpm/_holder.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/_utils.py` & `sberpm-2.6.3rc0/sberpm/_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_file_to_graph.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_file_to_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py` & `sberpm-2.6.3rc0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/conformance_checking/_conformance_checking.py` & `sberpm-2.6.3rc0/sberpm/conformance_checking/_conformance_checking.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/conformance_checking/_token_replay.py` & `sberpm-2.6.3rc0/sberpm/conformance_checking/_token_replay.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/decision_mining/_decision_mining.py` & `sberpm-2.6.3rc0/sberpm/decision_mining/_decision_mining.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/graph_stats/centrality.py` & `sberpm-2.6.3rc0/sberpm/graph_stats/centrality.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_activity_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_activity_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_base_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_base_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_id_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_id_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_trace_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_trace_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_transition_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_transition_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/metrics/_user_metric.py` & `sberpm-2.6.3rc0/sberpm/metrics/_user_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/__init__.py` & `sberpm-2.6.3rc0/sberpm/miners/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 from sberpm.miners._abstract_miner import AbstractMiner
 from sberpm.miners._alpha_miner import AlphaMiner, alpha_miner
 from sberpm.miners._alpha_plus_miner import AlphaPlusMiner, alpha_plus_miner
-from sberpm.miners._auto_miner import AutoMiner, auto_miner
 from sberpm.miners._causal_miner import CausalMiner, causal_miner
 from sberpm.miners._correlation_miner import CorrelationMiner, correlation_miner
 from sberpm.miners._heu_miner import HeuMiner, heu_miner
-from sberpm.miners._simple_miner import SimpleMiner, simple_miner  # do not move cause InductiveMiner depends
+from sberpm.miners._simple_miner import (
+    SimpleMiner,
+    simple_miner,
+)  # do not move cause InductiveMiner depends
 from sberpm.miners.mining_utils._node_utils import (
     ProcessTreeNode,
     ProcessTreeNodeType,
 )  # do not move cause InductiveMiner depends
 from sberpm.miners._inductive_miner import InductiveMiner, inductive_miner
-from sberpm.miners._ml_miner import MLMiner
-from sberpm.miners._parallel_miner import ParallelMiner
 
 __all__ = [
     "AbstractMiner",
     "AlphaMiner",
     "alpha_miner",
     "AlphaPlusMiner",
     "alpha_plus_miner",
-    "AutoMiner",
-    "auto_miner",
     "CausalMiner",
     "causal_miner",
     "CorrelationMiner",
     "correlation_miner",
     "HeuMiner",
     "heu_miner",
     "InductiveMiner",
     "inductive_miner",
-    "MLMiner",
-    "ParallelMiner",
     "ProcessTreeNode",
     "ProcessTreeNodeType",
     "SimpleMiner",
     "simple_miner",
 ]
```

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_abstract_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_abstract_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_alpha_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_alpha_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_alpha_plus_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_alpha_plus_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_causal_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_causal_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_correlation_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_correlation_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_heu_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_heu_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_inductive_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_inductive_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_inductive_utils.py` & `sberpm-2.6.3rc0/sberpm/miners/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/_simple_miner.py` & `sberpm-2.6.3rc0/sberpm/miners/_simple_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/mining_utils/_inductive_utils.py` & `sberpm-2.6.3rc0/sberpm/miners/mining_utils/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/miners/mining_utils/_node_utils.py` & `sberpm-2.6.3rc0/sberpm/miners/mining_utils/_node_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/__init__.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlier_detector.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outliercblof.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outliercblof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outliercustom.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outliercustom.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierforest.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierforest.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierlof.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierlof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/anomaly_detection/_outlierocsvm.py` & `sberpm-2.6.3rc0/sberpm/ml/anomaly_detection/_outlierocsvm.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/chronometrage/_chronometrage.py` & `sberpm-2.6.3rc0/sberpm/ml/chronometrage/_chronometrage.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/ml/utils/_perm_importance.py` & `sberpm-2.6.3rc0/sberpm/ml/utils/_perm_importance.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/models/_check_models.py` & `sberpm-2.6.3rc0/sberpm/models/_check_models.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/__init__.py` & `sberpm-2.6.3rc0/sberpm/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/_chart_painter.py` & `sberpm-2.6.3rc0/sberpm/visual/_chart_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/_graph.py` & `sberpm-2.6.3rc0/sberpm/visual/_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/_graphviz_painter.py` & `sberpm-2.6.3rc0/sberpm/visual/_graphviz_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/_matplotlib_painter.py` & `sberpm-2.6.3rc0/sberpm/visual/_matplotlib_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/_types.py` & `sberpm-2.6.3rc0/sberpm/visual/_types.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm/visual/utils.py` & `sberpm-2.6.3rc0/sberpm/visual/utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/sberpm.egg-info/PKG-INFO` & `sberpm-2.6.3rc0/sberpm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: sberpm
-Version: 2.6.2rc1
+Version: 2.6.3rc0
 Summary: Library that is intended to operate with various process mining tasks.
-Author: Sberbank Process Mining Team
-Author-email: AABugaenko@sberbank.ru
+Author: Sber Process Mining Team
+Author-email: SberPM_lib@sberbank.ru
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_RUS
 Requires-Dist: dataclassy==1.*
 Requires-Dist: dataenforce==0.1.2
@@ -65,9 +62,9 @@
 Additionally, you might need to install graphviz executables and add the path to the executables to PATH variable: https://graphviz.org/download/
 
 # Examples
 To find out how to work with SberPM, see [tutorials](https://pypi.org/project/sberpm/#files) in files tar.gz.
 
 # Contacts
 If you have any questions or suggestions, feel free to contact us!
-- Andrey Bugaenko (aabugaenko@sberbank.ru)
+- Библиотека Sber Process Mining ("SberPM_lib@sberbank.ru")
```

### Comparing `sberpm-2.6.2rc1/sberpm.egg-info/SOURCES.txt` & `sberpm-2.6.3rc0/sberpm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,61 +11,49 @@
 sberpm/_utils.py
 sberpm/_version.py
 sberpm.egg-info/PKG-INFO
 sberpm.egg-info/SOURCES.txt
 sberpm.egg-info/dependency_links.txt
 sberpm.egg-info/requires.txt
 sberpm.egg-info/top_level.txt
-sberpm/autoinsights/__init__.py
-sberpm/autoinsights/_influencing_activities.py
 sberpm/bpmn/__init__.py
 sberpm/bpmn/_bpmn_file_to_graph.py
 sberpm/bpmn/_bpmn_graph_to_file/__init__.py
 sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
 sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
 sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
 sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
 sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
-sberpm/column_matching/__init__.py
-sberpm/column_matching/_column_matching.py
-sberpm/column_matching/file_obf/_column_matching_.obfsbpm
 sberpm/conformance_checking/__init__.py
 sberpm/conformance_checking/_conformance_checking.py
 sberpm/conformance_checking/_token_replay.py
 sberpm/decision_mining/__init__.py
 sberpm/decision_mining/_decision_mining.py
 sberpm/graph_stats/__init__.py
 sberpm/graph_stats/centrality.py
 sberpm/imitation/__init__.py
 sberpm/imitation/_simulation.py
-sberpm/imitation/file_obf/_simulation_.obfsbpm
 sberpm/metrics/__init__.py
 sberpm/metrics/_activity_metric.py
 sberpm/metrics/_base_metric.py
 sberpm/metrics/_id_metric.py
 sberpm/metrics/_trace_metric.py
 sberpm/metrics/_transition_metric.py
 sberpm/metrics/_user_metric.py
 sberpm/metrics/_utils.py
 sberpm/miners/__init__.py
 sberpm/miners/_abstract_miner.py
 sberpm/miners/_alpha_miner.py
 sberpm/miners/_alpha_plus_miner.py
-sberpm/miners/_auto_miner.py
 sberpm/miners/_causal_miner.py
 sberpm/miners/_correlation_miner.py
 sberpm/miners/_heu_miner.py
 sberpm/miners/_inductive_miner.py
 sberpm/miners/_inductive_utils.py
-sberpm/miners/_ml_miner.py
-sberpm/miners/_parallel_miner.py
 sberpm/miners/_simple_miner.py
-sberpm/miners/file_obf/_auto_miner_.obfsbpm
-sberpm/miners/file_obf/_ml_miner_.obfsbpm
-sberpm/miners/file_obf/_parallel_miner_.obfsbpm
 sberpm/miners/mining_utils/__init__.py
 sberpm/miners/mining_utils/_inductive_utils.py
 sberpm/miners/mining_utils/_node_utils.py
 sberpm/ml/__init__.py
 sberpm/ml/anomaly_detection/__init__.py
 sberpm/ml/anomaly_detection/_outlier_detector.py
 sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
```

### Comparing `sberpm-2.6.2rc1/setup.py` & `sberpm-2.6.3rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from os import path, walk
 from platform import system
-from re import M, search 
+from re import M, search
 from typing import Iterable
 
 from setuptools import setup
 
 LIB_TITLE = "sberpm"
 PATH_SEPARATOR = "\\" if system() == "Windows" else "/"
 ROOT_PATH = path.abspath(path.dirname(__file__))
 LIB_PATH = f"{ROOT_PATH}{PATH_SEPARATOR}{LIB_TITLE}"
 VERSION_FILE = f"{LIB_TITLE}{PATH_SEPARATOR}_version.py"
 
+
 def get_packages() -> Iterable:
     """
     Returns:
     Iterable: list of packages available in library, nested starting with LIB_TITLE: sberpm
     """
 
     def replace_module_abs_path_with_relative_dotted(lib_module_abs_path):
         return f"{lib_module_abs_path.replace(f'{LIB_PATH}', f'{LIB_TITLE}').replace(f'{PATH_SEPARATOR}', '.')}"
 
-    return [replace_module_abs_path_with_relative_dotted(module) for module, _, _ in walk(LIB_PATH)]
+    return [
+        replace_module_abs_path_with_relative_dotted(module)
+        for module, _, _ in walk(LIB_PATH)
+    ]
 
 
 def get_readme_description() -> str:
     """
     Load README description
     """
-    with open(path.join(f"{ROOT_PATH}{PATH_SEPARATOR}", "README.md"), encoding="utf-8") as f:
+    with open(
+        path.join(f"{ROOT_PATH}{PATH_SEPARATOR}", "README.md"), encoding="utf-8"
+    ) as f:
         description = f.read()
 
     return description
 
 
 def get_version_number(version_file_path: str) -> str:
     version_line = open(version_file_path, "rt", encoding="utf8").read()
@@ -47,30 +53,27 @@
     """load requirements from a pip requirements file"""
     return [
         line
         for line in (line.strip() for line in open(filename, encoding="utf-8"))
         if line and not line.startswith("#")
     ]
 
+
 setup(
     name="sberpm",
     version=get_version_number(VERSION_FILE),
     description="Library that is intended to operate with various process mining tasks.",
     long_description=get_readme_description(),
     long_description_content_type="text/markdown",
-
-    author="Sberbank Process Mining Team",
-    author_email="AABugaenko@sberbank.ru",
+    author="Sber Process Mining Team",
+    author_email="SberPM_lib@sberbank.ru",
     packages=get_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=parse_requirements("requirements.txt"),
 )
```

### Comparing `sberpm-2.6.2rc1/tutorials/chrono_data.xlsx` & `sberpm-2.6.3rc0/tutorials/chrono_data.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/tutorials/example.xlsx` & `sberpm-2.6.3rc0/tutorials/example.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/tutorials/poster_PM/poster.png` & `sberpm-2.6.3rc0/tutorials/poster_PM/poster.png`

 * *Files identical despite different names*

### Comparing `sberpm-2.6.2rc1/tutorials/tutorial_en.ipynb` & `sberpm-2.6.3rc0/tutorials/tutorial_en.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923340886596864%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [1, 0]}}, 4: {'source': {insert: [(4, 'I. [Column "*

 * *            "matching](#I.-Column-matching) # only full library version\\n'), (27, ' 7. "*

 * *            "[ML-miners](#7.-ML-miners) # only full library version\\n'), (30, ' 10. "*

 * *            "[II-miner](#10.-II-miner) # only full library version\\n')], delete: [30, 27, 4]}}, "*

 * *            '7: {\'source\': {insert: [(0, "##### <font color=\'red\'>Full library '*

 * *            'version</font>\\n"), (1, \'\\n\')]}}, 33: {\'sour […]*

```diff
@@ -14,16 +14,14 @@
                 "__`sberpm`__ library is designed to analyse and investigate processes, display them as graphs and solve related classification and clustering problems using machine learning algorithms."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To get the full version of the library, write an email with a request to aabugaenko@sberbank.ru\n",
-                "\n",
                 "The page of the SberPM platform:\n",
                 "https://developers.sber.ru/portal/products/sber-process-mining"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -35,15 +33,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Contents\n",
                 "\n",
                 "[----------  Data preprocessing  ----------](#----------Data-preprocessing----------)\n",
                 "\n",
-                "I. [Column matching](#I.-Column-matching) \n",
+                "I. [Column matching](#I.-Column-matching) # only full library version\n",
                 "\n",
                 "II. [Log generator](#II.-Log-generator) # only full library version\n",
                 "\n",
                 "III. [Synthetic process IDs](#III.-Synthetic-process-IDs) # only full library version\n",
                 "\n",
                 "IV. [DataHolder](#IV.-DataHolder)\n",
                 "\n",
@@ -58,18 +56,18 @@
                 "I. [Miners and graph visualisation](#I.-Miners-and-graph-visualisation)\n",
                 " 1. [SimpleMiner](#1.-SimpleMiner)\n",
                 " 2. [CausalMiner](#2.-CausalMiner)\n",
                 " 3. [HeuMiner](#3.-HeuMiner)\n",
                 " 4. [AlphaMiner](#4.-AlphaMiner)\n",
                 " 5. [AlphaPlusMiner](#5.-AlphaPlusMiner)\n",
                 " 6. [InductiveMiner](#6.-InductiveMiner)\n",
-                " 7. [ML-miners](#7.-ML-miners)\n",
+                " 7. [ML-miners](#7.-ML-miners) # only full library version\n",
                 " 8. [NLP-Miner](#8.-NLP-miner) # only full library version\n",
                 " 9. [Correlation-Miner](#9.-Correlation-miner)\n",
-                " 10. [II-miner](#10.-II-miner)\n",
+                " 10. [II-miner](#10.-II-miner) # only full library version\n",
                 "\n",
                 "II. [Metrics](#II.-Metrics)\n",
                 "- [Metrics + graphs](#Metrics-+-graphs)\n",
                 "\n",
                 "III. [Conformance Checking](#III.-Conformance-Checking)\n",
                 "\n",
                 "IV. [BPMN](#IV.-BPMN)\n",
@@ -129,98 +127,17 @@
                 "## I. Column matching"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Column **Matching Module (sberpm.column_matching)** is a system for analyzing similarity of columns in two tables. Such analysis is performed using both text and numerical columns \u2013 in case columns in different tables have similar values, they will be matched."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "**Parameters of ColumnMatching**:\n",
-                "\n",
-                "* **data_left (pandas DataFrame)** \u2013 one table to compare\n",
-                "* **data_right (pandas DataFrame)** - another table to compare\n",
-                "* **p_value_threshold (float = default 0.05)** \u2013 Kolmogorov-Smirnov p-value threshold for numerical columns\n",
-                "* **iou_threshold (float = default 0.5)** \u2013 threshold for IOU (Intersection over Union) metric for text columns\n",
-                "\n",
-                "**Methods of ColumnMatching**:\n",
-                "* **get_result_pairs** returns pairs of similar columns in tables.\n",
-                "* **get_result_table** returns a pivot table where the axis are the column names from compared tables and the values are their similarity measures.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from pandas import DataFrame\n",
-                "from sberpm.column_matching import ColumnMatching"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Test on trivial data"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "data_left = DataFrame({\n",
-                "    \"names left\": [\"Alexander FFFFF\", \"Andrew Alexander\", \"Ilya Emilia\", \"Ilya Alexander\"] * 50,\n",
-                "    \"last names left\": [\"Arkhipov\", \"Kuznetsova\", \"Kuznetsova\", \"Bugaenko\"] * 50,\n",
-                "})\n",
-                "data_right = DataFrame({\n",
-                "    \"names right\": [\"Seva Alexander\", \"Alexander Vera\", \"Ilya Andrew\"] * 50,\n",
-                "    \"last names right\": [\"Zarubin\", \"Zarubin\", \"Kuznetsova\"] * 50,\n",
-                "})\n",
+                "##### <font color='red'>Full library version</font>\n",
                 "\n",
-                "column_map = ColumnMatching(\n",
-                "    data_left,\n",
-                "    data_right,\n",
-                "    p_value_threshold=0.05,\n",
-                "    iou_threshold=0.25,\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.map_columns()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.get_result_pairs()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.get_result_table()"
+                "Column **Matching Module (sberpm.column_matching)** is a system for analyzing similarity of columns in two tables. Such analysis is performed using both text and numerical columns \u2013 in case columns in different tables have similar values, they will be matched."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## II. Log generator\n",
@@ -473,25 +390,41 @@
             "metadata": {},
             "source": [
                 "Several algorithms are implemented in the library to build and draw the process graph. All of them are stored in the __`sberpm.miners`__ module and have one method:\n",
                 "- __apply__ - builds graph, which is saved in the graph field."
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%matplotlib inline\n",
+                "from sberpm.visual import GraphvizPainter"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 1. SimpleMiner"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`SimpleMiner` draws all edges found in the log (without any filtering).\n",
+                "`SimpleMiner` draws all edges found in the log (without any filtering)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "\n",
                 "In terms of Process Mining:\n",
                 "> If in at least one chain of activities from the log, some activity $X$ is directly followed by an activity $Y$ (a chain of the form $...XY...$), then write $X>Y$ ($Y$ follows $X$, _follows_ relation).\n",
                 "\n",
                 "SimpleMiner draws edges between such pairs of activities $X$ and $Y$ if $X>Y$ is true."
             ]
         },
@@ -847,86 +780,33 @@
                 "### 7. __ML-miners__"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "##### <font color='red'>Full library version</font>\n",
+                "\n",
                 "__ML-miner__ based on Lasso regression. \n",
                 "\n",
                 "With this miner, number of repetitoions of each stage in each process is calculated. Lasso-regression is fitted, in which a column of one type of activity is considered as a goal (dependent variable), and the rest of the columns of other activities - as features (indipendent variables). On the edges (links) only those relationships are displayed that have the absolute value of the Lasso coefficient more than the value of the threshold value.\n",
-                "``ML-miner`` draws the edges between such pairs of activity $X$ and $Y$, if $X$ affects $Y$.\n",
-                "\n",
-                "- __data_holder: DataHolder__ - An object containing a journal of events and the names of its necessary columns.\n",
-                "- __threshold: float (\u041f\u043e \u0443\u043c\u043e\u043b\u0447\u0430\u043d\u0438\u044e 0.05)__ - The threshold of the absolute value of the regression coefficient. The values exceeding the threshold value are considered significant connections between activity."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import MLMiner"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Miner\n",
-                "ml_miner = MLMiner(data_holder, threshold=0.1)\n",
-                "ml_miner.apply()\n",
-                "graph = ml_miner.graph\n",
-                "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "``ML-miner`` draws the edges between such pairs of activity $X$ and $Y$, if $X$ affects $Y$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### __Auto-miner__\n",
                 "\n",
-                "``Auto-miner`` based on Sequence Feature Selector.\n",
-                "\n",
-                "``Auto-miner`` draws edges between such pairs of activities $X$ and $Y$, if $X$ affects $Y$.\n",
+                "##### <font color='red'>Full library version</font>\n",
                 "\n",
-                "- __data_holder: DataHolder__ An object containing a journal of events and the names of its necessary columns."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import AutoMiner"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Miner\n",
-                "autominer = AutoMiner(data_holder)\n",
-                "autominer.apply()\n",
-                "graph = autominer.graph\n",
+                "``Auto-miner`` based on Sequence Feature Selector.\n",
                 "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "``Auto-miner`` draws edges between such pairs of activities $X$ and $Y$, if $X$ affects $Y$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 8. __NLP-miner__\n",
@@ -975,42 +855,21 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 10. __II-miner__\n",
+                "##### <font color='red'>Full library version</font>\n",
                 "\n",
                 "Miner for analyzing parallel actions.\n",
                 "  Counts intersections on temporary labels of activities.\n",
                 "  Parallel stages are stages with such copies of processes where \"begin\"-time and \"end\"-time are overlaped.\n",
                 "  In addition, there id `parallel_metric` node, which shows the number of time intersections to\n",
-                "this stage and other stages. From the blue nodes, the arrows indicate parallel stages.\n",
-                "\n",
-                "- __data_holder: DataHolder__ An object containing a journal of events and the names of its necessary columns.\n",
-                "- __Graph__ obtained graph of a process"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import ParallelMiner\n",
-                "\n",
-                "# Miner\n",
-                "parallel_miner = ParallelMiner(data_holder)\n",
-                "parallel_miner.apply()\n",
-                "graph = parallel_miner.graph\n",
-                "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "this stage and other stages. From the blue nodes, the arrows indicate parallel stages."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
```

### Comparing `sberpm-2.6.2rc1/tutorials/tutorial_ru.ipynb` & `sberpm-2.6.3rc0/tutorials/tutorial_ru.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9938488629442461%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [1, 0]}}, 4: {'source': {insert: [(4, 'I. [Мэтчинг "*

 * *            "таблиц](#I.-Мэтчинг-таблиц) # в полной версии библиотеки\\n'), (27, ' 7. "*

 * *            "[ML-miners](#7.-ML-miners) # в полной версии библиотеки\\n'), (30, ' 10. "*

 * *            "[II-miner](#10.-II-miner) # в полной версии библиотеки\\n')], delete: [30, 27, 4]}}, "*

 * *            '6: {\'source\': {insert: [(1, "##### <font color=\'red\'>В полной версии '*

 * *            'библиотеки</font>\\n"), (4, \'Данный модуль п […]*

```diff
@@ -14,16 +14,14 @@
                 "\u0411\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0430 __`sberpm`__ \u043f\u0440\u0435\u0434\u043d\u0430\u0437\u043d\u0430\u0447\u0435\u043d\u0430 \u0434\u043b\u044f \u0430\u043d\u0430\u043b\u0438\u0437\u0430 \u0438 \u0438\u0441\u0441\u043b\u0435\u0434\u043e\u0432\u0430\u043d\u0438\u044f \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0432, \u043f\u043e\u0441\u0442\u0440\u043e\u0435\u043d\u0438\u044f \u0438\u0445 \u0432 \u0432\u0438\u0434\u0435 \u0433\u0440\u0430\u0444\u043e\u0432 \u0438 \u0440\u0435\u0448\u0435\u043d\u0438\u044f \u0441\u043c\u0435\u0436\u043d\u044b\u0445 \u0437\u0430\u0434\u0430\u0447 \u043a\u043b\u0430\u0441\u0441\u0438\u0444\u0438\u043a\u0430\u0446\u0438\u0438 \u0438 \u043a\u043b\u0430\u0441\u0442\u0435\u0440\u0438\u0437\u0430\u0446\u0438\u0438 \u0441 \u0438\u0441\u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u043d\u0438\u0435\u043c \u0430\u043b\u0433\u043e\u0440\u0438\u0442\u043c\u043e\u0432 \u043c\u0430\u0448\u0438\u043d\u043d\u043e\u0433\u043e \u043e\u0431\u0443\u0447\u0435\u043d\u0438\u044f."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "__\u0414\u043b\u044f \u043f\u043e\u043b\u0443\u0447\u0435\u043d\u0438\u044f \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438, \u043d\u0430\u043f\u0438\u0448\u0438\u0442\u0435 \u043f\u0438\u0441\u044c\u043c\u043e \u0441 \u0437\u0430\u043f\u0440\u043e\u0441\u043e\u043c \u043d\u0430 aabugaenko@sberbank.ru__\n",
-                "\n",
                 "__\u0421\u0442\u0440\u0430\u043d\u0438\u0446\u0430 \u043f\u043b\u0430\u0442\u0444\u043e\u0440\u043c\u044b SberPM:\n",
                 "https://developers.sber.ru/portal/products/sber-process-mining__"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -35,15 +33,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## \u041e\u0433\u043b\u0430\u0432\u043b\u0435\u043d\u0438\u0435\n",
                 "\n",
                 "[----------  \u041f\u0440\u0435\u0434\u0432\u0430\u0440\u0438\u0442\u0435\u043b\u044c\u043d\u0430\u044f \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0430 \u0434\u0430\u043d\u043d\u044b\u0445  ----------](#------------\u041f\u0440\u0435\u0434\u0432\u0430\u0440\u0438\u0442\u0435\u043b\u044c\u043d\u0430\u044f-\u043e\u0431\u0440\u0430\u0431\u043e\u0442\u043a\u0430-\u0434\u0430\u043d\u043d\u044b\u0445------------)\n",
                 "\n",
-                "I. [\u041c\u044d\u0442\u0447\u0438\u043d\u0433 \u0442\u0430\u0431\u043b\u0438\u0446](#I.-\u041c\u044d\u0442\u0447\u0438\u043d\u0433-\u0442\u0430\u0431\u043b\u0438\u0446)\n",
+                "I. [\u041c\u044d\u0442\u0447\u0438\u043d\u0433 \u0442\u0430\u0431\u043b\u0438\u0446](#I.-\u041c\u044d\u0442\u0447\u0438\u043d\u0433-\u0442\u0430\u0431\u043b\u0438\u0446) # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 "\n",
                 "II. [\u0413\u0435\u043d\u0435\u0440\u0430\u0442\u043e\u0440 \u043b\u043e\u0433\u043e\u0432](#II.-\u0413\u0435\u043d\u0435\u0440\u0430\u0442\u043e\u0440-\u043b\u043e\u0433\u043e\u0432) # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 "\n",
                 "III. [\u0421\u0438\u043d\u0442\u0435\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0435 ID \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u0430](#III.-\u0421\u0438\u043d\u0442\u0435\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0435-ID-\u043f\u0440\u043e\u0446\u0435\u0441\u0441\u0430)  # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 "\n",
                 "IV. [DataHolder](#IV.-DataHolder)\n",
                 "\n",
@@ -58,18 +56,18 @@
                 "I. [\u041c\u0430\u0439\u043d\u0435\u0440\u044b \u0438 \u0432\u0438\u0437\u0443\u0430\u043b\u0438\u0437\u0430\u0446\u0438\u044f \u0433\u0440\u0430\u0444\u043e\u0432](#I.-\u041c\u0430\u0439\u043d\u0435\u0440\u044b-\u0438-\u0432\u0438\u0437\u0443\u0430\u043b\u0438\u0437\u0430\u0446\u0438\u044f-\u0433\u0440\u0430\u0444\u043e\u0432)\n",
                 " 1. [SimpleMiner](#1.-SimpleMiner)\n",
                 " 2. [CausalMiner](#2.-CausalMiner)\n",
                 " 3. [HeuMiner](#3.-HeuMiner)\n",
                 " 4. [AlphaMiner](#4.-AlphaMiner)\n",
                 " 5. [AlphaPlusMiner](#5.-AlphaPlusMiner)\n",
                 " 6. [InductiveMiner](#6.-InductiveMiner)\n",
-                " 7. [ML-miners](#7.-ML-miners)\n",
+                " 7. [ML-miners](#7.-ML-miners) # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 " 8. [NLP-Miner](#8.-NLP-miner) # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 " 9. [Correlation-Miner](#9.-Correlation-miner)\n",
-                " 10. [II-miner](#10.-II-miner)\n",
+                " 10. [II-miner](#10.-II-miner) # \u0432 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438\n",
                 "\n",
                 "II. [\u041c\u0435\u0442\u0440\u0438\u043a\u0438](#II.-\u041c\u0435\u0442\u0440\u0438\u043a\u0438)\n",
                 "- [\u041c\u0435\u0442\u0440\u0438\u043a\u0438 + \u0433\u0440\u0430\u0444\u044b](#\u041c\u0435\u0442\u0440\u0438\u043a\u0438-+-\u0433\u0440\u0430\u0444\u044b)\n",
                 "\n",
                 "III. [Conformance Checking](#III.-Conformance-Checking)\n",
                 "\n",
                 " IV. [BPMN](#IV.-BPMN)\n",
@@ -123,93 +121,18 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## I. \u041c\u044d\u0442\u0447\u0438\u043d\u0433 \u0442\u0430\u0431\u043b\u0438\u0446\n",
+                "##### <font color='red'>\u0412 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438</font>\n",
                 "\n",
-                "\u0414\u0430\u043d\u043d\u044b\u0439 \u043c\u043e\u0434\u0443\u043b\u044c **`sberpm.column_matching`** \u043f\u0440\u0435\u0434\u0441\u0442\u0430\u0432\u043b\u044f\u0435\u0442 \u0441\u043e\u0431\u043e\u0439 \u0441\u0438\u0441\u0442\u0435\u043c\u0443 \u0434\u043b\u044f \u0430\u043d\u0430\u043b\u0438\u0437\u0430 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u0441\u0442\u043e\u043b\u0431\u0446\u043e\u0432 \u0432 \u0434\u0432\u0443\u0445 \u0442\u0430\u0431\u043b\u0438\u0446\u0430\u0445. \u0410\u043d\u0430\u043b\u0438\u0437 \u043f\u0440\u043e\u0438\u0437\u0432\u043e\u0434\u0438\u0442\u0441\u044f \u043f\u043e \u0442\u0435\u043a\u0441\u0442\u043e\u0432\u044b\u043c \u0438 \u0447\u0438\u0441\u043b\u0435\u043d\u043d\u044b\u043c \u043a\u043e\u043b\u043e\u043d\u043a\u0430\u043c. \u041a\u043e\u043b\u043e\u043d\u043a\u0438, \u0443 \u043a\u043e\u0442\u043e\u0440\u044b\u0445 \u0431\u0443\u0434\u0443\u0442 \u043f\u043e\u0445\u043e\u0436\u0438\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u0432 \u0440\u0430\u0437\u043d\u044b\u0445 \u0442\u0430\u0431\u043b\u0438\u0446\u0430\u0445, \u0431\u0443\u0434\u0443\u0442 \u0441\u043e\u043f\u043e\u0441\u0442\u0430\u0432\u043b\u044f\u0442\u044c\u0441\u044f. \n",
-                "\n",
-                "\u041f\u0430\u0440\u0430\u043c\u0435\u0442\u0440\u044b, \u043f\u0435\u0440\u0435\u0434\u0430\u0432\u0430\u0435\u043c\u044b\u0435 \u0432 \u043a\u043b\u0430\u0441\u0441 **ColumnMatching**:\n",
-                "* **data_left (pandas DataFrame)** - \u043f\u0435\u0440\u0432\u0430\u044f \u0442\u0430\u0431\u043b\u0438\u0446\u0430 \u0434\u043b\u044f \u0441\u0440\u0430\u0432\u043d\u0435\u043d\u0438\u044f\n",
-                "* **data_right (pandas DataFrame)** - \u0432\u0442\u043e\u0440\u0430\u044f \u0442\u0430\u0431\u043b\u0438\u0446\u0430 \u0434\u043b\u044f \u0441\u0440\u0430\u0432\u043d\u0435\u043d\u0438\u044f\n",
-                "* **p_value_threshold (float = default 0.05)** - \u043f\u043e\u0440\u043e\u0433 \u0434\u043b\u044f p-value \u0442\u0435\u0441\u0442\u0430 \u041a\u043e\u043b\u043c\u043e\u0433\u043e\u0440\u043e\u0432\u0430-\u0421\u043c\u0438\u0440\u043d\u043e\u0432\u0430 \u0434\u043b\u044f \u0447\u0438\u0441\u043b\u0435\u043d\u043d\u044b\u0445 \u043a\u043e\u043b\u043e\u043d\u043e\u043a\n",
-                "* **iou_threshold (float = default 0.5)** - \u043f\u043e\u0440\u043e\u0433 \u0434\u043b\u044f \u043c\u0435\u0442\u0440\u0438\u043a\u0438 IOU \u0434\u043b\u044f \u0442\u0435\u043a\u0441\u0442\u043e\u0432\u044b\u0445 \u043a\u043e\u043b\u043e\u043d\u043e\u043a\n",
                 "\n",
-                "\u041c\u0435\u0442\u043e\u0434\u044b \u043a\u043b\u0430\u0441\u0441\u0430 **`ColumnMatching`**:\n",
-                "- **get_result_pairs** \u0432\u043e\u0437\u0432\u0440\u0430\u0449\u0430\u0435\u0442 \u043f\u0430\u0440\u044b \u0441 \u043f\u043e\u0445\u043e\u0436\u0438\u043c\u0438 \u043a\u043e\u043b\u043e\u043d\u043a\u0430\u043c\u0438 \u0438\u0437 \u043b\u0435\u0432\u043e\u0439 \u0438 \u043f\u0440\u0430\u0432\u043e\u0439 \u0442\u0430\u0431\u043b\u0438\u0446\u0435.\n",
-                "- **get_result_table** \u0432\u043e\u0437\u0432\u0440\u0430\u0449\u0430\u0435\u0442 \u0441\u0432\u043e\u0434\u043d\u0443\u044e \u0442\u0430\u0431\u043b\u0438\u0446\u0443, \u0432 \u043a\u043e\u0442\u043e\u0440\u043e\u0439 \u043f\u043e \u043e\u0441\u044f\u043c \u043a\u043e\u043b\u043e\u043d\u043a\u0438 \u0438\u0437 \u043b\u0435\u0432\u043e\u0439 \u0438 \u043f\u0440\u0430\u0432\u043e\u0439 \u0442\u0430\u0431\u043b\u0438\u0446\u0435, \u0430 \u0432 \u044f\u0447\u0435\u0439\u043a\u0430\u0445 \u043c\u0435\u0440\u044b \u043f\u043e\u0445\u043e\u0436\u0435\u0441\u0442\u0438 \u0441\u043e\u043e\u0442\u0432\u0435\u0442\u0441\u0442\u0432\u0443\u044e\u0449\u0438\u0445 \u043a\u043e\u043b\u043e\u043d\u043e\u043a."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from pandas import DataFrame\n",
-                "from sberpm.column_matching import ColumnMatching"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### \u0422\u0435\u0441\u0442 \u043d\u0430 \u0442\u0440\u0438\u0432\u0438\u0430\u043b\u044c\u043d\u044b\u0445 \u0441\u0438\u043d\u0442\u0435\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0445 \u0434\u0430\u043d\u043d\u044b\u0445"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "data_left = DataFrame({\n",
-                "    \"names left\": [\"Alexander FFFFF\", \"Andrew Alexander\", \"Ilya Emilia\", \"Ilya Alexander\"] * 50,\n",
-                "    \"last names left\": [\"Arkhipov\", \"Kuznetsova\", \"Kuznetsova\", \"Bugaenko\"] * 50,\n",
-                "})\n",
-                "data_right = DataFrame({\n",
-                "    \"names right\": [\"Seva Alexander\", \"Alexander Vera\", \"Ilya Andrew\"] * 50,\n",
-                "    \"last names right\": [\"Zarubin\", \"Zarubin\", \"Kuznetsova\"] * 50,\n",
-                "})\n",
-                "\n",
-                "column_map = ColumnMatching(\n",
-                "    data_left,\n",
-                "    data_right,\n",
-                "    p_value_threshold=0.05,\n",
-                "    iou_threshold=0.25,\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.map_columns()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.get_result_pairs()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "column_map.get_result_table()"
+                "\u0414\u0430\u043d\u043d\u044b\u0439 \u043c\u043e\u0434\u0443\u043b\u044c \u043f\u0440\u0435\u0434\u0441\u0442\u0430\u0432\u043b\u044f\u0435\u0442 \u0441\u043e\u0431\u043e\u0439 \u0441\u0438\u0441\u0442\u0435\u043c\u0443 \u0434\u043b\u044f \u0430\u043d\u0430\u043b\u0438\u0437\u0430 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u0441\u0442\u043e\u043b\u0431\u0446\u043e\u0432 \u0432 \u0434\u0432\u0443\u0445 \u0442\u0430\u0431\u043b\u0438\u0446\u0430\u0445. \u0410\u043d\u0430\u043b\u0438\u0437 \u043f\u0440\u043e\u0438\u0437\u0432\u043e\u0434\u0438\u0442\u0441\u044f \u043f\u043e \u0442\u0435\u043a\u0441\u0442\u043e\u0432\u044b\u043c \u0438 \u0447\u0438\u0441\u043b\u0435\u043d\u043d\u044b\u043c \u043a\u043e\u043b\u043e\u043d\u043a\u0430\u043c. \u041a\u043e\u043b\u043e\u043d\u043a\u0438, \u0443 \u043a\u043e\u0442\u043e\u0440\u044b\u0445 \u0431\u0443\u0434\u0443\u0442 \u043f\u043e\u0445\u043e\u0436\u0438\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u0432 \u0440\u0430\u0437\u043d\u044b\u0445 \u0442\u0430\u0431\u043b\u0438\u0446\u0430\u0445, \u0431\u0443\u0434\u0443\u0442 \u0441\u043e\u043f\u043e\u0441\u0442\u0430\u0432\u043b\u044f\u0442\u044c\u0441\u044f. "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## II. \u0413\u0435\u043d\u0435\u0440\u0430\u0442\u043e\u0440 \u043b\u043e\u0433\u043e\u0432\n",
@@ -858,94 +781,35 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 7. __ML-miners__"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import MLMiner"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "__ML-miner__ - \u043c\u0430\u0439\u043d\u0435\u0440 \u043e\u0441\u043d\u043e\u0432\u0430\u043d\u043d\u044b\u0439 \u043d\u0430 lasso-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u0438. \n",
-                "\n",
-                "\u0412 \u0434\u0430\u043d\u043d\u043e\u043c \u043c\u0430\u0439\u043d\u0435\u0440\u0435 \u043f\u043e\u0434\u0441\u0447\u0438\u0442\u044b\u0432\u0430\u044e\u0442\u0441\u044f \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e \u043f\u043e\u0432\u0442\u043e\u0440\u0435\u043d\u0438\u0439 \u043a\u0430\u0436\u0434\u043e\u0433\u043e \u044d\u0442\u0430\u043f\u0430 \u0432 \u043a\u0430\u0436\u0434\u043e\u043c \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u0435. \u0420\u0430\u0441\u0441\u0447\u0438\u0442\u044b\u0432\u0430\u0435\u0442\u0441\u044f \u043b\u0430\u0441\u0441\u043e-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u044f, \u0432 \u043a\u043e\u0442\u043e\u0440\u043e\u0439 \u0441\u0442\u043e\u043b\u0431\u0435\u0446 \u043e\u0434\u043d\u043e\u0433\u043e \u0432\u0438\u0434\u0430 \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u0438 \u0440\u0430\u0441\u0441\u043c\u0430\u0442\u0440\u0438\u0432\u0430\u0435\u0442\u0441\u044f \u043a\u0430\u043a \u0446\u0435\u043b\u044c, \u0430 \u043e\u0441\u0442\u0430\u043b\u044c\u043d\u044b\u0435 \u0441\u0442\u043e\u043b\u0431\u0446\u044b \u0434\u0440\u0443\u0433\u0438\u0445 \u0432\u0438\u0434\u043e\u0432 \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u0438 - \u043a\u0430\u043a \u043f\u0440\u0438\u0437\u043d\u0430\u043a\u0438. \u041d\u0430 \u0440\u0435\u0431\u0440\u0430\u0445 \u0433\u0440\u0430\u0444\u0430 \u043e\u0442\u043e\u0431\u0440\u0430\u0436\u0430\u044e\u0442\u0441\u044f \u0442\u043e\u043b\u044c\u043a\u043e \u0442\u0435 \u043e\u0442\u043d\u043e\u0448\u0435\u043d\u0438\u044f, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0438\u043c\u0435\u044e\u0442 \u0430\u0431\u0441\u043e\u043b\u044e\u0442\u043d\u043e\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435 \u043a\u043e\u044d\u0444\u0444\u0438\u0446\u0438\u0435\u043d\u0442\u0430 \u043b\u0430\u0441\u0441\u043e-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u0438 \u0431\u043e\u043b\u044c\u0448\u0435, \u0447\u0435\u043c \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435 \u043f\u043e\u0440\u043e\u0433\u043e\u0432\u043e\u0433\u043e \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f.\n",
-                "\n",
-                "``ML-miner`` \u0440\u0438\u0441\u0443\u0435\u0442 \u0440\u0435\u0431\u0440\u0430 \u043c\u0435\u0436\u0434\u0443 \u0442\u0430\u043a\u0438\u043c\u0438 \u043f\u0430\u0440\u0430\u043c\u0438 \u0430\u043a\u0442\u0438\u0432\u043d\u043e\u0441\u0442\u0435\u0439 $X$ \u0438 $Y$, \u0435\u0441\u043b\u0438 $X$ \u0432\u043b\u0438\u044f\u0435\u0442 \u043d\u0430 $Y$.\n",
-                "\n",
-                "* data_holder : DataHolder\n",
-                "    \u041e\u0431\u044a\u0435\u043a\u0442, \u0441\u043e\u0434\u0435\u0440\u0436\u0430\u0449\u0438\u0439 \u0436\u0443\u0440\u043d\u0430\u043b \u0441\u043e\u0431\u044b\u0442\u0438\u0439 \u0438 \u0438\u043c\u0435\u043d\u0430 \u0435\u0433\u043e \u043d\u0435\u043e\u0431\u0445\u043e\u0434\u0438\u043c\u044b\u0445 \u043a\u043e\u043b\u043e\u043d\u043e\u043a.\n",
+                "##### <font color='red'>\u0412 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438</font>\n",
                 "\n",
-                "* threshold: float (\u041f\u043e \u0443\u043c\u043e\u043b\u0447\u0430\u043d\u0438\u044e 0.05)\n",
-                "    \u041f\u043e\u0440\u043e\u0433 \u0430\u0431\u0441\u043e\u043b\u044e\u0442\u043d\u043e\u0433\u043e \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u043a\u043e\u044d\u0444\u0444\u0438\u0446\u0438\u0435\u043d\u0442\u0430 \u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u0438. \u0417\u043d\u0430\u0447\u0435\u043d\u0438\u044f \u043f\u0440\u0435\u0432\u044b\u0448\u0430\u044e\u0449\u0438\u0435 \u043f\u043e\u0440\u043e\u0433\u043e\u0432\u043e\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435, \u0441\u0447\u0438\u0442\u0430\u044e\u0442\u0441\u044f \u0437\u043d\u0430\u0447\u0438\u043c\u044b\u043c\u0438 \u0441\u0432\u044f\u0437\u044f\u043c\u0438 \u043c\u0435\u0436\u0434\u0443 \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u044c\u044e.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Miner\n",
-                "ml_miner = MLMiner(data_holder, threshold=0.1)\n",
-                "ml_miner.apply()\n",
-                "graph = ml_miner.graph\n",
+                "__ML-miner__ - \u043c\u0430\u0439\u043d\u0435\u0440 \u043e\u0441\u043d\u043e\u0432\u0430\u043d\u043d\u044b\u0439 \u043d\u0430 lasso-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u0438. \n",
                 "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "\u0412 \u0434\u0430\u043d\u043d\u043e\u043c \u043c\u0430\u0439\u043d\u0435\u0440\u0435 \u043f\u043e\u0434\u0441\u0447\u0438\u0442\u044b\u0432\u0430\u044e\u0442\u0441\u044f \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e \u043f\u043e\u0432\u0442\u043e\u0440\u0435\u043d\u0438\u0439 \u043a\u0430\u0436\u0434\u043e\u0433\u043e \u044d\u0442\u0430\u043f\u0430 \u0432 \u043a\u0430\u0436\u0434\u043e\u043c \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u0435. \u0420\u0430\u0441\u0441\u0447\u0438\u0442\u044b\u0432\u0430\u0435\u0442\u0441\u044f \u043b\u0430\u0441\u0441\u043e-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u044f, \u0432 \u043a\u043e\u0442\u043e\u0440\u043e\u0439 \u0441\u0442\u043e\u043b\u0431\u0435\u0446 \u043e\u0434\u043d\u043e\u0433\u043e \u0432\u0438\u0434\u0430 \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u0438 \u0440\u0430\u0441\u0441\u043c\u0430\u0442\u0440\u0438\u0432\u0430\u0435\u0442\u0441\u044f \u043a\u0430\u043a \u0446\u0435\u043b\u044c, \u0430 \u043e\u0441\u0442\u0430\u043b\u044c\u043d\u044b\u0435 \u0441\u0442\u043e\u043b\u0431\u0446\u044b \u0434\u0440\u0443\u0433\u0438\u0445 \u0432\u0438\u0434\u043e\u0432 \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u0438 - \u043a\u0430\u043a \u043f\u0440\u0438\u0437\u043d\u0430\u043a\u0438. \u041d\u0430 \u0440\u0435\u0431\u0440\u0430\u0445 \u0433\u0440\u0430\u0444\u0430 \u043e\u0442\u043e\u0431\u0440\u0430\u0436\u0430\u044e\u0442\u0441\u044f \u0442\u043e\u043b\u044c\u043a\u043e \u0442\u0435 \u043e\u0442\u043d\u043e\u0448\u0435\u043d\u0438\u044f, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0438\u043c\u0435\u044e\u0442 \u0430\u0431\u0441\u043e\u043b\u044e\u0442\u043d\u043e\u0435 \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435 \u043a\u043e\u044d\u0444\u0444\u0438\u0446\u0438\u0435\u043d\u0442\u0430 \u043b\u0430\u0441\u0441\u043e-\u0440\u0435\u0433\u0440\u0435\u0441\u0441\u0438\u0438 \u0431\u043e\u043b\u044c\u0448\u0435, \u0447\u0435\u043c \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u0435 \u043f\u043e\u0440\u043e\u0433\u043e\u0432\u043e\u0433\u043e \u0437\u043d\u0430\u0447\u0435\u043d\u0438\u044f."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### __Auto-miner__\n",
+                "##### <font color='red'>\u0412 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438</font>\n",
                 "\n",
-                "``Auto-miner`` \u043e\u0441\u043d\u043e\u0432\u0430\u043d \u043d\u0430 Sequence Feature Selector.\n",
-                "\n",
-                "``Auto-miner`` \u0440\u0438\u0441\u0443\u0435\u0442 \u0440\u0435\u0431\u0440\u0430 \u043c\u0435\u0436\u0434\u0443 \u0442\u0430\u043a\u0438\u043c\u0438 \u043f\u0430\u0440\u0430\u043c\u0438 \u0430\u043a\u0442\u0438\u0432\u043d\u043e\u0441\u0442\u0435\u0439 $X$ \u0438 $Y$, \u0435\u0441\u043b\u0438 $X$ \u0432\u043b\u0438\u044f\u0435\u0442 \u043d\u0430 $Y$.\n",
                 "\n",
-                "* data_holder : DataHolder\n",
-                "    \u041e\u0431\u044a\u0435\u043a\u0442, \u0441\u043e\u0434\u0435\u0440\u0436\u0430\u0449\u0438\u0439 \u0436\u0443\u0440\u043d\u0430\u043b \u0441\u043e\u0431\u044b\u0442\u0438\u0439 \u0438 \u0438\u043c\u0435\u043d\u0430 \u0435\u0433\u043e \u043d\u0435\u043e\u0431\u0445\u043e\u0434\u0438\u043c\u044b\u0445 \u0441\u0442\u043e\u043b\u0431\u0446\u043e\u0432.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import AutoMiner"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Miner\n",
-                "autominer = AutoMiner(data_holder)\n",
-                "autominer.apply()\n",
-                "graph = autominer.graph\n",
+                "``Auto-miner`` \u043e\u0441\u043d\u043e\u0432\u0430\u043d \u043d\u0430 Sequence Feature Selector.\n",
                 "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "``Auto-miner`` \u0440\u0438\u0441\u0443\u0435\u0442 \u0440\u0435\u0431\u0440\u0430 \u043c\u0435\u0436\u0434\u0443 \u0442\u0430\u043a\u0438\u043c\u0438 \u043f\u0430\u0440\u0430\u043c\u0438 \u0430\u043a\u0442\u0438\u0432\u043d\u043e\u0441\u0442\u0435\u0439 $X$ \u0438 $Y$, \u0435\u0441\u043b\u0438 $X$ \u0432\u043b\u0438\u044f\u0435\u0442 \u043d\u0430 $Y$."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 8. __NLP-miner__\n",
@@ -1005,46 +869,20 @@
                 "### 10. __II-miner__"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "##### <font color='red'>\u0412 \u043f\u043e\u043b\u043d\u043e\u0439 \u0432\u0435\u0440\u0441\u0438\u0438 \u0431\u0438\u0431\u043b\u0438\u043e\u0442\u0435\u043a\u0438</font>\n",
+                "\n",
                 "\u041c\u0430\u0439\u043d\u0435\u0440 \u0434\u043b\u044f \u0430\u043d\u0430\u043b\u0438\u0437\u0430 \u043f\u0430\u0440\u0430\u043b\u043b\u0435\u043b\u044c\u043d\u044b\u0445 \u0434\u0435\u0439\u0441\u0442\u0432\u0438\u0439.\n",
                 " \u041f\u043e\u0434\u0441\u0447\u0438\u0442\u044b\u0432\u0430\u0435\u0442 \u043f\u0435\u0440\u0435\u0441\u0435\u0447\u0435\u043d\u0438\u044f \u043f\u043e \u0432\u0440\u0435\u043c\u0435\u043d\u043d\u044b\u043c \u043c\u0435\u0442\u043a\u0430\u043c \u0434\u0435\u0439\u0441\u0442\u0432\u0438\u0439.\n",
                 " \u041f\u0430\u0440\u0430\u043b\u043b\u0435\u043b\u044c\u043d\u044b\u0435 \u044d\u0442\u0430\u043f\u044b - \u044d\u0442\u043e \u044d\u0442\u0430\u043f\u044b \u0441 \u0442\u0430\u043a\u0438\u043c\u0438 \u044d\u043a\u0437\u0435\u043c\u043f\u043b\u044f\u0440\u0430\u043c\u0438 \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0432, \u0447\u0442\u043e \u0432\u0440\u0435\u043c\u044f \u0438\u0445 \u043d\u0430\u0447\u0430\u043b\u0430 \u0438\n",
-                "\u043e\u043a\u043e\u043d\u0447\u0430\u043d\u0438\u044f \u043f\u0435\u0440\u0435\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f.\n",
-                " \u0414\u043e\u0431\u0430\u0432\u043b\u0435\u043d \u0443\u0437\u0435\u043b `parallel_metric`, \u043a\u043e\u0442\u043e\u0440\u044b\u0439 \u043f\u043e\u043a\u0430\u0437\u044b\u0432\u0430\u0435\u0442 \u043a\u043e\u043b\u0438\u0447\u0435\u0441\u0442\u0432\u043e \u043f\u0435\u0440\u0435\u0441\u0435\u0447\u0435\u043d\u0438\u0439 \u0432\u0440\u0435\u043c\u0435\u043d\u0438 \u043d\u0430\n",
-                "\u044d\u0442\u043e\u043c \u044d\u0442\u0430\u043f\u0435 \u0438 \u0434\u0440\u0443\u0433\u0438\u0445 \u044d\u0442\u0430\u043f\u0430\u0445. \u041e\u0442 \u0441\u0438\u043d\u0438\u0445 \u0443\u0437\u043b\u043e\u0432 \u0441\u0442\u0440\u0435\u043b\u043a\u0438 \u0443\u043a\u0430\u0437\u044b\u0432\u0430\u044e\u0442 \u043d\u0430 \u043f\u0430\u0440\u0430\u043b\u043b\u0435\u043b\u044c\u043d\u044b\u0435 \u044d\u0442\u0430\u043f\u044b.\n",
-                "\n",
-                "\u041f\u0430\u0440\u0430\u043c\u0435\u0442\u0440\u044b:\n",
-                " data_holder: DataHolder\n",
-                " \u041e\u0431\u044a\u0435\u043a\u0442, \u0441\u043e\u0434\u0435\u0440\u0436\u0430\u0449\u0438\u0439 \u0436\u0443\u0440\u043d\u0430\u043b \u0441\u043e\u0431\u044b\u0442\u0438\u0439 \u0438 \u0438\u043c\u0435\u043d\u0430 \u0435\u0433\u043e \u043d\u0435\u043e\u0431\u0445\u043e\u0434\u0438\u043c\u044b\u0445 \u0441\u0442\u043e\u043b\u0431\u0446\u043e\u0432.\n",
-                "\n",
-                " \u0410\u0440\u0433\u0443\u043c\u0435\u043d\u0442\u044b:\n",
-                " graph: \u0434\u043e\u0431\u044b\u0442\u044b\u0439 \u0433\u0440\u0430\u0444\u0438\u043a \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u0430 \u0434\u043b\u044f \u0440\u0438\u0441\u043e\u0432\u0430\u043d\u0438\u044f"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sberpm.miners import ParallelMiner\n",
-                "\n",
-                "# Miner\n",
-                "parallel_miner = ParallelMiner(data_holder)\n",
-                "parallel_miner.apply()\n",
-                "graph = parallel_miner.graph\n",
-                "\n",
-                "# Visualization\n",
-                "painter = GraphvizPainter()\n",
-                "painter.apply(graph)\n",
-                "painter.show()"
+                "\u043e\u043a\u043e\u043d\u0447\u0430\u043d\u0438\u044f \u043f\u0435\u0440\u0435\u043a\u0440\u044b\u0432\u0430\u0435\u0442\u0441\u044f."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
```

