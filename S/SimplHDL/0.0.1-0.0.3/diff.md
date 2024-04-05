# Comparing `tmp/SimplHDL-0.0.1.tar.gz` & `tmp/SimplHDL-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimplHDL-0.0.1.tar", last modified: Wed Jul 26 17:42:47 2023, max compression
+gzip compressed data, was "SimplHDL-0.0.3.tar", last modified: Fri Apr  5 12:19:54 2024, max compression
```

## Comparing `SimplHDL-0.0.1.tar` & `SimplHDL-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.430406 SimplHDL-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-26 17:42:47.430406 SimplHDL-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:42:47.430406 SimplHDL-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.422406 SimplHDL-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.426406 SimplHDL-0.0.1/src/SimplHDL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 17:42:47.000000 SimplHDL-0.0.1/src/SimplHDL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.426406 SimplHDL-0.0.1/src/simplhdl/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.426406 SimplHDL-0.0.1/src/simplhdl/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/parsers/fusesocparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/parsers/importlistparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/src/simplhdl/simplhdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:47.426406 SimplHDL-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 17:42:35.000000 SimplHDL-0.0.1/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    50717 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111558 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_light_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/drawing.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/docs/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/ghdl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/icarus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/quartus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/questasim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/vivado.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/xsim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/intel-ips.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/adder.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/hdl/adder.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/sim/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/sim/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/timing.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/top.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/alu.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/add.sv
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/alu.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/mul.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/sub.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/examples/hdl/alu/sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/aluif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/clockif.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/pyuvm.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/seq_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/agent.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/driver.svh
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/env.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/add_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/tb_env.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/tb_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/alu_if.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/test_add/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/test_add/test_add.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/timing.xdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/build.sbt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/hello.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/hello/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/hello/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/src/main/scala/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/src/main/scala/Hello.scala
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/syn/build.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/plugins/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/plugins/simple_parser/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/simple_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/src/SimplHDL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/implementationflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/modelsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/quartusflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/questasim/questasimflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/rivieraproflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/simulationflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vcs/vcsflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vivadoflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/xsim/xsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/chisel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/ipxact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/spd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/systemrdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/fusesocparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/simplhdlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/pyedaa/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/vhdllibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/run.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/pli.tab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/launch_run.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/run.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/steps.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/simplhdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/tox.ini
```

### Comparing `SimplHDL-0.0.1/src/simplhdl/parser.py` & `SimplHDL-0.0.3/src/simplhdl/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from pathlib import Path
 from typing import Callable
 from abc import ABCMeta, abstractmethod
-from pyEDAA.ProjectModel import FileSet  # type: ignore
+from argparse import Namespace
+
+from .pyedaa.fileset import FileSet
+from .pyedaa.project import Project
 
 
 class ParserBase(metaclass=ABCMeta):
 
-    def __init__(self, **kwargs):
+    def __init__(self):
         pass
 
     @abstractmethod
     def is_valid_format(self, filename: Path) -> bool:
         pass
 
     @abstractmethod
-    def parse(self, filename: Path) -> 'FileSet':
+    def parse(self, filename: Path, project: Project, args: Namespace) -> 'FileSet':
         pass
 
 
 class ParserFactory:
     """
     Factory for creating parsers
     """
@@ -34,13 +37,20 @@
                 raise Exception(f"Parser {name} already exists.")
             cls.registry[name] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
-    def get_parser(cls, filename: Path, **kwargs) -> 'ParserBase':
+    def get_parser(cls, filename: Path) -> 'ParserBase':
         for parser_class in cls.registry.values():
-            parser = parser_class(**kwargs)
+            parser = parser_class()
             if parser.is_valid_format(filename):
                 return parser
-        raise Exception(f"Couldn't find Parser for parsing {filename}")
+        if filename is None:
+            raise ParserError("Couldn't find Parser for parsing, try using the --projectspec <filename>")
+        else:
+            raise ParserError(f"Couldn't find Parser for parsing '{filename}'")
+
+
+class ParserError(Exception):
+    pass
```

