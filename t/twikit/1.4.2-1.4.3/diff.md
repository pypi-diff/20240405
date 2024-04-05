# Comparing `tmp/twikit-1.4.2.tar.gz` & `tmp/twikit-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.2.tar", last modified: Tue Apr  2 02:34:04 2024, max compression
+gzip compressed data, was "twikit-1.4.3.tar", last modified: Fri Apr  5 01:16:04 2024, max compression
```

## Comparing `twikit-1.4.2.tar` & `twikit-1.4.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.921992 twikit-1.4.2/
--rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     3534 2024-04-02 02:34:04.918995 twikit-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 02:34:04.921992 twikit-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.833226 twikit-1.4.2/twikit/
--rw-rw-rw-   0        0        0      601 2024-04-02 02:33:47.000000 twikit-1.4.2/twikit/__init__.py
--rw-rw-rw-   0        0        0   108902 2024-04-01 07:28:24.000000 twikit-1.4.2/twikit/client.py
--rw-rw-rw-   0        0        0     2076 2024-03-29 07:12:11.000000 twikit-1.4.2/twikit/errors.py
--rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.2/twikit/group.py
--rw-rw-rw-   0        0        0     1887 2024-04-01 07:48:50.000000 twikit-1.4.2/twikit/http.py
--rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.2/twikit/list.py
--rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/trend.py
--rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.2/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.915008 twikit-1.4.2/twikit/twikit_async/
--rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   112410 2024-03-30 16:49:28.000000 twikit-1.4.2/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.2/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1929 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.2/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.2/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.2/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     2215 2024-03-29 18:39:44.000000 twikit-1.4.2/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.2/twikit/user.py
--rw-rw-rw-   0        0        0    19707 2024-04-01 07:29:32.000000 twikit-1.4.2/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.856166 twikit-1.4.2/twikit.egg-info/
--rw-rw-rw-   0        0        0     3534 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.417485 twikit-1.4.3/
+-rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3534 2024-04-05 01:16:04.414492 twikit-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 01:16:04.417485 twikit-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.309772 twikit-1.4.3/twikit/
+-rw-rw-rw-   0        0        0      601 2024-04-05 01:12:09.000000 twikit-1.4.3/twikit/__init__.py
+-rw-rw-rw-   0        0        0   107913 2024-04-05 01:08:17.000000 twikit-1.4.3/twikit/client.py
+-rw-rw-rw-   0        0        0     2076 2024-03-29 07:12:11.000000 twikit-1.4.3/twikit/errors.py
+-rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.3/twikit/group.py
+-rw-rw-rw-   0        0        0     1887 2024-04-01 07:48:50.000000 twikit-1.4.3/twikit/http.py
+-rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.3/twikit/list.py
+-rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/trend.py
+-rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.3/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.409506 twikit-1.4.3/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   111344 2024-04-05 01:04:43.000000 twikit-1.4.3/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.3/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1929 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.3/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.3/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.3/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3354 2024-04-02 05:30:54.000000 twikit-1.4.3/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.3/twikit/user.py
+-rw-rw-rw-   0        0        0    20911 2024-04-05 01:12:40.000000 twikit-1.4.3/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.327725 twikit-1.4.3/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3534 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.2/LICENSE` & `twikit-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/PKG-INFO` & `twikit-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.2/README.md` & `twikit-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/setup.py` & `twikit-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/__init__.py` & `twikit-1.4.3/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 )
 from .message import Message
 from .trend import Trend
 from .tweet import ScheduledTweet, Tweet
 from .user import User
 from .utils import build_query
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
```

### Comparing `twikit-1.4.2/twikit/client.py` & `twikit-1.4.3/twikit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .user import User
 from .utils import (
     LIST_FEATURES,
     FEATURES,
     TOKEN,
     USER_FEATURES,
     Endpoint,
+    Flow,
     Result,
     build_tweet_data,
     build_user_data,
     find_dict,
     get_query_id,
     urlencode
 )
@@ -57,14 +58,15 @@
 
     def __init__(self, language: str | None = None, **kwargs) -> None:
         self._token = TOKEN
         self.language = language
         self.http = HTTPClient(**kwargs)
         self._user_id = None
         self._user_agent = UserAgent().random.strip()
+        self._act_as = None
 
     def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
         response = self.http.post(
             Endpoint.GUEST_TOKEN,
@@ -91,14 +93,17 @@
         if self.language is not None:
             headers['Accept-Language'] = self.language
             headers['X-Twitter-Client-Language'] = self.language
 
         csrf_token = self._get_csrf_token()
         if csrf_token is not None:
             headers['X-Csrf-Token'] = csrf_token
+        if self._act_as is not None:
+            headers['X-Act-As-User-Id'] = self._act_as
+            headers['X-Contributor-Version'] = '1'
         return headers
 
     def _get_csrf_token(self) -> str:
         """
         Retrieves the Cross-Site Request Forgery (CSRF) token from the
         current session's cookies.
 
@@ -147,127 +152,85 @@
         guest_token = self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
-        def _execute_task(
-            flow_token: str | None = None,
-            subtask_input: dict | None = None,
-            flow_name: str | None = None
-        ) -> dict:
-            url = Endpoint.TASK
-            if flow_name is not None:
-                url += f'?flow_name={flow_name}'
-
-            data = {}
-            if flow_token is not None:
-                data['flow_token'] = flow_token
-            if subtask_input is not None:
-                data['subtask_inputs'] = [subtask_input]
-
-            response = self.http.post(
-                url, data=json.dumps(data), headers=headers
-            ).json()
-            return response
-
-        flow_token = _execute_task(flow_name='login')['flow_token']
-        flow_token = _execute_task(flow_token)['flow_token']
-        response = _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'LoginEnterUserIdentifierSSO',
-                'settings_list': {
-                    'setting_responses': [
-                        {
-                            'key': 'user_identifier',
-                            'response_data': {
-                                'text_data': {'result': auth_info_1}
-                            }
+        flow = Flow(self, Endpoint.LOGIN_FLOW, headers)
+
+        flow.execute_task(params={'flow_name': 'login'})
+        flow.execute_task()
+        flow.execute_task({
+            'subtask_id': 'LoginEnterUserIdentifierSSO',
+            'settings_list': {
+                'setting_responses': [
+                    {
+                        'key': 'user_identifier',
+                        'response_data': {
+                            'text_data': {'result': auth_info_1}
                         }
-                    ],
+                    }
+                ],
+                'link': 'next_link'
+            }
+        })
+
+        if flow.task_id == 'LoginEnterAlternateIdentifierSubtask':
+            flow.execute_task({
+                'subtask_id': 'LoginEnterAlternateIdentifierSubtask',
+                'enter_text': {
+                    'text': auth_info_2,
                     'link': 'next_link'
                 }
+            })
+
+        flow.execute_task({
+            'subtask_id': 'LoginEnterPassword',
+            'enter_password': {
+                'password': password,
+                'link': 'next_link'
             }
-        )
+        })
 
-        flow_token = response['flow_token']
-        task_id = response['subtasks'][0]['subtask_id']
+        flow.execute_task({
+            'subtask_id': 'AccountDuplicationCheck',
+            'check_logged_in_account': {
+                'link': 'AccountDuplicationCheck_false'
+            }
+        })
 
-        if task_id == 'LoginEnterAlternateIdentifierSubtask':
-            response = _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginEnterAlternateIdentifierSubtask',
-                    'enter_text': {
-                        'text': auth_info_2,
-                        'link': 'next_link'
-                    }
-                }
-            )
-            flow_token = response['flow_token']
+        if not flow.response['subtasks']:
+            return
 
-        response = _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'LoginEnterPassword',
-                'enter_password': {
-                    'password': password,
-                    'link': 'next_link'
-                }
-            }
-        )
+        self._user_id = find_dict(flow.response, 'id_str')[0]
 
-        flow_token = response['flow_token']
+        if flow.task_id == 'LoginTwoFactorAuthChallenge':
+            print(find_dict(flow.response, 'secondary_text')[0]['text'])
 
-        response = _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'AccountDuplicationCheck',
-                'check_logged_in_account': {
-                    'link': 'AccountDuplicationCheck_false'
+            flow.execute_task({
+                'subtask_id': 'LoginTwoFactorAuthChallenge',
+                'enter_text': {
+                    'text': input('>>> '),
+                    'link': 'next_link'
                 }
-            },
-        )
+            })
 
-        if not response['subtasks']:
-            return
-        flow_token = response['flow_token']
-        task_id = response['subtasks'][0]['subtask_id']
-        self._user_id = find_dict(response, 'id_str')[0]
-
-        if task_id == 'LoginTwoFactorAuthChallenge':
-            print(find_dict(response, 'secondary_text')[0]['text'])
-            response = _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginTwoFactorAuthChallenge',
-                    'enter_text': {
-                        'text': input('>>> '),
-                        'link': 'next_link'
-                    }
-                }
-            )
-            task_id = response['subtasks'][0]['subtask_id']
+        if flow.task_id == 'LoginAcid':
+            print(find_dict(flow.response, 'secondary_text')[0]['text'])
 
-        if task_id == 'LoginAcid':
-            print(find_dict(response, 'secondary_text')[0]['text'])
-            response = _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginAcid',
-                    'enter_text': {
-                        'text': input('>>> '),
-                        'link': 'next_link'
-                    }
+            flow.execute_task({
+                'subtask_id': 'LoginAcid',
+                'enter_text': {
+                    'text': input('>>> '),
+                    'link': 'next_link'
                 }
-            )
+            })
 
-        return response
+        return flow.response
 
     def logout(self) -> Response:
         """
         Logs out of the currently logged-in account.
         """
         response = self.http.post(
             Endpoint.LOGOUT,
@@ -381,14 +344,26 @@
         .get_cookies
         .save_cookies
         .set_cookies
         """
         with open(path, 'r', encoding='utf-8') as f:
             self.set_cookies(json.load(f))
 
+    def set_delegate_account(self, user_id: str | None) -> None:
+        """
+        Sets the account to act as.
+
+        Parameters
+        ----------
+        user_id : str | None
+            The user ID of the account to act as.
+            Set to None to clear the delegated account.
+        """
+        self._act_as = user_id
+
     def _search(
         self,
         query: str,
         product: str,
         count: int,
         cursor: str | None
     ) -> dict:
```

### Comparing `twikit-1.4.2/twikit/errors.py` & `twikit-1.4.3/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/group.py` & `twikit-1.4.3/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/http.py` & `twikit-1.4.3/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/list.py` & `twikit-1.4.3/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/message.py` & `twikit-1.4.3/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/notification.py` & `twikit-1.4.3/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/trend.py` & `twikit-1.4.3/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/tweet.py` & `twikit-1.4.3/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/__init__.py` & `twikit-1.4.3/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/client.py` & `twikit-1.4.3/twikit/twikit_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import Poll, ScheduledTweet, Tweet
 from .user import User
-from .utils import Result
+from .utils import Flow, Result
 
 
 class Client:
     """
     A client for interacting with the Twitter API.
     Since this class is for asynchronous use,
     methods must be executed using await.
@@ -59,14 +59,15 @@
 
     def __init__(self, language: str | None = None, **kwargs) -> None:
         self._token = TOKEN
         self.language = language
         self.http = HTTPClient(**kwargs)
         self._user_id = None
         self._user_agent = UserAgent().random.strip()
+        self._act_as = None
 
     async def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
         response = (await self.http.post(
             Endpoint.GUEST_TOKEN,
@@ -93,14 +94,16 @@
         if self.language is not None:
             headers['Accept-Language'] = self.language
             headers['X-Twitter-Client-Language'] = self.language
 
         csrf_token = self._get_csrf_token()
         if csrf_token is not None:
             headers['X-Csrf-Token'] = csrf_token
+        if self._act_as is not None:
+            headers['X-Act-As-User-Id'] = self._act_as
         return headers
 
     def _get_csrf_token(self) -> str:
         """
         Retrieves the Cross-Site Request Forgery (CSRF) token from the
         current session's cookies.
 
@@ -149,128 +152,85 @@
         guest_token = await self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
-        async def _execute_task(
-            flow_token: str | None = None,
-            subtask_input: dict | None = None,
-            flow_name: str | None = None
-        ) -> dict:
-            url = Endpoint.TASK
-            if flow_name is not None:
-                url += f'?flow_name={flow_name}'
-
-            data = {}
-            if flow_token is not None:
-                data['flow_token'] = flow_token
-            if subtask_input is not None:
-                data['subtask_inputs'] = [subtask_input]
-
-            response = (await self.http.post(
-                url, data=json.dumps(data), headers=headers
-            )).json()
-            return response
-
-        flow_token = (await _execute_task(flow_name='login'))['flow_token']
-        flow_token = (await _execute_task(flow_token))['flow_token']
-        response = await _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'LoginEnterUserIdentifierSSO',
-                'settings_list': {
-                    'setting_responses': [
-                        {
-                            'key': 'user_identifier',
-                            'response_data': {
-                                'text_data': {'result': auth_info_1}
-                            }
-                        }
-                    ],
-                    'link': 'next_link'
-                }
-            }
-        )
-
-        flow_token = response['flow_token']
-        task_id = response['subtasks'][0]['subtask_id']
+        flow = Flow(self, Endpoint.LOGIN_FLOW, headers)
 
-        if task_id == 'LoginEnterAlternateIdentifierSubtask':
-            response = await _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginEnterAlternateIdentifierSubtask',
-                    'enter_text': {
-                        'text': auth_info_2,
-                        'link': 'next_link'
+        await flow.execute_task(params={'flow_name': 'login'})
+        await flow.execute_task()
+        await flow.execute_task({
+            'subtask_id': 'LoginEnterUserIdentifierSSO',
+            'settings_list': {
+                'setting_responses': [
+                    {
+                        'key': 'user_identifier',
+                        'response_data': {
+                            'text_data': {'result': auth_info_1}
+                        }
                     }
-                }
-            )
-            flow_token = response['flow_token']
+                ],
+                'link': 'next_link'
+            }
+        })
 
-        response = await _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'LoginEnterPassword',
-                'enter_password': {
-                    'password': password,
+        if flow.task_id == 'LoginEnterAlternateIdentifierSubtask':
+            await flow.execute_task({
+                'subtask_id': 'LoginEnterAlternateIdentifierSubtask',
+                'enter_text': {
+                    'text': auth_info_2,
                     'link': 'next_link'
                 }
-            }
-        )
+            })
 
-        flow_token = response['flow_token']
+        await flow.execute_task({
+            'subtask_id': 'LoginEnterPassword',
+            'enter_password': {
+                'password': password,
+                'link': 'next_link'
+            }
+        })
 
-        response = await _execute_task(
-            flow_token,
-            {
-                'subtask_id': 'AccountDuplicationCheck',
-                'check_logged_in_account': {
-                    'link': 'AccountDuplicationCheck_false'
-                }
-            },
-        )
+        await flow.execute_task({
+            'subtask_id': 'AccountDuplicationCheck',
+            'check_logged_in_account': {
+                'link': 'AccountDuplicationCheck_false'
+            }
+        })
 
-        if not response['subtasks']:
+        if not flow.response['subtasks']:
             return
 
-        flow_token = response['flow_token']
-        task_id = response['subtasks'][0]['subtask_id']
-        self._user_id = find_dict(response, 'id_str')[0]
-
-        if task_id == 'LoginTwoFactorAuthChallenge':
-            print(find_dict(response, 'secondary_text')[0]['text'])
-            response = await _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginTwoFactorAuthChallenge',
-                    'enter_text': {
-                        'text': input('>>> '),
-                        'link': 'next_link'
-                    }
+        self._user_id = find_dict(flow.response, 'id_str')[0]
+
+        if flow.task_id == 'LoginTwoFactorAuthChallenge':
+            print(find_dict(flow.response, 'secondary_text')[0]['text'])
+
+            await flow.execute_task({
+                'subtask_id': 'LoginTwoFactorAuthChallenge',
+                'enter_text': {
+                    'text': input('>>> '),
+                    'link': 'next_link'
                 }
-            )
-            task_id = response['subtasks'][0]['subtask_id']
+            })
 
-        if task_id == 'LoginAcid':
-            print(find_dict(response, 'secondary_text')[0]['text'])
-            response = await _execute_task(
-                flow_token,
-                {
-                    'subtask_id': 'LoginAcid',
-                    'enter_text': {
-                        'text': input('>>> '),
-                        'link': 'next_link'
-                    }
+        if flow.task_id == 'LoginAcid':
+            print(find_dict(flow.response, 'secondary_text')[0]['text'])
+
+            await flow.execute_task({
+                'subtask_id': 'LoginAcid',
+                'enter_text': {
+                    'text': input('>>> '),
+                    'link': 'next_link'
                 }
-            )
+            })
 
-        return response
+        return flow.response
 
     async def logout(self) -> Response:
         """
         Logs out of the currently logged-in account.
         """
         response = await self.http.post(
             Endpoint.LOGOUT,
@@ -384,14 +344,26 @@
         .get_cookies
         .save_cookies
         .set_cookies
         """
         with open(path, 'r', encoding='utf-8') as f:
             self.set_cookies(json.load(f))
 
+    def set_delegate_account(self, user_id: str | None) -> None:
+        """
+        Sets the account to act as.
+
+        Parameters
+        ----------
+        user_id : str | None
+            The user ID of the account to act as.
+            Set to None to clear the delegated account.
+        """
+        self._act_as = user_id
+
     async def _search(
         self,
         query: str,
         product: str,
         count: int,
         cursor: str | None
     ) -> dict:
```

### Comparing `twikit-1.4.2/twikit/twikit_async/errors.py` & `twikit-1.4.3/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/group.py` & `twikit-1.4.3/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/http.py` & `twikit-1.4.3/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/list.py` & `twikit-1.4.3/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/message.py` & `twikit-1.4.3/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/notification.py` & `twikit-1.4.3/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/trend.py` & `twikit-1.4.3/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/tweet.py` & `twikit-1.4.3/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/user.py` & `twikit-1.4.3/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/twikit_async/utils.py` & `twikit-1.4.3/twikit/twikit_async/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from __future__ import annotations
 
-from typing import Awaitable, Generic, Iterator, TypeVar
+import json
+from typing import TYPE_CHECKING, Awaitable, Generic, Iterator, TypeVar
+
+if TYPE_CHECKING:
+    from .client import Client
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
@@ -73,7 +77,43 @@
         return self.__results[index]
 
     def __len__(self) -> int:
         return len(self.__results)
 
     def __repr__(self) -> str:
         return self.__results.__repr__()
+
+
+class Flow:
+    def __init__(self, client: Client, endpoint: str, headers: dict) -> None:
+        self._client = client
+        self.endpoint = endpoint
+        self.headers = headers
+        self.response = None
+
+    async def execute_task(self, *subtask_inputs, **kwargs) -> None:
+        data = {}
+
+        if self.token is not None:
+            data['flow_token'] = self.token
+        if subtask_inputs is not None:
+            data['subtask_inputs'] = list(subtask_inputs)
+
+        response = (await self._client.http.post(
+            self.endpoint,
+            data=json.dumps(data),
+            headers=self.headers,
+            **kwargs
+        )).json()
+        self.response = response
+
+    @property
+    def token(self) -> str | None:
+        if self.response is None:
+            return None
+        return self.response.get('flow_token')
+
+    @property
+    def task_id(self) -> str | None:
+        if self.response is None:
+            return None
+        return self.response['subtasks'][0]['subtask_id']
```

### Comparing `twikit-1.4.2/twikit/user.py` & `twikit-1.4.3/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.2/twikit/utils.py` & `twikit-1.4.3/twikit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
+import json
 from datetime import datetime
 from typing import (
     Any,
+    TYPE_CHECKING,
     Callable,
     Generic,
     Iterator,
     Literal,
     TypedDict,
     TypeVar
 )
 from urllib import parse
 
+if TYPE_CHECKING:
+    from .client import Client
+
 # This token is common to all accounts and does not need to be changed.
 TOKEN = 'AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA'
 
 FEATURES = {
     'creator_subscriptions_tweet_preview_api_enabled': True,
     'c9s_tweet_anatomy_moderator_badge_enabled': True,
     'tweetypie_unmention_optimization_enabled': True,
@@ -61,15 +66,15 @@
 }
 
 
 class Endpoint:
     """
     A class containing Twitter API endpoints.
     """
-    TASK = 'https://api.twitter.com/1.1/onboarding/task.json'
+    LOGIN_FLOW = 'https://api.twitter.com/1.1/onboarding/task.json'
     LOGOUT = 'https://api.twitter.com/1.1/account/logout.json'
     CREATE_TWEET = 'https://twitter.com/i/api/graphql/SiM_cAu83R0wnrpmKQQSEw/CreateTweet'
     DELETE_TWEET = 'https://twitter.com/i/api/graphql/VaenaVgh5q5ih7kvyVjgtg/DeleteTweet'
     SEARCH_TIMELINE = 'https://twitter.com/i/api/graphql/flaR-PUMshxFWZWPNpq4zA/SearchTimeline'
     UPLOAD_MEDIA = 'https://upload.twitter.com/i/media/upload.json'
     GUEST_TOKEN = 'https://api.twitter.com/1.1/guest/activate.json'
     CREATE_CARD = 'https://caps.twitter.com/v2/cards/create.json'
@@ -129,14 +134,15 @@
     DELETE_SCHEDULED_TWEET = 'https://twitter.com/i/api/graphql/CTOVqej0JBXAZSwkp1US0g/DeleteScheduledTweet'
     SETTINGS = 'https://api.twitter.com/1.1/account/settings.json'
     LIST_MANAGEMENT = 'https://twitter.com/i/api/graphql/47170qwZCt5aFo9cBwFoNA/ListsManagementPageTimeline'
     NOTIFICATIONS_ALL = 'https://twitter.com/i/api/2/notifications/all.json'
     NOTIFICATIONS_VERIFIED = 'https://twitter.com/i/api/2/notifications/verified.json'
     NOTIFICATIONS_MENTIONES = 'https://twitter.com/i/api/2/notifications/mentions.json'
     VOTE = 'https://caps.twitter.com/v2/capi/passthrough/1'
+    REPORT_FLOW = 'https://twitter.com/i/api/1.1/report/flow.json'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
@@ -207,14 +213,50 @@
     def __len__(self) -> int:
         return len(self.__results)
 
     def __repr__(self) -> str:
         return self.__results.__repr__()
 
 
+class Flow:
+    def __init__(self, client: Client, endpoint: str, headers: dict) -> None:
+        self._client = client
+        self.endpoint = endpoint
+        self.headers = headers
+        self.response = None
+
+    def execute_task(self, *subtask_inputs, **kwargs) -> None:
+        data = {}
+
+        if self.token is not None:
+            data['flow_token'] = self.token
+        if subtask_inputs is not None:
+            data['subtask_inputs'] = list(subtask_inputs)
+
+        response = self._client.http.post(
+            self.endpoint,
+            data=json.dumps(data),
+            headers=self.headers,
+            **kwargs
+        ).json()
+        self.response = response
+
+    @property
+    def token(self) -> str | None:
+        if self.response is None:
+            return None
+        return self.response.get('flow_token')
+
+    @property
+    def task_id(self) -> str | None:
+        if self.response is None:
+            return None
+        return self.response['subtasks'][0]['subtask_id']
+
+
 def find_dict(obj: list | dict, key: str | int) -> list[Any]:
     """
     Retrieves elements from a nested dictionary.
     """
     results = []
     if isinstance(obj, dict):
         if key in obj:
```

### Comparing `twikit-1.4.2/twikit.egg-info/PKG-INFO` & `twikit-1.4.3/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.2/twikit.egg-info/SOURCES.txt` & `twikit-1.4.3/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

