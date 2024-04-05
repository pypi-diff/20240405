# Comparing `tmp/t_bug_catcher-0.3.1.tar.gz` & `tmp/t_bug_catcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-vorsusec/t_bug_catcher-0.3.1.tar", last modified: Wed Apr  3 09:17:17 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-wp4cs3e9/t_bug_catcher-0.4.0.tar", last modified: Fri Apr  5 10:38:50 2024, max compression
```

## Comparing `t_bug_catcher-0.3.1.tar` & `t_bug_catcher-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-03 09:17:17.311958 t_bug_catcher-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10474 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    44239 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.213371 t_bug_catcher-0.4.0/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44721 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/jira.py
+-rw-rw-rw-   0 root         (0) root         (0)     5760 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-05 10:38:50.000000 t_bug_catcher-0.4.0/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 10:38:50.217371 t_bug_catcher-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-05 10:38:22.000000 t_bug_catcher-0.4.0/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.3.1/PKG-INFO` & `t_bug_catcher-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.3.1
+Version: 0.4.0
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: bugsnag>=4.6.1
 Requires-Dist: retry~=0.9.2
+Requires-Dist: whispers>=2.2.1
 
 t-bug-catcher
 ==============
 
 Description
 -----------
 The `t-bug-catcher` package is a bug reporting tool that allows users to easily submit bug reports for the application.
```

### Comparing `t_bug_catcher-0.3.1/README.rst` & `t_bug_catcher-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.1/setup.py` & `t_bug_catcher-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.3.1",
+    version="0.4.0",
     zip_safe=False,
     install_requires=install_requirements,
 )
```

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.0/t_bug_catcher/bug_catcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 from types import TracebackType
 from typing import List, Optional
 
 from .bug_snag import BugSnag
 from .config import CONFIG
 from .jira import Jira
+from .stack_saver import StackSaver
 from .utils import logger
 from .utils.common import get_frames
 
 
 class Configurator:
     """Configurer class for configuring the JiraPoster and BugSnag."""
 
@@ -85,14 +86,15 @@
 
     def __init__(self):
         """Initializes the BugCatcher class."""
         self.__jira: Jira = Jira()
         self.__bug_snag: BugSnag = BugSnag()
         self.__configurator: Configurator = Configurator(self.__jira, self.__bug_snag)
         self.__sys_excepthook = None
+        self.__stack_saver = StackSaver()
 
     @property
     def configure(self):
         """Configures the JiraPoster and BugSnag classes."""
         return self.__configurator
 
     def report_error(
@@ -127,19 +129,22 @@
             _, exception, _ = sys.exc_info()
 
         handled_error = getattr(exception, "handled_error", None)
         if handled_error:
             logger.warning(f"Exception {handled_error} already reported.")
             return
 
+        stack_trace = self.__stack_saver.save_stack_trace(exception)
+
         if self.__configurator.is_jira_configured:
             self.__jira.report_error(
                 exception=exception,
                 assignee=assignee,
                 attachments=attachments,
+                stack_trace=stack_trace,
                 additional_info=description,
                 metadata=metadata,
             )
 
         if self.__configurator.is_bugsnag_configured:
             self.__bug_snag.report_error(
                 exception=exception,
@@ -239,16 +244,18 @@
             return
 
         handled_error = getattr(exc_value, "handled_error", None)
         if handled_error:
             logger.warning(f"Exception {handled_error} already reported.")
             return
 
+        stack_trace = self.__stack_saver.save_stack_trace(exc_value)
+
         if self.__configurator.is_jira_configured:
-            self.__jira.report_unhandled_error(exc_type, exc_value, exc_traceback)
+            self.__jira.report_unhandled_error(exc_type, exc_value, exc_traceback, stack_trace)
         if self.__configurator.is_bugsnag_configured:
             self.__bug_snag.report_unhandled_error(exc_type, exc_value, exc_traceback)
 
     def __get_sys_hook_attribute(self, attribute: str = "bug_catcher_client"):
         """Checks if the system hook is installed.
 
         Args:
```

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.0/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher/config.py` & `t_bug_catcher-0.4.0/t_bug_catcher/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     SUPPORT_BOARD = "AB"
 
     RC_RUN_LINK = (
         f"https://cloud.robocorp.com/organizations/{os.environ.get('RC_ORGANIZATION_ID')}"
         f"/workspaces/{os.environ.get('RC_WORKSPACE_ID')}/processes"
         f"/{os.environ.get('RC_PROCESS_ID')}/runs/{os.environ.get('RC_PROCESS_RUN_ID')}/"
+        f"stepRuns/{os.environ.get('RC_ACTIVITY_RUN_ID')}/"
     )
 
     ENVIRONMENT = (
         "robocloud"
         if not variables.get("environment") and os.environ.get("RC_PROCESS_RUN_ID")
         else variables.get("environment", "local")
     )
```

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.0/t_bug_catcher/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -955,23 +955,25 @@
         return response
 
     def report_error(
         self,
         exception: Optional[Exception] = None,
         assignee: Optional[str] = None,
         attachments: Union[List, str, Path, None] = None,
+        stack_trace: Optional[str] = None,
         metadata: Optional[dict] = None,
         additional_info: Optional[str] = None,
     ) -> dict:
         """Create a Jira issue with the given attachments.
 
         Args:
             exception (Exception, optional): The exception to be added to the Jira issue.
             assignee (str, optional): The assignee to be added to the Jira issue.
             attachments (List, optional): List of attachments to be added to the Jira issue.
+            stack_trace (str, optional): Stack trace to be added to the Jira issue.
             metadata (dict, optional): Metadata to be added to the Jira issue.
             additional_info (str, optional): Additional information to be added to the Jira issue.
 
         Returns:
             The response from creating the Jira issue.
         """
         try:
@@ -1008,14 +1010,17 @@
                     attachments=attachments,
                     summary=summary,
                     additional_info=additional_info,
                     metadata=metadata,
                 )
                 return existing_ticket
 
+            if stack_trace:
+                attachments.insert(0, stack_trace)
+
             assignee_id = None
             assignee = assignee if assignee else self._default_assignee
             if assignee:
                 try:
                     assignee_id = self.__get_assignee(assignee)
                 except Exception as ex:
                     logger.info(f"Failed to get assignee {assignee} due to: {ex}")
@@ -1032,27 +1037,31 @@
             response = self.__create_new_ticket(
                 summary=summary,
                 description=description,
                 assignee_id=assignee_id,
                 attachments=attachments,
                 labels=["bug_catcher"],
             )
+            if os.path.exists(stack_trace):
+                os.remove(stack_trace)
             return response
         except Exception as ex:
             logger.warning(f"Failed to create Jira issue due to: {ex.__class__.__name__}: {ex}")
             return False
 
-    def report_unhandled_error(self, exc_type: type, exc_value: Union[Exception, str], exc_traceback: TracebackType):
+    def report_unhandled_error(
+        self, exc_type: type, exc_value: Union[Exception, str], exc_traceback: TracebackType, stack_trace: str = None
+    ):
         """Report an unhandled error to Jira.
 
         Args:
             exc_type (type): The type of the exception.
             exc_value (Exception, str): The value of the exception.
             exc_traceback (TracebackType): The traceback of the exception.
-            assignee (str, optional): The assignee to be added to the Jira issue.
+            stack_trace (str, optional): Stack trace to be added to the Jira issue.
 
         Returns:
             The response from creating the Jira issue.
         """
         try:
             summary = self.__create_summary(exc_type, exc_value, exc_traceback)
             error_id = self.__generate_error_id(exc_type=exc_type, exc_traceback=exc_traceback)
@@ -1082,16 +1091,19 @@
                 error_id=error_id,
             )
 
             response = self.__create_new_ticket(
                 summary=summary,
                 description=description,
                 assignee_id=assignee_id,
+                attachments=[stack_trace] if stack_trace else None,
                 labels=["bug_catcher", "fatal_error"],
             )
+            if os.path.exists(stack_trace):
+                os.remove(stack_trace)
             return response
         except Exception as ex:
             logger.warning(f"Failed to create Jira issue due to: {ex.__class__.__name__}: {ex}")
             return False
 
     @retry_if_bad_request
     def add_attachment(self, attachment: str, ticket_id: str) -> Optional[dict]:
```

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.0/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.0/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.3.1
+Version: 0.4.0
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: bugsnag>=4.6.1
 Requires-Dist: retry~=0.9.2
+Requires-Dist: whispers>=2.2.1
 
 t-bug-catcher
 ==============
 
 Description
 -----------
 The `t-bug-catcher` package is a bug reporting tool that allows users to easily submit bug reports for the application.
```

### Comparing `t_bug_catcher-0.3.1/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.0/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 t_bug_catcher/__init__.py
 t_bug_catcher/bug_catcher.py
 t_bug_catcher/bug_snag.py
 t_bug_catcher/config.py
 t_bug_catcher/exceptions.py
 t_bug_catcher/jira.py
+t_bug_catcher/stack_saver.py
 t_bug_catcher/workitems.py
 t_bug_catcher.egg-info/PKG-INFO
 t_bug_catcher.egg-info/SOURCES.txt
 t_bug_catcher.egg-info/dependency_links.txt
 t_bug_catcher.egg-info/not-zip-safe
 t_bug_catcher.egg-info/requires.txt
 t_bug_catcher.egg-info/top_level.txt
```

### Comparing `t_bug_catcher-0.3.1/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.0/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

