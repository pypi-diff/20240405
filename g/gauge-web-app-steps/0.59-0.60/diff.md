# Comparing `tmp/gauge-web-app-steps-0.59.tar.gz` & `tmp/gauge-web-app-steps-0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauge-web-app-steps-0.59.tar", last modified: Fri Dec  8 10:02:05 2023, max compression
+gzip compressed data, was "gauge-web-app-steps-0.60.tar", last modified: Fri Apr  5 13:45:12 2024, max compression
```

## Comparing `gauge-web-app-steps-0.59.tar` & `gauge-web-app-steps-0.60.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:02:05.516159 gauge-web-app-steps-0.59/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-12-08 10:02:05.516159 gauge-web-app-steps-0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:02:05.512158 gauge-web-app-steps-0.59/gauge_web_app_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/app_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/bymapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:02:05.512158 gauge-web-app-steps-0.59/gauge_web_app_steps/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/config/common_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/config/local_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/config/saucelabs_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:02:05.516159 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/browsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18989 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/driver/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/imagepaths.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/keymapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/sauce_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    49004 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/gauge_web_app_steps/web_app_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:02:05.512158 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-08 10:02:05.000000 gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 10:02:05.516159 gauge-web-app-steps-0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-08 10:01:56.000000 gauge-web-app-steps-0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.679677 gauge-web-app-steps-0.60/gauge_web_app_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/app_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/bymapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/gauge_web_app_steps/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/common_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/saucelabs_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/element_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/imagepaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/keymapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/sauce_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/web_app_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.679677 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/setup.py
```

### Comparing `gauge-web-app-steps-0.59/LICENCE` & `gauge-web-app-steps-0.60/LICENCE`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/PKG-INFO` & `gauge-web-app-steps-0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.59
+Version: 0.60
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -100,15 +100,15 @@
 
 Mathematical expressions can also be evaluated. For example: `#{5 + 5 * 5}` is evaluated to `30`.
 
 It is possible to combine the two features. Placeholder substitution takes place before mathematical expression evaluation.
 
 ### Functional Expressions
 
-Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted it will be use ISO format. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
+Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted ISO format will be used. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
 
 ### Expression Examples
 
 Note that the property expressions start with `$`, mathematical expressions with `#`, and functional expressions with `!`.
 
 > \* Open "\${homepage_url}/home"
```

### Comparing `gauge-web-app-steps-0.59/README.md` & `gauge-web-app-steps-0.60/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 Mathematical expressions can also be evaluated. For example: `#{5 + 5 * 5}` is evaluated to `30`.
 
 It is possible to combine the two features. Placeholder substitution takes place before mathematical expression evaluation.
 
 ### Functional Expressions
 
-Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted it will be use ISO format. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
+Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted ISO format will be used. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
 
 ### Expression Examples
 
 Note that the property expressions start with `$`, mathematical expressions with `#`, and functional expressions with `!`.
 
 > \* Open "\${homepage_url}/home"
```

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/app_context.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/app_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from .driver import Browser, DriverFactory
 from .imagepaths import ImagePath
 from .images import Images
 from .report import Report
 from .config import common_config as config
 from .config import local_config, saucelabs_config
 
+app_context_key = "_app_ctx"
+timeout_key = "_timeout"
 
 class AppContext:
     """
     Context objects are created and kept here.
     """
 
     def __init__(self, ctx: ExecutionContext = None) -> None:
```

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/bymapper.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/bymapper.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/config/common_config.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/config/common_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/config/local_config.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/config/local_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/config/saucelabs_config.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/config/saucelabs_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/driver/browsers.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/browsers.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/driver/driver_factory.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/driver_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,15 @@
             'browserName': browser.value,
             'appium:deviceName': saucelabs_config.get_device_name(),
             'appium:platformVersion': config.get_operating_system_version(),
             'sauce:options': self._get_sauce_options()
         }
         options = self._create_browser_options()
         if operating_system == OperatingSystem.ANDROID:
+            desired_capabilities['appium:automationName'] = 'UiAutomator2'
             desired_capabilities["goog:chromeOptions"] = {
                 'w3c': True,
                 'extensions': []
             }
         elif operating_system == OperatingSystem.IOS:
             desired_capabilities["appium:automationName"] = "XCUITest"
         capabilities_options = options.load_capabilities(desired_capabilities)
```

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/driver/operating_system.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/operating_system.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/imagepaths.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/imagepaths.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/images.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/images.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/report.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/report.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/sauce_tunnel.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/sauce_tunnel.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/selector.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/selector.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps/web_app_steps.py` & `gauge-web-app-steps-0.60/gauge_web_app_steps/web_app_steps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 #
 # Copyright IBM Corp. 2019-
 # SPDX-License-Identifier: MIT
 #
 
 import base64
-import numexpr
 import os
 import re
 import time
 import traceback
 import urllib
-import uuid
 
-from datetime import datetime
 from itertools import filterfalse
-from string import Template
-from typing import Any, Callable, Iterable, List, Tuple
+from typing import Tuple
 from getgauge.python import data_store, step, before_spec, after_spec, screenshot, before_suite, after_suite, before_step, ExecutionContext
-from numpy import array2string
-from selenium.common.exceptions import TimeoutException, JavascriptException, WebDriverException
+from selenium.common.exceptions import JavascriptException, WebDriverException
 from selenium.webdriver import Remote
 from selenium.webdriver.common.action_chains import ActionChains
-from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
-from .app_context import AppContext
-from .bymapper import ByMapper
+from .app_context import AppContext, app_context_key, timeout_key
 from .config import common_config as config
 from .driver.browsers import Browser
-from .imagepaths import ImagePath
-from .images import Images
+from .element_lookup import find_element, find_elements, find_attribute, get_text_from_element, get_marker, wait_until
 from .keymapper import KeyMapper
 from .report import Report
 from .sauce_tunnel import SauceTunnel
 from .selector import SelectKey, Selector
+from .screenshot import (append_structured_similarity, create_screenshot, create_failure_screenshot, 
+                        create_actual_screenshot_file_path, create_expected_screenshot_file_path, crop_image,
+                        get_structured_similarity_to_expected, ssim_screenshot_scrolling, ssim_screenshot_noscrolling)
+from .substitute import substitute
 
 
 # Repeat an action a number of times before failing
 max_attempts = 12
-error_message_key = "_err_msg"
-app_context_key = "_app_ctx"
 basic_auth_key = "_basic_auth"
-timeout_key = "_timeout"
-
+error_message_key = "_err_msg"
 
 @before_suite
 def before_suite_hook() -> None:
     SauceTunnel.start()
 
 
 @after_suite
@@ -103,38 +95,37 @@
     to the Error message as intended by the gauge framework (corrupt file format in base64).
     That is why the picture is saved and linked into the report with the Messages.write_message way.
     """
     if driver() is None:
         # Error before driver initialization
         return b''
     try:
-        screenshot_file_path = image_path().create_failure_screenshot_file_path()
-        driver().save_screenshot(screenshot_file_path)
+        screenshot_file_path = create_failure_screenshot()
         report().log_image(screenshot_file_path, "Step Failure Screenshot")
         with open(screenshot_file_path, "rb") as sf:
             file_bin = sf.read()
         return base64.b64encode(file_bin)  # is not displayed correctly
     except Exception as e:
         report().log(str(e))
         return b''
 
 
 # Steps -------------------------------------------
 
 
 @step("Wait <secs>")
 def wait_for(secs_param: str) -> None:
-    secs = _substitute(secs_param)
+    secs = substitute(secs_param)
     time.sleep(float(secs))
 
 
 @step("Wait for window <secs> and save handle as <placeholder>")
 def wait_for_window(secs_param: str, placeholder_name_param: str) -> None:
-    secs = _substitute(secs_param)
-    placeholder_name = _substitute(placeholder_name_param)
+    secs = substitute(secs_param)
+    placeholder_name = substitute(placeholder_name_param)
     assert placeholder_name in data_store.scenario.keys(), "Expected saved window handles. Did you use '* Save window handles'?"
     
     time.sleep(float(secs))
     wh_now = driver().window_handles
     #previous saved window handles
     wh_then = data_store.scenario[placeholder_name]
     if len(wh_now) > len(wh_then):
@@ -150,16 +141,16 @@
 @step("Maximize")
 def maximize() -> None:
     driver().maximize_window()
 
 
 @step("Window size <width>x<height>")
 def window_size(width_param: str, height_param: str) -> None:
-    width = int(_substitute(width_param))
-    height = int(_substitute(height_param))
+    width = int(substitute(width_param))
+    height = int(substitute(height_param))
     outer_width, inner_width, outer_height, inner_height = driver().execute_script("""
     return [window.outerWidth, window.innerWidth, window.outerHeight, window.innerHeight]""")
     if outer_width == 0:
         outer_width = inner_width
     if outer_height == 0:
         outer_height = inner_height
     report().log_debug("outer width: {}, inner width: {}, width: {}, outer height: {}, inner height: {}, height: {}"\
@@ -199,15 +190,15 @@
 @step("Forward")
 def forward() -> None:
     driver().forward()
 
 
 @step("Open <page>")
 def open_page(page_param: str) -> None:
-    page = _substitute(page_param)
+    page = substitute(page_param)
     basic_auth_list = data_store.spec.get(basic_auth_key, [])
     webdriver = driver()
     uses_basic_auth = False
     for regexp, authorization in basic_auth_list:
         if re.match(regexp, page):
             uses_basic_auth = True
             report().log(f"URL matches `{regexp}` - using basic auth")
@@ -232,57 +223,57 @@
                 pass
 
 
 @step("Open <page> for <user>: <password>")
 def open_page_for_user_and_password(page_param: str, user_param: str, password_param: str) -> None:
     report().log("This step is deprecated for security concerns. Instead use:")
     report().log("`* Register authentication <user>: <password> for <regexp>`")
-    page = _substitute(page_param)
+    page = substitute(page_param)
     prefix_match = re.match(r"https?://", page)
     prefix = prefix_match.group(0) if prefix_match else ""
     page = page[len(prefix):]
-    user = urllib.parse.quote_plus(_substitute(user_param))
-    password = urllib.parse.quote_plus(_substitute(password_param))
+    user = urllib.parse.quote_plus(substitute(user_param))
+    password = urllib.parse.quote_plus(substitute(password_param))
     url = "{}{}:{}@{}".format(prefix, user, password, page)
     driver().get(url)
     # Chrome sometimes opens the page in the middle, when visited before
     time.sleep(0.3)
     if "#" not in page:
         driver().execute_script("window.scrollTo(0, 0);")
 
 
 @step("Register authentication <user>: <password> for <regexp>")
 def register_basic_auth_for_regexp(user_param: str, password_param: str, regexp_param: str):
     # Basic auth with CDP is not supported by all browser yet
-    username = _substitute(user_param)
-    password = _substitute(password_param)
-    regexp = _substitute(regexp_param)
+    username = substitute(user_param)
+    password = substitute(password_param)
+    regexp = substitute(regexp_param)
     authorization = base64.b64encode(f"{username}:{password}".encode("utf-8")).decode("ascii")
     auth_list = data_store.spec.get(basic_auth_key, [])
     auth_list.append((regexp, authorization, ))
     data_store.spec[basic_auth_key] = auth_list
 
 
 @step("Remove authentication for <regexp>")
 def remove_basic_auth_for_regexp(regexp_param: str):
-    regexp = _substitute(regexp_param)
+    regexp = substitute(regexp_param)
     auth_list = data_store.spec.get(basic_auth_key, [])
     auth_list[:] = filterfalse(lambda t: regexp == t[0], auth_list)
 
 
 @step("Print window handles")
 def print_window_handles() -> None:
     window_handles = driver().window_handles
     report().log("Windows: [{}]".format(", ".join(window_handles)))
 
 
 @step("Switch to window <window_param>")
 def switch_to_window(window_param: str) -> None:
     if window_param.isdigit():
-        window_num = int(_substitute(window_param))
+        window_num = int(substitute(window_param))
         window = driver().window_handles[window_num]
         driver().switch_to.window(window)
         report().log(f"Switched to window with index {window_num}")
     else:
         original_window = driver().current_window_handle
         handles = driver().window_handles
         for handle in handles:
@@ -300,30 +291,30 @@
 @step("Switch to default content")
 def switch_to_default_content() -> None:
     driver().switch_to.default_content()
 
 
 @step("Switch to frame <frame_param>")
 def switch_to_frame(frame_name_or_index_param: str) -> None:
-    frame_param = _substitute(frame_name_or_index_param)
+    frame_param = substitute(frame_name_or_index_param)
     if frame_param.isdigit():
         index = int(frame_param)
-        frames = _find_elements("tag name", "frame")
+        frames = find_elements("tag name", "frame")
         if len(frames) == 0:
-            frames = _find_elements("tag name", "iframe")
+            frames = find_elements("tag name", "iframe")
         assert len(frames)  > 0, "no frames or iframes found in current page."
         assert len(frames) >= index, f"frame index {index} is higher than number of frames in current page: {len(frames)}"
         driver().switch_to.frame(frames[index])
     else:
         driver().switch_to.frame(frame_param)
 
 
 @step("Switch to frame <by> = <by_value>")
 def switch_to_frame_by_selector(by: str, by_value: str) -> None:
-    frame = _find_element(by, by_value)
+    frame = find_element(by, by_value)
     driver().switch_to.frame(frame)
 
 
 @step("Dismiss alert")
 def dismiss_alert() -> None:
     driver().switch_to.alert.dismiss()
     driver().switch_to.default_content()
@@ -333,62 +324,56 @@
 def accept_alert() -> None:
     driver().switch_to.alert.accept()
     driver().switch_to.default_content()
 
 
 @step("Answer in prompt <text>")
 def answer_in_prompt(text: str) -> None:
-    prompt_text = _substitute(text)
+    prompt_text = substitute(text)
     alert = driver().switch_to.alert
     alert.send_keys(prompt_text)
     alert.accept()
     driver().switch_to.default_content()
 
 
 @step("Take a screenshot <file>")
 def take_screenshot(image_file_name_param: str) -> None:
-    image_file_name = _substitute(image_file_name_param)
-    screenshot_file_path = image_path().create_screenshot_file_path(image_file_name)
-    driver().save_screenshot(screenshot_file_path)
+    image_file_name = substitute(image_file_name_param)
+    screenshot_file_path = create_screenshot(image_file_name)
     report().log_image(screenshot_file_path)
 
 
 @step("Take a screenshot of <by> = <by_value> <file>")
 def take_screenshot_of_element(by: str, by_value: str, image_file_name_param: str) -> None:
-    element = _find_element(by, by_value)
-    image_file_name = _substitute(image_file_name_param)
-    screenshot_file_path = image_path().create_screenshot_file_path(image_file_name)
-    driver().save_screenshot(screenshot_file_path)
+    element = find_element(by, by_value)
+    image_file_name = substitute(image_file_name_param)
+    screenshot_file_path = create_screenshot(image_file_name)
     pixel_ratio = _device_pixel_ratio()
     viewport_offset = _viewport_offset()
-    images().crop_image_file(
+    crop_image(
         screenshot_file_path,
         element.location,
         element.size,
         pixel_ratio,
         viewport_offset
     )
     report().log_image(screenshot_file_path)
 
 
 @step("Take screenshots of whole page <file>")
 def take_screenshots_of_whole_page(image_file_name_param: str) -> None:
-    image_file_name = _substitute(image_file_name_param)
     if _is_firefox_page_screenshot_no_scrolling():
-        _screenshot_of_whole_page_no_scrolling(image_file_name)
+        image_file_name = substitute(image_file_name_param)
+        screenshot_file_path = create_screenshot(image_file_name)
+        report().log_image(screenshot_file_path)
     else:
+        image_file_name = substitute(image_file_name_param)
         _screenshot_of_whole_page_with_scrolling(image_file_name)
 
 
-def _screenshot_of_whole_page_no_scrolling(image_file_name: str) -> None:
-    screenshot_file_path = image_path().create_screenshot_file_path(image_file_name)
-    driver().save_full_page_screenshot(screenshot_file_path)
-    report().log_image(screenshot_file_path)
-
-
 def _screenshot_of_whole_page_with_scrolling(image_file_name: str) -> None:
     postfix = 1
     should_continue = True
     while should_continue:
         filename_with_postfix = "".join((image_file_name, "_", str(postfix)))
         postfix += 1
         take_screenshot(filename_with_postfix)
@@ -398,350 +383,350 @@
         after_scroll_offset = driver().execute_script("return window.pageYOffset")
         if after_scroll_offset <= current_offset or postfix > 32:
             should_continue = False
 
 
 @step("Check <by> = <by_value>")
 def check_element(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     if not element.is_selected():
         element.click()
 
 
 @step("Uncheck <by> = <by_value>")
 def uncheck_element(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     if element.is_selected():
         element.click()
 
 
 @step("Select <by> = <by_value> option <select_key> = <select_value>")
 def select_option(by: str, by_value: str, select_key_param: str, select_value_param: str) -> None:
-    element = _find_element(by, by_value)
-    select_key = _substitute(select_key_param)
-    select_value = _substitute(select_value_param)
+    element = find_element(by, by_value)
+    select_key = substitute(select_key_param)
+    select_value = substitute(select_value_param)
     key = SelectKey.to_enum(select_key)
     Selector.select(element, select_value, key)
 
 
 @step("Click <by> = <by_value>")
 def click_element(by: str, by_value: str) -> None:
-    _find_element(by, by_value).click()
+    find_element(by, by_value).click()
 
 
 @step("Double click <by> = <by_value>")
 def double_click_element(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     ActionChains(driver()).double_click(element).perform()
 
 
 @step("Click <by> = <by_value> <key_down>")
 def click_element_with_key_down(by: str, by_value: str, key_down_param: str) -> None:
-    keys_down = _map_keys(_substitute(key_down_param))
-    element = _find_element(by, by_value)
+    keys_down = KeyMapper.map_keys(substitute(key_down_param))
+    element = find_element(by, by_value)
     ac = ActionChains(driver())
     for key in keys_down:
         ac.key_down(key)
     ac.click(element)
     for key in keys_down:
         ac.key_up(key)
     ac.perform()
 
 
 @step("Right click <by> = <by_value>")
 def right_click_element(by: str, by_value: str) -> None:
     actionChains = ActionChains(driver())
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     actionChains.context_click(element).perform()
 
 
 @step("Type <string>")
 def type_string(a_string_param: str) -> None:
-    a_string = _substitute(a_string_param)
+    a_string = substitute(a_string_param)
     if not _is_mobile_operating_system():
         ActionChains(driver())\
             .send_keys(a_string)\
             .perform()
     else:
         _focused_element().send_keys(a_string)
 
 
 @step("Type <key_down> <string>")
 def type_string_with_key_down(key_down_param: str, a_string_param: str) -> None:
-    keys_down = _map_keys(_substitute(key_down_param))
-    a_string = _substitute(a_string_param)
+    keys_down = KeyMapper.map_keys(substitute(key_down_param))
+    a_string = substitute(a_string_param)
     ac = ActionChains(driver())
     for key in keys_down:
         ac.key_down(key)
     ac.send_keys(a_string)
     for key in keys_down:
         ac.key_up(key)
     ac.perform()
 
 
 @step("Type <by> = <by_value> <string>")
 def type_string_into_element(by: str, by_value: str, a_string_param: str) -> None:
-    a_string = _substitute(a_string_param)
-    element = _find_element(by, by_value)
+    a_string = substitute(a_string_param)
+    element = find_element(by, by_value)
     element.clear()
     if not _is_mobile_operating_system():
         ActionChains(driver())\
             .click(element)\
             .send_keys(a_string)\
             .perform()
     else:
         element.click()
         element.send_keys(a_string)
 
 
 @step("Type <by> = <by_value> <key_down> <string>")
 def type_string_into_element_with_key_down(by: str, by_value: str, key_down_param: str, a_string_param: str) -> None:
-    keys_down = _map_keys(_substitute(key_down_param))
-    a_string = _substitute(a_string_param)
-    element = _find_element(by, by_value)
+    keys_down = KeyMapper.map_keys(substitute(key_down_param))
+    a_string = substitute(a_string_param)
+    element = find_element(by, by_value)
     element.clear()
     ac = ActionChains(driver())\
         .click(element)
     for key in keys_down:
         ac.key_down(key)
     ac.send_keys(a_string)
     for key in keys_down:
         ac.key_up(key)
     ac.perform()
 
 
 @step("Send keys <keys>")
 def send_keys(keys_param: str) -> None:
-    send_keys = _map_keys(_substitute(keys_param))
+    send_keys = KeyMapper.map_keys(substitute(keys_param))
     ActionChains(driver())\
         .send_keys(send_keys)\
         .perform()
 
 
 @step("Send keys <key_down> <keys>")
 def send_keys_with_key_down(key_down_param: str, keys_param: str) -> None:
-    keys_down = _map_keys(_substitute(key_down_param))
-    send_keys = _map_keys(_substitute(keys_param))
+    keys_down = KeyMapper.map_keys(substitute(key_down_param))
+    send_keys = KeyMapper.map_keys(substitute(keys_param))
     ac = ActionChains(driver())
     for key in keys_down:
         ac.key_down(key)
     ac.send_keys(send_keys)
     for key in keys_down:
         ac.key_up(key)
     ac.perform()
 
 
 @step("Send <by> = <by_value> keys <keys>")
 def send_keys_to_element(by: str, by_value: str, keys_param: str) -> None:
-    send_keys = _map_keys(_substitute(keys_param))
-    element = _find_element(by, by_value)
+    send_keys = KeyMapper.map_keys(substitute(keys_param))
+    element = find_element(by, by_value)
     ActionChains(driver())\
         .click(element)\
         .send_keys(send_keys)\
         .perform()
 
 
 @step("Send <by> = <by_value> keys <key_down> <keys>")
 def send_keys_to_element_with_key_down(by: str, by_value: str, key_down_param: str, keys_param: str) -> None:
-    keys_down = _map_keys(_substitute(key_down_param))
-    send_keys = _map_keys(_substitute(keys_param))
-    element = _find_element(by, by_value)
+    keys_down = KeyMapper.map_keys(substitute(key_down_param))
+    send_keys = KeyMapper.map_keys(substitute(keys_param))
+    element = find_element(by, by_value)
     ac = ActionChains(driver())\
         .click(element)
     for key in keys_down:
         ac.key_down(key)
     ac.send_keys(send_keys)
     for key in keys_down:
         ac.key_up(key)
     ac.perform()
 
 
 @step("Clear <by> = <by_value>")
 def clear_element(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     element.clear()
 
 
 @step("Mouse down <by> = <by_value>")
 def mouse_down(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     ActionChains(driver()).move_to_element(element).click_and_hold(element).perform()
 
 
 @step("Mouse up <by> = <by_value>")
 def mouse_up(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     ActionChains(driver()).move_to_element(element).release(element).perform()
 
 
 @step("Move to <by> = <by_value>")
 def move_into_view(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     # the following script is needed for some browsers
     driver().execute_script("arguments[0].scrollIntoView(true);", element)
     try:
         ActionChains(driver()).move_to_element(element).perform()
     except WebDriverException as e:
         # in some mobile browsers it fails
         report().log_debug(f"received exception while moving to {element}: {e}")
 
 
 @step("Move to and center <by> = <by_value>")
 def move_into_view_and_center(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     driver().execute_script("arguments[0].scrollIntoView({block: 'center', inline: 'nearest'});", element)
 
 
 @step("Move out")
 def move_out_of_view() -> None:
-    element = _find_element("css selector", "body")
+    element = find_element("css selector", "body")
     ActionChains(driver()).move_to_element_with_offset(element, 0, 0).perform()
 
 
 @step("Hover over <by> = <by_value>")
 def hover_over(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     ActionChains(driver()).move_to_element(element).perform()
 
 
 @step("Scroll <by> = <by_value> into view")
 def scrollElementIntoView(by: str, by_value: str) -> None:
-    _find_element(by, by_value)\
+    find_element(by, by_value)\
         .location_once_scrolled_into_view
 
 
 @step("Drag and drop <by_source> = <by_value_source> into <by_dest> = <by_value_dest>")
 def dragAndDropElement(by_source: str, by_value_source: str, by_dest: str, by_value_dest: str) -> None:
-    sourceElement = _find_element(by_source, by_value_source)
-    destinationElement = _find_element(by_dest, by_value_dest)
+    sourceElement = find_element(by_source, by_value_source)
+    destinationElement = find_element(by_dest, by_value_dest)
     ActionChains(driver()).drag_and_drop(sourceElement, destinationElement).perform()
 
 
 @step("Upload file = <file_path> into <by> = <by_value>")
 def uploadFile(file_path_param: str, by: str, by_value: str) -> None:
-    file_path = _substitute(file_path_param)
-    _find_element(by, by_value).send_keys(file_path)
+    file_path = substitute(file_path_param)
+    find_element(by, by_value).send_keys(file_path)
 
 
 @step("Execute <script>")
 def execute_script(script_param: str) -> None:
-    script = _substitute(script_param)
+    script = substitute(script_param)
     driver().execute_script(script)
 
 
 @step("Execute <script> and save result in <placeholder>")
 def execute_script_save_result(script_param: str, placeholder_name_param: str) -> None:
-    script = _substitute(script_param)
-    placeholder_name = _substitute(placeholder_name_param)
+    script = substitute(script_param)
+    placeholder_name = substitute(placeholder_name_param)
     res = driver().execute_script(script)
     data_store.scenario[placeholder_name] = res
 
 
 @step("Execute <script> with <by> = <by_value> as <elem>")
 def execute_script_on_element(script_param: str, by: str, by_value: str, elem_param: str) -> None:
-    script = _substitute(script_param)
-    elem = _substitute(elem_param)
+    script = substitute(script_param)
+    elem = substitute(elem_param)
     assert elem in script, f"no element with name '{elem}' is referred to in the script"
-    found = _find_element(by, by_value)
+    found = find_element(by, by_value)
     driver().execute_script(f"var {elem}=arguments[0]; {script}", found)
 
 
 @step("Execute <script> with <by> = <by_value> as <elem> and save result in <placeholder>")
 def execute_script_on_element_save_result(script_param: str, by: str, by_value: str, elem_param: str, placeholder_name_param: str) -> None:
-    script = _substitute(script_param)
-    elem = _substitute(elem_param)
-    placeholder_name = _substitute(placeholder_name_param)
+    script = substitute(script_param)
+    elem = substitute(elem_param)
+    placeholder_name = substitute(placeholder_name_param)
     assert elem in script, f"no element with name '{elem}' is referred to in the script"
-    found = _find_element(by, by_value)
+    found = find_element(by, by_value)
     res = driver().execute_script(f"var {elem}=arguments[0]; {script}", found)
     data_store.scenario[placeholder_name] = res
 
 
 @step("Execute async <script>")
 def execute_async_script(script_param: str) -> None:
-    script = _substitute(script_param)
+    script = substitute(script_param)
     driver().execute_async_script(script)
 
 
 @step("Execute async <script> and save result in <placeholder> with callback <callback>")
 def execute_async_script_save_result(script_param: str, placeholder_name_param: str, callback_param: str) -> None:
-    script = _substitute(script_param)
-    placeholder_name = _substitute(placeholder_name_param)
-    callback = _substitute(callback_param)
+    script = substitute(script_param)
+    placeholder_name = substitute(placeholder_name_param)
+    callback = substitute(callback_param)
     assert callback in script, f"no callback with name '{callback}' is invoked in the script"
     res = driver().execute_async_script(f"var {callback}=arguments[arguments.length-1]; {script}")
     data_store.scenario[placeholder_name] = res
 
 
 @step("Execute async <script> with <by> = <by_value> as <elem>")
 def execute_async_script_on_element(script_param: str, by: str, by_value: str, elem_param: str) -> None:
-    script = _substitute(script_param)
-    elem = _substitute(elem_param)
+    script = substitute(script_param)
+    elem = substitute(elem_param)
     assert elem in script, f"no element with name '{elem}' is referred to in the script"
-    found = _find_element(by, by_value)
+    found = find_element(by, by_value)
     driver().execute_async_script(f"var {elem}=arguments[0]; {script}", found)
 
 
 @step("Execute async <script> with <by> = <by_value> as <elem> and save result in <placeholder> with callback <callback>")
 def execute_async_script_on_element_save_result(
     script_param: str,
     by: str,
     by_value: str,
     elem_param: str,
     placeholder_name_param: str,
     callback_param: str
 ) -> None:
-    script = _substitute(script_param)
-    elem = _substitute(elem_param)
-    placeholder_name = _substitute(placeholder_name_param)
-    callback = _substitute(callback_param)
+    script = substitute(script_param)
+    elem = substitute(elem_param)
+    placeholder_name = substitute(placeholder_name_param)
+    callback = substitute(callback_param)
     assert elem in script, f"no element with name '{elem}' is referred to in the script"
     assert callback in script, f"no callback with name '{callback}' is invoked in the script"
-    found = _find_element(by, by_value)
+    found = find_element(by, by_value)
     res = driver().execute_async_script(f"var {elem}=arguments[0]; var {callback}=arguments[arguments.length-1]; {script}", found)
     data_store.scenario[placeholder_name] = res
 
 
 @step("Save placeholder <placeholder> = <value>")
 def save_placeholder(placeholder_name_param: str, placeholder_value_param: str) -> None:
-    placeholder_name = _substitute(placeholder_name_param)
-    placeholder_value = _substitute(placeholder_value_param)
+    placeholder_name = substitute(placeholder_name_param)
+    placeholder_value = substitute(placeholder_value_param)
     data_store.scenario[placeholder_name] = placeholder_value
 
 
 @step("Save placeholder <placeholder> from <by> = <by_value>")
 def save_placeholder_from_element(placeholder_name_param: str, by: str, by_value: str) -> None:
-    placeholder_name = _substitute(placeholder_name_param)
-    text = _get_text_from_element(by, by_value)
+    placeholder_name = substitute(placeholder_name_param)
+    text = get_text_from_element(by, by_value)
     data_store.scenario[placeholder_name] = text
 
 
 @step("Save placeholder <placeholder> from attribute <attribute_param> of <by> = <by_value>")
 def save_placeholder_from_element_attribute(placeholder_name_param: str, attribute_param: str, by: str, by_value: str) -> None:
-    placeholder_name = _substitute(placeholder_name_param)
-    attribute = _substitute(attribute_param)
-    attribute_value = _find_attribute(by, by_value, attribute)
+    placeholder_name = substitute(placeholder_name_param)
+    attribute = substitute(attribute_param)
+    attribute_value = find_attribute(by, by_value, attribute)
     data_store.scenario[placeholder_name] = attribute_value
 
 
 @step("Save window handles as <placeholder>")
 def save_window_handles(placeholder_name_param: str) -> None:
-    placeholder_name = _substitute(placeholder_name_param)
+    placeholder_name = substitute(placeholder_name_param)
     data_store.scenario[placeholder_name] = driver().window_handles
 
 
 @step("Save window title as <placeholder>")
 def save_window_title(placeholder_name_param: str) -> None:
-    placeholder_name = _substitute(placeholder_name_param)
+    placeholder_name = substitute(placeholder_name_param)
     data_store.scenario[placeholder_name] = driver().title
 
 
 @step("Set timeout <seconds>")
 def set_timeout(seconds_param: str):
-    seconds = _substitute(seconds_param)
+    seconds = substitute(seconds_param)
     assert seconds.replace('.', '', 1).isdigit(),\
         _err_msg(f"argument '{seconds_param}' should be a number")
     data_store.scenario[timeout_key] = float(seconds)
 
 
 @step("Reset timeout")
 def reset_timeout():
@@ -749,21 +734,21 @@
 
 
 # Steps Asserts ------------------------------------------------
 
 
 @step("Show message in an error case <error_message>")
 def show_error_message_in_case(error_msg_param: str) -> None:
-    error_msg = _substitute(error_msg_param)
+    error_msg = substitute(error_msg_param)
     data_store.scenario[error_message_key] = error_msg
 
 
 @step("Assert window handles is <windows_num>")
 def assert_window_handle_num(window_num_param: str) -> None:
-    window_num = _substitute(window_num_param)
+    window_num = substitute(window_num_param)
     expected = int(window_num)
     actual = len(driver().window_handles)
     assert expected == actual,\
         _err_msg(f"expected {expected} window handles, got {actual}")
 
 
 @step("Assert title equals <title>")
@@ -778,261 +763,250 @@
     dialog_text = driver().switch_to.alert.text
     assert expected_text == dialog_text,\
         _err_msg(f"expected dialog text: {expected_text}, actual {dialog_text}")
 
 
 @step("Assert url equals <url>")
 def assert_url(expected_url_param: str) -> None:
-    expected_url = _substitute(expected_url_param)
+    expected_url = substitute(expected_url_param)
     current_url = driver().current_url
     assert expected_url == current_url,\
         _err_msg(f"expected url: {expected_url}, actual {current_url}")
 
 
 @step("Assert url starts with <url>")
 def assert_url_starts_with(expected_url_param: str) -> None:
-    expected_url = _substitute(expected_url_param)
+    expected_url = substitute(expected_url_param)
     current_url = driver().current_url
     assert current_url.startswith(expected_url),\
         _err_msg(f"url {current_url} does not start with {expected_url}")
 
 
 @step("Assert url ends with <url>")
 def assert_url_ends_with(expected_url_param: str) -> None:
-    expected_url = _substitute(expected_url_param)
+    expected_url = substitute(expected_url_param)
     current_url = driver().current_url
     assert current_url.endswith(expected_url),\
         _err_msg(f"url {current_url} does not end with {expected_url}")
 
 
 @step("Assert url contains <url>")
 def assert_url_contains(expected_url_param: str) -> None:
-    expected_url = _substitute(expected_url_param)
+    expected_url = substitute(expected_url_param)
     current_url = driver().current_url
     assert expected_url in current_url,\
         _err_msg(f"url {current_url} does not contain {expected_url}")
 
 
 # see also before_step_hook
 @step(["Assert <by> = <by_value> exists", "Assert <by> = <by_value> is displayed"])
 def assert_element_exists(by: str, by_value: str) -> None:
-    marker = _marker(_substitute(by), _substitute(by_value))
-    visible = _wait_until(EC.visibility_of_element_located(marker))
+    marker = get_marker(substitute(by), substitute(by_value))
+    visible = wait_until(EC.visibility_of_element_located(marker))
     assert visible,\
         _err_msg(f"element {by} = {by_value} does not exists")
 
 
 # see also before_step_hook
 @step(["Assert <by> = <by_value> does not exist", "Assert <by> = <by_value> is invisible"])
 def assert_element_does_not_exist(by_param: str, by_value_param: str) -> None:
-    by = _substitute(by_param)
-    by_value = _substitute(by_value_param)
-    marker = _marker(by, by_value)
-    invisible = _wait_until(EC.invisibility_of_element(marker))
+    by = substitute(by_param)
+    by_value = substitute(by_value_param)
+    marker = get_marker(by, by_value)
+    invisible = wait_until(EC.invisibility_of_element(marker))
     assert invisible, \
         _err_msg(f"element {by} = {by_value} exists")
 
 
 @step("Assert <by> = <by_value> is enabled")
 def assert_element_is_enabled(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     assert element.is_enabled(),\
         _err_msg(f"element {by} = {by_value} is disabled")
 
 
 @step("Assert <by> = <by_value> is disabled")
 def assert_element_is_disabled(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     assert not element.is_enabled(), \
         _err_msg(f"element {by} = {by_value} is enabled")
 
 
 @step("Assert <by> = <by_value> is selected")
 def assert_element_is_selected(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     assert element.is_selected(),\
         _err_msg(f"element {by} = {by_value} is not selected")
 
 
 @step("Assert <by> = <by_value> has selected value <value>")
 def assert_selected_option(by: str, by_value: str, expected_param: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     actual = Selector.get_selected_value(element)
-    expected = _substitute(expected_param)
+    expected = substitute(expected_param)
     assert expected == actual,\
         _err_msg(f"expected value: {expected}, actual {actual}")
 
 
 @step("Assert <by> = <by_value> is not selected")
 def assert_element_is_not_selected(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     assert not element.is_selected(), \
         _err_msg(f"element {by} = {by_value} is selected")
 
 
 @step("Assert <by> = <by_value> equals <string>")
 def assert_text_equals(by: str, by_value: str, expected_text_param: str) -> None:
-    expected_text = _substitute(expected_text_param)
-    text = _get_text_from_element(by, by_value)
+    expected_text = substitute(expected_text_param)
+    text = get_text_from_element(by, by_value)
     assert text == expected_text,\
         _err_msg(f"element {by} = {by_value} expected text {expected_text}, actual {text}")
 
 
 @step("Assert <by> = <by_value> does not equal <string>")
 def assert_text_does_not_equal(by: str, by_value: str, expected_text_param: str) -> None:
-    expected_text = _substitute(expected_text_param)
-    text = _get_text_from_element(by, by_value)
+    expected_text = substitute(expected_text_param)
+    text = get_text_from_element(by, by_value)
     assert text != expected_text,\
         _err_msg(f"element {by} = {by_value} expected actual {text} not to be equal to {expected_text}")
 
 
 @step("Assert <by> = <by_value> regexp <regexp>")
 def assert_regexp_in_element(by: str, by_value: str, regexp_param: str) -> None:
-    regexp = _substitute(regexp_param)
-    text = _get_text_from_element(by, by_value)
+    regexp = substitute(regexp_param)
+    text = get_text_from_element(by, by_value)
     assert re.match(regexp, text),\
         _err_msg(f"element {by} = {by_value}: regexp {regexp} does not match {text}")
 
 
 @step("Assert <by> = <by_value> contains <string>")
 def assert_text_contains(by: str, by_value: str, contains_text_param: str) -> None:
-    contains_text = _substitute(contains_text_param)
-    text = _get_text_from_element(by, by_value)
+    contains_text = substitute(contains_text_param)
+    text = get_text_from_element(by, by_value)
     assert contains_text in text,\
         _err_msg(f"element {by} = {by_value} expected actual {text} to contain {contains_text}")
 
 
 @step("Assert <by> = <by_value> does not contain <string>")
 def assert_text_does_not_contain(by: str, by_value: str, contains_text_param: str) -> None:
-    contains_text = _substitute(contains_text_param)
-    text = _get_text_from_element(by, by_value)
+    contains_text = substitute(contains_text_param)
+    text = get_text_from_element(by, by_value)
     assert contains_text not in text,\
         _err_msg(f"element {by} = {by_value} expected actual {text} to not contain {contains_text}")
 
 
 @step("Assert <by> = <by_value> css <css_property_name> is <css_expected_value>")
 def assert_css_property(by: str, by_value: str, css_property_name_param: str, css_expected_value_param: str) -> None:
-    element = _find_element(by, by_value)
-    css_property_name = _substitute(css_property_name_param)
-    css_expected_value = _substitute(css_expected_value_param)
+    element = find_element(by, by_value)
+    css_property_name = substitute(css_property_name_param)
+    css_expected_value = substitute(css_expected_value_param)
     css_actual_value = element.value_of_css_property(css_property_name)
     assert css_actual_value == css_expected_value,\
         _err_msg(f"element {by} = {by_value}: css property {css_property_name} expected: {css_expected_value}, actual: {css_actual_value}")
 
 
 @step("Assert <by> = <by_value> is focused")
 def assert_element_is_focused(by: str, by_value: str) -> None:
-    element = _find_element(by, by_value)
+    element = find_element(by, by_value)
     assert element == _focused_element(),\
         _err_msg(f"element {by} = {by_value} is not in focus")
 
 
 @step("Assert <by> = <by_value> attribute <attribute> exists")
 def assert_attribute_exists(by: str, by_value: str, attribute_param: str) -> None:
-    attribute = _substitute(attribute_param)
-    found_value =  _find_attribute(by, by_value, attribute)
+    attribute = substitute(attribute_param)
+    found_value =  find_attribute(by, by_value, attribute)
     assert found_value, _err_msg(f"element {by} = {by_value} has no attribute {attribute}")
 
 
 @step("Assert <by> = <by_value> attribute <attribute> contains <value>")
 def assert_attribute_contains(by: str, by_value: str, attribute_param: str, value_param: str) -> None:
-    attribute = _substitute(attribute_param)
-    value = _substitute(value_param)
-    found_value = _find_attribute(by, by_value, attribute)
+    attribute = substitute(attribute_param)
+    value = substitute(value_param)
+    found_value = find_attribute(by, by_value, attribute)
     assert found_value, _err_msg(f"element {by} = {by_value} has no attribute {attribute}")
     assert value in found_value, _err_msg(f"attribute {attribute} in element {by} = {by_value} does not contain {value} - found: {found_value}")
 
 
 @step("Assert <by> = <by_value> attribute <attribute> equals <value>")
 def assert_attribute_equals(by: str, by_value: str, attribute_param: str, value_param: str) -> None:
-    attribute = _substitute(attribute_param)
-    value = _substitute(value_param)
-    found_value = _find_attribute(by, by_value, attribute)
+    attribute = substitute(attribute_param)
+    value = substitute(value_param)
+    found_value = find_attribute(by, by_value, attribute)
     assert found_value, _err_msg(f"element {by} = {by_value} has no attribute {attribute}")
     assert value == found_value, _err_msg(f"attribute {attribute} in element {by} = {by_value} does not equal {value} - found: {found_value}")
 
 
 @step("Assert <by> = <by_value> attribute <attribute> does not contain <value>")
 def assert_attribute_does_not_contain(by: str, by_value: str, attribute_param: str, value_param: str) -> None:
-    attribute = _substitute(attribute_param)
-    value = _substitute(value_param)
-    found_value = _find_attribute(by, by_value, attribute)
+    attribute = substitute(attribute_param)
+    value = substitute(value_param)
+    found_value = find_attribute(by, by_value, attribute)
     if found_value:
         assert value not in found_value, _err_msg(f"attribute {attribute} in element {by} = {by_value} contains {value} - found: {found_value}")
 
 
 @step("Assert <by> = <by_value> screenshot resembles <file> with SSIM more than <threshold>")
 def assert_image_resembles(by: str, by_value: str, image_file_name_param: str, threshold_param: str) -> None:
-    element = _find_element(by, by_value)
-    threshold = float(_substitute(threshold_param))
+    element = find_element(by, by_value)
+    threshold = float(substitute(threshold_param))
     assert 0.0 <= threshold <= 1.0, "threshold must be between 0.0 and 1.0"
-    image_file_name = _substitute(image_file_name_param)
-    actual_screenshot_full_path = image_path().create_actual_screenshot_file_path(image_file_name)
-    driver().save_screenshot(actual_screenshot_full_path)
     pixel_ratio = _device_pixel_ratio()
     viewport_offset = _viewport_offset()
-    images().crop_image_file(
-        actual_screenshot_full_path,
-        element.location,
-        element.size,
-        pixel_ratio,
-        viewport_offset
-    )
-    expected_screenshot_full_path = image_path().create_expected_screenshot_file_path(image_file_name)
-    diff_formats = config.get_diff_formats()
-    ssim = images().adapt_and_compare_images(expected_screenshot_full_path, actual_screenshot_full_path, diff_formats)
+    image_file_name = substitute(image_file_name_param)
+    ssim = get_structured_similarity_to_expected(image_file_name, element.location, element.size, pixel_ratio, viewport_offset)
     assert ssim >= threshold, \
         _err_msg(f"SSIM {ssim} is less than threshold {threshold}")
 
 
 @step("Assert page screenshots resemble <file> with SSIM more than <threshold>")
 def assert_whole_page_resembles(image_file_name_param: str, threshold_param: str) -> None:
-    threshold = float(_substitute(threshold_param))
+    threshold = float(substitute(threshold_param))
     assert 0.0 <= threshold <= 1.0, "threshold must be between 0.0 and 1.0"
-    image_file_name = _substitute(image_file_name_param)
+    image_file_name = substitute(image_file_name_param)
     if _is_firefox_page_screenshot_no_scrolling():
-        failed_asserts = _ssim_screenshot_noscrolling(image_file_name, threshold)
+        failed_asserts = ssim_screenshot_noscrolling(image_file_name, threshold)
     else:
-        failed_asserts = _ssim_screenshot_scrolling(image_file_name, threshold)
+        failed_asserts = ssim_screenshot_scrolling(image_file_name, threshold)
     assert len(failed_asserts) == 0,\
             _err_msg("Assertions failed:\n\t{}".format("\n\t".join(failed_asserts)))
 
 
 @step("Assert page screenshots resemble <file> with SSIM more than <threshold> for <pages> pages")
 def assert_pages_resemble(image_file_name_param: str, threshold_param: str, pages_param: str) -> None:
     """This step exists in case the upper step does not work, f.i. due to framework restrictions"""
-    threshold = float(_substitute(threshold_param))
+    threshold = float(substitute(threshold_param))
     assert 0.0 <= threshold <= 1.0, "threshold must be between 0.0 and 1.0"
-    image_file_name = _substitute(image_file_name_param)
-    pages = int(_substitute(pages_param))
+    image_file_name = substitute(image_file_name_param)
+    pages = int(substitute(pages_param))
     failed_asserts = []
     for page in range(1, pages + 1):
-        actual_screenshot_full_path = image_path().create_actual_screenshot_file_path(image_file_name, page)
-        driver().save_screenshot(actual_screenshot_full_path)
-        expected_screenshot_full_path = image_path().create_expected_screenshot_file_path(image_file_name, page)
+        actual_screenshot_full_path = create_actual_screenshot_file_path(image_file_name, page)
+        expected_screenshot_full_path = create_expected_screenshot_file_path(image_file_name, page)
         page += 1
         send_keys("PAGE_DOWN")
         time.sleep(0.6)
         if not os.path.isfile(expected_screenshot_full_path):
             failed_asserts.append("screenshot {} does not exist".format(expected_screenshot_full_path))
         else:
-            _append_structured_similarity(failed_asserts, expected_screenshot_full_path, actual_screenshot_full_path, threshold)
+            append_structured_similarity(failed_asserts, expected_screenshot_full_path, actual_screenshot_full_path, threshold)
+
     assert len(failed_asserts) == 0,\
             _err_msg("Assertions failed:\n\t{}".format("\n\t".join(failed_asserts)))
 
 
 @step("Fail <message>")
 def fail(message_param: str) -> None:
-    message = _substitute(message_param)
+    message = substitute(message_param)
     report().log(message)
     assert False
 
 @step("Print message <message>")
 def print_message(message_param: str) -> None:
-    message = _substitute(message_param)
+    message = substitute(message_param)
     report().log(message)
 
 # Context methods -------------------------------------------
 
 
 def driver() -> Remote:
     app_ctx: AppContext = data_store.spec[app_context_key]
@@ -1040,211 +1014,30 @@
 
 
 def report() -> Report:
     app_ctx: AppContext = data_store.spec[app_context_key]
     return app_ctx.report
 
 
-def image_path() -> ImagePath:
-    app_ctx: AppContext = data_store.spec[app_context_key]
-    return app_ctx.image_path
-
-
-def images() -> Images:
-    app_ctx: AppContext = data_store.spec[app_context_key]
-    return app_ctx.images
-
-
 # Private methods -------------------------------------------
 
-
-def _substitute(gauge_param: str) -> str:
-    """Substitutes placeholders in a step parameter with values from environment variables
-    and evaluates mathematical expressions.
-    The environment variables are usually defined in the env/*.properties files in the gauge project
-    or are placed into the context with specific steps.
-    So the same placeholder can be replaced with different values in different environments.
-    Examples:
-    * Open "${homepage_url}/home"
-    * Assert "id" = "sum" equals "#{5 + 6}"
-    * Assert "id" = "sum" equals "#{5 + $addend}"
-    In the first example, the placeholder `homepage_url` will be substituted by the environment variable with the same name.
-    The substitution of placeholders is 'safe', which means, that if no variable is found, the placeholder will be unchanged.
-    The second example shows a mathematical expression. Those expressions can throw exceptions, when they are invalid.
-    The third example shows placeholders and mathematical expressions combined.
-    Generally, placeholders are substituted first, expressions are evaluated sencond.
-    """
-    template = Template(gauge_param)
-    #pipe operator for sets does not work on windows
-    substituted = template.safe_substitute(os.environ)
-    template = Template(substituted)
-    substituted = template.safe_substitute(data_store.scenario)
-    substituted = _substitute_expressions('#', substituted, lambda expression: array2string(numexpr.evaluate(expression)) )
-    substituted = _substitute_expressions('!', substituted, lambda expression: _evaluate_expression(expression))
-    return substituted
-
-
-def _substitute_expressions(marker_char: str, text: str, evaluator: Callable[[str], str]) -> str:
-    substituted = text
-    while True:
-        start = substituted.find(marker_char + '{')
-        end = substituted.find('}', start)
-        if start < 0 or end < 0:
-            break
-        expression = substituted[start + 2:end]
-        before = substituted[0:start]
-        after = substituted[end + 1:len(substituted)]
-        value = evaluator(expression)
-        substituted = before + value + after
-    return substituted
-
-
-def _evaluate_expression(expression: str) -> str:
-    expression_lower = expression.lower()
-    if expression_lower == "uuid":
-        return str(uuid.uuid4())
-    elif expression_lower.startswith("time"):
-        if expression_lower.startswith("time:"):
-            format = expression.split(':', 2)[1]
-        elif expression_lower == "time":
-            format = None
-        else:
-            raise ValueError(f"unsupported substitute {expression}")
-        if format is None:
-            return datetime.now().isoformat()
-        else:
-            return datetime.now().strftime(format)
-    else:
-        raise ValueError(f"unsupported substitute {expression}")
-
-
-def _marker(by_string: str, by_value: str) -> tuple[str, str]:
-    mapped_by = ByMapper.map_string(by_string)
-    if mapped_by == By.ID:
-        mapped_by = By.CSS_SELECTOR
-        by_value = f"#{by_value}"
-    return mapped_by, by_value
-
-
-def _wait_until(condition: Callable[[Remote], Any]) -> Any:
-    timeout = data_store.scenario.get(timeout_key, config.get_implicit_timeout())
-    try:
-        return WebDriverWait(driver(), timeout).until(condition)
-    except TimeoutException:
-        return False
-
-
-def _find_element(by_param: str, by_value_param: str) -> WebElement:
-    by = _substitute(by_param)
-    by_value = _substitute(by_value_param)
-    marker = _marker(by, by_value)
-    return driver().find_element(*marker)
-
-
-def _find_elements(by_param: str, by_value_param: str) -> List[WebElement]:
-    by = _substitute(by_param)
-    by_value = _substitute(by_value_param)
-    marker = _marker(by, by_value)
-    return driver().find_elements(*marker)
-
-
-def _get_text_from_element(by: str, by_value: str) -> str:
-    element = _find_element(by, by_value)
-    if "input" == element.tag_name:
-        return element.get_attribute("value")
-    else:
-        return element.text
-
-
-def _find_attribute(by: str, by_value: str, attribute: str) -> str | bool:
-    """
-    This will return the string value of the attribute.
-    Empty attributes will return 'true', never an empty string.
-    If the attribute does not exist, it will return `False`.
-    """
-    def _element_attribute(driver: Remote) -> Any:
-        marker = _marker(_substitute(by), _substitute(by_value))
-        element = driver.find_element(*marker)
-        value = element.get_dom_attribute(attribute)
-        return value if value is not None else False
-    return _wait_until(_element_attribute)
-
-
 def _device_pixel_ratio() -> int:
     return int(driver().execute_script("return window.devicePixelRatio"))
 
 
 def _viewport_offset() -> int:
     return int(driver().execute_script("return window.pageYOffset"))
 
-
-def _map_keys(keys_param: str) -> Iterable[str]:
-    keys = re.split(r'[,\s]+', keys_param)
-    unknown_keys = [k for k in keys if k not in KeyMapper._KEYS]
-    assert len(unknown_keys) == 0,\
-        "Keys %s unknown.\nUse those instead: %s" % (unknown_keys, KeyMapper._KEYS)
-    send_keys = [KeyMapper.map_string(k) for k in keys]
-    return send_keys
-
-
-def _scroll() -> int:
-    """
-    Scrolls down the size of the current window height and returns True, if scrolling down is still possible
-    (The page is not ended yet)
-    """
-    current_offset: int = driver().execute_script("return window.pageYOffset")
-    driver().execute_script("window.scrollBy(0, window.innerHeight)")
-    time.sleep(0.3)
-    after_scroll_offset: int = driver().execute_script("return window.pageYOffset")
-    return after_scroll_offset > current_offset
-
-
 def _is_firefox_page_screenshot_no_scrolling() -> bool:
     return config.get_browser() == Browser.FIREFOX and config.is_whole_page_screenshot()
 
 
 def _is_mobile_operating_system() -> bool:
     return config.get_operating_system().is_mobile()
 
 
-def _ssim_screenshot_noscrolling(image_file_name: str, threshold: float) -> Iterable[str]:
-    failed_asserts = []
-    actual_screenshot_full_path = image_path().create_actual_screenshot_file_path(image_file_name)
-    driver().save_full_page_screenshot(actual_screenshot_full_path)
-    expected_screenshot_full_path = image_path().create_expected_screenshot_file_path(image_file_name)
-    if not os.path.isfile(expected_screenshot_full_path):
-        failed_asserts.append("screenshot {} does not exist".format(expected_screenshot_full_path))
-    else:
-        _append_structured_similarity(failed_asserts, expected_screenshot_full_path, actual_screenshot_full_path, threshold)
-    return failed_asserts
-
-
-def _ssim_screenshot_scrolling(image_file_name: str, threshold: float) -> Iterable[str]:
-    failed_asserts = []
-    postfix = 1
-    should_continue = True
-    while should_continue:
-        actual_screenshot_full_path = image_path().create_actual_screenshot_file_path(image_file_name, postfix)
-        driver().save_screenshot(actual_screenshot_full_path)
-        expected_screenshot_full_path = image_path().create_expected_screenshot_file_path(image_file_name, postfix)
-        should_continue = _scroll() and postfix <= 32
-        postfix += 1
-        if not os.path.isfile(expected_screenshot_full_path):
-            failed_asserts.append("screenshot {} does not exist".format(expected_screenshot_full_path))
-        else:
-            _append_structured_similarity(failed_asserts, expected_screenshot_full_path, actual_screenshot_full_path, threshold)
-    return failed_asserts
-
-
-def _append_structured_similarity(asserts: list, expected_screenshot: str, actual_screenshot: str, threshold: float) -> Iterable[str]:
-    diff_formats = config.get_diff_formats()
-    ssim = images().adapt_and_compare_images(expected_screenshot, actual_screenshot, diff_formats)
-    if ssim < threshold:
-        asserts.append("SSIM {} is less than threshold {} for {}".format(ssim, threshold, actual_screenshot))
-
-
 def _focused_element() -> WebElement:
     return driver().switch_to.active_element
 
 
 def _err_msg(default_msg: str) -> str:
     return str(data_store.scenario.get(error_message_key, default_msg))
```

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/PKG-INFO` & `gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.59
+Version: 0.60
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -100,15 +100,15 @@
 
 Mathematical expressions can also be evaluated. For example: `#{5 + 5 * 5}` is evaluated to `30`.
 
 It is possible to combine the two features. Placeholder substitution takes place before mathematical expression evaluation.
 
 ### Functional Expressions
 
-Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted it will be use ISO format. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
+Functional expressions will generate a result during step execution. There are 2 expressions: One will generate a UUID, and the other will yield the current date and time: `!{uuid}`, `!{time}`, `!{time:%Y-%m-%d}`. The time format is optional, if omitted ISO format will be used. The time format pattern is described in the [Python language documentation](https://docs.python.org/3.10/library/time.html#time.strftime).
 
 ### Expression Examples
 
 Note that the property expressions start with `$`, mathematical expressions with `#`, and functional expressions with `!`.
 
 > \* Open "\${homepage_url}/home"
```

### Comparing `gauge-web-app-steps-0.59/gauge_web_app_steps.egg-info/SOURCES.txt` & `gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENCE
 README.md
 pyproject.toml
 setup.py
 gauge_web_app_steps/__init__.py
 gauge_web_app_steps/app_context.py
 gauge_web_app_steps/bymapper.py
+gauge_web_app_steps/element_lookup.py
 gauge_web_app_steps/imagepaths.py
 gauge_web_app_steps/images.py
 gauge_web_app_steps/keymapper.py
 gauge_web_app_steps/report.py
 gauge_web_app_steps/sauce_tunnel.py
+gauge_web_app_steps/screenshot.py
 gauge_web_app_steps/selector.py
+gauge_web_app_steps/substitute.py
 gauge_web_app_steps/web_app_steps.py
 gauge_web_app_steps.egg-info/PKG-INFO
 gauge_web_app_steps.egg-info/SOURCES.txt
 gauge_web_app_steps.egg-info/dependency_links.txt
 gauge_web_app_steps.egg-info/not-zip-safe
 gauge_web_app_steps.egg-info/requires.txt
 gauge_web_app_steps.egg-info/top_level.txt
```

### Comparing `gauge-web-app-steps-0.59/setup.py` & `gauge-web-app-steps-0.60/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     long_description = long_description.replace('./docs/', 'https://github.com/IBM/gauge-web-app-steps/tree/master/docs/')
 
 setup(
     name='gauge-web-app-steps',
-    version='0.59',
+    version='0.60',
     description='Provides basic steps for a Gauge project, that runs tests with Selenium and Appium',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/IBM/gauge-web-app-steps',
     author='Tobias Lehmann',
     author_email='derdualist1@gmail.com',
     license='MIT',
     packages=['gauge_web_app_steps', 'gauge_web_app_steps.config', 'gauge_web_app_steps.driver'],
     install_requires=[
-        'Appium-Python-Client>=2.9.0',
-        'getgauge',
-        'numexpr>=2.8.1',
-        'scikit-image==0.21.0',
-        'selenium>=4.11.2',
-        'webcolors==1.11.1',
-        'webdriver-manager>=4.0.0',
+        'Appium-Python-Client==4.0.0',
+        'getgauge==0.4.2',
+        'numexpr==2.9.0',
+        'scikit-image==0.22.0',
+        'selenium==4.19.0',
+        'webcolors==1.13',
+        'webdriver-manager==4.0.1',
     ],
     zip_safe=False
 )
```

