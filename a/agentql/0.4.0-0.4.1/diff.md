# Comparing `tmp/agentql-0.4.0.tar.gz` & `tmp/agentql-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.4.0.tar", max compression
+gzip compressed data, was "agentql-0.4.1.tar", max compression
```

## Comparing `agentql-0.4.0.tar` & `agentql-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2024-04-04 00:16:44.754820 agentql-0.4.0/LICENSE
--rw-r--r--   0        0        0      111 2024-04-04 00:16:44.754820 agentql-0.4.0/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-04-04 00:16:44.842820 agentql-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/__init__.py
--rw-r--r--   0        0        0       78 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_api_constants.py
--rw-r--r--   0        0        0     4741 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_errors.py
--rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     5986 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/character_utils.py
--rw-r--r--   0        0        0     4997 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/node.py
--rw-r--r--   0        0        0     4686 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/source.py
--rw-r--r--   0        0        0     1602 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/token.py
--rw-r--r--   0        0        0      213 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_syntax/token_kind.py
--rw-r--r--   0        0        0      468 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_typing.py
--rw-r--r--   0        0        0      204 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/_core/_utils.py
--rw-r--r--   0        0        0      363 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     1853 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_api.py
--rw-r--r--   0        0        0     1605 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_popup.py
--rw-r--r--   0        0        0     5460 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_response_proxy.py
--rw-r--r--   0        0        0    10787 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_session.py
--rw-r--r--   0        0        0     5331 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/async_api/_web_driver.py
--rw-r--r--   0        0        0        0 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/__init__.py
--rw-r--r--   0        0        0      168 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/__init__.py
--rw-r--r--   0        0        0      193 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_driver_constants.py
--rw-r--r--   0        0        0      290 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_driver_settings.py
--rw-r--r--   0        0        0     1980 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_html_constants.py
--rw-r--r--   0        0        0     3813 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/_network_monitor.py
--rw-r--r--   0        0        0    26759 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_async.py
--rw-r--r--   0        0        0    26608 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_sync.py
--rw-r--r--   0        0        0      363 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     1813 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_api.py
--rw-r--r--   0        0        0     1525 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_popup.py
--rw-r--r--   0        0        0     4917 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_response_proxy.py
--rw-r--r--   0        0        0    10540 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_session.py
--rw-r--r--   0        0        0     4770 2024-04-04 00:16:44.842820 agentql-0.4.0/src/agentql/sync_api/_web_driver.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-05 17:21:47.290799 agentql-0.4.1/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-05 17:21:47.290799 agentql-0.4.1/PACKAGE_README.md
+-rw-r--r--   0        0        0      771 2024-04-05 17:21:47.378800 agentql-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     4741 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     5986 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      145 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     4997 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     2431 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     4686 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      213 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      535 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0      204 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     2574 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     1605 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     5460 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0    10787 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     5331 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      290 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     3813 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    26759 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    26608 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     2528 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1525 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     4917 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0    10540 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     4770 2024-04-05 17:21:47.378800 agentql-0.4.1/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.1/PKG-INFO
```

### Comparing `agentql-0.4.0/LICENSE` & `agentql-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/pyproject.toml` & `agentql-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.4.0"
+version = "0.4.1"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.4.0/src/agentql/__init__.py` & `agentql-0.4.1/src/agentql/__init__.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_errors.py` & `agentql-0.4.1/src/agentql/_core/_errors.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_js_snippets/generate_accessibility_tree.js` & `agentql-0.4.1/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_js_snippets/set_iframe_path.js` & `agentql-0.4.1/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/character_utils.py` & `agentql-0.4.1/src/agentql/_core/_syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/lexer.py` & `agentql-0.4.1/src/agentql/_core/_syntax/lexer.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/node.py` & `agentql-0.4.1/src/agentql/_core/_syntax/node.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/parser.py` & `agentql-0.4.1/src/agentql/_core/_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/source.py` & `agentql-0.4.1/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/_core/_syntax/token.py` & `agentql-0.4.1/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/async_api/_api.py` & `agentql-0.4.1/src/agentql/async_api/_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
 This module is an entrypoint to AgentQL service
 """
 
 import logging
 from typing import Any
 
+from playwright.async_api import Locator, Page
+
 from agentql.ext.playwright import PlaywrightWebDriverAsync as PlaywrightWebDriver
 
 from ._session import Session
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger(__name__)
 
 
+class PlaywrightDriverTypeStub(WebDriver[Locator, Page]):
+    pass
+
+
 async def start_async_session(
     url: str = "",
     *,
-    web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightWebDriver(),
+    web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightDriverTypeStub(),
     user_auth_session: Any = None,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
     """Start a new asynchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
@@ -29,12 +35,24 @@
 
     Returns:
     -------
     Session: An instance of AgentQL Session class for asynchronous environment.
     """
     log.debug(f"Starting asynchronous session with {url}")
 
-    await web_driver.start_browser(user_auth_session=user_auth_session)
-    if url:
-        await web_driver.open_url(url)
-    session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
+    # this is a dirty hack to avoid instantiating PlaywrightWebDriver as a default value
+    # which will be cached and reused across all sessions. This may cause problems when
+    # start_session is called multiple times with default params. In this case driver will
+    # be reused which is a problem since its stateful.
+    if isinstance(web_driver, PlaywrightDriverTypeStub):
+        web_driver = PlaywrightWebDriver()  # type: ignore
+
+    try:
+        await web_driver.start_browser(user_auth_session=user_auth_session)
+        if url:
+            await web_driver.open_url(url)
+        session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
+    except Exception as e:
+        log.error(f"Failed to start session: {e}")
+        await web_driver.stop_browser()
+        raise e
     return session
```

### Comparing `agentql-0.4.0/src/agentql/async_api/_popup.py` & `agentql-0.4.1/src/agentql/async_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/async_api/_response_proxy.py` & `agentql-0.4.1/src/agentql/async_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/async_api/_session.py` & `agentql-0.4.1/src/agentql/async_api/_session.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/async_api/_web_driver.py` & `agentql-0.4.1/src/agentql/async_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/ext/playwright/_html_constants.py` & `agentql-0.4.1/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/ext/playwright/_network_monitor.py` & `agentql-0.4.1/src/agentql/ext/playwright/_network_monitor.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_async.py` & `agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/ext/playwright/playwright_driver_sync.py` & `agentql-0.4.1/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/sync_api/_api.py` & `agentql-0.4.1/src/agentql/sync_api/_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
 This module is an entrypoint to AgentQL service
 """
 
 import logging
 from typing import Any
 
+from playwright.sync_api import Locator, Page
+
 from agentql.ext.playwright import PlaywrightWebDriverSync as PlaywrightWebDriver
 
 from ._session import Session
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("agentql")
+
+
+class PlaywrightDriverTypeStub(WebDriver[Locator, Page]):
+    pass
 
 
 def start_session(
     url: str = "",
     *,
-    web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightWebDriver(),
+    web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightDriverTypeStub(),
     user_auth_session: Any = None,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
     """Start a new synchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
     ----------
     url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
@@ -29,12 +35,24 @@
 
     Returns:
     -------
     Session: An instance of AgentQL Session class for synchronous environment.
     """
     log.debug(f"Starting session with {url}")
 
-    web_driver.start_browser(user_auth_session=user_auth_session)
-    if url:
-        web_driver.open_url(url)
-    session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
+    # this is a dirty hack to avoid instantiating PlaywrightWebDriver as a default value
+    # which will be cached and reused across all sessions. This may cause problems when
+    # start_session is called multiple times with default params. In this case driver will
+    # be reused which is a problem since its stateful.
+    if isinstance(web_driver, PlaywrightDriverTypeStub):
+        web_driver = PlaywrightWebDriver()  # type: ignore
+
+    try:
+        web_driver.start_browser(user_auth_session=user_auth_session)
+        if url:
+            web_driver.open_url(url)
+        session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
+    except Exception as e:
+        log.error(f"Failed to start session: {e}")
+        web_driver.stop_browser()
+        raise e
     return session
```

### Comparing `agentql-0.4.0/src/agentql/sync_api/_popup.py` & `agentql-0.4.1/src/agentql/sync_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/sync_api/_response_proxy.py` & `agentql-0.4.1/src/agentql/sync_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/sync_api/_session.py` & `agentql-0.4.1/src/agentql/sync_api/_session.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/src/agentql/sync_api/_web_driver.py` & `agentql-0.4.1/src/agentql/sync_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.0/PKG-INFO` & `agentql-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

