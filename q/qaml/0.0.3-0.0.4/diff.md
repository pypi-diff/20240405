# Comparing `tmp/qaml-0.0.3.tar.gz` & `tmp/qaml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.3.tar", last modified: Tue Apr  2 21:58:54 2024, max compression
+gzip compressed data, was "qaml-0.0.4.tar", last modified: Fri Apr  5 17:33:13 2024, max compression
```

## Comparing `qaml-0.0.3.tar` & `qaml-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:58:54.723286 qaml-0.0.3/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.3/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 21:58:54.723143 qaml-0.0.3/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.3/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-02 21:58:31.000000 qaml-0.0.3/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:58:54.722301 qaml-0.0.3/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.3/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      780 2024-04-02 21:57:41.000000 qaml-0.0.3/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     7228 2024-04-02 21:26:12.000000 qaml-0.0.3/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:58:54.723004 qaml-0.0.3/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-02 21:58:54.000000 qaml-0.0.3/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-02 21:58:54.723319 qaml-0.0.3/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.287952 qaml-0.0.4/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.4/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-05 17:33:13.287789 qaml-0.0.4/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.4/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-05 17:33:08.000000 qaml-0.0.4/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.286951 qaml-0.0.4/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.4/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      780 2024-04-02 21:57:41.000000 qaml-0.0.4/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     8160 2024-04-04 15:32:11.000000 qaml-0.0.4/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-05 17:33:13.287623 qaml-0.0.4/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-05 17:33:13.000000 qaml-0.0.4/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-05 17:33:13.287987 qaml-0.0.4/setup.cfg
```

### Comparing `qaml-0.0.3/LICENSE` & `qaml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.3/PKG-INFO` & `qaml-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.3/pyproject.toml` & `qaml-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.3/qaml/__main__.py` & `qaml-0.0.4/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.3/qaml/client.py` & `qaml-0.0.4/qaml/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,47 +12,48 @@
 import requests
 
 class BaseClient:
     def __init__(self, api_key):
         self.api_key = api_key
         self.driver = None
         self.platform = None
+        self.screen_size = None
 
     def setup_driver(self):
-        pass
+        raise NotImplementedError
 
     def tap_coordinates(self, x, y):
-        pass
+        raise NotImplementedError
 
     def drag(self, startX, startY, endX, endY):
-        pass
+        raise NotImplementedError
 
     def swipe(self, direction):
-        pass
+        raise NotImplementedError
 
     def scroll(self, direction):
-        pass
+        raise NotImplementedError
 
     def type_text(self, text):
-        pass
+        raise NotImplementedError
 
     def sleep(self, duration):
         time.sleep(duration)
 
     def execute(self, script):
         screenshot = self.driver.get_screenshot_as_base64()
         PIL_image = Image.open(BytesIO(base64.b64decode(screenshot)))
         longer_side = max(PIL_image.size)
         aspect_ratio = PIL_image.size[0] / PIL_image.size[1]
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
         buffered = BytesIO()
         PIL_image.save(buffered, format="PNG")
         screenshot = base64.b64encode(buffered.getvalue()).decode("utf-8")
-        payload = {"action": script, "screen_size": self.driver.get_window_size(), "screenshot": screenshot}
+        payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot}
         response = requests.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(response.text)
         actions = response.json()
         available_functions = {
             "tap": self.tap_coordinates,
             "drag": self.drag,
             "swipe": self.swipe,
@@ -68,36 +69,45 @@
 class AndroidClient(BaseClient):
     def __init__(self, api_key, driver=None):
         super().__init__(api_key)
         self.platform = "Android"
         if driver:
             self.driver = driver
         else:
-            self.setup_driver()
+            for _ in range(3):
+                try:
+                    self.setup_driver()
+                    break
+                except:
+                    pass
+            else:
+                raise Exception("Failed to setup the driver.")
+        self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self):
         caps = {'deviceName': 'Android Device', 'automationName': 'UiAutomator2', 'autoGrantPermissions': True,
                 'newCommandTimeout': 600, 'mjpegScreenshotUrl': "http://localhost:4723/stream.mjpeg"}
         options = UiAutomator2Options().load_capabilities(caps)
         self.driver = webdriver.Remote('http://localhost:4723', options=options)
         self.driver.start_recording_screen()
         self.driver.update_settings({'waitForIdleTimeout': 0, 'shouldWaitForQuiescence': False, 'maxTypingFrequency': 60})
+        # get screenshot to test if the driver is working
+        self.driver.get_screenshot_as_base64()
 
     def tap_coordinates(self, x, y):
         self.driver.tap([(x, y)], 1)
 
     def drag(self, startX, startY, endX, endY):
         self.driver.swipe(startX, startY, endX, endY, 1)
 
     def swipe(self, direction):
-        window_size = self.driver.get_window_size()
-        left = window_size["width"] * 0.2
-        top = window_size["height"] * 0.2
-        width = window_size["width"] * 0.6
-        height = window_size["height"] * 0.6
+        left = self.window_size["width"] * 0.2
+        top = self.window_size["height"] * 0.2
+        width = self.window_size["width"] * 0.6
+        height = self.window_size["height"] * 0.6
         self.driver.execute_script("mobile: swipeGesture", {"left": left, "top": top, "width": width, "height": height, "direction": direction, "percent": 1.0})
 
     def scroll(self, direction):
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
@@ -106,27 +116,38 @@
 class IOSClient(BaseClient):
     def __init__(self, api_key, driver=None, ios_udid=None):
         super().__init__(api_key)
         self.platform = "iOS"
         if driver:
             self.driver = driver
         else:
-            self.setup_driver(ios_udid)
+            # try 3 times to setup the driver
+            for _ in range(3):
+                try:
+                    self.setup_driver(ios_udid)
+                    break
+                except:
+                    pass
+            else:
+                raise Exception("Failed to setup the driver.")
+        self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self, udid):
         options = XCUITestOptions()
         options.udid = udid
         custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
         options.load_capabilities(custom_caps)
         try:
             self.driver = webdriver.Remote('http://localhost:4723', options=options)
         except:
             self.driver = webdriver.Remote('http://localhost:4723/wd/hub', options=options)
-        self.driver.start_recording_screen()
+        self.driver.start_recording_screen(forceRestart=True)
         self.driver.update_settings({'waitForIdleTimeout': 0, 'shouldWaitForQuiescence': False, 'maxTypingFrequency': 60})
+        # get screenshot to test if the driver is working
+        self.driver.get_screenshot_as_base64()
 
     def tap_coordinates(self, x, y):
         self.driver.execute_script("mobile: tap", {"x": x, "y": y})
 
     def drag(self, startX, startY, endX, endY):
         self.driver.execute_script("mobile: dragFromToForDuration", {"fromX": startX, "fromY": startY, "toX": endX, "toY": endY, "duration": 1})
```

### Comparing `qaml-0.0.3/qaml.egg-info/PKG-INFO` & `qaml-0.0.4/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

