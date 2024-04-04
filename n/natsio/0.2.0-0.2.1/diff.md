# Comparing `tmp/natsio-0.2.0.tar.gz` & `tmp/natsio-0.2.1.tar.gz`

## Comparing `natsio-0.2.0.tar` & `natsio-0.2.1.tar`

### file list

```diff
@@ -1,59 +1,61 @@
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 natsio-0.2.0/TODO.md
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 natsio-0.2.0/main.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 natsio-0.2.0/pyrightconfig.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 natsio-0.2.0/certs/client-cert.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 natsio-0.2.0/certs/client-key.pem
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 natsio-0.2.0/certs/rootCA.pem
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 natsio-0.2.0/certs/server-cert.pem
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 natsio-0.2.0/certs/server-key.pem
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/const.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/abc/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/abc/client.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/abc/connection.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/abc/dispatcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/abc/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/client/__init__.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/client/config.py
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/client/core.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/client/status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/connection/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/connection/protocol.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/connection/status.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/connection/stream.py
--rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/connection/tcp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/__init__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/base.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/connection.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/protocol.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/stream.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/exceptions/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/messages/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/messages/core.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/messages/dispatcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/__init__.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/parser.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/__init__.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/connect.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/err.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/hmsg.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/hpub.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/info.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/msg.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/ok.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/ping_pong.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/pub.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/sub.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/protocol/operations/unsub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/subscriptions/__init__.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/subscriptions/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/utils/__init__.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/utils/json.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/utils/logger.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 natsio-0.2.0/natsio/utils/uuid.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 natsio-0.2.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 natsio-0.2.0/LICENSE
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 natsio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 natsio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 natsio-0.2.1/TODO.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 natsio-0.2.1/main.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 natsio-0.2.1/pyrightconfig.json
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 natsio-0.2.1/test.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 natsio-0.2.1/certs/client-cert.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 natsio-0.2.1/certs/client-key.pem
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 natsio-0.2.1/certs/rootCA.pem
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 natsio-0.2.1/certs/server-cert.pem
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 natsio-0.2.1/certs/server-key.pem
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/const.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/abc/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/abc/client.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/abc/connection.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/abc/dispatcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/abc/protocol.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/client/__init__.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/client/config.py
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/client/core.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/client/status.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/connection/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/connection/protocol.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/connection/status.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/connection/stream.py
+-rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/connection/tcp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/base.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/connection.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/protocol.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/stream.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/exceptions/subscription.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/messages/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/messages/core.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/messages/dispatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/__init__.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/parser.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/__init__.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/connect.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/err.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/hmsg.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/hpub.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/info.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/msg.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/ok.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/ping_pong.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/pub.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/sub.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/protocol/operations/unsub.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/subscriptions/__init__.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/subscriptions/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/utils/__init__.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/utils/json.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/utils/logger.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 natsio-0.2.1/natsio/utils/uuid.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 natsio-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 natsio-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 natsio-0.2.1/README.md
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 natsio-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 natsio-0.2.1/PKG-INFO
```

### Comparing `natsio-0.2.0/main.py` & `natsio-0.2.1/main.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/certs/client-cert.pem` & `natsio-0.2.1/certs/client-cert.pem`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/certs/client-key.pem` & `natsio-0.2.1/certs/client-key.pem`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/certs/rootCA.pem` & `natsio-0.2.1/certs/rootCA.pem`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/certs/server-cert.pem` & `natsio-0.2.1/certs/server-cert.pem`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/certs/server-key.pem` & `natsio-0.2.1/certs/server-key.pem`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/abc/connection.py` & `natsio-0.2.1/natsio/abc/connection.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/abc/dispatcher.py` & `natsio-0.2.1/natsio/abc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/client/config.py` & `natsio-0.2.1/natsio/client/config.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/client/core.py` & `natsio-0.2.1/natsio/client/core.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/connection/protocol.py` & `natsio-0.2.1/natsio/connection/protocol.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/connection/stream.py` & `natsio-0.2.1/natsio/connection/stream.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/connection/tcp.py` & `natsio-0.2.1/natsio/connection/tcp.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/exceptions/client.py` & `natsio-0.2.1/natsio/exceptions/client.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/exceptions/connection.py` & `natsio-0.2.1/natsio/exceptions/connection.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/exceptions/protocol.py` & `natsio-0.2.1/natsio/exceptions/protocol.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/exceptions/subscription.py` & `natsio-0.2.1/natsio/exceptions/subscription.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/messages/core.py` & `natsio-0.2.1/natsio/messages/core.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/messages/dispatcher.py` & `natsio-0.2.1/natsio/messages/dispatcher.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/parser.py` & `natsio-0.2.1/natsio/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/connect.py` & `natsio-0.2.1/natsio/protocol/operations/connect.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/hmsg.py` & `natsio-0.2.1/natsio/protocol/operations/hmsg.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/hpub.py` & `natsio-0.2.1/natsio/protocol/operations/hpub.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/info.py` & `natsio-0.2.1/natsio/protocol/operations/info.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/msg.py` & `natsio-0.2.1/natsio/protocol/operations/msg.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/ping_pong.py` & `natsio-0.2.1/natsio/protocol/operations/ping_pong.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/pub.py` & `natsio-0.2.1/natsio/protocol/operations/pub.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/sub.py` & `natsio-0.2.1/natsio/protocol/operations/sub.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/protocol/operations/unsub.py` & `natsio-0.2.1/natsio/protocol/operations/unsub.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/natsio/subscriptions/core.py` & `natsio-0.2.1/natsio/subscriptions/core.py`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/LICENSE` & `natsio-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `natsio-0.2.0/pyproject.toml` & `natsio-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "natsio"
 description = "NATS client for Python"
 requires-python = ">=3.9"
 license = "MIT"
+readme = "README.md"
 authors = [{ name = "Corrupt Mane", email = "corruptmane@gmail.com" }]
 maintainers = [{ name = "Corrupt Mane", email = "corruptmane@gmail.com" }]
 keywords = [
     "nats",
     "nats.io",
     "nats-python",
     "nats-client",
```

