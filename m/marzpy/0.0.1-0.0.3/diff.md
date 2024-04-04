# Comparing `tmp/marzpy-0.0.1.tar.gz` & `tmp/marzpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marzpy-0.0.1.tar", last modified: Mon Sep 18 22:28:19 2023, max compression
+gzip compressed data, was "marzpy-0.0.3.tar", last modified: Thu Apr  4 23:20:32 2024, max compression
```

## Comparing `marzpy-0.0.1.tar` & `marzpy-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-09-18 22:28:19.347919 marzpy-0.0.1/
--rw-rw-rw-   0        0        0      333 2023-09-18 22:28:19.346922 marzpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10402 2023-09-18 21:49:48.000000 marzpy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-09-18 22:28:19.321988 marzpy-0.0.1/marzpy/
--rw-rw-rw-   0        0        0       30 2023-09-18 22:02:28.000000 marzpy-0.0.1/marzpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-18 22:28:19.345923 marzpy-0.0.1/marzpy/api/
--rw-rw-rw-   0        0        0      461 2023-09-18 22:01:55.000000 marzpy-0.0.1/marzpy/api/__init__.py
--rw-rw-rw-   0        0        0     3334 2023-09-18 22:01:59.000000 marzpy-0.0.1/marzpy/api/admin.py
--rw-rw-rw-   0        0        0     1385 2023-09-18 22:02:02.000000 marzpy-0.0.1/marzpy/api/core.py
--rw-rw-rw-   0        0        0     3510 2023-09-18 22:02:06.000000 marzpy-0.0.1/marzpy/api/node.py
--rw-rw-rw-   0        0        0     1019 2023-09-18 22:02:10.000000 marzpy-0.0.1/marzpy/api/send_requests.py
--rw-rw-rw-   0        0        0     1260 2023-09-18 22:02:13.000000 marzpy-0.0.1/marzpy/api/subscription.py
--rw-rw-rw-   0        0        0     1345 2023-09-18 22:02:16.000000 marzpy-0.0.1/marzpy/api/system.py
--rw-rw-rw-   0        0        0     2942 2023-09-18 22:02:20.000000 marzpy-0.0.1/marzpy/api/template.py
--rw-rw-rw-   0        0        0     4708 2023-09-18 22:02:22.000000 marzpy-0.0.1/marzpy/api/user.py
--rw-rw-rw-   0        0        0      311 2023-09-18 22:02:31.000000 marzpy-0.0.1/marzpy/marzban.py
-drwxrwxrwx   0        0        0        0 2023-09-18 22:28:19.330990 marzpy-0.0.1/marzpy.egg-info/
--rw-rw-rw-   0        0        0      333 2023-09-18 22:28:19.000000 marzpy-0.0.1/marzpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-09-18 22:28:19.000000 marzpy-0.0.1/marzpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-18 22:28:19.000000 marzpy-0.0.1/marzpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-09-18 22:28:19.000000 marzpy-0.0.1/marzpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-18 22:28:19.347919 marzpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-09-18 22:26:03.000000 marzpy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 23:20:28.000000 marzpy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 23:20:32.092160 marzpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-04 23:20:28.000000 marzpy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.088160 marzpy-0.0.3/marzpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/marzpy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/send_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/marzban.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/marzpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:20:32.092160 marzpy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 23:20:28.000000 marzpy-0.0.3/setup.py
```

### Comparing `marzpy-0.0.1/README.md` & `marzpy-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,359 +1,363 @@
-# marzpy
-A Python library that helps you easily use [Marzban](https://github.com/Gozargah/Marzban)'s API panel
-## installation
-```
-pip install marzpy
-```
-requirements : ```requests```
-# How To Use
-```python
-from marzpy import Marzban
-
-panel = Marzban("username","password","https://example.com")
-
-mytoken = panel.get_token()
-
-# panel.anyfunction()
-
-```
-# Features
-
-- Admin
-    - [get token](#get-token)
-    - [get admin](#get-current-admin)
-    - [create admin](#create-admin)
-    - [modify admin](#modify-admin)
-    - [remove admin](#remove-admin)
-    - [get all admins](#get-all-admins)
-- Subscription
-    - [user subscription](#user-subscription)
-    - [user subscription info](#user-subscription-info)
-- System
-    - [get system stats](#get-system-stats)
-    - [get inbounds](#get-inbounds)
-    - [get hosts](#get-hosts)
-    - [modify hosts](#modify-hosts)
-- Core
-    - [get core stats](#get-core-stats)
-    - [restart core](#restart-core)
-    - [get core config](#get-core-config)
-    - [modify core config](#modify-core-config)
-- User
-    - [add user](#add-user)
-    - [get user](#get-user)
-    - [modify user](#modify-user)
-    - [remove user](#remove-user)
-    - [reset user data usage](#reset-user-data-usage)
-    - [reset all users data usage](#reset-all-users-data-usage)
-    - [get all users](#get-all-users)
-    - [get user usage](#get-user-usage)
-- User Template
-    - [get all user templates](#get-all-user-templates)
-    - [add user template](#add-user-template)
-    - [get user template](#get-user-template)
-    - [modify user template](#modify-user-template)
-    - [remove user template](#remove-user-template)
-- Node
-    - [add node](#add-node)
-    - [get node](#get-node)
-    - [modify node](#modify-node)
-    - [remove node](#remove-node)
-    - [get all nodes](#get-all-nodes)
-    - [reconenct node](#reconenct-node)
-    - [get all nodes usage](#get-node-usage)
-
-# Examples
-### Get Token
-```python
-
-from marzpy import Marzban
-
-panel = Marzban("username","password","https://example.com")
-
-mytoken = panel.get_token()
-
-```
-### Get Current admin
-```python
-admin = panel.get_current_admin(token=mytoken)
-print(admin) #output: {'username': 'admin', 'is_sudo': True}
-```
-### Create Admin
-```python
-info = {'username':'test','password':'pasword','is_sudo':False}
-rsault = panel.create_admin(token=mytoken,data=info)
-print(result) #output: success
-```
-### Modify Admin
-```python
-target_admin = "test"
-info = {'password':'newpassword','is_sudo':False}
-result = panel.change_admin_password(username=target_admin,token=mytoken,data=info)
-print(result) #output: success
-```
-### Remove Admin
-```python
-target_admin = "test"
-result = panel.delete_admin(username=target_admin,token=mytoken)
-print(result) #output: success
-```
-### Get All Admins
-```python
-result = panel.get_all_admins(token=mytoken)
-print(result) 
-#output: [{'username': 'test', 'is_sudo': True}, {'username': 'test1', 'is_sudo': False}]
-```
-### User Subscription
-```python
-subscription_url = "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
-result = panel.get_subscription(subscription_url)
-print(result) #output: Configs
-```
-### User Subscription info
-```python
-subscription_url =  "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
-result = panel.get_subscription_info(subscription_url)
-print(result) #output: User information (usage,links,inbounds,....)
-```
-### Get System Stats
-```python
-result = panel.get_system_stats(token=mytoken)
-print(result) #output: system stats Memory & CPU usage ...
-```
-### Get Inbounds
-```python
-result = panel.get_inbounds(token=mytoken)
-print(result) #output: list of inbounds
-```
-### Get Hosts
-```python
-result = panel.get_hosts(token=mytoken)
-print(result) #output: list of hosts
-```
-### Modify Hosts
-```python
-hosts = {
-  "VMess TCP": [
-    {
-      "remark": "somename",
-      "address": "someaddress",
-      "port": 0,
-      "sni": "somesni",
-      "host": "somehost",
-      "security": "inbound_default",
-      "alpn": "",
-      "fingerprint": ""
-    }
-  ]
-}
-# **Backup first**
-result = panel.modify_hosts(token=mytoken,data=hosts)
-print(result) #output: hosts
-```
-### Get Core Stats
-```python
-result = panel.get_xray_core(token=mytoken)
-print(result)
- #output: {'version': '1.8.1', 'started': True, 'logs_websocket': '/api/core/logs'}
-```
-### Restart Core
-```python
-result = panel.restart_xray_core(token=mytoken)
-print(result)
- #output: success
-```
-### Get Core Config
-```python
-result = panel.get_xray_config(token=mytoken)
-print(result) #output: your xray core config
-```
-### Modify Core Config
-```python
-new_config={"your config"}
-result = panel.modify_xray_config(token=mytoken,config=new_config)
-print(result) #output: success
-```
-### Add User
-```python
-from marzpy.api.user import User
-
-user = User(
-    username="Mewhrzad",
-    proxies={
-        "vmess": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
-        "vless": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
-    },
-    inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
-    expire=0,
-    data_limit=0,
-    data_limit_reset_strategy="no_reset",
-)
-result = panel.add_user(user=user, token=token) #return new User object
-
-print(result.username) #-> Mewhrzad, #user.proxies, #user.inbounds, #user.expire, #user.data_limit, #userdata_limit_reset_strategy, #user.status, #user.used_traffic, #user.lifetime_used_traffic, #user.created_at, #user.links, #user.subscription_url, #user.excluded_inbounds
-```
-### Get User
-```python
-result = panel.get_user("Mewhrzad",token=mytoken) #return User object
-print(result.subscription_url)
-```
-### Modify User
-```python
-new_user = User(
-    username="test",
-    proxies={
-        "vmess": {"id": "35e4e39c-7d5c-4f4b-8b71-558e4f37ff53"},
-        "vless": {"id": "35e4e39c-7d5c-4f4b-8b71-558e4f37ff53"},
-    },
-    inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
-    expire=0,
-    data_limit=0,
-    data_limit_reset_strategy="no_reset",
-    status="active",
-)
-result = panel.modify_user("Mewhrzad", token=mytoken, user=new_user)
-print(result.subscription_url) #output: modified user object
-```
-### Remove User
-```python
-result = panel.delete_user("test", token=mytoken)
-print(result) #output: success
-```
-### Reset User Data Usage
-```python
-result = panel.reset_user_traffic("test", token=mytoken)
-print(result) #output: success
-```
-### Reset All Users Data Usage
-```python
-result = panel.reset_all_users_traffic(token=mytoken)
-print(result) #output: success
-```
-### Get All Users
-```python
-result = panel.get_all_users(token=mytoken) #return list of users
-for user in result:
-    print(user.username) 
-```
-### Get User Usage
-```python
-result = panel.get_user_usage("mewhrzad",token=mytoken)
-print(result) 
-#output: [{'node_id': None, 'node_name': 'MTN', 'used_traffic': 0}, 
-#{'node_id': 1, 'node_name': 'MCI', 'used_traffic': 0}]
-```
-### Get All User Templates
-```python
-result = panel.get_all_templates(token=mytoken) #return template list object
-for template in result:
-    print(template.name)
-```
-### Add User Template
-```python
-from marzpy.api.template import Template
-
-temp = Template(
-    name="new_template",
-    inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
-    data_limit=0,
-    expire_duration=0,
-    username_prefix=None,
-    username_suffix=None,
-)
-result = panel.add_template(token=mytoken, template=temp)  # return new Template object
-print(result.name) #output: new_template
-```
-### Get User Template
-```python
-template_id = 11
-result = panel.get_template_by_id(token=mytoken, id=template_id) # return Template object
-print(result.name) #output: new_template
-```
-### Modify User Template
-```python
-from marzpy.api.template import Template
-
-temp = Template(
-    name="new_template2",
-    inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
-    data_limit=0,
-    expire_duration=0,
-    username_prefix=None,
-    username_suffix=None,
-)
-result = panel.modify_template_by_id(
-    id=1, token=mytoken, template=temp)  # return Modified Template object
-print(result.name) #output: new_template2
-```
-### Remove User Template
-```python
-result = panel.delete_template_by_id(id=1, token=mytoken)
-print(result) #output: success
-```
-### Add Node
-```python
-from marzpy.api.node import Node
-
-my_node = Node(
-    name="somename",
-    address="test.example.com",
-    port=62050,
-    api_port=62051,
-    certificate="your_cert",
-    id=4,
-    xray_version="1.8.1",
-    status="connected",
-    message="string",
-)
-
-result = panel.add_node(token=mytoken, node=my_node)  # return new Node object
-print(result.address)
-```
-### Get Node
-```python
-result = panel.get_node_by_id(id=1, token=mytoken)  # return exist Node object
-print(result.address) #output: address of node 1
-```
-### Modify Node
-```python
-from marzpy.api.node import Node
-
-my_node = Node(
-    name="somename",
-    address="test.example.com",
-    port=62050,
-    api_port=62051,
-    certificate="your_cert",
-    id=4,
-    xray_version="1.8.1",
-    status="connected",
-    message="string",
-)
-
-result = panel.modify_node_by_id(id=1, token=mytoken,node=my_node)  # return modified Node object
-print(result.address) #output:test.example.com
-```
-### Remove Node
-```python
-result = panel.delete_node(id=1, token=mytoken)
-print(result) #output: success
-```
-### Get All Nodes
-```python
-result = panel.get_all_nodes(token=mytoken)  # return List of Node object
-for node in result:
-    print(node.address)
-```
-### Reconenct Node
-```python
-result = panel.reconnect_node(id=1,token=mytoken)
-print(result) #output: success
-```
-### Get Node Usage
-```python
-result = panel.get_nodes_usage(token=mytoken)
-for node in result:
-    print(node)
-#output:{'node_id': 1, 'node_name': 'N1', 'uplink': 1000000000000, 'downlink': 1000000000000}
-# {'node_id': 2, 'node_name': 'N2', 'uplink': 1000000000000, 'downlink': 1000000000000}
-```
+# marzpy
+A Python library that helps you easily use [Marzban](https://github.com/Gozargah/Marzban)'s API panel
+## installation
+```shell
+pip install marzpy
+```
+requirements : ```requests```
+# How To Use
+```python
+from marzpy import Marzban
+
+panel = Marzban("username","password","https://example.com")
+
+mytoken = panel.get_token()
+
+# panel.anyfunction()
+
+```
+# Features
+
+- Admin
+    - [get token](#get-token)
+    - [get admin](#get-current-admin)
+    - [create admin](#create-admin)
+    - [modify admin](#modify-admin)
+    - [remove admin](#remove-admin)
+    - [get all admins](#get-all-admins)
+- Subscription
+    - [user subscription](#user-subscription)
+    - [user subscription info](#user-subscription-info)
+- System
+    - [get system stats](#get-system-stats)
+    - [get inbounds](#get-inbounds)
+    - [get hosts](#get-hosts)
+    - [modify hosts](#modify-hosts)
+- Core
+    - [get core stats](#get-core-stats)
+    - [restart core](#restart-core)
+    - [get core config](#get-core-config)
+    - [modify core config](#modify-core-config)
+- User
+    - [add user](#add-user)
+    - [get user](#get-user)
+    - [modify user](#modify-user)
+    - [remove user](#remove-user)
+    - [reset user data usage](#reset-user-data-usage)
+    - [reset all users data usage](#reset-all-users-data-usage)
+    - [get all users](#get-all-users)
+    - [get user usage](#get-user-usage)
+- User Template
+    - [get all user templates](#get-all-user-templates)
+    - [add user template](#add-user-template)
+    - [get user template](#get-user-template)
+    - [modify user template](#modify-user-template)
+    - [remove user template](#remove-user-template)
+- Node
+    - [add node](#add-node)
+    - [get node](#get-node)
+    - [modify node](#modify-node)
+    - [remove node](#remove-node)
+    - [get all nodes](#get-all-nodes)
+    - [reconenct node](#reconenct-node)
+    - [get all nodes usage](#get-node-usage)
+    - 
+## Thanks To 
+
+- [ErfanTech](https://github.com/ErfanTech) :laughing:
+
+# Examples
+### Get Token
+```python
+
+from marzpy import Marzban
+
+panel = Marzban("username","password","https://example.com")
+
+mytoken = panel.get_token()
+
+```
+### Get Current admin
+```python
+admin = panel.get_current_admin(token=mytoken)
+print(admin) #output: {'username': 'admin', 'is_sudo': True}
+```
+### Create Admin
+```python
+info = {'username':'test','password':'pasword','is_sudo':False}
+rsault = panel.create_admin(token=mytoken,data=info)
+print(result) #output: success
+```
+### Modify Admin
+```python
+target_admin = "test"
+info = {'password':'newpassword','is_sudo':False}
+result = panel.change_admin_password(username=target_admin,token=mytoken,data=info)
+print(result) #output: success
+```
+### Remove Admin
+```python
+target_admin = "test"
+result = panel.delete_admin(username=target_admin,token=mytoken)
+print(result) #output: success
+```
+### Get All Admins
+```python
+result = panel.get_all_admins(token=mytoken)
+print(result) 
+#output: [{'username': 'test', 'is_sudo': True}, {'username': 'test1', 'is_sudo': False}]
+```
+### User Subscription
+```python
+subscription_url = "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
+result = panel.get_subscription(subscription_url)
+print(result) #output: Configs
+```
+### User Subscription info
+```python
+subscription_url =  "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
+result = panel.get_subscription_info(subscription_url)
+print(result) #output: User information (usage,links,inbounds,....)
+```
+### Get System Stats
+```python
+result = panel.get_system_stats(token=mytoken)
+print(result) #output: system stats Memory & CPU usage ...
+```
+### Get Inbounds
+```python
+result = panel.get_inbounds(token=mytoken)
+print(result) #output: list of inbounds
+```
+### Get Hosts
+```python
+result = panel.get_hosts(token=mytoken)
+print(result) #output: list of hosts
+```
+### Modify Hosts
+```python
+hosts = {
+  "VMess TCP": [
+    {
+      "remark": "somename",
+      "address": "someaddress",
+      "port": 0,
+      "sni": "somesni",
+      "host": "somehost",
+      "security": "inbound_default",
+      "alpn": "",
+      "fingerprint": ""
+    }
+  ]
+}
+# **Backup first**
+result = panel.modify_hosts(token=mytoken,data=hosts)
+print(result) #output: hosts
+```
+### Get Core Stats
+```python
+result = panel.get_xray_core(token=mytoken)
+print(result)
+ #output: {'version': '1.8.1', 'started': True, 'logs_websocket': '/api/core/logs'}
+```
+### Restart Core
+```python
+result = panel.restart_xray_core(token=mytoken)
+print(result)
+ #output: success
+```
+### Get Core Config
+```python
+result = panel.get_xray_config(token=mytoken)
+print(result) #output: your xray core config
+```
+### Modify Core Config
+```python
+new_config={"your config"}
+result = panel.modify_xray_config(token=mytoken,config=new_config)
+print(result) #output: success
+```
+### Add User
+```python
+from marzpy.api.user import User
+
+user = User(
+    username="Mewhrzad",
+    proxies={
+        "vmess": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
+        "vless": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
+    },
+    inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
+    expire=0,
+    data_limit=0,
+    data_limit_reset_strategy="no_reset",
+)
+result = panel.add_user(user=user, token=token) #return new User object
+
+print(result.username) #-> Mewhrzad, #user.proxies, #user.inbounds, #user.expire, #user.data_limit, #userdata_limit_reset_strategy, #user.status, #user.used_traffic, #user.lifetime_used_traffic, #user.created_at, #user.links, #user.subscription_url, #user.excluded_inbounds
+```
+### Get User
+```python
+result = panel.get_user("Mewhrzad",token=mytoken) #return User object
+print(result.subscription_url)
+```
+### Modify User
+```python
+new_user = User(
+    username="test",
+    proxies={
+        "vmess": {"id": "35e4e39c-7d5c-4f4b-8b71-558e4f37ff53"},
+        "vless": {"id": "35e4e39c-7d5c-4f4b-8b71-558e4f37ff53"},
+    },
+    inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
+    expire=0,
+    data_limit=0,
+    data_limit_reset_strategy="no_reset",
+    status="active",
+)
+result = panel.modify_user("Mewhrzad", token=mytoken, user=new_user)
+print(result.subscription_url) #output: modified user object
+```
+### Remove User
+```python
+result = panel.delete_user("test", token=mytoken)
+print(result) #output: success
+```
+### Reset User Data Usage
+```python
+result = panel.reset_user_traffic("test", token=mytoken)
+print(result) #output: success
+```
+### Reset All Users Data Usage
+```python
+result = panel.reset_all_users_traffic(token=mytoken)
+print(result) #output: success
+```
+### Get All Users
+```python
+result = panel.get_all_users(token=mytoken) #return list of users
+for user in result:
+    print(user.username) 
+```
+### Get User Usage
+```python
+result = panel.get_user_usage("mewhrzad",token=mytoken)
+print(result) 
+#output: [{'node_id': None, 'node_name': 'MTN', 'used_traffic': 0}, 
+#{'node_id': 1, 'node_name': 'MCI', 'used_traffic': 0}]
+```
+### Get All User Templates
+```python
+result = panel.get_all_templates(token=mytoken) #return template list object
+for template in result:
+    print(template.name)
+```
+### Add User Template
+```python
+from marzpy.api.template import Template
+
+temp = Template(
+    name="new_template",
+    inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
+    data_limit=0,
+    expire_duration=0,
+    username_prefix=None,
+    username_suffix=None,
+)
+result = panel.add_template(token=mytoken, template=temp)  # return new Template object
+print(result.name) #output: new_template
+```
+### Get User Template
+```python
+template_id = 11
+result = panel.get_template_by_id(token=mytoken, id=template_id) # return Template object
+print(result.name) #output: new_template
+```
+### Modify User Template
+```python
+from marzpy.api.template import Template
+
+temp = Template(
+    name="new_template2",
+    inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
+    data_limit=0,
+    expire_duration=0,
+    username_prefix=None,
+    username_suffix=None,
+)
+result = panel.modify_template_by_id(
+    id=1, token=mytoken, template=temp)  # return Modified Template object
+print(result.name) #output: new_template2
+```
+### Remove User Template
+```python
+result = panel.delete_template_by_id(id=1, token=mytoken)
+print(result) #output: success
+```
+### Add Node
+```python
+from marzpy.api.node import Node
+
+my_node = Node(
+    name="somename",
+    address="test.example.com",
+    port=62050,
+    api_port=62051,
+    certificate="your_cert",
+    id=4,
+    xray_version="1.8.1",
+    status="connected",
+    message="string",
+)
+
+result = panel.add_node(token=mytoken, node=my_node)  # return new Node object
+print(result.address)
+```
+### Get Node
+```python
+result = panel.get_node_by_id(id=1, token=mytoken)  # return exist Node object
+print(result.address) #output: address of node 1
+```
+### Modify Node
+```python
+from marzpy.api.node import Node
+
+my_node = Node(
+    name="somename",
+    address="test.example.com",
+    port=62050,
+    api_port=62051,
+    certificate="your_cert",
+    id=4,
+    xray_version="1.8.1",
+    status="connected",
+    message="string",
+)
+
+result = panel.modify_node_by_id(id=1, token=mytoken,node=my_node)  # return modified Node object
+print(result.address) #output:test.example.com
+```
+### Remove Node
+```python
+result = panel.delete_node(id=1, token=mytoken)
+print(result) #output: success
+```
+### Get All Nodes
+```python
+result = panel.get_all_nodes(token=mytoken)  # return List of Node object
+for node in result:
+    print(node.address)
+```
+### Reconenct Node
+```python
+result = panel.reconnect_node(id=1,token=mytoken)
+print(result) #output: success
+```
+### Get Node Usage
+```python
+result = panel.get_nodes_usage(token=mytoken)
+for node in result:
+    print(node)
+#output:{'node_id': 1, 'node_name': 'N1', 'uplink': 1000000000000, 'downlink': 1000000000000}
+# {'node_id': 2, 'node_name': 'N2', 'uplink': 1000000000000, 'downlink': 1000000000000}
+```
```

### Comparing `marzpy-0.0.1/marzpy/api/admin.py` & `marzpy-0.0.3/marzpy/api/admin.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from .send_requests import *
-
-
-class Admin:
-    def __init__(self, username: str, password: str, panel_address: str):
-        self.username = username
-        self.password = password
-        self.panel_address = panel_address
-
-    def get_token(self):
-        """login for Authorization token
-
-        Returns: `~dict`: Authorization token
-        """
-        try:
-            request_address = f"{self.panel_address}/api/admin/token"
-            payload = {"username": self.username, "password": self.password}
-            response = requests.post(
-                request_address,
-                data=payload,
-                timeout=3000,
-                headers={
-                    "Accept": "application/json",
-                    "Content-Type": "application/x-www-form-urlencoded",
-                },
-            )
-            response.raise_for_status()  # Raise an exception for non-200 status codes
-            result = json.loads(response.content)
-            result["panel_address"] = self.panel_address
-            return result
-        except requests.exceptions.RequestException as ex:
-            print(f"Request Exception: {ex}")
-            return None
-        except json.JSONDecodeError as ex:
-            print(f"JSON Decode Error: {ex}")
-            return None
-
-    def get_current_admin(self, token: dict):
-        """get current admin who has logged in.
-
-        Parameters:
-            token (``dict``) : Authorization token
-
-        Returns:
-        `~dict`: {"username": "str" , "is_sudo": true}
-        """
-        return send_request(endpoint="admin", token=token, method="get")
-
-    def create_admin(self, token: dict, data: dict):
-        """add new admin.
-
-        Parameters:
-            token (``dict``) : Authorization token
-            data (``dict``) : information of new admin
-
-        Returns:
-        `~dict`: username && is_sudo
-        """
-        send_request(endpoint="admin", token=token, method="post", data=data)
-        return "success"
-
-    def change_admin_password(self, username: str, token: dict, data: dict):
-        """change exist admins password.
-
-        *you cant modify sudo admins password*
-
-        Parameters:
-            username (``str``) : username of admin
-            token (``dict``) : Authorization token
-            data (``dict``) : information of new admin
-
-        Returns:
-        `~dict`: username && is_sudo
-        """
-        send_request(
-            endpoint=f"admin/{username}",
-            token=token,
-            method="put",
-            data=data,
-        )
-        return "success"
-
-    def delete_admin(self, username: str, token: dict):
-        """delete admin.
-
-        Parameters:
-            username (``str``) : username of admin
-            token (``dict``) : Authorization token
-
-        Returns:
-        `~str`: success
-        """
-        send_request(endpoint=f"admin/{username}", token=token, method="delete")
-        return "success"
-
-    def get_all_admins(self, token: dict):
-        """get all admins.
-
-        Parameters:
-            token (``dict``) : Authorization token
-
-        Returns:
-        `~list`: [{username && is_sudo}]
-        """
-        return send_request(endpoint=f"admins", token=token, method="get")
+from .send_requests import *
+
+
+class Admin:
+    def __init__(self, username: str, password: str, panel_address: str):
+        self.username = username
+        self.password = password
+        self.panel_address = panel_address
+
+    def get_token(self):
+        """login for Authorization token
+
+        Returns: `~dict`: Authorization token
+        """
+        try:
+            request_address = f"{self.panel_address}/api/admin/token"
+            payload = {"username": self.username, "password": self.password}
+            response = requests.post(
+                request_address,
+                data=payload,
+                timeout=3000,
+                headers={
+                    "Accept": "application/json",
+                    "Content-Type": "application/x-www-form-urlencoded",
+                },
+            )
+            response.raise_for_status()  # Raise an exception for non-200 status codes
+            result = json.loads(response.content)
+            result["panel_address"] = self.panel_address
+            return result
+        except requests.exceptions.RequestException as ex:
+            print(f"Request Exception: {ex}")
+            return None
+        except json.JSONDecodeError as ex:
+            print(f"JSON Decode Error: {ex}")
+            return None
+
+    def get_current_admin(self, token: dict):
+        """get current admin who has logged in.
+
+        Parameters:
+            token (``dict``) : Authorization token
+
+        Returns:
+        `~dict`: {"username": "str" , "is_sudo": true}
+        """
+        return send_request(endpoint="admin", token=token, method="get")
+
+    def create_admin(self, token: dict, data: dict):
+        """add new admin.
+
+        Parameters:
+            token (``dict``) : Authorization token
+            data (``dict``) : information of new admin
+
+        Returns:
+        `~dict`: username && is_sudo
+        """
+        send_request(endpoint="admin", token=token, method="post", data=data)
+        return "success"
+
+    def change_admin_password(self, username: str, token: dict, data: dict):
+        """change exist admins password.
+
+        *you cant modify sudo admins password*
+
+        Parameters:
+            username (``str``) : username of admin
+            token (``dict``) : Authorization token
+            data (``dict``) : information of new admin
+
+        Returns:
+        `~dict`: username && is_sudo
+        """
+        send_request(
+            endpoint=f"admin/{username}",
+            token=token,
+            method="put",
+            data=data,
+        )
+        return "success"
+
+    def delete_admin(self, username: str, token: dict):
+        """delete admin.
+
+        Parameters:
+            username (``str``) : username of admin
+            token (``dict``) : Authorization token
+
+        Returns:
+        `~str`: success
+        """
+        send_request(endpoint=f"admin/{username}", token=token, method="delete")
+        return "success"
+
+    def get_all_admins(self, token: dict):
+        """get all admins.
+
+        Parameters:
+            token (``dict``) : Authorization token
+
+        Returns:
+        `~list`: [{username && is_sudo}]
+        """
+        return send_request(endpoint=f"admins", token=token, method="get")
```

### Comparing `marzpy-0.0.1/marzpy/api/node.py` & `marzpy-0.0.3/marzpy/api/node.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from .send_requests import *
-
-
-class Node:
-    def __init__(
-        self,
-        name="",
-        address="",
-        port=0,
-        api_port=0,
-        certificate="",
-        id=0,
-        xray_version="",
-        status="",
-        message="",
-    ):
-        self.name = name
-        self.address = address
-        self.port = port
-        self.api_port = api_port
-        self.certificate = certificate
-        self.id = id
-        self.xray_version = xray_version
-        self.status = status
-        self.message = message
-
-
-class NodeMethods:
-    def __init__(self) -> None:
-        pass
-
-    def add_node(self, token: dict, node: Node):
-        """add new node.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-            node (``api.Node``): node object
-
-        Returns:
-            `~object`: information of new node
-        """
-        return Node(
-            **send_request(
-                endpoint="node", token=token, method="post", data=node.__dict__
-            )
-        )
-
-    def get_node_by_id(self, id: int, token: dict):
-        """get exist node from id.
-
-        Parameters:
-            id (``int``): id of node
-
-            token (``dict``): Authorization token
-
-        Returns:
-            `~object`: information of new node
-        """
-        return Node(**send_request(endpoint=f"node/{id}", token=token, method="get"))
-
-    def modify_node_by_id(self, id: int, token: dict, node: object):
-        """edit exist node from id.
-
-        Parameters:
-            id (``int``): id of node
-
-            token (``dict``): Authorization token
-
-            node (``api.Node``): node object
-
-        Returns:
-            `~object`: information of new node
-        """
-        request = send_request(
-            endpoint=f"node/{id}", token=token, method="put", data=node.__dict__
-        )
-        return Node(**request)
-
-    def delete_node(self, id: int, token: dict):
-        """delete node from id.
-
-        Parameters:
-            id (``int``): id of node
-
-            token (``dict``): Authorization token
-
-        Returns:
-            `~str`: success
-        """
-        send_request(endpoint=f"node/{id}", token=token, method="delete")
-        return "success"
-
-    def get_all_nodes(self, token: dict):
-        """get all nodes.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-        Returns:
-            `~list of objects`: [Node]
-        """
-        request = send_request(endpoint="nodes", token=token, method="get")
-        node_list = [Node()]
-        for node in request:
-            node_list.append(Node(**node))
-        del node_list[0]
-        return node_list
-
-    def reconnect_node(self, id: int, token: dict):
-        """reconnect from id.
-
-        Parameters:
-            id (``int``): id of node
-
-            token (``dict``): Authorization token
-
-        Returns:
-            `~str`: success
-        """
-        request = send_request(
-            endpoint=f"node/{id}/reconnect", token=token, method="post"
-        )
-
-        return "success"
-
-    def get_nodes_usage(self, token: dict):
-        """get all nodes usage.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-        Returns:
-            `~dict`: "usage" : []
-        """
-        request = send_request(endpoint="nodes/usage", token=token, method="get")
-        return request["usages"]
+from .send_requests import *
+
+
+class Node:
+    def __init__(
+        self,
+        name="",
+        address="",
+        port=0,
+        api_port=0,
+        certificate="",
+        id=0,
+        xray_version="",
+        status="",
+        message="",
+    ):
+        self.name = name
+        self.address = address
+        self.port = port
+        self.api_port = api_port
+        self.certificate = certificate
+        self.id = id
+        self.xray_version = xray_version
+        self.status = status
+        self.message = message
+
+
+class NodeMethods:
+    def __init__(self) -> None:
+        pass
+
+    def add_node(self, token: dict, node: Node):
+        """add new node.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+            node (``api.Node``): node object
+
+        Returns:
+            `~object`: information of new node
+        """
+        return Node(
+            **send_request(
+                endpoint="node", token=token, method="post", data=node.__dict__
+            )
+        )
+
+    def get_node_by_id(self, id: int, token: dict):
+        """get exist node from id.
+
+        Parameters:
+            id (``int``): id of node
+
+            token (``dict``): Authorization token
+
+        Returns:
+            `~object`: information of new node
+        """
+        return Node(**send_request(endpoint=f"node/{id}", token=token, method="get"))
+
+    def modify_node_by_id(self, id: int, token: dict, node: object):
+        """edit exist node from id.
+
+        Parameters:
+            id (``int``): id of node
+
+            token (``dict``): Authorization token
+
+            node (``api.Node``): node object
+
+        Returns:
+            `~object`: information of new node
+        """
+        request = send_request(
+            endpoint=f"node/{id}", token=token, method="put", data=node.__dict__
+        )
+        return Node(**request)
+
+    def delete_node(self, id: int, token: dict):
+        """delete node from id.
+
+        Parameters:
+            id (``int``): id of node
+
+            token (``dict``): Authorization token
+
+        Returns:
+            `~str`: success
+        """
+        send_request(endpoint=f"node/{id}", token=token, method="delete")
+        return "success"
+
+    def get_all_nodes(self, token: dict):
+        """get all nodes.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+        Returns:
+            `~list of objects`: [Node]
+        """
+        request = send_request(endpoint="nodes", token=token, method="get")
+        node_list = [Node()]
+        for node in request:
+            node_list.append(Node(**node))
+        del node_list[0]
+        return node_list
+
+    def reconnect_node(self, id: int, token: dict):
+        """reconnect from id.
+
+        Parameters:
+            id (``int``): id of node
+
+            token (``dict``): Authorization token
+
+        Returns:
+            `~str`: success
+        """
+        request = send_request(
+            endpoint=f"node/{id}/reconnect", token=token, method="post"
+        )
+
+        return "success"
+
+    def get_nodes_usage(self, token: dict):
+        """get all nodes usage.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+        Returns:
+            `~dict`: "usage" : []
+        """
+        request = send_request(endpoint="nodes/usage", token=token, method="get")
+        return request["usages"]
```

### Comparing `marzpy-0.0.1/marzpy/api/system.py` & `marzpy-0.0.3/marzpy/api/system.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from .send_requests import send_request
-
-
-class System:
-    def __init__(self) -> None:
-        pass
-
-    def get_system_stats(self, token: dict):
-        """get server stats.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-        Returns:
-            `~dict`: server stats
-        """
-        return send_request(endpoint="system", token=token, method="get")
-
-    def get_inbounds(self, token: dict):
-        """get server inbounds.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-        Returns:
-            `~dict`: server inbounds
-        """
-        return send_request(endpoint="inbounds", token=token, method="get")
-
-    def get_hosts(self, token: dict):
-        """get server hosts.
-
-        Parameters:
-            token (``dict``): Authorization token
-
-        Returns:
-            `~dict`: server hosts
-        """
-        return send_request(endpoint="hosts", token=token, method="get")
-
-    def modify_hosts(self, token: dict, data: dict):
-        """get server hosts.
-
-        Parameters:
-            token (``dict``): Authorization token
-            data (``dict``) : new hosts data
-        Returns:
-            `~dict`: server hosts
-        """
-        return send_request(endpoint="hosts", token=token, method="put", data=data)
+from .send_requests import send_request
+
+
+class System:
+    def __init__(self) -> None:
+        pass
+
+    def get_system_stats(self, token: dict):
+        """get server stats.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+        Returns:
+            `~dict`: server stats
+        """
+        return send_request(endpoint="system", token=token, method="get")
+
+    def get_inbounds(self, token: dict):
+        """get server inbounds.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+        Returns:
+            `~dict`: server inbounds
+        """
+        return send_request(endpoint="inbounds", token=token, method="get")
+
+    def get_hosts(self, token: dict):
+        """get server hosts.
+
+        Parameters:
+            token (``dict``): Authorization token
+
+        Returns:
+            `~dict`: server hosts
+        """
+        return send_request(endpoint="hosts", token=token, method="get")
+
+    def modify_hosts(self, token: dict, data: dict):
+        """get server hosts.
+
+        Parameters:
+            token (``dict``): Authorization token
+            data (``dict``) : new hosts data
+        Returns:
+            `~dict`: server hosts
+        """
+        return send_request(endpoint="hosts", token=token, method="put", data=data)
```

### Comparing `marzpy-0.0.1/marzpy/api/template.py` & `marzpy-0.0.3/marzpy/api/template.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from .send_requests import *
-
-
-class Template:
-    def __init__(
-        self,
-        name="",
-        inbounds={},
-        data_limit={},
-        expire_duration=0,
-        username_prefix="",
-        username_suffix="",
-        id=None,
-    ):
-        self.name = name
-        self.inbounds = inbounds
-        self.data_limit = data_limit
-        self.expire_duration = expire_duration
-        self.username_prefix = username_prefix
-        self.username_suffix = username_suffix
-        self.id = id
-
-
-class TemplateMethods:
-    def get_all_templates(self, token: dict):
-        """get all templates list.
-
-        Parameters:
-            token (``dict``) : Authorization token
-
-        Returns:
-            `~list`: list of templates
-        """
-        request = send_request(endpoint="user_template", token=token, method="get")
-        template_list = [Template()]
-        for user in request:
-            template_list.append(Template(**user))
-        del template_list[0]
-        return template_list
-
-    def add_template(self, template: Template, token: dict):
-        """add new template.
-
-        Parameters:
-            token (``dict``) : Authorization token
-            template (``api.template object``) : template
-
-        Returns:
-            `~object`: information of new template
-        """
-        request = send_request(
-            endpoint="user_template", token=token, method="post", data=template.__dict__
-        )
-        return Template(**request)
-
-    def get_template_by_id(self, id: int, token: dict):
-        """get exist template from id.
-
-        Parameters:
-            id (``id``) : template id
-            token (``dict``) : Authorization token
-        Returns:
-            `~object`: information of template
-        """
-        request = send_request(
-            endpoint=f"user_template/{id}", token=token, method="get"
-        )
-
-        return Template(**request)
-
-    def modify_template_by_id(self, id: int, token: dict, template: Template):
-        """edit exist template from id.
-
-        Parameters:
-            id (``id``) : template id
-            token (``dict``) : Authorization token
-            template (``object``) template
-        Returns:
-            `~object`: information of edited template
-        """
-        request = send_request(
-            endpoint=f"user_template/{id}",
-            token=token,
-            method="put",
-            data=template.__dict__,
-        )
-        return Template(**request)
-
-    def delete_template_by_id(self, id: int, token: dict):
-        """delete template from id.
-
-        Parameters:
-            id (``id``) : template id
-            token (``dict``) : Authorization token
-        Returns:
-            `~str`: success
-        """
-        send_request(endpoint=f"user_template/{id}", token=token, method="delete")
-        return "success"
+from .send_requests import *
+
+
+class Template:
+    def __init__(
+        self,
+        name="",
+        inbounds={},
+        data_limit={},
+        expire_duration=0,
+        username_prefix="",
+        username_suffix="",
+        id=None,
+    ):
+        self.name = name
+        self.inbounds = inbounds
+        self.data_limit = data_limit
+        self.expire_duration = expire_duration
+        self.username_prefix = username_prefix
+        self.username_suffix = username_suffix
+        self.id = id
+
+
+class TemplateMethods:
+    def get_all_templates(self, token: dict):
+        """get all templates list.
+
+        Parameters:
+            token (``dict``) : Authorization token
+
+        Returns:
+            `~list`: list of templates
+        """
+        request = send_request(endpoint="user_template", token=token, method="get")
+        template_list = [Template()]
+        for user in request:
+            template_list.append(Template(**user))
+        del template_list[0]
+        return template_list
+
+    def add_template(self, template: Template, token: dict):
+        """add new template.
+
+        Parameters:
+            token (``dict``) : Authorization token
+            template (``api.template object``) : template
+
+        Returns:
+            `~object`: information of new template
+        """
+        request = send_request(
+            endpoint="user_template", token=token, method="post", data=template.__dict__
+        )
+        return Template(**request)
+
+    def get_template_by_id(self, id: int, token: dict):
+        """get exist template from id.
+
+        Parameters:
+            id (``id``) : template id
+            token (``dict``) : Authorization token
+        Returns:
+            `~object`: information of template
+        """
+        request = send_request(
+            endpoint=f"user_template/{id}", token=token, method="get"
+        )
+
+        return Template(**request)
+
+    def modify_template_by_id(self, id: int, token: dict, template: Template):
+        """edit exist template from id.
+
+        Parameters:
+            id (``id``) : template id
+            token (``dict``) : Authorization token
+            template (``object``) template
+        Returns:
+            `~object`: information of edited template
+        """
+        request = send_request(
+            endpoint=f"user_template/{id}",
+            token=token,
+            method="put",
+            data=template.__dict__,
+        )
+        return Template(**request)
+
+    def delete_template_by_id(self, id: int, token: dict):
+        """delete template from id.
+
+        Parameters:
+            id (``id``) : template id
+            token (``dict``) : Authorization token
+        Returns:
+            `~str`: success
+        """
+        send_request(endpoint=f"user_template/{id}", token=token, method="delete")
+        return "success"
```

