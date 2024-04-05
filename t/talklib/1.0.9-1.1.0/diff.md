# Comparing `tmp/talklib-1.0.9.tar.gz` & `tmp/talklib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talklib-1.0.9.tar", last modified: Thu Feb  8 22:37:42 2024, max compression
+gzip compressed data, was "talklib-1.1.0.tar", last modified: Fri Apr  5 19:08:27 2024, max compression
```

## Comparing `talklib-1.0.9.tar` & `talklib-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-08 22:37:31.000000 talklib-1.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-08 22:37:42.233012 talklib-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-02-08 22:37:31.000000 talklib-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-08 22:37:31.000000 talklib-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 22:37:31.000000 talklib-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 22:37:42.233012 talklib-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/talklib/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/ev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)    21482 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-08 22:37:31.000000 talklib-1.0.9/src/talklib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:37:42.233012 talklib-1.0.9/src/talklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-08 22:37:42.000000 talklib-1.0.9/src/talklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:08:27.297556 talklib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-05 19:08:21.000000 talklib-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-05 19:08:27.297556 talklib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-05 19:08:21.000000 talklib-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-05 19:08:21.000000 talklib-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 19:08:21.000000 talklib-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:08:27.297556 talklib-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:08:27.293556 talklib-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:08:27.297556 talklib-1.1.0/src/talklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-05 19:08:21.000000 talklib-1.1.0/src/talklib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:08:27.297556 talklib-1.1.0/src/talklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-05 19:08:27.000000 talklib-1.1.0/src/talklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 19:08:27.000000 talklib-1.1.0/src/talklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:08:27.000000 talklib-1.1.0/src/talklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 19:08:27.000000 talklib-1.1.0/src/talklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 19:08:27.000000 talklib-1.1.0/src/talklib.egg-info/top_level.txt
```

### Comparing `talklib-1.0.9/LICENSE.txt` & `talklib-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.0.9/PKG-INFO` & `talklib-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,27 +61,29 @@
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov==4.0.0
 Requires-Dist: pytz==2022.6
 Requires-Dist: pywin32-ctypes==0.2.2
 Requires-Dist: readme-renderer==42.0
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: tomli==2.0.1
-Requires-Dist: twilio==7.15.3
+Requires-Dist: twilio==9.0.2
 Requires-Dist: twine==4.0.2
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: yarl==1.9.2
 Requires-Dist: zipp==3.17.0
 
 # talklib
 
+![tests](https://github.com/Nashville-Public-Library/talklib/actions/workflows/talklib.yml/badge.svg)
+
 ## A package to automate processing of shows/segments airing on the TL
 
 [Skip to Examples](#examples)
 
 *THIS README IS INTENDED TO ASSIST TL STAFF IN INSTALLING AND USING THIS PACKAGE*
 
 Use this module to process the following types of shows/segments:
@@ -119,32 +121,32 @@
 
 The entire list of these is in the ev.py file. Make sure to set all of these on your PC(s). They are case-sensitive!
 
 ---
 ## Installation
 
 - Open a terminal/command prompt
-- Run `pip install git+https://github.com/talkinglibrary/talklib.git`
+- Run `pip install talklib`. That's it!
     - Depending on your OS, instead of `pip` you may need to use `pip3`
     - This will install the package globally. If you're a TL user just trying to install the package for everyday use, that's likely what you want to do. If you want to install it locally (for testing, etc.), see the [development](#development) section below.
-- (you must have [Git](https://git-scm.com/) installed for this to work)
+    - If you already have it installed and need to update it to the newest version, run `pip install --upgrade talklib`
 
 ---
 
 ## About WireReady
 
 Before we begin, a general note:
 
 ### We run most of our Python scripts via WireReady (WR)
 - The "Run" command in WR defaults to running from a different directory AND a different drive letter. This causes confusion.
 - WR also does not run `.py` files by default. 
 - These are some of the reasons why we do not run `.py` files directly from WR.
 - Instead, we tell WR to run a Batch script (`.bat` file) which in turn will run the Python script (`.py` file).
 - Ensure the Batch & Python scripts are in the same directory.
-- A sample `.bat` file (`Example.bat`) is included in this repo. 
+- A sample `.bat` file (`Example.bat`) is included in the [misc](https://github.com/Nashville-Public-Library/misc/tree/main/talklib_examples) repo. 
 - PLEASE NOTE: the `.bat` file will run all Python files in the folder. This is one reason it is best to separate your Python files into different folders, each with its own `.bat` file.
 
 Here is what an example directory structure should look like:
 ````
 D:\wireready
     \Washington Post
         -WP.bat
@@ -332,15 +334,15 @@
 - executes the script with the attributes you set
 - should be the last line in your script
 
 this should be the only method/function you call directly from an outside script. Even if your IDE shows you all the available methods, please ignore them as most of them are not (yet) designed to be called directly.
 
 
 ----
-## Examples
+## Examples<a id="examples"></a>
 ### RSS Example
 
 The minimum attributes you must set are `show`, `show_filename`, and `url`.
 
 Here is an example script:
 
 ````python
@@ -348,19 +350,14 @@
 
 SD = TLShow()
 
 SD.show = 'Skywalker Daily News'
 SD.show_filename = 'SDN'
 SD.url = 'https://somesite.org/sdn-feed.rss'
 
-# these are optional
-SD.remove_yesterday = True
-SD.check_if_above = 59
-SD.check_if_below = 55
-
 SD.run()
 ````
 ---
 ### Local Example
 
 "Local" shows are shows whose files we already have downloaded ahead of time.
 
@@ -374,18 +371,14 @@
 MWB = TLShow()
 
 MWB.show = 'Magical World of Bees'
 MWB.show_filename = 'MWB'
 MWB.is_local = True
 MWB.local_file = 'D:Production\path\to\the\file.wav'
 
-# these are optional
-MWB.remove_source = True
-MBW.twilio_enable = False
-
 MWB.run()
 ````
 ----
 ### Permalink Example
 
 "Permalink" shows are shows whose audio URL does not change, E.G. PNS & Cirrus
 
@@ -399,26 +392,22 @@
 WK = TLShow()
 
 WK.show = 'Who Knows'
 WK.show_filename = 'WhoKnows'
 WK.url = 'https://somesite.org/who-knows-static'
 WK.is_permalink = True
 
-# these are optional
-WK.notifications = False
-WK.include_date = True
-
 WK.run()
 ````
 
 ### Misc. Examples
 
 Here are some examples of how to access/modify certain attributes. 
 
-### Disable Twilio
+### Disable Twilio<a id="disable-twilio"></a>
 
 To disable Twilio notifications, simply add a line like this:
 
 ````python
 from talklib import TLShow
 
 SD = TLShow()
@@ -445,30 +434,31 @@
 SD.url = 'https://somesite.org/sdn-feed.rss'
 SD.ffmpeg.compression_level = 18
 
 SD.run()
 ````
 
 -----
-## Development
+## Development<a id="development"></a>
 
 - Clone this repository
-    - `git clone https://github.com/talkinglibrary/talklib.git`
+    - `git clone https://github.com/Nashville-Public-Library/talklib.git`
 - cd into the folder
     - `cd talklib`
 - Create a virtual environment
-    - `py -m venv venv`
-    - depending on your OS, instead of `py` you may need to use `python` or `python3`
+    - `python -m venv venv`
+    - depending on your OS, instead of `python`you may need to use `py` or `python3`
 - Activate virtual environment
     - On Windows: `venv\Scripts\activate`
     - On Mac: `source venv/bin/activate`
 - Update pip
-    - `py -m pip install --upgrade pip`
+    - `pip install --upgrade pip`
     - depending on your OS, instead of `pip` you may need to run `pip3`
 - Install the package into your virtual environment
     - `pip install -e .`
 - Run Pytest
     - `pytest`
+        - to see code coverage, use `pytest --cov=talklib`
     - The tests can take a while to run. Watch the terminal output for progress.
     - If the tests fail, you may have installed something incorrectly. 
     - You must be connected to the internet to run the tests
```

### Comparing `talklib-1.0.9/README.md` & `talklib-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # talklib
 
+![tests](https://github.com/Nashville-Public-Library/talklib/actions/workflows/talklib.yml/badge.svg)
+
 ## A package to automate processing of shows/segments airing on the TL
 
 [Skip to Examples](#examples)
 
 *THIS README IS INTENDED TO ASSIST TL STAFF IN INSTALLING AND USING THIS PACKAGE*
 
 Use this module to process the following types of shows/segments:
@@ -41,32 +43,32 @@
 
 The entire list of these is in the ev.py file. Make sure to set all of these on your PC(s). They are case-sensitive!
 
 ---
 ## Installation
 
 - Open a terminal/command prompt
-- Run `pip install git+https://github.com/talkinglibrary/talklib.git`
+- Run `pip install talklib`. That's it!
     - Depending on your OS, instead of `pip` you may need to use `pip3`
     - This will install the package globally. If you're a TL user just trying to install the package for everyday use, that's likely what you want to do. If you want to install it locally (for testing, etc.), see the [development](#development) section below.
-- (you must have [Git](https://git-scm.com/) installed for this to work)
+    - If you already have it installed and need to update it to the newest version, run `pip install --upgrade talklib`
 
 ---
 
 ## About WireReady
 
 Before we begin, a general note:
 
 ### We run most of our Python scripts via WireReady (WR)
 - The "Run" command in WR defaults to running from a different directory AND a different drive letter. This causes confusion.
 - WR also does not run `.py` files by default. 
 - These are some of the reasons why we do not run `.py` files directly from WR.
 - Instead, we tell WR to run a Batch script (`.bat` file) which in turn will run the Python script (`.py` file).
 - Ensure the Batch & Python scripts are in the same directory.
-- A sample `.bat` file (`Example.bat`) is included in this repo. 
+- A sample `.bat` file (`Example.bat`) is included in the [misc](https://github.com/Nashville-Public-Library/misc/tree/main/talklib_examples) repo. 
 - PLEASE NOTE: the `.bat` file will run all Python files in the folder. This is one reason it is best to separate your Python files into different folders, each with its own `.bat` file.
 
 Here is what an example directory structure should look like:
 ````
 D:\wireready
     \Washington Post
         -WP.bat
@@ -254,15 +256,15 @@
 - executes the script with the attributes you set
 - should be the last line in your script
 
 this should be the only method/function you call directly from an outside script. Even if your IDE shows you all the available methods, please ignore them as most of them are not (yet) designed to be called directly.
 
 
 ----
-## Examples
+## Examples<a id="examples"></a>
 ### RSS Example
 
 The minimum attributes you must set are `show`, `show_filename`, and `url`.
 
 Here is an example script:
 
 ````python
@@ -270,19 +272,14 @@
 
 SD = TLShow()
 
 SD.show = 'Skywalker Daily News'
 SD.show_filename = 'SDN'
 SD.url = 'https://somesite.org/sdn-feed.rss'
 
-# these are optional
-SD.remove_yesterday = True
-SD.check_if_above = 59
-SD.check_if_below = 55
-
 SD.run()
 ````
 ---
 ### Local Example
 
 "Local" shows are shows whose files we already have downloaded ahead of time.
 
@@ -296,18 +293,14 @@
 MWB = TLShow()
 
 MWB.show = 'Magical World of Bees'
 MWB.show_filename = 'MWB'
 MWB.is_local = True
 MWB.local_file = 'D:Production\path\to\the\file.wav'
 
-# these are optional
-MWB.remove_source = True
-MBW.twilio_enable = False
-
 MWB.run()
 ````
 ----
 ### Permalink Example
 
 "Permalink" shows are shows whose audio URL does not change, E.G. PNS & Cirrus
 
@@ -321,26 +314,22 @@
 WK = TLShow()
 
 WK.show = 'Who Knows'
 WK.show_filename = 'WhoKnows'
 WK.url = 'https://somesite.org/who-knows-static'
 WK.is_permalink = True
 
-# these are optional
-WK.notifications = False
-WK.include_date = True
-
 WK.run()
 ````
 
 ### Misc. Examples
 
 Here are some examples of how to access/modify certain attributes. 
 
-### Disable Twilio
+### Disable Twilio<a id="disable-twilio"></a>
 
 To disable Twilio notifications, simply add a line like this:
 
 ````python
 from talklib import TLShow
 
 SD = TLShow()
@@ -367,30 +356,31 @@
 SD.url = 'https://somesite.org/sdn-feed.rss'
 SD.ffmpeg.compression_level = 18
 
 SD.run()
 ````
 
 -----
-## Development
+## Development<a id="development"></a>
 
 - Clone this repository
-    - `git clone https://github.com/talkinglibrary/talklib.git`
+    - `git clone https://github.com/Nashville-Public-Library/talklib.git`
 - cd into the folder
     - `cd talklib`
 - Create a virtual environment
-    - `py -m venv venv`
-    - depending on your OS, instead of `py` you may need to use `python` or `python3`
+    - `python -m venv venv`
+    - depending on your OS, instead of `python`you may need to use `py` or `python3`
 - Activate virtual environment
     - On Windows: `venv\Scripts\activate`
     - On Mac: `source venv/bin/activate`
 - Update pip
-    - `py -m pip install --upgrade pip`
+    - `pip install --upgrade pip`
     - depending on your OS, instead of `pip` you may need to run `pip3`
 - Install the package into your virtual environment
     - `pip install -e .`
 - Run Pytest
     - `pytest`
+        - to see code coverage, use `pytest --cov=talklib`
     - The tests can take a while to run. Watch the terminal output for progress.
     - If the tests fail, you may have installed something incorrectly. 
     - You must be connected to the internet to run the tests
```

### Comparing `talklib-1.0.9/pyproject.toml` & `talklib-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "talklib"
-version = "1.0.9"
+version = "1.1.0"
 description = "A package to automate processing of shows/segments airing on the TL"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 maintainers = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
@@ -18,8 +18,8 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["talklib*"]
-exclude = [".tests*"]
+exclude = [".tests*"]
```

### Comparing `talklib-1.0.9/requirements.txt` & `talklib-1.1.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 pytest==7.2.0
 pytest-cov==4.0.0
 pytz==2022.6
 pywin32-ctypes==0.2.2
 readme-renderer==42.0
-requests==2.28.1
+requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.0
 tomli==2.0.1
-twilio==7.15.3
+twilio==9.0.2
 twine==4.0.2
 urllib3==1.26.13
 yarl==1.9.2
 zipp==3.17.0
```

### Comparing `talklib-1.0.9/src/talklib/ev.py` & `talklib-1.1.0/src/talklib/ev.py`

 * *Files identical despite different names*

### Comparing `talklib-1.0.9/src/talklib/ffmpeg.py` & `talklib-1.1.0/src/talklib/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,46 +13,46 @@
         self.input_file = input_file
         self.output_file = output_file
         self.breakaway = breakaway
         self.compression_level = compression_level
         self.sample_rate = sample_rate
         self.audio_channels = audio_channels
 
-    def build_input_commands(self) -> dict:
+    def __build_input_commands(self) -> dict:
         command = {}
         command.update({'hide_banner': None})
         command.update({'loglevel': 'quiet'})
         command.update({'filename': self.input_file})
 
         return command
     
-    def build_output_commands(self) -> dict:
+    def __build_output_commands(self) -> dict:
         command = {}
         command.update({'ar': self.sample_rate})
         command.update({'ac': self.audio_channels})
         command.update({'af': f'loudnorm=I=-{self.compression_level}'})
         if self.breakaway:
             command.update({'t': self.breakaway})
         command.update({'y': None})
         command.update({'filename': self.output_file})
 
         return command
     
     def get_commands(self):
-        input_commands = self.build_input_commands()
-        output_commands = self.build_output_commands()
+        input_commands = self.__build_input_commands()
+        output_commands = self.__build_output_commands()
         stream = ffmpeg.input(**input_commands)
         stream = ffmpeg.output(stream, **output_commands)
         ffmpeg_commands = ffmpeg.get_args(stream)
         return ffmpeg_commands
 
     def convert(self):
         '''convert file with ffmpeg and return filename'''
-        input_commands = self.build_input_commands()
-        output_commands = self.build_output_commands()
+        input_commands = self.__build_input_commands()
+        output_commands = self.__build_output_commands()
         stream = ffmpeg.input(**input_commands)
         stream = ffmpeg.output(stream, **output_commands)
         ffmpeg.run(stream, capture_stdout=True)
         return self.output_file
     
     def get_length_in_minutes(self) -> float:
         duration = ffmpeg.probe(filename=self.input_file)
```

### Comparing `talklib-1.0.9/src/talklib/notify.py` & `talklib-1.1.0/src/talklib/notify.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 from email.message import EmailMessage
+from enum import Enum
 import logging
 from logging.handlers import SysLogHandler
 import smtplib
 
 from twilio.rest import Client
 
 from talklib.ev import EV
 
+class LogLevel(Enum):
+    INFO = logging.INFO
+    DEBUG = logging.DEBUG
+    WARNING = logging.WARNING
+    ERROR = logging.ERROR
+    CRITICAL = logging.CRITICAL
+
 class Syslog:
-    def __init__ (
-        self,
-        # syslog_host: str = EV().syslog_host,
-        syslog_port: int = 514,
-                  ):
+    def __init__ (self):
         self.syslog_host = EV().syslog_host
-        self.syslog_port = syslog_port
+        self.syslog_port = 514
 
-    def send_syslog_message(self, message: str):
-        my_logger = logging.getLogger('MyLogger')
-        my_logger.setLevel(logging.DEBUG)
+    def send_syslog_message(self, message: str, level: str = 'info'):
+        '''
+        Send message to Syslog server.
+        Levels: info (default), debug, warning, error, critical.
+
+        The level type and the my_logger.method() function must match!
+        '''
         handler = SysLogHandler(address=(self.syslog_host, self.syslog_port))
+
+        my_logger = logging.getLogger('MyLogger')
+        my_logger.setLevel(LogLevel[level.upper()].value)
         my_logger.addHandler(handler)
 
-        my_logger.info(message)
+        my_logger.log(level=LogLevel[level.upper()].value, msg=message)
         my_logger.removeHandler(handler) # don't forget this after you send the message!
 
 class Notify:
     def __init__ (self,
                   syslog_enable: bool = True,
                   twilio_enable: bool = True,
                   email_enable: bool = True,
@@ -34,19 +45,19 @@
         
         self.syslog_enable = syslog_enable
         self.twilio_enable = twilio_enable
         self.email_enable = email_enable
         self.syslog = Syslog()
         self.EV = EV()
 
-    def send_syslog(self, message: str) -> None:
+    def send_syslog(self, message: str, level: str) -> None:
         '''send message to syslog server'''
         if not self.syslog_enable:
             return
-        self.syslog.send_syslog_message(message=message)
+        self.syslog.send_syslog_message(message=message, level=level)
     
     def send_call(self, message: str) -> None:
         '''send voice call via twilio'''
         if self.twilio_enable:
             client = Client(self.EV.twilio_sid, self.EV.twilio_token)
 
             call = client.calls.create(
```

### Comparing `talklib-1.0.9/src/talklib/show.py` & `talklib-1.1.0/src/talklib/show.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime
 import glob
 import os
 import shutil
 import time
 import xml.etree.ElementTree as ET
 
-import ffmpeg
 import requests
 
 from talklib.ev import EV
 from talklib.notify import Notify
 from talklib.utils import get_timestamp, clear_screen, print_to_screen_and_wait, today_is_weekday
 from talklib.ffmpeg import FFMPEG
 
@@ -37,451 +36,451 @@
     def __str__(self) -> str:
         return "This is a really cool, useful thing. Calling this should give useful info. I'll come back to it. TODO"
     
     def six_digit_date_string(self) -> str:
         date = datetime.now().strftime("%m%d%y")
         return date
     
-    def create_output_filename(self) -> str:
+    def __create_output_filename(self) -> str:
         '''returns the audio filename to use depending on whether we should include the date'''
         if self.include_date:
-            date = TLShow.six_digit_date_string(self)
-            outputFile = (f"{self.show_filename}-{date}.wav")
+            date = self.six_digit_date_string()
+            output_file = (f"{self.show_filename}-{date}.wav")
         else:
-            outputFile = (f'{self.show_filename}.wav')
-        return outputFile
+            output_file = (f'{self.show_filename}.wav')
+        self.__prep_syslog(message=f'Filename will be: {output_file}')
+        return output_file
 
-    def convert(self, input):
+    def __convert(self, input):
         ffmpeg = self.ffmpeg
         ffmpeg.input_file = input
-        ffmpeg.output_file = self.create_output_filename()
-        self.prep_syslog(message='preparing to convert')
+        ffmpeg.output_file = self.__create_output_filename()
+        self.__prep_syslog(message='preparing to convert')
         ffmpeg_commands = ffmpeg.get_commands()
-        self.prep_syslog(message=f'FFmpeg commands: {ffmpeg_commands}')
+        self.__prep_syslog(message=f'FFmpeg commands: {ffmpeg_commands}')
         try:
             file = ffmpeg.convert()
-            self.prep_syslog(message='file converted successfully')
+            self.__prep_syslog(message='file converted successfully')
             return file
         except Exception as ffmpeg_exception:
-            self.send_notifications(message=ffmpeg_exception, subject='Error')
-            self.prep_syslog(message=f'conversion failed: {ffmpeg_exception}')
+            self.__send_notifications(message=f'FFmpeg error: {ffmpeg_exception}', subject='Error')
             raise Exception (ffmpeg_exception)
 
 
-    def copy_then_remove(self, fileToCopy):
+    def __copy_then_remove(self, fileToCopy):
         '''TODO explain'''
         
         for destination in self.destinations:
-            TLShow.prep_syslog(self, message=f'Copying {fileToCopy} to {destination}...')
+            self.__prep_syslog(message=f'Copying {fileToCopy} to {destination}...')
             shutil.copy(fileToCopy, destination)
 
         #this is the file we're copying, so it is the file already converted. we always want to remove this.
-        TLShow.remove(self, fileToDelete=fileToCopy, is_output_file=True)
+        self.__remove(fileToDelete=fileToCopy, is_output_file=True)
 
-    def decide_whether_to_remove(self) -> bool:
+    def __decide_whether_to_remove(self) -> bool:
         '''
         url shows should always remove the "source" files,
         since these are the files downloaded from the internet.
         local shows are downloaded ahead of time. we do not necessarily 
         want to delete these.
-        delete this line (don't ask).
         '''
         if self.url:
             return True
         elif self.local_file:
             if self.remove_source == True:
                 return True 
             else:
                 return False
 
-    def remove(self, fileToDelete, is_output_file: bool=False):
+    def __remove(self, fileToDelete, is_output_file: bool=False):
         '''TODO explain'''
-        if TLShow.decide_whether_to_remove(self) or is_output_file:
-            TLShow.prep_syslog(self, message=f'Deleting {fileToDelete}')
+        if TLShow.__decide_whether_to_remove(self) or is_output_file:
+            self.__prep_syslog(message=f'Deleting {fileToDelete}')
             try:
                 os.remove(fileToDelete)
             except Exception as e:
-                self.prep_syslog(message=e)
+                self.__prep_syslog(message=e, level='warning')
 
-    def remove_yesterday_files(self):
+    def __remove_yesterday_files(self):
         '''
         delete yesterday's files from destinations. 
         OK to use glob wildcards since there should only ever be one file
         '''
         if self.remove_yesterday:
             for destination in self.destinations:
                 matched_filenames = glob.glob(f'{destination}/{self.show_filename}*.wav')
                 if matched_filenames:
                     for file in matched_filenames:
-                        TLShow.prep_syslog(self, message=f'Deleting existing matched file: {file}')
-                        os.remove(f'{file}')
+                        self.__prep_syslog(message=f'Deleting existing matched file: {file}')
+                        os.remove(file)
                 else:
-                    TLShow.prep_syslog(self, message=f"{self.show}: Cannot find existing matched files in {destination}. Continuing...")
+                    self.__prep_syslog(message=f"{self.show}: Cannot find existing matched files in {destination}. Continuing...", level='warning')
 
-    def download_file(self):
+    def __download_file(self):
         '''
         Download audio file from RSS feed or permalink.
         If this is a permalink show, we can just use the URL. BUT
         if this is an RSS show, the URL links to an RSS feed, so 
         we need to call the function for that.
 
         please split these into separate functions, one for permalink 
         and one for RSS. or implement some other method to test against
         a user declaring URL & is_permalink with an RSS URL, which
         currently will throw an error.
         '''
         if self.is_permalink:
             download_URL = self.url
         else:
-            download_URL = TLShow.get_RSS_audio_url(self)
+            download_URL = self.__get_RSS_audio_url()
 
-        TLShow.prep_syslog(self, message=f'Attempting to download audio file.')
+        self.__prep_syslog(message=f'Attempting to download audio file.')
         input_file = 'input.mp3'  # name the file we download
         with open (input_file, mode='wb') as downloaded_file:
             a = requests.get(download_URL)
             downloaded_file.write(a.content)
             downloaded_file.close()
         
-        TLShow.prep_syslog(self, message=f'File downloaded successfully in {os.getcwd()}.')
+        self.__prep_syslog(message=f'File downloaded successfully in {os.getcwd()}.')
         return downloaded_file.name
 
     def check_downloaded_file(self, fileToCheck, how_many_attempts):
         '''TODO explain'''
         try:
             filesize = os.path.getsize(fileToCheck)
         except FileNotFoundError as error:
-            TLShow.send_notifications(self, message=f'It looks like the file does not exist. Here is the error: {error}', subject='Error')
+            self.__send_notifications(message=f'It looks like the file does not exist. Here is the error: {error}', subject='Error')
             raise FileNotFoundError
             
         is_not_empty = False
         while how_many_attempts < 3:
             if filesize > 0:
-                TLShow.prep_syslog(self, message='File is not empty. Continuing...')
+                self.__prep_syslog(message='File is not empty. Continuing...')
                 is_not_empty = True
                 return True
             else:
-                TLShow.prep_syslog(self, message=f'File is empty. Will download again. Attempt # {how_many_attempts}.')
+                self.__prep_syslog(message=f'File is empty. Will download again. Attempt # {how_many_attempts}.', level='warning')
                 how_many_attempts = how_many_attempts+1
-                TLShow.download_file(self)
-                TLShow.check_downloaded_file(self, fileToCheck=fileToCheck, how_many_attempts=how_many_attempts)
+                self.__download_file()
+                self.check_downloaded_file(fileToCheck=fileToCheck, how_many_attempts=how_many_attempts)
         if not is_not_empty:
             toSend = (
 f"There was a problem with {self.show}.\n\n\
 It looks like the downloaded file is empty. Please check manually! Yesterday's file will remain.\n\n\
 {get_timestamp()}"
 )
-            TLShow.send_notifications(self, message=toSend, subject='Error')
-            TLShow.remove(self, fileToDelete=fileToCheck)
+            self.__send_notifications(message=toSend, subject='Error')
+            self.__remove(fileToDelete=fileToCheck)
             raise Exception (toSend)
             
-    def prep_syslog(self, message: str):
+    def __prep_syslog(self, message: str, level: str = 'info'):
         '''send message to syslog server'''
         message = f'{self.show}: {message}'
-        self.notifications.send_syslog(message=message)
+        self.notifications.send_syslog(message=message, level=level)
 
 
-    def prep_send_mail(self, message: str, subject: str):
+    def __prep_send_mail(self, message: str, subject: str):
         '''send email to TL gmail account via relay address'''
         subject = f'{subject}: {self.show}'
         self.notifications.send_mail(subject=subject, message=message)
 
-    def send_sms_if_enabled(self, message: str):
+    def __send_sms_if_enabled(self, message: str):
         '''send sms via twilio IF twilio_enable is set to True'''
         self.notifications.send_sms(message=message)
 
-    def send_notifications(self, message: str, subject: str):
+    def __send_notifications(self, message: str, subject: str, syslog_level: str = 'error'):
         '''we generally only want to send SMS via Twilio if today is on a weekend'''
         if today_is_weekday():
-            TLShow.prep_send_mail(self, message=message, subject=subject)
-            TLShow.prep_syslog(self, message=message)
+            self.__prep_send_mail(message=message, subject=subject)
+            self.__prep_syslog(message=message, level=syslog_level)
         else:
-            TLShow.send_sms_if_enabled(self, message=message)
-            TLShow.prep_send_mail(self, message=message, subject=subject)
-            TLShow.prep_syslog(self, message=message)
+            self.__send_sms_if_enabled(message=message)
+            self.__prep_send_mail(message=message, subject=subject)
+            self.__prep_syslog(message=message, level=syslog_level)
 
-    def check_file_transferred(self, fileToCheck):
+    def __check_file_transferred(self, fileToCheck):
         '''check if file transferred to destination(s)'''
         numberOfDestinations = len(self.destinations) - 1
         success = False
         while numberOfDestinations >= 0:
             if os.path.isfile(f'{self.destinations[numberOfDestinations]}/{fileToCheck}'):
                 numberOfDestinations = numberOfDestinations-1
-                TLShow.prep_syslog(self, message=f'{fileToCheck} arrived at {self.destinations[numberOfDestinations]}')
+                self.__prep_syslog(message=f'{fileToCheck} arrived at {self.destinations[numberOfDestinations]}')
                 success = True
             else:
                 toSend = (f"There was a problem with {self.show}.\n\n\
 It looks like the file either wasn't converted or didn't transfer correctly. \
 Please check manually!\n\n\
 {get_timestamp()}")
-                TLShow.send_notifications(self, message=toSend, subject='Error')
+                self.__send_notifications(message=toSend, subject='Error')
                 print_to_screen_and_wait(message=toSend)
                 break
         if success:
-            TLShow.countdown(self)
+            self.__countdown()
 
-    def check_length(self, fileToCheck):
+    def __check_length(self, fileToCheck):
         '''
         Check length of converted file with ffprobe. if too long or short, send notification.
         Notice we do not raise exceptions or halt execution. This is strictly for checking/notifying and
         troubleshooting afterwards. Do not raise exceptions here.
         '''
         # if these are not declared, don't run this check.
         if not (self.check_if_below and self.check_if_above):
-            TLShow.prep_syslog(self, message='The check length function is turned off.')
-        else:
-            TLShow.prep_syslog(self, message=f'Checking whether length is between \
+            self.__prep_syslog(message='The check length function is turned off.', level='warning')
+            return
+        
+        self.__prep_syslog(message=f'Checking whether length is between \
 {self.check_if_below} and {self.check_if_above}')
 
-            duration = FFMPEG(input_file=fileToCheck).get_length_in_minutes()
+        duration = FFMPEG(input_file=fileToCheck).get_length_in_minutes()
 
-            if duration > self.check_if_above:
-                toSend = (f"Today's {self.show} is {duration} minutes long! \
+        if duration > self.check_if_above:
+            toSend = (f"Today's {self.show} is {duration} minutes long! \
 Please check manually and make edits to bring it below {self.check_if_above} minutes.\n\n\
 {get_timestamp()}")
-                TLShow.send_notifications(self, message=toSend, subject='Check Length')
+            self.__send_notifications(message=toSend, subject='Check Length', syslog_level='warning')
 
-            elif duration < self.check_if_below:
-                toSend = (f"Today's {self.show} is only {duration} minutes long! \
+        elif duration < self.check_if_below:
+            toSend = (f"Today's {self.show} is only {duration} minutes long! \
 This is unusual and could indicate a problem with the file. Please check manually!\n\n\
 {get_timestamp()}")
-                TLShow.send_notifications(self, message=toSend, subject='Check Length')
+            self.__send_notifications(message=toSend, subject='Check Length', syslog_level='warning')
 
-            else:
-                TLShow.prep_syslog(self, message=f'File is {duration} minute(s). Continuing...')
-            
-            return duration
+        else:
+            self.__prep_syslog(message=f'File is {duration} minute(s). Continuing...')
+        
+        return duration
 
-    def get_feed(self):
+    def __get_feed(self):
         '''get the feed and create an ET object, which can then be called from other functions.'''
         try:
             header = {'User-Agent': 'Darth Vader'}  # usually helpful to identify yourself
             rssfeed = requests.get(self.url, headers=header)
             rssfeed = rssfeed.text
             rssfeed = ET.fromstring(rssfeed)
             return rssfeed
         except Exception as a:
             to_send = (
 f"There's a Problem with {self.show}. It looks like the issue is with the URL/feed. \
 Here's the error: {a}\n\n\
 Is this a permalink show? Did you forget to set the is_permalink attribute?\n\n\
 {get_timestamp()}"
                 )
-            TLShow.send_notifications(self, subject='Error', message=to_send)
+            self.__send_notifications(subject='Error', message=to_send)
             raise Exception (a)
 
-    def check_feed_updated(self) -> bool:
+    def __check_feed_updated(self) -> bool:
         '''
         get the ET object from the get_feed function, 
         then parse through it to check whether there is an entry with today's date.
         If yes, return True.
 
         The format for this date is a standard format (E.G. '17 Oct 2022') set by 
         a standards organization. Most podcasts/RSS feeds follow this standard.
         '''
-        root = TLShow.get_feed(self)
-        for t in root.findall('channel'):
-            item = t.find('item')  # 'find' only returns the first match!
+        root = self.__get_feed()
+        for channel in root.findall('channel'):
+            item = channel.find('item')  # 'find' only returns the first match!
             pub_date = item.find('pubDate').text
             today = datetime.now().strftime("%a, %d %b %Y")
             if today in pub_date:
-                TLShow.prep_syslog(self, message='The feed is updated.')
+                self.__prep_syslog(message='The feed is updated.')
                 return True
 
-    def get_RSS_audio_url(self) -> str:
+    def __get_RSS_audio_url(self) -> str:
         '''TODO: explain'''
-        root = TLShow.get_feed(self)
-        for t in root.findall('channel'):
-            item = t.find('item')  # 'find' only returns the first match!
+        root = self.__get_feed()
+        for channel in root.findall('channel'):
+            item = channel.find('item')  # 'find' only returns the first match!
             audio_url = item.find('enclosure').attrib
             audio_url = audio_url.get('url')
-            TLShow.prep_syslog(self, message=f'Audio URL is: {audio_url}')
+            self.__prep_syslog(message=f'Audio URL is: {audio_url}')
             return audio_url
 
-    def check_feed_loop(self) -> str:
+    def __check_feed_loop(self) -> str:
         '''
         occasionally, the first time we check the feed, it is not showing as updated.
         It's being cached, or something...? So we are checking it 3 times, for good measure.
         '''
-        i = 0
+        count = 0
         feed_updated = False
-        while i < 3:
-            TLShow.prep_syslog(self, message=f'Attempt {i} to check feed.')
-            feed_updated = TLShow.check_feed_updated(self)
+        while count < 3:
+            self.__prep_syslog(message=f'Attempt {count} to check feed.')
+            feed_updated = self.__check_feed_updated()
             if feed_updated:
                 break
             else:
                 time.sleep(1)
-                i = i+1
+                count = count+1
         return feed_updated
 
-    def countdown(self):
+    def __countdown(self):
         '''
         the reason for this is to give a visual cue to the user
         that the script has finished and is about to exit.
         Otherwise, the user does not know what happened; they
         just see the screen disappear.
         '''
         clear_screen()
         to_send = 'All Done.'
-        TLShow.prep_syslog(self, message=to_send)
+        self.__prep_syslog(message=to_send)
         print(f'{to_send}\n')
         number = 5
         i = 0
         while i < number:
             print(f'This window will close in {number} seconds...', end='\r')
             number = number-1
             time.sleep(1)
 
-    def check_str_and_bool_type(attrib_to_check, type_to_check: str | bool, attrib_return: str):
+    def __check_str_and_bool_type(self, attrib_to_check, type_to_check: str | bool, attrib_return: str):
         '''
         we are checking whether an attribute is either type str or bool, depending on what is passed in.
         
         'attrib_return' is solely for printing the message back out to the screen/log,
         it is not needed for the actual type check.
         (I can't figure out how else to get the name of the attribute)
         '''
         if  type(attrib_to_check) != type_to_check:
             raise Exception (f"Sorry, '{attrib_return}' attribute must be type: {type_to_check}, but you used {type(attrib_to_check)}.")
 
-    def check_int_and_float_type(attrib_to_check, attrib_return: str):
+    def __check_int_and_float_type(self, attrib_to_check, attrib_return: str):
         '''
         Attributes passed here can be either int or float.
         '''
         if not (type(attrib_to_check) == int or type(attrib_to_check) == float):
             raise Exception (f'Sorry, the {attrib_return} attribute must be a valid number (without quotes).')
 
-    def check_attributes_are_valid(self):
+    def __check_attributes_are_valid(self):
         '''
         Run some checks on the attributes the user has set. I.E. the required
         attributes have been set, they are the right type, etc.
         '''
-        TLShow.prep_syslog(self, message='checking user defined attributes')
+        self.__prep_syslog(message='checking user defined attributes')
 
         if not self.show:
             raise Exception ('Sorry, you need to specify a name for the show.')
         else:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.show, type_to_check=str, attrib_return='show')
+            self.__check_str_and_bool_type(attrib_to_check=self.show, type_to_check=str, attrib_return='show')
 
         if not self.show_filename:
             raise Exception ('Sorry, you need to specify a filename for the show.')
         else:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.show_filename, type_to_check=str, attrib_return='show_filename')
+            self.__check_str_and_bool_type(attrib_to_check=self.show_filename, type_to_check=str, attrib_return='show_filename')
 
         if not self.url:
             if not self.is_local:
                 raise Exception('Sorry, you need to specify either a URL or a local file')
 
         if self.url and self.is_local:
             raise Exception ('Sorry, you cannot specify both a URL and a local audio file. You must choose only one.')
         
         if self.url and self.local_file:
             raise Exception ('Sorry, you cannot specify both a URL and a local audio file. You must choose only one.')
 
         if self.url:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.url, type_to_check=str, attrib_return='url')
+            self.__check_str_and_bool_type(attrib_to_check=self.url, type_to_check=str, attrib_return='url')
         
         if self.is_local:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.is_local, type_to_check=bool, attrib_return='is_local')
+            self.__check_str_and_bool_type(attrib_to_check=self.is_local, type_to_check=bool, attrib_return='is_local')
 
         if self.local_file:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.local_file, type_to_check=str, attrib_return='local_file')
+            self.__check_str_and_bool_type(attrib_to_check=self.local_file, type_to_check=str, attrib_return='local_file')
         
         if self.ffmpeg.breakaway:
-            TLShow.check_int_and_float_type(attrib_to_check=self.ffmpeg.breakaway, attrib_return='breakaway')
+            self.__check_int_and_float_type(attrib_to_check=self.ffmpeg.breakaway, attrib_return='breakaway')
         
         if self.ffmpeg.compression_level:
-            TLShow.check_int_and_float_type(attrib_to_check=self.ffmpeg.compression_level, attrib_return='fflevel')
+            self.__check_int_and_float_type(attrib_to_check=self.ffmpeg.compression_level, attrib_return='fflevel')
 
         if self.is_permalink:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.is_permalink, type_to_check=bool, attrib_return='is_permalink')
+            self.__check_str_and_bool_type(attrib_to_check=self.is_permalink, type_to_check=bool, attrib_return='is_permalink')
 
         if not (self.check_if_above and self.check_if_below):
             print('\n(You did not specify check_if_below and/or check_if_above. These checks will not be run.')
         
         if self.check_if_above:
-            TLShow.check_int_and_float_type(attrib_to_check=self.check_if_above, attrib_return='check_if_above')
+            self.__check_int_and_float_type(attrib_to_check=self.check_if_above, attrib_return='check_if_above')
         
         if self.check_if_below:
-            TLShow.check_int_and_float_type(attrib_to_check=self.check_if_below, attrib_return='check_if_below')
+            self.__check_int_and_float_type(attrib_to_check=self.check_if_below, attrib_return='check_if_below')
         
         if self.notifications.syslog_enable:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.notifications.syslog_enable, type_to_check=bool, attrib_return='notifications')
+            self.__check_str_and_bool_type(attrib_to_check=self.notifications.syslog_enable, type_to_check=bool, attrib_return='notifications')
 
         if self.notifications.twilio_enable:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.notifications.twilio_enable, type_to_check=bool, attrib_return='twilio_enable')
+            self.__check_str_and_bool_type(attrib_to_check=self.notifications.twilio_enable, type_to_check=bool, attrib_return='twilio_enable')
         
         if self.notifications.email_enable:
-            TLShow.check_str_and_bool_type(attrib_to_check=self.notifications.email_enable, type_to_check=bool, attrib_return='twilio_enable')
+            self.__check_str_and_bool_type(attrib_to_check=self.notifications.email_enable, type_to_check=bool, attrib_return='twilio_enable')
 
     def run(self):
         '''begins to process the file'''
 
-        TLShow.prep_syslog(self, message=f'Starting script')
+        self.__prep_syslog(message=f'Starting script')
         print(f"I'm working on {self.show}. Just a moment...\n")
 
-        TLShow.check_attributes_are_valid(self)
+        self.__check_attributes_are_valid()
 
         if self.url and self.is_permalink:
-            TLShow.prep_syslog(self, message='permalink show detected')
-            TLShow.run_URL_permalink(self)
+            self.__prep_syslog(message='permalink show detected')
+            self.__run_URL_permalink()
 
         # if url but not permalink, it must be an RSS feed...right?
         elif self.url:
-            TLShow.prep_syslog(self, message='URL show detected')
-            TLShow.run_URL_RSS(self)
+            self.__prep_syslog(message='URL show detected')
+            self.__run_URL_RSS()
 
         elif self.is_local:
-            TLShow.prep_syslog(self, message='local show detected')
-            TLShow.run_local(self)
+            self.__prep_syslog(message='local show detected')
+            self.__run_local()
                    
         else:
             raise Exception ('Sorry, something bad happened')
 
-    def run_URL_permalink(self):
+    def __run_URL_permalink(self):
         # if url is declared, it's either an RSS or permalink show
         if self.url and self.is_permalink:
-            TLShow.remove_yesterday_files(self)
-            downloaded_file = TLShow.download_file(self)
-            if TLShow.check_downloaded_file(self, fileToCheck=downloaded_file, how_many_attempts=0):
-                output_file = TLShow.convert(self, input=downloaded_file)
-            TLShow.check_length(self, fileToCheck=output_file)
-            TLShow.remove(self, fileToDelete=downloaded_file)
-            TLShow.copy_then_remove(self, fileToCopy=output_file)
-            TLShow.check_file_transferred(self, fileToCheck=output_file)
-
-    def run_URL_RSS(self):
-        if TLShow.check_feed_loop(self):
-            TLShow.remove_yesterday_files(self)
-            downloaded_file = TLShow.download_file(self)
-            if TLShow.check_downloaded_file(self, fileToCheck=downloaded_file, how_many_attempts=0):
-                output_file = TLShow.convert(self, input=downloaded_file)
-            TLShow.check_length(self, fileToCheck=output_file)
-            TLShow.remove(self, fileToDelete=downloaded_file)
-            TLShow.copy_then_remove(self, fileToCopy=output_file)
-            TLShow.check_file_transferred(self, fileToCheck=output_file)
+            self.__remove_yesterday_files()
+            downloaded_file = self.__download_file()
+            if self.check_downloaded_file(fileToCheck=downloaded_file, how_many_attempts=0):
+                output_file = self.__convert(input=downloaded_file)
+            self.__check_length(fileToCheck=output_file)
+            self.__remove(fileToDelete=downloaded_file)
+            self.__copy_then_remove(fileToCopy=output_file)
+            self.__check_file_transferred(fileToCheck=output_file)
+
+    def __run_URL_RSS(self):
+        if self.__check_feed_loop():
+            self.__remove_yesterday_files()
+            downloaded_file = self.__download_file()
+            if self.check_downloaded_file(fileToCheck=downloaded_file, how_many_attempts=0):
+                output_file = self.__convert(input=downloaded_file)
+            self.__check_length(fileToCheck=output_file)
+            self.__remove(fileToDelete=downloaded_file)
+            self.__copy_then_remove(fileToCopy=output_file)
+            self.__check_file_transferred(fileToCheck=output_file)
         else:
             toSend = (
 f"There was a problem with {self.show}.\n\n\
 It looks like today's file hasn't yet been posted. Please check and download manually! Yesterday's file will remain.\n\n\
 {get_timestamp()}"
                 )
-            TLShow.send_notifications(self, message=toSend, subject='Error')
+            self.__send_notifications(message=toSend, subject='Error')
             print_to_screen_and_wait(message=toSend)
             raise Exception
     
-    def run_local(self):
+    def __run_local(self):
         if self.local_file:
-            if TLShow.check_downloaded_file(self, fileToCheck=self.local_file, how_many_attempts=0):
-                output_file = TLShow.convert(self, input=self.local_file)
-            TLShow.check_length(self, fileToCheck=output_file)
-            TLShow.remove(self, fileToDelete=self.local_file)
-            TLShow.copy_then_remove(self, fileToCopy=output_file)
-            TLShow.check_file_transferred(self, fileToCheck=output_file)
+            if self.check_downloaded_file(fileToCheck=self.local_file, how_many_attempts=0):
+                output_file = self.__convert(input=self.local_file)
+            self.__check_length(fileToCheck=output_file)
+            self.__remove(fileToDelete=self.local_file)
+            self.__copy_then_remove(fileToCopy=output_file)
+            self.__check_file_transferred(fileToCheck=output_file)
         else:
             to_send = (
 f"There was a problem with {self.show}.\n\n\
 It looks like the source file doesn't exist. Please check manually! Yesterday's file will remain.\n\n\
 {get_timestamp()}"
                 )
-            TLShow.send_notifications(self, message=to_send, subject='Error')
+            self.__send_notifications(message=to_send, subject='Error')
             print_to_screen_and_wait(message=to_send)
             raise FileNotFoundError
```

### Comparing `talklib-1.0.9/src/talklib.egg-info/PKG-INFO` & `talklib-1.1.0/src/talklib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,27 +61,29 @@
 Requires-Dist: pyparsing==3.0.9
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.2.0
 Requires-Dist: pytest-cov==4.0.0
 Requires-Dist: pytz==2022.6
 Requires-Dist: pywin32-ctypes==0.2.2
 Requires-Dist: readme-renderer==42.0
-Requires-Dist: requests==2.28.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.0
 Requires-Dist: tomli==2.0.1
-Requires-Dist: twilio==7.15.3
+Requires-Dist: twilio==9.0.2
 Requires-Dist: twine==4.0.2
 Requires-Dist: urllib3==1.26.13
 Requires-Dist: yarl==1.9.2
 Requires-Dist: zipp==3.17.0
 
 # talklib
 
+![tests](https://github.com/Nashville-Public-Library/talklib/actions/workflows/talklib.yml/badge.svg)
+
 ## A package to automate processing of shows/segments airing on the TL
 
 [Skip to Examples](#examples)
 
 *THIS README IS INTENDED TO ASSIST TL STAFF IN INSTALLING AND USING THIS PACKAGE*
 
 Use this module to process the following types of shows/segments:
@@ -119,32 +121,32 @@
 
 The entire list of these is in the ev.py file. Make sure to set all of these on your PC(s). They are case-sensitive!
 
 ---
 ## Installation
 
 - Open a terminal/command prompt
-- Run `pip install git+https://github.com/talkinglibrary/talklib.git`
+- Run `pip install talklib`. That's it!
     - Depending on your OS, instead of `pip` you may need to use `pip3`
     - This will install the package globally. If you're a TL user just trying to install the package for everyday use, that's likely what you want to do. If you want to install it locally (for testing, etc.), see the [development](#development) section below.
-- (you must have [Git](https://git-scm.com/) installed for this to work)
+    - If you already have it installed and need to update it to the newest version, run `pip install --upgrade talklib`
 
 ---
 
 ## About WireReady
 
 Before we begin, a general note:
 
 ### We run most of our Python scripts via WireReady (WR)
 - The "Run" command in WR defaults to running from a different directory AND a different drive letter. This causes confusion.
 - WR also does not run `.py` files by default. 
 - These are some of the reasons why we do not run `.py` files directly from WR.
 - Instead, we tell WR to run a Batch script (`.bat` file) which in turn will run the Python script (`.py` file).
 - Ensure the Batch & Python scripts are in the same directory.
-- A sample `.bat` file (`Example.bat`) is included in this repo. 
+- A sample `.bat` file (`Example.bat`) is included in the [misc](https://github.com/Nashville-Public-Library/misc/tree/main/talklib_examples) repo. 
 - PLEASE NOTE: the `.bat` file will run all Python files in the folder. This is one reason it is best to separate your Python files into different folders, each with its own `.bat` file.
 
 Here is what an example directory structure should look like:
 ````
 D:\wireready
     \Washington Post
         -WP.bat
@@ -332,15 +334,15 @@
 - executes the script with the attributes you set
 - should be the last line in your script
 
 this should be the only method/function you call directly from an outside script. Even if your IDE shows you all the available methods, please ignore them as most of them are not (yet) designed to be called directly.
 
 
 ----
-## Examples
+## Examples<a id="examples"></a>
 ### RSS Example
 
 The minimum attributes you must set are `show`, `show_filename`, and `url`.
 
 Here is an example script:
 
 ````python
@@ -348,19 +350,14 @@
 
 SD = TLShow()
 
 SD.show = 'Skywalker Daily News'
 SD.show_filename = 'SDN'
 SD.url = 'https://somesite.org/sdn-feed.rss'
 
-# these are optional
-SD.remove_yesterday = True
-SD.check_if_above = 59
-SD.check_if_below = 55
-
 SD.run()
 ````
 ---
 ### Local Example
 
 "Local" shows are shows whose files we already have downloaded ahead of time.
 
@@ -374,18 +371,14 @@
 MWB = TLShow()
 
 MWB.show = 'Magical World of Bees'
 MWB.show_filename = 'MWB'
 MWB.is_local = True
 MWB.local_file = 'D:Production\path\to\the\file.wav'
 
-# these are optional
-MWB.remove_source = True
-MBW.twilio_enable = False
-
 MWB.run()
 ````
 ----
 ### Permalink Example
 
 "Permalink" shows are shows whose audio URL does not change, E.G. PNS & Cirrus
 
@@ -399,26 +392,22 @@
 WK = TLShow()
 
 WK.show = 'Who Knows'
 WK.show_filename = 'WhoKnows'
 WK.url = 'https://somesite.org/who-knows-static'
 WK.is_permalink = True
 
-# these are optional
-WK.notifications = False
-WK.include_date = True
-
 WK.run()
 ````
 
 ### Misc. Examples
 
 Here are some examples of how to access/modify certain attributes. 
 
-### Disable Twilio
+### Disable Twilio<a id="disable-twilio"></a>
 
 To disable Twilio notifications, simply add a line like this:
 
 ````python
 from talklib import TLShow
 
 SD = TLShow()
@@ -445,30 +434,31 @@
 SD.url = 'https://somesite.org/sdn-feed.rss'
 SD.ffmpeg.compression_level = 18
 
 SD.run()
 ````
 
 -----
-## Development
+## Development<a id="development"></a>
 
 - Clone this repository
-    - `git clone https://github.com/talkinglibrary/talklib.git`
+    - `git clone https://github.com/Nashville-Public-Library/talklib.git`
 - cd into the folder
     - `cd talklib`
 - Create a virtual environment
-    - `py -m venv venv`
-    - depending on your OS, instead of `py` you may need to use `python` or `python3`
+    - `python -m venv venv`
+    - depending on your OS, instead of `python`you may need to use `py` or `python3`
 - Activate virtual environment
     - On Windows: `venv\Scripts\activate`
     - On Mac: `source venv/bin/activate`
 - Update pip
-    - `py -m pip install --upgrade pip`
+    - `pip install --upgrade pip`
     - depending on your OS, instead of `pip` you may need to run `pip3`
 - Install the package into your virtual environment
     - `pip install -e .`
 - Run Pytest
     - `pytest`
+        - to see code coverage, use `pytest --cov=talklib`
     - The tests can take a while to run. Watch the terminal output for progress.
     - If the tests fail, you may have installed something incorrectly. 
     - You must be connected to the internet to run the tests
```

### Comparing `talklib-1.0.9/src/talklib.egg-info/requires.txt` & `talklib-1.1.0/src/talklib.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 pytest==7.2.0
 pytest-cov==4.0.0
 pytz==2022.6
 pywin32-ctypes==0.2.2
 readme-renderer==42.0
-requests==2.28.1
+requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.0
 tomli==2.0.1
-twilio==7.15.3
+twilio==9.0.2
 twine==4.0.2
 urllib3==1.26.13
 yarl==1.9.2
 zipp==3.17.0
```

