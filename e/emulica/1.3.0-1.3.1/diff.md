# Comparing `tmp/emulica-1.3.0.tar.gz` & `tmp/emulica-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emulica-1.3.0.tar", last modified: Thu Apr  4 14:47:08 2024, max compression
+gzip compressed data, was "emulica-1.3.1.tar", last modified: Fri Apr  5 13:57:52 2024, max compression
```

## Comparing `emulica-1.3.0.tar` & `emulica-1.3.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    35149 2024-04-04 14:46:54.957282 emulica-1.3.0/LICENSE
--rw-r--r--   0        0        0      760 2024-04-04 14:46:54.957282 emulica-1.3.0/README.md
--rw-r--r--   0        0        0      797 2024-04-04 14:47:08.845246 emulica-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       65 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/__init__.py
--rw-r--r--   0        0        0     1607 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/__init__.py
--rw-r--r--   0        0        0    12161 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/controler.py
--rw-r--r--   0        0        0    28727 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/emuML.py
--rw-r--r--   0        0        0   113659 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/emulation.py
--rw-r--r--   0        0        0    13870 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/plot.py
--rw-r--r--   0        0        0    19947 2024-04-04 14:46:54.957282 emulica-1.3.0/src/emulica/core/properties.py
--rw-r--r--   0        0        0        0 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3062 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/assy.png
--rw-r--r--   0        0        0     1034 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/bad_no_emu.emu
--rw-r--r--   0        0        0     1109 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/bad_no_model.emu
--rw-r--r--   0        0        0     1177 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/bad_no_props.emu
--rw-r--r--   0        0        0     4593 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/cell.emu
--rw-r--r--   0        0        0     2139 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/cell.xml
--rw-r--r--   0        0        0     3079 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/create.png
--rw-r--r--   0        0        0     3004 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/dispose.png
--rw-r--r--   0        0        0     3059 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/holder.png
--rw-r--r--   0        0        0     3226 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/make.png
--rw-r--r--   0        0        0     3319 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/move.png
--rw-r--r--   0        0        0     1711 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/cell.xml
--rw-r--r--   0        0        0      665 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim1.xml
--rw-r--r--   0        0        0     2380 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim14.xml
--rw-r--r--   0        0        0      576 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim15.xml
--rw-r--r--   0        0        0     2080 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim4.xml
--rw-r--r--   0        0        0     2349 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim7.xml
--rw-r--r--   0        0        0      812 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/old-xml/sim8.xml
--rw-r--r--   0        0        0    11355 2024-04-04 14:46:54.957282 emulica-1.3.0/tests/data/plot_gantt1.png
--rw-r--r--   0        0        0    13994 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/plot_holder1.png
--rw-r--r--   0        0        0     8587 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/plot_leg1.png
--rw-r--r--   0        0        0     8093 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/plot_prod1.png
--rw-r--r--   0        0        0    19913 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/plot_prod2.png
--rw-r--r--   0        0        0     1377 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim1.emu
--rw-r--r--   0        0        0     4572 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim1.png
--rw-r--r--   0        0        0      886 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim1.xml
--rw-r--r--   0        0        0     3205 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim14.xml
--rw-r--r--   0        0        0     1282 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim15.emu
--rw-r--r--   0        0        0      763 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim15.xml
--rw-r--r--   0        0        0      884 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim15_bad_submodel.emu
--rw-r--r--   0        0        0      871 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim1_renaming.xml
--rw-r--r--   0        0        0     6494 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim4.emu
--rw-r--r--   0        0        0     3030 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim4.xml
--rw-r--r--   0        0        0    20630 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim6.ods
--rw-r--r--   0        0        0     3332 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim7.xml
--rw-r--r--   0        0        0     1046 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/sim8.xml
--rw-r--r--   0        0        0     3040 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/data/unassy.png
--rw-r--r--   0        0        0      132 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/set_path.py
--rw-r--r--   0        0        0     4945 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_absobs.py
--rw-r--r--   0        0        0     2389 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_bug1.py
--rw-r--r--   0        0        0     2896 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_holderstate.py
--rw-r--r--   0        0        0     2243 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_plot.py
--rw-r--r--   0        0        0     1734 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_server.py
--rw-r--r--   0        0        0     2618 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_setupmatrix.py
--rw-r--r--   0        0        0     4793 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim1.py
--rw-r--r--   0        0        0    10339 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim10.py
--rw-r--r--   0        0        0     2432 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim11.py
--rw-r--r--   0        0        0     3634 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim12.py
--rw-r--r--   0        0        0     2808 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim13.py
--rw-r--r--   0        0        0     7521 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim14.py
--rw-r--r--   0        0        0     7841 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim15.py
--rw-r--r--   0        0        0     7534 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim16.py
--rw-r--r--   0        0        0     8661 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim17.py
--rw-r--r--   0        0        0     1160 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim18.py
--rw-r--r--   0        0        0     7018 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim19.py
--rw-r--r--   0        0        0     3955 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim2.py
--rw-r--r--   0        0        0    12676 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim20.py
--rw-r--r--   0        0        0     6928 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim21.py
--rw-r--r--   0        0        0     4723 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim22.py
--rw-r--r--   0        0        0     7050 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim3.py
--rw-r--r--   0        0        0     7033 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim4.py
--rw-r--r--   0        0        0     8203 2024-04-04 14:46:54.961282 emulica-1.3.0/tests/test_sim5.py
--rw-r--r--   0        0        0     4127 2024-04-04 14:46:54.965282 emulica-1.3.0/tests/test_sim6.py
--rw-r--r--   0        0        0     8271 2024-04-04 14:46:54.965282 emulica-1.3.0/tests/test_sim7.py
--rw-r--r--   0        0        0     5973 2024-04-04 14:46:54.965282 emulica-1.3.0/tests/test_sim8.py
--rw-r--r--   0        0        0     2399 2024-04-04 14:46:54.965282 emulica-1.3.0/tests/test_sim9.py
--rw-r--r--   0        0        0      234 2024-04-04 14:46:54.965282 emulica-1.3.0/tests/util.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 emulica-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 13:57:39.238944 emulica-1.3.1/LICENSE
+-rw-r--r--   0        0        0      760 2024-04-05 13:57:39.238944 emulica-1.3.1/README.md
+-rw-r--r--   0        0        0      797 2024-04-05 13:57:52.855093 emulica-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/__init__.py
+-rw-r--r--   0        0        0     1607 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/__init__.py
+-rw-r--r--   0        0        0    12161 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/controler.py
+-rw-r--r--   0        0        0    28727 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/emuML.py
+-rw-r--r--   0        0        0   113924 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/emulation.py
+-rw-r--r--   0        0        0    13870 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/plot.py
+-rw-r--r--   0        0        0    19947 2024-04-05 13:57:39.238944 emulica-1.3.1/src/emulica/core/properties.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:57:39.238944 emulica-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3062 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/assy.png
+-rw-r--r--   0        0        0     1034 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/bad_no_emu.emu
+-rw-r--r--   0        0        0     1109 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/bad_no_model.emu
+-rw-r--r--   0        0        0     1177 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/bad_no_props.emu
+-rw-r--r--   0        0        0     4593 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/cell.emu
+-rw-r--r--   0        0        0     2139 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/cell.xml
+-rw-r--r--   0        0        0     3079 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/create.png
+-rw-r--r--   0        0        0     3004 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/dispose.png
+-rw-r--r--   0        0        0     3059 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/holder.png
+-rw-r--r--   0        0        0     3226 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/make.png
+-rw-r--r--   0        0        0     3319 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/move.png
+-rw-r--r--   0        0        0     1711 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/cell.xml
+-rw-r--r--   0        0        0      665 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim1.xml
+-rw-r--r--   0        0        0     2380 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim14.xml
+-rw-r--r--   0        0        0      576 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim15.xml
+-rw-r--r--   0        0        0     2080 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim4.xml
+-rw-r--r--   0        0        0     2349 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim7.xml
+-rw-r--r--   0        0        0      812 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/old-xml/sim8.xml
+-rw-r--r--   0        0        0    11355 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/plot_gantt1.png
+-rw-r--r--   0        0        0    13994 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/plot_holder1.png
+-rw-r--r--   0        0        0     8587 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/plot_leg1.png
+-rw-r--r--   0        0        0     8093 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/plot_prod1.png
+-rw-r--r--   0        0        0    19913 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/plot_prod2.png
+-rw-r--r--   0        0        0     1377 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim1.emu
+-rw-r--r--   0        0        0     4572 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim1.png
+-rw-r--r--   0        0        0      886 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim1.xml
+-rw-r--r--   0        0        0     3205 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim14.xml
+-rw-r--r--   0        0        0     1282 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim15.emu
+-rw-r--r--   0        0        0      763 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim15.xml
+-rw-r--r--   0        0        0      884 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim15_bad_submodel.emu
+-rw-r--r--   0        0        0      871 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim1_renaming.xml
+-rw-r--r--   0        0        0     6494 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim4.emu
+-rw-r--r--   0        0        0     3030 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim4.xml
+-rw-r--r--   0        0        0    20630 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim6.ods
+-rw-r--r--   0        0        0     3332 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim7.xml
+-rw-r--r--   0        0        0     1046 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/sim8.xml
+-rw-r--r--   0        0        0     3040 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/data/unassy.png
+-rw-r--r--   0        0        0      132 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/set_path.py
+-rw-r--r--   0        0        0     4945 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_absobs.py
+-rw-r--r--   0        0        0     2389 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_bug1.py
+-rw-r--r--   0        0        0     2896 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_holderstate.py
+-rw-r--r--   0        0        0     2243 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_plot.py
+-rw-r--r--   0        0        0     1734 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_server.py
+-rw-r--r--   0        0        0     2618 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_setupmatrix.py
+-rw-r--r--   0        0        0     4793 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_sim1.py
+-rw-r--r--   0        0        0    10339 2024-04-05 13:57:39.242944 emulica-1.3.1/tests/test_sim10.py
+-rw-r--r--   0        0        0     2432 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim11.py
+-rw-r--r--   0        0        0     3634 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim12.py
+-rw-r--r--   0        0        0     2808 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim13.py
+-rw-r--r--   0        0        0     7521 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim14.py
+-rw-r--r--   0        0        0     7841 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim15.py
+-rw-r--r--   0        0        0     7534 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim16.py
+-rw-r--r--   0        0        0     8661 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim17.py
+-rw-r--r--   0        0        0     1160 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim18.py
+-rw-r--r--   0        0        0     7018 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim19.py
+-rw-r--r--   0        0        0     3955 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim2.py
+-rw-r--r--   0        0        0    12676 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim20.py
+-rw-r--r--   0        0        0     6928 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim21.py
+-rw-r--r--   0        0        0     4723 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim22.py
+-rw-r--r--   0        0        0     7050 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim3.py
+-rw-r--r--   0        0        0     7033 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim4.py
+-rw-r--r--   0        0        0     8203 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim5.py
+-rw-r--r--   0        0        0     4127 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim6.py
+-rw-r--r--   0        0        0     8271 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim7.py
+-rw-r--r--   0        0        0     5973 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim8.py
+-rw-r--r--   0        0        0     2399 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/test_sim9.py
+-rw-r--r--   0        0        0      234 2024-04-05 13:57:39.246944 emulica-1.3.1/tests/util.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 emulica-1.3.1/PKG-INFO
```

### Comparing `emulica-1.3.0/LICENSE` & `emulica-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/README.md` & `emulica-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/pyproject.toml` & `emulica-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "emulica"
-version = "1.3.0"
+version = "1.3.1"
 description = "Emulation of logistic systems"
 authors = [
     { name = "Rémi Pannequin", email = "remi.pannequin@univ-lorraine.fr" },
 ]
 dependencies = [
     "matplotlib",
     "simpy>4.0.0",
```

### Comparing `emulica-1.3.0/src/emulica/core/__init__.py` & `emulica-1.3.1/src/emulica/core/__init__.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/src/emulica/core/controler.py` & `emulica-1.3.1/src/emulica/core/controler.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/src/emulica/core/emuML.py` & `emulica-1.3.1/src/emulica/core/emuML.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/src/emulica/core/emulation.py` & `emulica-1.3.1/src/emulica/core/emulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1193,26 +1193,29 @@
                 if 'productType' in request_cmd.how.keys():
                     prod_type = request_cmd.how['productType']
                 else:
                     prod_type = 'defaulType'
                 module.quantity_created += 1
                 module.emit(Module.STATE_CHANGE_SIGNAL, prod_type)
                 prod = Product(module.model, pid, prod_type)
-                #Set physical properties of the product
+                # Set physical properties of the product
                 for (prop, value) in module.properties['product_prop'].items():
                     prod[prop] = value
                 if 'physical-properties' in request_cmd.how.keys():
                     for (prop, value) in request_cmd.how['physical-properties'].items():
                         if prop in module.properties['product_prop'].keys():
                             logger.warning(_("""physical property {0} from create request supersedes property from module""").format(prop))
                         prod[prop] = value
                 if request_cmd.what == CreateAct.produce_keyword:
                     for ev in module.properties['destination'].put_product(prod):
                         yield ev
-                    report = Report(module.fullname(), 'create-done', date=self.env.now)
+                    report = Report(module.fullname(),
+                                    'create-done',
+                                    date=self.env.now,
+                                    params=request_cmd.how)
                     yield module.report_socket.put(report)
 
 
 class DisposeAct(Actuator):
     """A dispose actuator fetch product from a Holder when requested, and dispose it.
 
     Attributes:
@@ -1251,15 +1254,18 @@
                     yield self.env.timeout(request_cmd.when - now)
                 if request_cmd.what == DisposeAct.produce_keyword:
                     lock_rq = module.properties['source'].lock.request()
                     yield lock_rq
                     prod = module.properties['source'].fetch_product()
                     prod.dispose()
                     module.properties['source'].lock.release(lock_rq)
-                    report = Report(module.fullname(), 'dispose-done', date=self.env.now)
+                    report = Report(module.fullname(),
+                                    'dispose-done',
+                                    date=self.env.now,
+                                    params=request_cmd.how)
                     yield module.report_socket.put(report)
                     module.emit(Module.STATE_CHANGE_SIGNAL, None)
 
 
 class SpaceAct(Actuator):
     """This actuator change the position of a product.
     It is configured with a program_table (i.e. a dictionary that associate
```

### Comparing `emulica-1.3.0/src/emulica/core/plot.py` & `emulica-1.3.1/src/emulica/core/plot.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/src/emulica/core/properties.py` & `emulica-1.3.1/src/emulica/core/properties.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/assy.png` & `emulica-1.3.1/tests/data/assy.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/bad_no_emu.emu` & `emulica-1.3.1/tests/data/bad_no_emu.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/bad_no_model.emu` & `emulica-1.3.1/tests/data/bad_no_model.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/bad_no_props.emu` & `emulica-1.3.1/tests/data/bad_no_props.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/cell.emu` & `emulica-1.3.1/tests/data/cell.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/cell.xml` & `emulica-1.3.1/tests/data/cell.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/create.png` & `emulica-1.3.1/tests/data/create.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/dispose.png` & `emulica-1.3.1/tests/data/dispose.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/holder.png` & `emulica-1.3.1/tests/data/holder.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/make.png` & `emulica-1.3.1/tests/data/make.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/move.png` & `emulica-1.3.1/tests/data/move.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/cell.xml` & `emulica-1.3.1/tests/data/old-xml/cell.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim1.xml` & `emulica-1.3.1/tests/data/old-xml/sim1.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim14.xml` & `emulica-1.3.1/tests/data/old-xml/sim14.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim15.xml` & `emulica-1.3.1/tests/data/old-xml/sim15.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim4.xml` & `emulica-1.3.1/tests/data/old-xml/sim4.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim7.xml` & `emulica-1.3.1/tests/data/old-xml/sim7.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/old-xml/sim8.xml` & `emulica-1.3.1/tests/data/old-xml/sim8.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/plot_gantt1.png` & `emulica-1.3.1/tests/data/plot_gantt1.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/plot_holder1.png` & `emulica-1.3.1/tests/data/plot_holder1.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/plot_leg1.png` & `emulica-1.3.1/tests/data/plot_leg1.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/plot_prod1.png` & `emulica-1.3.1/tests/data/plot_prod1.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/plot_prod2.png` & `emulica-1.3.1/tests/data/plot_prod2.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim1.emu` & `emulica-1.3.1/tests/data/sim1.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim1.png` & `emulica-1.3.1/tests/data/sim1.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim1.xml` & `emulica-1.3.1/tests/data/sim1.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim14.xml` & `emulica-1.3.1/tests/data/sim14.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim15.emu` & `emulica-1.3.1/tests/data/sim15.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim15.xml` & `emulica-1.3.1/tests/data/sim15.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim15_bad_submodel.emu` & `emulica-1.3.1/tests/data/sim15_bad_submodel.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim1_renaming.xml` & `emulica-1.3.1/tests/data/sim1_renaming.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim4.emu` & `emulica-1.3.1/tests/data/sim4.emu`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim4.xml` & `emulica-1.3.1/tests/data/sim4.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim6.ods` & `emulica-1.3.1/tests/data/sim6.ods`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim7.xml` & `emulica-1.3.1/tests/data/sim7.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/sim8.xml` & `emulica-1.3.1/tests/data/sim8.xml`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/data/unassy.png` & `emulica-1.3.1/tests/data/unassy.png`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_absobs.py` & `emulica-1.3.1/tests/test_absobs.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_bug1.py` & `emulica-1.3.1/tests/test_bug1.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_holderstate.py` & `emulica-1.3.1/tests/test_holderstate.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_plot.py` & `emulica-1.3.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_server.py` & `emulica-1.3.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_setupmatrix.py` & `emulica-1.3.1/tests/test_setupmatrix.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim1.py` & `emulica-1.3.1/tests/test_sim1.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim10.py` & `emulica-1.3.1/tests/test_sim10.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim11.py` & `emulica-1.3.1/tests/test_sim11.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim12.py` & `emulica-1.3.1/tests/test_sim12.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim13.py` & `emulica-1.3.1/tests/test_sim13.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim14.py` & `emulica-1.3.1/tests/test_sim14.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim15.py` & `emulica-1.3.1/tests/test_sim15.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim16.py` & `emulica-1.3.1/tests/test_sim16.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim17.py` & `emulica-1.3.1/tests/test_sim17.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim18.py` & `emulica-1.3.1/tests/test_sim18.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim19.py` & `emulica-1.3.1/tests/test_sim19.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim2.py` & `emulica-1.3.1/tests/test_sim2.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim20.py` & `emulica-1.3.1/tests/test_sim20.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim21.py` & `emulica-1.3.1/tests/test_sim21.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim22.py` & `emulica-1.3.1/tests/test_sim22.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim3.py` & `emulica-1.3.1/tests/test_sim3.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim4.py` & `emulica-1.3.1/tests/test_sim4.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim5.py` & `emulica-1.3.1/tests/test_sim5.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim6.py` & `emulica-1.3.1/tests/test_sim6.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim7.py` & `emulica-1.3.1/tests/test_sim7.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim8.py` & `emulica-1.3.1/tests/test_sim8.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/tests/test_sim9.py` & `emulica-1.3.1/tests/test_sim9.py`

 * *Files identical despite different names*

### Comparing `emulica-1.3.0/PKG-INFO` & `emulica-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emulica
-Version: 1.3.0
+Version: 1.3.1
 Summary: Emulation of logistic systems
 Author-Email: Rémi Pannequin <remi.pannequin@univ-lorraine.fr>
 License: GPL-3
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

