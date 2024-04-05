# Comparing `tmp/mpi4jax-0.4.0.post5.tar.gz` & `tmp/mpi4jax-0.4.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi4jax-0.4.0.post5.tar", last modified: Wed Feb 28 09:00:06 2024, max compression
+gzip compressed data, was "mpi4jax-0.4.0.post6.tar", last modified: Fri Apr  5 16:03:31 2024, max compression
```

## Comparing `mpi4jax-0.4.0.post5.tar` & `mpi4jax-0.4.0.post6.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.871032 mpi4jax-0.4.0.post5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/examples/shallow_water.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/mpi4jax/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.871032 mpi4jax-0.4.0.post5/mpi4jax/_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/_latest_jax_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.875032 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.875032 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/mpi4jax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.875032 mpi4jax-0.4.0.post5/mpi4jax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.875032 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.879032 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/mpi4jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-28 09:00:06.000000 mpi4jax-0.4.0.post5/mpi4jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.879032 mpi4jax-0.4.0.post5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/tests/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_allreduce_matvec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_send_and_recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/collective_ops/test_sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:00:06.883032 mpi4jax-0.4.0.post5/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/experimental/test_notoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_has_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-02-28 08:59:02.000000 mpi4jax-0.4.0.post5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.363869 mpi4jax-0.4.0.post6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/examples/shallow_water.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/mpi4jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.367869 mpi4jax-0.4.0.post6/mpi4jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/_latest_jax_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/mpi4jax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/mpi4jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_send_and_recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/experimental/test_notoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_has_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/versioneer.py
```

### Comparing `mpi4jax-0.4.0.post5/LICENSE.md` & `mpi4jax-0.4.0.post6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/PKG-INFO` & `mpi4jax-0.4.0.post6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.0.post5
+Version: 0.4.0.post6
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.0.post5/README.rst` & `mpi4jax-0.4.0.post6/README.rst`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/examples/shallow_water.py` & `mpi4jax-0.4.0.post6/examples/shallow_water.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/__init__.py` & `mpi4jax-0.4.0.post6/mpi4jax/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/__init__.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/allgather.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/allreduce.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/alltoall.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/barrier.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/bcast.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/gather.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/recv.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/reduce.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/scan.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/scatter.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/send.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/send.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/collective_ops/sendrecv.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/decorators.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/decorators.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/jax_compat.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/utils.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/validation.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/__init__.py` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx` & `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/__init__.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/allgather.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/allreduce.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/alltoall.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/barrier.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/bcast.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/gather.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/recv.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/reduce.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/scan.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/scatter.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/send.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/send.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax/experimental/notoken/collective_ops/sendrecv.py` & `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/mpi4jax.egg-info/PKG-INFO` & `mpi4jax-0.4.0.post6/mpi4jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.0.post5
+Version: 0.4.0.post6
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.0.post5/mpi4jax.egg-info/SOURCES.txt` & `mpi4jax-0.4.0.post6/mpi4jax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/pyproject.toml` & `mpi4jax-0.4.0.post6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/setup.py` & `mpi4jax-0.4.0.post6/setup.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_allgather.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_allreduce.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_allreduce_matvec.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce_matvec.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_alltoall.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_barrier.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_bcast.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_common.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_common.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_gather.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_reduce.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_scan.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_scatter.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_send_and_recv.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_send_and_recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/collective_ops/test_sendrecv.py` & `mpi4jax-0.4.0.post6/tests/collective_ops/test_sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/experimental/test_notoken.py` & `mpi4jax-0.4.0.post6/tests/experimental/test_notoken.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/test_decorators.py` & `mpi4jax-0.4.0.post6/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/test_jax_compat.py` & `mpi4jax-0.4.0.post6/tests/test_jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/tests/test_validation.py` & `mpi4jax-0.4.0.post6/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post5/versioneer.py` & `mpi4jax-0.4.0.post6/versioneer.py`

 * *Files identical despite different names*

