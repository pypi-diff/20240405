# Comparing `tmp/kebbie-0.1.2.tar.gz` & `tmp/kebbie-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kebbie-0.1.2.tar", last modified: Fri Mar 29 11:12:52 2024, max compression
+gzip compressed data, was "kebbie-0.1.3.tar", last modified: Fri Apr  5 11:59:36 2024, max compression
```

## Comparing `kebbie-0.1.2.tar` & `kebbie-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:12:52.701365 kebbie-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-29 11:12:50.000000 kebbie-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-03-29 11:12:52.701365 kebbie-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-03-29 11:12:50.000000 kebbie-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:12:52.701365 kebbie-0.1.2/kebbie/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/correctors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/gesture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/noise_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-03-29 11:12:50.000000 kebbie-0.1.2/kebbie/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:12:52.701365 kebbie-0.1.2/kebbie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 11:12:52.000000 kebbie-0.1.2/kebbie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-29 11:12:50.000000 kebbie-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 11:12:52.701365 kebbie-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-29 11:12:50.000000 kebbie-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.560562 kebbie-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 11:59:30.000000 kebbie-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-05 11:59:36.560562 kebbie-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-05 11:59:30.000000 kebbie-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.556562 kebbie-0.1.3/kebbie/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35066 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/gesture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-04-05 11:59:30.000000 kebbie-0.1.3/kebbie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:59:36.556562 kebbie-0.1.3/kebbie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 11:59:36.000000 kebbie-0.1.3/kebbie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-05 11:59:30.000000 kebbie-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:59:36.560562 kebbie-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 11:59:30.000000 kebbie-0.1.3/setup.py
```

### Comparing `kebbie-0.1.2/LICENSE` & `kebbie-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/PKG-INFO` & `kebbie-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.1.2/README.md` & `kebbie-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/__init__.py` & `kebbie-0.1.3/kebbie/__init__.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/cmd.py` & `kebbie-0.1.3/kebbie/cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,62 +3,60 @@
 import argparse
 import json
 import sys
 from typing import List
 
 from kebbie import evaluate
 from kebbie.correctors import EmulatorCorrector
-from kebbie.emulator import DEFAULT_IOS_NAME, DEFAULT_IOS_PLATFORM, Emulator
+from kebbie.emulator import Emulator
 from kebbie.utils import get_soda_dataset
 
 
 def instantiate_correctors(
-    keyboard: str, ios_name: str, ios_platform: str, fast_mode: bool = True, instantiate_emulator: bool = True
+    keyboard: str, fast_mode: bool = True, instantiate_emulator: bool = True
 ) -> List[EmulatorCorrector]:
     """Create the right correctors (with the right platform, etc...) given the
     arguments from the command line.
 
     Args:
         keyboard (str): Name fo the keyboard to load.
-        ios_name (str): (For iOS emulator only) Name of the device.
-        ios_platform (str): (For iOS emulator only) Name of the iOS version.
         fast_mode (bool, optional): If `True`, the corrector will be
             instantiated in fast mode (only AC).
         instantiate_emulator (bool, optional): If `True`, the emulators are
             instantiated (which trigger the layout detection). If `False`, only
             the corrector is instantiated, not the emulator.
 
     Returns:
         The list of created Correctors.
     """
     if keyboard in ["gboard", "tappa"]:
-        # Android keyboards can be parallel & are detected automatically
+        # Android keyboards
         return [
             EmulatorCorrector(
                 device=d,
                 platform="android",
                 keyboard=keyboard,
                 fast_mode=fast_mode,
                 instantiate_emulator=instantiate_emulator,
-                ios_name=ios_name,
-                ios_platform=ios_platform,
             )
-            for d in Emulator.get_devices()
+            for d in Emulator.get_android_devices()
         ]
     else:
-        # iOS keyboards need to specify the exact name & platform...
+        # iOS keyboards
         return [
             EmulatorCorrector(
+                device=i,
                 platform="ios",
                 keyboard=keyboard,
                 fast_mode=fast_mode,
                 instantiate_emulator=instantiate_emulator,
                 ios_name=ios_name,
                 ios_platform=ios_platform,
             )
+            for i, (ios_platform, ios_name) in enumerate(Emulator.get_ios_devices())
         ]
 
 
 def common_args(parser: argparse.ArgumentParser):
     """Add common arguments to the given parser.
 
     Args:
@@ -69,28 +67,14 @@
         "-K",
         dest="keyboard",
         type=str,
         required=True,
         choices=["gboard", "ios", "tappa"],
         help="Which keyboard, to be tested, is currently installed on the emulator.",
     )
-    parser.add_argument(
-        "--ios_name",
-        dest="ios_name",
-        type=str,
-        default=DEFAULT_IOS_NAME,
-        help="Name of the emulated device (only for iOS).",
-    )
-    parser.add_argument(
-        "--ios_platform",
-        dest="ios_platform",
-        type=str,
-        default=DEFAULT_IOS_PLATFORM,
-        help="Name of the emulated platform (only for iOS).",
-    )
 
 
 def cli():
     """Entry-point of the `kebbie` command line."""
     # create the top-level parser
     parser = argparse.ArgumentParser(description="Kebbie's command line.")
     subparsers = parser.add_subparsers(title="commands", dest="cmd")
@@ -141,28 +125,26 @@
 
     args = parser.parse_args()
 
     if args.cmd is None:
         parser.print_help(sys.stderr)
         sys.exit(1)
     elif args.cmd == "evaluate":
-        correctors = instantiate_correctors(
-            args.keyboard, args.ios_name, args.ios_platform, fast_mode=not args.all_tasks, instantiate_emulator=False
-        )
+        correctors = instantiate_correctors(args.keyboard, fast_mode=not args.all_tasks, instantiate_emulator=False)
 
         # Get dataset, and filter it to keep only a small number of sentences
         dataset = get_soda_dataset(args.n_sentences)
 
         # Run the evaluation
         results = evaluate(correctors, dataset=dataset, track_mistakes=args.track_mistakes)
 
         # Save the results in a file
         with open(args.result_file, "w", encoding="utf-8") as f:
             json.dump(results, f, ensure_ascii=False, indent=4)
 
         print("Overall score : ", results["overall_score"])
 
     elif args.cmd == "show_layout":
-        correctors = instantiate_correctors(args.keyboard, args.ios_name, args.ios_platform)
+        correctors = instantiate_correctors(args.keyboard)
         for c in correctors:
             c.emulator.show_keyboards()
             print(f"Predictions : {c.emulator.get_predictions()}")
```

### Comparing `kebbie-0.1.2/kebbie/correctors.py` & `kebbie-0.1.3/kebbie/correctors.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/emulator.py` & `kebbie-0.1.3/kebbie/emulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,14 @@
     "xcodeSigningId": "iPhone Developer",
     "useNewWDA": False,
     "usePrebuiltWdDA": True,
     "startIWDP": True,
     "bundleId": "com.apple.MobileSMS",
     "newCommandTimeout": 3600,
 }
-DEFAULT_IOS_NAME = "iPhone 15 Pro"
-DEFAULT_IOS_PLATFORM = "17.4"
 BROWSER_PAD_URL = "https://www.justnotepad.com"
 ANDROID_TYPING_FIELD_CLASS_NAME = "android.widget.EditText"
 DUMMY_RECIPIENT = "0"
 IOS_TYPING_FIELD_ID = "messageBodyField"
 IOS_START_CHAT_CLASS_NAME = "XCUIElementTypeCell"
 TESSERACT_CONFIG = "-c tessedit_char_blacklist=0123456789”:!@·$%&/()=.¿?"
 PREDICTION_DELAY = 0.4
@@ -230,29 +228,30 @@
     def __init__(
         self,
         platform: str,
         keyboard: str,
         device: str = None,
         host: str = "127.0.0.1",
         port: str = "4723",
-        ios_name: str = DEFAULT_IOS_NAME,
-        ios_platform: str = DEFAULT_IOS_PLATFORM,
+        ios_name: str = None,
+        ios_platform: str = None,
     ):
         super().__init__()
 
         self.platform = platform.lower()
         if self.platform not in [ANDROID, IOS]:
             raise ValueError(f"Unknown platform : {self.platform}. Please specify `{ANDROID}` or `{IOS}`.")
 
         # Start appium
         capabilities = ANDROID_CAPABILITIES if self.platform == ANDROID else IOS_CAPABILITIES
         if self.platform == IOS:
             capabilities["deviceName"] = ios_name
             capabilities["platformVersion"] = ios_platform
-        if device is not None:
+            capabilities["wdaLocalPort"] = 8000 + device
+        if self.platform == ANDROID and device is not None:
             capabilities["udid"] = device
         self.driver = webdriver.Remote(f"{host}:{port}", capabilities)
         self.driver.implicitly_wait(20)
 
         self.screen_size = self.driver.get_window_size()
 
         self.keyboard = keyboard.lower()
@@ -302,26 +301,55 @@
             self.typing_field = typing_fields[0]
         else:
             self.driver.find_element(By.CLASS_NAME, IOS_START_CHAT_CLASS_NAME).click()
             self.typing_field = self.driver.find_element(By.ID, IOS_TYPING_FIELD_ID)
         self.typing_field.click()
         self.typing_field.clear()
 
-    def get_devices() -> List[str]:
+    def get_android_devices() -> List[str]:
         """Static method that uses the `adb devices` command to retrieve the
         list of devices running.
 
         Returns:
             List of detected device UDID.
         """
         result = subprocess.run(["adb", "devices"], stdout=subprocess.PIPE)
         devices = result.stdout.decode().split("\n")
         devices = [d.split()[0] for d in devices if not (d.startswith("List of devices attached") or len(d) == 0)]
         return devices
 
+    def get_ios_devices() -> List[Tuple[str, str]]:
+        """Static method that uses the `xcrun simctl` command to retrieve the
+        list of booted devices.
+
+        Returns:
+            List of booted device platform and device name.
+        """
+        devices = []
+
+        result = subprocess.run(["xcrun", "simctl", "list", "devices"], stdout=subprocess.PIPE)
+        out = result.stdout.decode().split("\n")
+
+        curr_platform = ""
+        for line in out:
+            if line.startswith("== ") and line.endswith(" =="):
+                continue
+            elif line.startswith("-- ") and line.endswith(" --"):
+                curr_platform = line[3:-3]
+            else:
+                m = re.match(r"\s+([^\t]+)\s+\([A-Z0-9\-]+\)\s+\((Booted|Shutdown)\)", line)
+                if m:
+                    device_name = m.group(1)
+                    status = m.group(2)
+
+                    if status == "Booted" and curr_platform.startswith("iOS "):
+                        devices.append((curr_platform[4:], device_name))
+
+        return devices
+
     def _paste(self, text: str):
         """Paste the given text into the typing field, to quickly simulate
         typing a context.
 
         Args:
             text (str): Text to paste.
         """
@@ -626,15 +654,15 @@
         layout["numbers"] = screen_layout
 
         # Reset out keyboard to the original layer
         self.tap(layout["numbers"]["letters"], layout["keyboard_frame"])
 
         # Fix the keys' offset compared to the keyboard frame
         if self.android:
-            self.layout = self._offset_keys(layout)
+            self.layout = self._apply_status_bar_offset(layout)
         else:
             self.layout = layout
 
     def get_suggestions(self) -> List[str]:
         """Method to retrieve the keyboard suggestions from the XML tree.
 
         Note that it's slower to access the XML through methods like
@@ -670,18 +698,14 @@
         """
         layout = {}
         if keyboard_frame is None:
             if self.android:
                 # Detect the keyboard frame
                 kb = root.find_element(By.ID, "android:id/inputArea")
                 keyboard_frame = self._get_frame(kb)
-
-                # Offset the position of the keyboard frame because of the status bar
-                sb_bounds = self._get_status_bar_bounds()
-                keyboard_frame[1] -= sb_bounds[3]
             else:
                 keyboard_frame = self._get_frame(root)
 
         for key_elem in root.find_elements(By.XPATH, self.xpath_keys):
             label = self._get_label(key_elem, current_layout=current_layout)
             if label is not None:
                 layout[label] = self._get_frame(key_elem)
@@ -753,39 +777,47 @@
 
         Returns:
             Bounds of the status bar.
         """
         sb = self.driver.find_element(By.ID, "com.android.systemui:id/status_bar")
         return self._get_frame(sb)
 
-    def _offset_keys(self, layout: Dict) -> Dict:
-        """Method offsetting the keys of a given layout to fit in the keyboard
-        frame.
-
-        After auto-detecting the keys of a layout, the keys are still offset on
-        Y-axis by some amount. So just find by how much they are beyond the
-        keyboard frame, and then update them accordingly.
+    def _apply_status_bar_offset(self, layout: Dict) -> Dict:
+        """Method offsetting the given layout to match the screen.
+
+        On Android, somehow the detected positions for the keys aren't matching
+        what we see on screen. This is because of the status bar, which shift
+        everything. So, detect the status bar, and shift back the keys to the
+        right position.
 
         Args:
             layout (Dict): Layout to fix.
 
         Returns:
             Fixed layout.
         """
-        # Find the offset between the keyboard frame and the keys
-        keyboard_max_y = layout["keyboard_frame"][1] + layout["keyboard_frame"][3]
-        keys_max_y = 0
-        for k in layout["lowercase"]:
-            keys_max_y = max(keys_max_y, layout["lowercase"][k][1] + layout["lowercase"][k][3])
-        offset = layout["keyboard_frame"][1] + keys_max_y - keyboard_max_y
+        sb_bounds = self._get_status_bar_bounds()
+        dy = sb_bounds[3]
+        screen_size = layout["keyboard_frame"][1] + layout["keyboard_frame"][3]
+
+        # First of all, offset the keyboard frame
+        frame_dy1 = int(dy * (layout["keyboard_frame"][1] / screen_size))
+        frame_dy2 = int(dy * ((layout["keyboard_frame"][1] + layout["keyboard_frame"][3]) / screen_size))
+        layout["keyboard_frame"][1] -= frame_dy1
+        layout["keyboard_frame"][3] -= frame_dy2 - frame_dy1
 
-        # Update the layout considering the offset
+        # Then do the same for each keys of each layouts
         for layer in ["lowercase", "uppercase", "numbers"]:
             for k in layout[layer]:
-                layout[layer][k][1] -= offset
+                dy1 = int(dy * ((layout["keyboard_frame"][1] + layout[layer][k][1]) / screen_size))
+                dy2 = int(
+                    dy * ((layout["keyboard_frame"][1] + layout[layer][k][1] + layout[layer][k][3]) / screen_size)
+                )
+                layout[layer][k][1] -= dy1 - frame_dy1
+                layout[layer][k][3] -= dy2 - dy1
 
         return layout
 
 
 class GboardLayoutDetector(LayoutDetector):
     """Layout detector for the Gboard keyboard. See `LayoutDetector` for more
     information.
```

### Comparing `kebbie-0.1.2/kebbie/gesture.py` & `kebbie-0.1.3/kebbie/gesture.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/layout.py` & `kebbie-0.1.3/kebbie/layout.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/noise_model.py` & `kebbie-0.1.3/kebbie/noise_model.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/oracle.py` & `kebbie-0.1.3/kebbie/oracle.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/scorer.py` & `kebbie-0.1.3/kebbie/scorer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/tokenizer.py` & `kebbie-0.1.3/kebbie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie/utils.py` & `kebbie-0.1.3/kebbie/utils.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/kebbie.egg-info/PKG-INFO` & `kebbie-0.1.3/kebbie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.1.2/kebbie.egg-info/requires.txt` & `kebbie-0.1.3/kebbie.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/pyproject.toml` & `kebbie-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kebbie-0.1.2/setup.py` & `kebbie-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require["all"] = sum(extras_require.values(), [])
 extras_require["dev"] = (
     extras_require["test"] + extras_require["hook"] + extras_require["lint"] + extras_require["docs"]
 )
 
 setuptools.setup(
     name="kebbie",
-    version="0.1.2",
+    version="0.1.3",
     author="Nicolas REMOND",
     author_email="nicolas.remond@thingthing.co",
     description="A small framework to test and compare mobile keyboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FleksySDK/kebbie",
     packages=setuptools.find_packages(),
```

