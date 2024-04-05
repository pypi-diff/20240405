# Comparing `tmp/pytest_sentry-0.2.0.tar.gz` & `tmp/pytest_sentry-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_sentry-0.2.0.tar", last modified: Thu Apr  4 14:30:11 2024, max compression
+gzip compressed data, was "pytest_sentry-0.2.1.tar", last modified: Thu Apr  4 17:00:00 2024, max compression
```

## Comparing `pytest_sentry-0.2.0.tar` & `pytest_sentry-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.668431 pytest_sentry-0.2.0/pytest_sentry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 14:30:11.000000 pytest_sentry-0.2.0/pytest_sentry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/pytest_sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 14:30:11.672431 pytest_sentry-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:30:11.668431 pytest_sentry-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_envvars.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 14:30:07.000000 pytest_sentry-0.2.0/tests/test_tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:00:00.899453 pytest_sentry-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-04 17:00:00.899453 pytest_sentry-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:00:00.899453 pytest_sentry-0.2.1/pytest_sentry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 17:00:00.000000 pytest_sentry-0.2.1/pytest_sentry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/pytest_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-04 17:00:00.899453 pytest_sentry-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:00:00.899453 pytest_sentry-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 16:59:57.000000 pytest_sentry-0.2.1/tests/test_tracing.py
```

### Comparing `pytest_sentry-0.2.0/LICENSE` & `pytest_sentry-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.2.0/PKG-INFO` & `pytest_sentry-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pytest_sentry
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pytest plugin to send testrun information to Sentry.io
 Home-page: https://github.com/untitaker/pytest-sentry
 Author: Markus Unterwaditzer
 Author-email: markus@unterwaditzer.net
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest
-Requires-Dist: sentry-sdk==2.0.0rc4
+Requires-Dist: sentry-sdk
 Requires-Dist: wrapt
 
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
@@ -95,22 +95,22 @@
 
     pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
 
 Advanced Options
 ================
 
 ``pytest-sentry`` supports marking your tests to use a different DSN, client or
-scope per-test. You can use this to provide custom options to the ``Client``
+hub per-test. You can use this to provide custom options to the ``Client``
 object from the `Sentry SDK for Python
 <https://github.com/getsentry/sentry-python>`_::
 
     import random
     import pytest
 
-    from sentry_sdk import Scope
+    from sentry_sdk import Hub
     from pytest_sentry import Client
 
     @pytest.mark.sentry_client(None)
     def test_no_sentry():
         # Even though flaky, this test never gets reported to sentry
         assert random.random() > 0.5
 
@@ -119,15 +119,15 @@
         # Use a different DSN to report errors for this one
         assert random.random() > 0.5
 
     # Other invocations:
 
     @pytest.mark.sentry_client(Client("CUSTOM DSN"))
     @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
-    @pytest.mark.sentry_client(Scope(Client("CUSTOM DSN")))
+    @pytest.mark.sentry_client(Hub(Client("CUSTOM DSN")))
     @pytest.mark.sentry_client({"dsn": ..., "debug": True})
 
 
 The ``Client`` class exposed by ``pytest-sentry`` only has different default
 integrations. It disables some of the error-capturing integrations to avoid
 sending random expected errors into your project.
 
@@ -136,20 +136,20 @@
 
 You will notice that the global functions such as
 ``sentry_sdk.capture_message`` will not actually send events into the same DSN
 you configured this plugin with. That's because ``pytest-sentry`` goes to
 extreme lenghts to keep its own SDK setup separate from the SDK setup of the
 tested code.
 
-``pytest-sentry`` exposes the ``sentry_test_scope`` fixture whose return value is
-the ``Scope`` being used to send events to Sentry. Use ``with use_scope(entry_test_scope):``
+``pytest-sentry`` exposes the ``sentry_test_hub`` fixture whose return value is
+the ``Hub`` being used to send events to Sentry. Use ``with sentry_test_hub:``
 to temporarily switch context. You can use this to set custom tags like so::
 
-    def test_foo(sentry_test_scope):
-        with use_scope(sentry_test_scope):
+    def test_foo(sentry_test_hub):
+        with sentry_test_hub:
             sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
 
 
 Why all the hassle with the context manager? Just imagine if your tested
 application would start to log some (expected) errors on its own. You would
 immediately exceed your quota!
```

### Comparing `pytest_sentry-0.2.0/README.rst` & `pytest_sentry-0.2.1/pytest_sentry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pytest_sentry
+Version: 0.2.1
+Summary: A pytest plugin to send testrun information to Sentry.io
+Home-page: https://github.com/untitaker/pytest-sentry
+Author: Markus Unterwaditzer
+Author-email: markus@unterwaditzer.net
+License: BSD-2-Clause
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pytest
+Requires-Dist: sentry-sdk
+Requires-Dist: wrapt
+
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
     :target: https://pypi.org/project/pytest-sentry/
 
@@ -80,22 +95,22 @@
 
     pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
 
 Advanced Options
 ================
 
 ``pytest-sentry`` supports marking your tests to use a different DSN, client or
-scope per-test. You can use this to provide custom options to the ``Client``
+hub per-test. You can use this to provide custom options to the ``Client``
 object from the `Sentry SDK for Python
 <https://github.com/getsentry/sentry-python>`_::
 
     import random
     import pytest
 
-    from sentry_sdk import Scope
+    from sentry_sdk import Hub
     from pytest_sentry import Client
 
     @pytest.mark.sentry_client(None)
     def test_no_sentry():
         # Even though flaky, this test never gets reported to sentry
         assert random.random() > 0.5
 
@@ -104,15 +119,15 @@
         # Use a different DSN to report errors for this one
         assert random.random() > 0.5
 
     # Other invocations:
 
     @pytest.mark.sentry_client(Client("CUSTOM DSN"))
     @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
-    @pytest.mark.sentry_client(Scope(Client("CUSTOM DSN")))
+    @pytest.mark.sentry_client(Hub(Client("CUSTOM DSN")))
     @pytest.mark.sentry_client({"dsn": ..., "debug": True})
 
 
 The ``Client`` class exposed by ``pytest-sentry`` only has different default
 integrations. It disables some of the error-capturing integrations to avoid
 sending random expected errors into your project.
 
@@ -121,20 +136,20 @@
 
 You will notice that the global functions such as
 ``sentry_sdk.capture_message`` will not actually send events into the same DSN
 you configured this plugin with. That's because ``pytest-sentry`` goes to
 extreme lenghts to keep its own SDK setup separate from the SDK setup of the
 tested code.
 
-``pytest-sentry`` exposes the ``sentry_test_scope`` fixture whose return value is
-the ``Scope`` being used to send events to Sentry. Use ``with use_scope(entry_test_scope):``
+``pytest-sentry`` exposes the ``sentry_test_hub`` fixture whose return value is
+the ``Hub`` being used to send events to Sentry. Use ``with sentry_test_hub:``
 to temporarily switch context. You can use this to set custom tags like so::
 
-    def test_foo(sentry_test_scope):
-        with use_scope(sentry_test_scope):
+    def test_foo(sentry_test_hub):
+        with sentry_test_hub:
             sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
 
 
 Why all the hassle with the context manager? Just imagine if your tested
 application would start to log some (expected) errors on its own. You would
 immediately exceed your quota!
```

### Comparing `pytest_sentry-0.2.0/pytest_sentry.egg-info/PKG-INFO` & `pytest_sentry-0.2.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest_sentry
-Version: 0.2.0
-Summary: A pytest plugin to send testrun information to Sentry.io
-Home-page: https://github.com/untitaker/pytest-sentry
-Author: Markus Unterwaditzer
-Author-email: markus@unterwaditzer.net
-License: BSD-2-Clause
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: pytest
-Requires-Dist: sentry-sdk==2.0.0rc4
-Requires-Dist: wrapt
-
 =============
 pytest-sentry
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-sentry
     :target: https://pypi.org/project/pytest-sentry/
 
@@ -95,22 +80,22 @@
 
     pytestmarker = pytest.mark.sentry_client({"traces_sample_rate": 0.0})
 
 Advanced Options
 ================
 
 ``pytest-sentry`` supports marking your tests to use a different DSN, client or
-scope per-test. You can use this to provide custom options to the ``Client``
+hub per-test. You can use this to provide custom options to the ``Client``
 object from the `Sentry SDK for Python
 <https://github.com/getsentry/sentry-python>`_::
 
     import random
     import pytest
 
-    from sentry_sdk import Scope
+    from sentry_sdk import Hub
     from pytest_sentry import Client
 
     @pytest.mark.sentry_client(None)
     def test_no_sentry():
         # Even though flaky, this test never gets reported to sentry
         assert random.random() > 0.5
 
@@ -119,15 +104,15 @@
         # Use a different DSN to report errors for this one
         assert random.random() > 0.5
 
     # Other invocations:
 
     @pytest.mark.sentry_client(Client("CUSTOM DSN"))
     @pytest.mark.sentry_client(lambda: Client("CUSTOM DSN"))
-    @pytest.mark.sentry_client(Scope(Client("CUSTOM DSN")))
+    @pytest.mark.sentry_client(Hub(Client("CUSTOM DSN")))
     @pytest.mark.sentry_client({"dsn": ..., "debug": True})
 
 
 The ``Client`` class exposed by ``pytest-sentry`` only has different default
 integrations. It disables some of the error-capturing integrations to avoid
 sending random expected errors into your project.
 
@@ -136,20 +121,20 @@
 
 You will notice that the global functions such as
 ``sentry_sdk.capture_message`` will not actually send events into the same DSN
 you configured this plugin with. That's because ``pytest-sentry`` goes to
 extreme lenghts to keep its own SDK setup separate from the SDK setup of the
 tested code.
 
-``pytest-sentry`` exposes the ``sentry_test_scope`` fixture whose return value is
-the ``Scope`` being used to send events to Sentry. Use ``with use_scope(entry_test_scope):``
+``pytest-sentry`` exposes the ``sentry_test_hub`` fixture whose return value is
+the ``Hub`` being used to send events to Sentry. Use ``with sentry_test_hub:``
 to temporarily switch context. You can use this to set custom tags like so::
 
-    def test_foo(sentry_test_scope):
-        with use_scope(sentry_test_scope):
+    def test_foo(sentry_test_hub):
+        with sentry_test_hub:
             sentry_sdk.set_tag("pull_request", os.environ['EXAMPLE_CI_PULL_REQUEST'])
 
 
 Why all the hassle with the context manager? Just imagine if your tested
 application would start to log some (expected) errors on its own. You would
 immediately exceed your quota!
```

### Comparing `pytest_sentry-0.2.0/pytest_sentry.py` & `pytest_sentry-0.2.1/pytest_sentry.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import pytest
 
 import wrapt
 import sentry_sdk
 from sentry_sdk.integrations import Integration
 
-from sentry_sdk import Scope, capture_exception
+from sentry_sdk import Hub, capture_exception
 from sentry_sdk.tracing import Transaction
-from sentry_sdk.scope import add_global_event_processor, use_scope
+from sentry_sdk.scope import add_global_event_processor
 
 _ENVVARS_AS_TAGS = frozenset(
     [
         "GITHUB_WORKFLOW",  # The name of the workflow.
         "GITHUB_RUN_ID",  # A unique number for each run within a repository. This number does not change if you re-run the workflow run.
         "GITHUB_RUN_NUMBER",  # A unique number for each run of a particular workflow in a repository. This number begins at 1 for the workflow's first run, and increments with each new run. This number does not change if you re-run the workflow run.
         "GITHUB_ACTION",  # The unique identifier (id) of the action.
@@ -55,15 +55,15 @@
 
         self.always_report = always_report
 
     @staticmethod
     def setup_once():
         @add_global_event_processor
         def procesor(event, hint):
-            if Scope.get_client().get_integration(PytestIntegration) is None:
+            if Hub.current.get_integration(PytestIntegration) is None:
                 return event
 
             for key in _ENVVARS_AS_TAGS:
                 value = os.environ.get(key)
                 if not value:
                     continue
                 event.setdefault("tags", {})["pytest_environ.{}".format(key)] = value
@@ -78,90 +78,87 @@
 
             return event
 
 
 class Client(sentry_sdk.Client):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("dsn", os.environ.get("PYTEST_SENTRY_DSN", None))
-        kwargs.setdefault(
-            "traces_sample_rate",
-            float(os.environ.get("PYTEST_SENTRY_TRACES_SAMPLE_RATE", 1.0)),
-        )
+        kwargs.setdefault("traces_sample_rate", float(os.environ.get("PYTEST_SENTRY_TRACES_SAMPLE_RATE", 1.0)))
         kwargs.setdefault("_experiments", {}).setdefault(
             "auto_enabling_integrations", True
         )
         kwargs.setdefault("environment", os.environ.get("SENTRY_ENVIRONMENT", "test"))
         kwargs.setdefault("integrations", []).append(PytestIntegration())
 
         sentry_sdk.Client.__init__(self, *args, **kwargs)
 
 
 def hookwrapper(itemgetter, **kwargs):
     """
-    A version of pytest.hookimpl that sets the current scope to the correct one
+    A version of pytest.hookimpl that sets the current hub to the correct one
     and skips the hook if the integration is disabled.
 
     Assumes the function is a hookwrapper, ie yields once
     """
 
     @wrapt.decorator
-    def _with_scope(wrapped, instance, args, kwargs):
+    def _with_hub(wrapped, instance, args, kwargs):
         item = itemgetter(*args, **kwargs)
-        scope = _resolve_scope_marker_value(item.get_closest_marker("sentry_client"))
+        hub = _resolve_hub_marker_value(item.get_closest_marker("sentry_client"))
 
-        if scope.client.get_integration(PytestIntegration) is None:
+        if hub.get_integration(PytestIntegration) is None:
             yield
         else:
-            with use_scope(scope):
+            with hub:
                 gen = wrapped(*args, **kwargs)
 
             while True:
                 try:
-                    with use_scope(scope):
+                    with hub:
                         chunk = next(gen)
 
                     y = yield chunk
 
-                    with use_scope(scope):
+                    with hub:
                         gen.send(y)
 
                 except StopIteration:
                     break
 
     def inner(f):
-        return pytest.hookimpl(hookwrapper=True, **kwargs)(_with_scope(f))
+        return pytest.hookimpl(hookwrapper=True, **kwargs)(_with_hub(f))
 
     return inner
 
 
 def pytest_load_initial_conftests(early_config, parser, args):
     early_config.addinivalue_line(
         "markers",
-        "sentry_client(client=None): Use this client instance for reporting tests. You can also pass a DSN string directly, or a `Scope` if you need it.",
+        "sentry_client(client=None): Use this client instance for reporting tests. You can also pass a DSN string directly, or a `Hub` if you need it.",
     )
 
 
 def _start_transaction(**kwargs):
     transaction = Transaction.continue_from_headers(
-        dict(Scope.get_current_scope().iter_trace_propagation_headers()), **kwargs
+        dict(Hub.current.iter_trace_propagation_headers()), **kwargs
     )
     transaction.same_process_as_parent = True
     return sentry_sdk.start_transaction(transaction)
 
 
 @hookwrapper(itemgetter=lambda item: item)
 def pytest_runtest_protocol(item):
     op = "pytest.runtest.protocol"
 
     name = item.nodeid
 
     # We use the full name including parameters because then we can identify
     # how often a single test has run as part of the same GITHUB_RUN_ID.
 
-    with _start_transaction(op=op, name="{} {}".format(op, name)) as tx:
+    with _start_transaction(op=op, name=u"{} {}".format(op, name)) as tx:
         yield
 
         # Purposefully drop transaction to spare quota. We only created it to
         # have a trace_id to correlate by.
         tx.sampled = False
 
 
@@ -170,24 +167,22 @@
     op = "pytest.runtest.call"
 
     name = item.nodeid
 
     # We use the full name including parameters because then we can identify
     # how often a single test has run as part of the same GITHUB_RUN_ID.
 
-    with _start_transaction(op=op, name="{} {}".format(op, name)):
+    with _start_transaction(op=op, name=u"{} {}".format(op, name)):
         yield
 
 
 @hookwrapper(itemgetter=lambda fixturedef, request: request._pyfuncitem)
 def pytest_fixture_setup(fixturedef, request):
     op = "pytest.fixture.setup"
-    with _start_transaction(
-        op=op, name="{} {}".format(op, fixturedef.argname)
-    ) as transaction:
+    with _start_transaction(op=op, name=u"{} {}".format(op, fixturedef.argname)) as transaction:
         transaction.set_tag("pytest.fixture.scope", fixturedef.scope)
         yield
 
 
 @hookwrapper(tryfirst=True, itemgetter=lambda item, call: item)
 def pytest_runtest_makereport(item, call):
     sentry_sdk.set_tag("pytest.result", "pending")
@@ -199,76 +194,76 @@
         cur_exc_chain = getattr(item, "pytest_sentry_exc_chain", [])
 
         if call.excinfo is not None:
             item.pytest_sentry_exc_chain = cur_exc_chain = cur_exc_chain + [
                 call.excinfo
             ]
 
-        integration = Scope.get_client().get_integration(PytestIntegration)
+        integration = Hub.current.get_integration(PytestIntegration)
 
         if (cur_exc_chain and call.excinfo is None) or integration.always_report:
             for exc_info in cur_exc_chain:
                 capture_exception((exc_info.type, exc_info.value, exc_info.tb))
 
 
-DEFAULT_SCOPE = Scope(client=Client())
+DEFAULT_HUB = Hub(Client())
 
-_scope_cache = {}
+_hub_cache = {}
 
 
-def _resolve_scope_marker_value(marker_value):
-    if id(marker_value) not in _scope_cache:
-        _scope_cache[id(marker_value)] = rv = _resolve_scope_marker_value_uncached(
+def _resolve_hub_marker_value(marker_value):
+    if id(marker_value) not in _hub_cache:
+        _hub_cache[id(marker_value)] = rv = _resolve_hub_marker_value_uncached(
             marker_value
         )
         return rv
 
-    return _scope_cache[id(marker_value)]
+    return _hub_cache[id(marker_value)]
 
 
-def _resolve_scope_marker_value_uncached(marker_value):
+def _resolve_hub_marker_value_uncached(marker_value):
     if marker_value is None:
-        marker_value = DEFAULT_SCOPE
+        marker_value = DEFAULT_HUB
     else:
         marker_value = marker_value.args[0]
 
     if callable(marker_value):
         marker_value = marker_value()
 
     if marker_value is None:
         # user explicitly disabled reporting
-        return Scope()
+        return Hub()
 
     if isinstance(marker_value, str):
-        return Scope(client=Client(marker_value))
+        return Hub(Client(marker_value))
 
     if isinstance(marker_value, dict):
-        return Scope(client=Client(**marker_value))
+        return Hub(Client(**marker_value))
 
     if isinstance(marker_value, Client):
-        return Scope(client=marker_value)
+        return Hub(marker_value)
 
-    if isinstance(marker_value, Scope):
+    if isinstance(marker_value, Hub):
         return marker_value
 
     raise RuntimeError(
-        "The `sentry_client` value must be a client, scope or string, not {}".format(
+        "The `sentry_client` value must be a client, hub or string, not {}".format(
             repr(type(marker_value))
         )
     )
 
 
 @pytest.fixture
-def sentry_test_scope(request):
+def sentry_test_hub(request):
     """
-    Gives back the current scope.
+    Gives back the current hub.
     """
 
     item = request.node
-    return _resolve_scope_marker_value(item.get_closest_marker("sentry_client"))
+    return _resolve_hub_marker_value(item.get_closest_marker("sentry_client"))
 
 
 def _process_stacktrace(stacktrace):
     for frame in stacktrace["frames"]:
         frame["in_app"] = not frame["module"].startswith(
             ("_pytest.", "pytest.", "pluggy.")
         )
```

### Comparing `pytest_sentry-0.2.0/setup.cfg` & `pytest_sentry-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest_sentry
-version = 0.2.0
+version = 0.2.1
 description = A pytest plugin to send testrun information to Sentry.io
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/untitaker/pytest-sentry
 author = Markus Unterwaditzer
 author_email = markus@unterwaditzer.net
 license = BSD-2-Clause
@@ -12,15 +12,15 @@
 classifiers = 
 	License :: OSI Approved :: BSD License
 
 [options]
 py_modules = pytest_sentry
 install_requires = 
 	pytest
-	sentry-sdk==2.0.0rc4
+	sentry-sdk
 	wrapt
 
 [options.entry_points]
 pytest11 = 
 	sentry = pytest_sentry
 
 [egg_info]
```

### Comparing `pytest_sentry-0.2.0/tests/test_envvars.py` & `pytest_sentry-0.2.1/tests/test_envvars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 import sentry_sdk
-from sentry_sdk.scope import use_scope
 import pytest_sentry
 
 events = []
 envelopes = []
 
 
 class MyTransport(sentry_sdk.Transport):
@@ -23,17 +22,17 @@
     events.clear()
     envelopes.clear()
 
 
 pytestmark = pytest.mark.sentry_client(pytest_sentry.Client(transport=MyTransport()))
 
 
-def test_basic(sentry_test_scope):
-    with use_scope(sentry_test_scope):
-        sentry_test_scope.capture_message("hi")
+def test_basic(sentry_test_hub):
+    with sentry_test_hub:
+        sentry_test_hub.capture_message("hi")
 
     (event,) = events
     assert event["tags"]["pytest_environ.GITHUB_RUN_ID"] == "123abc"
 
 
 def test_transaction(request):
     @request.addfinalizer
```

### Comparing `pytest_sentry-0.2.0/tests/test_retries.py` & `pytest_sentry-0.2.1/tests/test_retries.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.2.0/tests/test_skip.py` & `pytest_sentry-0.2.1/tests/test_skip.py`

 * *Files identical despite different names*

### Comparing `pytest_sentry-0.2.0/tests/test_tracing.py` & `pytest_sentry-0.2.1/tests/test_tracing.py`

 * *Files identical despite different names*

