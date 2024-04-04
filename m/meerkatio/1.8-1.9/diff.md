# Comparing `tmp/meerkatio-1.8.tar.gz` & `tmp/meerkatio-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerkatio-1.8.tar", last modified: Fri Mar 29 23:12:06 2024, max compression
+gzip compressed data, was "meerkatio-1.9.tar", last modified: Thu Apr  4 22:30:20 2024, max compression
```

## Comparing `meerkatio-1.8.tar` & `meerkatio-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-03-29 23:12:06.930779 meerkatio-1.8/
--rw-r--r--   0 808cleanups   (501) staff       (20)    35148 2024-03-29 23:00:11.000000 meerkatio-1.8/LICENSE
--rw-r--r--   0 808cleanups   (501) staff       (20)    43069 2024-03-29 23:12:06.930609 meerkatio-1.8/PKG-INFO
-drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-03-29 23:12:06.928142 meerkatio-1.8/meerkat/
--rw-r--r--   0 808cleanups   (501) staff       (20)     2093 2024-03-29 23:10:31.000000 meerkatio-1.8/meerkat/__init__.py
--rw-r--r--   0 808cleanups   (501) staff       (20)      640 2024-03-05 07:40:37.000000 meerkatio-1.8/meerkat/api.py
--rw-r--r--   0 808cleanups   (501) staff       (20)      894 2024-03-29 23:10:56.000000 meerkatio-1.8/meerkat/cli.py
-drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-03-29 23:12:06.928508 meerkatio-1.8/meerkat/ping_sounds/
--rw-r--r--   0 808cleanups   (501) staff       (20)    21359 2024-03-05 07:06:55.000000 meerkatio-1.8/meerkat/ping_sounds/default_ping.mp3
-drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-03-29 23:12:06.930038 meerkatio-1.8/meerkatio.egg-info/
--rw-r--r--   0 808cleanups   (501) staff       (20)    43069 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/PKG-INFO
--rw-r--r--   0 808cleanups   (501) staff       (20)      338 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/SOURCES.txt
--rw-r--r--   0 808cleanups   (501) staff       (20)        1 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/dependency_links.txt
--rw-r--r--   0 808cleanups   (501) staff       (20)       48 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/entry_points.txt
--rw-r--r--   0 808cleanups   (501) staff       (20)       23 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/requires.txt
--rw-r--r--   0 808cleanups   (501) staff       (20)        8 2024-03-29 23:12:06.000000 meerkatio-1.8/meerkatio.egg-info/top_level.txt
--rw-r--r--   0 808cleanups   (501) staff       (20)       38 2024-03-29 23:12:06.930825 meerkatio-1.8/setup.cfg
--rw-r--r--   0 808cleanups   (501) staff       (20)      696 2024-03-29 23:12:04.000000 meerkatio-1.8/setup.py
-drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-03-29 23:12:06.930186 meerkatio-1.8/tests/
--rw-r--r--   0 808cleanups   (501) staff       (20)       65 2024-02-19 07:04:14.000000 meerkatio-1.8/tests/test_meerkat_notification.py
+drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-04-04 22:30:20.110752 meerkatio-1.9/
+-rw-r--r--   0 808cleanups   (501) staff       (20)    35148 2024-03-29 23:00:11.000000 meerkatio-1.9/LICENSE
+-rw-r--r--   0 808cleanups   (501) staff       (20)    43228 2024-04-04 22:30:20.110568 meerkatio-1.9/PKG-INFO
+drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-04-04 22:30:20.108421 meerkatio-1.9/meerkat/
+-rw-r--r--   0 808cleanups   (501) staff       (20)     2258 2024-04-04 06:52:15.000000 meerkatio-1.9/meerkat/__init__.py
+-rw-r--r--   0 808cleanups   (501) staff       (20)      760 2024-04-04 05:18:01.000000 meerkatio-1.9/meerkat/api.py
+-rw-r--r--   0 808cleanups   (501) staff       (20)      981 2024-04-04 05:15:51.000000 meerkatio-1.9/meerkat/cli.py
+drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-04-04 22:30:20.108777 meerkatio-1.9/meerkat/ping_sounds/
+-rw-r--r--   0 808cleanups   (501) staff       (20)    21359 2024-03-05 07:06:55.000000 meerkatio-1.9/meerkat/ping_sounds/default_ping.mp3
+drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-04-04 22:30:20.109974 meerkatio-1.9/meerkatio.egg-info/
+-rw-r--r--   0 808cleanups   (501) staff       (20)    43228 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/PKG-INFO
+-rw-r--r--   0 808cleanups   (501) staff       (20)      338 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/SOURCES.txt
+-rw-r--r--   0 808cleanups   (501) staff       (20)        1 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/dependency_links.txt
+-rw-r--r--   0 808cleanups   (501) staff       (20)       48 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/entry_points.txt
+-rw-r--r--   0 808cleanups   (501) staff       (20)       23 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/requires.txt
+-rw-r--r--   0 808cleanups   (501) staff       (20)        8 2024-04-04 22:30:20.000000 meerkatio-1.9/meerkatio.egg-info/top_level.txt
+-rw-r--r--   0 808cleanups   (501) staff       (20)       38 2024-04-04 22:30:20.110797 meerkatio-1.9/setup.cfg
+-rw-r--r--   0 808cleanups   (501) staff       (20)      696 2024-04-04 22:27:25.000000 meerkatio-1.9/setup.py
+drwxr-xr-x   0 808cleanups   (501) staff       (20)        0 2024-04-04 22:30:20.110128 meerkatio-1.9/tests/
+-rw-r--r--   0 808cleanups   (501) staff       (20)       65 2024-02-19 07:04:14.000000 meerkatio-1.9/tests/test_meerkat_notification.py
```

### Comparing `meerkatio-1.8/LICENSE` & `meerkatio-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meerkatio-1.8/PKG-INFO` & `meerkatio-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerkatio
-Version: 1.8
+Version: 1.9
 Summary: Simple notification tool for multi-tasking developers
 Author: MeerkatIO
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MeerkatIO Documentation
 
 ## Introduction
 
-Welcome to the MeerkatIO documentation. MeerkatIO is a powerful command line interface (CLI) and Python module designed to help developers step away from their computer while their code is running.
+Welcome to the [MeerkatIO](https://www.meerkatio.com/)
+ documentation. [MeerkatIO](https://www.meerkatio.com/) is a powerful command line interface (CLI) and Python module designed to help developers step away from their computer while their code is running.
 
 ## Meerkat Python SDK
 
 ### Installation
 
 ```bash
 # PyPi
@@ -719,15 +720,15 @@
 output = build_model()
 meerkat.email(f"""
 	Send a multi-line email with the output of a function:
 	{output}
 """)
 
 # Send SMS message when the script is finished
-%sms "Script completed!"
+meerkat.sms("Script completed!")
 ```
 
 ### Jupyter Notebook Example
 
 ```python
 %load_ext meerkat
 
@@ -752,15 +753,15 @@
 ```bash
 # PyPi
 $ pip3 install meerkatio
 ```
 
 ### Authenticating
 
-After creating an account at MeerkatIO you can use the same account credentials to authenticate the CLI, giving you access to the full suite of MeerkatIO services. No authentication is required to use the free Ping feature of MeerkatIO.
+After creating an account at [MeerkatIO](https://www.meerkatio.com/) you can use the same account credentials to authenticate the CLI, giving you access to the full suite of [MeerkatIO](https://www.meerkatio.com/) services. No authentication is required to use the free Ping feature of [MeerkatIO](https://www.meerkatio.com/).
 
 ```bash
 $ meerkat login
 ```
 
 ### CLI Examples
```

### Comparing `meerkatio-1.8/meerkat/__init__.py` & `meerkatio-1.9/meerkat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,43 +24,40 @@
         os.system(f'aplay {file_name}')
     elif system == 'Windows':
         os.system(f'powershell -c "(New-Object Media.SoundPlayer \'{file_name}\').PlaySync();"')
     else:
         print('Unsupported operating system.')
 
 #
-# User Management Functions
-#
-def login(email: str, password: str) -> bool:
-    token = get_user_token(email, password)
-
-    if not token:
-        print("Invalid Meerkat Token!")
-        return False
-
-    os.environ["MEERKAT_TOKEN"] = token
-    return True
-
-#
 # Notification Functions
 #
 def ping():
     sound_path = pkg_resources.resource_filename('meerkat', 'ping_sounds/default_ping.mp3')
     _play_sound(sound_path)
 
 def email(token=None, message=""):
     if token == None:
         token = os.environ.get("MEERKAT_TOKEN")
 
     if not token:
-        print("No Meerkat token found in the environment")
+        print("No MeerkatIO token found in the environment. Please login or go to https://meerkatio.com to set up your account to enable this feature.")
         return
     
     return send_meerkat_notification("email", token, message)
 
+def sms(token=None, message=""):
+    if token == None:
+        token = os.environ.get("MEERKAT_TOKEN")
+
+    if not token:
+        print("No MeerkatIO token found in the environment. Please login or go to https://meerkatio.com to set up your account to enable this feature.")
+        return
+    
+    return send_meerkat_notification("sms", token, message)
+
 #
 # iPython Extension
 #
 
 @magics_class
 class MeerkatMagics(Magics):
     @line_magic
@@ -70,16 +67,15 @@
 
     @line_magic
     def email(self, line):
         email(line)
 
     @line_magic
     def sms(self, line):
-        #TODO: send_sms(line)
-        pass
+        sms(line)
 
 try:
     # Register the magics with the notebook
     ip = get_ipython()
     ip.register_magics(MeerkatMagics)
 except:
     # not in a notebook
```

### Comparing `meerkatio-1.8/meerkat/api.py` & `meerkatio-1.9/meerkat/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import requests
 import json
 
-MEERKAT_BASE_URL = "http://127.0.0.1:5000/"
+MEERKAT_BASE_URL = "https://meerkatio.com/"
+#MEERKAT_BASE_URL = "http://127.0.0.1:5000/"
 
 def send_meerkat_notification(notification_type: str, token: str, message: str):
     response = requests.post(MEERKAT_BASE_URL + "api/notification/send", json={
         "method": notification_type,
-        "token": token,
+        "meerkat_token": token,
         "message": message
     })
-    print(response)
+    if response.status_code != 200:
+        print(f"MeerkatIO Error: {response.text}")
 
 def get_user_token(email, password):
     response = requests.post(MEERKAT_BASE_URL + "api/user/token", json={
         "email": email,
         "password": password
     })
     if response.status_code == 200:
```

### Comparing `meerkatio-1.8/meerkat/cli.py` & `meerkatio-1.9/meerkat/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import click
 import os
 
-from meerkat import email as send_email, ping as send_ping
+from meerkat import email as send_email, ping as send_ping, sms as send_sms
 from meerkat.api import get_user_token
 
 @click.group()
 def meerkat():
     pass
 
 @meerkat.command()
 def ping():
     send_ping()
 
 @meerkat.command()
 @click.argument('message', type=str)
 def email(message):
-    result = send_email(message=message)
-    click.echo(f'{result}')
+    send_email(message=message)
+
+@meerkat.command()
+@click.argument('message', type=str)
+def sms(message):
+    send_sms(message=message)
 
 @meerkat.command()
 def login():
     email = click.prompt("Enter Email")
     password = click.prompt("Enter Password", hide_input=True)
     token = get_user_token(email, password)
 
@@ -29,11 +33,11 @@
         return
 
     #save token to user HOME and set OS env
     with open(os.path.expanduser("~") + "/.meerkat", "w") as file:
         file.write(token)
     os.environ["MEERKAT_TOKEN"] = token
 
-    click.echo(f"\nMeerkat initialized successfully.")
+    click.echo(f"\nMeerkatIO initialized successfully!")
 
 if __name__ == "__main__":
     meerkat()
```

### Comparing `meerkatio-1.8/meerkat/ping_sounds/default_ping.mp3` & `meerkatio-1.9/meerkat/ping_sounds/default_ping.mp3`

 * *Files identical despite different names*

### Comparing `meerkatio-1.8/meerkatio.egg-info/PKG-INFO` & `meerkatio-1.9/meerkatio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerkatio
-Version: 1.8
+Version: 1.9
 Summary: Simple notification tool for multi-tasking developers
 Author: MeerkatIO
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,15 +680,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MeerkatIO Documentation
 
 ## Introduction
 
-Welcome to the MeerkatIO documentation. MeerkatIO is a powerful command line interface (CLI) and Python module designed to help developers step away from their computer while their code is running.
+Welcome to the [MeerkatIO](https://www.meerkatio.com/)
+ documentation. [MeerkatIO](https://www.meerkatio.com/) is a powerful command line interface (CLI) and Python module designed to help developers step away from their computer while their code is running.
 
 ## Meerkat Python SDK
 
 ### Installation
 
 ```bash
 # PyPi
@@ -719,15 +720,15 @@
 output = build_model()
 meerkat.email(f"""
 	Send a multi-line email with the output of a function:
 	{output}
 """)
 
 # Send SMS message when the script is finished
-%sms "Script completed!"
+meerkat.sms("Script completed!")
 ```
 
 ### Jupyter Notebook Example
 
 ```python
 %load_ext meerkat
 
@@ -752,15 +753,15 @@
 ```bash
 # PyPi
 $ pip3 install meerkatio
 ```
 
 ### Authenticating
 
-After creating an account at MeerkatIO you can use the same account credentials to authenticate the CLI, giving you access to the full suite of MeerkatIO services. No authentication is required to use the free Ping feature of MeerkatIO.
+After creating an account at [MeerkatIO](https://www.meerkatio.com/) you can use the same account credentials to authenticate the CLI, giving you access to the full suite of [MeerkatIO](https://www.meerkatio.com/) services. No authentication is required to use the free Ping feature of [MeerkatIO](https://www.meerkatio.com/).
 
 ```bash
 $ meerkat login
 ```
 
 ### CLI Examples
```

### Comparing `meerkatio-1.8/setup.py` & `meerkatio-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='meerkatio',
-    version='1.8',
+    version='1.9',
     packages=find_packages(),
     package_data={'meerkat': ['ping_sounds/*.mp3']},
     include_package_data=True,
     install_requires=[
         "requests",
         "click",
         "ipython"
```

