# Comparing `tmp/github-app-handler-0.9.tar.gz` & `tmp/github-app-handler-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-app-handler-0.9.tar", last modified: Fri Jan  5 16:24:19 2024, max compression
+gzip compressed data, was "github-app-handler-0.9.1.tar", last modified: Fri Jan  5 17:36:06 2024, max compression
```

## Comparing `github-app-handler-0.9.tar` & `github-app-handler-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:24:19.646931 github-app-handler-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-05 16:24:09.000000 github-app-handler-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-01-05 16:24:19.642931 github-app-handler-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-05 16:24:09.000000 github-app-handler-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:24:19.642931 github-app-handler-0.9/github_app_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-01-05 16:24:19.000000 github-app-handler-0.9/github_app_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-05 16:24:19.000000 github-app-handler-0.9/github_app_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 16:24:19.000000 github-app-handler-0.9/github_app_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 16:24:19.000000 github-app-handler-0.9/github_app_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-05 16:24:19.000000 github-app-handler-0.9/github_app_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:24:19.642931 github-app-handler-0.9/githubapp/
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/LazyCompletableGithubObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:24:19.642931 github-app-handler-0.9/githubapp/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/check_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/check_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/issue_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/pull_request_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/events/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-01-05 16:24:09.000000 github-app-handler-0.9/githubapp/webhook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-05 16:24:09.000000 github-app-handler-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 16:24:09.000000 github-app-handler-0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 16:24:19.646931 github-app-handler-0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 16:24:19.642931 github-app-handler-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-01-05 16:24:09.000000 github-app-handler-0.9/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-05 16:24:09.000000 github-app-handler-0.9/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-01-05 16:24:09.000000 github-app-handler-0.9/tests/test_lazy_completable_gituhb_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-05 16:24:09.000000 github-app-handler-0.9/tests/test_webhook_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:36:06.184132 github-app-handler-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-05 17:36:06.180132 github-app-handler-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:36:06.180132 github-app-handler-0.9.1/github_app_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-01-05 17:36:06.000000 github-app-handler-0.9.1/github_app_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-01-05 17:36:06.000000 github-app-handler-0.9.1/github_app_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 17:36:06.000000 github-app-handler-0.9.1/github_app_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 17:36:06.000000 github-app-handler-0.9.1/github_app_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-05 17:36:06.000000 github-app-handler-0.9.1/github_app_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:36:06.180132 github-app-handler-0.9.1/githubapp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/LazyCompletableGithubObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:36:06.180132 github-app-handler-0.9.1/githubapp/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/check_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/check_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/issue_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/pull_request_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/events/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/githubapp/webhook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 17:36:06.184132 github-app-handler-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:36:06.180132 github-app-handler-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/tests/test_lazy_completable_gituhb_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-05 17:35:52.000000 github-app-handler-0.9.1/tests/test_webhook_handler.py
```

### Comparing `github-app-handler-0.9/LICENSE` & `github-app-handler-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/PKG-INFO` & `github-app-handler-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-app-handler
-Version: 0.9
+Version: 0.9.1
 Summary: Package to help creates Github Apps.
 Author: Heitor Luis Polidoro
 License: MIT
 Project-URL: Homepage, https://github.com/heitorpolidoro/github-app-handler
 Keywords: github,app,githubapp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `github-app-handler-0.9/README.md` & `github-app-handler-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/github_app_handler.egg-info/PKG-INFO` & `github-app-handler-0.9.1/github_app_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-app-handler
-Version: 0.9
+Version: 0.9.1
 Summary: Package to help creates Github Apps.
 Author: Heitor Luis Polidoro
 License: MIT
 Project-URL: Homepage, https://github.com/heitorpolidoro/github-app-handler
 Keywords: github,app,githubapp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `github-app-handler-0.9/github_app_handler.egg-info/SOURCES.txt` & `github-app-handler-0.9.1/github_app_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/LazyCompletableGithubObject.py` & `github-app-handler-0.9.1/githubapp/LazyCompletableGithubObject.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Example:
 
     lazy_obj = LazyCompletableGithubObject.get_lazy_instance(Repo, id=123)
     print(lazy_obj.name) # Makes API request here to get name
 """
 import os
-from typing import Any, TypeVar, Union
+from typing import Any, Optional, TypeVar, Union
 
 from github import Consts, GithubIntegration, GithubRetry
 from github.Auth import AppAuth, AppUserAuth, Token
 from github.GithubObject import CompletableGithubObject
 from github.Requester import Requester
 
 from githubapp.events.event import Event
@@ -100,28 +100,34 @@
     def __init__(
         self,
         requester: "Requester" = None,
         headers: dict[str, Union[str, int]] = None,
         attributes: dict[str, Any] = None,
         completed: bool = False,
     ) -> None:
-        # if attributes.get("url", "").startswith("https://github"):
-        #     attributes["url"] = attributes["url"].replace("https://github.com", "https://api.github.com/repos")
+        if attributes.get("url", "").startswith("https://github"):
+            attributes["url"] = attributes["url"].replace(
+                "https://github.com", "https://api.github.com/repos"
+            )
         #     attributes["url"] = attributes["url"].replace("/commit/", "/commits/")
         # if isinstance(self, GitCommit):
         #     attributes["sha"] = attributes["id"]
         # noinspection PyTypeChecker
         CompletableGithubObject.__init__(
             self,
             requester=requester,
             headers=headers or {},
             attributes=attributes,
             completed=completed,
         )
         self._requester = LazyRequester()
 
     @staticmethod
-    def get_lazy_instance(clazz: type[T], attributes: dict[str, Any]) -> T:
+    def get_lazy_instance(
+        clazz: type[T], attributes: Optional[dict[str, Any]]
+    ) -> Optional[T]:
         """Makes the clazz a subclass of LazyCompletableGithubObject"""
+        if attributes is None:
+            return None
         return type(clazz.__name__, (LazyCompletableGithubObject, clazz), {})(
             attributes=attributes
         )
```

### Comparing `github-app-handler-0.9/githubapp/events/__init__.py` & `github-app-handler-0.9.1/githubapp/events/__init__.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/check_run.py` & `github-app-handler-0.9.1/githubapp/events/check_run.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/check_suite.py` & `github-app-handler-0.9.1/githubapp/events/check_suite.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/create.py` & `github-app-handler-0.9.1/githubapp/events/create.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/event.py` & `github-app-handler-0.9.1/githubapp/events/event.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/issue_comment.py` & `github-app-handler-0.9.1/githubapp/events/issue_comment.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/issues.py` & `github-app-handler-0.9.1/githubapp/events/issues.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/pull_request_review.py` & `github-app-handler-0.9.1/githubapp/events/pull_request_review.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/push.py` & `github-app-handler-0.9.1/githubapp/events/push.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/release.py` & `github-app-handler-0.9.1/githubapp/events/release.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/events/status.py` & `github-app-handler-0.9.1/githubapp/events/status.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/githubapp/webhook_handler.py` & `github-app-handler-0.9.1/githubapp/webhook_handler.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/pyproject.toml` & `github-app-handler-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/tests/test_event.py` & `github-app-handler-0.9.1/tests/test_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     "head_commit": {"id": 123},
     "pusher": {},
     "changes": {
         "old_issue": {},
         "old_repository": {},
     },
     "commits": [{"id": 123}],
+    "check_run": {},
+    "check_suite": {},
+    "pull_request": {},
+    "review": {},
 }
 LISTS = [
     "branches",
 ]
 
 
 def fill_body(body, *attributes):
```

### Comparing `github-app-handler-0.9/tests/test_handler.py` & `github-app-handler-0.9.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `github-app-handler-0.9/tests/test_lazy_completable_gituhb_objects.py` & `github-app-handler-0.9.1/tests/test_lazy_completable_gituhb_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,45 @@
     def _initAttributes(self) -> None:
         self._attr1: Attribute[str] = NotSet
         self._url: Attribute[str] = NotSet
 
     def _useAttributes(self, attributes: dict[str, Any]) -> None:
         if "attr1" in attributes:  # pragma no branch
             self._attr1 = self._makeStringAttribute(attributes["attr1"])
-        self._url = self._makeStringAttribute("url")
+        self._url = self._makeStringAttribute(attributes.get("url", "url"))
 
     @property
     def attr1(self) -> Union[str, None]:
         self._completeIfNotSet(self._attr1)
         return self._attr1.value
 
+    @property
+    def url(self) -> Union[str, None]:
+        return self._url.value
+
 
 def test_lazy():
     instance = LazyCompletableGithubObject.get_lazy_instance(LazyClass, attributes={})
     assert isinstance(instance, LazyClass)
 
 
+def test_lazy_null_attributes():
+    assert (
+        LazyCompletableGithubObject.get_lazy_instance(LazyClass, attributes=None)
+        is None
+    )
+
+
+def test_lazy_fix_url():
+    instance = LazyCompletableGithubObject.get_lazy_instance(
+        LazyClass, attributes={"url": "https://github.com/potato"}
+    )
+    assert instance.url == "https://api.github.com/repos/potato"
+
+
 def test_lazy_requester_private_key():
     with (
         mock.patch("githubapp.LazyCompletableGithubObject.GithubIntegration"),
         mock.patch("githubapp.LazyCompletableGithubObject.AppAuth") as app_auth,
         mock.patch("githubapp.LazyCompletableGithubObject.Token"),
         mock.patch(
             "githubapp.LazyCompletableGithubObject.Requester._Requester__check",
```

### Comparing `github-app-handler-0.9/tests/test_webhook_handler.py` & `github-app-handler-0.9.1/tests/test_webhook_handler.py`

 * *Files identical despite different names*

