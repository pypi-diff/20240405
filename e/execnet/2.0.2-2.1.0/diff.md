# Comparing `tmp/execnet-2.0.2.tar.gz` & `tmp/execnet-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  9 15:04:38 2023, max compression
+gzip compressed data, last modified: Fri Apr  5 18:23:17 2024, max compression
```

## Comparing `execnet-2.0.2.tar` & `execnet-2.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      603 2023-07-09 15:04:38.000000 execnet-2.0.2/tox.ini
--rw-r--r--   0        0        0     3197 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/Makefile
--rw-r--r--   0        0        0        2 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/__init__.py
--rw-r--r--   0        0        0     8213 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/basics.rst
--rw-r--r--   0        0        0       98 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/changelog.rst
--rw-r--r--   0        0        0     6160 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/conf.py
--rw-r--r--   0        0        0      603 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/examples.rst
--rw-r--r--   0        0        0     1240 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/implnotes.rst
--rw-r--r--   0        0        0     3374 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/index.rst
--rw-r--r--   0        0        0      798 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/install.rst
--rw-r--r--   0        0        0      726 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/support.rst
--rw-r--r--   0        0        0    24123 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/basic1.png
--rw-r--r--   0        0        0    10202 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/codespeak.png
--rw-r--r--   0        0        0    36750 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/execnet.png
--rw-r--r--   0        0        0    17805 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/pythonring.png
--rw-r--r--   0        0        0      806 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_templates/indexsidebar.html
--rw-r--r--   0        0        0     1298 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_templates/layout.html
--rw-r--r--   0        0        0      379 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/conftest.py
--rw-r--r--   0        0        0      342 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/funcmultiplier.py
--rw-r--r--   0        0        0     4844 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/hybridpython.rst
--rw-r--r--   0        0        0      953 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/popen_read_multiple.py
--rw-r--r--   0        0        0      392 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/py3topy2.py
--rw-r--r--   0        0        0      671 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/redirect_remote_output.py
--rw-r--r--   0        0        0      142 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/remote1.py
--rw-r--r--   0        0        0      279 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/remotecmd.py
--rw-r--r--   0        0        0      243 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/servefiles.py
--rw-r--r--   0        0        0     3886 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/svn-sync-repo.py
--rw-r--r--   0        0        0     4859 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/sysinfo.py
--rw-r--r--   0        0        0     1348 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/taskserver.py
--rw-r--r--   0        0        0     2003 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_debug.rst
--rw-r--r--   0        0        0       47 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_funcmultiplier.py
--rw-r--r--   0        0        0     3504 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_group.rst
--rw-r--r--   0        0        0     6301 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_info.rst
--rw-r--r--   0        0        0     2990 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_multi.rst
--rw-r--r--   0        0        0      741 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_proxy.rst
--rw-r--r--   0        0        0      574 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_ssh_fileserver.rst
--rw-r--r--   0        0        0      958 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/__init__.py
--rw-r--r--   0        0        0      160 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/_version.py
--rw-r--r--   0        0        0     7115 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway.py
--rw-r--r--   0        0        0    51114 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_base.py
--rw-r--r--   0        0        0     2990 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_bootstrap.py
--rw-r--r--   0        0        0     6836 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_io.py
--rw-r--r--   0        0        0     2501 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_socket.py
--rw-r--r--   0        0        0    10291 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/multi.py
--rw-r--r--   0        0        0     7611 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/rsync.py
--rw-r--r--   0        0        0     3828 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/rsync_remote.py
--rw-r--r--   0        0        0     1788 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/xspec.py
--rw-r--r--   0        0        0        2 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/__init__.py
--rw-r--r--   0        0        0      418 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/loop_socketserver.py
--rw-r--r--   0        0        0      306 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/quitserver.py
--rw-r--r--   0        0        0     2480 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/shell.py
--rw-r--r--   0        0        0     3696 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/socketserver.py
--rw-r--r--   0        0        0     3044 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/socketserverservice.py
--rw-r--r--   0        0        0      186 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/xx.py
--rw-r--r--   0        0        0     5476 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/conftest.py
--rw-r--r--   0        0        0    11537 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_basics.py
--rw-r--r--   0        0        0    11840 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_channel.py
--rw-r--r--   0        0        0      839 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_compatibility_regressions.py
--rw-r--r--   0        0        0    16362 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_gateway.py
--rw-r--r--   0        0        0     7526 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_multi.py
--rw-r--r--   0        0        0     9731 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_rsync.py
--rw-r--r--   0        0        0     3621 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_serializer.py
--rw-r--r--   0        0        0     4028 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_termination.py
--rw-r--r--   0        0        0     4890 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_threadpool.py
--rw-r--r--   0        0        0     8636 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_xspec.py
--rw-r--r--   0        0        0      188 2023-07-09 15:04:38.000000 execnet-2.0.2/.gitignore
--rw-r--r--   0        0        0     1054 2023-07-09 15:04:38.000000 execnet-2.0.2/LICENSE
--rw-r--r--   0        0        0     1593 2023-07-09 15:04:38.000000 execnet-2.0.2/README.rst
--rw-r--r--   0        0        0     1559 2023-07-09 15:04:38.000000 execnet-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2923 2023-07-09 15:04:38.000000 execnet-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-04-05 18:23:17.000000 execnet-2.1.0/tox.ini
+-rw-r--r--   0        0        0     3197 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/Makefile
+-rw-r--r--   0        0        0        2 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/__init__.py
+-rw-r--r--   0        0        0     8005 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/basics.rst
+-rw-r--r--   0        0        0       98 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/changelog.rst
+-rw-r--r--   0        0        0     6478 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/conf.py
+-rw-r--r--   0        0        0      603 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/examples.rst
+-rw-r--r--   0        0        0     1239 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/implnotes.rst
+-rw-r--r--   0        0        0     3308 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/index.rst
+-rw-r--r--   0        0        0      798 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/install.rst
+-rw-r--r--   0        0        0      726 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/support.rst
+-rw-r--r--   0        0        0    24123 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/basic1.png
+-rw-r--r--   0        0        0    10202 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/codespeak.png
+-rw-r--r--   0        0        0    36750 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/execnet.png
+-rw-r--r--   0        0        0    17805 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_static/pythonring.png
+-rw-r--r--   0        0        0      806 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_templates/indexsidebar.html
+-rw-r--r--   0        0        0      843 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/_templates/layout.html
+-rw-r--r--   0        0        0      379 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/funcmultiplier.py
+-rw-r--r--   0        0        0     4844 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/hybridpython.rst
+-rw-r--r--   0        0        0      954 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/popen_read_multiple.py
+-rw-r--r--   0        0        0      392 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/py3topy2.py
+-rw-r--r--   0        0        0      702 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/redirect_remote_output.py
+-rw-r--r--   0        0        0      142 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/remote1.py
+-rw-r--r--   0        0        0      279 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/remotecmd.py
+-rw-r--r--   0        0        0      243 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/servefiles.py
+-rw-r--r--   0        0        0     3887 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/svn-sync-repo.py
+-rw-r--r--   0        0        0     4858 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/sysinfo.py
+-rw-r--r--   0        0        0     1348 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/taskserver.py
+-rw-r--r--   0        0        0     2003 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_debug.rst
+-rw-r--r--   0        0        0       47 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_funcmultiplier.py
+-rw-r--r--   0        0        0     3501 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_group.rst
+-rw-r--r--   0        0        0     6271 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_info.rst
+-rw-r--r--   0        0        0     2990 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_multi.rst
+-rw-r--r--   0        0        0      746 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_proxy.rst
+-rw-r--r--   0        0        0      573 2024-04-05 18:23:17.000000 execnet-2.1.0/doc/example/test_ssh_fileserver.rst
+-rw-r--r--   0        0        0     1157 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/_version.py
+-rw-r--r--   0        0        0     7783 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway.py
+-rw-r--r--   0        0        0    59128 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_base.py
+-rw-r--r--   0        0        0     2770 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_bootstrap.py
+-rw-r--r--   0        0        0     8052 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_io.py
+-rw-r--r--   0        0        0     2956 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/gateway_socket.py
+-rw-r--r--   0        0        0    11714 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/multi.py
+-rw-r--r--   0        0        0        0 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/py.typed
+-rw-r--r--   0        0        0     8874 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/rsync.py
+-rw-r--r--   0        0        0     4208 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/rsync_remote.py
+-rw-r--r--   0        0        0     2256 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/xspec.py
+-rw-r--r--   0        0        0        2 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/__init__.py
+-rw-r--r--   0        0        0      418 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/loop_socketserver.py
+-rw-r--r--   0        0        0      304 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/quitserver.py
+-rw-r--r--   0        0        0     2601 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/shell.py
+-rw-r--r--   0        0        0     3935 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/socketserver.py
+-rw-r--r--   0        0        0     3181 2024-04-05 18:23:17.000000 execnet-2.1.0/src/execnet/script/socketserverservice.py
+-rw-r--r--   0        0        0     6275 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/conftest.py
+-rw-r--r--   0        0        0    13407 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_basics.py
+-rw-r--r--   0        0        0    12780 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_channel.py
+-rw-r--r--   0        0        0      847 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_compatibility_regressions.py
+-rw-r--r--   0        0        0    21016 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_gateway.py
+-rw-r--r--   0        0        0     8435 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_multi.py
+-rw-r--r--   0        0        0    10438 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_rsync.py
+-rw-r--r--   0        0        0     3767 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_serializer.py
+-rw-r--r--   0        0        0     4785 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_termination.py
+-rw-r--r--   0        0        0     5499 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_threadpool.py
+-rw-r--r--   0        0        0     9218 2024-04-05 18:23:17.000000 execnet-2.1.0/testing/test_xspec.py
+-rw-r--r--   0        0        0      188 2024-04-05 18:23:17.000000 execnet-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1054 2024-04-05 18:23:17.000000 execnet-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1574 2024-04-05 18:23:17.000000 execnet-2.1.0/README.rst
+-rw-r--r--   0        0        0     2901 2024-04-05 18:23:17.000000 execnet-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2905 2024-04-05 18:23:17.000000 execnet-2.1.0/PKG-INFO
```

### Comparing `execnet-2.0.2/tox.ini` & `execnet-2.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist=py{37,38,39,310,311,pypy37},docs,linting
+envlist=py{38,39,310,311,312,pypy38},docs,linting
 isolated_build = true
 
 [testenv]
 usedevelop=true
 setenv =
     PYTHONWARNDEFAULTENCODING = 1
 deps=
```

### Comparing `execnet-2.0.2/doc/Makefile` & `execnet-2.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/basics.rst` & `execnet-2.1.0/doc/basics.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 API in a nutshell
 ==============================================================================
 
 execnet ad-hoc instantiates local and remote Python interpreters.
 Each interpreter is accessible through a **Gateway** which manages
 code and data communication.  **Channels** allow to exchange
 data between the local and the remote end.  **Groups**
-help to manage creation and termination of sub interpreters.
+help to manage creation and termination of sub-interpreters.
 
 .. image:: _static/basic1.png
 
 .. currentmodule:: execnet
 
 Gateways: bootstrapping Python interpreters
 ===================================================
@@ -22,18 +22,18 @@
 
 .. autofunction:: execnet.makegateway(spec)
 
 Here is an example which instantiates a simple Python subprocess::
 
     >>> gateway = execnet.makegateway()
 
-gateways allow to `remote execute code`_ and
+Gateways allow to `remote execute code`_ and
 `exchange data`_ bidirectionally.
 
-examples for valid gateway specifications
+Examples for valid gateway specifications
 -------------------------------------------
 
 * ``ssh=wyvern//python=python3.3//chdir=mycache`` specifies a Python3.3
   interpreter on the host ``wyvern``.  The remote process will have
   ``mycache`` as its current working directory.
 
 * ``ssh=-p 5000 myhost`` makes execnet pass "-p 5000 myhost" arguments
@@ -78,23 +78,23 @@
 
 All gateways offer a simple method to execute source code
 in the instantiated subprocess-interpreter:
 
 .. automethod:: Gateway.remote_exec(source)
 
 It is allowed to pass a module object as source code
-in which case it's source code will be obtained and
+in which case its source code will be obtained and
 get sent for remote execution.  ``remote_exec`` returns
 a channel object whose symmetric counterpart channel
 is available to the remotely executing source.
 
 
 .. method:: Gateway.reconfigure([py2str_as_py3str=True, py3str_as_py2str=False])
 
-    reconfigures the string-coercion behaviour of the gateway
+    Reconfigures the string-coercion behaviour of the gateway
 
 .. _`Channel`:
 .. _`channel-api`:
 
 .. _`exchange data`:
 
 Channels: exchanging data with remote code
@@ -134,22 +134,22 @@
 process-exit, using a small timeout.  This is fine
 for interactive sessions or random scripts which
 you rather like to error out than hang.  If you start many
 processes then you often want to call ``group.terminate()``
 yourself and specify a larger or not timeout.
 
 
-threading models: gevent, eventlet, thread
-===========================================
+threading models: gevent, eventlet, thread, main_thread_only
+====================================================================
 
 .. versionadded:: 1.2 (status: experimental!)
 
-execnet supports "thread", "eventlet" and "gevent" as thread models
-on each of the two sides.  You need to decide which model to use
-before you create any gateways::
+execnet supports "main_thread_only", "thread", "eventlet" and "gevent"
+as thread models on each of the two sides.  You need to decide which
+model to use before you create any gateways::
 
     # content of threadmodel.py
     import execnet
     # locally use "eventlet", remotely use "thread" model
     execnet.set_execmodel("eventlet", "thread")
     gw = execnet.makegateway()
     print (gw)
@@ -160,25 +160,18 @@
 you can execute this little test file::
 
     $ python threadmodel.py
     <Gateway id='gw0' receive-live, eventlet model, 0 active channels>
     <RInfo 'numchannels=0, numexecuting=0, execmodel=thread'>
     1
 
-.. note::
-
-    With python3 you can (as of December 2013) only use the thread model
-    because neither eventlet-0.14.0 nor gevent-1.0 support Python3.
-    When they start to support Python3, execnet will probably just work
-    because it is itself Python3 compatible.
-
 How to execute in the main thread
 ------------------------------------------------
 
-When the remote side of a gateway uses the 'thread' model, execution
+When the remote side of a gateway uses the "thread" model, execution
 will preferably run in the main thread.  This allows GUI loops
 or other code to behave correctly.  If you, however, start multiple
 executions concurrently, they will run in non-main threads.
 
 
 remote_status: get low-level execution info
 ===================================================
@@ -223,15 +216,15 @@
 :EXECNET_DEBUG=1:  write per-process trace-files to ``execnet-debug-PID``
 :EXECNET_DEBUG=2:  perform tracing to stderr (popen-gateway workers will send this to their instantiator)
 
 
 .. _`dumps/loads`:
 .. _`dumps/loads API`:
 
-cross-interpreter serialization of python objects
+Cross-interpreter serialization of Python objects
 =======================================================
 
 .. versionadded:: 1.1
 
 Execnet exposes a function pair which you can safely use to
 store and load values from different Python interpreters
 (e.g. Python2 and Python3, PyPy and Jython). Here is
```

### Comparing `execnet-2.0.2/doc/conf.py` & `execnet-2.1.0/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 release = ".".join(version.split(".")[:2])
 
 # -- General configuration ----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings.
 # They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.doctest"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
@@ -79,14 +83,24 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3", None),
+}
+
+nitpicky = True
+nitpick_ignore = [
+    ("py:class", "execnet.gateway_base.ChannelFileRead"),
+    ("py:class", "execnet.gateway_base.ChannelFileWrite"),
+    ("py:class", "execnet.gateway.Gateway"),
+]
 
 # -- Options for HTML output --------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
 html_theme = "sphinxdoc"
```

### Comparing `execnet-2.0.2/doc/examples.rst` & `execnet-2.1.0/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/implnotes.rst` & `execnet-2.1.0/doc/implnotes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
 gateway_base.py
 ----------------------
 
-the code of this module is sent to the "other side"
+The code of this module is sent to the "other side"
 as a means of bootstrapping a Gateway object
 capable of receiving and executing code,
 and routing data through channels.
 
 Gateways operate on InputOutput objects offering
 a write and a read(n) method.
```

### Comparing `execnet-2.0.2/doc/index.rst` & `execnet-2.1.0/doc/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 .. image:: _static/pythonring.png
    :align: right
 
 
 .. warning::
 
     execnet currently is in maintenance-only mode, mostly because it is still the backend
@@ -13,46 +11,46 @@
 all major computing platforms today.
 
 **execnet** provides a `share-nothing model`_ with `channel-send/receive`_
 communication for distributing execution across many Python interpreters
 across version, platform and network barriers.  It has
 a minimal and fast API targeting the following uses:
 
-* distribute tasks to (many) local or remote CPUs
-* write and deploy hybrid multi-process applications
-* write scripts to administer multiple environments
+* Distribute tasks to (many) local or remote CPUs
+* Write and deploy hybrid multi-process applications
+* Write scripts to administer multiple environments
 
 .. _`channel-send/receive`: http://en.wikipedia.org/wiki/Channel_(programming)
 .. _`share-nothing model`: http://en.wikipedia.org/wiki/Shared_nothing_architecture
 
 
 .. _Python: http://www.python.org
 
 Features
 ------------------
 
-* automatic bootstrapping: no manual remote installation.
+* Automatic bootstrapping: no manual remote installation.
 
-* safe and simple serialization of python builtin
+* Safe and simple serialization of Python builtin
   types for sending/receiving structured data messages.
   (New in 1.1) execnet offers a new :ref:`dumps/loads <dumps/loads>`
   API which allows cross-interpreter compatible serialization
   of Python builtin types.
 
-* flexible communication: synchronous send/receive as well as
+* Flexible communication: synchronous send/receive as well as
   callback/queue mechanisms supported
 
-* easy creation, handling and termination of multiple processes
+* Easy creation, handling and termination of multiple processes
 
-* well tested interactions between CPython 2.5-2.7, CPython-3.3, Jython 2.5.1
+* Well tested interactions between CPython 2.5-2.7, CPython-3.3, Jython 2.5.1
   and PyPy interpreters.
 
-* fully interoperable between Windows and Unix-ish systems.
+* Fully interoperable between Windows and Unix-ish systems.
 
-* many tested :doc:`examples`
+* Many tested :doc:`examples`
 
 Known uses
 -------------------
 
 * `pytest`_ uses it for its `distributed testing`_ mechanism.
 
 * `quora`_ uses it for `connecting CPython and PyPy`_.
@@ -60,15 +58,15 @@
 * Jacob Perkins uses it for his `Distributed NTLK with execnet`_
   project to launch computation processes through ssh.  He also
   compares `disco and execnet`_ in a subsequent post.
 
 * Ronny Pfannschmidt uses it for his `anyvc`_ VCS-abstraction project
   to bridge the Python2/Python3 version gap.
 
-* sysadmins and developers are using it for ad-hoc custom scripting
+* Sysadmins and developers are using it for ad-hoc custom scripting
 
 .. _`quora`: http://quora.com
 .. _`connecting CPython and PyPy`: http://www.quora.com/Quora-Infrastructure/Did-Quoras-switch-to-PyPy-result-in-increased-memory-consumption
 
 .. _`pytest`: https://docs.pytest.org
 .. _`distributed testing`: https://pypi.python.org/pypi/pytest-xdist
 .. _`Distributed NTLK with execnet`: http://streamhacker.com/2009/11/29/distributed-nltk-execnet/
@@ -83,15 +81,14 @@
 Currently there are no plans to improve the project further, being maintained mostly because it is
 used as backend of the popular `pytest-xdist <https://github.com/pytest-dev/pytest-xdist>`__ plugin.
 
 ``execnet`` was conceived originally by `Holger Krekel`_ and is licensed under the MIT license
 since version 1.2.
 
 .. _`basic API`: basics.html
-.. _`actively developed`: https://github.com/pytest-dev/execnet
 .. _`Holger Krekel`: http://twitter.com/hpk42
 
 .. toctree::
    :hidden:
 
    support
    implnotes
```

### Comparing `execnet-2.0.2/doc/install.rst` & `execnet-2.1.0/doc/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Info in a nutshell
 ====================
 
-**Pythons**: 3.7+, PyPy 3
+**Pythons**: 3.8+, PyPy 3
 
 **Operating systems**: Linux, Windows, OSX, Unix
 
 **Distribution names**:
 
 * PyPI name: ``execnet``
 * Redhat Fedora: ``python-execnet``
```

### Comparing `execnet-2.0.2/doc/support.rst` & `execnet-2.1.0/doc/support.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Contact and Support channels
 ------------------------------
 
 If you have interest, questions, issues or suggestions you
 are welcome to:
 
-* join `execnet-dev`_ for general discussions
-* join `execnet-commit`_ to be notified of changes
-* clone the `github repository`_ and submit patches
-* hang out on the #pytest channel on `irc.libera.chat <ircs://irc.libera.chat/#pytest>`_
+* Join `execnet-dev`_ for general discussions
+* Join `execnet-commit`_ to be notified of changes
+* Clone the `github repository`_ and submit patches
+* Hang out on the #pytest channel on `irc.libera.chat <ircs://irc.libera.chat/#pytest>`_
   (using an IRC client, via `webchat <https://web.libera.chat/#pytest>`_,
   or `via Matrix <https://matrix.to/#/%23pytest:libera.chat>`_).
 
 .. _`execnet-dev`: http://mail.python.org/mailman/listinfo/execnet-dev
 .. _`execnet-commit`: http://mail.python.org/mailman/listinfo/execnet-commit
 .. _`github repository`: https://github.com/pytest-dev/execnet
```

### Comparing `execnet-2.0.2/doc/_static/basic1.png` & `execnet-2.1.0/doc/_static/basic1.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/_static/codespeak.png` & `execnet-2.1.0/doc/_static/codespeak.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/_static/execnet.png` & `execnet-2.1.0/doc/_static/execnet.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/_static/pythonring.png` & `execnet-2.1.0/doc/_static/pythonring.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/_templates/indexsidebar.html` & `execnet-2.1.0/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/example/hybridpython.rst` & `execnet-2.1.0/doc/example/hybridpython.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/example/popen_read_multiple.py` & `execnet-2.1.0/doc/example/popen_read_multiple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 example
 
 reading results from possibly blocking code running in sub processes.
 """
+
 import execnet
 
 NUM_PROCESSES = 5
 
 channels = []
 for i in range(NUM_PROCESSES):
     gw = execnet.makegateway()  # or use SSH or socket gateways
```

### Comparing `execnet-2.0.2/doc/example/redirect_remote_output.py` & `execnet-2.1.0/doc/example/redirect_remote_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 showcasing features of the channel object:
 
 - sending a channel over a channel
 - adapting a channel to a file object
 - setting a callback for receiving channel data
 
 """
+
 import execnet
 
 gw = execnet.makegateway()
 
 outchan = gw.remote_exec(
     """
     import sys
@@ -22,15 +23,15 @@
 
 
 # note: callbacks execute in receiver thread!
 def write(data):
     print("received:", repr(data))
 
 
-outchan.setcallback(write)
+outchan.setcallback(write)  # type: ignore[attr-defined]
 
 gw.remote_exec(
     """
     print('hello world')
     print('remote execution ends')
 """
 ).waitclose()
```

### Comparing `execnet-2.0.2/doc/example/svn-sync-repo.py` & `execnet-2.1.0/doc/example/svn-sync-repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 """
 
 small utility for hot-syncing a svn repository through ssh.
 uses execnet.
 
 """
+
 import os
 import pathlib
 import subprocess
 import sys
 
 import execnet
```

### Comparing `execnet-2.0.2/doc/example/sysinfo.py` & `execnet-2.1.0/doc/example/sysinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 sysinfo.py [host1] [host2] [options]
 
 obtain system info from remote machine.
 
 (c) Holger Krekel, MIT license
 """
+
 import optparse
 import re
 import sys
 
 import execnet
 
-
 parser = optparse.OptionParser(usage=__doc__)
 parser.add_option(
     "-f",
     "--sshconfig",
     action="store",
     dest="ssh_config",
     default=None,
@@ -125,15 +125,15 @@
     debug("ERROR", args[0] + ":", *args[1:])
 
 
 def getinfo(sshname, ssh_config=None, loginfo=sys.stdout):
     if ssh_config:
         spec = f"ssh=-F {ssh_config} {sshname}"
     else:
-        spec += "ssh=%s" % sshname
+        spec = "ssh=%s" % sshname
     debug("connecting to", repr(spec))
     try:
         gw = execnet.makegateway(spec)
     except OSError:
         error("could not get sshgatway", sshname)
     else:
         ri = RemoteInfo(gw)
```

### Comparing `execnet-2.0.2/doc/example/taskserver.py` & `execnet-2.1.0/doc/example/taskserver.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/doc/example/test_debug.rst` & `execnet-2.1.0/doc/example/test_debug.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-Debugging execnet / Wire messages
+Debugging execnet / wire messages
 ===============================================================
 
 By setting the environment variable ``EXECNET_DEBUG`` you can
 configure the execnet tracing mechanism:
 
 :EXECNET_DEBUG=1:  write per-process trace-files to ``${TEMPROOT}/execnet-debug-PID``
 :EXECNET_DEBUG=2:  perform tracing to stderr (popen-gateway workers will send this to their instantiator)
```

### Comparing `execnet-2.0.2/doc/example/test_group.rst` & `execnet-2.1.0/doc/example/test_group.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Managing multiple gateways and clusters
 ==================================================
 
 Usings Groups for managing multiple gateways
 ------------------------------------------------------
 
 Use ``execnet.Group`` to manage membership and lifetime of
-of multiple gateways::
+multiple gateways::
 
     >>> import execnet
     >>> group = execnet.Group(['popen'] * 2)
     >>> len(group)
     2
     >>> group
     <Group ['gw0', 'gw1']>
@@ -21,15 +21,15 @@
     True
     >>> group['gw1'] == group[1]
     True
     >>> group.terminate() # exit all member gateways
     >>> group
     <Group []>
 
-Assigning Gateway IDs
+Assigning gateway IDs
 ------------------------------------------------------
 
 All gateways are created as part of a group and receive
 a per-group unique ``id`` after successful initialization.
 Pass an ``id=MYNAME`` part to ``group.makegateway``. Example::
 
     >>> import execnet
@@ -62,35 +62,35 @@
     >>> import execnet
     >>> gw = execnet.makegateway()
     >>> gw in execnet.default_group
     True
     >>> execnet.default_group.defaultspec # used for empty makegateway() calls
     'popen'
 
-Robust Termination of ssh/popen processes
+Robust termination of SSH/popen processes
 -----------------------------------------------
 
 Use ``group.terminate(timeout)`` if you want to terminate
-member gateways and ensure that no local sub processes remain
-you can specify a ``timeout`` after which an attempt at killing
+member gateways and ensure that no local subprocesses remain.
+You can specify a ``timeout`` after which an attempt at killing
 the related process is made::
 
     >>> import execnet
     >>> group = execnet.Group()
     >>> gw = group.makegateway("popen//id=sleeper")
     >>> ch = gw.remote_exec("import time ; time.sleep(2.0)")
     >>> group
     <Group ['sleeper']>
     >>> group.terminate(timeout=1.0)
     >>> group
     <Group []>
 
 execnet aims to provide totally robust termination so if
 you have left-over processes or other termination issues
-please :doc:`report them <../support>`.  thanks!
+please :doc:`report them <../support>`.  Thanks!
 
 
 Using Groups to manage a certain type of gateway
 ------------------------------------------------------
 
 Set ``group.defaultspec`` to determine the default gateway
 specification used by ``group.makegateway()``:
```

### Comparing `execnet-2.0.2/doc/example/test_info.rst` & `execnet-2.1.0/doc/example/test_info.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-basic local and remote communication
-=========================================
+Basic local and remote communication
+====================================
 
 Execute source code in subprocess, communicate through a channel
 -------------------------------------------------------------------
 
 You can instantiate a subprocess gateway, execute code
 in it and bidirectionally send messages::
 
@@ -21,16 +21,16 @@
 
 The initiating and the "other" process work use a `share-nothing
 model`_ and ``channel.send|receive`` are means to pass basic data
 messages between two processes.
 
 .. _`share-nothing model`: http://en.wikipedia.org/wiki/Shared_nothing_architecture
 
-remote-exec a function (avoiding inlined source part I)
--------------------------------------------------------------------
+Remote-exec a function (avoiding inlined source part I)
+-------------------------------------------------------
 
 You can send and remote execute parametrized pure functions like this:
 
 .. include:: funcmultiplier.py
     :literal:
 
 The ``multiplier`` function executes remotely and establishes
@@ -45,16 +45,16 @@
 
 * You will get an explicit error if you try to execute non-pure
   functions, i.e. functions that access any global state (which
   will not be available remotely as we have a share-nothing model
   between the nodes).
 
 
-remote-exec a module (avoiding inlined source part II)
---------------------------------------------------------------
+Remote-exec a module (avoiding inlined source part II)
+------------------------------------------------------
 
 You can pass a module object to ``remote_exec`` in which case
 its source code will be sent.  No dependencies will be transferred
 so the module must be self-contained or only use modules that are
 installed on the "other" side.   Module code can detect if it is
 running in a remote_exec situation by checking for the special
 ``__name__`` attribute.
@@ -82,16 +82,16 @@
     >>> gw = execnet.makegateway()
     >>> ch = gw.remote_exec("import os; channel.send(os.getcwd())")
     >>> res = ch.receive()
     >>> assert res == os.getcwd()
 
 "ssh" gateways default to the login home directory.
 
-Get information from remote ssh account
---------------------------------------------
+Get information from remote SSH account
+---------------------------------------
 
 Use simple execution to obtain information from remote environments::
 
   >>> import execnet, os
   >>> gw = execnet.makegateway("ssh=codespeak.net")
   >>> channel = gw.remote_exec("""
   ...     import sys, os
@@ -139,15 +139,15 @@
     >>> c1.receive()
     'hello'
     >>> c2.receive()
     'world'
 
 
 
-a simple command loop pattern
+A simple command loop pattern
 --------------------------------------------------------------
 
 If you want the remote side to serve a number
 of synchronous function calls into your module
 you can setup a serving loop and write a local protocol.
 
 .. include:: remotecmd.py
@@ -185,10 +185,10 @@
 You can then instruct execnet on your local machine to bootstrap
 itself into the remote socket endpoint::
 
     import execnet
     gw = execnet.makegateway("socket=TARGET-IP:8888")
 
 That's it, you can now use the gateway object just like
-a popen- or ssh-based one.
+a popen- or SSH-based one.
 
 .. include:: test_ssh_fileserver.rst
```

### Comparing `execnet-2.0.2/doc/example/test_multi.rst` & `execnet-2.1.0/doc/example/test_multi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-advanced (multi) channel communication
+Advanced (multi) channel communication
 =====================================================
 
 MultiChannel: container for multiple channels
 ------------------------------------------------------
 
 Use ``execnet.MultiChannel`` to work with multiple channels::
 
@@ -15,15 +15,15 @@
     >>> mch[0] is ch1 and mch[1] is ch2
     True
     >>> ch1 in mch and ch2 in mch
     True
     >>> sum(mch.receive_each())
     3
 
-receive results from sub processes with a Queue
+Receive results from sub processes with a Queue
 -----------------------------------------------------
 
 Use ``MultiChannel.make_receive_queue()`` to get a queue
 from which to obtain results::
 
     >>> ch1 = execnet.makegateway().remote_exec("channel.send(1)")
     >>> ch2 = execnet.makegateway().remote_exec("channel.send(2)")
@@ -48,15 +48,15 @@
     >>> ch.send(1)
     >>> ch.waitclose()
     >>> assert l == [42]
 
 Note that the callback function will be executed in the
 receiver thread and should not block or run for too long.
 
-robustly receive results and termination notification
+Robustly receive results and termination notification
 -----------------------------------------------------
 
 Use ``MultiChannel.make_receive_queue(endmarker)`` to specify
 an object to be put to the queue when the remote side of a channel
 is closed.  The endmarker will also be put to the Queue if the gateway
 is blocked in execution and is terminated/killed::
 
@@ -72,15 +72,15 @@
     ...    chan1, res1 = queue.get()
     ...    assert res1 == 42
     >>> group
     <Group []>
 
 
 
-saturate multiple Hosts and CPUs with tasks to process
+Saturate multiple Hosts and CPUs with tasks to process
 --------------------------------------------------------
 
 If you have multiple CPUs or hosts you can create as many
 gateways and then have a process sit on each CPU and wait
 for a task to proceed.  One complication is that we
 want to ensure clean termination of all processes
 and loose no result.  Here is an example that just uses
```

### Comparing `execnet-2.0.2/doc/example/test_ssh_fileserver.rst` & `execnet-2.1.0/doc/example/test_ssh_fileserver.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 Receive file contents from remote SSH account
 -----------------------------------------------------
 
 Here is some small server code that you can use to retrieve
 contents of remote files:
 
 .. include:: servefiles.py
```

### Comparing `execnet-2.0.2/src/execnet/__init__.py` & `execnet-2.1.0/src/execnet/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,43 +2,51 @@
 execnet
 -------
 
 pure python lib for connecting to local and remote Python Interpreters.
 
 (c) 2012, Holger Krekel and others
 """
+
 from ._version import version as __version__
+from .gateway import Gateway
+from .gateway_base import Channel
 from .gateway_base import DataFormatError
+from .gateway_base import DumpError
+from .gateway_base import LoadError
+from .gateway_base import RemoteError
+from .gateway_base import TimeoutError
 from .gateway_base import dump
 from .gateway_base import dumps
 from .gateway_base import load
 from .gateway_base import loads
-from .gateway_base import RemoteError
-from .gateway_base import TimeoutError
 from .gateway_bootstrap import HostNotFound
-from .multi import default_group
 from .multi import Group
-from .multi import makegateway
 from .multi import MultiChannel
+from .multi import default_group
+from .multi import makegateway
 from .multi import set_execmodel
 from .rsync import RSync
 from .xspec import XSpec
 
-
 __all__ = [
     "__version__",
     "makegateway",
     "set_execmodel",
     "HostNotFound",
     "RemoteError",
     "TimeoutError",
     "XSpec",
+    "Gateway",
     "Group",
     "MultiChannel",
     "RSync",
     "default_group",
+    "Channel",
     "dumps",
+    "dump",
+    "DumpError",
     "loads",
     "load",
-    "dump",
+    "LoadError",
     "DataFormatError",
 ]
```

### Comparing `execnet-2.0.2/src/execnet/gateway.py` & `execnet-2.1.0/src/execnet/gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,137 @@
-"""
-gateway code for initiating popen, socket and ssh connections.
+"""Gateway code for initiating popen, socket and ssh connections.
+
 (c) 2004-2013, Holger Krekel and others
 """
+
+from __future__ import annotations
+
 import inspect
 import linecache
-import os
-import sys
 import textwrap
 import types
-
-import execnet
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import Callable
 
 from . import gateway_base
+from .gateway_base import IO
+from .gateway_base import Channel
 from .gateway_base import Message
-
-importdir = os.path.dirname(os.path.dirname(execnet.__file__))
+from .multi import Group
+from .xspec import XSpec
 
 
 class Gateway(gateway_base.BaseGateway):
     """Gateway to a local or remote Python Interpreter."""
 
-    def __init__(self, io, spec):
+    _group: Group
+
+    def __init__(self, io: IO, spec: XSpec) -> None:
+        """:private:"""
         super().__init__(io=io, id=spec.id, _startcount=1)
         self.spec = spec
         self._initreceive()
 
     @property
-    def remoteaddress(self):
-        return self._io.remoteaddress
+    def remoteaddress(self) -> str:
+        # Only defined for remote IO types.
+        return self._io.remoteaddress  # type: ignore[attr-defined,no-any-return]
 
-    def __repr__(self):
-        """return string representing gateway type and status."""
+    def __repr__(self) -> str:
+        """A string representing gateway type and status."""
         try:
-            r = self.hasreceiver() and "receive-live" or "not-receiving"
-            i = len(self._channelfactory.channels())
+            r: str = self.hasreceiver() and "receive-live" or "not-receiving"
+            i = str(len(self._channelfactory.channels()))
         except AttributeError:
             r = "uninitialized"
             i = "no"
-        return "<{} id={!r} {}, {} model, {} active channels>".format(
-            self.__class__.__name__, self.id, r, self.execmodel.backend, i
-        )
+        return f"<{self.__class__.__name__} id={self.id!r} {r}, {self.execmodel.backend} model, {i} active channels>"
 
-    def exit(self):
-        """trigger gateway exit.  Defer waiting for finishing
-        of receiver-thread and subprocess activity to when
-        group.terminate() is called.
+    def exit(self) -> None:
+        """Trigger gateway exit.
+
+        Defer waiting for finishing of receiver-thread and subprocess activity
+        to when group.terminate() is called.
         """
         self._trace("gateway.exit() called")
         if self not in self._group:
             self._trace("gateway already unregistered with group")
             return
         self._group._unregister(self)
         try:
             self._trace("--> sending GATEWAY_TERMINATE")
             self._send(Message.GATEWAY_TERMINATE)
             self._trace("--> io.close_write")
             self._io.close_write()
-        except (ValueError, EOFError, OSError):
-            v = sys.exc_info()[1]
+        except (ValueError, EOFError, OSError) as exc:
             self._trace("io-error: could not send termination sequence")
-            self._trace(" exception: %r" % v)
+            self._trace(" exception: %r" % exc)
 
-    def reconfigure(self, py2str_as_py3str=True, py3str_as_py2str=False):
-        """
-        set the string coercion for this gateway
-        the default is to try to convert py2 str as py3 str,
-        but not to try and convert py3 str to py2 str
+    def reconfigure(
+        self, py2str_as_py3str: bool = True, py3str_as_py2str: bool = False
+    ) -> None:
+        """Set the string coercion for this gateway.
+
+        The default is to try to convert py2 str as py3 str, but not to try and
+        convert py3 str to py2 str.
         """
         self._strconfig = (py2str_as_py3str, py3str_as_py2str)
         data = gateway_base.dumps_internal(self._strconfig)
         self._send(Message.RECONFIGURE, data=data)
 
-    def _rinfo(self, update=False):
-        """return some sys/env information from remote."""
+    def _rinfo(self, update: bool = False) -> RInfo:
+        """Return some sys/env information from remote."""
         if update or not hasattr(self, "_cache_rinfo"):
             ch = self.remote_exec(rinfo_source)
             try:
                 self._cache_rinfo = RInfo(ch.receive())
             finally:
                 ch.waitclose()
         return self._cache_rinfo
 
-    def hasreceiver(self):
-        """return True if gateway is able to receive data."""
+    def hasreceiver(self) -> bool:
+        """Whether gateway is able to receive data."""
         return self._receivepool.active_count() > 0
 
-    def remote_status(self):
-        """return information object about remote execution status."""
+    def remote_status(self) -> RemoteStatus:
+        """Obtain information about the remote execution status."""
         channel = self.newchannel()
         self._send(Message.STATUS, channel.id)
         statusdict = channel.receive()
         # the other side didn't actually instantiate a channel
         # so we just delete the internal id/channel mapping
         self._channelfactory._local_close(channel.id)
         return RemoteStatus(statusdict)
 
-    def remote_exec(self, source, **kwargs):
-        """return channel object and connect it to a remote
+    def remote_exec(
+        self,
+        source: str | types.FunctionType | Callable[..., object] | types.ModuleType,
+        **kwargs: object,
+    ) -> Channel:
+        """Return channel object and connect it to a remote
         execution thread where the given ``source`` executes.
 
         * ``source`` is a string: execute source string remotely
           with a ``channel`` put into the global namespace.
         * ``source`` is a pure function: serialize source and
           call function with ``**kwargs``, adding a
           ``channel`` object to the keyword arguments.
         * ``source`` is a pure module: execute source of module
-          with a ``channel`` in its global namespace
+          with a ``channel`` in its global namespace.
 
         In all cases the binding ``__name__='__channelexec__'``
         will be available in the global namespace of the remotely
         executing code.
         """
         call_name = None
         file_name = None
         if isinstance(source, types.ModuleType):
             file_name = inspect.getsourcefile(source)
-            linecache.updatecache(file_name)
+            linecache.updatecache(file_name)  # type: ignore[arg-type]
             source = inspect.getsource(source)
         elif isinstance(source, types.FunctionType):
             call_name = source.__name__
             file_name = inspect.getsourcefile(source)
             source = _source_of_function(source)
         else:
             source = textwrap.dedent(str(source))
@@ -131,61 +143,65 @@
         self._send(
             Message.CHANNEL_EXEC,
             channel.id,
             gateway_base.dumps_internal((source, file_name, call_name, kwargs)),
         )
         return channel
 
-    def remote_init_threads(self, num=None):
+    def remote_init_threads(self, num: int | None = None) -> None:
         """DEPRECATED.  Is currently a NO-OPERATION already."""
-        print("WARNING: remote_init_threads()" " is a no-operation in execnet-1.2")
+        print("WARNING: remote_init_threads() is a no-operation in execnet-1.2")
 
 
 class RInfo:
-    def __init__(self, kwargs):
+    def __init__(self, kwargs) -> None:
         self.__dict__.update(kwargs)
 
-    def __repr__(self):
-        info = ", ".join("%s=%s" % item for item in sorted(self.__dict__.items()))
+    def __repr__(self) -> str:
+        info = ", ".join(f"{k}={v}" for k, v in sorted(self.__dict__.items()))
         return "<RInfo %r>" % info
 
+    if TYPE_CHECKING:
+
+        def __getattr__(self, name: str) -> Any: ...
+
 
 RemoteStatus = RInfo
 
 
-def rinfo_source(channel):
-    import sys
+def rinfo_source(channel) -> None:
     import os
+    import sys
 
     channel.send(
         dict(
             executable=sys.executable,
             version_info=sys.version_info[:5],
             platform=sys.platform,
             cwd=os.getcwd(),
             pid=os.getpid(),
         )
     )
 
 
-def _find_non_builtin_globals(source, codeobj):
+def _find_non_builtin_globals(source: str, codeobj: types.CodeType) -> list[str]:
     import ast
     import builtins
 
     vars = dict.fromkeys(codeobj.co_varnames)
     return [
         node.id
         for node in ast.walk(ast.parse(source))
         if isinstance(node, ast.Name)
         and node.id not in vars
         and node.id not in builtins.__dict__
     ]
 
 
-def _source_of_function(function):
+def _source_of_function(function: types.FunctionType | Callable[..., object]) -> str:
     if function.__name__ == "<lambda>":
         raise ValueError("can't evaluate lambda functions'")
     # XXX: we dont check before remote instantiation
     #      if arguments are used properly
     try:
         sig = inspect.getfullargspec(function)
     except AttributeError:
@@ -199,16 +215,16 @@
     codeobj = function.__code__
 
     if closure is not None:
         raise ValueError("functions with closures can't be passed")
 
     try:
         source = inspect.getsource(function)
-    except OSError:
-        raise ValueError("can't find source file for %s" % function)
+    except OSError as e:
+        raise ValueError("can't find source file for %s" % function) from e
 
     source = textwrap.dedent(source)  # just for inner functions
 
     used_globals = _find_non_builtin_globals(source, codeobj)
     if used_globals:
         raise ValueError("the use of non-builtin globals isn't supported", used_globals)
```

### Comparing `execnet-2.0.2/src/execnet/gateway_base.py` & `execnet-2.1.0/src/execnet/gateway_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,81 @@
-"""
-base execnet gateway code send to the other side for bootstrapping.
-
-NOTE: aims to be compatible to Python 2.5-3.X, Jython and IronPython
+"""Base execnet gateway code send to the other side for bootstrapping.
 
 :copyright: 2004-2015
 :authors:
     - Holger Krekel
     - Armin Rigo
     - Benjamin Peterson
     - Ronny Pfannschmidt
     - many others
 """
+
 from __future__ import annotations
 
 import abc
 import os
 import struct
 import sys
 import traceback
 import weakref
 from _thread import interrupt_main
 from io import BytesIO
+from typing import Any
 from typing import Callable
+from typing import Iterator
+from typing import Literal
+from typing import MutableSet
+from typing import Protocol
+from typing import cast
+from typing import overload
+
+
+class WriteIO(Protocol):
+    def write(self, data: bytes, /) -> None: ...
+
+
+class ReadIO(Protocol):
+    def read(self, numbytes: int, /) -> bytes: ...
+
+
+class IO(Protocol):
+    execmodel: ExecModel
+
+    def read(self, numbytes: int, /) -> bytes: ...
+
+    def write(self, data: bytes, /) -> None: ...
+
+    def close_read(self) -> None: ...
+
+    def close_write(self) -> None: ...
+
+    def wait(self) -> int | None: ...
+
+    def kill(self) -> None: ...
+
+
+class Event(Protocol):
+    """Protocol for types which look like threading.Event."""
+
+    def is_set(self) -> bool: ...
+
+    def set(self) -> None: ...
+
+    def clear(self) -> None: ...
+
+    def wait(self, timeout: float | None = None) -> bool: ...
 
 
 class ExecModel(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
-    def backend(self):
+    def backend(self) -> str:
         raise NotImplementedError()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<ExecModel %r>" % self.backend
 
     @property
     @abc.abstractmethod
     def queue(self):
         raise NotImplementedError()
 
@@ -45,39 +86,39 @@
 
     @property
     @abc.abstractmethod
     def socket(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def start(self, func, args=()):
+    def start(self, func, args=()) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def get_ident(self):
+    def get_ident(self) -> int:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def sleep(self, delay):
+    def sleep(self, delay: float) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def fdopen(self, fd, mode, bufsize=1):
+    def fdopen(self, fd, mode, bufsize=1, closefd=True):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def Lock(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def RLock(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def Event(self):
+    def Event(self) -> Event:
         raise NotImplementedError()
 
 
 class ThreadExecModel(ExecModel):
     backend = "thread"
 
     @property
@@ -94,33 +135,33 @@
 
     @property
     def socket(self):
         import socket
 
         return socket
 
-    def get_ident(self):
+    def get_ident(self) -> int:
         import _thread
 
         return _thread.get_ident()
 
-    def sleep(self, delay):
+    def sleep(self, delay: float) -> None:
         import time
 
         time.sleep(delay)
 
-    def start(self, func, args=()):
+    def start(self, func, args=()) -> None:
         import _thread
 
-        return _thread.start_new_thread(func, args)
+        _thread.start_new_thread(func, args)
 
-    def fdopen(self, fd, mode, bufsize=1):
+    def fdopen(self, fd, mode, bufsize=1, closefd=True):
         import os
 
-        return os.fdopen(fd, mode, bufsize, encoding="utf-8")
+        return os.fdopen(fd, mode, bufsize, encoding="utf-8", closefd=closefd)
 
     def Lock(self):
         import threading
 
         return threading.RLock()
 
     def RLock(self):
@@ -130,14 +171,18 @@
 
     def Event(self):
         import threading
 
         return threading.Event()
 
 
+class MainThreadOnlyExecModel(ThreadExecModel):
+    backend = "main_thread_only"
+
+
 class EventletExecModel(ExecModel):
     backend = "eventlet"
 
     @property
     def queue(self):
         import eventlet
 
@@ -151,33 +196,33 @@
 
     @property
     def socket(self):
         import eventlet.green.socket
 
         return eventlet.green.socket
 
-    def get_ident(self):
+    def get_ident(self) -> int:
         import eventlet.green.thread
 
-        return eventlet.green.thread.get_ident()
+        return eventlet.green.thread.get_ident()  # type: ignore[no-any-return]
 
-    def sleep(self, delay):
+    def sleep(self, delay: float) -> None:
         import eventlet
 
         eventlet.sleep(delay)
 
-    def start(self, func, args=()):
+    def start(self, func, args=()) -> None:
         import eventlet
 
-        return eventlet.spawn_n(func, *args)
+        eventlet.spawn_n(func, *args)
 
-    def fdopen(self, fd, mode, bufsize=1):
+    def fdopen(self, fd, mode, bufsize=1, closefd=True):
         import eventlet.green.os
 
-        return eventlet.green.os.fdopen(fd, mode, bufsize)
+        return eventlet.green.os.fdopen(fd, mode, bufsize, closefd=closefd)
 
     def Lock(self):
         import eventlet.green.threading
 
         return eventlet.green.threading.RLock()
 
     def RLock(self):
@@ -208,34 +253,34 @@
 
     @property
     def socket(self):
         import gevent
 
         return gevent.socket
 
-    def get_ident(self):
+    def get_ident(self) -> int:
         import gevent.thread
 
-        return gevent.thread.get_ident()
+        return gevent.thread.get_ident()  # type: ignore[no-any-return]
 
-    def sleep(self, delay):
+    def sleep(self, delay: float) -> None:
         import gevent
 
         gevent.sleep(delay)
 
-    def start(self, func, args=()):
+    def start(self, func, args=()) -> None:
         import gevent
 
-        return gevent.spawn(func, *args)
+        gevent.spawn(func, *args)
 
-    def fdopen(self, fd, mode, bufsize=1):
+    def fdopen(self, fd, mode, bufsize=1, closefd=True):
         # XXX
         import gevent.fileobject
 
-        return gevent.fileobject.FileObjectThread(fd, mode, bufsize)
+        return gevent.fileobject.FileObjectThread(fd, mode, bufsize, closefd=closefd)
 
     def Lock(self):
         import gevent.lock
 
         return gevent.lock.RLock()
 
     def RLock(self):
@@ -245,163 +290,179 @@
 
     def Event(self):
         import gevent.event
 
         return gevent.event.Event()
 
 
-def get_execmodel(backend):
-    if hasattr(backend, "backend"):
+def get_execmodel(backend: str | ExecModel) -> ExecModel:
+    if isinstance(backend, ExecModel):
         return backend
     if backend == "thread":
         return ThreadExecModel()
+    elif backend == "main_thread_only":
+        return MainThreadOnlyExecModel()
     elif backend == "eventlet":
         return EventletExecModel()
     elif backend == "gevent":
         return GeventExecModel()
     else:
         raise ValueError(f"unknown execmodel {backend!r}")
 
 
 class Reply:
-    """reply instances provide access to the result
-    of a function execution that got dispatched
-    through WorkerPool.spawn()
-    """
+    """Provide access to the result of a function execution that got dispatched
+    through WorkerPool.spawn()."""
 
-    def __init__(self, task, threadmodel):
+    def __init__(self, task, threadmodel: ExecModel) -> None:
         self.task = task
         self._result_ready = threadmodel.Event()
         self.running = True
 
-    def get(self, timeout=None):
+    def get(self, timeout: float | None = None):
         """get the result object from an asynchronous function execution.
         if the function execution raised an exception,
         then calling get() will reraise that exception
         including its traceback.
         """
         self.waitfinish(timeout)
         try:
             return self._result
         except AttributeError:
-            raise self._excinfo[1].with_traceback(self._excinfo[2])
+            raise self._exc from None
 
-    def waitfinish(self, timeout=None):
+    def waitfinish(self, timeout: float | None = None) -> None:
         if not self._result_ready.wait(timeout):
             raise OSError(f"timeout waiting for {self.task!r}")
 
-    def run(self):
+    def run(self) -> None:
         func, args, kwargs = self.task
         try:
             try:
                 self._result = func(*args, **kwargs)
-            except BaseException:
-                # sys may be already None when shutting down the interpreter
-                if sys is not None:
-                    self._excinfo = sys.exc_info()
+            except BaseException as exc:
+                self._exc = exc
         finally:
             self._result_ready.set()
             self.running = False
 
 
 class WorkerPool:
     """A WorkerPool allows to spawn function executions
     to threads, returning a reply object on which you
     can ask for the result (and get exceptions reraised).
 
     This implementation allows the main thread to integrate
     itself into performing function execution through
     calling integrate_as_primary_thread() which will return
     when the pool received a trigger_shutdown().
+
+    By default allows unlimited number of spawns.
     """
 
-    def __init__(self, execmodel, hasprimary=False):
-        """by default allow unlimited number of spawns."""
+    _primary_thread_task: Reply | None
+
+    def __init__(self, execmodel: ExecModel, hasprimary: bool = False) -> None:
         self.execmodel = execmodel
         self._running_lock = self.execmodel.Lock()
-        self._running = set()
+        self._running: MutableSet[Reply] = set()
         self._shuttingdown = False
-        self._waitall_events = []
+        self._waitall_events: list[Event] = []
         if hasprimary:
-            if self.execmodel.backend != "thread":
+            if self.execmodel.backend not in ("thread", "main_thread_only"):
                 raise ValueError("hasprimary=True requires thread model")
-            self._primary_thread_task_ready = self.execmodel.Event()
+            self._primary_thread_task_ready: Event | None = self.execmodel.Event()
         else:
             self._primary_thread_task_ready = None
 
-    def integrate_as_primary_thread(self):
-        """integrate the thread with which we are called as a primary
-        thread for executing functions triggered with spawn().
-        """
-        assert self.execmodel.backend == "thread", self.execmodel
+    def integrate_as_primary_thread(self) -> None:
+        """Integrate the thread with which we are called as a primary
+        thread for executing functions triggered with spawn()."""
+        assert self.execmodel.backend in ("thread", "main_thread_only"), self.execmodel
         primary_thread_task_ready = self._primary_thread_task_ready
+        assert primary_thread_task_ready is not None
         # interacts with code at REF1
         while 1:
             primary_thread_task_ready.wait()
             reply = self._primary_thread_task
             if reply is None:  # trigger_shutdown() woke us up
                 break
             self._perform_spawn(reply)
             # we are concurrent with trigger_shutdown and spawn
             with self._running_lock:
                 if self._shuttingdown:
                     break
-                primary_thread_task_ready.clear()
+                # Only clear if _try_send_to_primary_thread has not
+                # yet set the next self._primary_thread_task reply
+                # after waiting for this one to complete.
+                if reply is self._primary_thread_task:
+                    primary_thread_task_ready.clear()
 
-    def trigger_shutdown(self):
+    def trigger_shutdown(self) -> None:
         with self._running_lock:
             self._shuttingdown = True
             if self._primary_thread_task_ready is not None:
                 self._primary_thread_task = None
                 self._primary_thread_task_ready.set()
 
-    def active_count(self):
+    def active_count(self) -> int:
         return len(self._running)
 
-    def _perform_spawn(self, reply):
+    def _perform_spawn(self, reply: Reply) -> None:
         reply.run()
         with self._running_lock:
             self._running.remove(reply)
             if not self._running:
                 while self._waitall_events:
                     waitall_event = self._waitall_events.pop()
                     waitall_event.set()
 
-    def _try_send_to_primary_thread(self, reply):
+    def _try_send_to_primary_thread(self, reply: Reply) -> bool:
         # REF1 in 'thread' model we give priority to running in main thread
         # note that we should be called with _running_lock hold
         primary_thread_task_ready = self._primary_thread_task_ready
         if primary_thread_task_ready is not None:
             if not primary_thread_task_ready.is_set():
                 self._primary_thread_task = reply
                 # wake up primary thread
                 primary_thread_task_ready.set()
                 return True
+            elif (
+                self.execmodel.backend == "main_thread_only"
+                and self._primary_thread_task is not None
+            ):
+                self._primary_thread_task.waitfinish()
+                self._primary_thread_task = reply
+                # wake up primary thread (it's okay if this is already set
+                # because we waited for the previous task to finish above
+                # and integrate_as_primary_thread will not clear it when
+                # it enters self._running_lock if it detects that a new
+                # task is available)
+                primary_thread_task_ready.set()
+                return True
         return False
 
-    def spawn(self, func, *args, **kwargs):
-        """return Reply object for the asynchronous dispatch
-        of the given func(*args, **kwargs).
-        """
+    def spawn(self, func, *args, **kwargs) -> Reply:
+        """Asynchronously dispatch func(*args, **kwargs) and return a Reply."""
         reply = Reply((func, args, kwargs), self.execmodel)
         with self._running_lock:
             if self._shuttingdown:
                 raise ValueError("pool is shutting down")
             self._running.add(reply)
             if not self._try_send_to_primary_thread(reply):
                 self.execmodel.start(self._perform_spawn, (reply,))
         return reply
 
-    def terminate(self, timeout=None):
-        """trigger shutdown and wait for completion of all executions."""
+    def terminate(self, timeout: float | None = None) -> bool:
+        """Trigger shutdown and wait for completion of all executions."""
         self.trigger_shutdown()
         return self.waitall(timeout=timeout)
 
-    def waitall(self, timeout=None):
-        """wait until all active spawns have finished executing."""
+    def waitall(self, timeout: float | None = None) -> bool:
+        """Wait until all active spawns have finished executing."""
         with self._running_lock:
             if not self._running:
                 return True
             # if a Reply still runs, we let run_and_release
             # signal us -- note that we are still holding the
             # _running_lock to avoid race conditions
             my_waitall_event = self.execmodel.Event()
@@ -412,255 +473,268 @@
 sysex = (KeyboardInterrupt, SystemExit)
 
 
 DEBUG = os.environ.get("EXECNET_DEBUG")
 pid = os.getpid()
 if DEBUG == "2":
 
-    def trace(*msg):
+    def trace(*msg: object) -> None:
         try:
             line = " ".join(map(str, msg))
             sys.stderr.write(f"[{pid}] {line}\n")
             sys.stderr.flush()
         except Exception:
             pass  # nothing we can do, likely interpreter-shutdown
 
 elif DEBUG:
-    import tempfile
     import os
+    import tempfile
 
     fn = os.path.join(tempfile.gettempdir(), "execnet-debug-%d" % pid)
     # sys.stderr.write("execnet-debug at %r" % (fn,))
     debugfile = open(fn, "w")
 
-    def trace(*msg):
+    def trace(*msg: object) -> None:
         try:
             line = " ".join(map(str, msg))
             debugfile.write(line + "\n")
             debugfile.flush()
-        except Exception:
+        except Exception as exc:
             try:
-                v = sys.exc_info()[1]
-                sys.stderr.write(f"[{pid}] exception during tracing: {v!r}\n")
+                sys.stderr.write(f"[{pid}] exception during tracing: {exc!r}\n")
             except Exception:
                 pass  # nothing we can do, likely interpreter-shutdown
 
 else:
     notrace = trace = lambda *msg: None
 
 
 class Popen2IO:
     error = (IOError, OSError, EOFError)
 
-    def __init__(self, outfile, infile, execmodel):
+    def __init__(self, outfile, infile, execmodel: ExecModel) -> None:
         # we need raw byte streams
         self.outfile, self.infile = outfile, infile
         if sys.platform == "win32":
             import msvcrt
 
             try:
                 msvcrt.setmode(infile.fileno(), os.O_BINARY)
                 msvcrt.setmode(outfile.fileno(), os.O_BINARY)
             except (AttributeError, OSError):
                 pass
         self._read = getattr(infile, "buffer", infile).read
         self._write = getattr(outfile, "buffer", outfile).write
         self.execmodel = execmodel
 
-    def read(self, numbytes):
+    def read(self, numbytes: int) -> bytes:
         """Read exactly 'numbytes' bytes from the pipe."""
         # a file in non-blocking mode may return less bytes, so we loop
         buf = b""
         while numbytes > len(buf):
             data = self._read(numbytes - len(buf))
             if not data:
                 raise EOFError("expected %d bytes, got %d" % (numbytes, len(buf)))
             buf += data
         return buf
 
-    def write(self, data):
-        """write out all data bytes."""
+    def write(self, data: bytes) -> None:
+        """Write out all data bytes."""
         assert isinstance(data, bytes)
         self._write(data)
         self.outfile.flush()
 
-    def close_read(self):
+    def close_read(self) -> None:
         self.infile.close()
 
-    def close_write(self):
+    def close_write(self) -> None:
         self.outfile.close()
 
 
 class Message:
-    """encapsulates Messages and their wire protocol."""
+    """Encapsulates Messages and their wire protocol."""
 
     # message code -> name, handler
     _types: dict[int, tuple[str, Callable[[Message, BaseGateway], None]]] = {}
 
-    def __init__(self, msgcode, channelid=0, data=b""):
+    def __init__(self, msgcode: int, channelid: int = 0, data: bytes = b"") -> None:
         self.msgcode = msgcode
         self.channelid = channelid
         self.data = data
 
     @staticmethod
-    def from_io(io):
+    def from_io(io: ReadIO) -> Message:
         try:
             header = io.read(9)  # type 1, channel 4, payload 4
             if not header:
                 raise EOFError("empty read")
-        except EOFError:
-            e = sys.exc_info()[1]
-            raise EOFError("couldn't load message header, " + e.args[0])
+        except EOFError as e:
+            raise EOFError("couldn't load message header, " + e.args[0]) from None
         msgtype, channel, payload = struct.unpack("!bii", header)
         return Message(msgtype, channel, io.read(payload))
 
-    def to_io(self, io):
+    def to_io(self, io: WriteIO) -> None:
         header = struct.pack("!bii", self.msgcode, self.channelid, len(self.data))
         io.write(header + self.data)
 
-    def received(self, gateway):
+    def received(self, gateway: BaseGateway) -> None:
         handler = self._types[self.msgcode][1]
         handler(self, gateway)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         name = self._types[self.msgcode][0]
-        return "<Message {} channel={} lendata={}>".format(
-            name, self.channelid, len(self.data)
-        )
+        return f"<Message {name} channel={self.channelid} lendata={len(self.data)}>"
 
-    def _status(message, gateway):
+    def _status(message: Message, gateway: BaseGateway) -> None:
         # we use the channelid to send back information
         # but don't instantiate a channel object
         d = {
             "numchannels": len(gateway._channelfactory._channels),
-            "numexecuting": gateway._execpool.active_count(),
+            # TODO(typing): Attribute `_execpool` is only on WorkerGateway.
+            "numexecuting": gateway._execpool.active_count(),  # type: ignore[attr-defined]
             "execmodel": gateway.execmodel.backend,
         }
         gateway._send(Message.CHANNEL_DATA, message.channelid, dumps_internal(d))
         gateway._send(Message.CHANNEL_CLOSE, message.channelid)
 
     STATUS = 0
     _types[STATUS] = ("STATUS", _status)
 
-    def _reconfigure(message, gateway):
+    def _reconfigure(message: Message, gateway: BaseGateway) -> None:
+        data = loads_internal(message.data, gateway)
+        assert isinstance(data, tuple)
+        strconfig: tuple[bool, bool] = data
         if message.channelid == 0:
-            target = gateway
+            gateway._strconfig = strconfig
         else:
-            target = gateway._channelfactory.new(message.channelid)
-        target._strconfig = loads_internal(message.data, gateway)
+            gateway._channelfactory.new(message.channelid)._strconfig = strconfig
 
     RECONFIGURE = 1
     _types[RECONFIGURE] = ("RECONFIGURE", _reconfigure)
 
-    def _gateway_terminate(message, gateway):
+    def _gateway_terminate(message: Message, gateway: BaseGateway) -> None:
         raise GatewayReceivedTerminate(gateway)
 
     GATEWAY_TERMINATE = 2
     _types[GATEWAY_TERMINATE] = ("GATEWAY_TERMINATE", _gateway_terminate)
 
-    def _channel_exec(message, gateway):
+    def _channel_exec(message: Message, gateway: BaseGateway) -> None:
         channel = gateway._channelfactory.new(message.channelid)
         gateway._local_schedulexec(channel=channel, sourcetask=message.data)
 
     CHANNEL_EXEC = 3
     _types[CHANNEL_EXEC] = ("CHANNEL_EXEC", _channel_exec)
 
-    def _channel_data(message, gateway):
+    def _channel_data(message: Message, gateway: BaseGateway) -> None:
         gateway._channelfactory._local_receive(message.channelid, message.data)
 
     CHANNEL_DATA = 4
     _types[CHANNEL_DATA] = ("CHANNEL_DATA", _channel_data)
 
-    def _channel_close(message, gateway):
+    def _channel_close(message: Message, gateway: BaseGateway) -> None:
         gateway._channelfactory._local_close(message.channelid)
 
     CHANNEL_CLOSE = 5
     _types[CHANNEL_CLOSE] = ("CHANNEL_CLOSE", _channel_close)
 
-    def _channel_close_error(message, gateway):
-        remote_error = RemoteError(loads_internal(message.data))
+    def _channel_close_error(message: Message, gateway: BaseGateway) -> None:
+        error_message = loads_internal(message.data)
+        assert isinstance(error_message, str)
+        remote_error = RemoteError(error_message)
         gateway._channelfactory._local_close(message.channelid, remote_error)
 
     CHANNEL_CLOSE_ERROR = 6
     _types[CHANNEL_CLOSE_ERROR] = ("CHANNEL_CLOSE_ERROR", _channel_close_error)
 
-    def _channel_last_message(message, gateway):
+    def _channel_last_message(message: Message, gateway: BaseGateway) -> None:
         gateway._channelfactory._local_close(message.channelid, sendonly=True)
 
     CHANNEL_LAST_MESSAGE = 7
     _types[CHANNEL_LAST_MESSAGE] = ("CHANNEL_LAST_MESSAGE", _channel_last_message)
 
 
 class GatewayReceivedTerminate(Exception):
     """Receiverthread got termination message."""
 
 
-def geterrortext(excinfo, format_exception=traceback.format_exception, sysex=sysex):
+def geterrortext(
+    exc: BaseException,
+    format_exception=traceback.format_exception,
+    sysex: tuple[type[BaseException], ...] = sysex,
+) -> str:
     try:
-        l = format_exception(*excinfo)
+        # In py310, can change this to:
+        # l = format_exception(exc)
+        l = format_exception(type(exc), exc, exc.__traceback__)
         errortext = "".join(l)
     except sysex:
         raise
     except BaseException:
-        errortext = f"{excinfo[0].__name__}: {excinfo[1]}"
+        errortext = f"{type(exc).__name__}: {exc}"
     return errortext
 
 
 class RemoteError(Exception):
     """Exception containing a stringified error from the other side."""
 
-    def __init__(self, formatted):
+    def __init__(self, formatted: str) -> None:
         super().__init__()
         self.formatted = formatted
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.formatted
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}: {self.formatted}"
 
-    def warn(self):
+    def warn(self) -> None:
         if self.formatted != INTERRUPT_TEXT:
             # XXX do this better
             sys.stderr.write(f"[{os.getpid()}] Warning: unhandled {self!r}\n")
 
 
 class TimeoutError(IOError):
     """Exception indicating that a timeout was reached."""
 
 
 NO_ENDMARKER_WANTED = object()
 
 
 class Channel:
-    "Communication channel between two Python Interpreter execution points."
+    """Communication channel between two Python Interpreter execution points."""
+
     RemoteError = RemoteError
     TimeoutError = TimeoutError
     _INTERNALWAKEUP = 1000
     _executing = False
 
-    def __init__(self, gateway, id):
+    def __init__(self, gateway: BaseGateway, id: int) -> None:
+        """:private:"""
         assert isinstance(id, int)
         assert not isinstance(gateway, type)
         self.gateway = gateway
         # XXX: defaults copied from Unserializer
         self._strconfig = getattr(gateway, "_strconfig", (True, False))
         self.id = id
         self._items = self.gateway.execmodel.queue.Queue()
         self._closed = False
         self._receiveclosed = self.gateway.execmodel.Event()
-        self._remoteerrors = []
+        self._remoteerrors: list[RemoteError] = []
 
-    def _trace(self, *msg):
+    def _trace(self, *msg: object) -> None:
         self.gateway._trace(self.id, *msg)
 
-    def setcallback(self, callback, endmarker=NO_ENDMARKER_WANTED):
-        """set a callback function for receiving items.
+    def setcallback(
+        self,
+        callback: Callable[[Any], Any],
+        endmarker: object = NO_ENDMARKER_WANTED,
+    ) -> None:
+        """Set a callback function for receiving items.
 
-        All already queued items will immediately trigger the callback.
+        All already-queued items will immediately trigger the callback.
         Afterwards the callback will execute in the receiver thread
         for each received data item and calls to ``receive()`` will
         raise an error.
         If an endmarker is specified the callback will eventually
         be called with the endmarker when the channel closes.
         """
         _callbacks = self.gateway._channelfactory._callbacks
@@ -681,21 +755,22 @@
                         items.put(olditem)  # for other receivers
                         if endmarker is not NO_ENDMARKER_WANTED:
                             callback(endmarker)
                         break
                     else:
                         callback(olditem)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         flag = self.isclosed() and "closed" or "open"
         return "<Channel id=%d %s>" % (self.id, flag)
 
-    def __del__(self):
+    def __del__(self) -> None:
         if self.gateway is None:  # can be None in tests
-            return
+            return  # type: ignore[unreachable]
+
         self._trace("channel.__del__")
         # no multithreading issues here, because we have the last ref to 'self'
         if self._closed:
             # state transition "closed" --> "deleted"
             for error in self._remoteerrors:
                 error.warn()
         elif self._receiveclosed.is_set():
@@ -727,33 +802,52 @@
             except AttributeError:
                 pass
             return None
 
     #
     # public API for channel objects
     #
-    def isclosed(self):
-        """return True if the channel is closed. A closed
-        channel may still hold items.
+    def isclosed(self) -> bool:
+        """Return True if the channel is closed.
+
+        A closed channel may still hold items.
         """
         return self._closed
 
-    def makefile(self, mode="w", proxyclose=False):
-        """return a file-like object.
+    @overload
+    def makefile(self, mode: Literal["r"], proxyclose: bool = ...) -> ChannelFileRead:
+        pass
+
+    @overload
+    def makefile(
+        self,
+        mode: Literal["w"] = ...,
+        proxyclose: bool = ...,
+    ) -> ChannelFileWrite:
+        pass
+
+    def makefile(
+        self,
+        mode: Literal["r", "w"] = "w",
+        proxyclose: bool = False,
+    ) -> ChannelFileWrite | ChannelFileRead:
+        """Return a file-like object.
+
         mode can be 'w' or 'r' for writeable/readable files.
-        if proxyclose is true file.close() will also close the channel.
+        If proxyclose is true, file.close() will also close the channel.
         """
         if mode == "w":
             return ChannelFileWrite(channel=self, proxyclose=proxyclose)
         elif mode == "r":
             return ChannelFileRead(channel=self, proxyclose=proxyclose)
         raise ValueError(f"mode {mode!r} not available")
 
-    def close(self, error=None):
-        """close down this channel with an optional error message.
+    def close(self, error=None) -> None:
+        """Close down this channel with an optional error message.
+
         Note that closing of a channel tied to remote_exec happens
         automatically at the end of execution and cannot
         be done explicitly.
         """
         if self._executing:
             raise OSError("cannot explicitly close channel within remote_exec")
         if self._closed:
@@ -776,136 +870,155 @@
             self._closed = True  # --> "closed"
             self._receiveclosed.set()
             queue = self._items
             if queue is not None:
                 queue.put(ENDMARKER)
             self.gateway._channelfactory._no_longer_opened(self.id)
 
-    def waitclose(self, timeout=None):
-        """wait until this channel is closed (or the remote side
+    def waitclose(self, timeout: float | None = None) -> None:
+        """Wait until this channel is closed (or the remote side
         otherwise signalled that no more data was being sent).
+
         The channel may still hold receiveable items, but not receive
-        any more after waitclose() has returned.  Exceptions from executing
-        code on the other side are reraised as local channel.RemoteErrors.
+        any more after waitclose() has returned.
+
+        Exceptions from executing code on the other side are reraised as local
+        channel.RemoteErrors.
+
         EOFError is raised if the reading-connection was prematurely closed,
         which often indicates a dying process.
+
         self.TimeoutError is raised after the specified number of seconds
         (default is None, i.e. wait indefinitely).
         """
         # wait for non-"opened" state
         self._receiveclosed.wait(timeout=timeout)
         if not self._receiveclosed.is_set():
             raise self.TimeoutError("Timeout after %r seconds" % timeout)
         error = self._getremoteerror()
         if error:
             raise error
 
-    def send(self, item):
-        """sends the given item to the other side of the channel,
+    def send(self, item: object) -> None:
+        """Sends the given item to the other side of the channel,
         possibly blocking if the sender queue is full.
-        The item must be a simple python type and will be
-        copied to the other side by value.  IOError is
-        raised if the write pipe was prematurely closed.
+
+        The item must be a simple Python type and will be
+        copied to the other side by value.
+
+        OSError is raised if the write pipe was prematurely closed.
         """
         if self.isclosed():
             raise OSError(f"cannot send to {self!r}")
         self.gateway._send(Message.CHANNEL_DATA, self.id, dumps_internal(item))
 
-    def receive(self, timeout=None):
-        """receive a data item that was sent from the other side.
-        timeout: None [default] blocked waiting.  A positive number
+    def receive(self, timeout: float | None = None) -> Any:
+        """Receive a data item that was sent from the other side.
+
+        timeout: None [default] blocked waiting. A positive number
         indicates the number of seconds after which a channel.TimeoutError
         exception will be raised if no item was received.
+
         Note that exceptions from the remotely executing code will be
         reraised as channel.RemoteError exceptions containing
         a textual representation of the remote traceback.
         """
         itemqueue = self._items
         if itemqueue is None:
             raise OSError("cannot receive(), channel has receiver callback")
         try:
             x = itemqueue.get(timeout=timeout)
         except self.gateway.execmodel.queue.Empty:
-            raise self.TimeoutError("no item after %r seconds" % timeout)
+            raise self.TimeoutError("no item after %r seconds" % timeout) from None
         if x is ENDMARKER:
             itemqueue.put(x)  # for other receivers
             raise self._getremoteerror() or EOFError()
         else:
             return x
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         return self
 
-    def next(self):
+    def next(self) -> Any:
         try:
             return self.receive()
         except EOFError:
-            raise StopIteration
+            raise StopIteration from None
 
     __next__ = next
 
-    def reconfigure(self, py2str_as_py3str=True, py3str_as_py2str=False):
-        """
-        set the string coercion for this channel
-        the default is to try to convert py2 str as py3 str,
+    def reconfigure(
+        self, py2str_as_py3str: bool = True, py3str_as_py2str: bool = False
+    ) -> None:
+        """Set the string coercion for this channel.
+
+        The default is to try to convert py2 str as py3 str,
         but not to try and convert py3 str to py2 str
         """
         self._strconfig = (py2str_as_py3str, py3str_as_py2str)
         data = dumps_internal(self._strconfig)
         self.gateway._send(Message.RECONFIGURE, self.id, data=data)
 
 
 ENDMARKER = object()
 INTERRUPT_TEXT = "keyboard-interrupted"
+MAIN_THREAD_ONLY_DEADLOCK_TEXT = (
+    "concurrent remote_exec would cause deadlock for main_thread_only execmodel"
+)
 
 
 class ChannelFactory:
-    def __init__(self, gateway, startcount=1):
-        self._channels = weakref.WeakValueDictionary()
-        self._callbacks = {}
+    def __init__(self, gateway: BaseGateway, startcount: int = 1) -> None:
+        self._channels: weakref.WeakValueDictionary[int, Channel] = (
+            weakref.WeakValueDictionary()
+        )
+        # Channel ID => (callback, end marker, strconfig)
+        self._callbacks: dict[
+            int, tuple[Callable[[Any], Any], object, tuple[bool, bool]]
+        ] = {}
         self._writelock = gateway.execmodel.Lock()
         self.gateway = gateway
         self.count = startcount
         self.finished = False
         self._list = list  # needed during interp-shutdown
 
-    def new(self, id=None):
-        """create a new Channel with 'id' (or create new id if None)."""
+    def new(self, id: int | None = None) -> Channel:
+        """Create a new Channel with 'id' (or create new id if None)."""
         with self._writelock:
             if self.finished:
                 raise OSError(f"connection already closed: {self.gateway}")
             if id is None:
                 id = self.count
                 self.count += 2
             try:
                 channel = self._channels[id]
             except KeyError:
                 channel = self._channels[id] = Channel(self.gateway, id)
             return channel
 
-    def channels(self):
+    def channels(self) -> list[Channel]:
         return self._list(self._channels.values())
 
     #
     # internal methods, called from the receiver thread
     #
-    def _no_longer_opened(self, id):
+    def _no_longer_opened(self, id: int) -> None:
         try:
             del self._channels[id]
         except KeyError:
             pass
         try:
             callback, endmarker, strconfig = self._callbacks.pop(id)
         except KeyError:
             pass
         else:
             if endmarker is not NO_ENDMARKER_WANTED:
                 callback(endmarker)
 
-    def _local_close(self, id, remoteerror=None, sendonly=False):
+    def _local_close(self, id: int, remoteerror=None, sendonly: bool = False) -> None:
         channel = self._channels.get(id)
         if channel is None:
             # channel already in "deleted" state
             if remoteerror:
                 remoteerror.warn()
             self._no_longer_opened(id)
         else:
@@ -916,94 +1029,93 @@
             if queue is not None:
                 queue.put(ENDMARKER)
             self._no_longer_opened(id)
             if not sendonly:  # otherwise #--> "sendonly"
                 channel._closed = True  # --> "closed"
             channel._receiveclosed.set()
 
-    def _local_receive(self, id, data):
+    def _local_receive(self, id: int, data) -> None:
         # executes in receiver thread
         channel = self._channels.get(id)
         try:
             callback, endmarker, strconfig = self._callbacks[id]
         except KeyError:
-            queue = channel and channel._items
+            queue = channel._items if channel is not None else None
             if queue is None:
                 pass  # drop data
             else:
                 item = loads_internal(data, channel)
                 queue.put(item)
         else:
             try:
                 data = loads_internal(data, channel, strconfig)
                 callback(data)  # even if channel may be already closed
-            except Exception:
-                excinfo = sys.exc_info()
-                self.gateway._trace("exception during callback: %s" % excinfo[1])
-                errortext = self.gateway._geterrortext(excinfo)
+            except Exception as exc:
+                self.gateway._trace("exception during callback: %s" % exc)
+                errortext = self.gateway._geterrortext(exc)
                 self.gateway._send(
                     Message.CHANNEL_CLOSE_ERROR, id, dumps_internal(errortext)
                 )
                 self._local_close(id, errortext)
 
-    def _finished_receiving(self):
+    def _finished_receiving(self) -> None:
         with self._writelock:
             self.finished = True
         for id in self._list(self._channels):
             self._local_close(id, sendonly=True)
         for id in self._list(self._callbacks):
             self._no_longer_opened(id)
 
 
 class ChannelFile:
-    def __init__(self, channel, proxyclose=True):
+    def __init__(self, channel: Channel, proxyclose: bool = True) -> None:
         self.channel = channel
         self._proxyclose = proxyclose
 
-    def isatty(self):
+    def isatty(self) -> bool:
         return False
 
-    def close(self):
+    def close(self) -> None:
         if self._proxyclose:
             self.channel.close()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         state = self.channel.isclosed() and "closed" or "open"
         return "<ChannelFile %d %s>" % (self.channel.id, state)
 
 
 class ChannelFileWrite(ChannelFile):
-    def write(self, out):
+    def write(self, out: bytes) -> None:
         self.channel.send(out)
 
-    def flush(self):
+    def flush(self) -> None:
         pass
 
 
 class ChannelFileRead(ChannelFile):
-    def __init__(self, channel, proxyclose=True):
+    def __init__(self, channel: Channel, proxyclose: bool = True) -> None:
         super().__init__(channel, proxyclose)
-        self._buffer = None
+        self._buffer: str | None = None
 
-    def read(self, n):
+    def read(self, n: int) -> str:
         try:
             if self._buffer is None:
-                self._buffer = self.channel.receive()
+                self._buffer = cast(str, self.channel.receive())
             while len(self._buffer) < n:
-                self._buffer += self.channel.receive()
+                self._buffer += cast(str, self.channel.receive())
         except EOFError:
             self.close()
         if self._buffer is None:
             ret = ""
         else:
             ret = self._buffer[:n]
             self._buffer = self._buffer[n:]
         return ret
 
-    def readline(self):
+    def readline(self) -> str:
         if self._buffer is not None:
             i = self._buffer.find("\n")
             if i != -1:
                 return self.read(i + 1)
             line = self.read(len(self._buffer) + 1)
         else:
             line = self.read(1)
@@ -1012,106 +1124,119 @@
             if not c:
                 break
             line += c
         return line
 
 
 class BaseGateway:
-    exc_info = sys.exc_info
     _sysex = sysex
     id = "<worker>"
 
-    def __init__(self, io, id, _startcount=2):
+    def __init__(self, io: IO, id, _startcount: int = 2) -> None:
         self.execmodel = io.execmodel
         self._io = io
         self.id = id
         self._strconfig = (Unserializer.py2str_as_py3str, Unserializer.py3str_as_py2str)
         self._channelfactory = ChannelFactory(self, _startcount)
         self._receivelock = self.execmodel.RLock()
         # globals may be NONE at process-termination
         self.__trace = trace
         self._geterrortext = geterrortext
         self._receivepool = WorkerPool(self.execmodel)
 
-    def _trace(self, *msg):
+    def _trace(self, *msg: object) -> None:
         self.__trace(self.id, *msg)
 
-    def _initreceive(self):
+    def _initreceive(self) -> None:
         self._receivepool.spawn(self._thread_receiver)
 
-    def _thread_receiver(self):
-        def log(*msg):
+    def _thread_receiver(self) -> None:
+        def log(*msg: object) -> None:
             self._trace("[receiver-thread]", *msg)
 
         log("RECEIVERTHREAD: starting to run")
         io = self._io
         try:
             while 1:
                 msg = Message.from_io(io)
                 log("received", msg)
                 with self._receivelock:
                     msg.received(self)
                     del msg
         except (KeyboardInterrupt, GatewayReceivedTerminate):
             pass
-        except EOFError:
+        except EOFError as exc:
             log("EOF without prior gateway termination message")
-            self._error = self.exc_info()[1]
-        except Exception:
-            log(self._geterrortext(self.exc_info()))
+            self._error = exc
+        except Exception as exc:
+            log(self._geterrortext(exc))
         log("finishing receiving thread")
         # wake up and terminate any execution waiting to receive
         self._channelfactory._finished_receiving()
         log("terminating execution")
         self._terminate_execution()
         log("closing read")
         self._io.close_read()
         log("closing write")
         self._io.close_write()
         log("terminating our receive pseudo pool")
         self._receivepool.trigger_shutdown()
 
-    def _terminate_execution(self):
+    def _terminate_execution(self) -> None:
         pass
 
-    def _send(self, msgcode, channelid=0, data=b""):
+    def _send(self, msgcode: int, channelid: int = 0, data: bytes = b"") -> None:
         message = Message(msgcode, channelid, data)
         try:
             message.to_io(self._io)
             self._trace("sent", message)
-        except (OSError, ValueError):
-            e = sys.exc_info()[1]
+        except (OSError, ValueError) as e:
             self._trace("failed to send", message, e)
             # ValueError might be because the IO is already closed
-            raise OSError("cannot send (already closed?)")
+            raise OSError("cannot send (already closed?)") from e
 
-    def _local_schedulexec(self, channel, sourcetask):
+    def _local_schedulexec(self, channel: Channel, sourcetask: bytes) -> None:
         channel.close("execution disallowed")
 
     # _____________________________________________________________________
     #
     # High Level Interface
     # _____________________________________________________________________
     #
-    def newchannel(self):
-        """return a new independent channel."""
+    def newchannel(self) -> Channel:
+        """Return a new independent channel."""
         return self._channelfactory.new()
 
-    def join(self, timeout=None):
+    def join(self, timeout: float | None = None) -> None:
         """Wait for receiverthread to terminate."""
         self._trace("waiting for receiver thread to finish")
-        self._receivepool.waitall()
+        self._receivepool.waitall(timeout)
 
 
 class WorkerGateway(BaseGateway):
-    def _local_schedulexec(self, channel, sourcetask):
-        sourcetask = loads_internal(sourcetask)
-        self._execpool.spawn(self.executetask, (channel, sourcetask))
+    def _local_schedulexec(self, channel: Channel, sourcetask: bytes) -> None:
+        if self._execpool.execmodel.backend == "main_thread_only":
+            assert self._executetask_complete is not None
+            # It's necessary to wait for a short time in order to ensure
+            # that we do not report a false-positive deadlock error, since
+            # channel close does not elicit a response that would provide
+            # a guarantee to remote_exec callers that the previous task
+            # has released the main thread. If the timeout expires then it
+            # should be practically impossible to report a false-positive.
+            if not self._executetask_complete.wait(timeout=1):
+                channel.close(MAIN_THREAD_ONLY_DEADLOCK_TEXT)
+                return
+            # It's only safe to clear here because the above wait proves
+            # that there is not a previous task about to set it again.
+            self._executetask_complete.clear()
 
-    def _terminate_execution(self):
+        sourcetask_ = loads_internal(sourcetask)
+        self._execpool.spawn(self.executetask, (channel, sourcetask_))
+
+    def _terminate_execution(self) -> None:
         # called from receiverthread
         self._trace("shutting down execution pool")
         self._execpool.trigger_shutdown()
         if not self._execpool.waitall(5.0):
             self._trace("execution ongoing after 5 secs," " trying interrupt_main")
             # We try hard to terminate execution based on the assumption
             # that there is only one gateway object running per-process.
@@ -1123,37 +1248,46 @@
                 interrupt_main()
             if not self._execpool.waitall(10.0):
                 self._trace(
                     "execution did not finish in another 10 secs, " "calling os._exit()"
                 )
                 os._exit(1)
 
-    def serve(self):
-        def trace(msg):
+    def serve(self) -> None:
+        def trace(msg: str) -> None:
             self._trace("[serve] " + msg)
 
-        hasprimary = self.execmodel.backend == "thread"
+        hasprimary = self.execmodel.backend in ("thread", "main_thread_only")
         self._execpool = WorkerPool(self.execmodel, hasprimary=hasprimary)
+        self._executetask_complete = None
+        if self.execmodel.backend == "main_thread_only":
+            self._executetask_complete = self.execmodel.Event()
+            # Initialize state to indicate that there is no previous task
+            # executing so that we don't need a separate flag to track this.
+            self._executetask_complete.set()
         trace("spawning receiver thread")
         self._initreceive()
         try:
             if hasprimary:
                 # this will return when we are in shutdown
                 trace("integrating as primary thread")
                 self._execpool.integrate_as_primary_thread()
             trace("joining receiver thread")
             self.join()
         except KeyboardInterrupt:
             # in the worker we can't really do anything sensible
             trace("swallowing keyboardinterrupt, serve finished")
 
-    def executetask(self, item):
+    def executetask(
+        self,
+        item: tuple[Channel, tuple[str, str | None, str | None, dict[str, object]]],
+    ) -> None:
         try:
             channel, (source, file_name, call_name, kwargs) = item
-            loc = {"channel": channel, "__name__": "__channelexec__"}
+            loc: dict[str, Any] = {"channel": channel, "__name__": "__channelexec__"}
             self._trace(f"execution starts[{channel.id}]: {repr(source)[:50]}")
             channel._executing = True
             try:
                 co = compile(source + "\n", file_name or "<remote exec>", "exec")
                 exec(co, loc)
                 if call_name:
                     self._trace("calling %s(**%60r)" % (call_name, kwargs))
@@ -1161,24 +1295,28 @@
                     function(channel, **kwargs)
             finally:
                 channel._executing = False
                 self._trace("execution finished")
         except KeyboardInterrupt:
             channel.close(INTERRUPT_TEXT)
             raise
-        except BaseException:
-            excinfo = self.exc_info()
-            if not isinstance(excinfo[1], EOFError):
+        except BaseException as exc:
+            if not isinstance(exc, EOFError):
                 if not channel.gateway._channelfactory.finished:
-                    self._trace(f"got exception: {excinfo[1]!r}")
-                    errortext = self._geterrortext(excinfo)
+                    self._trace(f"got exception: {exc!r}")
+                    errortext = self._geterrortext(exc)
                     channel.close(errortext)
                     return
             self._trace("ignoring EOFError because receiving finished")
         channel.close()
+        if self._executetask_complete is not None:
+            # Indicate that this task has finished executing, meaning
+            # that there is no possibility of it triggering a deadlock
+            # for the next spawn call.
+            self._executetask_complete.set()
 
 
 #
 # Cross-Python pickling code, tested from test_serializer.py
 #
 
 
@@ -1190,15 +1328,15 @@
     """Error while serializing an object."""
 
 
 class LoadError(DataFormatError):
     """Error while unserializing an object."""
 
 
-def bchr(n):
+def bchr(n: int) -> bytes:
     return bytes([n])
 
 
 DUMPFORMAT_VERSION = bchr(2)
 
 FOUR_BYTE_INT_MAX = 2147483647
 
@@ -1209,15 +1347,15 @@
 
 
 class _Stop(Exception):
     pass
 
 
 class opcode:
-    """container for name -> num mappings."""
+    """Container for name -> num mappings."""
 
     BUILDTUPLE = b"@"
     BYTES = b"A"
     CHANNEL = b"B"
     FALSE = b"C"
     FLOAT = b"D"
     FROZENSET = b"E"
@@ -1239,370 +1377,398 @@
 
 
 class Unserializer:
     num2func: dict[bytes, Callable[[Unserializer], None]] = {}
     py2str_as_py3str = True  # True
     py3str_as_py2str = False  # false means py2 will get unicode
 
-    def __init__(self, stream, channel_or_gateway=None, strconfig=None):
-        gateway = getattr(channel_or_gateway, "gateway", channel_or_gateway)
-        strconfig = getattr(channel_or_gateway, "_strconfig", strconfig)
+    def __init__(
+        self,
+        stream: ReadIO,
+        channel_or_gateway: Channel | BaseGateway | None = None,
+        strconfig: tuple[bool, bool] | None = None,
+    ) -> None:
+        if isinstance(channel_or_gateway, Channel):
+            gw: BaseGateway | None = channel_or_gateway.gateway
+        else:
+            gw = channel_or_gateway
+        if channel_or_gateway is None:
+            strconfig = None
+        else:
+            strconfig = channel_or_gateway._strconfig
         if strconfig:
             self.py2str_as_py3str, self.py3str_as_py2str = strconfig
         self.stream = stream
-        self.channelfactory = getattr(gateway, "_channelfactory", gateway)
+        if gw is None:
+            self.channelfactory = None
+        else:
+            self.channelfactory = gw._channelfactory
 
-    def load(self, versioned=False):
+    def load(self, versioned: bool = False) -> Any:
         if versioned:
             ver = self.stream.read(1)
             if ver != DUMPFORMAT_VERSION:
                 raise LoadError("wrong dumpformat version %r" % ver)
-        self.stack = []
+        self.stack: list[object] = []
         try:
             while True:
                 opcode = self.stream.read(1)
                 if not opcode:
                     raise EOFError
                 try:
                     loader = self.num2func[opcode]
                 except KeyError:
                     raise LoadError(
-                        "unknown opcode %r - " "wire protocol corruption?" % (opcode,)
-                    )
+                        f"unknown opcode {opcode!r} - wire protocol corruption?"
+                    ) from None
                 loader(self)
         except _Stop:
             if len(self.stack) != 1:
-                raise LoadError("internal unserialization error")
+                raise LoadError("internal unserialization error") from None
             return self.stack.pop(0)
         else:
             raise LoadError("didn't get STOP")
 
-    def load_none(self):
+    def load_none(self) -> None:
         self.stack.append(None)
 
     num2func[opcode.NONE] = load_none
 
-    def load_true(self):
+    def load_true(self) -> None:
         self.stack.append(True)
 
     num2func[opcode.TRUE] = load_true
 
-    def load_false(self):
+    def load_false(self) -> None:
         self.stack.append(False)
 
     num2func[opcode.FALSE] = load_false
 
-    def load_int(self):
+    def load_int(self) -> None:
         i = self._read_int4()
         self.stack.append(i)
 
     num2func[opcode.INT] = load_int
 
-    def load_longint(self):
+    def load_longint(self) -> None:
         s = self._read_byte_string()
         self.stack.append(int(s))
 
     num2func[opcode.LONGINT] = load_longint
 
     load_long = load_int
     num2func[opcode.LONG] = load_long
     load_longlong = load_longint
     num2func[opcode.LONGLONG] = load_longlong
 
-    def load_float(self):
+    def load_float(self) -> None:
         binary = self.stream.read(FLOAT_FORMAT_SIZE)
         self.stack.append(struct.unpack(FLOAT_FORMAT, binary)[0])
 
     num2func[opcode.FLOAT] = load_float
 
-    def load_complex(self):
+    def load_complex(self) -> None:
         binary = self.stream.read(COMPLEX_FORMAT_SIZE)
         self.stack.append(complex(*struct.unpack(COMPLEX_FORMAT, binary)))
 
     num2func[opcode.COMPLEX] = load_complex
 
-    def _read_int4(self):
-        return struct.unpack("!i", self.stream.read(4))[0]
+    def _read_int4(self) -> int:
+        value: int = struct.unpack("!i", self.stream.read(4))[0]
+        return value
 
-    def _read_byte_string(self):
+    def _read_byte_string(self) -> bytes:
         length = self._read_int4()
         as_bytes = self.stream.read(length)
         return as_bytes
 
-    def load_py3string(self):
+    def load_py3string(self) -> None:
         as_bytes = self._read_byte_string()
         if self.py3str_as_py2str:
             # XXX Should we try to decode into latin-1?
             self.stack.append(as_bytes)
         else:
             self.stack.append(as_bytes.decode("utf-8"))
 
     num2func[opcode.PY3STRING] = load_py3string
 
-    def load_py2string(self):
+    def load_py2string(self) -> None:
         as_bytes = self._read_byte_string()
         if self.py2str_as_py3str:
-            s = as_bytes.decode("latin-1")
+            s: bytes | str = as_bytes.decode("latin-1")
         else:
             s = as_bytes
         self.stack.append(s)
 
     num2func[opcode.PY2STRING] = load_py2string
 
-    def load_bytes(self):
+    def load_bytes(self) -> None:
         s = self._read_byte_string()
         self.stack.append(s)
 
     num2func[opcode.BYTES] = load_bytes
 
-    def load_unicode(self):
+    def load_unicode(self) -> None:
         self.stack.append(self._read_byte_string().decode("utf-8"))
 
     num2func[opcode.UNICODE] = load_unicode
 
-    def load_newlist(self):
+    def load_newlist(self) -> None:
         length = self._read_int4()
         self.stack.append([None] * length)
 
     num2func[opcode.NEWLIST] = load_newlist
 
-    def load_setitem(self):
+    def load_setitem(self) -> None:
         if len(self.stack) < 3:
             raise LoadError("not enough items for setitem")
         value = self.stack.pop()
         key = self.stack.pop()
-        self.stack[-1][key] = value
+        self.stack[-1][key] = value  # type: ignore[index]
 
     num2func[opcode.SETITEM] = load_setitem
 
-    def load_newdict(self):
+    def load_newdict(self) -> None:
         self.stack.append({})
 
     num2func[opcode.NEWDICT] = load_newdict
 
-    def _load_collection(self, type_):
+    def _load_collection(self, type_: type) -> None:
         length = self._read_int4()
         if length:
             res = type_(self.stack[-length:])
             del self.stack[-length:]
             self.stack.append(res)
         else:
             self.stack.append(type_())
 
-    def load_buildtuple(self):
+    def load_buildtuple(self) -> None:
         self._load_collection(tuple)
 
     num2func[opcode.BUILDTUPLE] = load_buildtuple
 
-    def load_set(self):
+    def load_set(self) -> None:
         self._load_collection(set)
 
     num2func[opcode.SET] = load_set
 
-    def load_frozenset(self):
+    def load_frozenset(self) -> None:
         self._load_collection(frozenset)
 
     num2func[opcode.FROZENSET] = load_frozenset
 
-    def load_stop(self):
+    def load_stop(self) -> None:
         raise _Stop
 
     num2func[opcode.STOP] = load_stop
 
-    def load_channel(self):
+    def load_channel(self) -> None:
         id = self._read_int4()
+        assert self.channelfactory is not None
         newchannel = self.channelfactory.new(id)
         self.stack.append(newchannel)
 
     num2func[opcode.CHANNEL] = load_channel
 
 
-def dumps(obj):
-    """return a serialized bytestring of the given obj.
+def dumps(obj: object) -> bytes:
+    """Serialize the given obj to a bytestring.
 
     The obj and all contained objects must be of a builtin
-    python type (so nested dicts, sets, etc. are all ok but
+    Python type (so nested dicts, sets, etc. are all OK but
     not user-level instances).
     """
-    return _Serializer().save(obj, versioned=True)
+    return _Serializer().save(obj, versioned=True)  # type: ignore[return-value]
 
 
-def dump(byteio, obj):
+def dump(byteio, obj: object) -> None:
     """write a serialized bytestring of the given obj to the given stream."""
     _Serializer(write=byteio.write).save(obj, versioned=True)
 
 
-def loads(bytestring, py2str_as_py3str=False, py3str_as_py2str=False):
-    """return the object as deserialized from the given bytestring.
+def loads(
+    bytestring: bytes, py2str_as_py3str: bool = False, py3str_as_py2str: bool = False
+) -> Any:
+    """Deserialize the given bytestring to an object.
 
-    py2str_as_py3str: if true then string (str) objects previously
+    py2str_as_py3str: If true then string (str) objects previously
                       dumped on Python2 will be loaded as Python3
                       strings which really are text objects.
-    py3str_as_py2str: if true then string (str) objects previously
+    py3str_as_py2str: If true then string (str) objects previously
                       dumped on Python3 will be loaded as Python2
                       strings instead of unicode objects.
 
-    if the bytestring was dumped with an incompatible protocol
+    If the bytestring was dumped with an incompatible protocol
     version or if the bytestring is corrupted, the
     ``execnet.DataFormatError`` will be raised.
     """
     io = BytesIO(bytestring)
     return load(
         io, py2str_as_py3str=py2str_as_py3str, py3str_as_py2str=py3str_as_py2str
     )
 
 
-def load(io, py2str_as_py3str=False, py3str_as_py2str=False):
-    """derserialize an object form the specified stream.
+def load(
+    io: ReadIO, py2str_as_py3str: bool = False, py3str_as_py2str: bool = False
+) -> Any:
+    """Derserialize an object form the specified stream.
 
     Behaviour and parameters are otherwise the same as with ``loads``
     """
     strconfig = (py2str_as_py3str, py3str_as_py2str)
     return Unserializer(io, strconfig=strconfig).load(versioned=True)
 
 
-def loads_internal(bytestring, channelfactory=None, strconfig=None):
+def loads_internal(
+    bytestring: bytes,
+    channelfactory=None,
+    strconfig: tuple[bool, bool] | None = None,
+) -> Any:
     io = BytesIO(bytestring)
     return Unserializer(io, channelfactory, strconfig).load()
 
 
-def dumps_internal(obj):
-    return _Serializer().save(obj)
+def dumps_internal(obj: object) -> bytes:
+    return _Serializer().save(obj)  # type: ignore[return-value]
 
 
 class _Serializer:
     _dispatch: dict[type, Callable[[_Serializer, object], None]] = {}
 
-    def __init__(self, write=None):
+    def __init__(self, write: Callable[[bytes], None] | None = None) -> None:
         if write is None:
-            self._streamlist = []
+            self._streamlist: list[bytes] = []
             write = self._streamlist.append
         self._write = write
 
-    def save(self, obj, versioned=False):
+    def save(self, obj: object, versioned: bool = False) -> bytes | None:
         # calling here is not re-entrant but multiple instances
         # may write to the same stream because of the common platform
         # atomic-write guarantee (concurrent writes each happen atomically)
         if versioned:
             self._write(DUMPFORMAT_VERSION)
         self._save(obj)
         self._write(opcode.STOP)
         try:
             streamlist = self._streamlist
         except AttributeError:
             return None
         return b"".join(streamlist)
 
-    def _save(self, obj):
+    def _save(self, obj: object) -> None:
         tp = type(obj)
         try:
             dispatch = self._dispatch[tp]
         except KeyError:
             methodname = "save_" + tp.__name__
-            meth = getattr(self.__class__, methodname, None)
+            meth: Callable[[_Serializer, object], None] | None = getattr(
+                self.__class__, methodname, None
+            )
             if meth is None:
-                raise DumpError(f"can't serialize {tp}")
+                raise DumpError(f"can't serialize {tp}") from None
             dispatch = self._dispatch[tp] = meth
         dispatch(self, obj)
 
-    def save_NoneType(self, non):
+    def save_NoneType(self, non: None) -> None:
         self._write(opcode.NONE)
 
-    def save_bool(self, boolean):
+    def save_bool(self, boolean: bool) -> None:
         if boolean:
             self._write(opcode.TRUE)
         else:
             self._write(opcode.FALSE)
 
-    def save_bytes(self, bytes_):
+    def save_bytes(self, bytes_: bytes) -> None:
         self._write(opcode.BYTES)
         self._write_byte_sequence(bytes_)
 
-    def save_str(self, s):
+    def save_str(self, s: str) -> None:
         self._write(opcode.PY3STRING)
         self._write_unicode_string(s)
 
-    def _write_unicode_string(self, s):
+    def _write_unicode_string(self, s: str) -> None:
         try:
             as_bytes = s.encode("utf-8")
-        except UnicodeEncodeError:
-            raise DumpError("strings must be utf-8 encodable")
+        except UnicodeEncodeError as e:
+            raise DumpError("strings must be utf-8 encodable") from e
         self._write_byte_sequence(as_bytes)
 
-    def _write_byte_sequence(self, bytes_):
+    def _write_byte_sequence(self, bytes_: bytes) -> None:
         self._write_int4(len(bytes_), "string is too long")
         self._write(bytes_)
 
-    def _save_integral(self, i, short_op, long_op):
+    def _save_integral(self, i: int, short_op: bytes, long_op: bytes) -> None:
         if i <= FOUR_BYTE_INT_MAX:
             self._write(short_op)
             self._write_int4(i)
         else:
             self._write(long_op)
             self._write_byte_sequence(str(i).rstrip("L").encode("ascii"))
 
-    def save_int(self, i):
+    def save_int(self, i: int) -> None:
         self._save_integral(i, opcode.INT, opcode.LONGINT)
 
-    def save_long(self, l):
+    def save_long(self, l: int) -> None:
         self._save_integral(l, opcode.LONG, opcode.LONGLONG)
 
-    def save_float(self, flt):
+    def save_float(self, flt: float) -> None:
         self._write(opcode.FLOAT)
         self._write(struct.pack(FLOAT_FORMAT, flt))
 
-    def save_complex(self, cpx):
+    def save_complex(self, cpx: complex) -> None:
         self._write(opcode.COMPLEX)
         self._write(struct.pack(COMPLEX_FORMAT, cpx.real, cpx.imag))
 
-    def _write_int4(self, i, error="int must be less than %i" % (FOUR_BYTE_INT_MAX,)):
+    def _write_int4(
+        self, i: int, error: str = "int must be less than %i" % (FOUR_BYTE_INT_MAX,)
+    ) -> None:
         if i > FOUR_BYTE_INT_MAX:
             raise DumpError(error)
         self._write(struct.pack("!i", i))
 
-    def save_list(self, L):
+    def save_list(self, L: list[object]) -> None:
         self._write(opcode.NEWLIST)
         self._write_int4(len(L), "list is too long")
         for i, item in enumerate(L):
             self._write_setitem(i, item)
 
-    def _write_setitem(self, key, value):
+    def _write_setitem(self, key: object, value: object) -> None:
         self._save(key)
         self._save(value)
         self._write(opcode.SETITEM)
 
-    def save_dict(self, d):
+    def save_dict(self, d: dict[object, object]) -> None:
         self._write(opcode.NEWDICT)
         for key, value in d.items():
             self._write_setitem(key, value)
 
-    def save_tuple(self, tup):
+    def save_tuple(self, tup: tuple[object, ...]) -> None:
         for item in tup:
             self._save(item)
         self._write(opcode.BUILDTUPLE)
         self._write_int4(len(tup), "tuple is too long")
 
-    def _write_set(self, s, op):
+    def _write_set(self, s: set[object] | frozenset[object], op: bytes) -> None:
         for item in s:
             self._save(item)
         self._write(op)
         self._write_int4(len(s), "set is too long")
 
-    def save_set(self, s):
+    def save_set(self, s: set[object]) -> None:
         self._write_set(s, opcode.SET)
 
-    def save_frozenset(self, s):
+    def save_frozenset(self, s: frozenset[object]) -> None:
         self._write_set(s, opcode.FROZENSET)
 
-    def save_Channel(self, channel):
+    def save_Channel(self, channel: Channel) -> None:
         self._write(opcode.CHANNEL)
         self._write_int4(channel.id)
 
 
-def init_popen_io(execmodel):
+def init_popen_io(execmodel: ExecModel) -> Popen2IO:
     if not hasattr(os, "dup"):  # jython
         io = Popen2IO(sys.stdout, sys.stdin, execmodel)
         import tempfile
 
         sys.stdin = tempfile.TemporaryFile("r")
         sys.stdout = tempfile.TemporaryFile("w")
     else:
@@ -1626,15 +1792,17 @@
 
         # stderr for win32
         if os.name == "nt":
             sys.stderr = execmodel.fdopen(os.dup(2), "w", 1)
             os.dup2(fd, 2)
         os.close(fd)
         io = Popen2IO(stdout, stdin, execmodel)
-        sys.stdin = execmodel.fdopen(0, "r", 1)
-        sys.stdout = execmodel.fdopen(1, "w", 1)
+        # Use closefd=False since 0 and 1 are shared with
+        # sys.__stdin__ and sys.__stdout__.
+        sys.stdin = execmodel.fdopen(0, "r", 1, closefd=False)
+        sys.stdout = execmodel.fdopen(1, "w", 1, closefd=False)
     return io
 
 
-def serve(io, id):
+def serve(io: IO, id) -> None:
     trace(f"creating workergateway on {io!r}")
     WorkerGateway(io=io, id=id, _startcount=2).serve()
```

### Comparing `execnet-2.0.2/src/execnet/gateway_bootstrap.py` & `execnet-2.1.0/src/execnet/gateway_bootstrap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-"""
-code to initialize the remote side of a gateway once the io is created
-"""
+"""Code to initialize the remote side of a gateway once the IO is created."""
+
+from __future__ import annotations
+
 import inspect
 import os
 
 import execnet
 
 from . import gateway_base
-from .gateway import Gateway
+from .gateway_base import IO
+from .xspec import XSpec
 
 importdir = os.path.dirname(os.path.dirname(execnet.__file__))
 
 
 class HostNotFound(Exception):
     pass
 
 
-def bootstrap_import(io, spec):
-    # only insert the importdir into the path if we must.  This prevents
+def bootstrap_import(io: IO, spec: XSpec) -> None:
+    # Only insert the importdir into the path if we must.  This prevents
     # bugs where backports expect to be shadowed by the standard library on
-    # newer versions of python but would instead shadow the standard library
+    # newer versions of python but would instead shadow the standard library.
     sendexec(
         io,
         "import sys",
         "if %r not in sys.path:" % importdir,
         "    sys.path.insert(0, %r)" % importdir,
         "from execnet.gateway_base import serve, init_popen_io, get_execmodel",
         "sys.stdout.write('1')",
@@ -31,33 +33,33 @@
         "execmodel = get_execmodel(%r)" % spec.execmodel,
         "serve(init_popen_io(execmodel), id='%s-worker')" % spec.id,
     )
     s = io.read(1)
     assert s == b"1", repr(s)
 
 
-def bootstrap_exec(io, spec):
+def bootstrap_exec(io: IO, spec: XSpec) -> None:
     try:
         sendexec(
             io,
             inspect.getsource(gateway_base),
             "execmodel = get_execmodel(%r)" % spec.execmodel,
             "io = init_popen_io(execmodel)",
             "io.write('1'.encode('ascii'))",
             "serve(io, id='%s-worker')" % spec.id,
         )
         s = io.read(1)
         assert s == b"1"
     except EOFError:
         ret = io.wait()
-        if ret == 255:
-            raise HostNotFound(io.remoteaddress)
+        if ret == 255 and hasattr(io, "remoteaddress"):
+            raise HostNotFound(io.remoteaddress) from None
 
 
-def bootstrap_socket(io, id):
+def bootstrap_socket(io: IO, id) -> None:
     # XXX: switch to spec
     from execnet.gateway_socket import SocketIO
 
     sendexec(
         io,
         inspect.getsource(gateway_base),
         "import socket",
@@ -69,41 +71,26 @@
         "io.write('1'.encode('ascii'))",
         "serve(io, id='%s-worker')" % id,
     )
     s = io.read(1)
     assert s == b"1"
 
 
-def sendexec(io, *sources):
+def sendexec(io: IO, *sources: str) -> None:
     source = "\n".join(sources)
     io.write((repr(source) + "\n").encode("utf-8"))
 
 
-def fix_pid_for_jython_popen(gw):
-    """
-    fix for jython 2.5.1
-    """
-    spec, io = gw.spec, gw._io
-    if spec.popen and not spec.via:
-        # XXX: handle the case of remote being jython
-        #      and not having the popen pid
-        if io.popen.pid is None:
-            io.popen.pid = gw.remote_exec(
-                "import os; channel.send(os.getpid())"
-            ).receive()
-
-
-def bootstrap(io, spec):
+def bootstrap(io: IO, spec: XSpec) -> execnet.Gateway:
     if spec.popen:
         if spec.via or spec.python:
             bootstrap_exec(io, spec)
         else:
             bootstrap_import(io, spec)
     elif spec.ssh or spec.vagrant_ssh:
         bootstrap_exec(io, spec)
     elif spec.socket:
         bootstrap_socket(io, spec)
     else:
         raise ValueError("unknown gateway type, can't bootstrap")
-    gw = Gateway(io, spec)
-    fix_pid_for_jython_popen(gw)
+    gw = execnet.Gateway(io, spec)
     return gw
```

### Comparing `execnet-2.0.2/src/execnet/gateway_io.py` & `execnet-2.1.0/src/execnet/gateway_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,128 @@
-"""
-execnet io initialization code
+"""execnet IO initialization code.
 
-creates io instances used for gateway io
+Creates IO instances used for gateway IO.
 """
-import os
+
+from __future__ import annotations
+
 import shlex
 import sys
+from typing import TYPE_CHECKING
+from typing import cast
+
+if TYPE_CHECKING:
+    from execnet.gateway_base import Channel
+    from execnet.gateway_base import ExecModel
+    from execnet.xspec import XSpec
 
 try:
-    from execnet.gateway_base import Popen2IO, Message
+    from execnet.gateway_base import Message
+    from execnet.gateway_base import Popen2IO
 except ImportError:
-    from __main__ import Popen2IO, Message  # type: ignore[no-redef]
+    from __main__ import Message  # type: ignore[no-redef]
+    from __main__ import Popen2IO  # type: ignore[no-redef]
 
 from functools import partial
 
 
 class Popen2IOMaster(Popen2IO):
-    def __init__(self, args, execmodel):
+    # Set externally, for some specs only.
+    remoteaddress: str
+
+    def __init__(self, args, execmodel: ExecModel) -> None:
         PIPE = execmodel.subprocess.PIPE
         self.popen = p = execmodel.subprocess.Popen(args, stdout=PIPE, stdin=PIPE)
         super().__init__(p.stdin, p.stdout, execmodel=execmodel)
 
-    def wait(self):
+    def wait(self) -> int | None:
         try:
-            return self.popen.wait()
+            return self.popen.wait()  # type: ignore[no-any-return]
         except OSError:
-            pass  # subprocess probably dead already
+            return None
 
-    def kill(self):
-        killpopen(self.popen)
-
-
-def killpopen(popen):
-    try:
-        popen.kill()
-    except OSError as e:
-        sys.stderr.write("ERROR killing: %s\n" % e)
-        sys.stderr.flush()
+    def kill(self) -> None:
+        try:
+            self.popen.kill()
+        except OSError as e:
+            sys.stderr.write("ERROR killing: %s\n" % e)
+            sys.stderr.flush()
 
 
 popen_bootstrapline = "import sys;exec(eval(sys.stdin.readline()))"
 
 
-def shell_split_path(path):
+def shell_split_path(path: str) -> list[str]:
     """
     Use shell lexer to split the given path into a list of components,
     taking care to handle Windows' '\' correctly.
     """
     if sys.platform.startswith("win"):
         # replace \\ by / otherwise shlex will strip them out
         path = path.replace("\\", "/")
     return shlex.split(path)
 
 
-def popen_args(spec):
+def popen_args(spec: XSpec) -> list[str]:
     args = shell_split_path(spec.python) if spec.python else [sys.executable]
     args.append("-u")
     if spec.dont_write_bytecode:
         args.append("-B")
     args.extend(["-c", popen_bootstrapline])
     return args
 
 
-def ssh_args(spec):
+def ssh_args(spec: XSpec) -> list[str]:
     # NOTE: If changing this, you need to sync those changes to vagrant_args
     # as well, or, take some time to further refactor the commonalities of
     # ssh_args and vagrant_args.
     remotepython = spec.python or "python"
     args = ["ssh", "-C"]
     if spec.ssh_config is not None:
         args.extend(["-F", str(spec.ssh_config)])
 
+    assert spec.ssh is not None
     args.extend(spec.ssh.split())
     remotecmd = f'{remotepython} -c "{popen_bootstrapline}"'
     args.append(remotecmd)
     return args
 
 
-def vagrant_ssh_args(spec):
+def vagrant_ssh_args(spec: XSpec) -> list[str]:
     # This is the vagrant-wrapped version of SSH. Unfortunately the
     # command lines are incompatible to just channel through ssh_args
     # due to ordering/templating issues.
     # NOTE: This should be kept in sync with the ssh_args behaviour.
     # spec.vagrant is identical to spec.ssh in that they both carry
     # the remote host "address".
+    assert spec.vagrant_ssh is not None
     remotepython = spec.python or "python"
     args = ["vagrant", "ssh", spec.vagrant_ssh, "--", "-C"]
     if spec.ssh_config is not None:
         args.extend(["-F", str(spec.ssh_config)])
     remotecmd = f'{remotepython} -c "{popen_bootstrapline}"'
     args.extend([remotecmd])
     return args
 
 
-def create_io(spec, execmodel):
+def create_io(spec: XSpec, execmodel: ExecModel) -> Popen2IOMaster:
     if spec.popen:
         args = popen_args(spec)
         return Popen2IOMaster(args, execmodel)
     if spec.ssh:
         args = ssh_args(spec)
         io = Popen2IOMaster(args, execmodel)
         io.remoteaddress = spec.ssh
         return io
     if spec.vagrant_ssh:
         args = vagrant_ssh_args(spec)
         io = Popen2IOMaster(args, execmodel)
         io.remoteaddress = spec.vagrant_ssh
         return io
+    assert False
 
 
 #
 # Proxy Gateway handling code
 #
 # master: proxy initiator
 # forwarder: forwards between master and sub
@@ -120,93 +132,105 @@
 RIO_WAIT = 2
 RIO_REMOTEADDRESS = 3
 RIO_CLOSE_WRITE = 4
 
 
 class ProxyIO:
     """A Proxy IO object allows to instantiate a Gateway
-    through another "via" gateway.  A master:ProxyIO object
-    provides an IO object effectively connected to the sub
-    via the forwarder.  To achieve this, master:ProxyIO interacts
-    with forwarder:serve_proxy_io() which itself
-    instantiates and interacts with the sub.
+    through another "via" gateway.
+
+    A master:ProxyIO object provides an IO object effectively connected to the
+    sub via the forwarder. To achieve this, master:ProxyIO interacts with
+    forwarder:serve_proxy_io() which itself instantiates and interacts with the
+    sub.
     """
 
-    def __init__(self, proxy_channel, execmodel):
+    def __init__(self, proxy_channel: Channel, execmodel: ExecModel) -> None:
         # after exchanging the control channel we use proxy_channel
         # for messaging IO
         self.controlchan = proxy_channel.gateway.newchannel()
         proxy_channel.send(self.controlchan)
         self.iochan = proxy_channel
         self.iochan_file = self.iochan.makefile("r")
         self.execmodel = execmodel
 
-    def read(self, nbytes):
-        return self.iochan_file.read(nbytes)
+    def read(self, nbytes: int) -> bytes:
+        # TODO(typing): The IO protocol requires bytes here but ChannelFileRead
+        # returns str.
+        return self.iochan_file.read(nbytes)  # type: ignore[return-value]
 
-    def write(self, data):
-        return self.iochan.send(data)
+    def write(self, data: bytes) -> None:
+        self.iochan.send(data)
 
-    def _controll(self, event):
+    def _controll(self, event: int) -> object:
         self.controlchan.send(event)
         return self.controlchan.receive()
 
-    def close_write(self):
+    def close_write(self) -> None:
         self._controll(RIO_CLOSE_WRITE)
 
-    def kill(self):
+    def close_read(self) -> None:
+        raise NotImplementedError()
+
+    def kill(self) -> None:
         self._controll(RIO_KILL)
 
-    def wait(self):
-        return self._controll(RIO_WAIT)
+    def wait(self) -> int | None:
+        response = self._controll(RIO_WAIT)
+        assert response is None or isinstance(response, int)
+        return response
 
     @property
-    def remoteaddress(self):
-        return self._controll(RIO_REMOTEADDRESS)
+    def remoteaddress(self) -> str:
+        response = self._controll(RIO_REMOTEADDRESS)
+        assert isinstance(response, str)
+        return response
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<RemoteIO via {self.iochan.gateway.id}>"
 
 
 class PseudoSpec:
-    def __init__(self, vars):
+    def __init__(self, vars) -> None:
         self.__dict__.update(vars)
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> None:
         return None
 
 
-def serve_proxy_io(proxy_channelX):
+def serve_proxy_io(proxy_channelX: Channel) -> None:
     execmodel = proxy_channelX.gateway.execmodel
     log = partial(
         proxy_channelX.gateway._trace, "serve_proxy_io:%s" % proxy_channelX.id
     )
-    spec = PseudoSpec(proxy_channelX.receive())
+    spec = cast("XSpec", PseudoSpec(proxy_channelX.receive()))
     # create sub IO object which we will proxy back to our proxy initiator
     sub_io = create_io(spec, execmodel)
-    control_chan = proxy_channelX.receive()
+    control_chan = cast("Channel", proxy_channelX.receive())
     log("got control chan", control_chan)
 
     # read data from master, forward it to the sub
     # XXX writing might block, thus blocking the receiver thread
-    def forward_to_sub(data):
+    def forward_to_sub(data: bytes) -> None:
         log("forward data to sub, size %s" % len(data))
         sub_io.write(data)
 
     proxy_channelX.setcallback(forward_to_sub)
 
-    def control(data):
+    def control(data: int) -> None:
         if data == RIO_WAIT:
             control_chan.send(sub_io.wait())
         elif data == RIO_KILL:
-            control_chan.send(sub_io.kill())
+            sub_io.kill()
+            control_chan.send(None)
         elif data == RIO_REMOTEADDRESS:
             control_chan.send(sub_io.remoteaddress)
         elif data == RIO_CLOSE_WRITE:
-            control_chan.send(sub_io.close_write())
+            sub_io.close_write()
+            control_chan.send(None)
 
     control_chan.setcallback(control)
 
     # write data to the master coming from the sub
     forward_to_master_file = proxy_channelX.makefile("w")
 
     # read bootstrap byte from sub, send it on to master
@@ -224,8 +248,8 @@
             log("EOF from sub, terminating proxying loop", spec.id)
             break
         message.to_io(forward_to_master_file)
     # proxy_channelX will be closed from remote_exec's finalization code
 
 
 if __name__ == "__channelexec__":
-    serve_proxy_io(channel)  # type: ignore[name-defined]
+    serve_proxy_io(channel)  # type: ignore[name-defined] # noqa:F821
```

### Comparing `execnet-2.0.2/src/execnet/multi.py` & `execnet-2.1.0/src/execnet/multi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,138 @@
 """
 Managing Gateway Groups and interactions with multiple channels.
 
 (c) 2008-2014, Holger Krekel and others
 """
+
+from __future__ import annotations
+
 import atexit
-import sys
+import types
 from functools import partial
 from threading import Lock
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import Callable
+from typing import Iterable
+from typing import Iterator
+from typing import Literal
+from typing import Sequence
+from typing import overload
 
 from . import gateway_bootstrap
 from . import gateway_io
+from .gateway_base import Channel
+from .gateway_base import ExecModel
+from .gateway_base import WorkerPool
 from .gateway_base import get_execmodel
 from .gateway_base import trace
-from .gateway_base import WorkerPool
 from .xspec import XSpec
 
+if TYPE_CHECKING:
+    from .gateway import Gateway
+
+
 NO_ENDMARKER_WANTED = object()
 
 
 class Group:
-    """Gateway Groups."""
+    """Gateway Group."""
 
     defaultspec = "popen"
 
-    def __init__(self, xspecs=(), execmodel="thread"):
-        """initialize group and make gateways as specified.
-        execmodel can be 'thread' or 'eventlet'.
+    def __init__(
+        self, xspecs: Iterable[XSpec | str | None] = (), execmodel: str = "thread"
+    ) -> None:
+        """Initialize a group and make gateways as specified.
+
+        execmodel can be one of the supported execution models.
         """
-        self._gateways = []
+        self._gateways: list[Gateway] = []
         self._autoidcounter = 0
         self._autoidlock = Lock()
-        self._gateways_to_join = []
+        self._gateways_to_join: list[Gateway] = []
         # we use the same execmodel for all of the Gateway objects
         # we spawn on our side.  Probably we should not allow different
         # execmodels between different groups but not clear.
         # Note that "other side" execmodels may differ and is typically
         # specified by the spec passed to makegateway.
         self.set_execmodel(execmodel)
         for xspec in xspecs:
             self.makegateway(xspec)
         atexit.register(self._cleanup_atexit)
 
     @property
-    def execmodel(self):
+    def execmodel(self) -> ExecModel:
         return self._execmodel
 
     @property
-    def remote_execmodel(self):
+    def remote_execmodel(self) -> ExecModel:
         return self._remote_execmodel
 
-    def set_execmodel(self, execmodel, remote_execmodel=None):
+    def set_execmodel(
+        self, execmodel: str, remote_execmodel: str | None = None
+    ) -> None:
         """Set the execution model for local and remote site.
 
-        execmodel can be one of "thread" or "eventlet" (XXX gevent).
+        execmodel can be one of the supported execution models.
         It determines the execution model for any newly created gateway.
-        If remote_execmodel is not specified it takes on the value
-        of execmodel.
+        If remote_execmodel is not specified it takes on the value of execmodel.
 
         NOTE: Execution models can only be set before any gateway is created.
-
         """
         if self._gateways:
             raise ValueError(
                 "can not set execution models if " "gateways have been created already"
             )
         if remote_execmodel is None:
             remote_execmodel = execmodel
         self._execmodel = get_execmodel(execmodel)
         self._remote_execmodel = get_execmodel(remote_execmodel)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         idgateways = [gw.id for gw in self]
         return "<Group %r>" % idgateways
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: int | str | Gateway) -> Gateway:
         if isinstance(key, int):
             return self._gateways[key]
         for gw in self._gateways:
             if gw == key or gw.id == key:
                 return gw
         raise KeyError(key)
 
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> bool:
         try:
             self[key]
             return True
         except KeyError:
             return False
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._gateways)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Gateway]:
         return iter(list(self._gateways))
 
-    def makegateway(self, spec=None):
-        """create and configure a gateway to a Python interpreter.
+    def makegateway(self, spec: XSpec | str | None = None) -> Gateway:
+        """Create and configure a gateway to a Python interpreter.
+
         The ``spec`` string encodes the target gateway type
         and configuration information. The general format is::
 
             key1=value1//key2=value2//...
 
         If you leave out the ``=value`` part a True value is assumed.
         Valid types: ``popen``, ``ssh=hostname``, ``socket=host:port``.
         Valid configuration::
 
             id=<string>     specifies the gateway id
             python=<path>   specifies which python interpreter to execute
-            execmodel=model 'thread', 'eventlet', 'gevent' model for execution
+            execmodel=model 'thread', 'main_thread_only', 'eventlet', 'gevent' execution model
             chdir=<path>    specifies to which directory to change
             nice=<path>     specifies process priority of new process
             env:NAME=value  specifies a remote environment variable setting.
 
         If no spec is given, self.defaultspec is used.
         """
         if not spec:
@@ -130,16 +151,16 @@
             gw = gateway_bootstrap.bootstrap(proxy_io_master, spec)
         elif spec.popen or spec.ssh or spec.vagrant_ssh:
             io = gateway_io.create_io(spec, execmodel=self.execmodel)
             gw = gateway_bootstrap.bootstrap(io, spec)
         elif spec.socket:
             from . import gateway_socket
 
-            io = gateway_socket.create_io(spec, self, execmodel=self.execmodel)
-            gw = gateway_bootstrap.bootstrap(io, spec)
+            sio = gateway_socket.create_io(spec, self, execmodel=self.execmodel)
+            gw = gateway_bootstrap.bootstrap(sio, spec)
         else:
             raise ValueError(f"no gateway type found for {spec._spec!r}")
         gw.spec = spec
         self._register(gw)
         if spec.chdir or spec.nice or spec.env:
             channel = gw.remote_exec(
                 """
@@ -157,149 +178,166 @@
             """
             )
             nice = spec.nice and int(spec.nice) or 0
             channel.send((spec.chdir, nice, spec.env))
             channel.waitclose()
         return gw
 
-    def allocate_id(self, spec):
+    def allocate_id(self, spec: XSpec) -> None:
         """(re-entrant) allocate id for the given xspec object."""
         if spec.id is None:
             with self._autoidlock:
                 id = "gw" + str(self._autoidcounter)
                 self._autoidcounter += 1
                 if id in self:
                     raise ValueError(f"already have gateway with id {id!r}")
                 spec.id = id
 
-    def _register(self, gateway):
+    def _register(self, gateway: Gateway) -> None:
         assert not hasattr(gateway, "_group")
         assert gateway.id
         assert gateway.id not in self
         self._gateways.append(gateway)
         gateway._group = self
 
-    def _unregister(self, gateway):
+    def _unregister(self, gateway: Gateway) -> None:
         self._gateways.remove(gateway)
         self._gateways_to_join.append(gateway)
 
-    def _cleanup_atexit(self):
+    def _cleanup_atexit(self) -> None:
         trace(f"=== atexit cleanup {self!r} ===")
         self.terminate(timeout=1.0)
 
-    def terminate(self, timeout=None):
-        """trigger exit of member gateways and wait for termination
-        of member gateways and associated subprocesses.  After waiting
-        timeout seconds try to to kill local sub processes of popen-
-        and ssh-gateways.  Timeout defaults to None meaning
-        open-ended waiting and no kill attempts.
-        """
+    def terminate(self, timeout: float | None = None) -> None:
+        """Trigger exit of member gateways and wait for termination
+        of member gateways and associated subprocesses.
+
+        After waiting timeout seconds try to to kill local sub processes of
+        popen- and ssh-gateways.
 
+        Timeout defaults to None meaning open-ended waiting and no kill
+        attempts.
+        """
         while self:
-            vias = {}
+            vias: set[str] = set()
             for gw in self:
                 if gw.spec.via:
-                    vias[gw.spec.via] = True
+                    vias.add(gw.spec.via)
             for gw in self:
                 if gw.id not in vias:
                     gw.exit()
 
-            def join_wait(gw):
+            def join_wait(gw: Gateway) -> None:
                 gw.join()
                 gw._io.wait()
 
-            def kill(gw):
+            def kill(gw: Gateway) -> None:
                 trace("Gateways did not come down after timeout: %r" % gw)
                 gw._io.kill()
 
             safe_terminate(
                 self.execmodel,
                 timeout,
                 [
                     (partial(join_wait, gw), partial(kill, gw))
                     for gw in self._gateways_to_join
                 ],
             )
             self._gateways_to_join[:] = []
 
-    def remote_exec(self, source, **kwargs):
+    def remote_exec(
+        self,
+        source: str | types.FunctionType | Callable[..., object] | types.ModuleType,
+        **kwargs,
+    ) -> MultiChannel:
         """remote_exec source on all member gateways and return
-        MultiChannel connecting to all sub processes.
-        """
+        a MultiChannel connecting to all sub processes."""
         channels = []
         for gw in self:
             channels.append(gw.remote_exec(source, **kwargs))
         return MultiChannel(channels)
 
 
 class MultiChannel:
-    def __init__(self, channels):
+    def __init__(self, channels: Sequence[Channel]) -> None:
         self._channels = channels
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._channels)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Channel]:
         return iter(self._channels)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: int) -> Channel:
         return self._channels[key]
 
-    def __contains__(self, chan):
+    def __contains__(self, chan: Channel) -> bool:
         return chan in self._channels
 
-    def send_each(self, item):
+    def send_each(self, item: object) -> None:
         for ch in self._channels:
             ch.send(item)
 
-    def receive_each(self, withchannel=False):
+    @overload
+    def receive_each(self, withchannel: Literal[False] = ...) -> list[Any]:
+        pass
+
+    @overload
+    def receive_each(self, withchannel: Literal[True]) -> list[tuple[Channel, Any]]:
+        pass
+
+    def receive_each(
+        self, withchannel: bool = False
+    ) -> list[tuple[Channel, Any]] | list[Any]:
         assert not hasattr(self, "_queue")
-        l = []
+        l: list[object] = []
         for ch in self._channels:
             obj = ch.receive()
             if withchannel:
                 l.append((ch, obj))
             else:
                 l.append(obj)
         return l
 
-    def make_receive_queue(self, endmarker=NO_ENDMARKER_WANTED):
+    def make_receive_queue(self, endmarker: object = NO_ENDMARKER_WANTED):
         try:
-            return self._queue
+            return self._queue  # type: ignore[has-type]
         except AttributeError:
             self._queue = None
             for ch in self._channels:
                 if self._queue is None:
                     self._queue = ch.gateway.execmodel.queue.Queue()
 
-                def putreceived(obj, channel=ch):
-                    self._queue.put((channel, obj))
+                def putreceived(obj, channel: Channel = ch) -> None:
+                    self._queue.put((channel, obj))  # type: ignore[union-attr]
 
                 if endmarker is NO_ENDMARKER_WANTED:
                     ch.setcallback(putreceived)
                 else:
                     ch.setcallback(putreceived, endmarker=endmarker)
             return self._queue
 
-    def waitclose(self):
+    def waitclose(self) -> None:
         first = None
         for ch in self._channels:
             try:
                 ch.waitclose()
-            except ch.RemoteError:
+            except ch.RemoteError as exc:
                 if first is None:
-                    first = sys.exc_info()
+                    first = exc
         if first:
-            raise first[1].with_traceback(first[2])
+            raise first
 
 
-def safe_terminate(execmodel, timeout, list_of_paired_functions):
+def safe_terminate(
+    execmodel: ExecModel, timeout: float | None, list_of_paired_functions
+) -> None:
     workerpool = WorkerPool(execmodel)
 
-    def termkill(termfunc, killfunc):
+    def termkill(termfunc, killfunc) -> None:
         termreply = workerpool.spawn(termfunc)
         try:
             termreply.get(timeout=timeout)
         except OSError:
             killfunc()
 
     replylist = []
```

### Comparing `execnet-2.0.2/src/execnet/rsync.py` & `execnet-2.1.0/src/execnet/rsync.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,104 @@
 """
 1:N rsync implementation on top of execnet.
 
 (c) 2006-2009, Armin Rigo, Holger Krekel, Maciej Fijalkowski
 """
+
+from __future__ import annotations
+
 import os
 import stat
 from hashlib import md5
 from queue import Queue
+from typing import Callable
+from typing import Literal
 
 import execnet.rsync_remote
+from execnet.gateway import Gateway
+from execnet.gateway_base import BaseGateway
+from execnet.gateway_base import Channel
 
 
 class RSync:
     """This class allows to send a directory structure (recursively)
     to one or multiple remote filesystems.
 
     There is limited support for symlinks, which means that symlinks
     pointing to the sourcetree will be send "as is" while external
     symlinks will be just copied (regardless of existence of such
     a path on remote side).
     """
 
-    def __init__(self, sourcedir, callback=None, verbose=True):
+    def __init__(self, sourcedir, callback=None, verbose: bool = True) -> None:
         self._sourcedir = str(sourcedir)
         self._verbose = verbose
-        assert callback is None or hasattr(callback, "__call__")
+        assert callback is None or callable(callback)
         self._callback = callback
-        self._channels = {}
-        self._receivequeue = Queue()
-        self._links = []
+        self._channels: dict[Channel, Callable[[], None] | None] = {}
+        self._receivequeue: Queue[
+            tuple[
+                Channel,
+                (
+                    None
+                    | tuple[Literal["send"], tuple[list[str], bytes]]
+                    | tuple[Literal["list_done"], None]
+                    | tuple[Literal["ack"], str]
+                    | tuple[Literal["links"], None]
+                    | tuple[Literal["done"], None]
+                ),
+            ]
+        ] = Queue()
+        self._links: list[tuple[Literal["linkbase", "link"], str, str]] = []
 
-    def filter(self, path):
+    def filter(self, path: str) -> bool:
         return True
 
-    def _end_of_channel(self, channel):
+    def _end_of_channel(self, channel: Channel) -> None:
         if channel in self._channels:
             # too early!  we must have got an error
             channel.waitclose()
             # or else we raise one
             raise OSError(f"connection unexpectedly closed: {channel.gateway} ")
 
-    def _process_link(self, channel):
+    def _process_link(self, channel: Channel) -> None:
         for link in self._links:
             channel.send(link)
         # completion marker, this host is done
         channel.send(42)
 
-    def _done(self, channel):
-        """Call all callbacks"""
+    def _done(self, channel: Channel) -> None:
+        """Call all callbacks."""
         finishedcallback = self._channels.pop(channel)
         if finishedcallback:
             finishedcallback()
         channel.waitclose()
 
-    def _list_done(self, channel):
+    def _list_done(self, channel: Channel) -> None:
         # sum up all to send
         if self._callback:
             s = sum([self._paths[i] for i in self._to_send[channel]])
             self._callback("list", s, channel)
 
-    def _send_item(self, channel, data):
-        """Send one item"""
-        modified_rel_path, checksum = data
-        modifiedpath = os.path.join(self._sourcedir, *modified_rel_path)
+    def _send_item(
+        self,
+        channel: Channel,
+        modified_rel_path_components: list[str],
+        checksum: bytes,
+    ) -> None:
+        """Send one item."""
+        modifiedpath = os.path.join(self._sourcedir, *modified_rel_path_components)
         try:
             f = open(modifiedpath, "rb")
             data = f.read()
         except OSError:
             data = None
 
         # provide info to progress callback function
-        modified_rel_path = "/".join(modified_rel_path)
+        modified_rel_path = "/".join(modified_rel_path_components)
         if data is not None:
             self._paths[modified_rel_path] = len(data)
         else:
             self._paths[modified_rel_path] = 0
         if channel not in self._to_send:
             self._to_send[channel] = []
         self._to_send[channel].append(modified_rel_path)
@@ -84,99 +108,108 @@
             f.close()
             if checksum is not None and checksum == md5(data).digest():
                 data = None  # not really modified
             else:
                 self._report_send_file(channel.gateway, modified_rel_path)
         channel.send(data)
 
-    def _report_send_file(self, gateway, modified_rel_path):
+    def _report_send_file(self, gateway: BaseGateway, modified_rel_path: str) -> None:
         if self._verbose:
             print(f"{gateway} <= {modified_rel_path}")
 
-    def send(self, raises=True):
-        """Sends a sourcedir to all added targets. Flag indicates
-        whether to raise an error or return in case of lack of
-        targets
+    def send(self, raises: bool = True) -> None:
+        """Sends a sourcedir to all added targets.
+
+        raises indicates whether to raise an error or return in case of lack of
+        targets.
         """
         if not self._channels:
             if raises:
                 raise OSError(
                     "no targets available, maybe you " "are trying call send() twice?"
                 )
             return
         # normalize a trailing '/' away
         self._sourcedir = os.path.dirname(os.path.join(self._sourcedir, "x"))
         # send directory structure and file timestamps/sizes
         self._send_directory_structure(self._sourcedir)
 
         # paths and to_send are only used for doing
         # progress-related callbacks
-        self._paths = {}
-        self._to_send = {}
+        self._paths: dict[str, int] = {}
+        self._to_send: dict[Channel, list[str]] = {}
 
         # send modified file to clients
         while self._channels:
             channel, req = self._receivequeue.get()
             if req is None:
                 self._end_of_channel(channel)
             else:
-                command, data = req
-                if command == "links":
+                if req[0] == "links":
                     self._process_link(channel)
-                elif command == "done":
+                elif req[0] == "done":
                     self._done(channel)
-                elif command == "ack":
+                elif req[0] == "ack":
                     if self._callback:
-                        self._callback("ack", self._paths[data], channel)
-                elif command == "list_done":
+                        self._callback("ack", self._paths[req[1]], channel)
+                elif req[0] == "list_done":
                     self._list_done(channel)
-                elif command == "send":
-                    self._send_item(channel, data)
-                    del data
+                elif req[0] == "send":
+                    self._send_item(channel, req[1][0], req[1][1])
                 else:
-                    assert "Unknown command %s" % command
+                    assert "Unknown command %s" % req[0]  # type: ignore[unreachable]
 
-    def add_target(self, gateway, destdir, finishedcallback=None, **options):
-        """Adds a remote target specified via a gateway
-        and a remote destination directory.
-        """
+    def add_target(
+        self,
+        gateway: Gateway,
+        destdir: str | os.PathLike[str],
+        finishedcallback: Callable[[], None] | None = None,
+        **options,
+    ) -> None:
+        """Add a remote target specified via a gateway and a remote destination
+        directory."""
         for name in options:
             assert name in ("delete",)
 
-        def itemcallback(req):
+        def itemcallback(req) -> None:
             self._receivequeue.put((channel, req))
 
         channel = gateway.remote_exec(execnet.rsync_remote)
         channel.reconfigure(py2str_as_py3str=False, py3str_as_py2str=False)
         channel.setcallback(itemcallback, endmarker=None)
         channel.send((str(destdir), options))
         self._channels[channel] = finishedcallback
 
-    def _broadcast(self, msg):
+    def _broadcast(self, msg: object) -> None:
         for channel in self._channels:
             channel.send(msg)
 
-    def _send_link(self, linktype, basename, linkpoint):
+    def _send_link(
+        self,
+        linktype: Literal["linkbase", "link"],
+        basename: str,
+        linkpoint: str,
+    ) -> None:
         self._links.append((linktype, basename, linkpoint))
 
-    def _send_directory(self, path):
+    def _send_directory(self, path: str) -> None:
         # dir: send a list of entries
         names = []
         subpaths = []
         for name in os.listdir(path):
             p = os.path.join(path, name)
             if self.filter(p):
                 names.append(name)
                 subpaths.append(p)
         mode = os.lstat(path).st_mode
-        self._broadcast([mode] + names)
+        self._broadcast([mode, *names])
         for p in subpaths:
             self._send_directory_structure(p)
 
-    def _send_link_structure(self, path):
+    def _send_link_structure(self, path: str) -> None:
         sourcedir = self._sourcedir
         basename = path[len(self._sourcedir) + 1 :]
         linkpoint = os.readlink(path)
         # On Windows, readlink returns an extended path (//?/) for
         # absolute links, but relpath doesn't like mixing extended
         # and non-extended paths. So fix it up ourselves.
         if (
@@ -185,24 +218,26 @@
             and not self._sourcedir.startswith("\\\\?\\")
         ):
             sourcedir = "\\\\?\\" + self._sourcedir
         try:
             relpath = os.path.relpath(linkpoint, sourcedir)
         except ValueError:
             relpath = None
-        if relpath not in (None, os.curdir, os.pardir) and not relpath.startswith(
-            os.pardir + os.sep
+        if (
+            relpath is not None
+            and relpath not in (os.curdir, os.pardir)
+            and not relpath.startswith(os.pardir + os.sep)
         ):
             self._send_link("linkbase", basename, relpath)
         else:
             # relative or absolute link, just send it
             self._send_link("link", basename, linkpoint)
         self._broadcast(None)
 
-    def _send_directory_structure(self, path):
+    def _send_directory_structure(self, path: str) -> None:
         try:
             st = os.lstat(path)
         except OSError:
             self._broadcast((None, 0, 0))
             return
         if stat.S_ISREG(st.st_mode):
             # regular file: send a mode/timestamp/size pair
```

### Comparing `execnet-2.0.2/src/execnet/rsync_remote.py` & `execnet-2.1.0/src/execnet/rsync_remote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """
 (c) 2006-2013, Armin Rigo, Holger Krekel, Maciej Fijalkowski
 """
 
+from __future__ import annotations
 
-def serve_rsync(channel):
+from typing import TYPE_CHECKING
+from typing import Literal
+from typing import cast
+
+if TYPE_CHECKING:
+    from execnet.gateway_base import Channel
+
+
+def serve_rsync(channel: Channel) -> None:
     import os
-    import stat
     import shutil
+    import stat
     from hashlib import md5
 
-    destdir, options = channel.receive()
+    destdir, options = cast("tuple[str, dict[str, object]]", channel.receive())
     modifiedfiles = []
 
-    def remove(path):
+    def remove(path: str) -> None:
         assert path.startswith(destdir)
         try:
             os.unlink(path)
         except OSError:
             # assume it's a dir
             shutil.rmtree(path, True)
 
-    def receive_directory_structure(path, relcomponents):
+    def receive_directory_structure(path: str, relcomponents: list[str]) -> None:
         try:
             st = os.lstat(path)
         except OSError:
             st = None
         msg = channel.receive()
         if isinstance(msg, list):
             if st and not stat.S_ISDIR(st.st_mode):
@@ -38,15 +47,15 @@
                 # permission denied error (EACCES) would be raised
                 # when attempting to receive read-only directory
                 # structures.
                 os.chmod(path, mode | 0o700)
             entrynames = {}
             for entryname in msg:
                 destpath = os.path.join(path, entryname)
-                receive_directory_structure(destpath, relcomponents + [entryname])
+                receive_directory_structure(destpath, [*relcomponents, entryname])
                 entrynames[entryname] = True
             if options.get("delete"):
                 for othername in os.listdir(path):
                     if othername not in entrynames:
                         otherpath = os.path.join(path, othername)
                         remove(otherpath)
         elif msg is not None:
@@ -73,15 +82,15 @@
 
     receive_directory_structure(destdir, [])
 
     STRICT_CHECK = False  # seems most useful this way for py.test
     channel.send(("list_done", None))
 
     for path, (mode, time, size) in modifiedfiles:
-        data = channel.receive()
+        data = cast(bytes, channel.receive())
         channel.send(("ack", path[len(destdir) + 1 :]))
         if data is not None:
             if STRICT_CHECK and len(data) != size:
                 raise OSError(f"file modified during rsync: {path!r}")
             f = open(path, "wb")
             f.write(data)
             f.close()
@@ -93,15 +102,17 @@
             pass
         del data
     channel.send(("links", None))
 
     msg = channel.receive()
     while msg != 42:
         # we get symlink
-        _type, relpath, linkpoint = msg
+        _type, relpath, linkpoint = cast(
+            "tuple[Literal['linkbase', 'link'], str, str]", msg
+        )
         path = os.path.join(destdir, relpath)
         try:
             remove(path)
         except OSError:
             pass
         if _type == "linkbase":
             src = os.path.join(destdir, linkpoint)
@@ -110,8 +121,8 @@
             src = linkpoint
         os.symlink(src, path)
         msg = channel.receive()
     channel.send(("done", None))
 
 
 if __name__ == "__channelexec__":
-    serve_rsync(channel)  # type: ignore[name-defined]
+    serve_rsync(channel)  # type: ignore[name-defined]  # noqa:F821
```

### Comparing `execnet-2.0.2/src/execnet/script/shell.py` & `execnet-2.1.0/src/execnet/script/shell.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 #! /usr/bin/env python
 """
 a remote python shell
 
 for injection into startserver.py
 """
+
 import os
 import select
 import socket
 import sys
 from threading import Thread
 from traceback import print_exc
+from typing import NoReturn
 
 
-def clientside():
+def clientside() -> NoReturn:
     print("client side starting")
-    host, port = sys.argv[1].split(":")
-    port = int(port)
+    host, portstr = sys.argv[1].split(":")
+    port = int(portstr)
     myself = open(os.path.abspath(sys.argv[0])).read()
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.connect((host, port))
-    sock.sendall(repr(myself) + "\n")
+    sock.sendall((repr(myself) + "\n").encode())
     print("send boot string")
     inputlist = [sock, sys.stdin]
     try:
         while 1:
             r, w, e = select.select(inputlist, [], [])
             if sys.stdin in r:
-                line = raw_input()
-                sock.sendall(line + "\n")
+                line = input()
+                sock.sendall((line + "\n").encode())
             if sock in r:
-                line = sock.recv(4096)
+                line = sock.recv(4096).decode()
                 sys.stdout.write(line)
                 sys.stdout.flush()
     except BaseException:
         import traceback
 
-        print(traceback.print_exc())
+        traceback.print_exc()
 
     sys.exit(1)
 
 
 class promptagent(Thread):
-    def __init__(self, clientsock):
+    def __init__(self, clientsock) -> None:
         print("server side starting")
-        super.__init__()
+        super.__init__()  # type: ignore[call-overload]
         self.clientsock = clientsock
 
-    def run(self):
+    def run(self) -> None:
         print("Entering thread prompt loop")
         clientfile = self.clientsock.makefile("w")
 
         filein = self.clientsock.makefile("r")
         loc = self.clientsock.getsockname()
 
         while 1:
             try:
-                clientfile.write("%s %s >>> " % loc)
+                clientfile.write("{} {} >>> ".format(*loc))
                 clientfile.flush()
                 line = filein.readline()
                 if not line:
                     raise EOFError("nothing")
                 if line.strip():
                     oldout, olderr = sys.stdout, sys.stderr
                     sys.stdout, sys.stderr = clientfile, clientfile
```

### Comparing `execnet-2.0.2/src/execnet/script/socketserver.py` & `execnet-2.1.0/src/execnet/script/socketserver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 #! /usr/bin/env python
 """
-    start socket based minimal readline exec server
+start socket based minimal readline exec server
 
-    it can exeuted in 2 modes of operation
+it can exeuted in 2 modes of operation
 
-    1. as normal script, that listens for new connections
+1. as normal script, that listens for new connections
 
-    2. via existing_gateway.remote_exec (as imported module)
+2. via existing_gateway.remote_exec (as imported module)
 
 """
+
 # this part of the program only executes on the server side
 #
+from __future__ import annotations
+
 import os
 import sys
+from typing import TYPE_CHECKING
 
-progname = "socket_readline_exec_server-1.2"
-
-
-def get_fcntl():
-    try:
-        import fcntl
-    except ImportError:
-        fcntl = None
-    return fcntl
+try:
+    import fcntl
+except ImportError:
+    fcntl = None  # type: ignore[assignment]
+
+if TYPE_CHECKING:
+    from execnet.gateway_base import Channel
+    from execnet.gateway_base import ExecModel
 
+progname = "socket_readline_exec_server-1.2"
 
-fcntl = get_fcntl()
 
 debug = 0
 
 if debug:  # and not os.isatty(sys.stdin.fileno())
     f = open("/tmp/execnet-socket-pyout.log", "w")
     old = sys.stdout, sys.stderr
     sys.stdout = sys.stderr = f
 
 
-def print_(*args):
+def print_(*args) -> None:
     print(" ".join(str(arg) for arg in args))
 
 
 exec(
     """def exec_(source, locs):
     exec(source, locs)"""
 )
 
 
-def exec_from_one_connection(serversock):
+def exec_from_one_connection(serversock) -> None:
     print_(progname, "Entering Accept loop", serversock.getsockname())
     clientsock, address = serversock.accept()
-    print_(progname, "got new connection from %s %s" % address)
+    print_(progname, "got new connection from {} {}".format(*address))
     clientfile = clientsock.makefile("rb")
     print_("reading line")
     # rstrip so that we can use \r\n for telnet testing
     source = clientfile.readline().rstrip()
     clientfile.close()
     g = {"clientsock": clientsock, "address": address, "execmodel": execmodel}
     source = eval(source)
     if source:
         co = compile(source + "\n", "<socket server>", "exec")
         print_(progname, "compiled source, executing")
         try:
-            exec_(co, g)  # noqa
+            exec_(co, g)  # type: ignore[name-defined] # noqa: F821
         finally:
             print_(progname, "finished executing code")
             # background thread might hold a reference to this (!?)
             # clientsock.close()
 
 
-def bind_and_listen(hostport, execmodel):
+def bind_and_listen(hostport: str | tuple[str, int], execmodel: ExecModel):
     socket = execmodel.socket
     if isinstance(hostport, str):
         host, port = hostport.split(":")
         hostport = (host, int(port))
     serversock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     # set close-on-exec
     if hasattr(fcntl, "FD_CLOEXEC"):
@@ -82,30 +85,29 @@
         serversock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
     serversock.bind(hostport)
     serversock.listen(5)
     return serversock
 
 
-def startserver(serversock, loop=False):
+def startserver(serversock, loop: bool = False) -> None:
     execute_path = os.getcwd()
     try:
         while 1:
             try:
                 exec_from_one_connection(serversock)
             except (KeyboardInterrupt, SystemExit):
                 raise
-            except BaseException:
+            except BaseException as exc:
                 if debug:
                     import traceback
 
                     traceback.print_exc()
                 else:
-                    excinfo = sys.exc_info()
-                    print_("got exception", excinfo[1])
+                    print_("got exception", exc)
             os.chdir(execute_path)
             if not loop:
                 break
     finally:
         print_("leaving socketserver execloop")
         serversock.shutdown(2)
 
@@ -120,14 +122,15 @@
     from execnet.gateway_base import get_execmodel
 
     execmodel = get_execmodel("thread")
     serversock = bind_and_listen(hostport, execmodel)
     startserver(serversock, loop=True)
 
 elif __name__ == "__channelexec__":
-    chan = globals()["channel"]
+    chan: Channel = globals()["channel"]
     execmodel = chan.gateway.execmodel
     bindname = chan.receive()
+    assert isinstance(bindname, (str, tuple))
     sock = bind_and_listen(bindname, execmodel)
     port = sock.getsockname()
     chan.send(port)
     startserver(sock)
```

### Comparing `execnet-2.0.2/src/execnet/script/socketserverservice.py` & `execnet-2.1.0/src/execnet/script/socketserverservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """
 A windows service wrapper for the py.execnet socketserver.
 
 To use, run:
  python socketserverservice.py register
  net start ExecNetSocketServer
 """
-import socketserver
+
 import sys
 import threading
 
 import servicemanager
 import win32event
 import win32evtlogutil
 import win32service
 import win32serviceutil
 
+from execnet.gateway_base import get_execmodel
+
+from . import socketserver
 
 appname = "ExecNetSocketServer"
 
 
 class SocketServerService(win32serviceutil.ServiceFramework):
     _svc_name_ = appname
     _svc_display_name_ = "%s" % appname
     _svc_deps_ = ["EventLog"]
 
-    def __init__(self, args):
+    def __init__(self, args) -> None:
         # The exe-file has messages for the Event Log Viewer.
         # Register the exe-file as event source.
         #
         # Probably it would be better if this is done at installation time,
         # so that it also could be removed if the service is uninstalled.
         # Unfortunately it cannot be done in the 'if __name__ == "__main__"'
         # block below, because the 'frozen' exe-file does not run this code.
@@ -36,19 +39,19 @@
         win32evtlogutil.AddSourceToRegistry(
             self._svc_display_name_, servicemanager.__file__, "Application"
         )
         super.__init__(args)
         self.hWaitStop = win32event.CreateEvent(None, 0, 0, None)
         self.WAIT_TIME = 1000  # in milliseconds
 
-    def SvcStop(self):
+    def SvcStop(self) -> None:
         self.ReportServiceStatus(win32service.SERVICE_STOP_PENDING)
         win32event.SetEvent(self.hWaitStop)
 
-    def SvcDoRun(self):
+    def SvcDoRun(self) -> None:
         # Redirect stdout and stderr to prevent "IOError: [Errno 9]
         # Bad file descriptor". Windows services don't have functional
         # output streams.
         sys.stdout = sys.stderr = open("nul", "w")
 
         # Write a 'started' event to the event log...
         win32evtlogutil.ReportEvent(
@@ -58,15 +61,16 @@
             servicemanager.EVENTLOG_INFORMATION_TYPE,
             (self._svc_name_, ""),
         )
         print("Begin: %s" % self._svc_display_name_)
 
         hostport = ":8888"
         print("Starting py.execnet SocketServer on %s" % hostport)
-        serversock = socketserver.bind_and_listen(hostport)
+        exec_model = get_execmodel("thread")
+        serversock = socketserver.bind_and_listen(hostport, exec_model)
         thread = threading.Thread(
             target=socketserver.startserver, args=(serversock,), kwargs={"loop": True}
         )
         thread.setDaemon(True)
         thread.start()
 
         # wait to be stopped or self.WAIT_TIME to pass
```

### Comparing `execnet-2.0.2/testing/conftest.py` & `execnet-2.1.0/testing/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+from __future__ import annotations
+
 import shutil
 import sys
 from functools import lru_cache
 from typing import Callable
+from typing import Generator
 from typing import Iterator
 
 import execnet
 import pytest
-from execnet.gateway_base import get_execmodel
+from execnet.gateway import Gateway
+from execnet.gateway_base import ExecModel
 from execnet.gateway_base import WorkerPool
+from execnet.gateway_base import get_execmodel
 
 collect_ignore = ["build", "doc/_build"]
 
 rsyncdirs = ["conftest.py", "execnet", "testing", "doc"]
 
 
 @pytest.hookimpl(hookwrapper=True)
-def pytest_runtest_setup(item):
+def pytest_runtest_setup(item: pytest.Item) -> Generator[None, None, None]:
     if item.fspath.purebasename in ("test_group", "test_info"):
         getspecssh(item.config)  # will skip if no gx given
     yield
     if "pypy" in item.keywords and not item.config.option.pypy:
         pytest.skip("pypy tests skipped, use --pypy to run them.")
 
 
@@ -27,23 +32,23 @@
 def group_function() -> Iterator[execnet.Group]:
     group = execnet.Group()
     yield group
     group.terminate(0.5)
 
 
 @pytest.fixture
-def makegateway(group_function) -> Callable[[str], execnet.gateway.Gateway]:
+def makegateway(group_function: execnet.Group) -> Callable[[str], Gateway]:
     return group_function.makegateway
 
 
 pytest_plugins = ["pytester", "doctest"]
 
 
 # configuration information for tests
-def pytest_addoption(parser):
+def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup("execnet", "execnet testing options")
     group.addoption(
         "--gx",
         action="append",
         dest="gspecs",
         default=None,
         help="add a global test environment, XSpec-syntax. ",
@@ -62,104 +67,109 @@
             "Skips tests that assume your ISP doesn't put up a landing "
             "page on invalid addresses"
         ),
     )
 
 
 @pytest.fixture
-def specssh(request):
+def specssh(request: pytest.FixtureRequest) -> execnet.XSpec:
     return getspecssh(request.config)
 
 
 @pytest.fixture
-def specsocket(request):
+def specsocket(request: pytest.FixtureRequest) -> execnet.XSpec:
     return getsocketspec(request.config)
 
 
-def getgspecs(config):
-    return map(execnet.XSpec, config.getvalueorskip("gspecs"))
+def getgspecs(config: pytest.Config) -> list[execnet.XSpec]:
+    return [execnet.XSpec(gspec) for gspec in config.getvalueorskip("gspecs")]
 
 
-def getspecssh(config):
+def getspecssh(config: pytest.Config) -> execnet.XSpec:
     xspecs = getgspecs(config)
     for spec in xspecs:
         if spec.ssh:
             if not shutil.which("ssh"):
                 pytest.skip("command not found: ssh")
             return spec
     pytest.skip("need '--gx ssh=...'")
 
 
-def getsocketspec(config):
+def getsocketspec(config: pytest.Config) -> execnet.XSpec:
     xspecs = getgspecs(config)
     for spec in xspecs:
         if spec.socket:
             return spec
     pytest.skip("need '--gx socket=...'")
 
 
-def pytest_generate_tests(metafunc):
+def pytest_generate_tests(metafunc: pytest.Metafunc) -> None:
     if "gw" in metafunc.fixturenames:
         assert "anypython" not in metafunc.fixturenames, "need combine?"
         if hasattr(metafunc.function, "gwtypes"):
             gwtypes = metafunc.function.gwtypes
         elif hasattr(metafunc.cls, "gwtype"):
             gwtypes = [metafunc.cls.gwtype]
         else:
             gwtypes = ["popen", "socket", "ssh", "proxy"]
         metafunc.parametrize("gw", gwtypes, indirect=True)
 
 
-@lru_cache()
-def getexecutable(name):
+@lru_cache
+def getexecutable(name: str) -> str | None:
     if name == "sys.executable":
         return sys.executable
     return shutil.which(name)
 
 
 @pytest.fixture(params=("sys.executable", "pypy3"))
-def anypython(request):
+def anypython(request: pytest.FixtureRequest) -> str:
     name = request.param
     executable = getexecutable(name)
     if executable is None:
         pytest.skip(f"no {name} found")
     if "execmodel" in request.fixturenames and name != "sys.executable":
         backend = request.getfixturevalue("execmodel").backend
-        if backend != "thread":
+        if backend not in ("thread", "main_thread_only"):
             pytest.xfail(f"cannot run {backend!r} execmodel with bare {name}")
     return executable
 
 
 @pytest.fixture(scope="session")
-def group():
+def group() -> Iterator[execnet.Group]:
     g = execnet.Group()
     yield g
     g.terminate(timeout=1)
 
 
 @pytest.fixture
-def gw(request, execmodel, group):
+def gw(
+    request: pytest.FixtureRequest,
+    execmodel: ExecModel,
+    group: execnet.Group,
+) -> Gateway:
     try:
         return group[request.param]
     except KeyError:
         if request.param == "popen":
             gw = group.makegateway("popen//id=popen//execmodel=%s" % execmodel.backend)
         elif request.param == "socket":
             # if execmodel.backend != "thread":
             #    pytest.xfail(
             #        "cannot set remote non-thread execmodel for sockets")
             pname = "sproxy1"
             if pname not in group:
                 proxygw = group.makegateway("popen//id=%s" % pname)
             # assert group['proxygw'].remote_status().receiving
             gw = group.makegateway(
-                "socket//id=socket//installvia=%s"
-                "//execmodel=%s" % (pname, execmodel.backend)
+                f"socket//id=socket//installvia={pname}"
+                f"//execmodel={execmodel.backend}"
             )
-            gw.proxygw = proxygw
+            # TODO(typing): Clarify this assignment.
+            gw.proxygw = proxygw  # type: ignore[attr-defined]
             assert pname in group
         elif request.param == "ssh":
             sshhost = request.getfixturevalue("specssh").ssh
             # we don't use execmodel.backend here
             # but you can set it when specifying the ssh spec
             gw = group.makegateway(f"ssh={sshhost}//id=ssh")
         elif request.param == "proxy":
@@ -169,19 +179,21 @@
                 "//execmodel=%s" % execmodel.backend
             )
         else:
             assert 0, f"unknown execmodel: {request.param}"
         return gw
 
 
-@pytest.fixture(params=["thread", "eventlet", "gevent"], scope="session")
-def execmodel(request):
-    if request.param != "thread":
+@pytest.fixture(
+    params=["thread", "main_thread_only", "eventlet", "gevent"], scope="session"
+)
+def execmodel(request: pytest.FixtureRequest) -> ExecModel:
+    if request.param not in ("thread", "main_thread_only"):
         pytest.importorskip(request.param)
     if request.param in ("eventlet", "gevent") and sys.platform == "win32":
         pytest.xfail(request.param + " does not work on win32")
     return get_execmodel(request.param)
 
 
 @pytest.fixture
-def pool(execmodel):
+def pool(execmodel: ExecModel) -> WorkerPool:
     return WorkerPool(execmodel=execmodel)
```

### Comparing `execnet-2.0.2/testing/test_channel.py` & `execnet-2.1.0/testing/test_channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,165 @@
 """
 mostly functional tests of gateways.
 """
+
+from __future__ import annotations
+
 import time
 
 import pytest
-
+from execnet.gateway import Gateway
+from execnet.gateway_base import Channel
 
 needs_early_gc = pytest.mark.skipif("not hasattr(sys, 'getrefcount')")
 needs_osdup = pytest.mark.skipif("not hasattr(os, 'dup')")
 TESTTIMEOUT = 10.0  # seconds
 
 
 class TestChannelBasicBehaviour:
-    def test_serialize_error(self, gw):
+    def test_serialize_error(self, gw: Gateway) -> None:
         ch = gw.remote_exec("channel.send(ValueError(42))")
         excinfo = pytest.raises(ch.RemoteError, ch.receive)
         assert "can't serialize" in str(excinfo.value)
 
-    def test_channel_close_and_then_receive_error(self, gw):
+    def test_channel_close_and_then_receive_error(self, gw: Gateway) -> None:
         channel = gw.remote_exec("raise ValueError")
         pytest.raises(channel.RemoteError, channel.receive)
 
-    def test_channel_finish_and_then_EOFError(self, gw):
+    def test_channel_finish_and_then_EOFError(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.send(42)")
         x = channel.receive()
         assert x == 42
         pytest.raises(EOFError, channel.receive)
         pytest.raises(EOFError, channel.receive)
         pytest.raises(EOFError, channel.receive)
 
-    def test_waitclose_timeouterror(self, gw):
+    def test_waitclose_timeouterror(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.receive()")
         pytest.raises(channel.TimeoutError, channel.waitclose, 0.02)
         channel.send(1)
         channel.waitclose(timeout=TESTTIMEOUT)
 
-    def test_channel_receive_timeout(self, gw):
+    def test_channel_receive_timeout(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.send(channel.receive())")
         with pytest.raises(channel.TimeoutError):
             channel.receive(timeout=0.2)
         channel.send(1)
         channel.receive(timeout=TESTTIMEOUT)
 
-    def test_channel_receive_internal_timeout(self, gw, monkeypatch):
+    def test_channel_receive_internal_timeout(
+        self, gw: Gateway, monkeypatch: pytest.MonkeyPatch
+    ) -> None:
         channel = gw.remote_exec(
             """
             import time
             time.sleep(0.5)
             channel.send(1)
         """
         )
         monkeypatch.setattr(channel.__class__, "_INTERNALWAKEUP", 0.2)
         channel.receive()
 
-    def test_channel_close_and_then_receive_error_multiple(self, gw):
+    def test_channel_close_and_then_receive_error_multiple(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.send(42) ; raise ValueError")
         x = channel.receive()
         assert x == 42
         pytest.raises(channel.RemoteError, channel.receive)
 
-    def test_channel__local_close(self, gw):
+    def test_channel__local_close(self, gw: Gateway) -> None:
         channel = gw._channelfactory.new()
         gw._channelfactory._local_close(channel.id)
         channel.waitclose(0.1)
 
-    def test_channel__local_close_error(self, gw):
+    def test_channel__local_close_error(self, gw: Gateway) -> None:
         channel = gw._channelfactory.new()
         gw._channelfactory._local_close(channel.id, channel.RemoteError("error"))
         pytest.raises(channel.RemoteError, channel.waitclose, 0.01)
 
-    def test_channel_error_reporting(self, gw):
+    def test_channel_error_reporting(self, gw: Gateway) -> None:
         channel = gw.remote_exec("def foo():\n  return foobar()\nfoo()\n")
         excinfo = pytest.raises(channel.RemoteError, channel.receive)
         msg = str(excinfo.value)
         assert msg.startswith("Traceback (most recent call last):")
         assert "NameError" in msg
         assert "foobar" in msg
 
-    def test_channel_syntax_error(self, gw):
+    def test_channel_syntax_error(self, gw: Gateway) -> None:
         # missing colon
         channel = gw.remote_exec("def foo()\n return 1\nfoo()\n")
         excinfo = pytest.raises(channel.RemoteError, channel.receive)
         msg = str(excinfo.value)
         assert msg.startswith("Traceback (most recent call last):")
         assert "SyntaxError" in msg
 
-    def test_channel_iter(self, gw):
+    def test_channel_iter(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
               for x in range(3):
                 channel.send(x)
         """
         )
         l = list(channel)
         assert l == [0, 1, 2]
 
-    def test_channel_pass_in_structure(self, gw):
+    def test_channel_pass_in_structure(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             ch1, ch2 = channel.receive()
             data = ch1.receive()
             ch2.send(data+1)
         """
         )
         newchan1 = gw.newchannel()
         newchan2 = gw.newchannel()
         channel.send((newchan1, newchan2))
         newchan1.send(1)
         data = newchan2.receive()
         assert data == 2
 
-    def test_channel_multipass(self, gw):
+    def test_channel_multipass(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             channel.send(channel)
             xchan = channel.receive()
             assert xchan == channel
         """
         )
         newchan = channel.receive()
         assert newchan == channel
         channel.send(newchan)
         channel.waitclose()
 
-    def test_channel_passing_over_channel(self, gw):
+    def test_channel_passing_over_channel(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
-                    c = channel.gateway.newchannel()
-                    channel.send(c)
-                    c.send(42)
-                  """
+            c = channel.gateway.newchannel()
+            channel.send(c)
+            c.send(42)
+            """
         )
         c = channel.receive()
+        assert isinstance(c, Channel)
         x = c.receive()
         assert x == 42
 
         # check that the both sides previous channels are really gone
         channel.waitclose(TESTTIMEOUT)
         # assert c.id not in gw._channelfactory
         newchan = gw.remote_exec(
             """
-                    assert %d not in channel.gateway._channelfactory._channels
-                  """
+            assert %d not in channel.gateway._channelfactory._channels
+            """
             % channel.id
         )
         newchan.waitclose(TESTTIMEOUT)
         assert channel.id not in gw._channelfactory._channels
 
-    def test_channel_receiver_callback(self, gw):
-        l = []
+    def test_channel_receiver_callback(self, gw: Gateway) -> None:
+        l: list[int] = []
         # channel = gw.newchannel(receiver=l.append)
         channel = gw.remote_exec(
             source="""
             channel.send(42)
             channel.send(13)
             channel.send(channel.gateway.newchannel())
             """
@@ -160,16 +167,16 @@
         channel.setcallback(callback=l.append)
         pytest.raises(IOError, channel.receive)
         channel.waitclose(TESTTIMEOUT)
         assert len(l) == 3
         assert l[:2] == [42, 13]
         assert isinstance(l[2], channel.__class__)
 
-    def test_channel_callback_after_receive(self, gw):
-        l = []
+    def test_channel_callback_after_receive(self, gw: Gateway) -> None:
+        l: list[int] = []
         channel = gw.remote_exec(
             source="""
             channel.send(42)
             channel.send(13)
             channel.send(channel.gateway.newchannel())
             """
         )
@@ -178,40 +185,42 @@
         channel.setcallback(callback=l.append)
         pytest.raises(IOError, channel.receive)
         channel.waitclose(TESTTIMEOUT)
         assert len(l) == 2
         assert l[0] == 13
         assert isinstance(l[1], channel.__class__)
 
-    def test_waiting_for_callbacks(self, gw):
+    def test_waiting_for_callbacks(self, gw: Gateway) -> None:
         l = []
 
-        def callback(msg):
+        def callback(msg) -> None:
             import time
 
             time.sleep(0.2)
             l.append(msg)
 
         channel = gw.remote_exec(
             source="""
             channel.send(42)
             """
         )
         channel.setcallback(callback)
         channel.waitclose(TESTTIMEOUT)
         assert l == [42]
 
-    def test_channel_callback_stays_active(self, gw):
+    def test_channel_callback_stays_active(self, gw: Gateway) -> None:
         self.check_channel_callback_stays_active(gw, earlyfree=True)
 
-    def check_channel_callback_stays_active(self, gw, earlyfree=True):
+    def check_channel_callback_stays_active(
+        self, gw: Gateway, earlyfree: bool = True
+    ) -> Channel | None:
         if gw.spec.execmodel == "gevent":
             pytest.xfail("investigate gevent failure")
         # with 'earlyfree==True', this tests the "sendonly" channel state.
-        l = []
+        l: list[int] = []
         channel = gw.remote_exec(
             source="""
             import _thread
             import time
             def producer(subchannel):
                 for i in range(5):
                     time.sleep(0.15)
@@ -220,36 +229,36 @@
             _thread.start_new_thread(producer, (channel2,))
             del channel2
             """
         )
         subchannel = gw.newchannel()
         subchannel.setcallback(l.append)
         channel.send(subchannel)
-        if earlyfree:
-            subchannel = None
+        subchan = None if earlyfree else subchannel
         counter = 100
         while len(l) < 5:
-            if subchannel and subchannel.isclosed():
+            if subchan and subchan.isclosed():
                 break
             counter -= 1
             print(counter)
             if not counter:
                 pytest.fail("timed out waiting for the answer[%d]" % len(l))
             time.sleep(0.04)  # busy-wait
         assert l == [0, 100, 200, 300, 400]
-        return subchannel
+        return subchan
 
     @needs_early_gc
-    def test_channel_callback_remote_freed(self, gw):
+    def test_channel_callback_remote_freed(self, gw: Gateway) -> None:
         channel = self.check_channel_callback_stays_active(gw, earlyfree=False)
+        assert channel is not None
         # freed automatically at the end of producer()
         channel.waitclose(TESTTIMEOUT)
 
-    def test_channel_endmarker_callback(self, gw):
-        l = []
+    def test_channel_endmarker_callback(self, gw: Gateway) -> None:
+        l: list[int | Channel] = []
         channel = gw.remote_exec(
             source="""
             channel.send(42)
             channel.send(13)
             channel.send(channel.gateway.newchannel())
             """
         )
@@ -257,86 +266,89 @@
         pytest.raises(IOError, channel.receive)
         channel.waitclose(TESTTIMEOUT)
         assert len(l) == 4
         assert l[:2] == [42, 13]
         assert isinstance(l[2], channel.__class__)
         assert l[3] == 999
 
-    def test_channel_endmarker_callback_error(self, gw):
+    def test_channel_endmarker_callback_error(self, gw: Gateway) -> None:
         q = gw.execmodel.queue.Queue()
         channel = gw.remote_exec(
             source="""
             raise ValueError()
         """
         )
         channel.setcallback(q.put, endmarker=999)
         val = q.get(TESTTIMEOUT)
         assert val == 999
         err = channel._getremoteerror()
         assert err
         assert str(err).find("ValueError") != -1
 
-    def test_channel_callback_error(self, gw):
+    def test_channel_callback_error(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             def f(item):
                 raise ValueError(42)
             ch = channel.gateway.newchannel()
             ch.setcallback(f)
             channel.send(ch)
             channel.receive()
             assert ch.isclosed()
         """
         )
         subchan = channel.receive()
+        assert isinstance(subchan, Channel)
         subchan.send(1)
         with pytest.raises(subchan.RemoteError) as excinfo:
             subchan.waitclose(TESTTIMEOUT)
         assert "42" in excinfo.value.formatted
         channel.send(1)
         channel.waitclose()
 
 
 class TestChannelFile:
-    def test_channel_file_write(self, gw):
+    def test_channel_file_write(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             f = channel.makefile()
             f.write("hello world\\n")
             f.close()
             channel.send(42)
         """
         )
         first = channel.receive()
+        assert isinstance(first, str)
         assert first.strip() == "hello world"
         second = channel.receive()
         assert second == 42
 
-    def test_channel_file_write_error(self, gw):
+    def test_channel_file_write_error(self, gw: Gateway) -> None:
         channel = gw.remote_exec("pass")
         f = channel.makefile()
         assert not f.isatty()
         channel.waitclose(TESTTIMEOUT)
         with pytest.raises(IOError):
-            f.write("hello")
+            f.write(b"hello")
 
-    def test_channel_file_proxyclose(self, gw):
+    def test_channel_file_proxyclose(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             f = channel.makefile(proxyclose=True)
             f.write("hello world")
             f.close()
             channel.send(42)
         """
         )
         first = channel.receive()
+        assert isinstance(first, str)
         assert first.strip() == "hello world"
         pytest.raises(channel.RemoteError, channel.receive)
 
-    def test_channel_file_read(self, gw):
+    def test_channel_file_read(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             f = channel.makefile(mode='r')
             s = f.read(2)
             channel.send(s)
             s = f.read(5)
             channel.send(s)
@@ -344,32 +356,32 @@
         )
         channel.send("xyabcde")
         s1 = channel.receive()
         s2 = channel.receive()
         assert s1 == "xy"
         assert s2 == "abcde"
 
-    def test_channel_file_read_empty(self, gw):
+    def test_channel_file_read_empty(self, gw: Gateway) -> None:
         channel = gw.remote_exec("pass")
         f = channel.makefile(mode="r")
         s = f.read(3)
         assert s == ""
         s = f.read(5)
         assert s == ""
 
-    def test_channel_file_readline_remote(self, gw):
+    def test_channel_file_readline_remote(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             channel.send('123\\n45')
         """
         )
         channel.waitclose(TESTTIMEOUT)
         f = channel.makefile(mode="r")
         s = f.readline()
         assert s == "123\n"
         s = f.readline()
         assert s == "45"
 
-    def test_channel_makefile_incompatmode(self, gw):
+    def test_channel_makefile_incompatmode(self, gw: Gateway) -> None:
         channel = gw.newchannel()
         with pytest.raises(ValueError):
-            channel.makefile("rw")
+            channel.makefile("rw")  # type: ignore[call-overload]
```

### Comparing `execnet-2.0.2/testing/test_compatibility_regressions.py` & `execnet-2.1.0/testing/test_compatibility_regressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from execnet import gateway_base
 
 
-def test_opcodes():
+def test_opcodes() -> None:
     data = vars(gateway_base.opcode)
     computed = {k: v for k, v in data.items() if "__" not in k}
     assert computed == {
         "BUILDTUPLE": b"@",
         "BYTES": b"A",
         "CHANNEL": b"B",
         "FALSE": b"C",
```

### Comparing `execnet-2.0.2/testing/test_gateway.py` & `execnet-2.1.0/testing/test_gateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 mostly functional tests of gateways.
 """
+
+from __future__ import annotations
+
 import os
 import pathlib
 import shutil
 import signal
 import sys
 from textwrap import dedent
+from typing import Callable
 
 import execnet
 import pytest
 from execnet import gateway_base
 from execnet import gateway_io
+from execnet.gateway import Gateway
 
 TESTTIMEOUT = 10.0  # seconds
 needs_osdup = pytest.mark.skipif("not hasattr(os, 'dup')")
 
 
 flakytest = pytest.mark.xfail(
     reason="on some systems this test fails due to timing problems"
@@ -23,33 +28,33 @@
 skip_win_pypy = pytest.mark.xfail(
     condition=hasattr(sys, "pypy_version_info") and sys.platform.startswith("win"),
     reason="failing on Windows on PyPy (#63)",
 )
 
 
 class TestBasicGateway:
-    def test_correct_setup(self, gw):
+    def test_correct_setup(self, gw: Gateway) -> None:
         assert gw.hasreceiver()
         assert gw in gw._group
         assert gw.id in gw._group
         assert gw.spec
 
-    def test_repr_doesnt_crash(self, gw):
+    def test_repr_doesnt_crash(self, gw: Gateway) -> None:
         assert isinstance(repr(gw), str)
 
-    def test_attribute__name__(self, gw):
+    def test_attribute__name__(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.send(__name__)")
         name = channel.receive()
         assert name == "__channelexec__"
 
-    def test_gateway_status_simple(self, gw):
+    def test_gateway_status_simple(self, gw: Gateway) -> None:
         status = gw.remote_status()
         assert status.numexecuting == 0
 
-    def test_exc_info_is_clear_after_gateway_startup(self, gw):
+    def test_exc_info_is_clear_after_gateway_startup(self, gw: Gateway) -> None:
         ch = gw.remote_exec(
             """
                 import traceback, sys
                 excinfo = sys.exc_info()
                 if excinfo != (None, None, None):
                     r = traceback.format_exception(*excinfo)
                 else:
@@ -57,25 +62,25 @@
                 channel.send(r)
         """
         )
         res = ch.receive()
         if res != 0:
             pytest.fail("remote raised\n%s" % res)
 
-    def test_gateway_status_no_real_channel(self, gw):
+    def test_gateway_status_no_real_channel(self, gw: Gateway) -> None:
         numchan = gw._channelfactory.channels()
         gw.remote_status()
         numchan2 = gw._channelfactory.channels()
         # note that on CPython this can not really
         # fail because refcounting leads to immediate
         # closure of temporary channels
         assert numchan2 == numchan
 
     @flakytest
-    def test_gateway_status_busy(self, gw):
+    def test_gateway_status_busy(self, gw: Gateway) -> None:
         numchannels = gw.remote_status().numchannels
         ch1 = gw.remote_exec("channel.send(1); channel.receive()")
         ch2 = gw.remote_exec("channel.receive()")
         ch1.receive()
         status = gw.remote_status()
         assert status.numexecuting == 2  # number of active execution threads
         assert status.numchannels == numchannels + 2
@@ -88,28 +93,30 @@
             if status.numexecuting == 0:
                 break
         else:
             pytest.fail("did not get correct remote status")
         # race condition
         assert status.numchannels <= numchannels
 
-    def test_remote_exec_module(self, tmp_path, gw):
+    def test_remote_exec_module(self, tmp_path: pathlib.Path, gw: Gateway) -> None:
         p = tmp_path / "remotetest.py"
         p.write_text("channel.send(1)")
         mod = type(os)("remotetest")
         mod.__file__ = str(p)
         channel = gw.remote_exec(mod)
         name = channel.receive()
         assert name == 1
         p.write_text("channel.send(2)")
         channel = gw.remote_exec(mod)
         name = channel.receive()
         assert name == 2
 
-    def test_remote_exec_module_is_removed(self, gw, tmp_path, monkeypatch):
+    def test_remote_exec_module_is_removed(
+        self, gw: Gateway, tmp_path: pathlib.Path, monkeypatch: pytest.MonkeyPatch
+    ) -> None:
         remotetest = tmp_path / "remote.py"
         remotetest.write_text(
             dedent(
                 """
             def remote():
                 return True
 
@@ -118,44 +125,49 @@
                     channel.send(eval(item))  # noqa
 
             """
             )
         )
 
         monkeypatch.syspath_prepend(tmp_path)
-        import remote
+        import remote  # type: ignore[import-not-found]
 
         ch = gw.remote_exec(remote)
         # simulate sending the code to a remote location that does not have
         # access to the source
         shutil.rmtree(tmp_path)
         ch.send("remote()")
         try:
             result = ch.receive()
         finally:
             ch.close()
 
         assert result is True
 
-    def test_remote_exec_module_with_traceback(self, gw, tmp_path, monkeypatch):
+    def test_remote_exec_module_with_traceback(
+        self,
+        gw: Gateway,
+        tmp_path: pathlib.Path,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
         remotetestpy = tmp_path / "remotetest.py"
         remotetestpy.write_text(
             dedent(
                 """
             def run_me(channel=None):
                 raise ValueError('me')
 
             if __name__ == '__channelexec__':
                 run_me()
             """
             )
         )
 
         monkeypatch.syspath_prepend(tmp_path)
-        import remotetest
+        import remotetest  # type: ignore[import-not-found]
 
         ch = gw.remote_exec(remotetest)
         try:
             ch.receive()
         except execnet.gateway_base.RemoteError as e:
             assert 'remotetest.py", line 3, in run_me' in str(e)
             assert "ValueError: me" in str(e)
@@ -167,60 +179,61 @@
             ch.receive()
         except execnet.gateway_base.RemoteError as e:
             assert 'remotetest.py", line 3, in run_me' in str(e)
             assert "ValueError: me" in str(e)
         finally:
             ch.close()
 
-    def test_correct_setup_no_py(self, gw):
+    def test_correct_setup_no_py(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             import sys
             channel.send(list(sys.modules))
         """
         )
         remotemodules = channel.receive()
+        assert isinstance(remotemodules, list)
         assert "py" not in remotemodules, "py should not be imported on remote side"
 
-    def test_remote_exec_waitclose(self, gw):
+    def test_remote_exec_waitclose(self, gw: Gateway) -> None:
         channel = gw.remote_exec("pass")
         channel.waitclose(TESTTIMEOUT)
 
-    def test_remote_exec_waitclose_2(self, gw):
+    def test_remote_exec_waitclose_2(self, gw: Gateway) -> None:
         channel = gw.remote_exec("def gccycle(): pass")
         channel.waitclose(TESTTIMEOUT)
 
-    def test_remote_exec_waitclose_noarg(self, gw):
+    def test_remote_exec_waitclose_noarg(self, gw: Gateway) -> None:
         channel = gw.remote_exec("pass")
         channel.waitclose()
 
-    def test_remote_exec_error_after_close(self, gw):
+    def test_remote_exec_error_after_close(self, gw: Gateway) -> None:
         channel = gw.remote_exec("pass")
         channel.waitclose(TESTTIMEOUT)
         pytest.raises(IOError, channel.send, 0)
 
-    def test_remote_exec_no_explicit_close(self, gw):
+    def test_remote_exec_no_explicit_close(self, gw: Gateway) -> None:
         channel = gw.remote_exec("channel.close()")
         with pytest.raises(channel.RemoteError) as excinfo:
             channel.waitclose(TESTTIMEOUT)
         assert "explicit" in excinfo.value.formatted
 
-    def test_remote_exec_channel_anonymous(self, gw):
+    def test_remote_exec_channel_anonymous(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
            obj = channel.receive()
            channel.send(obj)
         """
         )
         channel.send(42)
         result = channel.receive()
         assert result == 42
 
     @needs_osdup
-    def test_confusion_from_os_write_stdout(self, gw):
+    def test_confusion_from_os_write_stdout(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             import os
             os.write(1, 'confusion!'.encode('ascii'))
             channel.send(channel.receive() * 6)
             channel.send(channel.receive() * 6)
         """
@@ -229,15 +242,15 @@
         res = channel.receive()
         assert res == 18
         channel.send(7)
         res = channel.receive()
         assert res == 42
 
     @needs_osdup
-    def test_confusion_from_os_write_stderr(self, gw):
+    def test_confusion_from_os_write_stderr(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             import os
             os.write(2, 'test'.encode('ascii'))
             channel.send(channel.receive() * 6)
             channel.send(channel.receive() * 6)
         """
@@ -245,15 +258,15 @@
         channel.send(3)
         res = channel.receive()
         assert res == 18
         channel.send(7)
         res = channel.receive()
         assert res == 42
 
-    def test__rinfo(self, gw):
+    def test__rinfo(self, gw: Gateway) -> None:
         rinfo = gw._rinfo()
         assert rinfo.executable
         assert rinfo.cwd
         assert rinfo.version_info
         assert repr(rinfo)
         old = gw.remote_exec(
             """
@@ -272,75 +285,81 @@
             gw._cache_rinfo = rinfo
             gw.remote_exec("import os ; os.chdir(%r)" % old).waitclose()
 
 
 class TestPopenGateway:
     gwtype = "popen"
 
-    def test_chdir_separation(self, tmp_path, makegateway):
+    def test_chdir_separation(
+        self, tmp_path: pathlib.Path, makegateway: Callable[[str], Gateway]
+    ) -> None:
         with pytest.MonkeyPatch.context() as mp:
             mp.chdir(tmp_path)
             gw = makegateway("popen")
         c = gw.remote_exec("import os ; channel.send(os.getcwd())")
         x = c.receive()
+        assert isinstance(x, str)
         assert x.lower() == str(tmp_path).lower()
 
-    def test_remoteerror_readable_traceback(self, gw):
+    def test_remoteerror_readable_traceback(self, gw: Gateway) -> None:
         with pytest.raises(gateway_base.RemoteError) as e:
             gw.remote_exec("x y").waitclose()
         assert "gateway_base" in e.value.formatted
 
-    def test_many_popen(self, makegateway):
+    def test_many_popen(self, makegateway: Callable[[str], Gateway]) -> None:
         num = 4
         l = []
         for i in range(num):
             l.append(makegateway("popen"))
         channels = []
         for gw in l:
             channel = gw.remote_exec("""channel.send(42)""")
             channels.append(channel)
         while channels:
             channel = channels.pop()
             ret = channel.receive()
             assert ret == 42
 
-    def test_rinfo_popen(self, gw):
+    def test_rinfo_popen(self, gw: Gateway) -> None:
         rinfo = gw._rinfo()
         assert rinfo.executable == sys.executable
         assert rinfo.cwd == os.getcwd()
         assert rinfo.version_info == sys.version_info
 
-    def test_waitclose_on_remote_killed(self, makegateway):
+    def test_waitclose_on_remote_killed(
+        self, makegateway: Callable[[str], Gateway]
+    ) -> None:
         gw = makegateway("popen")
         channel = gw.remote_exec(
             """
             import os
             import time
             channel.send(os.getpid())
             time.sleep(100)
         """
         )
         remotepid = channel.receive()
+        assert isinstance(remotepid, int)
         os.kill(remotepid, signal.SIGTERM)
         with pytest.raises(EOFError):
             channel.waitclose(TESTTIMEOUT)
         with pytest.raises(IOError):
             channel.send(None)
         with pytest.raises(EOFError):
             channel.receive()
 
-    def test_receive_on_remote_sysexit(self, gw):
+    def test_receive_on_remote_sysexit(self, gw: Gateway) -> None:
         channel = gw.remote_exec(
             """
             raise SystemExit()
         """
         )
         pytest.raises(channel.RemoteError, channel.receive)
 
-    def test_dont_write_bytecode(self, makegateway):
+    def test_dont_write_bytecode(self, makegateway: Callable[[str], Gateway]) -> None:
         check_sys_dont_write_bytecode = """
             import sys
             channel.send(sys.dont_write_bytecode)
         """
 
         gw = makegateway("popen")
         channel = gw.remote_exec(check_sys_dont_write_bytecode)
@@ -349,56 +368,61 @@
         gw = makegateway("popen//dont_write_bytecode")
         channel = gw.remote_exec(check_sys_dont_write_bytecode)
         ret = channel.receive()
         assert ret
 
 
 @pytest.mark.skipif("config.option.broken_isp")
-def test_socket_gw_host_not_found(gw, makegateway):
-    pytest.raises(execnet.HostNotFound, lambda: makegateway("socket=qwepoipqwe:9000"))
+def test_socket_gw_host_not_found(makegateway: Callable[[str], Gateway]) -> None:
+    with pytest.raises(execnet.HostNotFound):
+        makegateway("socket=qwepoipqwe:9000")
 
 
 class TestSshPopenGateway:
     gwtype = "ssh"
 
-    def test_sshconfig_config_parsing(self, monkeypatch, makegateway):
+    def test_sshconfig_config_parsing(
+        self, monkeypatch: pytest.MonkeyPatch, makegateway: Callable[[str], Gateway]
+    ) -> None:
         l = []
         monkeypatch.setattr(
             gateway_io, "Popen2IOMaster", lambda *args, **kwargs: l.append(args[0])
         )
-        pytest.raises(AttributeError, lambda: makegateway("ssh=xyz//ssh_config=qwe"))
+        with pytest.raises(AttributeError):
+            makegateway("ssh=xyz//ssh_config=qwe")
 
         assert len(l) == 1
         popen_args = l[0]
         i = popen_args.index("-F")
         assert popen_args[i + 1] == "qwe"
 
-    def test_sshaddress(self, gw, specssh):
+    def test_sshaddress(self, gw: Gateway, specssh: execnet.XSpec) -> None:
         assert gw.remoteaddress == specssh.ssh
 
-    def test_host_not_found(self, gw, makegateway):
-        pytest.raises(
-            execnet.HostNotFound, lambda: makegateway("ssh=nowhere.codespeak.net")
-        )
+    def test_host_not_found(
+        self, gw: Gateway, makegateway: Callable[[str], Gateway]
+    ) -> None:
+        with pytest.raises(execnet.HostNotFound):
+            makegateway("ssh=nowhere.codespeak.net")
 
 
 class TestThreads:
-    def test_threads(self, makegateway):
+    def test_threads(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("popen")
         gw.remote_init_threads(3)
         c1 = gw.remote_exec("channel.send(channel.receive())")
         c2 = gw.remote_exec("channel.send(channel.receive())")
         c2.send(1)
         res = c2.receive()
         assert res == 1
         c1.send(42)
         res = c1.receive()
         assert res == 42
 
-    def test_threads_race_sending(self, makegateway):
+    def test_threads_race_sending(self, makegateway: Callable[[str], Gateway]) -> None:
         # multiple threads sending data in parallel
         gw = makegateway("popen")
         num = 5
         gw.remote_init_threads(num)
         print("remote_init_threads(%d)" % num)
         channels = []
         for x in range(num):
@@ -414,15 +438,15 @@
             for x in range(10):
                 ch.receive(TESTTIMEOUT)
             ch.send(1)
         for ch in channels:
             ch.waitclose(TESTTIMEOUT)
 
     @flakytest
-    def test_status_with_threads(self, makegateway):
+    def test_status_with_threads(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("popen")
         c1 = gw.remote_exec("channel.send(1) ; channel.receive()")
         c2 = gw.remote_exec("channel.send(2) ; channel.receive()")
         c1.receive()
         c2.receive()
         rstatus = gw.remote_status()
         assert rstatus.numexecuting == 2
@@ -437,37 +461,48 @@
             rstatus = gw.remote_status()
             if rstatus.numexecuting == 0:
                 return
         assert 0, "numexecuting didn't drop to zero"
 
 
 class TestTracing:
-    def test_popen_filetracing(self, tmp_path, monkeypatch, makegateway):
+    def test_popen_filetracing(
+        self,
+        tmp_path: pathlib.Path,
+        monkeypatch: pytest.MonkeyPatch,
+        makegateway: Callable[[str], Gateway],
+    ) -> None:
         monkeypatch.setenv("TMP", str(tmp_path))
         monkeypatch.setenv("TEMP", str(tmp_path))  # windows
         monkeypatch.setenv("EXECNET_DEBUG", "1")
         gw = makegateway("popen")
         #  hack out the debuffilename
         fn = gw.remote_exec(
             "import execnet;channel.send(execnet.gateway_base.fn)"
         ).receive()
+        assert isinstance(fn, str)
         workerfile = pathlib.Path(fn)
         assert workerfile.exists()
         worker_line = "creating workergateway"
         with workerfile.open() as f:
             for line in f:
                 if worker_line in line:
                     break
             else:
                 pytest.fail(f"did not find {worker_line!r} in tracefile")
         gw.exit()
 
     @skip_win_pypy
     @flakytest
-    def test_popen_stderr_tracing(self, capfd, monkeypatch, makegateway):
+    def test_popen_stderr_tracing(
+        self,
+        capfd: pytest.CaptureFixture[str],
+        monkeypatch: pytest.MonkeyPatch,
+        makegateway: Callable[[str], Gateway],
+    ) -> None:
         monkeypatch.setenv("EXECNET_DEBUG", "2")
         gw = makegateway("popen")
         pid = gw.remote_exec("import os ; channel.send(os.getpid())").receive()
         out, err = capfd.readouterr()
         worker_line = "[%s] creating workergateway" % pid
         assert worker_line in err
         gw.exit()
@@ -489,16 +524,16 @@
             marks=pytest.mark.skipif(
                 sys.platform.startswith("win"), reason="invalid spec on Windows"
             ),
         ),
         ('popen//python="/u/test me/python" -e', ["/u/test me/python", "-e"]),
     ],
 )
-def test_popen_args(spec, expected_args):
-    expected_args = expected_args + ["-u", "-c", gateway_io.popen_bootstrapline]
+def test_popen_args(spec: str, expected_args: list[str]) -> None:
+    expected_args = [*expected_args, "-u", "-c", gateway_io.popen_bootstrapline]
     args = gateway_io.popen_args(execnet.XSpec(spec))
     assert args == expected_args
 
 
 @pytest.mark.parametrize(
     "interleave_getstatus",
     [
@@ -508,20 +543,105 @@
             id="no-interleave-remote-status",
             marks=pytest.mark.xfail(
                 reason="https://github.com/pytest-dev/execnet/issues/123",
             ),
         ),
     ],
 )
-def test_regression_gevent_hangs(group, interleave_getstatus):
+def test_regression_gevent_hangs(
+    group: execnet.Group, interleave_getstatus: bool
+) -> None:
     pytest.importorskip("gevent")
     gw = group.makegateway("popen//execmodel=gevent")
 
     print(gw.remote_status())
 
-    def sendback(channel):
+    def sendback(channel) -> None:
         channel.send(1234)
 
     ch = gw.remote_exec(sendback)
     if interleave_getstatus:
         print(gw.remote_status())
     assert ch.receive(timeout=0.5) == 1234
+
+
+def test_assert_main_thread_only(
+    execmodel: gateway_base.ExecModel, makegateway: Callable[[str], Gateway]
+) -> None:
+    if execmodel.backend != "main_thread_only":
+        pytest.skip("can only run with main_thread_only")
+
+    gw = makegateway(f"execmodel={execmodel.backend}//popen")
+
+    try:
+        # Submit multiple remote_exec requests in quick succession and
+        # assert that all tasks execute in the main thread. It is
+        # necessary to call receive on each channel before the next
+        # remote_exec call, since the channel will raise an error if
+        # concurrent remote_exec requests are submitted as in
+        # test_main_thread_only_concurrent_remote_exec_deadlock.
+        for i in range(10):
+            ch = gw.remote_exec(
+                """
+                    import time, threading
+                    time.sleep(0.02)
+                    channel.send(threading.current_thread() is threading.main_thread())
+            """
+            )
+
+            try:
+                res = ch.receive()
+            finally:
+                ch.close()
+                # This doesn't actually block because we closed
+                # the channel already, but it does check for remote
+                # errors and raise them.
+                ch.waitclose()
+            if res is not True:
+                pytest.fail("remote raised\n%s" % res)
+    finally:
+        gw.exit()
+        gw.join()
+
+
+def test_main_thread_only_concurrent_remote_exec_deadlock(
+    execmodel: gateway_base.ExecModel, makegateway: Callable[[str], Gateway]
+) -> None:
+    if execmodel.backend != "main_thread_only":
+        pytest.skip("can only run with main_thread_only")
+
+    gw = makegateway(f"execmodel={execmodel.backend}//popen")
+    channels = []
+    try:
+        # Submit multiple remote_exec requests in quick succession and
+        # assert that MAIN_THREAD_ONLY_DEADLOCK_TEXT is raised if
+        # concurrent remote_exec requests are submitted for the
+        # main_thread_only execmodel (as compensation for the lack of
+        # back pressure in remote_exec calls which do not attempt to
+        # block until the remote main thread is idle).
+        for i in range(2):
+            channels.append(
+                gw.remote_exec(
+                    """
+                    import threading
+                    channel.send(threading.current_thread() is threading.main_thread())
+                    # Wait forever, ensuring that the deadlock case triggers.
+                    channel.gateway.execmodel.Event().wait()
+            """
+                )
+            )
+
+        expected_results = (
+            True,
+            execnet.gateway_base.MAIN_THREAD_ONLY_DEADLOCK_TEXT,
+        )
+        for expected, ch in zip(expected_results, channels):
+            try:
+                res = ch.receive()
+            except execnet.RemoteError as e:
+                res = e.formatted
+            assert res == expected
+    finally:
+        for ch in channels:
+            ch.close()
+        gw.exit()
+        gw.join()
```

### Comparing `execnet-2.0.2/testing/test_rsync.py` & `execnet-2.1.0/testing/test_rsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import platform
 import sys
 import types
 
 import execnet
 import pytest
 from execnet import RSync
+from execnet.gateway import Gateway
 
 
 @pytest.fixture(scope="module")
-def group(request):
+def group(request: pytest.FixtureRequest) -> execnet.Group:
     group = execnet.Group()
     request.addfinalizer(group.terminate)
     return group
 
 
 @pytest.fixture(scope="module")
-def gw1(request, group):
+def gw1(request: pytest.FixtureRequest, group: execnet.Group) -> Gateway:
     gw = group.makegateway("popen//id=gw1")
     request.addfinalizer(gw.exit)
     return gw
 
 
 @pytest.fixture(scope="module")
-def gw2(request, group):
+def gw2(request: pytest.FixtureRequest, group: execnet.Group) -> Gateway:
     gw = group.makegateway("popen//id=gw2")
     request.addfinalizer(gw.exit)
     return gw
 
 
 needssymlink = pytest.mark.skipif(
     not hasattr(os, "symlink")
@@ -40,27 +41,27 @@
 class _dirs(types.SimpleNamespace):
     source: pathlib.Path
     dest1: pathlib.Path
     dest2: pathlib.Path
 
 
 @pytest.fixture
-def dirs(request, tmp_path) -> _dirs:
+def dirs(tmp_path: pathlib.Path) -> _dirs:
     dirs = _dirs(
         source=tmp_path / "source",
         dest1=tmp_path / "dest1",
         dest2=tmp_path / "dest2",
     )
     dirs.source.mkdir()
     dirs.dest1.mkdir()
     dirs.dest2.mkdir()
     return dirs
 
 
-def are_paths_equal(path1, path2):
+def are_paths_equal(path1: pathlib.Path, path2: pathlib.Path) -> bool:
     if os.path.__name__ == "ntpath":
         # On Windows, os.readlink returns an extended path (\\?\)
         # for absolute symlinks. However, extended does not compare
         # equal to non-extended, even when they refer to the same
         # path otherwise. So we have to fix it up ourselves...
         is_extended1 = str(path1).startswith("\\\\?\\")
         is_extended2 = str(path2).startswith("\\\\?\\")
@@ -68,21 +69,21 @@
             path2 = pathlib.Path("\\\\?\\" + str(path2))
         if not is_extended1 and is_extended2:
             path1 = pathlib.Path("\\\\?\\" + str(path1))
     return path1 == path2
 
 
 class TestRSync:
-    def test_notargets(self, dirs):
+    def test_notargets(self, dirs: _dirs) -> None:
         rsync = RSync(dirs.source)
         with pytest.raises(IOError):
             rsync.send()
-        assert rsync.send(raises=False) is None
+        assert rsync.send(raises=False) is None  # type: ignore[func-returns-value]
 
-    def test_dirsync(self, dirs, gw1, gw2):
+    def test_dirsync(self, dirs: _dirs, gw1: Gateway, gw2: Gateway) -> None:
         dest = dirs.dest1
         dest2 = dirs.dest2
         source = dirs.source
 
         for s in ("content1", "content2", "content2-a-bit-longer"):
             subdir = source / "subdir"
             subdir.mkdir(exist_ok=True)
@@ -111,55 +112,59 @@
         rsync = RSync(source)
         rsync.add_target(gw1, dest, delete=True)
         rsync.add_target(gw2, dest2)
         rsync.send()
         assert not dest.joinpath("subdir", "file1").exists()
         assert dest2.joinpath("subdir", "file1").exists()
 
-    def test_dirsync_twice(self, dirs, gw1, gw2):
+    def test_dirsync_twice(self, dirs: _dirs, gw1: Gateway, gw2: Gateway) -> None:
         source = dirs.source
         source.joinpath("hello").touch()
         rsync = RSync(source)
         rsync.add_target(gw1, dirs.dest1)
         rsync.send()
         assert dirs.dest1.joinpath("hello").exists()
         with pytest.raises(IOError):
             rsync.send()
-        assert rsync.send(raises=False) is None
+        assert rsync.send(raises=False) is None  # type: ignore[func-returns-value]
         rsync.add_target(gw1, dirs.dest2)
         rsync.send()
         assert dirs.dest2.joinpath("hello").exists()
         with pytest.raises(IOError):
             rsync.send()
-        assert rsync.send(raises=False) is None
+        assert rsync.send(raises=False) is None  # type: ignore[func-returns-value]
 
-    def test_rsync_default_reporting(self, capsys, dirs, gw1):
+    def test_rsync_default_reporting(
+        self, capsys: pytest.CaptureFixture[str], dirs: _dirs, gw1: Gateway
+    ) -> None:
         source = dirs.source
         source.joinpath("hello").touch()
         rsync = RSync(source)
         rsync.add_target(gw1, dirs.dest1)
         rsync.send()
         out, err = capsys.readouterr()
         assert out.find("hello") != -1
 
-    def test_rsync_non_verbose(self, capsys, dirs, gw1):
+    def test_rsync_non_verbose(
+        self, capsys: pytest.CaptureFixture[str], dirs: _dirs, gw1: Gateway
+    ) -> None:
         source = dirs.source
         source.joinpath("hello").touch()
         rsync = RSync(source, verbose=False)
         rsync.add_target(gw1, dirs.dest1)
         rsync.send()
         out, err = capsys.readouterr()
         assert not out
         assert not err
 
     @pytest.mark.skipif(
         sys.platform == "win32" or getattr(os, "_name", "") == "nt",
         reason="irrelevant on windows",
     )
-    def test_permissions(self, dirs, gw1, gw2):
+    def test_permissions(self, dirs: _dirs, gw1: Gateway, gw2: Gateway) -> None:
         source = dirs.source
         dest = dirs.dest1
         onedir = dirs.source / "one"
         onedir.mkdir()
         onedir.chmod(448)
         onefile = dirs.source / "file"
         onefile.touch()
@@ -190,15 +195,15 @@
         mode = destdir.stat().st_mode
         assert mode & 511 == 504
 
     @pytest.mark.skipif(
         sys.platform == "win32" or getattr(os, "_name", "") == "nt",
         reason="irrelevant on windows",
     )
-    def test_read_only_directories(self, dirs, gw1):
+    def test_read_only_directories(self, dirs: _dirs, gw1: Gateway) -> None:
         source = dirs.source
         dest = dirs.dest1
         sub = source / "sub"
         sub.mkdir()
         subsub = sub / "subsub"
         subsub.mkdir()
         sub.chmod(0o500)
@@ -210,15 +215,15 @@
         rsync.add_target(gw1, dest)
         rsync.send()
 
         assert dest.joinpath("sub").stat().st_mode & 0o700
         assert dest.joinpath("sub", "subsub").stat().st_mode & 0o700
 
     @needssymlink
-    def test_symlink_rsync(self, dirs, gw1):
+    def test_symlink_rsync(self, dirs: _dirs, gw1: Gateway) -> None:
         source = dirs.source
         dest = dirs.dest1
         subdir = dirs.source / "subdir"
         subdir.mkdir()
         sourcefile = subdir / "existent"
         sourcefile.touch()
         source.joinpath("rellink").symlink_to(sourcefile.relative_to(source))
@@ -232,15 +237,15 @@
         assert rellink == pathlib.Path("subdir/existent")
 
         abslink = pathlib.Path(os.readlink(str(dest / "abslink")))
         expected = dest.joinpath(sourcefile.relative_to(source))
         assert are_paths_equal(abslink, expected)
 
     @needssymlink
-    def test_symlink2_rsync(self, dirs, gw1):
+    def test_symlink2_rsync(self, dirs: _dirs, gw1: Gateway) -> None:
         source = dirs.source
         dest = dirs.dest1
         subdir = dirs.source / "subdir"
         subdir.mkdir()
         sourcefile = subdir / "somefile"
         sourcefile.touch()
         subdir.joinpath("link1").symlink_to(
@@ -257,15 +262,15 @@
         link1 = pathlib.Path(os.readlink(str(destsub / "link1")))
         assert are_paths_equal(link1, pathlib.Path("link2"))
         link2 = pathlib.Path(os.readlink(str(destsub / "link2")))
         assert are_paths_equal(link2, expected)
         link3 = pathlib.Path(os.readlink(str(destsub / "link3")))
         assert are_paths_equal(link3, source.parent)
 
-    def test_callback(self, dirs, gw1):
+    def test_callback(self, dirs: _dirs, gw1: Gateway) -> None:
         dest = dirs.dest1
         source = dirs.source
         source.joinpath("existent").write_text("a" * 100)
         source.joinpath("existant2").write_text("a" * 10)
         total = {}
 
         def callback(cmd, lgt, channel):
@@ -274,23 +279,23 @@
         rsync = RSync(source, callback=callback)
         # rsync = RSync()
         rsync.add_target(gw1, dest)
         rsync.send()
 
         assert total == {("list", 110): True, ("ack", 100): True, ("ack", 10): True}
 
-    def test_file_disappearing(self, dirs, gw1):
+    def test_file_disappearing(self, dirs: _dirs, gw1: Gateway) -> None:
         dest = dirs.dest1
         source = dirs.source
         source.joinpath("ex").write_text("a" * 100)
         source.joinpath("ex2").write_text("a" * 100)
 
         class DRsync(RSync):
-            def filter(self, x):
-                assert x != source
+            def filter(self, x: str) -> bool:
+                assert x != str(source)
                 if x.endswith("ex2"):
                     self.x = 1
                     source.joinpath("ex2").unlink()
                 return True
 
         rsync = DRsync(source)
         rsync.add_target(gw1, dest)
```

### Comparing `execnet-2.0.2/testing/test_serializer.py` & `execnet-2.1.0/testing/test_serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
+
 import os
 import subprocess
 import sys
 from pathlib import Path
 
 import execnet
 import pytest
 
-
 # We use the execnet folder in order to avoid triggering a missing apipkg.
 pyimportdir = os.fspath(Path(execnet.__file__).parent)
 
 
 class PythonWrapper:
-    def __init__(self, executable, tmp_path):
+    def __init__(self, executable: str, tmp_path: Path) -> None:
         self.executable = executable
         self.tmp_path = tmp_path
 
     def dump(self, obj_rep: str) -> bytes:
         script_file = self.tmp_path.joinpath("dump.py")
         script_file.write_text(
             f"""
@@ -28,15 +29,15 @@
 """
         )
         res = subprocess.run(
             [str(self.executable), str(script_file)], capture_output=True, check=True
         )
         return res.stdout
 
-    def load(self, data: bytes):
+    def load(self, data: bytes) -> list[str]:
         script_file = self.tmp_path.joinpath("load.py")
         script_file.write_text(
             rf"""
 import sys
 sys.path.insert(0, {pyimportdir!r})
 import gateway_base as serializer
 from io import BytesIO
@@ -47,36 +48,35 @@
 sys.stdout.write(type(obj).__name__ + "\n")
 sys.stdout.write(repr(obj))
 """
         )
         res = subprocess.run(
             [str(self.executable), str(script_file)],
             capture_output=True,
+            check=True,
         )
-        if res.returncode:
-            raise ValueError(res.stderr)
 
         return res.stdout.decode("ascii").splitlines()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<PythonWrapper for {self.executable}>"
 
 
 @pytest.fixture
-def py3(request, tmp_path):
+def py3(tmp_path: Path) -> PythonWrapper:
     return PythonWrapper(sys.executable, tmp_path)
 
 
 @pytest.fixture
-def dump(py3):
+def dump(py3: PythonWrapper):
     return py3.dump
 
 
 @pytest.fixture
-def load(py3):
+def load(py3: PythonWrapper):
     return py3.load
 
 
 simple_tests = [
     # expected before/after repr
     ("int", "4"),
     ("float", "3.25"),
@@ -84,22 +84,22 @@
     ("list", "[1, 2, 3]"),
     ("tuple", "(1, 2, 3)"),
     ("dict", "{(1, 2, 3): 32}"),
 ]
 
 
 @pytest.mark.parametrize(["tp_name", "repr"], simple_tests)
-def test_simple(tp_name, repr, dump, load):
+def test_simple(tp_name, repr, dump, load) -> None:
     p = dump(repr)
     tp, v = load(p)
     assert tp == tp_name
     assert v == repr
 
 
-def test_set(load, dump):
+def test_set(load, dump) -> None:
     p = dump("set((1, 2, 3))")
 
     tp, v = load(p)
     assert tp == "set"
     # assert v == "{1, 2, 3}" # ordering prevents this assertion
     assert v.startswith("{") and v.endswith("}")
     assert "1" in v and "2" in v and "3" in v
@@ -112,54 +112,54 @@
 def test_frozenset(load, dump):
     p = dump("frozenset((1, 2, 3))")
     tp, v = load(p)
     assert tp == "frozenset"
     assert v == "frozenset({1, 2, 3})"
 
 
-def test_long(load, dump):
+def test_long(load, dump) -> None:
     really_big = "9223372036854775807324234"
     p = dump(really_big)
     tp, v = load(p)
     assert tp == "int"
     assert v == really_big
 
 
-def test_bytes(dump, load):
+def test_bytes(dump, load) -> None:
     p = dump("b'hi'")
     tp, v = load(p)
     assert tp == "bytes"
     assert v == "b'hi'"
 
 
-def test_str(dump, load):
+def test_str(dump, load) -> None:
     p = dump("'xyz'")
     tp, s = load(p)
     assert tp == "str"
     assert s == "'xyz'"
 
 
-def test_unicode(load, dump):
+def test_unicode(load, dump) -> None:
     p = dump("u'hi'")
     tp, s = load(p)
     assert tp == "str"
     assert s == "'hi'"
 
 
-def test_bool(dump, load):
+def test_bool(dump, load) -> None:
     p = dump("True")
     tp, s = load(p)
     assert s == "True"
     assert tp == "bool"
 
 
-def test_none(dump, load):
+def test_none(dump, load) -> None:
     p = dump("None")
     tp, s = load(p)
     assert s == "None"
 
 
-def test_tuple_nested_with_empty_in_between(dump, load):
+def test_tuple_nested_with_empty_in_between(dump, load) -> None:
     p = dump("(1, (), 3)")
     tp, s = load(p)
     assert tp == "tuple"
     assert s == "(1, (), 3)"
```

### Comparing `execnet-2.0.2/testing/test_termination.py` & `execnet-2.1.0/testing/test_termination.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,130 @@
 import os
 import pathlib
 import shutil
 import signal
 import subprocess
 import sys
+from typing import Callable
 
 import execnet
 import pytest
+from execnet.gateway import Gateway
+from execnet.gateway_base import ExecModel
+from execnet.gateway_base import WorkerPool
 from test_gateway import TESTTIMEOUT
 
 execnetdir = pathlib.Path(execnet.__file__).parent.parent
 
 skip_win_pypy = pytest.mark.xfail(
     condition=hasattr(sys, "pypy_version_info") and sys.platform.startswith("win"),
     reason="failing on Windows on PyPy (#63)",
 )
 
 
-def test_exit_blocked_worker_execution_gateway(anypython, makegateway, pool):
+def test_exit_blocked_worker_execution_gateway(
+    anypython: str, makegateway: Callable[[str], Gateway], pool: WorkerPool
+) -> None:
     gateway = makegateway("popen//python=%s" % anypython)
     gateway.remote_exec(
         """
         import time
         time.sleep(10.0)
     """
     )
 
-    def doit():
+    def doit() -> int:
         gateway.exit()
         return 17
 
     reply = pool.spawn(doit)
     x = reply.get(timeout=5.0)
     assert x == 17
 
 
-def test_endmarker_delivery_on_remote_killterm(makegateway, execmodel):
-    if execmodel.backend != "thread":
+def test_endmarker_delivery_on_remote_killterm(
+    makegateway: Callable[[str], Gateway], execmodel: ExecModel
+) -> None:
+    if execmodel.backend not in ("thread", "main_thread_only"):
         pytest.xfail("test and execnet not compatible to greenlets yet")
     gw = makegateway("popen")
     q = execmodel.queue.Queue()
     channel = gw.remote_exec(
         source="""
         import os, time
         channel.send(os.getpid())
         time.sleep(100)
     """
     )
     pid = channel.receive()
+    assert isinstance(pid, int)
     os.kill(pid, signal.SIGTERM)
     channel.setcallback(q.put, endmarker=999)
     val = q.get(TESTTIMEOUT)
     assert val == 999
     err = channel._getremoteerror()
     assert isinstance(err, EOFError)
 
 
 @skip_win_pypy
-def test_termination_on_remote_channel_receive(monkeypatch, makegateway):
+def test_termination_on_remote_channel_receive(
+    monkeypatch: pytest.MonkeyPatch, makegateway: Callable[[str], Gateway]
+) -> None:
     if not shutil.which("ps"):
         pytest.skip("need 'ps' command to externally check process status")
     monkeypatch.setenv("EXECNET_DEBUG", "2")
     gw = makegateway("popen")
     pid = gw.remote_exec("import os ; channel.send(os.getpid())").receive()
     gw.remote_exec("channel.receive()")
     gw._group.terminate()
     command = ["ps", "-p", str(pid)]
-    output = subprocess.run(command, capture_output=True, text=True)
+    output = subprocess.run(command, capture_output=True, text=True, check=False)
     assert str(pid) not in output.stdout, output
 
 
-def test_close_initiating_remote_no_error(testdir, anypython):
-    p = testdir.makepyfile(
+def test_close_initiating_remote_no_error(
+    pytester: pytest.Pytester, anypython: str
+) -> None:
+    p = pytester.makepyfile(
         """
         import sys
         sys.path.insert(0, sys.argv[1])
         import execnet
         gw = execnet.makegateway("popen")
         print ("remote_exec1")
         ch1 = gw.remote_exec("channel.receive()")
         print ("remote_exec1")
         ch2 = gw.remote_exec("channel.receive()")
         print ("termination")
         execnet.default_group.terminate()
     """
     )
     popen = subprocess.Popen(
-        [str(anypython), str(p), str(execnetdir)], stdout=None, stderr=subprocess.PIPE
+        [anypython, str(p), str(execnetdir)], stdout=None, stderr=subprocess.PIPE
     )
     out, err = popen.communicate()
     print(err)
-    err = err.decode("utf8")
-    lines = [x for x in err.splitlines() if "*sys-package" not in x]
-    # print (lines)
+    errstr = err.decode("utf8")
+    lines = [x for x in errstr.splitlines() if "*sys-package" not in x]
     assert not lines
 
 
-def test_terminate_implicit_does_trykill(testdir, anypython, capfd, pool):
-    if pool.execmodel != "thread":
+def test_terminate_implicit_does_trykill(
+    pytester: pytest.Pytester,
+    anypython: str,
+    capfd: pytest.CaptureFixture[str],
+    pool: WorkerPool,
+) -> None:
+    if pool.execmodel.backend not in ("thread", "main_thread_only"):
         pytest.xfail("only os threading model supported")
-    p = testdir.makepyfile(
+    if sys.version_info >= (3, 12):
+        pytest.xfail(
+            "since python3.12 this test triggers RuntimeError: can't create new thread at interpreter shutdown"
+        )
+    p = pytester.makepyfile(
         """
         import sys
         sys.path.insert(0, %r)
         import execnet
         group = execnet.Group()
         gw = group.makegateway("popen")
         ch = gw.remote_exec("import time ; channel.send(1) ; time.sleep(100)")
@@ -121,13 +142,14 @@
 
         #  use process at-exit group.terminate call
     """
         % str(execnetdir)
     )
     popen = subprocess.Popen([str(anypython), str(p)], stdout=subprocess.PIPE)
     # sync with start-up
+    assert popen.stdout is not None
     popen.stdout.readline()
     reply = pool.spawn(popen.communicate)
     reply.get(timeout=50)
     out, err = capfd.readouterr()
     lines = [x for x in err.splitlines() if "*sys-package" not in x]
     assert not lines or "Killed" in err
```

### Comparing `execnet-2.0.2/testing/test_threadpool.py` & `execnet-2.1.0/testing/test_threadpool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,216 @@
 import os
-import sys
+from pathlib import Path
 
 import pytest
+from execnet.gateway_base import ExecModel
 from execnet.gateway_base import WorkerPool
 
 
-def test_execmodel(execmodel, tmp_path):
+def test_execmodel(execmodel: ExecModel, tmp_path: Path) -> None:
     assert execmodel.backend
     p = tmp_path / "somefile"
     p.write_text("content")
     fd = os.open(p, os.O_RDONLY)
     f = execmodel.fdopen(fd, "r")
     assert f.read() == "content"
     f.close()
 
 
-def test_execmodel_basic_attrs(execmodel):
+def test_execmodel_basic_attrs(execmodel: ExecModel) -> None:
     m = execmodel
     assert callable(m.start)
     assert m.get_ident()
 
 
-def test_simple(pool):
+def test_simple(pool: WorkerPool) -> None:
     reply = pool.spawn(lambda: 42)
     assert reply.get() == 42
 
 
-def test_some(pool, execmodel):
+def test_some(pool: WorkerPool, execmodel: ExecModel) -> None:
     q = execmodel.queue.Queue()
     num = 4
 
-    def f(i):
+    def f(i: int) -> None:
         q.put(i)
         while q.qsize():
             execmodel.sleep(0.01)
 
     for i in range(num):
         pool.spawn(f, i)
     for i in range(num):
         q.get()
     # assert len(pool._running) == 4
     assert pool.waitall(timeout=1.0)
     # execmodel.sleep(1)  helps on windows?
     assert len(pool._running) == 0
 
 
-def test_running_semnatics(pool, execmodel):
+def test_running_semnatics(pool: WorkerPool, execmodel: ExecModel) -> None:
     q = execmodel.queue.Queue()
 
-    def first():
+    def first() -> None:
         q.get()
 
     reply = pool.spawn(first)
     assert reply.running
     assert pool.active_count() == 1
     q.put(1)
     assert pool.waitall()
     assert pool.active_count() == 0
     assert not reply.running
 
 
-def test_waitfinish_on_reply(pool):
+def test_waitfinish_on_reply(pool: WorkerPool) -> None:
     l = []
     reply = pool.spawn(lambda: l.append(1))
     reply.waitfinish()
     assert l == [1]
     reply = pool.spawn(lambda: 0 / 0)
     reply.waitfinish()  # no exception raised
     pytest.raises(ZeroDivisionError, reply.get)
 
 
 @pytest.mark.xfail(reason="WorkerPool does not implement limited size")
-def test_limited_size(execmodel):
-    pool = WorkerPool(execmodel, size=1)
+def test_limited_size(execmodel: ExecModel) -> None:
+    pool = WorkerPool(execmodel, size=1)  # type: ignore[call-arg]
     q = execmodel.queue.Queue()
     q2 = execmodel.queue.Queue()
     q3 = execmodel.queue.Queue()
 
-    def first():
+    def first() -> None:
         q.put(1)
         q2.get()
 
     pool.spawn(first)
     assert q.get() == 1
 
-    def second():
+    def second() -> None:
         q3.put(3)
 
     # we spawn a second pool to spawn the second function
     # which should block
     pool2 = WorkerPool(execmodel)
     pool2.spawn(pool.spawn, second)
     assert not pool2.waitall(1.0)
     assert q3.qsize() == 0
     q2.put(2)
     assert pool2.waitall()
     assert pool.waitall()
 
 
-def test_get(pool):
-    def f():
+def test_get(pool: WorkerPool) -> None:
+    def f() -> int:
         return 42
 
     reply = pool.spawn(f)
     result = reply.get()
     assert result == 42
 
 
-def test_get_timeout(execmodel, pool):
-    def f():
+def test_get_timeout(execmodel: ExecModel, pool: WorkerPool) -> None:
+    def f() -> int:
         execmodel.sleep(0.2)
         return 42
 
     reply = pool.spawn(f)
     with pytest.raises(IOError):
         reply.get(timeout=0.01)
 
 
-def test_get_excinfo(pool):
-    def f():
+def test_get_excinfo(pool: WorkerPool) -> None:
+    def f() -> None:
         raise ValueError("42")
 
     reply = pool.spawn(f)
     with pytest.raises(ValueError):
         reply.get(1.0)
     with pytest.raises(ValueError):
         reply.get(1.0)
 
 
-def test_waitall_timeout(pool, execmodel):
+def test_waitall_timeout(pool: WorkerPool, execmodel: ExecModel) -> None:
     q = execmodel.queue.Queue()
 
-    def f():
+    def f() -> None:
         q.get()
 
     reply = pool.spawn(f)
     assert not pool.waitall(0.01)
     q.put(None)
     reply.get(timeout=1.0)
     assert pool.waitall(timeout=0.1)
 
 
 @pytest.mark.skipif(not hasattr(os, "dup"), reason="no os.dup")
-def test_pool_clean_shutdown(pool, capfd):
+def test_pool_clean_shutdown(
+    pool: WorkerPool, capfd: pytest.CaptureFixture[str]
+) -> None:
     q = pool.execmodel.queue.Queue()
 
-    def f():
+    def f() -> None:
         q.get()
 
     pool.spawn(f)
     assert not pool.waitall(timeout=1.0)
     pool.trigger_shutdown()
     with pytest.raises(ValueError):
         pool.spawn(f)
 
-    def wait_then_put():
+    def wait_then_put() -> None:
         pool.execmodel.sleep(0.1)
         q.put(1)
 
     pool.execmodel.start(wait_then_put)
     assert pool.waitall()
     out, err = capfd.readouterr()
     assert err == ""
 
 
-def test_primary_thread_integration(execmodel):
-    if execmodel.backend != "thread":
+def test_primary_thread_integration(execmodel: ExecModel) -> None:
+    if execmodel.backend not in ("thread", "main_thread_only"):
         with pytest.raises(ValueError):
             WorkerPool(execmodel=execmodel, hasprimary=True)
         return
     pool = WorkerPool(execmodel=execmodel, hasprimary=True)
     queue = execmodel.queue.Queue()
 
-    def do_integrate():
+    def do_integrate() -> None:
         queue.put(execmodel.get_ident())
         pool.integrate_as_primary_thread()
 
     execmodel.start(do_integrate)
 
-    def func():
+    def func() -> None:
         queue.put(execmodel.get_ident())
 
     pool.spawn(func)
     ident1 = queue.get()
     ident2 = queue.get()
     assert ident1 == ident2
     pool.terminate()
 
 
-def test_primary_thread_integration_shutdown(execmodel):
-    if execmodel.backend != "thread":
+def test_primary_thread_integration_shutdown(execmodel: ExecModel) -> None:
+    if execmodel.backend not in ("thread", "main_thread_only"):
         pytest.skip("can only run with threading")
     pool = WorkerPool(execmodel=execmodel, hasprimary=True)
     queue = execmodel.queue.Queue()
 
-    def do_integrate():
+    def do_integrate() -> None:
         queue.put(execmodel.get_ident())
         pool.integrate_as_primary_thread()
 
     execmodel.start(do_integrate)
     queue.get()
 
     queue2 = execmodel.queue.Queue()
 
-    def get_two():
+    def get_two() -> None:
         queue.put(execmodel.get_ident())
         queue2.get()
 
     reply = pool.spawn(get_two)
     # make sure get_two is running and blocked on queue2
     queue.get()
     # then shut down
```

### Comparing `execnet-2.0.2/testing/test_xspec.py` & `execnet-2.1.0/testing/test_xspec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from __future__ import annotations
 
 import os
 import shutil
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable
 
 import execnet
 import pytest
+from execnet import XSpec
+from execnet.gateway import Gateway
 from execnet.gateway_io import popen_args
 from execnet.gateway_io import ssh_args
 from execnet.gateway_io import vagrant_ssh_args
 
-XSpec = execnet.XSpec
-
-
 skip_win_pypy = pytest.mark.xfail(
     condition=hasattr(sys, "pypy_version_info") and sys.platform.startswith("win"),
     reason="failing on Windows on PyPy (#63)",
 )
 
 
 class TestXSpec:
-    def test_norm_attributes(self):
+    def test_norm_attributes(self) -> None:
         spec = XSpec(
             r"socket=192.168.102.2:8888//python=c:/this/python3.8//chdir=d:\hello"
         )
         assert spec.socket == "192.168.102.2:8888"
         assert spec.python == "c:/this/python3.8"
         assert spec.chdir == r"d:\hello"
         assert spec.nice is None
         assert not hasattr(spec, "_xyz")
 
         with pytest.raises(AttributeError):
-            spec._hello()
+            spec._hello()  # type: ignore[misc,operator]
 
         spec = XSpec("socket=192.168.102.2:8888//python=python2.5//nice=3")
         assert spec.socket == "192.168.102.2:8888"
         assert spec.python == "python2.5"
         assert spec.chdir is None
         assert spec.nice == "3"
 
@@ -44,205 +45,212 @@
         assert spec.ssh == "user@host"
         assert spec.python == "/usr/bin/python2.5"
         assert spec.chdir == "/hello/this"
 
         spec = XSpec("popen")
         assert spec.popen is True
 
-    def test_ssh_options(self):
+    def test_ssh_options(self) -> None:
         spec = XSpec("ssh=-p 22100 user@host//python=python3")
         assert spec.ssh == "-p 22100 user@host"
         assert spec.python == "python3"
 
         spec = XSpec(
             "ssh=-i ~/.ssh/id_rsa-passwordless_login -p 22100 user@host"
             "//python=python3"
         )
         assert spec.ssh == "-i ~/.ssh/id_rsa-passwordless_login -p 22100 user@host"
         assert spec.python == "python3"
 
-    def test_execmodel(self):
+    def test_execmodel(self) -> None:
         spec = XSpec("execmodel=thread")
         assert spec.execmodel == "thread"
         spec = XSpec("execmodel=eventlet")
         assert spec.execmodel == "eventlet"
 
-    def test_ssh_options_and_config(self):
+    def test_ssh_options_and_config(self) -> None:
         spec = XSpec("ssh=-p 22100 user@host//python=python3")
         spec.ssh_config = "/home/user/ssh_config"
         assert ssh_args(spec)[:6] == ["ssh", "-C", "-F", spec.ssh_config, "-p", "22100"]
 
-    def test_vagrant_options(self):
+    def test_vagrant_options(self) -> None:
         spec = XSpec("vagrant_ssh=default//python=python3")
         assert vagrant_ssh_args(spec)[:-1] == ["vagrant", "ssh", "default", "--", "-C"]
 
-    def test_popen_with_sudo_python(self):
+    def test_popen_with_sudo_python(self) -> None:
         spec = XSpec("popen//python=sudo python3")
         assert popen_args(spec) == [
             "sudo",
             "python3",
             "-u",
             "-c",
             "import sys;exec(eval(sys.stdin.readline()))",
         ]
 
-    def test_env(self):
+    def test_env(self) -> None:
         xspec = XSpec("popen//env:NAME=value1")
         assert xspec.env["NAME"] == "value1"
 
-    def test__samefilesystem(self):
+    def test__samefilesystem(self) -> None:
         assert XSpec("popen")._samefilesystem()
         assert XSpec("popen//python=123")._samefilesystem()
         assert not XSpec("popen//chdir=hello")._samefilesystem()
 
-    def test__spec_spec(self):
+    def test__spec_spec(self) -> None:
         for x in ("popen", "popen//python=this"):
             assert XSpec(x)._spec == x
 
-    def test_samekeyword_twice_raises(self):
+    def test_samekeyword_twice_raises(self) -> None:
         pytest.raises(ValueError, XSpec, "popen//popen")
         pytest.raises(ValueError, XSpec, "popen//popen=123")
 
-    def test_unknown_keys_allowed(self):
+    def test_unknown_keys_allowed(self) -> None:
         xspec = XSpec("hello=3")
         assert xspec.hello == "3"
 
-    def test_repr_and_string(self):
+    def test_repr_and_string(self) -> None:
         for x in ("popen", "popen//python=this"):
             assert repr(XSpec(x)).find("popen") != -1
             assert str(XSpec(x)) == x
 
-    def test_hash_equality(self):
+    def test_hash_equality(self) -> None:
         assert XSpec("popen") == XSpec("popen")
         assert hash(XSpec("popen")) == hash(XSpec("popen"))
         assert XSpec("popen//python=123") != XSpec("popen")
         assert hash(XSpec("socket=hello:8080")) != hash(XSpec("popen"))
 
 
 class TestMakegateway:
-    def test_no_type(self, makegateway):
+    def test_no_type(self, makegateway: Callable[[str], Gateway]) -> None:
         pytest.raises(ValueError, lambda: makegateway("hello"))
 
     @skip_win_pypy
-    def test_popen_default(self, makegateway):
+    def test_popen_default(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("")
         assert gw.spec.popen
         assert gw.spec.python is None
         rinfo = gw._rinfo()
         # assert rinfo.executable == sys.executable
         assert rinfo.cwd == os.getcwd()
         assert rinfo.version_info == sys.version_info
 
     @pytest.mark.skipif("not hasattr(os, 'nice')")
     @pytest.mark.xfail(reason="fails due to timing problems on busy single-core VMs")
-    def test_popen_nice(self, makegateway):
+    def test_popen_nice(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("popen")
 
-        def getnice(channel):
+        def getnice(channel) -> None:
             import os
 
             if hasattr(os, "nice"):
                 channel.send(os.nice(0))
             else:
                 channel.send(None)
 
         remotenice = gw.remote_exec(getnice).receive()
+        assert isinstance(remotenice, int)
         gw.exit()
         if remotenice is not None:
             gw = makegateway("popen//nice=5")
             remotenice2 = gw.remote_exec(getnice).receive()
             assert remotenice2 == remotenice + 5
 
-    def test_popen_env(self, makegateway):
+    def test_popen_env(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("popen//env:NAME123=123")
         ch = gw.remote_exec(
             """
             import os
             channel.send(os.environ['NAME123'])
         """
         )
         value = ch.receive()
         assert value == "123"
 
     @skip_win_pypy
-    def test_popen_explicit(self, makegateway):
+    def test_popen_explicit(self, makegateway: Callable[[str], Gateway]) -> None:
         gw = makegateway("popen//python=%s" % sys.executable)
         assert gw.spec.python == sys.executable
         rinfo = gw._rinfo()
         assert rinfo.executable == sys.executable
         assert rinfo.cwd == os.getcwd()
         assert rinfo.version_info == sys.version_info
 
     @skip_win_pypy
-    def test_popen_chdir_absolute(self, tmp_path, makegateway):
+    def test_popen_chdir_absolute(
+        self, tmp_path: Path, makegateway: Callable[[str], Gateway]
+    ) -> None:
         gw = makegateway("popen//chdir=%s" % tmp_path)
         rinfo = gw._rinfo()
         assert rinfo.cwd == str(tmp_path.resolve())
 
     @skip_win_pypy
-    def test_popen_chdir_newsub(self, monkeypatch, tmp_path, makegateway):
+    def test_popen_chdir_newsub(
+        self,
+        monkeypatch: pytest.MonkeyPatch,
+        tmp_path: Path,
+        makegateway: Callable[[str], Gateway],
+    ) -> None:
         monkeypatch.chdir(tmp_path)
         gw = makegateway("popen//chdir=hello")
         rinfo = gw._rinfo()
         expected = str(tmp_path.joinpath("hello").resolve()).lower()
         assert rinfo.cwd.lower() == expected
 
-    def test_ssh(self, specssh, makegateway):
+    def test_ssh(self, specssh: XSpec, makegateway: Callable[[str], Gateway]) -> None:
         sshhost = specssh.ssh
         gw = makegateway("ssh=%s//id=ssh1" % sshhost)
-        rinfo = gw._rinfo()
         assert gw.id == "ssh1"
-        gw2 = execnet.SshGateway(sshhost)
-        rinfo2 = gw2._rinfo()
-        assert rinfo.executable == rinfo2.executable
-        assert rinfo.cwd == rinfo2.cwd
-        assert rinfo.version_info == rinfo2.version_info
 
-    def test_vagrant(self, makegateway):
+    def test_vagrant(self, makegateway: Callable[[str], Gateway]) -> None:
         vagrant_bin = shutil.which("vagrant")
         if vagrant_bin is None:
             pytest.skip("Vagrant binary not in PATH")
         res = subprocess.run(
             [vagrant_bin, "status", "default", "--machine-readable"],
             capture_output=True,
             encoding="utf-8",
             errors="replace",
+            check=True,
         ).stdout
         print(res)
         if ",default,state,shutoff\n" in res:
             pytest.xfail("vm shutoff, run `vagrant up` first")
         if ",default,state,not_created\n" in res:
             pytest.xfail("vm not created, run `vagrant up` first")
         if ",default,state,running\n" not in res:
             pytest.fail("unknown vm state")
 
         gw = makegateway("vagrant_ssh=default//python=python3")
         rinfo = gw._rinfo()
-        rinfo.cwd == "/home/vagrant"
-        rinfo.executable == "/usr/bin/python"
+        assert rinfo.cwd == "/home/vagrant"
+        assert rinfo.executable == "/usr/bin/python"
 
-    def test_socket(self, specsocket, makegateway):
+    def test_socket(
+        self, specsocket: XSpec, makegateway: Callable[[str], Gateway]
+    ) -> None:
         gw = makegateway("socket=%s//id=sock1" % specsocket.socket)
         rinfo = gw._rinfo()
         assert rinfo.executable
         assert rinfo.cwd
         assert rinfo.version_info
         assert gw.id == "sock1"
         # we cannot instantiate a second gateway
 
     @pytest.mark.xfail(reason="we can't instantiate a second gateway")
-    def test_socket_second(self, specsocket, makegateway):
+    def test_socket_second(
+        self, specsocket: XSpec, makegateway: Callable[[str], Gateway]
+    ) -> None:
         gw = makegateway("socket=%s//id=sock1" % specsocket.socket)
         gw2 = makegateway("socket=%s//id=sock1" % specsocket.socket)
         rinfo = gw._rinfo()
         rinfo2 = gw2._rinfo()
         assert rinfo.executable == rinfo2.executable
         assert rinfo.cwd == rinfo2.cwd
         assert rinfo.version_info == rinfo2.version_info
 
-    def test_socket_installvia(self):
+    def test_socket_installvia(self) -> None:
         group = execnet.Group()
         group.makegateway("popen//id=p1")
         gw = group.makegateway("socket//installvia=p1//id=s1")
         assert gw.id == "s1"
         assert gw.remote_status()
         group.terminate()
```

### Comparing `execnet-2.0.2/LICENSE` & `execnet-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `execnet-2.0.2/README.rst` & `execnet-2.1.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 execnet: distributed Python deployment and communication
 ========================================================
 
-Important
----------
-
 .. image:: https://img.shields.io/pypi/v/execnet.svg
     :target: https://pypi.org/project/execnet/
 
 .. image:: https://anaconda.org/conda-forge/execnet/badges/version.svg
     :target: https://anaconda.org/conda-forge/execnet
 
 .. image:: https://img.shields.io/pypi/pyversions/execnet.svg
@@ -15,15 +12,15 @@
 
 .. image:: https://github.com/pytest-dev/execnet/workflows/test/badge.svg
     :target: https://github.com/pytest-dev/execnet/actions?query=workflow%3Atest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/python/black
 
-.. _execnet: http://codespeak.net/execnet
+.. _execnet: https://execnet.readthedocs.io
 
 execnet_ provides carefully tested means to ad-hoc interact with Python
 interpreters across version, platform and network barriers.  It provides
 a minimal and fast API targeting the following uses:
 
 * distribute tasks to local or remote processes
 * write and deploy hybrid multi-process applications
```

### Comparing `execnet-2.0.2/PKG-INFO` & `execnet-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: execnet
-Version: 2.0.2
+Version: 2.1.0
 Summary: execnet: rapid multi-Python deployment
 Project-URL: Homepage, https://execnet.readthedocs.io/en/latest/
 Author: holger krekel and others
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Requires-Dist: hatch; extra == 'testing'
 Requires-Dist: pre-commit; extra == 'testing'
 Requires-Dist: pytest; extra == 'testing'
 Requires-Dist: tox; extra == 'testing'
 Description-Content-Type: text/x-rst
 
 execnet: distributed Python deployment and communication
 ========================================================
 
-Important
----------
-
 .. image:: https://img.shields.io/pypi/v/execnet.svg
     :target: https://pypi.org/project/execnet/
 
 .. image:: https://anaconda.org/conda-forge/execnet/badges/version.svg
     :target: https://anaconda.org/conda-forge/execnet
 
 .. image:: https://img.shields.io/pypi/pyversions/execnet.svg
@@ -47,15 +44,15 @@
 
 .. image:: https://github.com/pytest-dev/execnet/workflows/test/badge.svg
     :target: https://github.com/pytest-dev/execnet/actions?query=workflow%3Atest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/python/black
 
-.. _execnet: http://codespeak.net/execnet
+.. _execnet: https://execnet.readthedocs.io
 
 execnet_ provides carefully tested means to ad-hoc interact with Python
 interpreters across version, platform and network barriers.  It provides
 a minimal and fast API targeting the following uses:
 
 * distribute tasks to local or remote processes
 * write and deploy hybrid multi-process applications
```

