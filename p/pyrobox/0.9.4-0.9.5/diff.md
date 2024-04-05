# Comparing `tmp/pyrobox-0.9.4.tar.gz` & `tmp/pyrobox-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrobox-0.9.4.tar", last modified: Mon Mar  4 18:45:45 2024, max compression
+gzip compressed data, was "pyrobox-0.9.5.tar", last modified: Fri Apr  5 15:23:46 2024, max compression
```

## Comparing `pyrobox-0.9.4.tar` & `pyrobox-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 18:45:45.705738 pyrobox-0.9.4/
--rw-rw-rw-   0        0        0     1062 2023-10-18 07:32:00.000000 pyrobox-0.9.4/LICENSE
--rw-rw-rw-   0        0        0    12163 2024-03-04 18:45:45.704740 pyrobox-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0    10823 2024-03-03 00:29:05.000000 pyrobox-0.9.4/README.md
--rw-rw-rw-   0        0        0       90 2023-10-18 07:32:00.000000 pyrobox-0.9.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-04 18:45:45.704740 pyrobox-0.9.4/pyrobox.egg-info/
--rw-rw-rw-   0        0        0    12163 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-04 18:45:45.000000 pyrobox-0.9.4/pyrobox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1026 2024-03-04 18:45:45.705738 pyrobox-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-03-03 00:29:05.000000 pyrobox-0.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 18:45:45.703738 pyrobox-0.9.4/src/
--rw-rw-rw-   0        0        0       84 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/__init__.py
--rw-rw-rw-   0        0        0       21 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/__main__.py
--rw-rw-rw-   0        0        0     3288 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/_arg_parser.py
--rw-rw-rw-   0        0        0      105 2023-10-23 20:27:16.000000 pyrobox-0.9.4/src/_exceptions.py
--rw-rw-rw-   0        0        0    10300 2024-03-03 00:43:49.000000 pyrobox-0.9.4/src/_fs_utils.py
--rw-rw-rw-   0        0        0     6710 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/_list_maker.py
--rw-rw-rw-   0        0        0   127679 2024-03-03 00:53:28.000000 pyrobox-0.9.4/src/_page_templates.py
--rw-rw-rw-   0        0        0     8167 2024-03-04 18:36:33.000000 pyrobox-0.9.4/src/_zipfly_manager.py
--rw-rw-rw-   0        0        0     3282 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/data_types.py
--rw-rw-rw-   0        0        0    12410 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/pickledb.py
--rw-rw-rw-   0        0        0    29881 2024-03-03 00:51:37.000000 pyrobox-0.9.4/src/pyroDB.py
--rw-rw-rw-   0        0        0    59259 2024-03-04 18:19:43.000000 pyrobox-0.9.4/src/pyroboxCore.py
--rw-rw-rw-   0        0        0     7687 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/pyrobox_ServerHost.py
--rw-rw-rw-   0        0        0    41218 2024-03-04 18:42:20.000000 pyrobox-0.9.4/src/server.py
--rw-rw-rw-   0        0        0    98958 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/tabulate.py
--rw-rw-rw-   0        0        0    13985 2024-03-03 00:29:05.000000 pyrobox-0.9.4/src/user_mgmt.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:23:46.084668 pyrobox-0.9.5/
+-rw-rw-rw-   0        0        0     1083 2024-04-03 16:35:01.000000 pyrobox-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0    12163 2024-04-05 15:23:46.084668 pyrobox-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11051 2024-04-03 16:35:01.000000 pyrobox-0.9.5/README.md
+-rw-rw-rw-   0        0        0       94 2024-04-03 16:35:01.000000 pyrobox-0.9.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-05 15:23:46.083671 pyrobox-0.9.5/pyrobox.egg-info/
+-rw-rw-rw-   0        0        0    12163 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 15:23:45.000000 pyrobox-0.9.5/pyrobox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1026 2024-04-05 15:23:46.086671 pyrobox-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      276 2024-04-03 16:35:01.000000 pyrobox-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 15:23:46.081677 pyrobox-0.9.5/src/
+-rw-rw-rw-   0        0        0       88 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/__init__.py
+-rw-rw-rw-   0        0        0       22 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/__main__.py
+-rw-rw-rw-   0        0        0     3385 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/_arg_parser.py
+-rw-rw-rw-   0        0        0      109 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/_exceptions.py
+-rw-rw-rw-   0        0        0    13329 2024-04-05 15:16:27.000000 pyrobox-0.9.5/src/_fs_utils.py
+-rw-rw-rw-   0        0        0     6979 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/_list_maker.py
+-rw-rw-rw-   0        0        0   133752 2024-04-05 15:20:03.000000 pyrobox-0.9.5/src/_page_templates.py
+-rw-rw-rw-   0        0        0     8530 2024-04-03 16:35:02.000000 pyrobox-0.9.5/src/_zipfly_manager.py
+-rw-rw-rw-   0        0        0     3418 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/data_types.py
+-rw-rw-rw-   0        0        0    12962 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/pickledb.py
+-rw-rw-rw-   0        0        0    31238 2024-04-03 16:35:02.000000 pyrobox-0.9.5/src/pyroDB.py
+-rw-rw-rw-   0        0        0    61406 2024-04-05 15:18:31.000000 pyrobox-0.9.5/src/pyroboxCore.py
+-rw-rw-rw-   0        0        0     7941 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/pyrobox_ServerHost.py
+-rw-rw-rw-   0        0        0    43384 2024-04-05 15:23:09.000000 pyrobox-0.9.5/src/server.py
+-rw-rw-rw-   0        0        0   101745 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/tabulate.py
+-rw-rw-rw-   0        0        0    14547 2024-04-03 16:35:01.000000 pyrobox-0.9.5/src/user_mgmt.py
```

### Comparing `pyrobox-0.9.4/LICENSE` & `pyrobox-0.9.5/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 RaSan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 RaSan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyrobox-0.9.4/PKG-INFO` & `pyrobox-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.9.4
+Version: 0.9.5
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
 Author: Rasan
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrobox Version: 0.9.4 Summary: Personal DropBox
+Metadata-Version: 2.1 Name: pyrobox Version: 0.9.5 Summary: Personal DropBox
 for Private Network Home-page: https://github.com/RaSan147/pyrobox Author:
 Rasan Author-email: wwwqweasd147@gmail.com Project-URL: Bug Tracker, https://
 github.com/RaSan147/pyrobox/issues Project-URL: Documentation, https://
 github.com/RaSan147/pyrobox Project-URL: Source Code, https://github.com/
 RaSan147/pyrobox Project-URL: Release Notes, https://github.com/RaSan147/
 pyrobox/releases Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `pyrobox-0.9.4/README.md` & `pyrobox-0.9.5/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-# pyrobox 🔥
-
-**`Note :`** DEFAULT UPLOAD PASSWORD: `SECret`
-
-* you can change it by editing the code (see `config` class at top)
-* to set password from command line, use `-k` or `--password` flag
-
-## Status
-
-[![Downloads](https://static.pepy.tech/badge/pyrobox)](https://pepy.tech/project/pyrobox)
-
-## Requesting for more suggesions and ideas
-
-## Feel Free to Support Me
-
-<a href="https://www.buymeacoffee.com/RaSan147" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-
-## Basic FEATURES
-
-* File Hosting system (Serve files from local Storage system)
-* Access Shared File System from Multiple Devices
-* Has optional account system (Admin can add users or allow signup) (Check ***Advanced Account System*** section)
-* Set Server Permission (Check ***Customization Options*** section)
-
-## Extra FEATURES
-
-* 🔽 DOWNLOAD AND VIDEO STREAM WITH **PAUSE AND RESUME**
-* 🔼 UPLOAD WITH **PASSWORD** (User password or server-wide password)
-* 👌 HTML5 drag and drop uploader
-* 📈 MULTIPLE FILE **UPLOAD**
-* 📝 RENAME
-* 📁 FOLDER DOWNLOAD as **ZIP** (uses temp folder)
-* ⏯ Built-in VIDEO PLAYER
-* 🔁 **DELETE FILE** (MOVE TO RECYCLE BIN)
-* 🔥 PERMANENTLY DELETE
-* ⛓ `File manager` like `NAVIGATION BAR`
-* 📑 Right click Context menu (Tap n hold on touch device)
-* 🧨 RELOAD SERVER FROM REMOTE [DEBUG PURPOSE]
-* 🆕 FOLDER CREATION
-* 💬 Pop-up messages UI(from my Web leach repo)
-* 🌐 (Didn't test yet) If you are using REAL IP AND ALLOW PYTHON TO USE PUBLIC NETWORK, YOUR SERVER CAN BE VISIBLE AROUND THE GLOBE. (also vulnerable, since you can't control access *yet*)
-* 🧬 Clone entire directory from Host to Client with least changes (last modified preserved)
-* 🔜 More comming soon
-* All of these without the need of any internet connection (having connection will provide better experience)
-
-## Server side requirement
-
-* Python 3.7 or higher. Older support available.[^1]
-* Basic knowledge about Python
-* `send2trash`, `natsort` python modules
-
-[^1]: [<=3.4 compatibility] is on the way.
-
-## Installation
-
-  1. **Install Python 3.7 or higher**
-  1. **Close older pyrobox process if already running**
-  1. Install using PIP
-
-### On Windows
-
-  1. Open `CMD` or `PowerShell`
-  1. Run `pip install -U pyrobox`
-  1. Run `pyrobox` to launch the server on the Terminal Current Working Directory.
-
-### On Linux
-
-  1. Open `Terminal`
-  1. Run `pip3 install -U pyrobox`
-  1. Run `pyrobox` to launch the server on the Terminal Current Working Directory.
-
-### CHECK [FAQ](#faq) FOR FUTURE HELP AND ISSUE FIX
-
-## Customization
-
-1. Simply running the code on will create a server on `CURRENT WORKING DIRECTORY` on `Port: 6969`
-1. On browser (on device under same router/wifi network), go to `deviceIP:port_number` to see the output like this: `http://192.168.0.101:6969/`
-    * you must allow python in firewall to access network, check [FAQ](#faq) for more help
-1. To change the server running directory, 
-    * i) either edit the code  (see `config` class at top)
-    * ii) or add `-d` or `--directory` command line argument when launching the program
-        * `pyrobox -d .` to launch the server in current directory (where the file is)
-        * `pyrobox -d "D:\Server\Public folder\"`  (Use Double-Quotation while directory has space)
-        * `pyrobox -d "D:/Server/Public folder"` (Forward or backward slash really doesn't matter, unless your terminal thinks otherwise)
-1. To change port number
-    * i) just edit the code for permanent change  (see `config` class at top)
-    * ii) or add the port number at the end of the command line arg  
-        * `pyrobox 45678` # will run on port 45678
-        * `pyrobox -d . 45678` # will run on port 45678 in current directory
-
-1. To specify alternate bind address
-    * Add bind add `-bind {address}` # ie: `-bind 127.0.0.2` or `-bind 127.0.0.99`
-
-1. To change upload password
-    * i) or add `-k` or `--password` command line argument when launching the program
-        * `pyrobox -k "my new password"` to launch the server with new password
-        * `pyrobox -k ""` to launch the server without password
-        * `pyrobox` to launch the server with default password (SECret)
-    * ii) just edit the code for permanent change  (see `config` class at top)
-
-1. Optional configurations
-
-usage: `local_server_pyrobox.py [--password PASSWORD] [--no-upload] [--no-zip] [--no-update] [--no-delete] [--no-download] [--read-only] [--view-only] [--bind ADDRESS] [--directory DIRECTORY] [--version] [-h] [port]`
-
-## Positional Arguments
-
-  | arg value             | Description |
-  | --------------------- | ------------|
-  | `port`                | Specify alternate port [default: 6969] |
-
-## Options
-
-  | Flags/Arg `value`     | Description |
-  | --------------------- | ------------|
-  |--password `PASSWORD`, -k  `PASSWORD` | Upload Password (GUESTS users and Nameless server users must use it to upload files)(default: SECret)|
-  |--directory `DIRECTORY`, -d `DIRECTORY` | Specify alternative directory [default: current directory]
-  |--bind `ADDRESS`, -b `ADDRESS` | Specify alternate bind address [default: all interfaces]|
-  |--version, -v          | show program's version number and exit|
-  |-h, --help             | show this help message and exit|
-  |--no-extra-log         | Disable file path and [= + - #] based logs (default: False)|
-
-## Customization Options
-
-  | Flags                | Description |
-  | -------------------- | ------------|
-  |--no-upload, -nu      | Files can't be uploaded (default: False)|
-  |--no-zip, -nz         | Disable Folder->Zip downloading (default: False)|
-  |--no-modify, -nm      | Disable File Modification (ie: **renaming**, **overwriting existing files**) (On upload, if file exists, will add a number at the end) (default: False)|
-  |--no-delete, -nd      | Disable File Deletion (default: False)|
-  |--no-download, -ndw   | Disable File Downloading [**videos won't play either**] (default: False)|
-  |--read-only, -ro      | Read Only Mode *disables upload and any modifications ie: rename, delete* (default: False)|
-  |--view-only, -vo      | Only allowed to see file list, nothing else (default: False)|
-
-## Advanced Account System
-
-> ### You must give a `--name [Name]` and `--admin-id [USER Name]`, `--admin-pass [PASSWORD]` to create an admin account. If guest not allowed `--no-guest-allowed` User must login to access the server. You can also disable signing up `--no-signup` (Only admin can add user from admin page). Admin can also update user permission from admin page.
-
-  | Flags/Arg `value`    | Description |
-  | -------------------- | ------------|
-  |--name `NAME`, -n `NAME` | Name of the user (default: None)|
-  |--admin-id `ADMIN_ID`, -aid `ADMIN_ID` | Admin ID (default: None)|
-  |--admin-pass `ADMIN_PASS`, -ak `ADMIN_PASS` | Admin Password (default: None)|
-  |--no-signup, -ns      | Disable Signing up (Only admin can add user from admin page)(default: False)|
-  |--no-guest-allowed, -ng | Disable Guest Access (default: False)|
-
-## Account Example
-
-  1. `pyrobox -n "My Server1" -aid "admin" -ak "admin123" -k "Guest_pass"` # will allow anyone to access the server, but they must use `Guest_pass` to upload files
-  1. `pyrobox -n "My Server2" -aid "admin" -ak "admin123" -ng` # If someone wants to access the server they must sign up via signup page first. No guest allowed
-  1. `pyrobox -n "My Server3" -aid "admin" -ak "admin123" -ng -ns` # Only admin can access the server. No guest allowed, no signup allowed. Admin can add user from admin page
-
-
-## TODO
-
-* https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
-* https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
-* https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
-* check output ip and port accuracy on multiple os  
-* https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
-* Add more flags to disable specific features
-
-## Support for more features
-
-## Context menu
-
-  **Right click on any file link**
-  <img src="https://user-images.githubusercontent.com/34002411/174422718-e19d33b2-4937-47d7-bcc2-610141c1e437.jpg" width=200>
-
-## FAQ
-
-<details>
-  <summary>Using WSL, "PIP not found"</summary>
-
-  > Run this to install `pip3` and add `pip` to path
-  
-  ``` bash
-  sudo apt -y purge python3-pip
-  sudo python3 -m pip uninstall pip
-  sudo apt -y install python3-pip
-  pip3 install --upgrade pip
-  echo "export PATH=\"${HOME}/.local/bin:$PATH\"" >>"${HOME}"/.bashrc
-  ```
-
-  > Re-running the file should work.
-</details>
-
-<details>
-  <summary>Using Linux, "PIP not found"</summary>
-
-  > Run this to install `pip3`
-
-  ``` bash
-  sudo apt -y purge python3-pip
-  sudo python3 -m pip uninstall pip
-  sudo apt -y install python3-pip
-  pip3 install --upgrade pip
-  ```
-
-  > Re-running the file should work.
-</details>
-
-<details>
-  <summary>Deleted (Move to Recycle), But WHERE ARE THEY?? [on LINUX & WSL]</summary>
-  
-  > Actually the feature is working fine, unfortunately NO-GUI mode linux and WSL don't recycle bin, so you can't find it!
-  > And to make things worse, **you need to manually clear the recyle bin** from `~/.local/share/Trash`
-  > **SO I'D RECOMMAND USING DELETE PARMANENTLY**
-</details>
-
-<details>
-  <summary>Running on WINDOWS, but can't access with other device [FIREWALL]</summary>
- 
-  > You probably have **FireWall ON** and not configured.
-  > For your safety, I'd recommend you to allow Python on private network and run the server when your network is Private.
-  > IN SHORT: ALLOW PYTHON ON FIREWALL, RUN THE SERVER
- 
-  > *note: allowed on private but using public network on firewall will cause similar issue, you gotta make both same or allow python both on public and private*
-</details>
-
-## Thanks to
-
-1. https://github.com/bones7456/bones7456/blob/master/SimpleHTTPServerWithUpload.py (the guy who made upload possible)
-1. https://gist.github.com/UniIsland/3346170 (the guy who made multiple file upload possible)
-1. https://github.com/SethMMorton/natsort (sorting titles)
-1. https://github.com/sandes/zipfly (*modified* lets you see the zip progress)
-1. https://github.com/sampotts/plyr (*improved* video player)
-
-***Disclaimer***: *the owner or the programmers or any content of this repository hold no responsibility for any kind of data loss or modification on your system and do not warrenty for such actions. I tried my best to prevent all sorts of ways (that I am currently aware of) to prevent data loss or unwanted data modification. See [Data Safety Measures](/data_safety.md) taken on this projects to prevent unwanted data loss.*
+# pyrobox 🔥
+
+**`Note :`** DEFAULT UPLOAD PASSWORD: `SECret`
+
+* you can change it by editing the code (see `config` class at top)
+* to set password from command line, use `-k` or `--password` flag
+
+## Status
+
+[![Downloads](https://static.pepy.tech/badge/pyrobox)](https://pepy.tech/project/pyrobox)
+
+## Requesting for more suggesions and ideas
+
+## Feel Free to Support Me
+
+<a href="https://www.buymeacoffee.com/RaSan147" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+
+## Basic FEATURES
+
+* File Hosting system (Serve files from local Storage system)
+* Access Shared File System from Multiple Devices
+* Has optional account system (Admin can add users or allow signup) (Check ***Advanced Account System*** section)
+* Set Server Permission (Check ***Customization Options*** section)
+
+## Extra FEATURES
+
+* 🔽 DOWNLOAD AND VIDEO STREAM WITH **PAUSE AND RESUME**
+* 🔼 UPLOAD WITH **PASSWORD** (User password or server-wide password)
+* 👌 HTML5 drag and drop uploader
+* 📈 MULTIPLE FILE **UPLOAD**
+* 📝 RENAME
+* 📁 FOLDER DOWNLOAD as **ZIP** (uses temp folder)
+* ⏯ Built-in VIDEO PLAYER
+* 🔁 **DELETE FILE** (MOVE TO RECYCLE BIN)
+* 🔥 PERMANENTLY DELETE
+* ⛓ `File manager` like `NAVIGATION BAR`
+* 📑 Right click Context menu (Tap n hold on touch device)
+* 🧨 RELOAD SERVER FROM REMOTE [DEBUG PURPOSE]
+* 🆕 FOLDER CREATION
+* 💬 Pop-up messages UI(from my Web leach repo)
+* 🌐 (Didn't test yet) If you are using REAL IP AND ALLOW PYTHON TO USE PUBLIC NETWORK, YOUR SERVER CAN BE VISIBLE AROUND THE GLOBE. (also vulnerable, since you can't control access *yet*)
+* 🧬 Clone entire directory from Host to Client with least changes (last modified preserved)
+* 🔜 More comming soon
+* All of these without the need of any internet connection (having connection will provide better experience)
+
+## Server side requirement
+
+* Python 3.7 or higher. Older support available.[^1]
+* Basic knowledge about Python
+* `send2trash`, `natsort` python modules
+
+[^1]: [<=3.4 compatibility] is on the way.
+
+## Installation
+
+  1. **Install Python 3.7 or higher**
+  1. **Close older pyrobox process if already running**
+  1. Install using PIP
+
+### On Windows
+
+  1. Open `CMD` or `PowerShell`
+  1. Run `pip install -U pyrobox`
+  1. Run `pyrobox` to launch the server on the Terminal Current Working Directory.
+
+### On Linux
+
+  1. Open `Terminal`
+  1. Run `pip3 install -U pyrobox`
+  1. Run `pyrobox` to launch the server on the Terminal Current Working Directory.
+
+### CHECK [FAQ](#faq) FOR FUTURE HELP AND ISSUE FIX
+
+## Customization
+
+1. Simply running the code on will create a server on `CURRENT WORKING DIRECTORY` on `Port: 6969`
+1. On browser (on device under same router/wifi network), go to `deviceIP:port_number` to see the output like this: `http://192.168.0.101:6969/`
+    * you must allow python in firewall to access network, check [FAQ](#faq) for more help
+1. To change the server running directory, 
+    * i) either edit the code  (see `config` class at top)
+    * ii) or add `-d` or `--directory` command line argument when launching the program
+        * `pyrobox -d .` to launch the server in current directory (where the file is)
+        * `pyrobox -d "D:\Server\Public folder\"`  (Use Double-Quotation while directory has space)
+        * `pyrobox -d "D:/Server/Public folder"` (Forward or backward slash really doesn't matter, unless your terminal thinks otherwise)
+1. To change port number
+    * i) just edit the code for permanent change  (see `config` class at top)
+    * ii) or add the port number at the end of the command line arg  
+        * `pyrobox 45678` # will run on port 45678
+        * `pyrobox -d . 45678` # will run on port 45678 in current directory
+
+1. To specify alternate bind address
+    * Add bind add `-bind {address}` # ie: `-bind 127.0.0.2` or `-bind 127.0.0.99`
+
+1. To change upload password
+    * i) or add `-k` or `--password` command line argument when launching the program
+        * `pyrobox -k "my new password"` to launch the server with new password
+        * `pyrobox -k ""` to launch the server without password
+        * `pyrobox` to launch the server with default password (SECret)
+    * ii) just edit the code for permanent change  (see `config` class at top)
+
+1. Optional configurations
+
+usage: `local_server_pyrobox.py [--password PASSWORD] [--no-upload] [--no-zip] [--no-update] [--no-delete] [--no-download] [--read-only] [--view-only] [--bind ADDRESS] [--directory DIRECTORY] [--version] [-h] [port]`
+
+## Positional Arguments
+
+  | arg value             | Description |
+  | --------------------- | ------------|
+  | `port`                | Specify alternate port [default: 6969] |
+
+## Options
+
+  | Flags/Arg `value`     | Description |
+  | --------------------- | ------------|
+  |--password `PASSWORD`, -k  `PASSWORD` | Upload Password (GUESTS users and Nameless server users must use it to upload files)(default: SECret)|
+  |--directory `DIRECTORY`, -d `DIRECTORY` | Specify alternative directory [default: current directory]
+  |--bind `ADDRESS`, -b `ADDRESS` | Specify alternate bind address [default: all interfaces]|
+  |--version, -v          | show program's version number and exit|
+  |-h, --help             | show this help message and exit|
+  |--no-extra-log         | Disable file path and [= + - #] based logs (default: False)|
+
+## Customization Options
+
+  | Flags                | Description |
+  | -------------------- | ------------|
+  |--no-upload, -nu      | Files can't be uploaded (default: False)|
+  |--no-zip, -nz         | Disable Folder->Zip downloading (default: False)|
+  |--no-modify, -nm      | Disable File Modification (ie: **renaming**, **overwriting existing files**) (On upload, if file exists, will add a number at the end) (default: False)|
+  |--no-delete, -nd      | Disable File Deletion (default: False)|
+  |--no-download, -ndw   | Disable File Downloading [**videos won't play either**] (default: False)|
+  |--read-only, -ro      | Read Only Mode *disables upload and any modifications ie: rename, delete* (default: False)|
+  |--view-only, -vo      | Only allowed to see file list, nothing else (default: False)|
+
+## Advanced Account System
+
+> ### You must give a `--name [Name]` and `--admin-id [USER Name]`, `--admin-pass [PASSWORD]` to create an admin account. If guest not allowed `--no-guest-allowed` User must login to access the server. You can also disable signing up `--no-signup` (Only admin can add user from admin page). Admin can also update user permission from admin page.
+
+  | Flags/Arg `value`    | Description |
+  | -------------------- | ------------|
+  |--name `NAME`, -n `NAME` | Name of the user (default: None)|
+  |--admin-id `ADMIN_ID`, -aid `ADMIN_ID` | Admin ID (default: None)|
+  |--admin-pass `ADMIN_PASS`, -ak `ADMIN_PASS` | Admin Password (default: None)|
+  |--no-signup, -ns      | Disable Signing up (Only admin can add user from admin page)(default: False)|
+  |--no-guest-allowed, -ng | Disable Guest Access (default: False)|
+
+## Account Example
+
+  1. `pyrobox -n "My Server1" -aid "admin" -ak "admin123" -k "Guest_pass"` # will allow anyone to access the server, but they must use `Guest_pass` to upload files
+  1. `pyrobox -n "My Server2" -aid "admin" -ak "admin123" -ng` # If someone wants to access the server they must sign up via signup page first. No guest allowed
+  1. `pyrobox -n "My Server3" -aid "admin" -ak "admin123" -ng -ns` # Only admin can access the server. No guest allowed, no signup allowed. Admin can add user from admin page
+
+
+## TODO
+
+* https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
+* https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
+* https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
+* check output ip and port accuracy on multiple os  
+* https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
+* Add more flags to disable specific features
+
+## Support for more features
+
+## Context menu
+
+  **Right click on any file link**
+  <img src="https://user-images.githubusercontent.com/34002411/174422718-e19d33b2-4937-47d7-bcc2-610141c1e437.jpg" width=200>
+
+## FAQ
+
+<details>
+  <summary>Using WSL, "PIP not found"</summary>
+
+  > Run this to install `pip3` and add `pip` to path
+  
+  ``` bash
+  sudo apt -y purge python3-pip
+  sudo python3 -m pip uninstall pip
+  sudo apt -y install python3-pip
+  pip3 install --upgrade pip
+  echo "export PATH=\"${HOME}/.local/bin:$PATH\"" >>"${HOME}"/.bashrc
+  ```
+
+  > Re-running the file should work.
+</details>
+
+<details>
+  <summary>Using Linux, "PIP not found"</summary>
+
+  > Run this to install `pip3`
+
+  ``` bash
+  sudo apt -y purge python3-pip
+  sudo python3 -m pip uninstall pip
+  sudo apt -y install python3-pip
+  pip3 install --upgrade pip
+  ```
+
+  > Re-running the file should work.
+</details>
+
+<details>
+  <summary>Deleted (Move to Recycle), But WHERE ARE THEY?? [on LINUX & WSL]</summary>
+  
+  > Actually the feature is working fine, unfortunately NO-GUI mode linux and WSL don't recycle bin, so you can't find it!
+  > And to make things worse, **you need to manually clear the recyle bin** from `~/.local/share/Trash`
+  > **SO I'D RECOMMAND USING DELETE PARMANENTLY**
+</details>
+
+<details>
+  <summary>Running on WINDOWS, but can't access with other device [FIREWALL]</summary>
+ 
+  > You probably have **FireWall ON** and not configured.
+  > For your safety, I'd recommend you to allow Python on private network and run the server when your network is Private.
+  > IN SHORT: ALLOW PYTHON ON FIREWALL, RUN THE SERVER
+ 
+  > *note: allowed on private but using public network on firewall will cause similar issue, you gotta make both same or allow python both on public and private*
+</details>
+
+## Thanks to
+
+1. https://github.com/bones7456/bones7456/blob/master/SimpleHTTPServerWithUpload.py (the guy who made upload possible)
+1. https://gist.github.com/UniIsland/3346170 (the guy who made multiple file upload possible)
+1. https://github.com/SethMMorton/natsort (sorting titles)
+1. https://github.com/sandes/zipfly (*modified* lets you see the zip progress)
+1. https://github.com/sampotts/plyr (*improved* video player)
+
+***Disclaimer***: *the owner or the programmers or any content of this repository hold no responsibility for any kind of data loss or modification on your system and do not warrenty for such actions. I tried my best to prevent all sorts of ways (that I am currently aware of) to prevent data loss or unwanted data modification. See [Data Safety Measures](/data_safety.md) taken on this projects to prevent unwanted data loss.*
```

### Comparing `pyrobox-0.9.4/pyrobox.egg-info/PKG-INFO` & `pyrobox-0.9.5/pyrobox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.9.4
+Version: 0.9.5
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
 Author: Rasan
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrobox Version: 0.9.4 Summary: Personal DropBox
+Metadata-Version: 2.1 Name: pyrobox Version: 0.9.5 Summary: Personal DropBox
 for Private Network Home-page: https://github.com/RaSan147/pyrobox Author:
 Rasan Author-email: wwwqweasd147@gmail.com Project-URL: Bug Tracker, https://
 github.com/RaSan147/pyrobox/issues Project-URL: Documentation, https://
 github.com/RaSan147/pyrobox Project-URL: Source Code, https://github.com/
 RaSan147/pyrobox Project-URL: Release Notes, https://github.com/RaSan147/
 pyrobox/releases Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `pyrobox-0.9.4/pyrobox.egg-info/SOURCES.txt` & `pyrobox-0.9.5/pyrobox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrobox-0.9.4/setup.cfg` & `pyrobox-0.9.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7972 6f62 6f78 0d0a 7665 7273   = pyrobox..vers
-00000020: 696f 6e20 3d20 302e 392e 340d 0a61 7574  ion = 0.9.4..aut
+00000020: 696f 6e20 3d20 302e 392e 350d 0a61 7574  ion = 0.9.5..aut
 00000030: 686f 7220 3d20 5261 7361 6e0d 0a61 7574  hor = Rasan..aut
 00000040: 686f 725f 656d 6169 6c20 3d20 7777 7771  hor_email = wwwq
 00000050: 7765 6173 6431 3437 4067 6d61 696c 2e63  weasd147@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 5065 7273 6f6e 616c 2044 726f 7042  = Personal DropB
 00000080: 6f78 2066 6f72 2050 7269 7661 7465 204e  ox for Private N
 00000090: 6574 776f 726b 0d0a 6c6f 6e67 5f64 6573  etwork..long_des
```

### Comparing `pyrobox-0.9.4/src/_arg_parser.py` & `pyrobox-0.9.5/src/_arg_parser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-# add additional arguments to the parser
-
-# the config must be imported from pyroboxCore
-# from pyroboxCore import config
-
-def main(config):
-	config.parser.add_argument('--password', '-k',
-							default=config.PASSWORD,
-							type=str,
-							help='[Value] Upload Password (default: %(default)s)')
-
-
-
-
-	config.parser.add_argument('--name', '-n',
-							type=str,
-							default=None,
-							help='[Value] In case you want to create a server User accounts based. --password must be always same and --admin-id and --admin-pass is required. See web doc for more info.'
-								'[default: None]')
-
-	config.parser.add_argument('--admin-id', '-aid',
-							type=str,
-							default=None,
-							help='[Value] User name for admin id (In case you want to create a server User accounts based. --name and --admin-pass is required)'
-								'[default: None]')
-
-	config.parser.add_argument('--admin-pass', '-ak',
-							type=str,
-							default=None,
-							help='[Value] Password for admin id (In case you want to create a User accounts based *named server*, --name and --admin-id is required)'
-								'[default: None]')
-
-
-
-
-	config.parser.add_argument('--no-signup', '-ns',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable signup page (default: %(default)s)")
-
-
-	config.parser.add_argument('--guest-allowed', '-ga',
-							action='store_true',
-							default=True,
-							help="[Flag] Allow guests to access server when USING Account based server (default: %(default)s)")
-
-	config.parser.add_argument('--no-guest-allowed', '-ng',
-							action='store_true',
-							default=None,
-							help="[Flag] Disallow guests to access server when USING Account/Admin based server (default: %(default)s)")
-
-	config.parser.add_argument('--no-upload', '-nu',
-							action='store_true',
-							default=False,
-							help="[Flag] Files can't be uploaded (default: %(default)s)")
-
-	config.parser.add_argument('--no-zip', '-nz',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable Folder->Zip downloading (default: %(default)s)")
-
-	config.parser.add_argument('--no-modify', '-nm',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable File Modification (ie: renaming, overwriting existing files) (On upload, if file exists, will add a number at the end(default: %(default)s)")
-
-	config.parser.add_argument('--no-delete', '-nd',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable File Deletion (default: %(default)s)")
-
-	config.parser.add_argument('--no-download', '-ndw',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable File Downloading [videos won't play either] (default: %(default)s)")
-
-	config.parser.add_argument('--read-only', '-ro',
-							action='store_true',
-							default=False,
-							help='[Flag] Read Only Mode *disables upload and any modifications ie: rename, delete* (default: %(default)s)')
-
-	config.parser.add_argument('--view-only', '-vo',
-							action='store_true',
-							default=False,
-							help="[Flag] Only allowed to see file list, nothing else (default: %(default)s)")
-
-
-
-
-
-
-
-
-	# config.parser.add_argument('--no-js', '-nj',
-	# 						action='store_true',
-	# 						default=False,
-	# 						help="Disable Javascript in page(default: %(default)s)")
+# add additional arguments to the parser
+
+# the config must be imported from pyroboxCore
+# from pyroboxCore import config
+
+def main(config):
+	config.parser.add_argument('--password', '-k',
+							default=config.PASSWORD,
+							type=str,
+							help='[Value] Upload Password (default: %(default)s)')
+
+
+
+
+	config.parser.add_argument('--name', '-n',
+							type=str,
+							default=None,
+							help='[Value] In case you want to create a server User accounts based. --password must be always same and --admin-id and --admin-pass is required. See web doc for more info.'
+								'[default: None]')
+
+	config.parser.add_argument('--admin-id', '-aid',
+							type=str,
+							default=None,
+							help='[Value] User name for admin id (In case you want to create a server User accounts based. --name and --admin-pass is required)'
+								'[default: None]')
+
+	config.parser.add_argument('--admin-pass', '-ak',
+							type=str,
+							default=None,
+							help='[Value] Password for admin id (In case you want to create a User accounts based *named server*, --name and --admin-id is required)'
+								'[default: None]')
+
+
+
+
+	config.parser.add_argument('--no-signup', '-ns',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable signup page (default: %(default)s)")
+
+
+	config.parser.add_argument('--guest-allowed', '-ga',
+							action='store_true',
+							default=True,
+							help="[Flag] Allow guests to access server when USING Account based server (default: %(default)s)")
+
+	config.parser.add_argument('--no-guest-allowed', '-ng',
+							action='store_true',
+							default=None,
+							help="[Flag] Disallow guests to access server when USING Account/Admin based server (default: %(default)s)")
+
+	config.parser.add_argument('--no-upload', '-nu',
+							action='store_true',
+							default=False,
+							help="[Flag] Files can't be uploaded (default: %(default)s)")
+
+	config.parser.add_argument('--no-zip', '-nz',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable Folder->Zip downloading (default: %(default)s)")
+
+	config.parser.add_argument('--no-modify', '-nm',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable File Modification (ie: renaming, overwriting existing files) (On upload, if file exists, will add a number at the end(default: %(default)s)")
+
+	config.parser.add_argument('--no-delete', '-nd',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable File Deletion (default: %(default)s)")
+
+	config.parser.add_argument('--no-download', '-ndw',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable File Downloading [videos won't play either] (default: %(default)s)")
+
+	config.parser.add_argument('--read-only', '-ro',
+							action='store_true',
+							default=False,
+							help='[Flag] Read Only Mode *disables upload and any modifications ie: rename, delete* (default: %(default)s)')
+
+	config.parser.add_argument('--view-only', '-vo',
+							action='store_true',
+							default=False,
+							help="[Flag] Only allowed to see file list, nothing else (default: %(default)s)")
+
+
+
+
+
+
+
+
+	# config.parser.add_argument('--no-js', '-nj',
+	# 						action='store_true',
+	# 						default=False,
+	# 						help="Disable Javascript in page(default: %(default)s)")
```

### Comparing `pyrobox-0.9.4/src/_fs_utils.py` & `pyrobox-0.9.5/src/_fs_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,478 +1,582 @@
-"""
-fs_utils.py
----------------
-File System Utilities
-
-* Why using Queue and other stuffs instead of os.walk()?
-	- os.walk() is slow, and accessing its stat is slow too.
-* Why making functions with almost same functionality?
-	-  imagine a function just returns all paths, another returns sizes. Using both of them together is using a bit inefficient.
-
-* os.scandir() also caches the stat of the files, so it's faster than os.walk().
-
-# GOT FASTER SOLUTIONS?
-> Make a pull request or open an issue here: https://github.com/RaSan147/pyrobox
-> Thanks for your help!
-"""
-
-import os
-from queue import Queue
-import re
-import urllib.parse
-
-
-from ._exceptions import LimitExceed
-
-
-
-
-def get_stat(path):
-	"""
-	Get the stat of a file.
-
-	path: path to the file
-
-	* can act as check_access(path) for files
-	"""
-	try:
-		return os.stat(path)
-	except Exception:
-		return False
-
-
-def check_access(path):
-	"""
-	Check if the user has access to the file.
-
-	path: path to the file
-	"""
-	if not os.path.exists(path):
-		return False
-
-	if os.path.isfile(path):
-		try:
-			with open(path, "rb") as f:
-				f.read(1)
-
-				return True
-		except Exception:
-			return False
-	else:
-		# if folder, check if it's stat is accessible
-		return bool(get_stat(path))
-
-
-
-def walk_dir(path, yield_dir=False):
-	"""
-	Iterate through a directory and its subdirectories
-	and `yield` the filePath object of each Files and Folders*.
-
-	path: path to the directory
-	yield_dir (bool): if True yields directories too (default: False)
-	"""
-
-	Q = Queue()
-	Q.put(path)
-	while not Q.empty():
-		path = Q.get()
-
-		try:
-			dir = os.scandir(path)
-		except OSError:
-			continue
-		for entry in dir:
-			try:
-				is_dir = entry.is_dir(follow_symlinks=False)
-			except OSError as error:
-				continue
-			if is_dir:
-				Q.put(entry.path)
-
-			if yield_dir or not is_dir:
-				yield entry
-
-		dir.close()
-
-
-# TODO: can be used in search feature
-def get_tree(path, include_dir=True):
-	"""
-	returns a list of files in a directory and its subdirectories.
-	[ [full path, relative path], ... ]
-
-	path: path to the directory
-	include_dir (bool): if True returns full path, else relative path
-	"""
-	home = path
-	tree = []
-
-	# Q = Queue()
-	# Q.put(path)
-	# while not Q.empty():
-	# 	path = Q.get()
-
-	# 	try:
-	# 		dir = os.scandir(path)
-	# 	except OSError:
-	# 		continue
-	# 	for entry in dir:
-	# 		try:
-	# 			is_dir = entry.is_dir(follow_symlinks=False)
-	# 		except OSError as error:
-	# 			continue
-	# 		if is_dir:
-	# 			Q.put(entry.path)
-
-	# 		if include_dir or not is_dir:
-	# 			tree.append([entry.path, entry.path.replace(home, "", 1)])
-
-	# 	dir.close()
-
-	for entry in walk_dir(path, yield_dir=include_dir):
-		tree.append([entry.path, entry.path.replace(home, "", 1)])
-
-	return tree
-
-
-
-def _get_tree_count(path):
-	count = 0
-
-	# Q = Queue()
-	# Q.put(path)
-	# while not Q.empty():
-	# 	path = Q.get()
-
-	# 	try:
-	# 		dir = os.scandir(path)
-	# 	except OSError:
-	# 		continue
-	# 	for entry in dir:
-	# 		try:
-	# 			is_dir = entry.is_dir(follow_symlinks=False)
-	# 		except OSError as error:
-	# 			continue
-	# 		if is_dir:
-	# 			Q.put(entry.path)
-	# 		else:
-	# 			count += 1
-
-	# 	dir.close()
-
-	for entry in walk_dir(path):
-		count += 1
-
-	return count
-
-
-def get_file_count(path):
-	"""
-	Get the number of files in a directory.
-	"""
-	return _get_tree_count(path)
-
-
-def _get_tree_size(path, limit=None, must_read=False):
-	"""
-	returns the size of a directory and its subdirectories.
-
-	path: path to the directory
-	limit (int): if not None, raises LimitExceed if the size is greater than limit
-	must_read (bool): if True, reads the first byte of each file to check if it's accessible
-	"""
-	r=[] #if return_list
-	total = 0
-	start_path = path
-
-	for entry in walk_dir(path):
-		try:
-			total += entry.stat(follow_symlinks=False).st_size
-		except OSError:
-			continue
-
-		if limit and total>limit:
-			raise LimitExceed
-
-		if must_read and not check_access(entry.path):
-			continue
-
-	return total
-
-def _get_tree_path_n_size(path, limit=-1, must_read=False, path_type="full", add_dirs=False):
-	"""
-	returns a list of files[size, path] in a directory and its subdirectories.
-		[ [`path`, size], ... ]
-		> path: `path_string` | `tuple(full_path, relative_path)`
-
-	path: path to the directory
-	path_type (str): "full" or "relative" or "both"
-	"""
-	r=[] #if return_list
-	total = 0
-	start_path = path
-
-	for entry in walk_dir(path, yield_dir=add_dirs):
-		size = 0
-		if not entry.is_dir():
-			try:
-				size = entry.stat(follow_symlinks=False).st_size
-			except OSError:
-				continue
-			total += size
-
-			if limit>0 and total>limit:
-				raise LimitExceed
-
-			if must_read and not check_access(entry.path):
-				continue
-
-
-		if path_type == "full":
-			r.append([entry.path, size])
-		elif path_type == "relative":
-			r.append([entry.path.replace(start_path, "", 1), size])
-		elif path_type == "both":
-			r.append([(entry.path, entry.path.replace(start_path, "", 1)), size])
-
-	return r
-
-
-def get_dir_size(start_path = '.', limit=None, must_read=False):
-	"""
-	Get the size of a directory and all its subdirectories.
-
-	start_path: path to start calculating from
-	limit (int): maximum folder size, if bigger returns `-1`
-	return_list (bool): if True returns a tuple of (total folder size, list of contents)
-	full_dir (bool): if True returns a full path, else relative path
-	both (bool): if True returns a tuple of (total folder size, (full path, relative path))
-	must_read (bool): if True only counts files that can be read
-	"""
-
-	return _get_tree_size(start_path, limit, must_read)
-
-
-def _get_tree_count_n_size(path):
-	"""
-	Get the size of a directory and all its subdirectories.
-	returns a tuple of (`total file count`, `total folder size`)
-
-	path: path to the directory
-	"""
-	total = 0
-	count = 0
-
-	for entry in walk_dir(path):
-		try:
-			total += entry.stat(follow_symlinks=False).st_size
-		except OSError:
-			continue
-
-		count += 1
-
-	return count, total
-
-def get_tree_count_n_size(start_path):
-	"""
-	Get the size of a directory and all its subdirectories.
-	returns a tuple of (`total file count`, `total folder size`)
-
-	path: path to the directory
-	"""
-
-	return _get_tree_count_n_size(start_path)
-
-
-def fmbytes(B=0, path=''):
-	'Return the given bytes as a file manager friendly KB, MB, GB, or TB string'
-	if path:
-		stat = get_stat(path)
-		if not stat: return "Unknown"
-		B = stat.st_size
-
-	B = B
-	KB = 1024
-	MB = (KB ** 2) # 1,048,576
-	GB = (KB ** 3) # 1,073,741,824
-	TB = (KB ** 4) # 1,099,511,627,776
-
-
-	if B/TB>1:
-		return '%.2f TB  '%(B/TB)
-	if B/GB>1:
-		return '%.2f GB  '%(B/GB)
-	if B/MB>1:
-		return '%.2f MB  '%(B/MB)
-	if B/KB>1:
-		return '%.2f KB  '%(B/KB)
-	if B>1:
-		return '%i bytes'%B
-
-	return "%i byte"%B
-
-
-def humanbytes(B):
-	'Return the given bytes as a human friendly KB, MB, GB, or TB string'
-	B = B
-	KB = 1024
-	MB = (KB ** 2) # 1,048,576
-	GB = (KB ** 3) # 1,073,741,824
-	TB = (KB ** 4) # 1,099,511,627,776
-	ret=''
-
-	if B>=TB:
-		ret+= '%i TB  '%(B//TB)
-		B%=TB
-	if B>=GB:
-		ret+= '%i GB  '%(B//GB)
-		B%=GB
-	if B>=MB:
-		ret+= '%i MB  '%(B//MB)
-		B%=MB
-	if B>=KB:
-		ret+= '%i KB  '%(B//KB)
-		B%=KB
-	if B>0:
-		ret+= '%i bytes'%B
-
-	return ret
-
-def get_dir_m_time(path):
-	"""
-	Get the last modified time of a directory and all its subdirectories.
-	"""
-
-	stat = get_stat(path)
-	return stat.st_mtime if stat else 0
-
-
-
-
-
-def get_titles(path, file=False):
-	"""Make titles for the header directory
-	path: the path of the file or directory
-	file: if True, path is a file, else it's a directory
-
-	output: `Viewing NAME`"""
-
-	paths = path.split('/')
-	if file:
-		return 'Viewing ' + paths[-1]
-	if paths[-2]=='':
-		return 'Viewing 🏠 HOME'
-	else:
-		return 'Viewing ' + paths[-2]
-
-
-
-def dir_navigator(path):
-	"""Makes each part of the header directory accessible like links
-	just like file manager, but with less CSS"""
-
-	dirs = re.sub("/{2,}", "/", path).split('/')
-	urls = ['/']
-	names = ['&#127968; HOME']
-	r = []
-
-	for i in range(1, len(dirs)-1):
-		dir = dirs[i]
-		# urls.append(urls[i-1] + urllib.parse.quote(dir, errors='surrogatepass' )+ '/' if not dir.endswith('/') else "")
-		urls.append(urls[i-1] + dir+ '/' if not dir.endswith('/') else "")
-		names.append(dir)
-
-	for i in range(len(names)):
-		tag = "<a class='dir_turns' href='" + urls[i] + "'>" + names[i] + "</a>"
-		r.append(tag)
-
-	return '<span class="dir_arrow">&#10151;</span>'.join(r)
-
-
-
-
-
-def loc(path, _os_name='Linux'):  # fc=0602 v
-	"""to fix dir problem based on os
-
-	args:
-	-----
-		x: directory
-		os_name: Os name *Linux"""
-
-	if _os_name == 'Windows':
-		return path.replace('/', '\\')
-
-	#else:
-	return path.replace('\\', '/')
-
-
-
-def writer(fname, mode, data, direc="", encoding='utf-8'):  # fc=0608 v
-	"""Writing on a file
-
-	why this monster?
-	> to avoid race condition, folder not found etc
-
-	args:
-	-----
-		fname: filename
-		mode: write mode (w, wb, a, ab)
-		data: data to write
-		direc: directory of the file, empty for current dir *None
-		func_code: (str) code of the running func *empty string
-		encoding: if encoding needs to be specified (only str, not binary data) *utf-8
-		timeout: how long to wait until free, 0 for unlimited, -1 for immidiate or crash"""
-
-	def write(location):
-		if 'b' not in mode:
-			with open(location, mode, encoding=encoding) as file:
-				file.write(data)
-		else:
-			with open(location, mode) as file:
-				file.write(data)
-
-	_direc, fname = os.path.split(fname)
-	direc = os.path.join(direc, _direc)
-
-	if any(i in fname for i in ('|:*"><?')) or any(i in direc for i in ('|:*"><?')):
-		# these characters are forbidden to use in file or folder Names
-		raise ValueError("Invalid file or folder name")
-	direc = loc(direc, 'Linux')
-
-	# directory and file names are auto stripped by OS
-	# or else shitty problems occurs
-
-	direc = direc.strip()
-	if not direc.endswith("/"):
-		direc+="/"
-
-	fname = fname.strip()
-
-
-	location = loc(direc + fname)
-
-	"""
-	if any(i in location for i in ('\\|:*"><?')):
-		location = Datasys.trans_str(location, {'\\|:*><?': '-', '"': "'"})
-	"""
-
-
-	# creates the directory, then write the file
-	try:
-		os.makedirs(direc, exist_ok=True)
-	except Exception as e:
-		if e.__class__.__name__ == "PermissionError":
-			_temp = ''
-			_temp2 = direc.split('/')
-			_temp3 = 0
-			for _temp3 in range(len(_temp2)):
-				_temp += _temp2[_temp3] + '/'
-				if not os.path.isdir(_temp):
-					break
-			raise PermissionError(f"Failed to make directory on {_temp}") from e
-		raise e
-
-
-	write(location)
-
+"""
+fs_utils.py
+---------------
+File System Utilities
+
+* Why using Queue and other stuffs instead of os.walk()?
+	- os.walk() is slow, and accessing its stat is slow too.
+* Why making functions with almost same functionality?
+	-  imagine a function just returns all paths, another returns sizes. Using both of them together is using a bit inefficient.
+
+* os.scandir() also caches the stat of the files, so it's faster than os.walk().
+
+# GOT FASTER SOLUTIONS?
+> Make a pull request or open an issue here: https://github.com/RaSan147/pyrobox
+> Thanks for your help!
+"""
+
+from io import BufferedWriter
+import os
+from queue import Queue
+import re
+import time
+import traceback
+import urllib.parse
+
+
+from ._exceptions import LimitExceed
+
+
+
+
+def get_stat(path):
+	"""
+	Get the stat of a file.
+
+	path: path to the file
+
+	* can act as check_access(path) for files
+	"""
+	try:
+		return os.stat(path)
+	except Exception:
+		return False
+
+
+def check_access(path):
+	"""
+	Check if the user has access to the file.
+
+	path: path to the file
+	"""
+	if not os.path.exists(path):
+		return False
+
+	if os.path.isfile(path):
+		try:
+			with open(path, "rb") as f:
+				f.read(1)
+
+				return True
+		except Exception:
+			return False
+	else:
+		# if folder, check if it's stat is accessible
+		return bool(get_stat(path))
+
+
+
+def walk_dir(path, yield_dir=False):
+	"""
+	Iterate through a directory and its subdirectories
+	and `yield` the filePath object of each Files and Folders*.
+
+	path: path to the directory
+	yield_dir (bool): if True yields directories too (default: False)
+	"""
+
+	Q = Queue()
+	Q.put(path)
+	while not Q.empty():
+		path = Q.get()
+
+		try:
+			dir = os.scandir(path)
+		except OSError:
+			continue
+		for entry in dir:
+			try:
+				is_dir = entry.is_dir(follow_symlinks=False)
+			except OSError as error:
+				continue
+			if is_dir:
+				Q.put(entry.path)
+
+			if yield_dir or not is_dir:
+				yield entry
+
+		dir.close()
+
+
+# TODO: can be used in search feature
+def get_tree(path, include_dir=True):
+	"""
+	returns a list of files in a directory and its subdirectories.
+	[ [full path, relative path], ... ]
+
+	path: path to the directory
+	include_dir (bool): if True returns full path, else relative path
+	"""
+	home = path
+	tree = []
+
+	# Q = Queue()
+	# Q.put(path)
+	# while not Q.empty():
+	# 	path = Q.get()
+
+	# 	try:
+	# 		dir = os.scandir(path)
+	# 	except OSError:
+	# 		continue
+	# 	for entry in dir:
+	# 		try:
+	# 			is_dir = entry.is_dir(follow_symlinks=False)
+	# 		except OSError as error:
+	# 			continue
+	# 		if is_dir:
+	# 			Q.put(entry.path)
+
+	# 		if include_dir or not is_dir:
+	# 			tree.append([entry.path, entry.path.replace(home, "", 1)])
+
+	# 	dir.close()
+
+	for entry in walk_dir(path, yield_dir=include_dir):
+		tree.append([entry.path, entry.path.replace(home, "", 1)])
+
+	return tree
+
+
+
+def _get_tree_count(path):
+	count = 0
+
+	# Q = Queue()
+	# Q.put(path)
+	# while not Q.empty():
+	# 	path = Q.get()
+
+	# 	try:
+	# 		dir = os.scandir(path)
+	# 	except OSError:
+	# 		continue
+	# 	for entry in dir:
+	# 		try:
+	# 			is_dir = entry.is_dir(follow_symlinks=False)
+	# 		except OSError as error:
+	# 			continue
+	# 		if is_dir:
+	# 			Q.put(entry.path)
+	# 		else:
+	# 			count += 1
+
+	# 	dir.close()
+
+	for entry in walk_dir(path):
+		count += 1
+
+	return count
+
+
+def get_file_count(path):
+	"""
+	Get the number of files in a directory.
+	"""
+	return _get_tree_count(path)
+
+
+def _get_tree_size(path, limit=None, must_read=False):
+	"""
+	returns the size of a directory and its subdirectories.
+
+	path: path to the directory
+	limit (int): if not None, raises LimitExceed if the size is greater than limit
+	must_read (bool): if True, reads the first byte of each file to check if it's accessible
+	"""
+	r=[] #if return_list
+	total = 0
+	start_path = path
+
+	for entry in walk_dir(path):
+		try:
+			total += entry.stat(follow_symlinks=False).st_size
+		except OSError:
+			continue
+
+		if limit and total>limit:
+			raise LimitExceed
+
+		if must_read and not check_access(entry.path):
+			continue
+
+	return total
+
+def _get_tree_path_n_size(path, limit=-1, must_read=False, path_type="full", add_dirs=False):
+	"""
+	returns a list of files[size, path] in a directory and its subdirectories.
+		[ [`path`, size], ... ]
+		> path: `path_string` | `tuple(full_path, relative_path)`
+
+	path: path to the directory
+	path_type (str): "full" or "relative" or "both"
+	"""
+	r=[] #if return_list
+	total = 0
+	start_path = path
+
+	for entry in walk_dir(path, yield_dir=add_dirs):
+		size = 0
+		if not entry.is_dir():
+			try:
+				size = entry.stat(follow_symlinks=False).st_size
+			except OSError:
+				continue
+			total += size
+
+			if limit>0 and total>limit:
+				raise LimitExceed
+
+			if must_read and not check_access(entry.path):
+				continue
+
+
+		if path_type == "full":
+			r.append([entry.path, size])
+		elif path_type == "relative":
+			r.append([entry.path.replace(start_path, "", 1), size])
+		elif path_type == "both":
+			r.append([(entry.path, entry.path.replace(start_path, "", 1)), size])
+
+	return r
+
+
+def get_dir_size(start_path = '.', limit=None, must_read=False):
+	"""
+	Get the size of a directory and all its subdirectories.
+
+	start_path: path to start calculating from
+	limit (int): maximum folder size, if bigger returns `-1`
+	return_list (bool): if True returns a tuple of (total folder size, list of contents)
+	full_dir (bool): if True returns a full path, else relative path
+	both (bool): if True returns a tuple of (total folder size, (full path, relative path))
+	must_read (bool): if True only counts files that can be read
+	"""
+
+	return _get_tree_size(start_path, limit, must_read)
+
+
+def _get_tree_count_n_size(path):
+	"""
+	Get the size of a directory and all its subdirectories.
+	returns a tuple of (`total file count`, `total folder size`)
+
+	path: path to the directory
+	"""
+	total = 0
+	count = 0
+
+	for entry in walk_dir(path):
+		try:
+			total += entry.stat(follow_symlinks=False).st_size
+		except OSError:
+			continue
+
+		count += 1
+
+	return count, total
+
+def get_tree_count_n_size(start_path):
+	"""
+	Get the size of a directory and all its subdirectories.
+	returns a tuple of (`total file count`, `total folder size`)
+
+	path: path to the directory
+	"""
+
+	return _get_tree_count_n_size(start_path)
+
+
+def fmbytes(B=0, path=''):
+	'Return the given bytes as a file manager friendly KB, MB, GB, or TB string'
+	if path:
+		stat = get_stat(path)
+		if not stat: return "Unknown"
+		B = stat.st_size
+
+	B = B
+	KB = 1024
+	MB = (KB ** 2) # 1,048,576
+	GB = (KB ** 3) # 1,073,741,824
+	TB = (KB ** 4) # 1,099,511,627,776
+
+
+	if B/TB>1:
+		return '%.2f TB  '%(B/TB)
+	if B/GB>1:
+		return '%.2f GB  '%(B/GB)
+	if B/MB>1:
+		return '%.2f MB  '%(B/MB)
+	if B/KB>1:
+		return '%.2f KB  '%(B/KB)
+	if B>1:
+		return '%i bytes'%B
+
+	return "%i byte"%B
+
+
+def humanbytes(B):
+	'Return the given bytes as a human friendly KB, MB, GB, or TB string'
+	B = B
+	KB = 1024
+	MB = (KB ** 2) # 1,048,576
+	GB = (KB ** 3) # 1,073,741,824
+	TB = (KB ** 4) # 1,099,511,627,776
+	ret=''
+
+	if B>=TB:
+		ret+= '%i TB  '%(B//TB)
+		B%=TB
+	if B>=GB:
+		ret+= '%i GB  '%(B//GB)
+		B%=GB
+	if B>=MB:
+		ret+= '%i MB  '%(B//MB)
+		B%=MB
+	if B>=KB:
+		ret+= '%i KB  '%(B//KB)
+		B%=KB
+	if B>0:
+		ret+= '%i bytes'%B
+
+	return ret
+
+def get_dir_m_time(path):
+	"""
+	Get the last modified time of a directory and all its subdirectories.
+	"""
+
+	stat = get_stat(path)
+	return stat.st_mtime if stat else 0
+
+
+
+
+
+def get_titles(path, file=False):
+	"""Make titles for the header directory
+	path: the path of the file or directory
+	file: if True, path is a file, else it's a directory
+
+	output: `Viewing NAME`"""
+
+	paths = path.split('/')
+	if file:
+		return 'Viewing ' + paths[-1]
+	if paths[-2]=='':
+		return 'Viewing 🏠 HOME'
+	else:
+		return 'Viewing ' + paths[-2]
+
+
+
+def dir_navigator(path):
+	"""Makes each part of the header directory accessible like links
+	just like file manager, but with less CSS"""
+
+	dirs = re.sub("/{2,}", "/", path).split('/')
+	urls = ['/']
+	names = ['&#127968; HOME']
+	r = []
+
+	for i in range(1, len(dirs)-1):
+		dir = dirs[i]
+		# urls.append(urls[i-1] + urllib.parse.quote(dir, errors='surrogatepass' )+ '/' if not dir.endswith('/') else "")
+		urls.append(urls[i-1] + dir+ '/' if not dir.endswith('/') else "")
+		names.append(dir)
+
+	for i in range(len(names)):
+		tag = "<a class='dir_turns' href='" + urls[i] + "'>" + names[i] + "</a>"
+		r.append(tag)
+
+	return '<span class="dir_arrow">&#10151;</span>'.join(r)
+
+
+
+
+
+def loc(path, _os_name='Linux'):  # fc=0602 v
+	"""to fix dir problem based on os
+
+	args:
+	-----
+		x: directory
+		os_name: Os name *Linux"""
+
+	if _os_name == 'Windows':
+		return path.replace('/', '\\')
+
+	#else:
+	return path.replace('\\', '/')
+
+
+
+def writer(fname, mode, data, direc="", encoding='utf-8'):  # fc=0608 v
+	"""Writing on a file
+
+	why this monster?
+	> to avoid race condition, folder not found etc
+
+	args:
+	-----
+		fname: filename
+		mode: write mode (w, wb, a, ab)
+		data: data to write
+		direc: directory of the file, empty for current dir *None
+		func_code: (str) code of the running func *empty string
+		encoding: if encoding needs to be specified (only str, not binary data) *utf-8
+		timeout: how long to wait until free, 0 for unlimited, -1 for immidiate or crash"""
+
+	def write(location):
+		if 'b' not in mode:
+			with open(location, mode, encoding=encoding) as file:
+				file.write(data)
+		else:
+			with open(location, mode) as file:
+				file.write(data)
+
+	_direc, fname = os.path.split(fname)
+	direc = os.path.join(direc, _direc)
+
+	if any(i in fname for i in ('|:*"><?')) or any(i in direc for i in ('|:*"><?')):
+		# these characters are forbidden to use in file or folder Names
+		raise ValueError("Invalid file or folder name")
+	direc = loc(direc, 'Linux')
+
+	# directory and file names are auto stripped by OS
+	# or else shitty problems occurs
+
+	direc = direc.strip()
+	if not direc.endswith("/"):
+		direc+="/"
+
+	fname = fname.strip()
+
+
+	location = loc(direc + fname)
+
+	"""
+	if any(i in location for i in ('\\|:*"><?')):
+		location = Datasys.trans_str(location, {'\\|:*><?': '-', '"': "'"})
+	"""
+
+
+	# creates the directory, then write the file
+	try:
+		os.makedirs(direc, exist_ok=True)
+	except Exception as e:
+		if e.__class__.__name__ == "PermissionError":
+			_temp = ''
+			_temp2 = direc.split('/')
+			_temp3 = 0
+			for _temp3 in range(len(_temp2)):
+				_temp += _temp2[_temp3] + '/'
+				if not os.path.isdir(_temp):
+					break
+			raise PermissionError(f"Failed to make directory on {_temp}") from e
+		raise e
+
+
+	write(location)
+
+
+class UploadHandler:
+	def __init__(self, uid):
+		self.serial_io = Queue()
+		# format [[temp_file_obj, mode, data?], ...]
+		# if mode is 's' then data is [os_f_path, overwrite]
+		# if mode is 'w' then data is the data to write
+		self.active = True
+		self.waited = 0
+		self.done = False
+		self.uid = uid
+		self.error = False
+		self.nap_time = 1
+
+		self.stop_on_error = True
+
+	def upload(self, temp_file, mode, data=None):
+		"""
+		* format `[[temp_file_obj, mode, data?], ...]`
+		* if `mode` is `s` then data is [os_f_path, overwrite]
+		* if `mode` is `w` then binary data is the data to write
+		"""
+		if not self.done:
+			self.serial_io.put([temp_file, mode, data])
+
+	def start(self, server):
+		try:
+			self._start(server)
+		except Exception as e:
+			traceback.print_exc()
+			server.log_error("Upload Failed")
+			self.kill()
+
+	def err(self, error_msg):
+		self.error = error_msg
+		if self.stop_on_error:
+			self.kill()
+
+	def sleep(self):
+		time.sleep(self.nap_time)
+
+
+
+	def _start(self, server):
+		while self.active or not self.serial_io.empty():
+			if not self.serial_io.empty():
+				self.waited = 0
+				req_data = self.serial_io.get()
+				file:BufferedWriter = req_data[0]
+				mode = req_data[1]
+				data = req_data[2]
+				if mode == "w": # write
+					file.write(data)
+				if mode == "s": #save
+					temp_fn = file.name
+					if not file.closed:
+						file.close()
+						os_f_path, overwrite = data
+						os_fn = os.path.basename(os_f_path)
+
+						name, ext = os.path.splitext(os_f_path)
+						while (not overwrite) and os.path.isfile(os_f_path):
+							n = 1
+							os_f_path = f"{name}({n}){ext}"
+							n += 1
+
+
+						try:
+							if os.path.exists(os_f_path): # if overwrite is disabled then the previous part will handle the new filename.
+								os.remove(os_f_path)
+							os.rename(temp_fn, os_f_path)
+						except Exception as e:
+							server.log_error(f'Failed to replace {temp_fn} with {os_f_path} by {self.uid}')
+							server.log_error(traceback.format_exc())
+							self.err(f"Failed to upload {os_fn}")
+
+							break
+	
+			else:
+				self.waited += 1
+				self.sleep()
+				if self.waited > 100:
+					self.active = False
+					break
+
+	def kill(self):
+		self.active = False
+		self.done = True
+		
+		for f in tuple(self.serial_io.queue):
+			name = f[0].name
+			if not f[0].closed:
+				f[0].close()
+
+			if os.path.exists(name):
+				os.remove(name)
+
+		self.serial_io.queue.clear()
+
+
+
```

### Comparing `pyrobox-0.9.4/src/_list_maker.py` & `pyrobox-0.9.5/src/_list_maker.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,269 +1,269 @@
-import os
-import posixpath
-import importlib.util
-from http import HTTPStatus
-import urllib.parse
-import html
-from typing import Union
-
-
-
-from .pyroboxCore import config, logger
-from .pyrobox_ServerHost import ServerHost as SH, SimpleCookie
-
-from .user_mgmt import User
-from . import _page_templates as pt
-
-from ._fs_utils import get_titles, dir_navigator, fmbytes
-
-
-
-
-def check_installed(pkg):
-	return bool(importlib.util.find_spec(pkg))
-
-
-
-try:
-	import natsort
-except Exception:
-	config.disabled_func["natsort"] = True
-	logger.warning("natsort module not found, natsort function disabled")
-
-def humansorted(li):
-	"""
-	Sort a list of strings like a human would
-	"""
-
-	if not config.disabled_func["natsort"]:
-		return natsort.humansorted(li)
-
-	return sorted(li, key=lambda x: x.lower())
-
-def scansort(li):
-	"""
-	Sort a list of os.scandir objects in File Explorer order
-	"""
-
-	if not config.disabled_func["natsort"]:
-		return natsort.humansorted(li, key=lambda x:x.name)
-
-	return sorted(li, key=lambda x: x.name.lower())
-
-def listsort(li):
-	"""
-	Sort a list of strings in More Human way
-	"""
-
-	return humansorted(li)
-
-
-
-
-#############################################
-#                FILE HANDLER               #
-#############################################
-
-
-
-def list_directory_json(self:SH, path=None):
-	"""
-	Helper to produce a directory listing (JSON).
-	Return json file of available files and folders
-	"""
-	if path == None:
-		path = self.translate_path(self.path)
-
-	try:
-		dir_list = scansort(os.scandir(path))
-	except OSError:
-		self.send_error(
-			HTTPStatus.NOT_FOUND,
-			"No permission to list directory")
-		return None
-	dir_dict = []
-
-
-	for file in dir_list:
-		name = file.name
-		displayname = linkname = name
-
-
-		if file.is_dir():
-			displayname = name + "/"
-			linkname = name + "/"
-		elif file.is_symlink():
-			displayname = name + "@"
-
-		dir_dict.append([urllib.parse.quote(linkname, errors='surrogatepass'),
-						html.escape(displayname, quote=False)])
-
-	return self.send_json(dir_dict)
-
-
-def list_directory_html(self:SH, path, user:User, cookie:Union[SimpleCookie, str]=None):
-	"""
-	Helper to produce a directory listing (absent index.html).
-
-	Return value is either a file object, or None (indicating an
-	error).  In either case, the headers are sent, making the
-	interface the same as for send_head().
-
-	"""
-	if user.NOPERMISSION or user.VIEW == False:
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You don't have permission to see file list", cookie=cookie)
-
-
-	try:
-		dir_list = scansort(os.scandir(path))
-	except OSError:
-		self.send_error(
-			HTTPStatus.NOT_FOUND,
-			"No permission to list directory")
-		return None
-
-
-	r_folders = [] # no js
-	r_files = [] # no js
-
-
-	LIST_STRING = '<li><a class= "%s" href="%s">%s</a></li><hr>'
-
-	for file in dir_list:
-		name = file.name
-
-		displayname = linkname = name
-		size=0
-		# Append / for directories or @ for symbolic links
-		_is_dir_ = True
-		if file.is_dir():
-			displayname = name + "/"
-			linkname = name + "/"
-		elif file.is_symlink():
-			displayname = name + "@"
-		else:
-			_is_dir_ =False
-			size = fmbytes(file.stat().st_size)
-			__, ext = posixpath.splitext(name)
-			if ext=='.html':
-				r_files.append(LIST_STRING % ("link", urllib.parse.quote(linkname,
-									errors='surrogatepass'),
-									html.escape(displayname, quote=False)))
-
-			elif self.guess_type(linkname).startswith('video/'):
-				r_files.append(LIST_STRING % ("vid", urllib.parse.quote(linkname,
-									errors='surrogatepass'),
-									html.escape(displayname, quote=False)))
-
-			elif self.guess_type(linkname).startswith('image/'):
-				r_files.append(LIST_STRING % ("file", urllib.parse.quote(linkname,
-									errors='surrogatepass'),
-									html.escape(displayname, quote=False)))
-
-			else:
-				r_files.append(LIST_STRING % ("file", urllib.parse.quote(linkname,
-									errors='surrogatepass'),
-									html.escape(displayname, quote=False)))
-
-		if _is_dir_:
-			r_folders.append(LIST_STRING % ("", urllib.parse.quote(linkname,
-									errors='surrogatepass'),
-									html.escape(displayname, quote=False)))
-
-
-	NO_JS_LINKS = "\n".join(r_folders +	r_files)
-
-	NO_JS_LINKS = " -->\n" + NO_JS_LINKS + "\n<!-- " # hack to hide the Template code
-
-	UPLOAD_FORM = ""
-
-	if user.UPLOAD and not user.READ_ONLY:
-		UPLOAD_FORM = " -->\n" + pt.upload_form() + "\n<!-- " # hack to hide the Template code
-
-	return self.html_main_page(user, PY_NO_JS_FILE_LIST=NO_JS_LINKS, PY_UPLOAD_FORM=UPLOAD_FORM,
-			cookie=cookie)
-
-
-
-
-
-def list_directory(self:SH, path, user:User, cookie:Union[SimpleCookie, str]=None):
-	"""
-	Helper to produce a directory listing (absent index.html).
-
-	Return value is either a file object, or None (indicating an
-	error).  In either case, the headers are sent, making the
-	interface the same as for send_head().
-
-	"""
-	try:
-		dir_list = scansort(os.scandir(path))
-	except OSError:
-		self.send_error(
-			HTTPStatus.NOT_FOUND,
-			"No permission to list directory")
-		return None
-
-	displaypath = self.get_displaypath(self.url_path)
-
-
-	title = get_titles(displaypath)
-
-
-	r_li= [] # type + file_link
-				# f  : File
-				# d  : Directory
-				# v  : Video
-				# h  : HTML
-	f_li = [] # file_names
-	s_li = [] # size list
-
-
-	# r.append("""<a href="../" style="background-color: #000;padding: 3px 20px 8px 20px;border-radius: 4px;">&#128281; {Prev folder}</a>""")
-	for file in dir_list:
-		#fullname = os.path.join(path, name)
-		name = file.name
-		displayname = linkname = name
-		size=0
-		# Append / for directories or @ for symbolic links
-		_is_dir_ = True
-		if file.is_dir():
-			displayname = name + "/"
-			linkname = name + "/"
-		elif file.is_symlink():
-			displayname = name + "@"
-		else:
-			_is_dir_ =False
-			size = fmbytes(file.stat().st_size)
-			__, ext = posixpath.splitext(name)
-			if ext=='.html':
-				r_li.append('h'+ urllib.parse.quote(linkname, errors='surrogatepass'))
-				f_li.append(html.escape(displayname, quote=False))
-
-			elif self.guess_type(linkname).startswith('video/'):
-				r_li.append('v'+ urllib.parse.quote(linkname, errors='surrogatepass'))
-				f_li.append(html.escape(displayname, quote=False))
-
-			elif self.guess_type(linkname).startswith('image/'):
-				r_li.append('i'+ urllib.parse.quote(linkname, errors='surrogatepass'))
-				f_li.append(html.escape(displayname, quote=False))
-
-			else:
-				r_li.append('f'+ urllib.parse.quote(linkname, errors='surrogatepass'))
-				f_li.append(html.escape(displayname, quote=False))
-		if _is_dir_:
-			r_li.append('d' + urllib.parse.quote(linkname, errors='surrogatepass'))
-			f_li.append(html.escape(displayname, quote=False))
-
-		s_li.append(size)
-
-	result = {
-		"status": "success",
-		"file_list": f_li,
-		"size_list": s_li,
-		"type_list": r_li,
-		"title": title,
-	}
-
-	return result
-
+import os
+import posixpath
+import importlib.util
+from http import HTTPStatus
+import urllib.parse
+import html
+from typing import Union
+
+
+
+from .pyroboxCore import config, logger
+from .pyrobox_ServerHost import ServerHost as SH, SimpleCookie
+
+from .user_mgmt import User
+from . import _page_templates as pt
+
+from ._fs_utils import get_titles, dir_navigator, fmbytes
+
+
+
+
+def check_installed(pkg):
+	return bool(importlib.util.find_spec(pkg))
+
+
+
+try:
+	import natsort
+except Exception:
+	config.disabled_func["natsort"] = True
+	logger.warning("natsort module not found, natsort function disabled")
+
+def humansorted(li):
+	"""
+	Sort a list of strings like a human would
+	"""
+
+	if not config.disabled_func["natsort"]:
+		return natsort.humansorted(li)
+
+	return sorted(li, key=lambda x: x.lower())
+
+def scansort(li):
+	"""
+	Sort a list of os.scandir objects in File Explorer order
+	"""
+
+	if not config.disabled_func["natsort"]:
+		return natsort.humansorted(li, key=lambda x:x.name)
+
+	return sorted(li, key=lambda x: x.name.lower())
+
+def listsort(li):
+	"""
+	Sort a list of strings in More Human way
+	"""
+
+	return humansorted(li)
+
+
+
+
+#############################################
+#                FILE HANDLER               #
+#############################################
+
+
+
+def list_directory_json(self:SH, path=None):
+	"""
+	Helper to produce a directory listing (JSON).
+	Return json file of available files and folders
+	"""
+	if path == None:
+		path = self.translate_path(self.path)
+
+	try:
+		dir_list = scansort(os.scandir(path))
+	except OSError:
+		self.send_error(
+			HTTPStatus.NOT_FOUND,
+			"No permission to list directory")
+		return None
+	dir_dict = []
+
+
+	for file in dir_list:
+		name = file.name
+		displayname = linkname = name
+
+
+		if file.is_dir():
+			displayname = name + "/"
+			linkname = name + "/"
+		elif file.is_symlink():
+			displayname = name + "@"
+
+		dir_dict.append([urllib.parse.quote(linkname, errors='surrogatepass'),
+						html.escape(displayname, quote=False)])
+
+	return self.send_json(dir_dict)
+
+
+def list_directory_html(self:SH, path, user:User, cookie:Union[SimpleCookie, str]=None):
+	"""
+	Helper to produce a directory listing (absent index.html).
+
+	Return value is either a file object, or None (indicating an
+	error).  In either case, the headers are sent, making the
+	interface the same as for send_head().
+
+	"""
+	if user.NOPERMISSION or user.VIEW == False:
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You don't have permission to see file list", cookie=cookie)
+
+
+	try:
+		dir_list = scansort(os.scandir(path))
+	except OSError:
+		self.send_error(
+			HTTPStatus.NOT_FOUND,
+			"No permission to list directory")
+		return None
+
+
+	r_folders = [] # no js
+	r_files = [] # no js
+
+
+	LIST_STRING = '<li><a class= "%s" href="%s">%s</a></li><hr>'
+
+	for file in dir_list:
+		name = file.name
+
+		displayname = linkname = name
+		size=0
+		# Append / for directories or @ for symbolic links
+		_is_dir_ = True
+		if file.is_dir():
+			displayname = name + "/"
+			linkname = name + "/"
+		elif file.is_symlink():
+			displayname = name + "@"
+		else:
+			_is_dir_ =False
+			size = fmbytes(file.stat().st_size)
+			__, ext = posixpath.splitext(name)
+			if ext=='.html':
+				r_files.append(LIST_STRING % ("link", urllib.parse.quote(linkname,
+									errors='surrogatepass'),
+									html.escape(displayname, quote=False)))
+
+			elif self.guess_type(linkname).startswith('video/'):
+				r_files.append(LIST_STRING % ("vid", urllib.parse.quote(linkname,
+									errors='surrogatepass'),
+									html.escape(displayname, quote=False)))
+
+			elif self.guess_type(linkname).startswith('image/'):
+				r_files.append(LIST_STRING % ("file", urllib.parse.quote(linkname,
+									errors='surrogatepass'),
+									html.escape(displayname, quote=False)))
+
+			else:
+				r_files.append(LIST_STRING % ("file", urllib.parse.quote(linkname,
+									errors='surrogatepass'),
+									html.escape(displayname, quote=False)))
+
+		if _is_dir_:
+			r_folders.append(LIST_STRING % ("", urllib.parse.quote(linkname,
+									errors='surrogatepass'),
+									html.escape(displayname, quote=False)))
+
+
+	NO_JS_LINKS = "\n".join(r_folders +	r_files)
+
+	NO_JS_LINKS = " -->\n" + NO_JS_LINKS + "\n<!-- " # hack to hide the Template code
+
+	UPLOAD_FORM = ""
+
+	if user.UPLOAD and not user.READ_ONLY:
+		UPLOAD_FORM = " -->\n" + pt.upload_form() + "\n<!-- " # hack to hide the Template code
+
+	return self.html_main_page(user, PY_NO_JS_FILE_LIST=NO_JS_LINKS, PY_UPLOAD_FORM=UPLOAD_FORM,
+			cookie=cookie)
+
+
+
+
+
+def list_directory(self:SH, path, user:User, cookie:Union[SimpleCookie, str]=None):
+	"""
+	Helper to produce a directory listing (absent index.html).
+
+	Return value is either a file object, or None (indicating an
+	error).  In either case, the headers are sent, making the
+	interface the same as for send_head().
+
+	"""
+	try:
+		dir_list = scansort(os.scandir(path))
+	except OSError:
+		self.send_error(
+			HTTPStatus.NOT_FOUND,
+			"No permission to list directory")
+		return None
+
+	displaypath = self.get_displaypath(self.url_path)
+
+
+	title = get_titles(displaypath)
+
+
+	r_li= [] # type + file_link
+				# f  : File
+				# d  : Directory
+				# v  : Video
+				# h  : HTML
+	f_li = [] # file_names
+	s_li = [] # size list
+
+
+	# r.append("""<a href="../" style="background-color: #000;padding: 3px 20px 8px 20px;border-radius: 4px;">&#128281; {Prev folder}</a>""")
+	for file in dir_list:
+		#fullname = os.path.join(path, name)
+		name = file.name
+		displayname = linkname = name
+		size=0
+		# Append / for directories or @ for symbolic links
+		_is_dir_ = True
+		if file.is_dir():
+			displayname = name + "/"
+			linkname = name + "/"
+		elif file.is_symlink():
+			displayname = name + "@"
+		else:
+			_is_dir_ =False
+			size = fmbytes(file.stat().st_size)
+			__, ext = posixpath.splitext(name)
+			if ext=='.html':
+				r_li.append('h'+ urllib.parse.quote(linkname, errors='surrogatepass'))
+				f_li.append(html.escape(displayname, quote=False))
+
+			elif self.guess_type(linkname).startswith('video/'):
+				r_li.append('v'+ urllib.parse.quote(linkname, errors='surrogatepass'))
+				f_li.append(html.escape(displayname, quote=False))
+
+			elif self.guess_type(linkname).startswith('image/'):
+				r_li.append('i'+ urllib.parse.quote(linkname, errors='surrogatepass'))
+				f_li.append(html.escape(displayname, quote=False))
+
+			else:
+				r_li.append('f'+ urllib.parse.quote(linkname, errors='surrogatepass'))
+				f_li.append(html.escape(displayname, quote=False))
+		if _is_dir_:
+			r_li.append('d' + urllib.parse.quote(linkname, errors='surrogatepass'))
+			f_li.append(html.escape(displayname, quote=False))
+
+		s_li.append(size)
+
+	result = {
+		"status": "success",
+		"file_list": f_li,
+		"size_list": s_li,
+		"type_list": r_li,
+		"title": title,
+	}
+
+	return result
+
```

### Comparing `pyrobox-0.9.4/src/_zipfly_manager.py` & `pyrobox-0.9.5/src/_zipfly_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-# -*- coding: utf-8 -*-
-zf__version__ = '6.0.5'
-# v
-
-import io
-import zipfile
-import tempfile
-import os
-import shutil
-import atexit
-import random
-import string
-import time
-import traceback
-import threading
-from collections import OrderedDict
-
-from ._fs_utils import get_dir_size, get_dir_m_time, _get_tree_path_n_size
-from ._exceptions import LimitExceed
-
-
-
-ZIP64_LIMIT = (1 << 31) + 1
-
-class ZipflyStream(io.RawIOBase):
-	def __init__(self):
-		self._buffer = b''
-		self._size = 0
-
-	def writable(self):
-		return True
-
-	def write(self, b):
-		if self.closed:
-			raise RuntimeError("ZipFly stream was closed!")
-		self._buffer += b
-		return len(b)
-
-	def get(self):
-		chunk = self._buffer
-		self._buffer = b''
-		self._size += len(chunk)
-		return chunk
-
-	def size(self):
-		return self._size
-
-
-class ZipFly:
-
-	def __init__(self,
-				 mode = 'w',
-				 paths = [],
-				 chunksize = 0x8000,
-				 compression = zipfile.ZIP_STORED,
-				 allowZip64 = True,
-				 compresslevel = None,
-				 storesize = 0,
-				 encode = 'utf-8',):
-
-		"""
-		@param store size : int : size of all files
-		in paths without compression
-		"""
-		if isinstance(chunksize, str):
-			chunksize = int(chunksize, 16)
-
-
-
-		self.comment = 'Written using Zipfly v' + zf__version__
-		self.mode = mode
-		self.paths = paths
-		self.filesystem = 'fs'
-		self.arcname = 'n'
-		self.compression = compression
-		self.chunksize = chunksize
-		self.allowZip64 = allowZip64
-		self.compresslevel = compresslevel
-		self.storesize = storesize
-		self.encode = encode
-		self.ezs = int('0x8e', 16) # empty zip size in bytes
-
-	def generator(self):
-
-		# stream
-		stream = ZipflyStream()
-
-		with zipfile.ZipFile(
-			stream,
-			mode = self.mode,
-			compression = self.compression,
-			allowZip64 = self.allowZip64,) as zf:
-
-			for path in self.paths:
-				if not self.arcname in path:
-
-					# arcname will be default path
-					path[self.arcname] = path[self.filesystem]
-
-
-				if os.path.isdir(path[self.filesystem]):
-					if os.listdir(path[self.filesystem]):
-						continue # not empty
-					# Write empty directory:
-					if path[self.arcname].endswith('\\'):
-						path[self.arcname] = path[self.arcname][:-1] + '/'
-
-					if not path[self.arcname].endswith('/'):
-						path[self.arcname] += '/'
-
-					if path[self.arcname].startswith('/') or path[self.arcname].startswith('\\'):
-						path[self.arcname] = path[self.arcname][1:]
-					z_info = zipfile.ZipInfo(path[self.arcname])
-					z_info.compress_type = zipfile.ZIP_STORED
-
-
-					zf.writestr(z_info, b'')
-
-					yield stream.get(), self.ezs
-					continue
-				z_info = zipfile.ZipInfo.from_file(
-					path[self.filesystem],
-					path[self.arcname],
-					strict_timestamps=False
-				)
-
-				with open( path[self.filesystem], 'rb' ) as e:
-					# Read from filesystem:
-					with zf.open( z_info, mode=self.mode ) as d:
-
-						for chunk in iter( lambda: e.read(self.chunksize), b'' ):
-
-							d.write(chunk)
-							yield stream.get(), len(chunk)
-		_chunk = stream.get()
-		yield _chunk,  len(_chunk)
-		self._buffer_size = stream.size()
-
-		# Flush and close this stream.
-		stream.close()
-
-	def get_size(self):
-		return self._buffer_size
-
-
-
-
-
-
-
-class Callable_dict(dict):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-		self.__dict__ = self
-
-	def __call__(self, *key):
-		return all([i in self for i in key])
-
-
-class FixSizeOrderedDict(OrderedDict, Callable_dict):
-	def __init__(self, *args, max=0, **kwargs):
-		self._max = max
-		super().__init__(*args, **kwargs)
-
-	def __setitem__(self, key, value):
-		OrderedDict.__setitem__(self, key, value)
-		if self._max > 0:
-			if len(self) > self._max:
-				self.popitem(False)
-
-class ZIP_Manager:
-	def __init__(self, zip_allowed, size_limit=-1) -> None:
-		self.zip_allowed = zip_allowed
-		self.size_limit = size_limit
-
-
-		self.zip_temp_dir = tempfile.gettempdir() + '/zip_temp/'
-		self.zip_ids = Callable_dict()
-		self.zip_path_ids = Callable_dict()
-		self.zip_in_progress = Callable_dict()
-		self.zip_id_status = Callable_dict()
-
-		self.assigend_zid = Callable_dict()
-		self.calculating = Callable_dict()
-		self.calculation_cache = FixSizeOrderedDict(max=100)
-
-		self.cleanup()
-		atexit.register(self.cleanup)
-
-		self.init_dir()
-
-
-	def init_dir(self):
-		os.makedirs(self.zip_temp_dir, exist_ok=True)
-
-
-	def cleanup(self):
-		shutil.rmtree(self.zip_temp_dir, ignore_errors=True)
-
-	def get_id(self, path, size=None):
-		"""
-		get id of the folder
-		if calculating or archiving, return id of the folder
-		"""
-		if self.calculating(path):
-			return self.calculating[path]
-
-
-		id = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(6))+'_'+ str(time.time())
-		id += '0'*(25-len(id))
-
-		self.calculating[path] = id
-
-		source_m_time = get_dir_m_time(path)
-		if size is None:
-			try:
-				fs = _get_tree_path_n_size(path, must_read=True, limit=self.size_limit, path_type="both", add_dirs=True)
-			except LimitExceed as e:
-				self.calculating.pop(path) # make sure to remove calculating flag (MAJOR BUG)
-				raise e
-
-			source_size = sum(i[1] for i in fs)
-			fm = [i[0] for i in fs]
-
-			self.calculation_cache[id] = (source_size, fm, source_m_time)
-		else:
-			source_size = size
-
-
-		self.calculating.pop(path)
-
-		exist = 1
-
-		prev_zid, prev_size, prev_m_time = 0,0,0
-		if self.zip_path_ids(path):
-			prev_zid, prev_size, prev_m_time = self.zip_path_ids[path]
-
-		elif self.assigend_zid(path):
-			prev_zid, prev_size, prev_m_time = self.assigend_zid[path]
-
-		else:
-			exist=0
-
-
-		if exist and prev_m_time == source_m_time and prev_size == source_size:
-			return prev_zid
-
-
-		self.assigend_zid[path] = (id, source_size, source_m_time)
-		return id
-
-
-
-
-	def archive(self, path, zid, size=None):
-		"""
-		archive the folder
-
-		`path`: path to archive
-		`zid`: id of the folder
-		`size`: size of the folder (optional)
-		"""
-		def err(msg):
-			self.zip_in_progress.pop(zid, None)
-			self.assigend_zid.pop(path, None)
-			self.zip_id_status[zid] = "ERROR: " + msg
-			return False
-		if not self.zip_allowed:
-			return err("ZIP FUNTION DISABLED")
-
-
-
-
-		# run zipfly
-		self.zip_in_progress[zid] = 0
-
-		if not self.calculation_cache(zid):
-			try:
-				fs = _get_tree_path_n_size(path, must_read=True, path_type="both", limit=self.size_limit, add_dirs=True)
-			except LimitExceed as e:
-				return err("DIRECTORY SIZE LIMIT EXCEED")
-			source_size = sum(i[1] for i in fs)
-			fm = [i[0] for i in fs]
-			source_m_time = get_dir_m_time(path)
-
-		else:
-			source_size, fm, source_m_time = self.calculation_cache[zid]
-			self.calculation_cache.pop(zid)
-
-		if len(fm)==0:
-			return err("FOLDER HAS NO FILES")
-
-
-		dir_name = os.path.basename(path)
-
-
-
-		zfile_name = os.path.join(self.zip_temp_dir, "{dir_name}({zid})".format(dir_name=dir_name, zid=zid) + ".zip")
-
-		self.init_dir()
-
-		paths = []
-		for xx in fm:
-			try:
-				i, j = xx
-			except:
-				print(xx)
-				traceback.print_exc()
-				continue
-			paths.append({"fs": i, "n":j})
-
-		zfly = ZipFly(paths = paths, chunksize=0x80000)
-
-
-
-		archived_size = 0
-
-		self.zip_id_status[zid] = "ARCHIVING"
-
-		try:
-			with open(zfile_name, "wb") as zf:
-				for chunk, c_size in zfly.generator():
-					zf.write(chunk)
-					archived_size += c_size
-					if source_size==0:
-						source_size+=1 # prevent division by 0
-					self.zip_in_progress[zid] = (archived_size/source_size)*100
-		except Exception as e:
-			traceback.print_exc()
-			return err(e)
-		self.zip_in_progress.pop(zid, None)
-		self.assigend_zid.pop(path, None)
-		self.zip_id_status[zid] = "DONE"
-
-
-
-		self.zip_path_ids[path] = zid, source_size, source_m_time
-		self.zip_ids[zid] = zfile_name
-		# zip_ids are never cleared in runtime due to the fact if someones downloading a zip, the folder content changed, other person asked for zip, new zip created and this id got removed, the 1st user wont be able to resume
-
-
-		return zid
-
-	def archive_thread(self, path, zid, size=None):
-		return threading.Thread(target=self.archive, args=(path, zid, size))
-
-
-if __name__ == "__main__":
-	paths = [
-		{
-			'fs': 'test(hahah)'
-		},
-	]
-
-	zfly = ZipFly(paths = paths)
-
-	generator = zfly.generator()
-	print (generator)
-	# <generator object ZipFly.generator at 0x7f74d52bcc50>
-
-
-	with open("large.zip", "wb") as f:
-		for i in generator:
+# -*- coding: utf-8 -*-
+zf__version__ = '6.0.5'
+# v
+
+import io
+import zipfile
+import tempfile
+import os
+import shutil
+import atexit
+import random
+import string
+import time
+import traceback
+import threading
+from collections import OrderedDict
+
+from ._fs_utils import get_dir_size, get_dir_m_time, _get_tree_path_n_size
+from ._exceptions import LimitExceed
+
+
+
+ZIP64_LIMIT = (1 << 31) + 1
+
+class ZipflyStream(io.RawIOBase):
+	def __init__(self):
+		self._buffer = b''
+		self._size = 0
+
+	def writable(self):
+		return True
+
+	def write(self, b):
+		if self.closed:
+			raise RuntimeError("ZipFly stream was closed!")
+		self._buffer += b
+		return len(b)
+
+	def get(self):
+		chunk = self._buffer
+		self._buffer = b''
+		self._size += len(chunk)
+		return chunk
+
+	def size(self):
+		return self._size
+
+
+class ZipFly:
+
+	def __init__(self,
+				 mode = 'w',
+				 paths = [],
+				 chunksize = 0x8000,
+				 compression = zipfile.ZIP_STORED,
+				 allowZip64 = True,
+				 compresslevel = None,
+				 storesize = 0,
+				 encode = 'utf-8',):
+
+		"""
+		@param store size : int : size of all files
+		in paths without compression
+		"""
+		if isinstance(chunksize, str):
+			chunksize = int(chunksize, 16)
+
+
+
+		self.comment = 'Written using Zipfly v' + zf__version__
+		self.mode = mode
+		self.paths = paths
+		self.filesystem = 'fs'
+		self.arcname = 'n'
+		self.compression = compression
+		self.chunksize = chunksize
+		self.allowZip64 = allowZip64
+		self.compresslevel = compresslevel
+		self.storesize = storesize
+		self.encode = encode
+		self.ezs = int('0x8e', 16) # empty zip size in bytes
+
+	def generator(self):
+
+		# stream
+		stream = ZipflyStream()
+
+		with zipfile.ZipFile(
+			stream,
+			mode = self.mode,
+			compression = self.compression,
+			allowZip64 = self.allowZip64,) as zf:
+
+			for path in self.paths:
+				if not self.arcname in path:
+
+					# arcname will be default path
+					path[self.arcname] = path[self.filesystem]
+
+
+				if os.path.isdir(path[self.filesystem]):
+					if os.listdir(path[self.filesystem]):
+						continue # not empty
+					# Write empty directory:
+					if path[self.arcname].endswith('\\'):
+						path[self.arcname] = path[self.arcname][:-1] + '/'
+
+					if not path[self.arcname].endswith('/'):
+						path[self.arcname] += '/'
+
+					if path[self.arcname].startswith('/') or path[self.arcname].startswith('\\'):
+						path[self.arcname] = path[self.arcname][1:]
+					z_info = zipfile.ZipInfo(path[self.arcname])
+					z_info.compress_type = zipfile.ZIP_STORED
+
+
+					zf.writestr(z_info, b'')
+
+					yield stream.get(), self.ezs
+					continue
+				z_info = zipfile.ZipInfo.from_file(
+					path[self.filesystem],
+					path[self.arcname],
+					strict_timestamps=False
+				)
+
+				with open( path[self.filesystem], 'rb' ) as e:
+					# Read from filesystem:
+					with zf.open( z_info, mode=self.mode ) as d:
+
+						for chunk in iter( lambda: e.read(self.chunksize), b'' ):
+
+							d.write(chunk)
+							yield stream.get(), len(chunk)
+		_chunk = stream.get()
+		yield _chunk,  len(_chunk)
+		self._buffer_size = stream.size()
+
+		# Flush and close this stream.
+		stream.close()
+
+	def get_size(self):
+		return self._buffer_size
+
+
+
+
+
+
+
+class Callable_dict(dict):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.__dict__ = self
+
+	def __call__(self, *key):
+		return all([i in self for i in key])
+
+
+class FixSizeOrderedDict(OrderedDict, Callable_dict):
+	def __init__(self, *args, max=0, **kwargs):
+		self._max = max
+		super().__init__(*args, **kwargs)
+
+	def __setitem__(self, key, value):
+		OrderedDict.__setitem__(self, key, value)
+		if self._max > 0:
+			if len(self) > self._max:
+				self.popitem(False)
+
+class ZIP_Manager:
+	def __init__(self, zip_allowed, size_limit=-1) -> None:
+		self.zip_allowed = zip_allowed
+		self.size_limit = size_limit
+
+
+		self.zip_temp_dir = tempfile.gettempdir() + '/zip_temp/'
+		self.zip_ids = Callable_dict()
+		self.zip_path_ids = Callable_dict()
+		self.zip_in_progress = Callable_dict()
+		self.zip_id_status = Callable_dict()
+
+		self.assigend_zid = Callable_dict()
+		self.calculating = Callable_dict()
+		self.calculation_cache = FixSizeOrderedDict(max=100)
+
+		self.cleanup()
+		atexit.register(self.cleanup)
+
+		self.init_dir()
+
+
+	def init_dir(self):
+		os.makedirs(self.zip_temp_dir, exist_ok=True)
+
+
+	def cleanup(self):
+		shutil.rmtree(self.zip_temp_dir, ignore_errors=True)
+
+	def get_id(self, path, size=None):
+		"""
+		get id of the folder
+		if calculating or archiving, return id of the folder
+		"""
+		if self.calculating(path):
+			return self.calculating[path]
+
+
+		id = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(6))+'_'+ str(time.time())
+		id += '0'*(25-len(id))
+
+		self.calculating[path] = id
+
+		source_m_time = get_dir_m_time(path)
+		if size is None:
+			try:
+				fs = _get_tree_path_n_size(path, must_read=True, limit=self.size_limit, path_type="both", add_dirs=True)
+			except LimitExceed as e:
+				self.calculating.pop(path) # make sure to remove calculating flag (MAJOR BUG)
+				raise e
+
+			source_size = sum(i[1] for i in fs)
+			fm = [i[0] for i in fs]
+
+			self.calculation_cache[id] = (source_size, fm, source_m_time)
+		else:
+			source_size = size
+
+
+		self.calculating.pop(path)
+
+		exist = 1
+
+		prev_zid, prev_size, prev_m_time = 0,0,0
+		if self.zip_path_ids(path):
+			prev_zid, prev_size, prev_m_time = self.zip_path_ids[path]
+
+		elif self.assigend_zid(path):
+			prev_zid, prev_size, prev_m_time = self.assigend_zid[path]
+
+		else:
+			exist=0
+
+
+		if exist and prev_m_time == source_m_time and prev_size == source_size:
+			return prev_zid
+
+
+		self.assigend_zid[path] = (id, source_size, source_m_time)
+		return id
+
+
+
+
+	def archive(self, path, zid, size=None):
+		"""
+		archive the folder
+
+		`path`: path to archive
+		`zid`: id of the folder
+		`size`: size of the folder (optional)
+		"""
+		def err(msg):
+			self.zip_in_progress.pop(zid, None)
+			self.assigend_zid.pop(path, None)
+			self.zip_id_status[zid] = "ERROR: " + msg
+			return False
+		if not self.zip_allowed:
+			return err("ZIP FUNTION DISABLED")
+
+
+
+
+		# run zipfly
+		self.zip_in_progress[zid] = 0
+
+		if not self.calculation_cache(zid):
+			try:
+				fs = _get_tree_path_n_size(path, must_read=True, path_type="both", limit=self.size_limit, add_dirs=True)
+			except LimitExceed as e:
+				return err("DIRECTORY SIZE LIMIT EXCEED")
+			source_size = sum(i[1] for i in fs)
+			fm = [i[0] for i in fs]
+			source_m_time = get_dir_m_time(path)
+
+		else:
+			source_size, fm, source_m_time = self.calculation_cache[zid]
+			self.calculation_cache.pop(zid)
+
+		if len(fm)==0:
+			return err("FOLDER HAS NO FILES")
+
+
+		dir_name = os.path.basename(path)
+
+
+
+		zfile_name = os.path.join(self.zip_temp_dir, "{dir_name}({zid})".format(dir_name=dir_name, zid=zid) + ".zip")
+
+		self.init_dir()
+
+		paths = []
+		for xx in fm:
+			try:
+				i, j = xx
+			except:
+				print(xx)
+				traceback.print_exc()
+				continue
+			paths.append({"fs": i, "n":j})
+
+		zfly = ZipFly(paths = paths, chunksize=0x80000)
+
+
+
+		archived_size = 0
+
+		self.zip_id_status[zid] = "ARCHIVING"
+
+		try:
+			with open(zfile_name, "wb") as zf:
+				for chunk, c_size in zfly.generator():
+					zf.write(chunk)
+					archived_size += c_size
+					if source_size==0:
+						source_size+=1 # prevent division by 0
+					self.zip_in_progress[zid] = (archived_size/source_size)*100
+		except Exception as e:
+			traceback.print_exc()
+			return err(e)
+		self.zip_in_progress.pop(zid, None)
+		self.assigend_zid.pop(path, None)
+		self.zip_id_status[zid] = "DONE"
+
+
+
+		self.zip_path_ids[path] = zid, source_size, source_m_time
+		self.zip_ids[zid] = zfile_name
+		# zip_ids are never cleared in runtime due to the fact if someones downloading a zip, the folder content changed, other person asked for zip, new zip created and this id got removed, the 1st user wont be able to resume
+
+
+		return zid
+
+	def archive_thread(self, path, zid, size=None):
+		return threading.Thread(target=self.archive, args=(path, zid, size))
+
+
+if __name__ == "__main__":
+	paths = [
+		{
+			'fs': 'test(hahah)'
+		},
+	]
+
+	zfly = ZipFly(paths = paths)
+
+	generator = zfly.generator()
+	print (generator)
+	# <generator object ZipFly.generator at 0x7f74d52bcc50>
+
+
+	with open("large.zip", "wb") as f:
+		for i in generator:
 			f.write(i[0])
```

### Comparing `pyrobox-0.9.4/src/data_types.py` & `pyrobox-0.9.5/src/data_types.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from collections import OrderedDict
-
-
-class Callable_dict(dict):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-		self.__dict__ = self
-
-	def __call__(self, *key):
-		return all([i in self for i in key])
-
-
-class GETdict(Callable_dict):
-	"""
-	to set item, use dict["key"] = value for the 1st time,
-	then use dict.key or dict["key"] to both get and set value
-
-	but using dick.key = value 1st, will assign it as attribute and its temporary
-	"""
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-		self.__dict__ = self
-
-
-	def __setitem__(self, key, value):
-		super().__setitem__(key, value)
-
-	def __setattr__(self, key, value):
-		if self(key):
-			self.__setitem__(key, value)
-		else:
-			super().__setattr__(key, value)
-
-	def  __getattr__(self, __name: str):
-		if self(__name):
-			return self.__getitem__(__name)
-		return super().__getattribute__(__name)
-
-
-	# def __getitem__(self, __key):
-	# 	return super().__getitem__(__key)
-
-class Flag(GETdict):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-		self.__dict__ = self
-
-	def __getitem__(self, __key):
-		return super().get(__key, None)
-
-	def  __getattr__(self, __name: str):
-		return super().get(__name, None)
-		# try:
-		# 	return super().__getitem__(__name)
-		# except Exception:
-		# 	return None
-
-
-class LimitedDict(OrderedDict):
-    def __init__(self, *args, max=0, **kwargs):
-        self._max = max
-        super().__init__(*args, **kwargs)
-
-    def __setitem__(self, key, value):
-        super().__setitem__(key, value)
-        if self._max > 0:
-            if len(self) > self._max:
-                self.popitem(False)
-
-
-
-from string import Template as _Template
-
-class Template(_Template):
-	"""Custom string.Template class that supports addition of string and template"""
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-	def __add__(self, other):
-		if isinstance(other, _Template):
-			return Template(self.template + other.template)
-		return Template(self.template + str(other))
-
-
-
-from queue import Queue
-
-class Zfunc(object):
-	"""Thread safe sequncial printing/queue task handler class"""
-
-	__all__ = ["new", "update"]
-	def __init__(self, caller, store_return=False):
-		super().__init__()
-
-		self.queue = Queue()
-		# stores [args, kwargs], ...
-		self.store_return = store_return
-		self.returner = Queue()
-		# queue to store return value if store_return enabled
-
-		self.BUSY = False
-
-		self.caller = caller
-
-	def next(self):
-		""" check if any item in queje and call, if already running or queue empty, returns """
-		if self.queue.empty() or self.BUSY:
-			return None
-
-		self.BUSY = True
-		args, kwargs = self.queue.get()
-
-		x = self.caller(*args, **kwargs)
-		if self.store_return:
-			self.returner.put(x)
-
-		self.BUSY = False
-
-		if not self.queue.empty():
-			# will make the loop continue running
-			return True
-
-
-	def update(self, *args, **kwargs):
-		""" Uses xprint and parse string"""
-
-		self.queue.put((args, kwargs))
-		while self.next() is True:
-			# use while instead of recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion.... error
-			pass
-
-
-
-	def new(self, caller, store_return=False):
-		self.__init__(caller, store_return)
-
+from collections import OrderedDict
+
+
+class Callable_dict(dict):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.__dict__ = self
+
+	def __call__(self, *key):
+		return all([i in self for i in key])
+
+
+class GETdict(Callable_dict):
+	"""
+	to set item, use dict["key"] = value for the 1st time,
+	then use dict.key or dict["key"] to both get and set value
+
+	but using dick.key = value 1st, will assign it as attribute and its temporary
+	"""
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.__dict__ = self
+
+
+	def __setitem__(self, key, value):
+		super().__setitem__(key, value)
+
+	def __setattr__(self, key, value):
+		if self(key):
+			self.__setitem__(key, value)
+		else:
+			super().__setattr__(key, value)
+
+	def  __getattr__(self, __name: str):
+		if self(__name):
+			return self.__getitem__(__name)
+		return super().__getattribute__(__name)
+
+
+	# def __getitem__(self, __key):
+	# 	return super().__getitem__(__key)
+
+class Flag(GETdict):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.__dict__ = self
+
+	def __getitem__(self, __key):
+		return super().get(__key, None)
+
+	def  __getattr__(self, __name: str):
+		return super().get(__name, None)
+		# try:
+		# 	return super().__getitem__(__name)
+		# except Exception:
+		# 	return None
+
+
+class LimitedDict(OrderedDict):
+    def __init__(self, *args, max=0, **kwargs):
+        self._max = max
+        super().__init__(*args, **kwargs)
+
+    def __setitem__(self, key, value):
+        super().__setitem__(key, value)
+        if self._max > 0:
+            if len(self) > self._max:
+                self.popitem(False)
+
+
+
+from string import Template as _Template
+
+class Template(_Template):
+	"""Custom string.Template class that supports addition of string and template"""
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+
+	def __add__(self, other):
+		if isinstance(other, _Template):
+			return Template(self.template + other.template)
+		return Template(self.template + str(other))
+
+
+
+from queue import Queue
+
+class Zfunc(object):
+	"""Thread safe sequncial printing/queue task handler class"""
+
+	__all__ = ["new", "update"]
+	def __init__(self, caller, store_return=False):
+		super().__init__()
+
+		self.queue = Queue()
+		# stores [args, kwargs], ...
+		self.store_return = store_return
+		self.returner = Queue()
+		# queue to store return value if store_return enabled
+
+		self.BUSY = False
+
+		self.caller = caller
+
+	def next(self):
+		""" check if any item in queje and call, if already running or queue empty, returns """
+		if self.queue.empty() or self.BUSY:
+			return None
+
+		self.BUSY = True
+		args, kwargs = self.queue.get()
+
+		x = self.caller(*args, **kwargs)
+		if self.store_return:
+			self.returner.put(x)
+
+		self.BUSY = False
+
+		if not self.queue.empty():
+			# will make the loop continue running
+			return True
+
+
+	def update(self, *args, **kwargs):
+		""" Uses xprint and parse string"""
+
+		self.queue.put((args, kwargs))
+		while self.next() is True:
+			# use while instead of recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion.... error
+			pass
+
+
+
+	def new(self, caller, store_return=False):
+		self.__init__(caller, store_return)
+
```

### Comparing `pyrobox-0.9.4/src/pyroboxCore.py` & `pyrobox-0.9.5/src/pyroboxCore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,2147 +1,2147 @@
-import traceback
-import json
-import string
-import random
-import base64
-import re
-from http import HTTPStatus
-from http.cookies import SimpleCookie
-from functools import partial
-import contextlib
-import urllib.request
-import urllib.parse
-import time
-import sys
-import socketserver
-import socket  # For gethostbyaddr()
-import shutil
-import posixpath
-import mimetypes
-import io
-import http.client
-import html
-import email.utils
-import datetime
-import argparse
-from string import Template
-from typing import Union
-from queue import Queue
-import logging
-import atexit
-import os
-
-__version__ = "0.9.3"
-enc = "utf-8"
-DEV_MODE = False
-
-
-__all__ = [
-	"HTTPServer", "ThreadingHTTPServer", "BaseHTTPRequestHandler",
-	"SimpleHTTPRequestHandler",
-]
-
-
-logging.basicConfig(level=logging.INFO, format='%(levelname)s: \n%(message)s')
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
-# set INFO to see all the requests
-# set WARNING to see only the requests that made change to the server
-# set ERROR to see only the requests that made the errors
-
-
-endl = "\n"
-T = t = true = True  # too lazy to type
-F = f = false = False  # too lazy to type
-
-
-class Config:
-	def __init__(self):
-		# DEFAULT DIRECTORY TO LAUNCH SERVER
-		self.ftp_dir = "."  # DEFAULT DIRECTORY TO LAUNCH SERVER
-
-		self.IP = None  # will be assigned by checking
-		self.protocol = "http"  # DEFAULT PROTOCOL TO LAUNCH SERVER
-
-		# DEFAULT PORT TO LAUNCH SERVER
-		self.port = 6969  # DEFAULT PORT TO LAUNCH SERVER
-
-		# UPLOAD PASSWORD SO THAT ANYONE RANDOM CAN'T UPLOAD
-		# CAN BE CHANGED BY USING --password NEW_PASSWORD
-		self.PASSWORD = "SECret"
-
-		# LOGGING
-		self.log_location = "./"  # fallback log_location = "./"
-		# if you want to see some important LOG in browser, may contain your important information
-		self.allow_web_log = True
-		self.write_log = False  # if you want to write log to file
-		self.log_extra = True
-
-		# ZIP FEATURES
-		self.default_zip = "zipfile"  # or "zipfile" to use python built in zip module
-
-		# CHECK FOR MISSING REQUIREMENTS
-		self.run_req_check = True
-
-		# FILE INFO
-		self.MAIN_FILE = os.path.realpath(__file__)
-		self.MAIN_FILE_dir = os.path.dirname(self.MAIN_FILE)
-
-		# OS DETECTION
-		self.OS = self.get_os()
-
-		# RUNNING SERVER STATS
-		self.ftp_dir = self.get_default_dir()
-		self.dev_mode = DEV_MODE
-		self.ASSETS = False  # if you want to use assets folder, set this to True
-		self.ASSETS_dir = os.path.join(self.MAIN_FILE_dir, "/../assets/")
-		self.reload = False
-
-		self.disabled_func = {
-			"reload": False,
-		}
-
-		# TEMP FILE MAPPING
-		self.temp_file = set()
-
-		# CLEAN TEMP FILES ON EXIT
-		atexit.register(self.clear_temp)
-
-		# ASSET MAPPING
-		self.file_list = {}
-
-		# COMMANDLINE ARGUMENTS PARSER
-		self.parser = argparse.ArgumentParser(add_help=False)
-
-		# Default error message template
-		self.DEFAULT_ERROR_MESSAGE = Template("""
-		<!DOCTYPE HTML>
-		<html lang="en">
-		<html>
-			<head>
-				<meta charset="utf-8">
-				<title>Error response</title>
-			</head>
-			<body>
-				<h1>Error response</h1>
-				<p>Error code: ${code}</p>
-				<p>Message: ${message}</p>
-				<p>Error code explanation: ${code} - ${explain}</p>
-				<h3>PyroBox Version: ${version}</h3>
-			</body>
-		</html>
-		""")
-
-		self.DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
-
-	def clear_temp(self):
-		for i in self.temp_file:
-			try:
-				os.remove(i)
-			except OSError:
-				pass
-
-	def get_os(self):
-		from platform import system as platform_system
-
-		out = platform_system()
-		if out == "Linux" and hasattr(sys, 'getandroidapilevel'):
-			# self.IP = "192.168.43.1"
-			return 'Android'
-
-		return out
-
-	def get_default_dir(self):
-		if self.get_os()== 'Android':
-			return '/storage/emulated/0/'
-		return './'
-
-	def address(self):
-		return f"{self.protocol}://{self.IP}:{self.port}"
-
-	def parse_default_args(self, port=0, directory="", bind=None):
-		if not port:
-			port = self.port
-		if not directory:
-			directory = self.ftp_dir
-		if not bind:
-			bind = None
-
-		parser = self.parser
-
-		parser.add_argument('--bind', '-b',
-							metavar='ADDRESS', default=bind,
-							help='[xxx.xxx.xxx.xxx] Specify alternate bind address '
-								'[default: all interfaces]')
-		parser.add_argument('--directory', '-d', default=directory,
-							help='[Value] Specify alternative directory '
-								'[default: current directory]')
-		parser.add_argument('port', action='store',
-							default=port, type=int,
-							nargs='?',
-							help=f'[Value] Specify alternate port [default: {port}]')
-		parser.add_argument('--version', '-v', action='version',
-							version=__version__)
-
-		parser.add_argument('-h', '--help', action='help',
-								default='==SUPPRESS==',
-								help=('[Option] show this help message and exit'))
-
-
-		parser.add_argument('--no-extra-log',
-							action='store_true',
-							default=False,
-							help="[Flag] Disable file path and [= + - #] based logs (default: %(default)s)")
-
-
-		args = parser.parse_known_args()[0]
-
-		self.log_extra = not args.no_extra_log
-
-		return args
-
-
-class Tools:
-	def __init__(self):
-		self.styles = {
-			"equal": "=",
-			"star": "*",
-			"hash": "#",
-			"dash": "-",
-			"udash": "_"
-		}
-
-	@staticmethod
-	def term_width():
-		""" Return CLI screen size (if not found, returns default value)
-		"""
-		return shutil.get_terminal_size()[0]
-
-	def text_box(self, *text, style="equal", sep=" "):
-		"""
-		Returns a string of text with a border around it.
-		"""
-		text = sep.join(map(str, text))
-		term_col = shutil.get_terminal_size()[0]
-
-		s = self.styles[style] if style in self.styles else style
-		tt = ""
-		for i in text.split('\n'):
-			tt += i.center(term_col) + '\n'
-		return (f"\n\n{s*term_col}\n{tt}{s*term_col}\n\n")
-
-	@staticmethod
-	def random_string(length=10):
-		"""Generates a random string
-		length : length of string
-		"""
-		letters = string.ascii_lowercase
-		return ''.join(random.choice(letters) for i in range(length))
-
-
-tools = Tools()
-config = Config()
-
-
-
-class Callable_dict(dict):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-		self.__dict__ = self
-
-	def __call__(self, *key):
-		return all([i in self for i in key])
-
-
-
-
-def reload_server():
-	"""reload the server process from file"""
-	file = config.MAIN_FILE
-	logger.info("Reloading...\n" +
-				" ".join(
-					["RE-RUNNING: ", sys.executable,
-						sys.executable, file, *sys.argv[1:]]
-				))
-	try:
-		os.execl(sys.executable, sys.executable, file, *sys.argv[1:])
-	except OSError:
-		traceback.print_exc()
-	sys.exit(0)
-
-
-def null(*args, **kwargs):
-	pass
-
-
-class Zfunc(object):
-	"""Thread safe sequncial printing/queue task handler class"""
-
-	__all__ = ["new", "update"]
-
-	def __init__(self, caller, store_return=False):
-		super().__init__()
-
-		self.queue = Queue()
-		# stores [args, kwargs], ...
-		self.store_return = store_return
-		self.returner = Queue()
-		# queue to store return value if store_return enabled
-
-		self.BUSY = False
-
-		self.caller = caller
-
-	def next(self):
-		""" check if any item in queje and call, if already running or queue empty, returns """
-		if self.queue.empty() or self.BUSY:
-			return None
-
-		self.BUSY = True
-		args, kwargs = self.queue.get()
-
-		x = self.caller(*args, **kwargs)
-		if self.store_return:
-			self.returner.put(x)
-
-		self.BUSY = False
-
-		if not self.queue.empty():
-			# will make the loop continue running
-			return True
-
-	def update(self, *args, **kwargs):
-		""" Uses xprint and parse string"""
-
-		self.queue.put((args, kwargs))
-		while self.next() is True:
-			# use while instead of recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion.... error
-			pass
-
-	def new(self, caller, store_return=False):
-		self.__init__(caller=caller, store_return=store_return)
-
-	def destroy(self):
-		"""Clear the queue
-		however if running, caller function will still keep running till end"""
-		self.__init__(caller=null, store_return=False)
-
-
-"""HTTP server classes.
-
-Note: BaseHTTPRequestHandler doesn't implement any HTTP request; see
-SimpleHTTPRequestHandler for simple implementations of GET, HEAD and POST,
-and CGIHTTPRequestHandler for CGI scripts.
-
-It does, however, optionally implement HTTP/1.1 persistent connections,
-as of version 0.3.
-
-XXX To do:
-
-- log requests even later (to capture byte count)
-- log user-agent header and other interesting goodies
-- send error log to separate file
-"""
-
-
-##############################################
-#         PAUSE AND RESUME FEATURE           #
-##############################################
-
-def copy_byte_range(infile, outfile, start=None, stop=None, bufsize=16*1024):
-	'''
-	TO SUPPORT PAUSE AND RESUME FEATURE
-	Like shutil.copyfileobj, but only copy a range of the streams.
-	Both start and stop are inclusive.
-	'''
-	if start is not None:
-		infile.seek(start)
-	while 1:
-		to_read = min(bufsize, stop + 1 - infile.tell() if stop else bufsize)
-		buf = infile.read(to_read)
-		if not buf:
-			break
-		outfile.write(buf)
-
-
-BYTE_RANGE_RE = re.compile(r'bytes=(\d+)-(\d+)?$')
-
-
-def parse_byte_range(byte_range):
-	'''Returns the two numbers in 'bytes=123-456' or throws ValueError.
-	The last number or both numbers may be None.
-	'''
-	if byte_range.strip() == '':
-		return None, None
-
-	m = BYTE_RANGE_RE.match(byte_range)
-	if not m:
-		raise ValueError(f'Invalid byte range {byte_range}')
-
-	# first, last = [x and int(x) for x in m.groups()] #
-
-	first, last = map((lambda x: int(x) if x else None), m.groups())
-
-	if last and last < first:
-		raise ValueError(f'Invalid byte range { byte_range}')
-	return first, last
-
-# ---------------------------x--------------------------------
-
-
-def URL_MANAGER(url: str):
-	"""
-	returns a tuple of (`path`, `query_dict`, `fragment`)\n
-
-	`url` = `'/store?page=10&limit=15&price=ASC#dskjfhs'`\n
-	`path` = `'/store'` or `/`\n
-	`query_dict` = `{'page': ['10'], 'limit': ['15'], 'price': ['ASC']}`\n
-	`fragment` = `dskjfhs`\n
-	"""
-
-	# url = '/store?page=10&limit=15&price#dskjfhs'
-	parse_result = urllib.parse.urlparse(url)
-
-	path = parse_result.path
-	if path == '':
-		path = '/'
-
-	dict_result = Callable_dict(urllib.parse.parse_qs(
-		parse_result.query, keep_blank_values=True))
-
-	return (path, dict_result, parse_result.fragment)
-
-if __name__ == "__main__":
-	print(URL_MANAGER('https://www.google.com'))
-	print(URL_MANAGER('https://www.google.com/store?page=10&limit=15&price=ASC#dskjfhs'))
-
-
-class HTTPServer(socketserver.TCPServer):
-
-	allow_reuse_address = True  # Seems to make sense in testing environment
-
-	def server_bind(self):
-		"""Override server_bind to store the server name."""
-		socketserver.TCPServer.server_bind(self)
-		host, port = self.server_address[:2]
-		self.server_name = socket.getfqdn(host)
-		self.server_port = port
-
-
-class ThreadingHTTPServer(socketserver.ThreadingMixIn, HTTPServer):
-	daemon_threads = True
-
-
-class BaseHTTPRequestHandler(socketserver.StreamRequestHandler):
-
-	"""HTTP request handler base class.
-
-	The various request details are stored in instance variables:
-
-	- client_address is the client IP address in the form (host,
-	port);
-
-	- command, path and version are the broken-down request line;
-
-	- headers is an instance of email.message.Message (or a derived
-	class) containing the header information;
-
-	- rfile is a file object open for reading positioned at the
-	start of the optional input data part;
-
-	- wfile is a file object open for writing.
-
-	IT IS IMPORTANT TO ADHERE TO THE PROTOCOL FOR WRITING!
-
-	The first thing to be written must be the response line.  Then
-	follow 0 or more header lines, then a blank line, and then the
-	actual data (if any).  The meaning of the header lines depends on
-	the command executed by the server; in most cases, when data is
-	returned, there should be at least one header line of the form
-
-	Content-type: <type>/<subtype>
-
-	where <type> and <subtype> should be registered MIME types,
-	e.g. "text/html" or "text/plain".
-
-	"""
-
-	# The Python system version, truncated to its first component.
-	sys_version = "Python/" + sys.version.split()[0]
-
-	# The server software version.  You may want to override this.
-	# The format is multiple whitespace-separated strings,
-	# where each string is of the form name[/version].
-	server_version = "BaseHTTP/" + __version__
-
-
-	# The default request version.  This only affects responses up until
-	# the point where the request line is parsed, so it mainly decides what
-	# the client gets back when sending a malformed request line.
-	# Most web servers default to HTTP 0.9, i.e. don't send a status line.
-	default_request_version = "HTTP/0.9"
-
-	def parse_request(self):
-		"""Parse a request (internal).
-
-		The request should be stored in self.raw_requestline; the results
-		are in self.command, self.path, self.request_version and
-		self.headers.
-
-		Return True for success, False for failure; on failure, any relevant
-		error response has already been sent back.
-
-		"""
-		self.command = ''  # set in case of error on the first line
-		self.request_version = version = self.default_request_version
-		self.close_connection = True
-		self.header_flushed = False # true when headers are flushed by self.flush_headers()
-		self.response_code_sent = False # true when response code (>=200) is sent by self.send_response()
-
-
-		requestline = str(self.raw_requestline, 'iso-8859-1')
-		requestline = requestline.rstrip('\r\n')
-		self.requestline = requestline
-		words = requestline.split()
-		if len(words) == 0:
-			return False
-
-		if len(words) >= 3:  # Enough to determine protocol version
-			version = words[-1]
-			try:
-				if not version.startswith('HTTP/'):
-					raise ValueError
-				base_version_number = version.split('/', 1)[1]
-				version_number = base_version_number.split(".")
-				# RFC 2145 section 3.1 says there can be only one "." and
-				#   - major and minor numbers MUST be treated as
-				#     separate integers;
-				#   - HTTP/2.4 is a lower version than HTTP/2.13, which in
-				#     turn is lower than HTTP/12.3;
-				#   - Leading zeros MUST be ignored by recipients.
-				if len(version_number) != 2:
-					raise ValueError
-				version_number = int(version_number[0]), int(version_number[1])
-			except (ValueError, IndexError):
-				self.send_error(
-					HTTPStatus.BAD_REQUEST,
-					"Bad request version (%r)" % version)
-				return False
-			if version_number >= (1, 1) and self.protocol_version >= "HTTP/1.1":
-				self.close_connection = False
-			if version_number >= (2, 0):
-				self.send_error(
-					HTTPStatus.HTTP_VERSION_NOT_SUPPORTED,
-					"Invalid HTTP version (%s)" % base_version_number)
-				return False
-			self.request_version = version
-
-		if not 2 <= len(words) <= 3:
-			self.send_error(
-				HTTPStatus.BAD_REQUEST,
-				"Bad request syntax (%r)" % requestline)
-			return False
-		command, path = words[:2]
-		if len(words) == 2:
-			self.close_connection = True
-			if command != 'GET':
-				self.send_error(
-					HTTPStatus.BAD_REQUEST,
-					"Bad HTTP/0.9 request type (%r)" % command)
-				return False
-		self.command, self.path = command, path
-
-
-		# gh-87389: The purpose of replacing '//' with '/' is to protect
-		# against open redirect attacks possibly triggered if the path starts
-		# with '//' because http clients treat //path as an absolute URI
-		# without scheme (similar to http://path) rather than a path.
-		if self.path.startswith('//'):
-			self.path = '/' + self.path.lstrip('/')  # Reduce to a single /
-
-		# Examine the headers and look for a Connection directive.
-		try:
-			self.headers = http.client.parse_headers(self.rfile,
-													 _class=self.MessageClass)
-		except http.client.LineTooLong as err:
-			self.send_error(
-				HTTPStatus.REQUEST_HEADER_FIELDS_TOO_LARGE,
-				"Line too long",
-				str(err))
-			return False
-		except http.client.HTTPException as err:
-			self.send_error(
-				HTTPStatus.REQUEST_HEADER_FIELDS_TOO_LARGE,
-				"Too many headers",
-				str(err)
-			)
-			return False
-
-		conntype = self.headers.get('Connection', "")
-		if conntype.lower() == 'close':
-			self.close_connection = True
-		elif (conntype.lower() == 'keep-alive' and
-			  self.protocol_version >= "HTTP/1.1"):
-			self.close_connection = False
-
-		# Load cookies from request
-		# Uses standard SimpleCookie
-		# doc: https://docs.python.org/3/library/http.cookies.html
-		self.cookie = SimpleCookie()
-		self.cookie.load(self.headers.get('Cookie', ""))
-		# print(tools.text_box("Cookie: ", self.cookie))
-
-		# Examine the headers and look for an Expect directive
-		expect = self.headers.get('Expect', "")
-		if (expect.lower() == "100-continue" and
-			self.protocol_version >= "HTTP/1.1" and
-				self.request_version >= "HTTP/1.1"):
-			if not self.handle_expect_100():
-				return False
-		return True
-
-	def handle_expect_100(self):
-		"""Decide what to do with an "Expect: 100-continue" header.
-
-		If the client is expecting a 100 Continue response, we must
-		respond with either a 100 Continue or a final response before
-		waiting for the request body. The default is to always respond
-		with a 100 Continue. You can behave differently (for example,
-		reject unauthorized requests) by overriding this method.
-
-		This method should either return True (possibly after sending
-		a 100 Continue response) or send an error response and return
-		False.
-
-		"""
-		self.send_response_only(HTTPStatus.CONTINUE)
-		self.end_headers()
-		return True
-
-	def handle_one_request(self):
-		"""Handle a single HTTP request.
-
-		You normally don't need to override this method; see the class
-		__doc__ string for information on how to handle specific HTTP
-		commands such as GET and POST.
-
-		"""
-		try:
-			self.raw_requestline = self.rfile.readline(65537)
-			if len(self.raw_requestline) > 65536:
-				self.requestline = ''
-				self.request_version = ''
-				self.command = ''
-				self.send_error(HTTPStatus.REQUEST_URI_TOO_LONG)
-				return
-			if not self.raw_requestline:
-				self.close_connection = True
-				return
-			if not self.parse_request():
-				# An error code has been sent, just exit
-				return
-			mname = 'do_' + self.command
-			if not hasattr(self, mname):
-				self.send_error(
-					HTTPStatus.NOT_IMPLEMENTED,
-					"Unsupported method (%r)" % self.command)
-				return
-			method = getattr(self, mname)
-
-			url_path, query, fragment = URL_MANAGER(self.path)
-			self.url_path = url_path
-			self.query = query
-			self.fragment = fragment
-
-			self.use_range = False
-
-			_hash = abs(hash((self.raw_requestline, tools.random_string(10))))
-			self.req_hash = base64.b64encode(
-					str(_hash).encode('ascii')
-				).decode()[:10]
-
-			_w = tools.term_width()
-			w = _w - len(str(self.req_hash)) - 2
-			w = w//2
-			if config.log_extra:
-				logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n' +
-						'\n'.join(
-								[f'{self.req_hash}|=>\t request\t: {self.command}',
-								 f'{self.req_hash}|=>\t url     \t: {url_path}',
-								 f'{self.req_hash}|=>\t query   \t: {query}',
-								 f'{self.req_hash}|=>\t fragment\t: {fragment}',
-								 f'{self.req_hash}|=>\t full url \t: {self.path}',
-								 ]) + '\n' +
-						'+'*w + f' {self.req_hash} ' + '+'*w
-						)
-
-			try:
-				method()
-			except Exception:
-				traceback.print_exc()
-
-			if config.log_extra:
-				logger.info('-'*w + f' {self.req_hash} ' + '-'*w + '\n' +
-						'#'*_w
-						)
-
-			# actually send the response if not already done.
-			self.wfile.flush()
-
-		except (TimeoutError, socket.timeout) as e:
-			# a read or a write timed out.  Discard this connection
-			self.log_error("Request timed out:", e)
-			self.close_connection = True
-			return
-
-	def handle(self):
-		"""Handle multiple requests if necessary."""
-		self.close_connection = True
-
-		self.handle_one_request()
-		while not self.close_connection:
-			self.handle_one_request()
-
-	def send_error(self, code, message=None, explain=None, error_message_format: Template = None, cookie:Union[SimpleCookie, str]=None):
-		"""Send and log an error reply.
-
-		Arguments are
-		* code:	an HTTP error code
-					3 digits
-		* message: a simple optional 1 line reason phrase.
-					*( HTAB / SP / VCHAR / %x80-FF )
-					defaults to short entry matching the response code
-		* explain: a detailed message defaults to the long entry
-					matching the response code.
-		* error_message_format: a `string.Template` for the error message
-					defaults to `config.DEFAULT_ERROR_MESSAGE`
-
-					auto-formatting values:
-						`${code}`: the HTTP error code
-						`${message}`: the HTTP error message
-						`${explain}`: the detailed error message
-						`${version}`: the server software version string
-
-		This sends an error response (so it must be called before any
-		output has been generated), logs the error, and finally sends
-		a piece of HTML explaining the error to the user.
-
-		"""
-
-		error_message_format = error_message_format if error_message_format else config.DEFAULT_ERROR_MESSAGE
-
-		error_content_type = config.DEFAULT_ERROR_CONTENT_TYPE
-
-		try:
-			shortmsg, longmsg = self.responses[code]
-		except KeyError:
-			shortmsg, longmsg = '???', '???'
-		if message is None:
-			message = shortmsg
-		if explain is None:
-			explain = longmsg
-		self.log_error("code", code, "message", message)
-		self.send_response(code, message)
-
-		self._send_cookie(cookie=cookie)
-
-		self.send_header('Connection', 'close')
-
-		# Message body is omitted for cases described in:
-		#  - RFC7230: 3.3. 1xx, 204(No Content), 304(Not Modified)
-		#  - RFC7231: 6.3.6. 205(Reset Content)
-		body = None
-		if (code >= 200 and
-				code not in (HTTPStatus.NO_CONTENT,
-							 HTTPStatus.RESET_CONTENT,
-							 HTTPStatus.NOT_MODIFIED)):
-			# HTML encode to prevent Cross Site Scripting attacks
-			# (see bug #1100201)
-			content = (error_message_format.safe_substitute(
-				code=code,
-				message=html.escape(message, quote=False),
-				explain=html.escape(explain, quote=False),
-				version=__version__
-			))
-			body = content.encode('UTF-8', 'replace')
-			self.send_header("Content-Type", error_content_type)
-			self.send_header('Content-Length', str(len(body)))
-		self.end_headers()
-
-		if self.command != 'HEAD' and body:
-			self.wfile.write(body)
-
-	def send_response(self, code, message=None):
-		"""Add the response header to the headers buffer and log the
-		response code.
-
-		Also send two standard headers with the server software
-		version and the current date.
-
-		"""
-		if self.response_code_sent:
-			return
-
-		if not code//100 ==1: # 1xx - Informational (allowes multiple responses)
-			self.response_code_sent = True
-
-		self.log_request(code)
-		self.send_response_only(code, message)
-		self.send_header('Server', self.version_string())
-		self.send_header('Date', self.date_time_string())
-
-	def send_response_only(self, code, message=None):
-		"""Send the response header only."""
-		if self.request_version != 'HTTP/0.9':
-			if message is None:
-				if code in self.responses:
-					message = self.responses[code][0]
-				else:
-					message = ''
-			if not hasattr(self, '_headers_buffer'):
-				self._headers_buffer = []
-			self._headers_buffer.append(("%s %d %s\r\n" %
-				(self.protocol_version, code, message)).encode(
-				'utf-8', 'strict'))
-
-	def send_header_string(self, lines:str):
-		"""Send a header multiline string to the headers buffer."""
-		for i in lines.split("\r\n"):
-			if not i:
-				continue
-			tag, _, msg = i.partition(":")
-			self.send_header(tag.strip(), msg.strip())
-
-
-	def _send_cookie(self, cookie:Union[SimpleCookie, str]=None):
-		"""Must send cookie after self.send_response(XXX)"""
-		if cookie is not None:
-			if isinstance(cookie, SimpleCookie):
-				cookie = cookie.output()
-
-			self.send_header_string(cookie)
-
-
-
-
-	def send_header(self, keyword, value):
-		"""Send a MIME header to the headers buffer."""
-		if self.request_version != 'HTTP/0.9':
-			if not hasattr(self, '_headers_buffer'):
-				self._headers_buffer = []
-			self._headers_buffer.append(
-				("%s: %s\r\n" % (keyword, value)).encode('utf-8', 'strict'))
-
-		if keyword.lower() == 'connection':
-			if value.lower() == 'close':
-				self.close_connection = True
-			elif value.lower() == 'keep-alive':
-				self.close_connection = False
-
-	def end_headers(self):
-		"""Send the blank line ending the MIME headers."""
-		if self.request_version != 'HTTP/0.9':
-			self._headers_buffer.append(b"\r\n")
-			self.flush_headers()
-
-	def flush_headers(self):
-		"""Flush the headers buffer."""
-		if self.header_flushed:
-			try:
-				raise RuntimeError("Headers already flushed")
-			except RuntimeError:
-				traceback.print_exc()
-			return
-		if hasattr(self, '_headers_buffer'):
-			self.wfile.write(b"".join(self._headers_buffer))
-			self._headers_buffer = []
-
-		self.header_flushed = True
-
-	def log_request(self, code='-', size='-'):
-		"""Log an accepted request.
-
-		This is called by send_response().
-
-		"""
-		if isinstance(code, HTTPStatus):
-			code = code.value
-		self.log_message(f'"{self.requestline}"', code, size)
-
-	def log_error(self, *args, **kwargs):
-		"""Log an error. [ERROR PRIORITY]
-
-		This is called when a request cannot be fulfilled.  By
-		default it passes the message on to log_message().
-
-		Arguments are the same as for log_message().
-
-		XXX This should go to the separate error log.
-
-		"""
-		self.log_message(*args, **kwargs, error=True)
-
-	def log_warning(self, *args, **kwargs):
-		"""Log a warning message [HIGH PRIORITY]"""
-		self.log_message(*args, **kwargs, warning=True)
-
-	def log_debug(self, *args, write=True, **kwargs):
-		"""Log a debug message [LOWEST PRIORITY]"""
-		self.log_message(*args, **kwargs, debug=True, write=write)
-
-	def log_info(self, *args, write=False, **kwargs):
-		"""Default log message [MEDIUM PRIORITY]"""
-		self.log_message(*args, **kwargs, write=write)
-
-	def _log_writer(self, message):
-		os.makedirs(config.log_location, exist_ok=True)
-		with open(config.log_location + 'log.txt', 'a+') as f:
-			f.write(
-				(f"#{self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"))
-
-	def log_message(self, *args, error=False, warning=False, debug=False, write=True, **kwargs):
-		"""Log an arbitrary message.
-
-		This is used by all other logging functions.  Override
-		it if you have specific logging wishes.
-
-		The client ip and current date/time are prefixed to
-		every message.
-
-		"""
-		if not args:
-			return
-
-		sep = kwargs.get('sep', ' ')
-		end = kwargs.get('end', '\n')
-
-		message = sep.join(map(str, args)) + end
-
-		message = f"# {self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"
-
-		if error:
-			logger.error(message)
-		elif warning:
-			logger.warning(message)
-		elif debug:
-			logger.debug(message)
-		else:
-			logger.info(message)
-
-		if not config.write_log:
-			return
-
-		if not hasattr(self, "Zlog_writer"):
-			self.Zlog_writer = Zfunc(self._log_writer)
-
-		try:
-			self.Zlog_writer.update(message)
-		except Exception:
-			traceback.print_exc()
-
-	def version_string(self):
-		"""Return the server software version string."""
-		return self.server_version + ' ' + self.sys_version
-
-	def date_time_string(self, timestamp=None):
-		"""Return the current date and time formatted for a message header."""
-		if timestamp is None:
-			timestamp = time.time()
-		return email.utils.formatdate(timestamp, usegmt=True)
-
-	def log_date_time_string(self):
-		"""Return the current time formatted for logging."""
-		now = time.time()
-		year, month, day, hh, mm, ss, x, y, z = time.localtime(now)
-		s = "%02d/%3s/%04d %02d:%02d:%02d" % (
-			day, self.monthname[month], year, hh, mm, ss)
-		return s
-
-	weekdayname = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
-
-	monthname = [None,
-				 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
-				 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
-
-	def address_string(self):
-		"""Return the client address."""
-
-		return self.client_address[0]
-
-	# Essentially static class variables
-
-	# The version of the HTTP protocol we support.
-	# Set this to HTTP/1.1 to enable automatic keepalive
-	protocol_version = "HTTP/1.0"
-
-	# MessageClass used to parse headers
-	MessageClass = http.client.HTTPMessage
-
-	# hack to maintain backwards compatibility
-	responses = {
-		v: (v.phrase, v.description)
-		for v in HTTPStatus.__members__.values()
-	}
-
-
-class SimpleHTTPRequestHandler(BaseHTTPRequestHandler):
-
-	"""Simple HTTP request handler with GET and HEAD commands.
-
-	This serves files from the current directory and any of its
-	subdirectories.  The MIME type for files is determined by
-	calling the .guess_type() method.
-
-	The GET and HEAD requests are identical except that the HEAD
-	request omits the actual contents of the file.
-
-	"""
-
-	server_version = "SimpleHTTP/" + __version__
-
-	if not mimetypes.inited:
-		mimetypes.init()  # try to read system mime.types
-	extensions_map = mimetypes.types_map.copy()
-	extensions_map.update({
-		'': 'application/octet-stream',  # Default
-			'.py': 'text/x-python',
-			'.c': 'text/x-c',
-			'.h': 'text/x-c',
-			'.css': 'text/css',
-
-			'.gz': 'application/gzip',
-			'.Z': 'application/octet-stream',
-			'.bz2': 'application/x-bzip2',
-			'.xz': 'application/x-xz',
-
-			'.webp': 'image/webp',
-
-			'opus': 'audio/opus',
-			'.oga': 'audio/ogg',
-			'.wav': 'audio/wav',
-
-			'.ogv': 'video/ogg',
-			'.ogg': 'application/ogg',
-			'm4a': 'audio/mp4',
-	})
-
-	handlers = {
-		'HEAD': [],
-		'POST': [],
-	}
-
-	def __init__(self, *args, directory=None, **kwargs):
-		if directory is None:
-			directory = os.getcwd()
-		# os.fspath() same as directory, but str, new in 3.6
-		self.directory = os.fspath(directory)
-		super().__init__(*args, **kwargs)
-		self.query = Callable_dict()
-
-	def do_GET(self):
-		"""Serve a GET request."""
-		try:
-			resp = self.send_head()
-		except Exception as e:
-			traceback.print_exc()
-			self.send_error(500, str(e))
-			return
-
-		if resp:
-			try:
-				self.copyfile(resp, self.wfile)
-			except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-				self.log_info(tools.text_box(e.__class__.__name__,
-							  e, "\nby ", self.address_string()))
-			finally:
-				resp.close()
-
-	def do_(self):
-		'''incase of errored request'''
-		self.send_error(HTTPStatus.BAD_REQUEST, "Bad request.")
-
-	@staticmethod
-	def on_req(type='', url='', hasQ=(), QV={}, fragent='', url_regex='', func=null):
-		'''called when request is received
-		type: GET, POST, HEAD, ...
-		url: url (must start with /)
-		hasQ: if url has query
-		QV: match query value
-		fragent: fragent of request
-		url_regex: url regex (must start with /) url regex, the url must start and end with this regex
-
-		if query is tuple|list, it will only check existence of key
-		if query is dict, it will check value of key
-		'''
-		self = __class__
-
-		type = type.upper()
-		if type == 'GET':
-			type = 'HEAD'
-
-		if type not in self.handlers:
-			self.handlers[type] = []
-
-		# FIXING TYPE ISSUE
-		if isinstance(hasQ, str):
-			hasQ = (hasQ,)
-
-		if url == '' and url_regex == '':
-			url_regex = '.*'
-
-		to_check = (url, hasQ, QV, fragent, url_regex)
-
-		def decorator(func):
-			self.handlers[type].append((to_check, func))
-			return func
-		return decorator
-
-	def test_req(self, url='', hasQ=(), QV={}, fragent='', url_regex=''):
-		'''test if request is matched'
-
-		args:
-			url: url relative path (must start with /)
-			hasQ: if url has query
-			QV: match query value
-			fragent: fragent of request
-			url_regex: url regex, the url must start and end with this regex
-
-
-		'''
-		if url_regex and not re.search("^"+url_regex+'$', self.url_path):
-				return False
-		if url and url != self.url_path:
-			return False
-
-		if isinstance(hasQ, str):
-			hasQ = (hasQ,)
-
-		if hasQ and self.query(*hasQ) is False:
-			return False
-		if QV:
-			for k, v in QV.items():
-				if not self.query(k):
-					return False
-				if self.query[k] != v:
-					return False
-
-		if fragent and self.fragment != fragent:
-			return False
-
-		return True
-
-	def do_HEAD(self):
-		"""Serve a HEAD request."""
-		resp = None
-		try:
-			resp = self.send_head()
-		except Exception as e:
-			traceback.print_exc()
-			self.send_error(500, str(e))
-			return
-		finally:
-			if resp:
-				resp.close()
-
-	def do_POST(self):
-		"""Serve a POST request."""
-		self.range = None, None
-
-		path = self.translate_path(self.path)
-		# DIRECTORY DONT CONTAIN SLASH / AT END
-
-		url_path, query, fragment = self.url_path, self.query, self.fragment
-		spathsplit = self.url_path.split("/")
-
-		try:
-			for case, func in self.handlers['POST']:
-				if self.test_req(*case):
-					try:
-						resp = func(self, url_path=url_path, query=query,
-								fragment=fragment, path=path, spathsplit=spathsplit)
-					except PostError:
-						traceback.print_exc()
-						# break if error is raised and send BAD_REQUEST (at end of loop)
-						break
-
-					if resp:
-						try:
-							self.copyfile(resp, self.wfile)
-						except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-							logger.info(tools.text_box(
-								e.__class__.__name__, e, "\nby ", [self.address_string()]))
-						finally:
-							resp.close()
-					return
-
-			return self.send_error(HTTPStatus.BAD_REQUEST, "Invalid request.")
-
-		except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
-			logger.info(tools.text_box(e.__class__.__name__,
-						e, "\nby ", [self.address_string()]))
-			return
-		except Exception as e:
-			traceback.print_exc()
-			self.send_error(500, str(e))
-			return
-
-	def redirect(self, location, cookie:Union[SimpleCookie, str]=None):
-		'''redirect to location'''
-		print("REDIRECT ", location)
-		self.send_response(302)
-		self.send_header("Location", location)
-		self._send_cookie(cookie)
-		self.end_headers()
-
-
-
-	def return_txt(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
-		'''returns only the head to client
-		and returns a file object to be used by copyfile'''
-		self.log_debug(f'[RETURNED] {code} to client')
-		if isinstance(msg, Template):
-			msg = msg.safe_substitute(
-				code=code,
-				message=HTTPStatus(code).phrase,
-				explain=HTTPStatus(code).description,
-				version=__version__
-			)
-		if not isinstance(msg, bytes):
-			encoded = msg.encode('utf-8', 'surrogateescape')
-		else:
-			encoded = msg
-
-		box = io.BytesIO()
-		box.write(encoded)
-		box.seek(0)
-
-		self.send_response(code)
-
-		self._send_cookie(cookie)
-
-
-
-		self.send_header("Content-Type", content_type)
-		self.send_header("Content-Length", str(len(encoded)))
-		self.end_headers()
-		return box
-
-	def send_txt(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
-		'''sends the head and file to client'''
-		file = self.return_txt(msg, code, content_type, cookie)
-		if self.command == "HEAD":
-			return  # to avoid sending file on get request
-		self.copyfile(file, self.wfile)
-		file.close()
-
-	def send_text(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
-		'''proxy to send_txt'''
-		self.send_txt(msg, code, content_type, cookie)
-
-	def return_script(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/javascript; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
-		'''proxy to send_txt'''
-		return self.return_txt(msg, code, content_type, cookie)
-
-	def send_script(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/javascript; charset=utf-8"):
-		'''proxy to send_txt'''
-		return self.send_txt(msg, code, content_type)
-
-	def return_css(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/css; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
-		'''proxy to send_txt'''
-		return self.return_txt(msg, code, content_type, cookie)
-
-	def send_css(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/css; charset=utf-8"):
-		'''proxy to send_txt'''
-		return self.send_txt(msg, code, content_type)
-
-	def send_json(self, obj:Union[object, str, bytes], code=200, cookie:Union[SimpleCookie, str]=None):
-		"""send object as json
-		obj: json-able object or json.dumps() string"""
-		if not isinstance(obj, str):
-			obj = json.dumps(obj, indent=1)
-		file = self.return_txt(obj, code, content_type="application/json", cookie=cookie)
-		if self.command == "HEAD":
-			return  # to avoid sending file on get request
-		self.copyfile(file, self.wfile)
-		file.close()
-
-	def return_file(self, path, filename=None, download=False, cache_control="", cookie:Union[SimpleCookie, str]=None):
-		file = None
-		is_attachment = "attachment;" if (self.query("dl") or download) else ""
-
-		first, last = 0, None
-
-		C_encoding = None
-
-		try:
-			ctype = self.guess_type(path)
-
-			# make sure texts are sent as utf-8
-			if ctype.startswith("text/"):
-				ctype += "; charset=utf-8"
-
-			# if file is gziped, send as gzip
-			if ctype == "application/gzip" and "gzip" in self.headers.get("Accept-Encoding", ""):
-				C_encoding = "gzip"
-
-			file = open(path, 'rb')
-			fs = os.fstat(file.fileno())
-
-			file_len = fs[6]
-			# Use browser cache if possible
-			if ("If-Modified-Since" in self.headers
-					and "If-None-Match" not in self.headers):
-				# compare If-Modified-Since and time of last file modification
-				try:
-					ims = email.utils.parsedate_to_datetime(
-						self.headers["If-Modified-Since"])
-				except (TypeError, IndexError, OverflowError, ValueError):
-					# ignore ill-formed values
-					pass
-				else:
-					if ims.tzinfo is None:
-						# obsolete format with no timezone, cf.
-						# https://tools.ietf.org/html/rfc7231#section-7.1.1.1
-						ims = ims.replace(tzinfo=datetime.timezone.utc)
-					if ims.tzinfo is datetime.timezone.utc:
-						# compare to UTC datetime of last modification
-						last_modif = datetime.datetime.fromtimestamp(
-							fs.st_mtime, datetime.timezone.utc)
-						# remove microseconds, like in If-Modified-Since
-						last_modif = last_modif.replace(microsecond=0)
-
-						if last_modif <= ims:
-							self.send_response(HTTPStatus.NOT_MODIFIED)
-							self.end_headers()
-							file.close()
-
-							return None
-
-			if self.use_range:
-				first = self.range[0]
-				if first is None:
-					first = 0
-				last = self.range[1]
-				if last is None or last >= file_len:
-					last = file_len - 1
-
-				if first >= file_len:  # PAUSE AND RESUME SUPPORT
-					self.send_error(416, 'Requested Range Not Satisfiable', cookie=cookie)
-					return None
-
-				self.send_response(206)
-				self._send_cookie(cookie=cookie)
-
-				self.send_header('Accept-Ranges', 'bytes')
-
-				response_length = last - first + 1
-
-				self.send_header('Content-Range',
-								f'bytes {first}-{last}/{file_len}')
-				self.send_header('Content-Length', str(response_length))
-
-			else:
-				self.send_response(HTTPStatus.OK)
-				self._send_cookie(cookie)
-
-				self.send_header("Content-Length", str(file_len))
-
-			if cache_control:
-				self.send_header("Cache-Control", cache_control)
-
-			self.send_header("Last-Modified",
-							self.date_time_string(fs.st_mtime))
-			self.send_header("Content-Type", ctype)
-
-			if C_encoding:
-				self.send_header("Content-Encoding", C_encoding)
-
-			self.send_header("Content-Disposition", is_attachment+' filename="%s"' %
-							(os.path.basename(path) if filename is None else filename))
-			self.end_headers()
-
-			return file
-
-		except PermissionError:
-			self.send_error(HTTPStatus.FORBIDDEN, "Permission denied", cookie)
-			return None
-
-		except OSError:
-			self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie)
-			return None
-
-		except Exception:
-			traceback.print_exc()
-
-			# if f and not f.closed(): f.close()
-			raise
-
-	def send_file(self, path, filename=None, download=False, cache_control='', cookie:Union[SimpleCookie, str]=None):
-		'''sends the head and file to client'''
-		file = self.return_file(path, filename, download, cache_control, cookie=cookie)
-		if self.command == "HEAD":
-			return  # to avoid sending file on get request
-		try:
-			self.copyfile(file, self.wfile)
-		finally:
-			file.close()
-
-
-	def send_head(self):
-		"""Common code for GET and HEAD commands.
-
-		This sends the response code and MIME headers.
-
-		Return value is either a file object (which has to be copied
-		to the outputfile by the caller unless the command was HEAD,
-		and must be closed by the caller under all circumstances), or
-		None, in which case the caller has nothing further to do.
-
-		"""
-
-		if 'Range' not in self.headers:
-			self.range = None, None
-			first, last = 0, 0
-
-		else:
-			try:
-				self.range = parse_byte_range(self.headers['Range'])
-				first, last = self.range
-				self.use_range = True
-			except ValueError as e:
-				self.send_error(400, 'Invalid byte range')
-				return None
-
-		path = self.translate_path(self.path)
-		# DIRECTORY DONT CONTAIN SLASH / AT END
-
-		url_path, query, fragment = self.url_path, self.query, self.fragment
-
-		spathsplit = self.url_path.split("/")
-
-		# GET WILL Also BE HANDLED BY HEAD
-		for case, func in self.handlers['HEAD']:
-			if self.test_req(*case):
-				return func(self, url_path=url_path, query=query, fragment=fragment, path=path, spathsplit=spathsplit)
-
-		return self.send_error(HTTPStatus.NOT_FOUND, "File not found")
-
-	def get_displaypath(self, url_path):
-		"""
-		Helper to produce a display path for the directory listing.
-		"""
-
-		try:
-			displaypath = urllib.parse.unquote(
-				url_path, errors='surrogatepass')
-		except UnicodeDecodeError:
-			displaypath = urllib.parse.unquote(url_path)
-		displaypath = html.escape(displaypath, quote=False)
-
-		return displaypath
-
-	def get_rel_path(self, filename):
-		"""Return the relative path to the file, FOR WEB."""
-		return urllib.parse.unquote(posixpath.join(self.url_path, filename), errors='surrogatepass')
-	
-	def get_web_path(self, path:str, times=1):
-		"""replace current directory with /"""
-		return path.replace(self.directory, "/", times)
-	
-	def path_safety_check(self, paths:Union[str, list], *more_paths:Union[str, list]):
-		"""check if path is safe
-		paths: list of paths to check"""
-		if isinstance(paths, str):
-			paths = [paths]
-
-		if more_paths:
-			for path in more_paths:
-				if isinstance(path, str):
-					paths.append(path)
-				elif isinstance(path, (list, tuple, set)):
-					paths += more_paths
-				else:
-					raise TypeError(f"Invalid type {type(path)} for path")
-
-
-		for path in paths:
-			if path.startswith(('../', '..\\', '/../', '\\..\\')) or '/../' in path or '\\..\\' in path or path.endswith(('/..', '\\..')):
-				return False
-			
-		return True
-
-
-		
-
-	def translate_path(self, path):
-		"""Translate a /-separated PATH to the local filename syntax.
-
-		Components that mean special things to the local file system
-		(e.g. drive or directory names) are ignored.  (XXX They should
-		probably be diagnosed.)
-
-		"""
-		# abandon query parameters
-		path = path.split('?', 1)[0]
-		path = path.split('#', 1)[0]
-		# Don't forget explicit trailing slash when normalizing. Issue17324
-		trailing_slash = path.rstrip().endswith('/')
-
-		try:
-			path = urllib.parse.unquote(path, errors='surrogatepass')
-		except UnicodeDecodeError:
-			path = urllib.parse.unquote(path)
-		path = posixpath.normpath(path)
-		words = path.split('/')
-		words = filter(None, words)
-		path = self.directory
-
-		for word in words:
-			if os.path.dirname(word) or word in (os.curdir, os.pardir):
-				# Ignore components that are not a simple file/directory name
-				continue
-			path = os.path.join(path, word)
-		if trailing_slash:
-			path += '/'
-
-		return os.path.normpath(path)  # fix OS based path issue
-
-	def copyfile(self, source, outputfile):
-		"""Copy all data between two file objects.
-
-		The SOURCE argument is a file object open for reading
-		(or anything with a read() method) and the DESTINATION
-		argument is a file object open for writing (or
-		anything with a write() method).
-
-		The only reason for overriding this would be to change
-		the block size or perhaps to replace newlines by CRLF
-		-- note however that this the default server uses this
-		to copy binary data as well.
-
-		"""
-		try:
-			# check if file readable
-			source.read(1)
-			source.seek(0)
-		except OSError as e:
-			traceback.print_exc()
-			raise e
-
-		if not self.range:
-			shutil.copyfileobj(source, outputfile)
-
-		else:
-			# SimpleHTTPRequestHandler uses shutil.copyfileobj, which doesn't let
-			# you stop the copying before the end of the file.
-			start, stop = self.range  # set in send_head()
-			copy_byte_range(source, outputfile, start, stop)
-
-	def guess_type(self, path):
-		"""Guess the type of a file.
-
-		Argument is a PATH (a filename).
-
-		Return value is a string of the form type/subtype,
-		usable for a MIME Content-type header.
-
-		The default implementation looks the file's extension
-		up in the table self.extensions_map, using application/octet-stream
-		as a default; however it would be permissible (if
-		slow) to look inside the data to make a better guess.
-
-		"""
-
-		base, ext = posixpath.splitext(path)
-		if ext in self.extensions_map:
-			return self.extensions_map[ext]
-		ext = ext.lower()
-		if ext in self.extensions_map:
-			return self.extensions_map[ext]
-		guess, _ = mimetypes.guess_type(path)
-		if guess:
-			return guess
-
-		return self.extensions_map['']  # return 'application/octet-stream'
-
-
-class PostError(Exception):
-	pass
-
-
-class ContentDisposition:
-	def __init__(self, content_disposition):
-		self.content_disposition = content_disposition
-		self.items = {}
-		self.parse()
-
-	def parse(self):
-		# Content-Disposition: form-data; name="post-type"
-		# Content-Disposition: form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
-		# Content-Disposition: form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
-
-		line = re.subn(r"Content-Disposition:", "",
-					   self.content_disposition, flags=re.IGNORECASE, count=1)[0]
-
-		# form-data; name="post-type"
-		# form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
-		# form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
-		parts = (i.strip() for i in line.split(";") if i.strip())
-
-		# form-data
-		# name="post-type"
-		# name="file"
-		# filename="C:\Users\user\Desktop\test.txt"
-		# filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
-
-		for part in parts:
-			pair = [i.strip() for i in part.split("=", 1)]
-
-			key = pair[0]
-			value = pair[1] if len(pair) > 1 else ""
-
-			if key.lower() == "filename*" and value.lower().startswith("utf-8''"):
-				value = urllib.parse.unquote(
-					value[7:], encoding="utf-8", errors='surrogatepass')
-
-				key = "filename"
-
-			self.items[key.lower()] = value.strip('"')
-
-	def get(self, key, default=None):
-		return self.items.get(key.lower(), default)
-
-	def __getitem__(self, key):
-		return self.items[key.lower()]
-
-	def __contains__(self, key):
-		return key.lower() in self.items
-
-
-class DealPostData:
-	"""do_login
-
-#get starting boundary
-0: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
-1: b'Content-Disposition: form-data; name="post-type"\r\n'
-2: b'\r\n'
-3: b'login\r\n'
-4: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
-5: b'Content-Disposition: form-data; name="username"\r\n'
-6: b'\r\n'
-7: b'xxx\r\n'
-8: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
-9: b'Content-Disposition: form-data; name="password"\r\n'
-10: b'\r\n'
-11: b'ccc\r\n'
-12: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa--\r\n'
-"""
-
-	boundary = b''
-	num = 0
-	remainbytes = 0
-
-	def __init__(self, req: SimpleHTTPRequestHandler) -> None:
-		"""After init, must call start() to get boundary and content_length"""
-		self.req = req
-		self.content_length = 0
-		self.content_type = ""
-
-		self.form = FormData(req, self, fake=True)
-
-
-	refresh = "<br><br><div class='pagination center' onclick='window.location.reload()'>Refresh &#128259;</div>"
-
-	def is_multipart(self):
-		return self.content_type.startswith("multipart/form-data")
-
-	def is_urlencoded(self):
-		return self.content_type.startswith("application/x-www-form-urlencoded")
-
-	def is_form_data(self):
-		return self.is_urlencoded() or self.is_multipart()
-
-	def is_json(self):
-		return self.content_type == "application/json"
-
-	def check_size_limit(self, max_size=-1):
-		"""
-		* check if content size is within limit
-		* return True if within limit
-		"""
-		if not max_size < 0 or self.content_length <= max_size:
-			raise PostError(
-				f"Content size limit exceeded: {self.content_length} > {max_size}")
-
-	def get(self, show=F, strip=F, Timeout=10, chunk_size=0):
-		"""
-		show: print line
-		strip: strip \r\n at end
-		Timeout: if having network issue on any side, will keep trying to get content until Timeout (in seconds)
-		"""
-		req = self.req
-
-		if self.remainbytes <= 0:
-			return b""
-
-		if chunk_size <= 0:
-			chunk_size = self.remainbytes
-
-		for _ in range(Timeout*2):
-			if self.is_multipart():
-				line = req.rfile.readline()
-			else:
-				line = req.rfile.read(chunk_size)
-			if line:
-				break
-			time.sleep(.5)
-		else:
-			raise ConnectionAbortedError
-
-		if show:
-			print(f"{self.num}: {line}")
-		self.remainbytes -= len(line)
-		self.num += 1
-
-		if strip and self.is_multipart() and line.endswith(b"\r\n"):
-			line = line.rpartition(b"\r\n")[0]
-
-		return line
-
-	def get_content(self, max_size=-1, chunk_size=0):
-		"""
-		* get content if not multipart
-		* return content
-		"""
-
-		self.check_size_limit(max_size=max_size)
-
-		n = self.remainbytes
-		line = b""
-
-		while n > 0:
-			chunk = n % 1024
-			n -= chunk
-
-			_line = self.get(chunk_size=chunk)
-			if not _line:
-				break
-			line += _line
-
-		return line
-
-	def get_json(self, max_size=-1):
-		"""
-		* get json data
-		* return parsed json data
-		"""
-
-		if not self.content_type == "application/json":
-			raise PostError("Content-Type is not application/json")
-
-		line = self.get_content(max_size=max_size)
-
-		return json.loads(line)
-
-	def skip(self,):
-		self.get()
-
-	def start(self):
-		'''reads upto line 0'''
-		req = self.req
-		self.content_type = req.headers['content-type']
-
-		if not self.content_type:
-			raise PostError("POST request without Content-Type")
-		if self.is_multipart():
-			self.boundary = self.content_type.split("=")[1].encode()
-
-		self.remainbytes = int(req.headers['content-length'])
-		self.content_length = self.remainbytes
-
-		# print(f"Content-Type: {self.content_type}")
-		# print(f"Content-Length: {self.content_length}")
-		# print(f"Request-header: {req.headers}")
-		# print(self.is_form_data())
-
-		if self.is_form_data():
-			self.form = FormData(req, self)
-
-
-class FormData:
-	"""
-	Handler for
-	`multipart/form-data` and
-	`application/x-www-form-urlencoded`
-	"""
-
-	def __init__(self, req: SimpleHTTPRequestHandler, dpd: DealPostData, fake=False) -> None:
-		"""
-		must be initialized from DealPostData
-		"""
-		self.req = req
-		self.dpd = dpd
-		self.fake = fake
-
-		self.content_length = dpd.content_length
-		self.content_type = dpd.content_type
-
-		self.is_multipart = self.dpd.is_multipart()
-		if self.fake:
-			return
-		self.boundary = dpd.boundary
-		if self.is_multipart:
-			# pass first boundary line (because after every field, there is a boundary line)
-			self.pass_bound()
-
-
-	def pass_bound(self):
-		"""
-		* pass boundary line in multipart
-		* raise error if boundary not found
-		"""
-		if self.fake:
-			raise PostError("Fake FormData")
-
-		if not self.is_multipart:
-			raise PostError("Not multipart")
-
-		line = self.dpd.get()
-		if not self.boundary in line:
-			self.req.log_error(f"Content boundary missing on line {self.dpd.num}\n", [
-							   line, self.boundary])
-
-	def get_a_dline(self, line: Union[bytes, str, None] = None):
-		"""
-		* get a line if not provided
-		* decoded if its in bytes
-		* return decoded line
-		"""
-		if self.fake:
-			raise PostError("Fake FormData")
-		# only these 2 needs fake check
-
-		if not line:
-			line = self.dpd.get()
-
-		if isinstance(line, bytes):
-			line = line.decode()
-
-		return line
-
-	def get_file_name(self, line: Union[bytes, str, None] = None):
-		"""
-		* get file name from Content-Disposition
-		* return file name
-		"""
-		line = self.get_a_dline(line)
-
-		cd = ContentDisposition(line)
-		fn = cd.get('filename')
-
-		if not fn:
-			raise PostError("Can't find out file name...")
-
-		return fn
-
-	def get_field_name(self, line=None):
-		"""
-		* get field name from Content-Disposition
-		* return field name
-		"""
-		line = self.get_a_dline(line)
-
-		# get name from Content-Disposition
-		return ContentDisposition(line).get('name')
-
-	def match_field_name(self, field_name: Union[None, str] = None):
-		"""
-		field_name: Expecting name of the field (str)
-		* if None, skip checking field name
-		* if `empty string`, field name must be empty too
-		"""
-		line = self.dpd.get()
-
-		got_field_name = self.get_field_name(line)
-
-		if field_name is not None and got_field_name != field_name:
-			raise PostError(
-				f"Invalid request: Expected {field_name} but got {got_field_name}")
-
-		return got_field_name
-
-	def get_multi_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None, decode=F):
-		'''read a form field
-		ends at boundary
-		verify_name: name of the field (str|bytes|None)
-		verify_msg: message to verify (str|bytes)
-		decode: decode the message
-		* if None, skip checking field name
-		* if `empty string`, field name must be empty too
-
-		returns: field `(name, value)` (str|bytes)
-		'''
-		decoded = False
-
-		if isinstance(verify_name, bytes):
-			verify_name = verify_name.decode()
-
-		# LINE 0 (boundary)
-		field_name = self.match_field_name(verify_name)  # LINE 1 (field name)
-		# if not verified, raise PostError
-
-		if not field_name:
-			return None, None
-
-		self.dpd.skip()  # LINE 2 (blank line)
-
-		line = b''
-		while 1:
-			_line = self.dpd.get()  # from LINE 3 till boundary (form field value)
-			if (not _line) or (self.boundary in _line):  # boundary
-				break
-			line += _line
-
-		if not line:
-			return None, None
-
-		line = line.rpartition(b"\r\n")[0]  # remove \r\n at end
-		if decode:
-			line = line.decode()
-			decoded = True
-		if verify_msg is not None:
-			if not decoded:
-				if isinstance(verify_msg, str):
-					verify_msg = verify_msg.encode()
-
-			if line != verify_msg:
-				raise PostError(
-					f"Invalid post request.\n Expected: {[verify_msg]}\n Got: {[line]}")
-
-		# self.pass_bound() # LINE 5 (boundary)
-
-		return field_name, line
-
-	def get_urlencoded_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None):
-		"""
-		* get a field from form data
-		* return decoded name, value
-
-		"""
-		line = b""
-		data = self.dpd.get(chunk_size=1)
-		while data or data == b"&":
-			line += data
-
-			data = self.dpd.get(chunk_size=1)
-
-		name, value = line.split(b"=", 1)
-		# URL decode
-		name, value = urllib.parse.unquote(name), urllib.parse.unquote(value)
-
-		if verify_name is not None:
-			if isinstance(verify_name, bytes):
-				verify_name = verify_name.decode()
-
-			if name != verify_name:
-				raise PostError(
-					f"Invalid post request.\n Expected: {verify_name}\n Got: {name}")
-
-		if verify_msg is not None:
-			if isinstance(verify_msg, bytes):
-				verify_msg = verify_msg.decode()
-
-			if value != verify_msg:
-				raise PostError(
-					f"Invalid post request.\n Expected: {verify_msg}\n Got: {value}")
-		return name, value
-
-	def get_urlencoded_iter(self, max_size=-1):
-		"""
-		Generator that yields the parts of the form data as dict.
-		"""
-
-		self.dpd.check_size_limit(max_size)
-
-
-		data = self.dpd.get().decode()
-		for part in data.split("&"):
-			name, value = part.split("=")
-			name, value = urllib.parse.unquote(
-				name), urllib.parse.unquote(value)
-
-			yield name, value
-
-	def get_multipart_iter(self, max_size=-1):
-		"""
-		Generator that yields the parts of the form data as dict.
-		"""
-
-		self.dpd.check_size_limit(max_size)
-
-		while True:
-			field_name, value = self.get_multi_field(decode=True)
-			if not field_name:
-				break
-			yield field_name, value
-
-	def get_parts(self, max_size=-1):
-		"""
-		Generator that yields the parts of the form data.
-		"""
-		if self.is_multipart:
-			g = self.get_multipart_iter
-		else:
-			g = self.get_urlencoded_iter
-
-		for part in g(max_size):
-			yield part
-
-
-def _get_best_family(*address):
-	infos = socket.getaddrinfo(
-		*address,
-		type=socket.SOCK_STREAM,
-		flags=socket.AI_PASSIVE
-	)
-	family, type, proto, canonname, sockaddr = next(iter(infos))
-	return family, sockaddr
-
-
-def get_ip(bind=None):
-	IP = bind  # or "127.0.0.1"
-	s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-	s.settimeout(0)
-	try:
-		# doesn't even have to be reachable
-		s.connect(('10.255.255.255', 1))
-		IP = s.getsockname()[0]
-	except:
-		try:
-			if config.OS == "Android":
-				IP = s.connect(("192.168.43.1",  1))
-				IP = s.getsockname()[0]
-				# Assigning this variable because Android does't return actual IP when hosting a hotspot
-		except (socket.herror, OSError):
-			pass
-	finally:
-		s.close()
-	return IP
-
-
-def test(HandlerClass=BaseHTTPRequestHandler,
-		 ServerClass=ThreadingHTTPServer,
-		 protocol="HTTP/1.0", port=8000, bind=None):
-	"""Test the HTTP request handler class.
-
-	This runs an HTTP server on port 8000 (or the port argument).
-
-	"""
-
-	global httpd
-	if sys.version_info >= (3, 8):  # BACKWARD COMPATIBILITY
-		ServerClass.address_family, addr = _get_best_family(bind, port)
-	else:
-		addr = (bind if bind != None else '', port)
-
-	device_ip = bind or "127.0.0.1"
-	# bind can be None (=> 127.0.0.1) or a string (=> 127.0.0.DDD)
-
-	HandlerClass.protocol_version = protocol
-	httpd = ServerClass(addr, HandlerClass)
-	host, port = httpd.socket.getsockname()[:2]
-	url_host = f'[{host}]' if ':' in host else host
-	hostname = socket.gethostname()
-	local_ip = config.IP if config.IP else get_ip(device_ip)
-	config.IP = local_ip
-
-	on_network = local_ip != (device_ip)
-
-	logger.info(tools.text_box(
-		# TODO: need to check since the output is "Serving HTTP on :: port 6969"
-		f"Serving HTTP on {host} port {port} \n",
-		# TODO: need to check since the output is "(http://[::]:6969/) ..."
-		f"(http://{url_host}:{port}/) ...\n",
-		f"Server is probably running on\n",
-		(f"[over NETWORK] {config.address()}\n" if on_network else ""),
-		f"[on DEVICE] http://localhost:{config.port} & http://127.0.0.1:{config.port}", style="star", sep=""
-	)
-	)
-	try:
-		httpd.serve_forever(poll_interval=0.1)
-	except KeyboardInterrupt:
-		logger.info("\nKeyboard interrupt received, exiting.")
-
-	except OSError:
-		logger.info("\nOSError received, exiting.")
-	finally:
-		if not config.reload:
-			sys.exit(0)
-
-
-class DualStackServer(ThreadingHTTPServer):  # UNSUPPORTED IN PYTHON 3.7
-
-	def handle_error(self, request, client_address):
-		pass
-
-	def server_bind(self):
-		# suppress exception when protocol is IPv4
-		with contextlib.suppress(Exception):
-			self.socket.setsockopt(
-				socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
-		return super().server_bind()
-
-	def finish_request(self, request, client_address):
-		self.RequestHandlerClass(request, client_address, self,
-								 directory=config.ftp_dir)
-
-
-def run(port=0, directory="", bind="", arg_parse=True, handler=SimpleHTTPRequestHandler):
-
-	if arg_parse:
-		args = config.parse_default_args(
-			port=port, directory=directory, bind=bind)
-
-		port = args.port
-		directory = args.directory
-		bind = args.bind
-
-	logger.info(tools.text_box("Running pyroboxCore: ",
-				config.MAIN_FILE, "Version: ", __version__))
-
-	if directory == config.ftp_dir and not os.path.isdir(config.ftp_dir):
-		logger.warning(
-			config.ftp_dir, "not found!\nReseting directory to current directory")
-		directory = "."
-
-	handler_class = partial(handler,
-							directory=directory)
-
-	config.port = port
-	if port > 65535 or port < 0:
-		raise ValueError("Port must be between 0 and 65535")
-
-	config.ftp_dir = directory
-
-	if not config.reload:
-		if sys.version_info > (3, 8):
-			test(
-				HandlerClass=handler_class,
-				ServerClass=DualStackServer,
-				port=port,
-				bind=bind,
-			)
-		else:  # BACKWARD COMPATIBILITY
-			test(
-				HandlerClass=handler_class,
-				ServerClass=ThreadingHTTPServer,
-				port=port,
-				bind=bind,
-			)
-
-	if config.reload == True:
-		reload_server()
-
-
-if __name__ == '__main__':
-	run()
+import traceback
+import json
+import string
+import random
+import base64
+import re
+from http import HTTPStatus
+from http.cookies import SimpleCookie
+from functools import partial
+import contextlib
+import urllib.request
+import urllib.parse
+import time
+import sys
+import socketserver
+import socket  # For gethostbyaddr()
+import shutil
+import posixpath
+import mimetypes
+import io
+import http.client
+import html
+import email.utils
+import datetime
+import argparse
+from string import Template
+from typing import Union
+from queue import Queue
+import logging
+import atexit
+import os
+
+__version__ = "0.9.5"
+enc = "utf-8"
+DEV_MODE = False
+
+
+__all__ = [
+	"HTTPServer", "ThreadingHTTPServer", "BaseHTTPRequestHandler",
+	"SimpleHTTPRequestHandler",
+]
+
+
+logging.basicConfig(level=logging.INFO, format='%(levelname)s: \n%(message)s')
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+# set INFO to see all the requests
+# set WARNING to see only the requests that made change to the server
+# set ERROR to see only the requests that made the errors
+
+
+endl = "\n"
+T = t = true = True  # too lazy to type
+F = f = false = False  # too lazy to type
+
+
+class Config:
+	def __init__(self):
+		# DEFAULT DIRECTORY TO LAUNCH SERVER
+		self.ftp_dir = "."  # DEFAULT DIRECTORY TO LAUNCH SERVER
+
+		self.IP = None  # will be assigned by checking
+		self.protocol = "http"  # DEFAULT PROTOCOL TO LAUNCH SERVER
+
+		# DEFAULT PORT TO LAUNCH SERVER
+		self.port = 6969  # DEFAULT PORT TO LAUNCH SERVER
+
+		# UPLOAD PASSWORD SO THAT ANYONE RANDOM CAN'T UPLOAD
+		# CAN BE CHANGED BY USING --password NEW_PASSWORD
+		self.PASSWORD = "SECret"
+
+		# LOGGING
+		self.log_location = "./"  # fallback log_location = "./"
+		# if you want to see some important LOG in browser, may contain your important information
+		self.allow_web_log = True
+		self.write_log = False  # if you want to write log to file
+		self.log_extra = True
+
+		# ZIP FEATURES
+		self.default_zip = "zipfile"  # or "zipfile" to use python built in zip module
+
+		# CHECK FOR MISSING REQUIREMENTS
+		self.run_req_check = True
+
+		# FILE INFO
+		self.MAIN_FILE = os.path.realpath(__file__)
+		self.MAIN_FILE_dir = os.path.dirname(self.MAIN_FILE)
+
+		# OS DETECTION
+		self.OS = self.get_os()
+
+		# RUNNING SERVER STATS
+		self.ftp_dir = self.get_default_dir()
+		self.dev_mode = DEV_MODE
+		self.ASSETS = False  # if you want to use assets folder, set this to True
+		self.ASSETS_dir = os.path.join(self.MAIN_FILE_dir, "/../assets/")
+		self.reload = False
+
+		self.disabled_func = {
+			"reload": False,
+		}
+
+		# TEMP FILE MAPPING
+		self.temp_file = set()
+
+		# CLEAN TEMP FILES ON EXIT
+		atexit.register(self.clear_temp)
+
+		# ASSET MAPPING
+		self.file_list = {}
+
+		# COMMANDLINE ARGUMENTS PARSER
+		self.parser = argparse.ArgumentParser(add_help=False)
+
+		# Default error message template
+		self.DEFAULT_ERROR_MESSAGE = Template("""
+		<!DOCTYPE HTML>
+		<html lang="en">
+		<html>
+			<head>
+				<meta charset="utf-8">
+				<title>Error response</title>
+			</head>
+			<body>
+				<h1>Error response</h1>
+				<p>Error code: ${code}</p>
+				<p>Message: ${message}</p>
+				<p>Error code explanation: ${code} - ${explain}</p>
+				<h3>PyroBox Version: ${version}</h3>
+			</body>
+		</html>
+		""")
+
+		self.DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
+
+	def clear_temp(self):
+		for i in self.temp_file:
+			try:
+				os.remove(i)
+			except OSError:
+				pass
+
+	def get_os(self):
+		from platform import system as platform_system
+
+		out = platform_system()
+		if out == "Linux" and hasattr(sys, 'getandroidapilevel'):
+			# self.IP = "192.168.43.1"
+			return 'Android'
+
+		return out
+
+	def get_default_dir(self):
+		if self.get_os()== 'Android':
+			return '/storage/emulated/0/'
+		return './'
+
+	def address(self):
+		return f"{self.protocol}://{self.IP}:{self.port}"
+
+	def parse_default_args(self, port=0, directory="", bind=None):
+		if not port:
+			port = self.port
+		if not directory:
+			directory = self.ftp_dir
+		if not bind:
+			bind = None
+
+		parser = self.parser
+
+		parser.add_argument('--bind', '-b',
+							metavar='ADDRESS', default=bind,
+							help='[xxx.xxx.xxx.xxx] Specify alternate bind address '
+								'[default: all interfaces]')
+		parser.add_argument('--directory', '-d', default=directory,
+							help='[Value] Specify alternative directory '
+								'[default: current directory]')
+		parser.add_argument('port', action='store',
+							default=port, type=int,
+							nargs='?',
+							help=f'[Value] Specify alternate port [default: {port}]')
+		parser.add_argument('--version', '-v', action='version',
+							version=__version__)
+
+		parser.add_argument('-h', '--help', action='help',
+								default='==SUPPRESS==',
+								help=('[Option] show this help message and exit'))
+
+
+		parser.add_argument('--no-extra-log',
+							action='store_true',
+							default=False,
+							help="[Flag] Disable file path and [= + - #] based logs (default: %(default)s)")
+
+
+		args = parser.parse_known_args()[0]
+
+		self.log_extra = not args.no_extra_log
+
+		return args
+
+
+class Tools:
+	def __init__(self):
+		self.styles = {
+			"equal": "=",
+			"star": "*",
+			"hash": "#",
+			"dash": "-",
+			"udash": "_"
+		}
+
+	@staticmethod
+	def term_width():
+		""" Return CLI screen size (if not found, returns default value)
+		"""
+		return shutil.get_terminal_size()[0]
+
+	def text_box(self, *text, style="equal", sep=" "):
+		"""
+		Returns a string of text with a border around it.
+		"""
+		text = sep.join(map(str, text))
+		term_col = shutil.get_terminal_size()[0]
+
+		s = self.styles[style] if style in self.styles else style
+		tt = ""
+		for i in text.split('\n'):
+			tt += i.center(term_col) + '\n'
+		return (f"\n\n{s*term_col}\n{tt}{s*term_col}\n\n")
+
+	@staticmethod
+	def random_string(length=10):
+		"""Generates a random string
+		length : length of string
+		"""
+		letters = string.ascii_lowercase
+		return ''.join(random.choice(letters) for i in range(length))
+
+
+tools = Tools()
+config = Config()
+
+
+
+class Callable_dict(dict):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.__dict__ = self
+
+	def __call__(self, *key):
+		return all([i in self for i in key])
+
+
+
+
+def reload_server():
+	"""reload the server process from file"""
+	file = config.MAIN_FILE
+	logger.info("Reloading...\n" +
+				" ".join(
+					["RE-RUNNING: ", sys.executable,
+						sys.executable, file, *sys.argv[1:]]
+				))
+	try:
+		os.execl(sys.executable, sys.executable, file, *sys.argv[1:])
+	except OSError:
+		traceback.print_exc()
+	sys.exit(0)
+
+
+def null(*args, **kwargs):
+	pass
+
+
+class Zfunc(object):
+	"""Thread safe sequncial printing/queue task handler class"""
+
+	__all__ = ["new", "update"]
+
+	def __init__(self, caller, store_return=False):
+		super().__init__()
+
+		self.queue = Queue()
+		# stores [args, kwargs], ...
+		self.store_return = store_return
+		self.returner = Queue()
+		# queue to store return value if store_return enabled
+
+		self.BUSY = False
+
+		self.caller = caller
+
+	def next(self):
+		""" check if any item in queje and call, if already running or queue empty, returns """
+		if self.queue.empty() or self.BUSY:
+			return None
+
+		self.BUSY = True
+		args, kwargs = self.queue.get()
+
+		x = self.caller(*args, **kwargs)
+		if self.store_return:
+			self.returner.put(x)
+
+		self.BUSY = False
+
+		if not self.queue.empty():
+			# will make the loop continue running
+			return True
+
+	def update(self, *args, **kwargs):
+		""" Uses xprint and parse string"""
+
+		self.queue.put((args, kwargs))
+		while self.next() is True:
+			# use while instead of recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion to avoid recursion.... error
+			pass
+
+	def new(self, caller, store_return=False):
+		self.__init__(caller=caller, store_return=store_return)
+
+	def destroy(self):
+		"""Clear the queue
+		however if running, caller function will still keep running till end"""
+		self.__init__(caller=null, store_return=False)
+
+
+"""HTTP server classes.
+
+Note: BaseHTTPRequestHandler doesn't implement any HTTP request; see
+SimpleHTTPRequestHandler for simple implementations of GET, HEAD and POST,
+and CGIHTTPRequestHandler for CGI scripts.
+
+It does, however, optionally implement HTTP/1.1 persistent connections,
+as of version 0.3.
+
+XXX To do:
+
+- log requests even later (to capture byte count)
+- log user-agent header and other interesting goodies
+- send error log to separate file
+"""
+
+
+##############################################
+#         PAUSE AND RESUME FEATURE           #
+##############################################
+
+def copy_byte_range(infile, outfile, start=None, stop=None, bufsize=16*1024):
+	'''
+	TO SUPPORT PAUSE AND RESUME FEATURE
+	Like shutil.copyfileobj, but only copy a range of the streams.
+	Both start and stop are inclusive.
+	'''
+	if start is not None:
+		infile.seek(start)
+	while 1:
+		to_read = min(bufsize, stop + 1 - infile.tell() if stop else bufsize)
+		buf = infile.read(to_read)
+		if not buf:
+			break
+		outfile.write(buf)
+
+
+BYTE_RANGE_RE = re.compile(r'bytes=(\d+)-(\d+)?$')
+
+
+def parse_byte_range(byte_range):
+	'''Returns the two numbers in 'bytes=123-456' or throws ValueError.
+	The last number or both numbers may be None.
+	'''
+	if byte_range.strip() == '':
+		return None, None
+
+	m = BYTE_RANGE_RE.match(byte_range)
+	if not m:
+		raise ValueError(f'Invalid byte range {byte_range}')
+
+	# first, last = [x and int(x) for x in m.groups()] #
+
+	first, last = map((lambda x: int(x) if x else None), m.groups())
+
+	if last and last < first:
+		raise ValueError(f'Invalid byte range { byte_range}')
+	return first, last
+
+# ---------------------------x--------------------------------
+
+
+def URL_MANAGER(url: str):
+	"""
+	returns a tuple of (`path`, `query_dict`, `fragment`)\n
+
+	`url` = `'/store?page=10&limit=15&price=ASC#dskjfhs'`\n
+	`path` = `'/store'` or `/`\n
+	`query_dict` = `{'page': ['10'], 'limit': ['15'], 'price': ['ASC']}`\n
+	`fragment` = `dskjfhs`\n
+	"""
+
+	# url = '/store?page=10&limit=15&price#dskjfhs'
+	parse_result = urllib.parse.urlparse(url)
+
+	path = parse_result.path
+	if path == '':
+		path = '/'
+
+	dict_result = Callable_dict(urllib.parse.parse_qs(
+		parse_result.query, keep_blank_values=True))
+
+	return (path, dict_result, parse_result.fragment)
+
+if __name__ == "__main__":
+	print(URL_MANAGER('https://www.google.com'))
+	print(URL_MANAGER('https://www.google.com/store?page=10&limit=15&price=ASC#dskjfhs'))
+
+
+class HTTPServer(socketserver.TCPServer):
+
+	allow_reuse_address = True  # Seems to make sense in testing environment
+
+	def server_bind(self):
+		"""Override server_bind to store the server name."""
+		socketserver.TCPServer.server_bind(self)
+		host, port = self.server_address[:2]
+		self.server_name = socket.getfqdn(host)
+		self.server_port = port
+
+
+class ThreadingHTTPServer(socketserver.ThreadingMixIn, HTTPServer):
+	daemon_threads = True
+
+
+class BaseHTTPRequestHandler(socketserver.StreamRequestHandler):
+
+	"""HTTP request handler base class.
+
+	The various request details are stored in instance variables:
+
+	- client_address is the client IP address in the form (host,
+	port);
+
+	- command, path and version are the broken-down request line;
+
+	- headers is an instance of email.message.Message (or a derived
+	class) containing the header information;
+
+	- rfile is a file object open for reading positioned at the
+	start of the optional input data part;
+
+	- wfile is a file object open for writing.
+
+	IT IS IMPORTANT TO ADHERE TO THE PROTOCOL FOR WRITING!
+
+	The first thing to be written must be the response line.  Then
+	follow 0 or more header lines, then a blank line, and then the
+	actual data (if any).  The meaning of the header lines depends on
+	the command executed by the server; in most cases, when data is
+	returned, there should be at least one header line of the form
+
+	Content-type: <type>/<subtype>
+
+	where <type> and <subtype> should be registered MIME types,
+	e.g. "text/html" or "text/plain".
+
+	"""
+
+	# The Python system version, truncated to its first component.
+	sys_version = "Python/" + sys.version.split()[0]
+
+	# The server software version.  You may want to override this.
+	# The format is multiple whitespace-separated strings,
+	# where each string is of the form name[/version].
+	server_version = "BaseHTTP/" + __version__
+
+
+	# The default request version.  This only affects responses up until
+	# the point where the request line is parsed, so it mainly decides what
+	# the client gets back when sending a malformed request line.
+	# Most web servers default to HTTP 0.9, i.e. don't send a status line.
+	default_request_version = "HTTP/0.9"
+
+	def parse_request(self):
+		"""Parse a request (internal).
+
+		The request should be stored in self.raw_requestline; the results
+		are in self.command, self.path, self.request_version and
+		self.headers.
+
+		Return True for success, False for failure; on failure, any relevant
+		error response has already been sent back.
+
+		"""
+		self.command = ''  # set in case of error on the first line
+		self.request_version = version = self.default_request_version
+		self.close_connection = True
+		self.header_flushed = False # true when headers are flushed by self.flush_headers()
+		self.response_code_sent = False # true when response code (>=200) is sent by self.send_response()
+
+
+		requestline = str(self.raw_requestline, 'iso-8859-1')
+		requestline = requestline.rstrip('\r\n')
+		self.requestline = requestline
+		words = requestline.split()
+		if len(words) == 0:
+			return False
+
+		if len(words) >= 3:  # Enough to determine protocol version
+			version = words[-1]
+			try:
+				if not version.startswith('HTTP/'):
+					raise ValueError
+				base_version_number = version.split('/', 1)[1]
+				version_number = base_version_number.split(".")
+				# RFC 2145 section 3.1 says there can be only one "." and
+				#   - major and minor numbers MUST be treated as
+				#     separate integers;
+				#   - HTTP/2.4 is a lower version than HTTP/2.13, which in
+				#     turn is lower than HTTP/12.3;
+				#   - Leading zeros MUST be ignored by recipients.
+				if len(version_number) != 2:
+					raise ValueError
+				version_number = int(version_number[0]), int(version_number[1])
+			except (ValueError, IndexError):
+				self.send_error(
+					HTTPStatus.BAD_REQUEST,
+					"Bad request version (%r)" % version)
+				return False
+			if version_number >= (1, 1) and self.protocol_version >= "HTTP/1.1":
+				self.close_connection = False
+			if version_number >= (2, 0):
+				self.send_error(
+					HTTPStatus.HTTP_VERSION_NOT_SUPPORTED,
+					"Invalid HTTP version (%s)" % base_version_number)
+				return False
+			self.request_version = version
+
+		if not 2 <= len(words) <= 3:
+			self.send_error(
+				HTTPStatus.BAD_REQUEST,
+				"Bad request syntax (%r)" % requestline)
+			return False
+		command, path = words[:2]
+		if len(words) == 2:
+			self.close_connection = True
+			if command != 'GET':
+				self.send_error(
+					HTTPStatus.BAD_REQUEST,
+					"Bad HTTP/0.9 request type (%r)" % command)
+				return False
+		self.command, self.path = command, path
+
+
+		# gh-87389: The purpose of replacing '//' with '/' is to protect
+		# against open redirect attacks possibly triggered if the path starts
+		# with '//' because http clients treat //path as an absolute URI
+		# without scheme (similar to http://path) rather than a path.
+		if self.path.startswith('//'):
+			self.path = '/' + self.path.lstrip('/')  # Reduce to a single /
+
+		# Examine the headers and look for a Connection directive.
+		try:
+			self.headers = http.client.parse_headers(self.rfile,
+													 _class=self.MessageClass)
+		except http.client.LineTooLong as err:
+			self.send_error(
+				HTTPStatus.REQUEST_HEADER_FIELDS_TOO_LARGE,
+				"Line too long",
+				str(err))
+			return False
+		except http.client.HTTPException as err:
+			self.send_error(
+				HTTPStatus.REQUEST_HEADER_FIELDS_TOO_LARGE,
+				"Too many headers",
+				str(err)
+			)
+			return False
+
+		conntype = self.headers.get('Connection', "")
+		if conntype.lower() == 'close':
+			self.close_connection = True
+		elif (conntype.lower() == 'keep-alive' and
+			  self.protocol_version >= "HTTP/1.1"):
+			self.close_connection = False
+
+		# Load cookies from request
+		# Uses standard SimpleCookie
+		# doc: https://docs.python.org/3/library/http.cookies.html
+		self.cookie = SimpleCookie()
+		self.cookie.load(self.headers.get('Cookie', ""))
+		# print(tools.text_box("Cookie: ", self.cookie))
+
+		# Examine the headers and look for an Expect directive
+		expect = self.headers.get('Expect', "")
+		if (expect.lower() == "100-continue" and
+			self.protocol_version >= "HTTP/1.1" and
+				self.request_version >= "HTTP/1.1"):
+			if not self.handle_expect_100():
+				return False
+		return True
+
+	def handle_expect_100(self):
+		"""Decide what to do with an "Expect: 100-continue" header.
+
+		If the client is expecting a 100 Continue response, we must
+		respond with either a 100 Continue or a final response before
+		waiting for the request body. The default is to always respond
+		with a 100 Continue. You can behave differently (for example,
+		reject unauthorized requests) by overriding this method.
+
+		This method should either return True (possibly after sending
+		a 100 Continue response) or send an error response and return
+		False.
+
+		"""
+		self.send_response_only(HTTPStatus.CONTINUE)
+		self.end_headers()
+		return True
+
+	def handle_one_request(self):
+		"""Handle a single HTTP request.
+
+		You normally don't need to override this method; see the class
+		__doc__ string for information on how to handle specific HTTP
+		commands such as GET and POST.
+
+		"""
+		try:
+			self.raw_requestline = self.rfile.readline(65537)
+			if len(self.raw_requestline) > 65536:
+				self.requestline = ''
+				self.request_version = ''
+				self.command = ''
+				self.send_error(HTTPStatus.REQUEST_URI_TOO_LONG)
+				return
+			if not self.raw_requestline:
+				self.close_connection = True
+				return
+			if not self.parse_request():
+				# An error code has been sent, just exit
+				return
+			mname = 'do_' + self.command
+			if not hasattr(self, mname):
+				self.send_error(
+					HTTPStatus.NOT_IMPLEMENTED,
+					"Unsupported method (%r)" % self.command)
+				return
+			method = getattr(self, mname)
+
+			url_path, query, fragment = URL_MANAGER(self.path)
+			self.url_path = url_path
+			self.query = query
+			self.fragment = fragment
+
+			self.use_range = False
+
+			_hash = abs(hash((self.raw_requestline, tools.random_string(10))))
+			self.req_hash = base64.b64encode(
+					str(_hash).encode('ascii')
+				).decode()[:10]
+
+			_w = tools.term_width()
+			w = _w - len(str(self.req_hash)) - 2
+			w = w//2
+			if config.log_extra:
+				logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n' +
+						'\n'.join(
+								[f'{self.req_hash}|=>\t request\t: {self.command}',
+								 f'{self.req_hash}|=>\t url     \t: {url_path}',
+								 f'{self.req_hash}|=>\t query   \t: {query}',
+								 f'{self.req_hash}|=>\t fragment\t: {fragment}',
+								 f'{self.req_hash}|=>\t full url \t: {self.path}',
+								 ]) + '\n' +
+						'+'*w + f' {self.req_hash} ' + '+'*w
+						)
+
+			try:
+				method()
+			except Exception:
+				traceback.print_exc()
+
+			if config.log_extra:
+				logger.info('-'*w + f' {self.req_hash} ' + '-'*w + '\n' +
+						'#'*_w
+						)
+
+			# actually send the response if not already done.
+			self.wfile.flush()
+
+		except (TimeoutError, socket.timeout) as e:
+			# a read or a write timed out.  Discard this connection
+			self.log_error("Request timed out:", e)
+			self.close_connection = True
+			return
+
+	def handle(self):
+		"""Handle multiple requests if necessary."""
+		self.close_connection = True
+
+		self.handle_one_request()
+		while not self.close_connection:
+			self.handle_one_request()
+
+	def send_error(self, code, message=None, explain=None, error_message_format: Template = None, cookie:Union[SimpleCookie, str]=None):
+		"""Send and log an error reply.
+
+		Arguments are
+		* code:	an HTTP error code
+					3 digits
+		* message: a simple optional 1 line reason phrase.
+					*( HTAB / SP / VCHAR / %x80-FF )
+					defaults to short entry matching the response code
+		* explain: a detailed message defaults to the long entry
+					matching the response code.
+		* error_message_format: a `string.Template` for the error message
+					defaults to `config.DEFAULT_ERROR_MESSAGE`
+
+					auto-formatting values:
+						`${code}`: the HTTP error code
+						`${message}`: the HTTP error message
+						`${explain}`: the detailed error message
+						`${version}`: the server software version string
+
+		This sends an error response (so it must be called before any
+		output has been generated), logs the error, and finally sends
+		a piece of HTML explaining the error to the user.
+
+		"""
+
+		error_message_format = error_message_format if error_message_format else config.DEFAULT_ERROR_MESSAGE
+
+		error_content_type = config.DEFAULT_ERROR_CONTENT_TYPE
+
+		try:
+			shortmsg, longmsg = self.responses[code]
+		except KeyError:
+			shortmsg, longmsg = '???', '???'
+		if message is None:
+			message = shortmsg
+		if explain is None:
+			explain = longmsg
+		self.log_error("code", code, "message", message)
+		self.send_response(code, message)
+
+		self._send_cookie(cookie=cookie)
+
+		self.send_header('Connection', 'close')
+
+		# Message body is omitted for cases described in:
+		#  - RFC7230: 3.3. 1xx, 204(No Content), 304(Not Modified)
+		#  - RFC7231: 6.3.6. 205(Reset Content)
+		body = None
+		if (code >= 200 and
+				code not in (HTTPStatus.NO_CONTENT,
+							 HTTPStatus.RESET_CONTENT,
+							 HTTPStatus.NOT_MODIFIED)):
+			# HTML encode to prevent Cross Site Scripting attacks
+			# (see bug #1100201)
+			content = (error_message_format.safe_substitute(
+				code=code,
+				message=html.escape(message, quote=False),
+				explain=html.escape(explain, quote=False),
+				version=__version__
+			))
+			body = content.encode('UTF-8', 'replace')
+			self.send_header("Content-Type", error_content_type)
+			self.send_header('Content-Length', str(len(body)))
+		self.end_headers()
+
+		if self.command != 'HEAD' and body:
+			self.wfile.write(body)
+
+	def send_response(self, code, message=None):
+		"""Add the response header to the headers buffer and log the
+		response code.
+
+		Also send two standard headers with the server software
+		version and the current date.
+
+		"""
+		if self.response_code_sent:
+			return
+
+		if not code//100 ==1: # 1xx - Informational (allowes multiple responses)
+			self.response_code_sent = True
+
+		self.log_request(code)
+		self.send_response_only(code, message)
+		self.send_header('Server', self.version_string())
+		self.send_header('Date', self.date_time_string())
+
+	def send_response_only(self, code, message=None):
+		"""Send the response header only."""
+		if self.request_version != 'HTTP/0.9':
+			if message is None:
+				if code in self.responses:
+					message = self.responses[code][0]
+				else:
+					message = ''
+			if not hasattr(self, '_headers_buffer'):
+				self._headers_buffer = []
+			self._headers_buffer.append(("%s %d %s\r\n" %
+				(self.protocol_version, code, message)).encode(
+				'utf-8', 'strict'))
+
+	def send_header_string(self, lines:str):
+		"""Send a header multiline string to the headers buffer."""
+		for i in lines.split("\r\n"):
+			if not i:
+				continue
+			tag, _, msg = i.partition(":")
+			self.send_header(tag.strip(), msg.strip())
+
+
+	def _send_cookie(self, cookie:Union[SimpleCookie, str]=None):
+		"""Must send cookie after self.send_response(XXX)"""
+		if cookie is not None:
+			if isinstance(cookie, SimpleCookie):
+				cookie = cookie.output()
+
+			self.send_header_string(cookie)
+
+
+
+
+	def send_header(self, keyword, value):
+		"""Send a MIME header to the headers buffer."""
+		if self.request_version != 'HTTP/0.9':
+			if not hasattr(self, '_headers_buffer'):
+				self._headers_buffer = []
+			self._headers_buffer.append(
+				("%s: %s\r\n" % (keyword, value)).encode('utf-8', 'strict'))
+
+		if keyword.lower() == 'connection':
+			if value.lower() == 'close':
+				self.close_connection = True
+			elif value.lower() == 'keep-alive':
+				self.close_connection = False
+
+	def end_headers(self):
+		"""Send the blank line ending the MIME headers."""
+		if self.request_version != 'HTTP/0.9':
+			self._headers_buffer.append(b"\r\n")
+			self.flush_headers()
+
+	def flush_headers(self):
+		"""Flush the headers buffer."""
+		if self.header_flushed:
+			try:
+				raise RuntimeError("Headers already flushed")
+			except RuntimeError:
+				traceback.print_exc()
+			return
+		if hasattr(self, '_headers_buffer'):
+			self.wfile.write(b"".join(self._headers_buffer))
+			self._headers_buffer = []
+
+		self.header_flushed = True
+
+	def log_request(self, code='-', size='-'):
+		"""Log an accepted request.
+
+		This is called by send_response().
+
+		"""
+		if isinstance(code, HTTPStatus):
+			code = code.value
+		self.log_message(f'"{self.requestline}"', code, size)
+
+	def log_error(self, *args, **kwargs):
+		"""Log an error. [ERROR PRIORITY]
+
+		This is called when a request cannot be fulfilled.  By
+		default it passes the message on to log_message().
+
+		Arguments are the same as for log_message().
+
+		XXX This should go to the separate error log.
+
+		"""
+		self.log_message(*args, **kwargs, error=True)
+
+	def log_warning(self, *args, **kwargs):
+		"""Log a warning message [HIGH PRIORITY]"""
+		self.log_message(*args, **kwargs, warning=True)
+
+	def log_debug(self, *args, write=True, **kwargs):
+		"""Log a debug message [LOWEST PRIORITY]"""
+		self.log_message(*args, **kwargs, debug=True, write=write)
+
+	def log_info(self, *args, write=False, **kwargs):
+		"""Default log message [MEDIUM PRIORITY]"""
+		self.log_message(*args, **kwargs, write=write)
+
+	def _log_writer(self, message):
+		os.makedirs(config.log_location, exist_ok=True)
+		with open(config.log_location + 'log.txt', 'a+') as f:
+			f.write(
+				(f"#{self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"))
+
+	def log_message(self, *args, error=False, warning=False, debug=False, write=True, **kwargs):
+		"""Log an arbitrary message.
+
+		This is used by all other logging functions.  Override
+		it if you have specific logging wishes.
+
+		The client ip and current date/time are prefixed to
+		every message.
+
+		"""
+		if not args:
+			return
+
+		sep = kwargs.get('sep', ' ')
+		end = kwargs.get('end', '\n')
+
+		message = sep.join(map(str, args)) + end
+
+		message = f"# {self.req_hash} by [{self.address_string()}] at [{self.log_date_time_string()}]|=> {message}\n"
+
+		if error:
+			logger.error(message)
+		elif warning:
+			logger.warning(message)
+		elif debug:
+			logger.debug(message)
+		else:
+			logger.info(message)
+
+		if not config.write_log:
+			return
+
+		if not hasattr(self, "Zlog_writer"):
+			self.Zlog_writer = Zfunc(self._log_writer)
+
+		try:
+			self.Zlog_writer.update(message)
+		except Exception:
+			traceback.print_exc()
+
+	def version_string(self):
+		"""Return the server software version string."""
+		return self.server_version + ' ' + self.sys_version
+
+	def date_time_string(self, timestamp=None):
+		"""Return the current date and time formatted for a message header."""
+		if timestamp is None:
+			timestamp = time.time()
+		return email.utils.formatdate(timestamp, usegmt=True)
+
+	def log_date_time_string(self):
+		"""Return the current time formatted for logging."""
+		now = time.time()
+		year, month, day, hh, mm, ss, x, y, z = time.localtime(now)
+		s = "%02d/%3s/%04d %02d:%02d:%02d" % (
+			day, self.monthname[month], year, hh, mm, ss)
+		return s
+
+	weekdayname = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+
+	monthname = [None,
+				 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
+				 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+
+	def address_string(self):
+		"""Return the client address."""
+
+		return self.client_address[0]
+
+	# Essentially static class variables
+
+	# The version of the HTTP protocol we support.
+	# Set this to HTTP/1.1 to enable automatic keepalive
+	protocol_version = "HTTP/1.0"
+
+	# MessageClass used to parse headers
+	MessageClass = http.client.HTTPMessage
+
+	# hack to maintain backwards compatibility
+	responses = {
+		v: (v.phrase, v.description)
+		for v in HTTPStatus.__members__.values()
+	}
+
+
+class SimpleHTTPRequestHandler(BaseHTTPRequestHandler):
+
+	"""Simple HTTP request handler with GET and HEAD commands.
+
+	This serves files from the current directory and any of its
+	subdirectories.  The MIME type for files is determined by
+	calling the .guess_type() method.
+
+	The GET and HEAD requests are identical except that the HEAD
+	request omits the actual contents of the file.
+
+	"""
+
+	server_version = "SimpleHTTP/" + __version__
+
+	if not mimetypes.inited:
+		mimetypes.init()  # try to read system mime.types
+	extensions_map = mimetypes.types_map.copy()
+	extensions_map.update({
+		'': 'application/octet-stream',  # Default
+			'.py': 'text/x-python',
+			'.c': 'text/x-c',
+			'.h': 'text/x-c',
+			'.css': 'text/css',
+
+			'.gz': 'application/gzip',
+			'.Z': 'application/octet-stream',
+			'.bz2': 'application/x-bzip2',
+			'.xz': 'application/x-xz',
+
+			'.webp': 'image/webp',
+
+			'opus': 'audio/opus',
+			'.oga': 'audio/ogg',
+			'.wav': 'audio/wav',
+
+			'.ogv': 'video/ogg',
+			'.ogg': 'application/ogg',
+			'm4a': 'audio/mp4',
+	})
+
+	handlers = {
+		'HEAD': [],
+		'POST': [],
+	}
+
+	def __init__(self, *args, directory=None, **kwargs):
+		if directory is None:
+			directory = os.getcwd()
+		# os.fspath() same as directory, but str, new in 3.6
+		self.directory = os.fspath(directory)
+		super().__init__(*args, **kwargs)
+		self.query = Callable_dict()
+
+	def do_GET(self):
+		"""Serve a GET request."""
+		try:
+			resp = self.send_head()
+		except Exception as e:
+			traceback.print_exc()
+			self.send_error(500, str(e))
+			return
+
+		if resp:
+			try:
+				self.copyfile(resp, self.wfile)
+			except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
+				self.log_info(tools.text_box(e.__class__.__name__,
+							  e, "\nby ", self.address_string()))
+			finally:
+				resp.close()
+
+	def do_(self):
+		'''incase of errored request'''
+		self.send_error(HTTPStatus.BAD_REQUEST, "Bad request.")
+
+	@staticmethod
+	def on_req(type='', url='', hasQ=(), QV={}, fragent='', url_regex='', func=null):
+		'''called when request is received
+		type: GET, POST, HEAD, ...
+		url: url (must start with /)
+		hasQ: if url has query
+		QV: match query value
+		fragent: fragent of request
+		url_regex: url regex (must start with /) url regex, the url must start and end with this regex
+
+		if query is tuple|list, it will only check existence of key
+		if query is dict, it will check value of key
+		'''
+		self = __class__
+
+		type = type.upper()
+		if type == 'GET':
+			type = 'HEAD'
+
+		if type not in self.handlers:
+			self.handlers[type] = []
+
+		# FIXING TYPE ISSUE
+		if isinstance(hasQ, str):
+			hasQ = (hasQ,)
+
+		if url == '' and url_regex == '':
+			url_regex = '.*'
+
+		to_check = (url, hasQ, QV, fragent, url_regex)
+
+		def decorator(func):
+			self.handlers[type].append((to_check, func))
+			return func
+		return decorator
+
+	def test_req(self, url='', hasQ=(), QV={}, fragent='', url_regex=''):
+		'''test if request is matched'
+
+		args:
+			url: url relative path (must start with /)
+			hasQ: if url has query
+			QV: match query value
+			fragent: fragent of request
+			url_regex: url regex, the url must start and end with this regex
+
+
+		'''
+		if url_regex and not re.search("^"+url_regex+'$', self.url_path):
+				return False
+		if url and url != self.url_path:
+			return False
+
+		if isinstance(hasQ, str):
+			hasQ = (hasQ,)
+
+		if hasQ and self.query(*hasQ) is False:
+			return False
+		if QV:
+			for k, v in QV.items():
+				if not self.query(k):
+					return False
+				if self.query[k] != v:
+					return False
+
+		if fragent and self.fragment != fragent:
+			return False
+
+		return True
+
+	def do_HEAD(self):
+		"""Serve a HEAD request."""
+		resp = None
+		try:
+			resp = self.send_head()
+		except Exception as e:
+			traceback.print_exc()
+			self.send_error(500, str(e))
+			return
+		finally:
+			if resp:
+				resp.close()
+
+	def do_POST(self):
+		"""Serve a POST request."""
+		self.range = None, None
+
+		path = self.translate_path(self.path)
+		# DIRECTORY DONT CONTAIN SLASH / AT END
+
+		url_path, query, fragment = self.url_path, self.query, self.fragment
+		spathsplit = self.url_path.split("/")
+
+		try:
+			for case, func in self.handlers['POST']:
+				if self.test_req(*case):
+					try:
+						resp = func(self, url_path=url_path, query=query,
+								fragment=fragment, path=path, spathsplit=spathsplit)
+					except PostError:
+						traceback.print_exc()
+						# break if error is raised and send BAD_REQUEST (at end of loop)
+						break
+
+					if resp:
+						try:
+							self.copyfile(resp, self.wfile)
+						except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
+							logger.info(tools.text_box(
+								e.__class__.__name__, e, "\nby ", [self.address_string()]))
+						finally:
+							resp.close()
+					return
+
+			return self.send_error(HTTPStatus.BAD_REQUEST, "Invalid request.")
+
+		except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
+			logger.info(tools.text_box(e.__class__.__name__,
+						e, "\nby ", [self.address_string()]))
+			return
+		except Exception as e:
+			traceback.print_exc()
+			self.send_error(500, str(e))
+			return
+
+	def redirect(self, location, cookie:Union[SimpleCookie, str]=None):
+		'''redirect to location'''
+		print("REDIRECT ", location)
+		self.send_response(302)
+		self.send_header("Location", location)
+		self._send_cookie(cookie)
+		self.end_headers()
+
+
+
+	def return_txt(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
+		'''returns only the head to client
+		and returns a file object to be used by copyfile'''
+		self.log_debug(f'[RETURNED] {code} to client')
+		if isinstance(msg, Template):
+			msg = msg.safe_substitute(
+				code=code,
+				message=HTTPStatus(code).phrase,
+				explain=HTTPStatus(code).description,
+				version=__version__
+			)
+		if not isinstance(msg, bytes):
+			encoded = msg.encode('utf-8', 'surrogateescape')
+		else:
+			encoded = msg
+
+		box = io.BytesIO()
+		box.write(encoded)
+		box.seek(0)
+
+		self.send_response(code)
+
+		self._send_cookie(cookie)
+
+
+
+		self.send_header("Content-Type", content_type)
+		self.send_header("Content-Length", str(len(encoded)))
+		self.end_headers()
+		return box
+
+	def send_txt(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
+		'''sends the head and file to client'''
+		file = self.return_txt(msg, code, content_type, cookie)
+		if self.command == "HEAD":
+			return  # to avoid sending file on get request
+		self.copyfile(file, self.wfile)
+		file.close()
+
+	def send_text(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/html; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
+		'''proxy to send_txt'''
+		self.send_txt(msg, code, content_type, cookie)
+
+	def return_script(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/javascript; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
+		'''proxy to send_txt'''
+		return self.return_txt(msg, code, content_type, cookie)
+
+	def send_script(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/javascript; charset=utf-8"):
+		'''proxy to send_txt'''
+		return self.send_txt(msg, code, content_type)
+
+	def return_css(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/css; charset=utf-8", cookie:Union[SimpleCookie, str]=None):
+		'''proxy to send_txt'''
+		return self.return_txt(msg, code, content_type, cookie)
+
+	def send_css(self, msg:Union[str, bytes, Template], code:int=200, content_type="text/css; charset=utf-8"):
+		'''proxy to send_txt'''
+		return self.send_txt(msg, code, content_type)
+
+	def send_json(self, obj:Union[object, str, bytes], code=200, cookie:Union[SimpleCookie, str]=None):
+		"""send object as json
+		obj: json-able object or json.dumps() string"""
+		if not isinstance(obj, str):
+			obj = json.dumps(obj, indent=1)
+		file = self.return_txt(obj, code, content_type="application/json", cookie=cookie)
+		if self.command == "HEAD":
+			return  # to avoid sending file on get request
+		self.copyfile(file, self.wfile)
+		file.close()
+
+	def return_file(self, path, filename=None, download=False, cache_control="", cookie:Union[SimpleCookie, str]=None):
+		file = None
+		is_attachment = "attachment;" if (self.query("dl") or download) else ""
+
+		first, last = 0, None
+
+		C_encoding = None
+
+		try:
+			ctype = self.guess_type(path)
+
+			# make sure texts are sent as utf-8
+			if ctype.startswith("text/"):
+				ctype += "; charset=utf-8"
+
+			# if file is gziped, send as gzip
+			if ctype == "application/gzip" and "gzip" in self.headers.get("Accept-Encoding", ""):
+				C_encoding = "gzip"
+
+			file = open(path, 'rb')
+			fs = os.fstat(file.fileno())
+
+			file_len = fs[6]
+			# Use browser cache if possible
+			if ("If-Modified-Since" in self.headers
+					and "If-None-Match" not in self.headers):
+				# compare If-Modified-Since and time of last file modification
+				try:
+					ims = email.utils.parsedate_to_datetime(
+						self.headers["If-Modified-Since"])
+				except (TypeError, IndexError, OverflowError, ValueError):
+					# ignore ill-formed values
+					pass
+				else:
+					if ims.tzinfo is None:
+						# obsolete format with no timezone, cf.
+						# https://tools.ietf.org/html/rfc7231#section-7.1.1.1
+						ims = ims.replace(tzinfo=datetime.timezone.utc)
+					if ims.tzinfo is datetime.timezone.utc:
+						# compare to UTC datetime of last modification
+						last_modif = datetime.datetime.fromtimestamp(
+							fs.st_mtime, datetime.timezone.utc)
+						# remove microseconds, like in If-Modified-Since
+						last_modif = last_modif.replace(microsecond=0)
+
+						if last_modif <= ims:
+							self.send_response(HTTPStatus.NOT_MODIFIED)
+							self.end_headers()
+							file.close()
+
+							return None
+
+			if self.use_range:
+				first = self.range[0]
+				if first is None:
+					first = 0
+				last = self.range[1]
+				if last is None or last >= file_len:
+					last = file_len - 1
+
+				if first >= file_len:  # PAUSE AND RESUME SUPPORT
+					self.send_error(416, 'Requested Range Not Satisfiable', cookie=cookie)
+					return None
+
+				self.send_response(206)
+				self._send_cookie(cookie=cookie)
+
+				self.send_header('Accept-Ranges', 'bytes')
+
+				response_length = last - first + 1
+
+				self.send_header('Content-Range',
+								f'bytes {first}-{last}/{file_len}')
+				self.send_header('Content-Length', str(response_length))
+
+			else:
+				self.send_response(HTTPStatus.OK)
+				self._send_cookie(cookie)
+
+				self.send_header("Content-Length", str(file_len))
+
+			if cache_control:
+				self.send_header("Cache-Control", cache_control)
+
+			self.send_header("Last-Modified",
+							self.date_time_string(fs.st_mtime))
+			self.send_header("Content-Type", ctype)
+
+			if C_encoding:
+				self.send_header("Content-Encoding", C_encoding)
+
+			self.send_header("Content-Disposition", is_attachment+' filename="%s"' %
+							(os.path.basename(path) if filename is None else filename))
+			self.end_headers()
+
+			return file
+
+		except PermissionError:
+			self.send_error(HTTPStatus.FORBIDDEN, "Permission denied", cookie)
+			return None
+
+		except OSError:
+			self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie)
+			return None
+
+		except Exception:
+			traceback.print_exc()
+
+			# if f and not f.closed(): f.close()
+			raise
+
+	def send_file(self, path, filename=None, download=False, cache_control='', cookie:Union[SimpleCookie, str]=None):
+		'''sends the head and file to client'''
+		file = self.return_file(path, filename, download, cache_control, cookie=cookie)
+		if self.command == "HEAD":
+			return  # to avoid sending file on get request
+		try:
+			self.copyfile(file, self.wfile)
+		finally:
+			file.close()
+
+
+	def send_head(self):
+		"""Common code for GET and HEAD commands.
+
+		This sends the response code and MIME headers.
+
+		Return value is either a file object (which has to be copied
+		to the outputfile by the caller unless the command was HEAD,
+		and must be closed by the caller under all circumstances), or
+		None, in which case the caller has nothing further to do.
+
+		"""
+
+		if 'Range' not in self.headers:
+			self.range = None, None
+			first, last = 0, 0
+
+		else:
+			try:
+				self.range = parse_byte_range(self.headers['Range'])
+				first, last = self.range
+				self.use_range = True
+			except ValueError as e:
+				self.send_error(400, 'Invalid byte range')
+				return None
+
+		path = self.translate_path(self.path)
+		# DIRECTORY DONT CONTAIN SLASH / AT END
+
+		url_path, query, fragment = self.url_path, self.query, self.fragment
+
+		spathsplit = self.url_path.split("/")
+
+		# GET WILL Also BE HANDLED BY HEAD
+		for case, func in self.handlers['HEAD']:
+			if self.test_req(*case):
+				return func(self, url_path=url_path, query=query, fragment=fragment, path=path, spathsplit=spathsplit)
+
+		return self.send_error(HTTPStatus.NOT_FOUND, "File not found")
+
+	def get_displaypath(self, url_path):
+		"""
+		Helper to produce a display path for the directory listing.
+		"""
+
+		try:
+			displaypath = urllib.parse.unquote(
+				url_path, errors='surrogatepass')
+		except UnicodeDecodeError:
+			displaypath = urllib.parse.unquote(url_path)
+		displaypath = html.escape(displaypath, quote=False)
+
+		return displaypath
+
+	def get_rel_path(self, filename):
+		"""Return the relative path to the file, FOR WEB."""
+		return urllib.parse.unquote(posixpath.join(self.url_path, filename), errors='surrogatepass')
+	
+	def get_web_path(self, path:str, times=1):
+		"""replace current directory with /"""
+		return path.replace(self.directory, "/", times)
+	
+	def path_safety_check(self, paths:Union[str, list], *more_paths:Union[str, list]):
+		"""check if path is safe
+		paths: list of paths to check"""
+		if isinstance(paths, str):
+			paths = [paths]
+
+		if more_paths:
+			for path in more_paths:
+				if isinstance(path, str):
+					paths.append(path)
+				elif isinstance(path, (list, tuple, set)):
+					paths += more_paths
+				else:
+					raise TypeError(f"Invalid type {type(path)} for path")
+
+
+		for path in paths:
+			if path.startswith(('../', '..\\', '/../', '\\..\\')) or '/../' in path or '\\..\\' in path or path.endswith(('/..', '\\..')):
+				return False
+			
+		return True
+
+
+		
+
+	def translate_path(self, path):
+		"""Translate a /-separated PATH to the local filename syntax.
+
+		Components that mean special things to the local file system
+		(e.g. drive or directory names) are ignored.  (XXX They should
+		probably be diagnosed.)
+
+		"""
+		# abandon query parameters
+		path = path.split('?', 1)[0]
+		path = path.split('#', 1)[0]
+		# Don't forget explicit trailing slash when normalizing. Issue17324
+		trailing_slash = path.rstrip().endswith('/')
+
+		try:
+			path = urllib.parse.unquote(path, errors='surrogatepass')
+		except UnicodeDecodeError:
+			path = urllib.parse.unquote(path)
+		path = posixpath.normpath(path)
+		words = path.split('/')
+		words = filter(None, words)
+		path = self.directory
+
+		for word in words:
+			if os.path.dirname(word) or word in (os.curdir, os.pardir):
+				# Ignore components that are not a simple file/directory name
+				continue
+			path = os.path.join(path, word)
+		if trailing_slash:
+			path += '/'
+
+		return os.path.normpath(path)  # fix OS based path issue
+
+	def copyfile(self, source, outputfile):
+		"""Copy all data between two file objects.
+
+		The SOURCE argument is a file object open for reading
+		(or anything with a read() method) and the DESTINATION
+		argument is a file object open for writing (or
+		anything with a write() method).
+
+		The only reason for overriding this would be to change
+		the block size or perhaps to replace newlines by CRLF
+		-- note however that this the default server uses this
+		to copy binary data as well.
+
+		"""
+		try:
+			# check if file readable
+			source.read(1)
+			source.seek(0)
+		except OSError as e:
+			traceback.print_exc()
+			raise e
+
+		if not self.range:
+			shutil.copyfileobj(source, outputfile)
+
+		else:
+			# SimpleHTTPRequestHandler uses shutil.copyfileobj, which doesn't let
+			# you stop the copying before the end of the file.
+			start, stop = self.range  # set in send_head()
+			copy_byte_range(source, outputfile, start, stop)
+
+	def guess_type(self, path):
+		"""Guess the type of a file.
+
+		Argument is a PATH (a filename).
+
+		Return value is a string of the form type/subtype,
+		usable for a MIME Content-type header.
+
+		The default implementation looks the file's extension
+		up in the table self.extensions_map, using application/octet-stream
+		as a default; however it would be permissible (if
+		slow) to look inside the data to make a better guess.
+
+		"""
+
+		base, ext = posixpath.splitext(path)
+		if ext in self.extensions_map:
+			return self.extensions_map[ext]
+		ext = ext.lower()
+		if ext in self.extensions_map:
+			return self.extensions_map[ext]
+		guess, _ = mimetypes.guess_type(path)
+		if guess:
+			return guess
+
+		return self.extensions_map['']  # return 'application/octet-stream'
+
+
+class PostError(Exception):
+	pass
+
+
+class ContentDisposition:
+	def __init__(self, content_disposition):
+		self.content_disposition = content_disposition
+		self.items = {}
+		self.parse()
+
+	def parse(self):
+		# Content-Disposition: form-data; name="post-type"
+		# Content-Disposition: form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
+		# Content-Disposition: form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+
+		line = re.subn(r"Content-Disposition:", "",
+					   self.content_disposition, flags=re.IGNORECASE, count=1)[0]
+
+		# form-data; name="post-type"
+		# form-data; name="file"; filename="C:\Users\user\Desktop\test.txt"
+		# form-data; name="file"; filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+		parts = (i.strip() for i in line.split(";") if i.strip())
+
+		# form-data
+		# name="post-type"
+		# name="file"
+		# filename="C:\Users\user\Desktop\test.txt"
+		# filename*=utf-8''%E6%B5%8B%E8%AF%95.txt
+
+		for part in parts:
+			pair = [i.strip() for i in part.split("=", 1)]
+
+			key = pair[0]
+			value = pair[1] if len(pair) > 1 else ""
+
+			if key.lower() == "filename*" and value.lower().startswith("utf-8''"):
+				value = urllib.parse.unquote(
+					value[7:], encoding="utf-8", errors='surrogatepass')
+
+				key = "filename"
+
+			self.items[key.lower()] = value.strip('"')
+
+	def get(self, key, default=None):
+		return self.items.get(key.lower(), default)
+
+	def __getitem__(self, key):
+		return self.items[key.lower()]
+
+	def __contains__(self, key):
+		return key.lower() in self.items
+
+
+class DealPostData:
+	"""do_login
+
+#get starting boundary
+0: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
+1: b'Content-Disposition: form-data; name="post-type"\r\n'
+2: b'\r\n'
+3: b'login\r\n'
+4: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
+5: b'Content-Disposition: form-data; name="username"\r\n'
+6: b'\r\n'
+7: b'xxx\r\n'
+8: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa\r\n'
+9: b'Content-Disposition: form-data; name="password"\r\n'
+10: b'\r\n'
+11: b'ccc\r\n'
+12: b'------WebKitFormBoundary7RGDIyjMpWhLXcZa--\r\n'
+"""
+
+	boundary = b''
+	num = 0
+	remainbytes = 0
+
+	def __init__(self, req: SimpleHTTPRequestHandler) -> None:
+		"""After init, must call start() to get boundary and content_length"""
+		self.req = req
+		self.content_length = 0
+		self.content_type = ""
+
+		self.form = FormData(req, self, fake=True)
+
+
+	refresh = "<br><br><div class='pagination center' onclick='window.location.reload()'>Refresh &#128259;</div>"
+
+	def is_multipart(self):
+		return self.content_type.startswith("multipart/form-data")
+
+	def is_urlencoded(self):
+		return self.content_type.startswith("application/x-www-form-urlencoded")
+
+	def is_form_data(self):
+		return self.is_urlencoded() or self.is_multipart()
+
+	def is_json(self):
+		return self.content_type == "application/json"
+
+	def check_size_limit(self, max_size=-1):
+		"""
+		* check if content size is within limit
+		* return True if within limit
+		"""
+		if not max_size < 0 or self.content_length <= max_size:
+			raise PostError(
+				f"Content size limit exceeded: {self.content_length} > {max_size}")
+
+	def get(self, show=F, strip=F, Timeout=10, chunk_size=0):
+		"""
+		show: print line
+		strip: strip \r\n at end
+		Timeout: if having network issue on any side, will keep trying to get content until Timeout (in seconds)
+		"""
+		req = self.req
+
+		if self.remainbytes <= 0:
+			return b""
+
+		if chunk_size <= 0:
+			chunk_size = self.remainbytes
+
+		for _ in range(Timeout*2):
+			if self.is_multipart():
+				line = req.rfile.readline()
+			else:
+				line = req.rfile.read(chunk_size)
+			if line:
+				break
+			time.sleep(.5)
+		else:
+			raise ConnectionAbortedError
+
+		if show:
+			print(f"{self.num}: {line}")
+		self.remainbytes -= len(line)
+		self.num += 1
+
+		if strip and self.is_multipart() and line.endswith(b"\r\n"):
+			line = line.rpartition(b"\r\n")[0]
+
+		return line
+
+	def get_content(self, max_size=-1, chunk_size=0):
+		"""
+		* get content if not multipart
+		* return content
+		"""
+
+		self.check_size_limit(max_size=max_size)
+
+		n = self.remainbytes
+		line = b""
+
+		while n > 0:
+			chunk = n % 1024
+			n -= chunk
+
+			_line = self.get(chunk_size=chunk)
+			if not _line:
+				break
+			line += _line
+
+		return line
+
+	def get_json(self, max_size=-1):
+		"""
+		* get json data
+		* return parsed json data
+		"""
+
+		if not self.content_type == "application/json":
+			raise PostError("Content-Type is not application/json")
+
+		line = self.get_content(max_size=max_size)
+
+		return json.loads(line)
+
+	def skip(self,):
+		self.get()
+
+	def start(self):
+		'''reads upto line 0'''
+		req = self.req
+		self.content_type = req.headers['content-type']
+
+		if not self.content_type:
+			raise PostError("POST request without Content-Type")
+		if self.is_multipart():
+			self.boundary = self.content_type.split("=")[1].encode()
+
+		self.remainbytes = int(req.headers['content-length'])
+		self.content_length = self.remainbytes
+
+		# print(f"Content-Type: {self.content_type}")
+		# print(f"Content-Length: {self.content_length}")
+		# print(f"Request-header: {req.headers}")
+		# print(self.is_form_data())
+
+		if self.is_form_data():
+			self.form = FormData(req, self)
+
+
+class FormData:
+	"""
+	Handler for
+	`multipart/form-data` and
+	`application/x-www-form-urlencoded`
+	"""
+
+	def __init__(self, req: SimpleHTTPRequestHandler, dpd: DealPostData, fake=False) -> None:
+		"""
+		must be initialized from DealPostData
+		"""
+		self.req = req
+		self.dpd = dpd
+		self.fake = fake
+
+		self.content_length = dpd.content_length
+		self.content_type = dpd.content_type
+
+		self.is_multipart = self.dpd.is_multipart()
+		if self.fake:
+			return
+		self.boundary = dpd.boundary
+		if self.is_multipart:
+			# pass first boundary line (because after every field, there is a boundary line)
+			self.pass_bound()
+
+
+	def pass_bound(self):
+		"""
+		* pass boundary line in multipart
+		* raise error if boundary not found
+		"""
+		if self.fake:
+			raise PostError("Fake FormData")
+
+		if not self.is_multipart:
+			raise PostError("Not multipart")
+
+		line = self.dpd.get()
+		if not self.boundary in line:
+			self.req.log_error(f"Content boundary missing on line {self.dpd.num}\n", [
+							   line, self.boundary])
+
+	def get_a_dline(self, line: Union[bytes, str, None] = None):
+		"""
+		* get a line if not provided
+		* decoded if its in bytes
+		* return decoded line
+		"""
+		if self.fake:
+			raise PostError("Fake FormData")
+		# only these 2 needs fake check
+
+		if not line:
+			line = self.dpd.get()
+
+		if isinstance(line, bytes):
+			line = line.decode()
+
+		return line
+
+	def get_file_name(self, line: Union[bytes, str, None] = None):
+		"""
+		* get file name from Content-Disposition
+		* return file name
+		"""
+		line = self.get_a_dline(line)
+
+		cd = ContentDisposition(line)
+		fn = cd.get('filename')
+
+		if not fn:
+			raise PostError("Can't find out file name...")
+
+		return fn
+
+	def get_field_name(self, line=None):
+		"""
+		* get field name from Content-Disposition
+		* return field name
+		"""
+		line = self.get_a_dline(line)
+
+		# get name from Content-Disposition
+		return ContentDisposition(line).get('name')
+
+	def match_field_name(self, field_name: Union[None, str] = None):
+		"""
+		field_name: Expecting name of the field (str)
+		* if None, skip checking field name
+		* if `empty string`, field name must be empty too
+		"""
+		line = self.dpd.get()
+
+		got_field_name = self.get_field_name(line)
+
+		if field_name is not None and got_field_name != field_name:
+			raise PostError(
+				f"Invalid request: Expected {field_name} but got {got_field_name}")
+
+		return got_field_name
+
+	def get_multi_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None, decode=F):
+		'''read a form field
+		ends at boundary
+		verify_name: name of the field (str|bytes|None)
+		verify_msg: message to verify (str|bytes)
+		decode: decode the message
+		* if None, skip checking field name
+		* if `empty string`, field name must be empty too
+
+		returns: field `(name, value)` (str|bytes)
+		'''
+		decoded = False
+
+		if isinstance(verify_name, bytes):
+			verify_name = verify_name.decode()
+
+		# LINE 0 (boundary)
+		field_name = self.match_field_name(verify_name)  # LINE 1 (field name)
+		# if not verified, raise PostError
+
+		if not field_name:
+			return None, None
+
+		self.dpd.skip()  # LINE 2 (blank line)
+
+		line = b''
+		while 1:
+			_line = self.dpd.get()  # from LINE 3 till boundary (form field value)
+			if (not _line) or (self.boundary in _line):  # boundary
+				break
+			line += _line
+
+		if not line:
+			return None, None
+
+		line = line.rpartition(b"\r\n")[0]  # remove \r\n at end
+		if decode:
+			line = line.decode()
+			decoded = True
+		if verify_msg is not None:
+			if not decoded:
+				if isinstance(verify_msg, str):
+					verify_msg = verify_msg.encode()
+
+			if line != verify_msg:
+				raise PostError(
+					f"Invalid post request.\n Expected: {[verify_msg]}\n Got: {[line]}")
+
+		# self.pass_bound() # LINE 5 (boundary)
+
+		return field_name, line
+
+	def get_urlencoded_field(self, verify_name: Union[None, bytes, str] = None, verify_msg: Union[None, bytes, str] = None):
+		"""
+		* get a field from form data
+		* return decoded name, value
+
+		"""
+		line = b""
+		data = self.dpd.get(chunk_size=1)
+		while data or data == b"&":
+			line += data
+
+			data = self.dpd.get(chunk_size=1)
+
+		name, value = line.split(b"=", 1)
+		# URL decode
+		name, value = urllib.parse.unquote(name), urllib.parse.unquote(value)
+
+		if verify_name is not None:
+			if isinstance(verify_name, bytes):
+				verify_name = verify_name.decode()
+
+			if name != verify_name:
+				raise PostError(
+					f"Invalid post request.\n Expected: {verify_name}\n Got: {name}")
+
+		if verify_msg is not None:
+			if isinstance(verify_msg, bytes):
+				verify_msg = verify_msg.decode()
+
+			if value != verify_msg:
+				raise PostError(
+					f"Invalid post request.\n Expected: {verify_msg}\n Got: {value}")
+		return name, value
+
+	def get_urlencoded_iter(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data as dict.
+		"""
+
+		self.dpd.check_size_limit(max_size)
+
+
+		data = self.dpd.get().decode()
+		for part in data.split("&"):
+			name, value = part.split("=")
+			name, value = urllib.parse.unquote(
+				name), urllib.parse.unquote(value)
+
+			yield name, value
+
+	def get_multipart_iter(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data as dict.
+		"""
+
+		self.dpd.check_size_limit(max_size)
+
+		while True:
+			field_name, value = self.get_multi_field(decode=True)
+			if not field_name:
+				break
+			yield field_name, value
+
+	def get_parts(self, max_size=-1):
+		"""
+		Generator that yields the parts of the form data.
+		"""
+		if self.is_multipart:
+			g = self.get_multipart_iter
+		else:
+			g = self.get_urlencoded_iter
+
+		for part in g(max_size):
+			yield part
+
+
+def _get_best_family(*address):
+	infos = socket.getaddrinfo(
+		*address,
+		type=socket.SOCK_STREAM,
+		flags=socket.AI_PASSIVE
+	)
+	family, type, proto, canonname, sockaddr = next(iter(infos))
+	return family, sockaddr
+
+
+def get_ip(bind=None):
+	IP = bind  # or "127.0.0.1"
+	s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+	s.settimeout(0)
+	try:
+		# doesn't even have to be reachable
+		s.connect(('10.255.255.255', 1))
+		IP = s.getsockname()[0]
+	except:
+		try:
+			if config.OS == "Android":
+				IP = s.connect(("192.168.43.1",  1))
+				IP = s.getsockname()[0]
+				# Assigning this variable because Android does't return actual IP when hosting a hotspot
+		except (socket.herror, OSError):
+			pass
+	finally:
+		s.close()
+	return IP
+
+
+def test(HandlerClass=BaseHTTPRequestHandler,
+		 ServerClass=ThreadingHTTPServer,
+		 protocol="HTTP/1.0", port=8000, bind=None):
+	"""Test the HTTP request handler class.
+
+	This runs an HTTP server on port 8000 (or the port argument).
+
+	"""
+
+	global httpd
+	if sys.version_info >= (3, 8):  # BACKWARD COMPATIBILITY
+		ServerClass.address_family, addr = _get_best_family(bind, port)
+	else:
+		addr = (bind if bind != None else '', port)
+
+	device_ip = bind or "127.0.0.1"
+	# bind can be None (=> 127.0.0.1) or a string (=> 127.0.0.DDD)
+
+	HandlerClass.protocol_version = protocol
+	httpd = ServerClass(addr, HandlerClass)
+	host, port = httpd.socket.getsockname()[:2]
+	url_host = f'[{host}]' if ':' in host else host
+	hostname = socket.gethostname()
+	local_ip = config.IP if config.IP else get_ip(device_ip)
+	config.IP = local_ip
+
+	on_network = local_ip != (device_ip)
+
+	logger.info(tools.text_box(
+		# TODO: need to check since the output is "Serving HTTP on :: port 6969"
+		f"Serving HTTP on {host} port {port} \n",
+		# TODO: need to check since the output is "(http://[::]:6969/) ..."
+		f"(http://{url_host}:{port}/) ...\n",
+		f"Server is probably running on\n",
+		(f"[over NETWORK] {config.address()}\n" if on_network else ""),
+		f"[on DEVICE] http://localhost:{config.port} & http://127.0.0.1:{config.port}", style="star", sep=""
+	)
+	)
+	try:
+		httpd.serve_forever(poll_interval=0.1)
+	except KeyboardInterrupt:
+		logger.info("\nKeyboard interrupt received, exiting.")
+
+	except OSError:
+		logger.info("\nOSError received, exiting.")
+	finally:
+		if not config.reload:
+			sys.exit(0)
+
+
+class DualStackServer(ThreadingHTTPServer):  # UNSUPPORTED IN PYTHON 3.7
+
+	def handle_error(self, request, client_address):
+		pass
+
+	def server_bind(self):
+		# suppress exception when protocol is IPv4
+		with contextlib.suppress(Exception):
+			self.socket.setsockopt(
+				socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
+		return super().server_bind()
+
+	def finish_request(self, request, client_address):
+		self.RequestHandlerClass(request, client_address, self,
+								 directory=config.ftp_dir)
+
+
+def run(port=0, directory="", bind="", arg_parse=True, handler=SimpleHTTPRequestHandler):
+
+	if arg_parse:
+		args = config.parse_default_args(
+			port=port, directory=directory, bind=bind)
+
+		port = args.port
+		directory = args.directory
+		bind = args.bind
+
+	logger.info(tools.text_box("Running pyroboxCore: ",
+				config.MAIN_FILE, "Version: ", __version__))
+
+	if directory == config.ftp_dir and not os.path.isdir(config.ftp_dir):
+		logger.warning(
+			config.ftp_dir, "not found!\nReseting directory to current directory")
+		directory = "."
+
+	handler_class = partial(handler,
+							directory=directory)
+
+	config.port = port
+	if port > 65535 or port < 0:
+		raise ValueError("Port must be between 0 and 65535")
+
+	config.ftp_dir = directory
+
+	if not config.reload:
+		if sys.version_info > (3, 8):
+			test(
+				HandlerClass=handler_class,
+				ServerClass=DualStackServer,
+				port=port,
+				bind=bind,
+			)
+		else:  # BACKWARD COMPATIBILITY
+			test(
+				HandlerClass=handler_class,
+				ServerClass=ThreadingHTTPServer,
+				port=port,
+				bind=bind,
+			)
+
+	if config.reload == True:
+		reload_server()
+
+
+if __name__ == '__main__':
+	run()
```

### Comparing `pyrobox-0.9.4/src/pyrobox_ServerHost.py` & `pyrobox-0.9.5/src/pyrobox_ServerHost.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-from http import HTTPStatus
-import os
-from typing import Union
-
-from ._fs_utils import get_titles, dir_navigator
-from .pyroDB import PickleTable
-from . import user_mgmt as u_mgmt
-from .user_mgmt import User
-
-from .pyroboxCore import config as CoreConfig, SimpleHTTPRequestHandler as SH_base, SimpleCookie, tools
-
-
-from string import Template
-from . import _page_templates as pt
-
-
-
-
-
-
-class ServerConfig():
-	def __init__(self, cli_args):
-		self.name = cli_args.name
-		self.admin_username = cli_args.admin_id
-		self.admin_password = cli_args.admin_pass
-
-		self.uDB = PickleTable()
-		self.configDB = PickleTable()
-		self.cli_args = cli_args
-
-
-		self.GUESTS =  not self.cli_args.no_guest_allowed  # unless account mode, everyone is guest
-
-		self.admin_perms = []
-		self.member_perms = []
-		self.guest_perms = []
-
-		self.init_config()
-		self.init_permissions(cli_args=cli_args)
-		self.init_account()
-
-		# Max size a zip file will be made
-		self.max_zip_size = 6*1024*1024*1024 # 6GB
-
-	def init_config(self):
-		if self.name:
-			if not self.name:
-				raise ValueError("If you want to create a server User accounts based, value of --name is required")
-			if not (self.admin_username and self.admin_password):
-				raise ValueError("If you want to create a User accounts based server, --name and --admin-id and --admin-pass values are required")
-
-			config_loc = os.path.join(CoreConfig.MAIN_FILE_dir, "config", self.name+ ".pdb")
-
-			os.makedirs(os.path.dirname(config_loc), exist_ok=True)
-			self.configDB = PickleTable(config_loc)
-
-		self.configDB.add_column("name", "value", exist_ok=True)
-
-
-
-	def init_account(self):
-		userDB_loc = "" # will  create in memory
-		if self.name:
-			userDB_loc = os.path.join(CoreConfig.MAIN_FILE_dir, "userDB", self.name+ ".pdb")
-			os.makedirs(os.path.dirname(userDB_loc), exist_ok=True)
-
-		self.user_handler = u_mgmt.User_handler(init_permissions= {"member": self.member_perms, "admin": self.admin_perms, "guest": self.guest_perms})
-
-		self.user_handler.load_db(userDB_loc)
-		self.uDB = self.user_handler.user_db
-
-		if (self.admin_username and self.admin_password):
-			_admin = self.user_handler.get_user(self.admin_username, temp=True)
-
-			if _admin:
-				if not _admin.is_admin:
-					raise ValueError(tools.text_box("Provided username is not an admin"))
-				if not _admin.check_password(self.admin_password):
-					raise ValueError(tools.text_box("Admin password is incorrect"))
-
-			elif self.uDB.height == 0:
-				self.user_handler.create_admin(self.admin_username, self.admin_password)
-
-			else:
-				raise ValueError(tools.text_box("Please start the server with an existing admin account"))
-
-		if self.GUESTS:
-			self.guest_id = self.user_handler.create_guest()
-
-# This will contain server configurations, user database and limits.
-
-
-	def init_permissions(self, cli_args):
-		def check(arg, perm):
-			if arg:
-				return perm
-
-		permits = u_mgmt.permits
-
-		DefaultPerms = self.configDB.find_1st("DefaultPerm", 'name')
-
-		if DefaultPerms:
-			self.DefaultPerms = DefaultPerms.row_obj()
-		else:
-			self.DefaultPerms = self.configDB.add_row(dict(name="DefaultPerm", value={}))
-
-		def remove_perm(perm_list, perm):
-			if perm in perm_list:
-				perm_list.remove(perm)
-
-		if self.DefaultPerms["value"].get("member", None):
-			self.member_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["member"])
-		else:
-			self.member_perms = [
-				permits.VIEW,
-				check(not cli_args.no_upload, permits.UPLOAD),
-				check(not cli_args.no_zip, permits.ZIP),
-				check(not cli_args.no_modify, permits.MODIFY),
-				check(not cli_args.no_delete, permits.DELETE),
-				check(not cli_args.no_download, permits.DOWNLOAD),
-				permits.MEMBER,
-			]
-
-			if cli_args.view_only or cli_args.read_only:
-				remove_perm(self.member_perms, permits.UPLOAD)
-				remove_perm(self.member_perms, permits.MODIFY)
-				remove_perm(self.member_perms, permits.DELETE)
-
-			if cli_args.view_only:
-				remove_perm(self.member_perms, permits.DOWNLOAD)
-
-
-		#######
-
-		if self.DefaultPerms["value"].get("admin", None):
-			self.admin_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["admin"])
-		else:
-			self.admin_perms = [
-				permits.VIEW,
-				permits.DELETE,
-				permits.DOWNLOAD,
-				permits.MODIFY,
-				permits.UPLOAD,
-				permits.ZIP,
-				permits.ADMIN,
-				permits.MEMBER,
-			]
-
-
-		#######
-		if self.DefaultPerms["value"].get("guest", None):
-			self.guest_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["guest"])
-		elif not self.name:
-			self.guest_perms = self.member_perms # if no account mode, guest is member
-			self.guest_perms.remove(permits.MEMBER) # remove member permission
-
-		else:
-			self.guest_perms = [
-				check(cli_args.guest_allowed, permits.VIEW),
-				check(not cli_args.no_upload, permits.UPLOAD),
-				check(not cli_args.no_zip, permits.ZIP),
-				check(not cli_args.no_modify, permits.MODIFY),
-				check(not cli_args.no_delete, permits.DELETE),
-				check(not cli_args.no_download, permits.DOWNLOAD),
-			]
-
-			if cli_args.view_only or cli_args.read_only:
-				remove_perm(self.guest_perms, permits.UPLOAD)
-				remove_perm(self.guest_perms, permits.MODIFY)
-				remove_perm(self.guest_perms, permits.DELETE)
-
-			if cli_args.view_only:
-				remove_perm(self.guest_perms, permits.DOWNLOAD)
-
-
-		# remove None values
-		self.member_perms = [x for x in self.member_perms if x is not None]
-		self.admin_perms = [x for x in self.admin_perms if x is not None]
-		self.guest_perms = [x for x in self.guest_perms if x is not None]
-
-		self.update_config_perms() # update the config file with the new permissions | can be used from the admin page
-
-	def update_config_perms(self):
-			"""
-			Update the permissions in the config file database
-
-			This method updates the default permissions for members, admins, and guests.
-			"""
-			self.DefaultPerms["value"]["member"] = User.pack_permission_from_list(self.member_perms)
-			self.DefaultPerms["value"]["admin"] = User.pack_permission_from_list(self.admin_perms)
-			self.DefaultPerms["value"]["guest"] = User.pack_permission_from_list(self.guest_perms)
-
-
-
-	def get_users(self):
-		return self.uDB.get_column("username")
-
-
-
-
-
-
-#############################################
-#            PATCH SERVER CLASS            #
-#############################################
-
-
-
-
-class ServerHost(SH_base):
-	"""
-	Just a wrapper for SH_base to add some extra functionality
-	"""
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-
-	def html_main_page(self, user:User, *args, cookie:Union[SimpleCookie, str]=None,  **kwargs):
-		"""
-		Return HTML page for the directory listing
-		"""
-
-		if user.NOPERMISSION or user.VIEW == False:
-			return self.send_error(HTTPStatus.UNAUTHORIZED, "You don't have permission to see file list", cookie=cookie)
-
-
-		displaypath = self.get_displaypath(self.url_path)
-
-		title = get_titles(displaypath)
-
-		_format = pt.directory_explorer_header().safe_substitute(
-			PY_ERROR_PAGE="",
-			PY_PAGE_TITLE=title,
-			PY_PUBLIC_URL=CoreConfig.address(),
-			PY_DIR_TREE_NO_JS=dir_navigator(displaypath),
-			*args, **kwargs)
-
-		return self.send_text(_format,  cookie=cookie)
-
-
-	def send_error(self, code, message=None, explain=None, cookie:Union[SimpleCookie, str]=None):
-		self.log_warning(["ERROR", code, message, explain]) # why warning? because it's not an server error, it's just a warning of error on client side
-
-		displaypath = self.get_displaypath(self.url_path)
-
-		title = get_titles(displaypath)
-
-		_format = pt.error_page().safe_substitute(
-			PY_ERROR_PAGE="active",
-			PY_PAGE_TITLE=title,
-			PY_PUBLIC_URL=CoreConfig.address(),
-			PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
-
-		return super().send_error(code, message, explain, Template(_format), cookie=cookie)
+from http import HTTPStatus
+import os
+from typing import Union
+
+from ._fs_utils import get_titles, dir_navigator
+from .pyroDB import PickleTable
+from . import user_mgmt as u_mgmt
+from .user_mgmt import User
+
+from .pyroboxCore import config as CoreConfig, SimpleHTTPRequestHandler as SH_base, SimpleCookie, tools
+
+
+from string import Template
+from . import _page_templates as pt
+
+
+
+
+
+
+class ServerConfig():
+	def __init__(self, cli_args):
+		self.name = cli_args.name
+		self.admin_username = cli_args.admin_id
+		self.admin_password = cli_args.admin_pass
+
+		self.uDB = PickleTable()
+		self.configDB = PickleTable()
+		self.cli_args = cli_args
+
+
+		self.GUESTS =  not self.cli_args.no_guest_allowed  # unless account mode, everyone is guest
+
+		self.admin_perms = []
+		self.member_perms = []
+		self.guest_perms = []
+
+		self.init_config()
+		self.init_permissions(cli_args=cli_args)
+		self.init_account()
+
+		# Max size a zip file will be made
+		self.max_zip_size = 6*1024*1024*1024 # 6GB
+
+	def init_config(self):
+		if self.name:
+			if not self.name:
+				raise ValueError("If you want to create a server User accounts based, value of --name is required")
+			if not (self.admin_username and self.admin_password):
+				raise ValueError("If you want to create a User accounts based server, --name and --admin-id and --admin-pass values are required")
+
+			config_loc = os.path.join(CoreConfig.MAIN_FILE_dir, "config", self.name+ ".pdb")
+
+			os.makedirs(os.path.dirname(config_loc), exist_ok=True)
+			self.configDB = PickleTable(config_loc)
+
+		self.configDB.add_column("name", "value", exist_ok=True)
+
+
+
+	def init_account(self):
+		userDB_loc = "" # will  create in memory
+		if self.name:
+			userDB_loc = os.path.join(CoreConfig.MAIN_FILE_dir, "userDB", self.name+ ".pdb")
+			os.makedirs(os.path.dirname(userDB_loc), exist_ok=True)
+
+		self.user_handler = u_mgmt.User_handler(init_permissions= {"member": self.member_perms, "admin": self.admin_perms, "guest": self.guest_perms})
+
+		self.user_handler.load_db(userDB_loc)
+		self.uDB = self.user_handler.user_db
+
+		if (self.admin_username and self.admin_password):
+			_admin = self.user_handler.get_user(self.admin_username, temp=True)
+
+			if _admin:
+				if not _admin.is_admin:
+					raise ValueError(tools.text_box("Provided username is not an admin"))
+				if not _admin.check_password(self.admin_password):
+					raise ValueError(tools.text_box("Admin password is incorrect"))
+
+			elif self.uDB.height == 0:
+				self.user_handler.create_admin(self.admin_username, self.admin_password)
+
+			else:
+				raise ValueError(tools.text_box("Please start the server with an existing admin account"))
+
+		if self.GUESTS:
+			self.guest_id = self.user_handler.create_guest()
+
+# This will contain server configurations, user database and limits.
+
+
+	def init_permissions(self, cli_args):
+		def check(arg, perm):
+			if arg:
+				return perm
+
+		permits = u_mgmt.permits
+
+		DefaultPerms = self.configDB.find_1st("DefaultPerm", 'name')
+
+		if DefaultPerms:
+			self.DefaultPerms = DefaultPerms.row_obj()
+		else:
+			self.DefaultPerms = self.configDB.add_row(dict(name="DefaultPerm", value={}))
+
+		def remove_perm(perm_list, perm):
+			if perm in perm_list:
+				perm_list.remove(perm)
+
+		if self.DefaultPerms["value"].get("member", None):
+			self.member_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["member"])
+		else:
+			self.member_perms = [
+				permits.VIEW,
+				check(not cli_args.no_upload, permits.UPLOAD),
+				check(not cli_args.no_zip, permits.ZIP),
+				check(not cli_args.no_modify, permits.MODIFY),
+				check(not cli_args.no_delete, permits.DELETE),
+				check(not cli_args.no_download, permits.DOWNLOAD),
+				permits.MEMBER,
+			]
+
+			if cli_args.view_only or cli_args.read_only:
+				remove_perm(self.member_perms, permits.UPLOAD)
+				remove_perm(self.member_perms, permits.MODIFY)
+				remove_perm(self.member_perms, permits.DELETE)
+
+			if cli_args.view_only:
+				remove_perm(self.member_perms, permits.DOWNLOAD)
+
+
+		#######
+
+		if self.DefaultPerms["value"].get("admin", None):
+			self.admin_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["admin"])
+		else:
+			self.admin_perms = [
+				permits.VIEW,
+				permits.DELETE,
+				permits.DOWNLOAD,
+				permits.MODIFY,
+				permits.UPLOAD,
+				permits.ZIP,
+				permits.ADMIN,
+				permits.MEMBER,
+			]
+
+
+		#######
+		if self.DefaultPerms["value"].get("guest", None):
+			self.guest_perms = User.unpack_permission_to_list(self.DefaultPerms["value"]["guest"])
+		elif not self.name:
+			self.guest_perms = self.member_perms # if no account mode, guest is member
+			self.guest_perms.remove(permits.MEMBER) # remove member permission
+
+		else:
+			self.guest_perms = [
+				check(cli_args.guest_allowed, permits.VIEW),
+				check(not cli_args.no_upload, permits.UPLOAD),
+				check(not cli_args.no_zip, permits.ZIP),
+				check(not cli_args.no_modify, permits.MODIFY),
+				check(not cli_args.no_delete, permits.DELETE),
+				check(not cli_args.no_download, permits.DOWNLOAD),
+			]
+
+			if cli_args.view_only or cli_args.read_only:
+				remove_perm(self.guest_perms, permits.UPLOAD)
+				remove_perm(self.guest_perms, permits.MODIFY)
+				remove_perm(self.guest_perms, permits.DELETE)
+
+			if cli_args.view_only:
+				remove_perm(self.guest_perms, permits.DOWNLOAD)
+
+
+		# remove None values
+		self.member_perms = [x for x in self.member_perms if x is not None]
+		self.admin_perms = [x for x in self.admin_perms if x is not None]
+		self.guest_perms = [x for x in self.guest_perms if x is not None]
+
+		self.update_config_perms() # update the config file with the new permissions | can be used from the admin page
+
+	def update_config_perms(self):
+			"""
+			Update the permissions in the config file database
+
+			This method updates the default permissions for members, admins, and guests.
+			"""
+			self.DefaultPerms["value"]["member"] = User.pack_permission_from_list(self.member_perms)
+			self.DefaultPerms["value"]["admin"] = User.pack_permission_from_list(self.admin_perms)
+			self.DefaultPerms["value"]["guest"] = User.pack_permission_from_list(self.guest_perms)
+
+
+
+	def get_users(self):
+		return self.uDB.get_column("username")
+
+
+
+
+
+
+#############################################
+#            PATCH SERVER CLASS            #
+#############################################
+
+
+
+
+class ServerHost(SH_base):
+	"""
+	Just a wrapper for SH_base to add some extra functionality
+	"""
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+
+
+	def html_main_page(self, user:User, *args, cookie:Union[SimpleCookie, str]=None,  **kwargs):
+		"""
+		Return HTML page for the directory listing
+		"""
+
+		if user.NOPERMISSION or user.VIEW == False:
+			return self.send_error(HTTPStatus.UNAUTHORIZED, "You don't have permission to see file list", cookie=cookie)
+
+
+		displaypath = self.get_displaypath(self.url_path)
+
+		title = get_titles(displaypath)
+
+		_format = pt.directory_explorer_header().safe_substitute(
+			PY_ERROR_PAGE="",
+			PY_PAGE_TITLE=title,
+			PY_PUBLIC_URL=CoreConfig.address(),
+			PY_DIR_TREE_NO_JS=dir_navigator(displaypath),
+			*args, **kwargs)
+
+		return self.send_text(_format,  cookie=cookie)
+
+
+	def send_error(self, code, message=None, explain=None, cookie:Union[SimpleCookie, str]=None):
+		self.log_warning(["ERROR", code, message, explain]) # why warning? because it's not an server error, it's just a warning of error on client side
+
+		displaypath = self.get_displaypath(self.url_path)
+
+		title = get_titles(displaypath)
+
+		_format = pt.error_page().safe_substitute(
+			PY_ERROR_PAGE="active",
+			PY_PAGE_TITLE=title,
+			PY_PUBLIC_URL=CoreConfig.address(),
+			PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
+
+		return super().send_error(code, message, explain, Template(_format), cookie=cookie)
```

### Comparing `pyrobox-0.9.4/src/server.py` & `pyrobox-0.9.5/src/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1613 +1,1624 @@
-
-
-
-# TODO
-# ----------------------------------------------------------------
-# * ADD MORE FILE TYPES
-# * ADD SEARCH
-
-import os
-#import sys
-import posixpath
-import shutil
-
-import datetime
-
-
-import urllib.parse
-import urllib.request
-
-#import subprocess
-import json
-from http import HTTPStatus
-from http.cookies import SimpleCookie
-
-
-import traceback
-
-from .pyroboxCore import config as CoreConfig, logger, DealPostData as DPD, run as run_server, tools, reload_server, __version__
-
-from ._fs_utils import get_titles, dir_navigator, get_dir_size, get_stat, get_tree_count_n_size, fmbytes, humanbytes
-from ._arg_parser import main as arg_parser
-from . import _page_templates as pt
-from ._exceptions import LimitExceed
-from ._zipfly_manager import ZIP_Manager
-from ._list_maker import list_directory, list_directory_json, list_directory_html
-
-
-from .pyrobox_ServerHost import ServerConfig, ServerHost as SH
-
-
-
-__version__ = __version__
-true = T = True
-false = F = False
-enc = "utf-8"
-
-###########################################
-# ADD COMMAND LINE ARGUMENTS
-###########################################
-arg_parser(CoreConfig)
-cli_args = CoreConfig.parser.parse_known_args()[0]
-CoreConfig.PASSWORD = cli_args.password
-
-logger.info(tools.text_box("Server Config", *({i: getattr(cli_args, i)} for i in vars(cli_args) if not (i.startswith("admin") or "password" in i))))
-
-
-Sconfig = ServerConfig(cli_args=cli_args)
-
-
-
-
-
-###########################################
-# CoreConfig.dev_mode = False
-pt.pt_config.dev_mode = CoreConfig.dev_mode
-
-CoreConfig.MAIN_FILE = os.path.abspath(__file__)
-
-CoreConfig.disabled_func.update({
-			"send2trash": False,
-			"natsort": False,
-			"zip": False,
-			"update": False,
-			"delete": False,
-			"download": False,
-			"upload": False,
-			"new_folder": False,
-			"rename": False,
-})
-
-########## ZIP MANAGER ################################
-# max_zip_size = 6*1024*1024*1024
-zip_manager = ZIP_Manager(CoreConfig, size_limit=Sconfig.max_zip_size)
-
-#######################################################
-
-
-
-# INSTALL REQUIRED PACKAGES
-REQUIREMENTS= ['send2trash', 'natsort']
-
-
-
-
-
-
-
-
-
-
-
-if not os.path.isdir(CoreConfig.log_location):
-	try:
-		os.mkdir(path=CoreConfig.log_location)
-	except Exception:
-		CoreConfig.log_location ="./"
-
-
-
-
-if not CoreConfig.disabled_func["send2trash"]:
-	try:
-		from send2trash import send2trash, TrashPermissionError
-	except Exception:
-		CoreConfig.disabled_func["send2trash"] = True
-		logger.warning("send2trash module not found, send2trash function disabled")
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# TODO check against user_mgmt
-# download file from url using urllib
-def fetch_url(url, file = None):
-	try:
-		with urllib.request.urlopen(url, timeout=5) as response:
-			data = response.read() # a `bytes` object
-			if not file:
-				return data
-
-		with open(file, 'wb') as f:
-			f.write(data)
-		return data
-	except Exception:
-		traceback.print_exc()
-		return None
-
-
-
-
-class PostError(Exception):
-	pass
-
-
-
-def handle_user_cookie(self: SH):
-	cookie = self.cookie
-	#print(cookie)
-	def get(k):
-		x = cookie.get(k)
-		if x is not None:
-			return x.value
-		return ""
-	username = get("user")
-	token = get("token")
-
-	self.log_info("COOKIE", username, token)
-
-	if not (username and token):
-		return None
-
-	user = Sconfig.user_handler.get_user(username)
-	#self.log_info("TEMP_USER", user)
-#	self.log_info("TEMP_TOKEN_CHECK", user.check_token(token))
-
-	if user:
-		if user.check_token(token):
-			return user
-		else:
-			return None
-	return None
-
-def add_user_cookie(user):
-	# add cookie with 1 year expire
-	cookie = SimpleCookie()
-	def x(k, v):
-		nonlocal cookie
-		cookie[k] = v
-		cookie[k]["expires"] = 365*86400
-		cookie[k]["path"] = "/"
-
-	x("user", user.username)
-	x("token", user.token_hex)
-	x("permissions", user.permission_pack)
-	return cookie
-
-def clear_user_cookie():
-	cookie = SimpleCookie()
-	keys = ("user", "token", "permissions")
-	for k in keys:
-		cookie[k] = ""
-		cookie[k]["expires"] = -1
-		cookie[k]["path"] = "/"
-
-	return cookie
-
-def Authorize_user(self:SH):
-	# do cookie stuffs and get user
-	user = handle_user_cookie(self)
-
-	# self.log_info("USER", user)
-
-
-	if not user and Sconfig.GUESTS:
-		user = Sconfig.guest_id # default guest user
-
-	if not user:
-		return None, clear_user_cookie()
-
-	cookie = add_user_cookie(user)
-
-
-	return user, cookie
-
-
-
-
-
-
-
-@SH.on_req('HEAD', hasQ="type")
-def get_page_type(self: SH, *args, **kwargs):
-	"""Return type of the page"""
-	user, cookie = Authorize_user(self)
-
-
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-
-	result= "unknown"
-
-	if self.query("admin"):
-		result = "admin"
-
-	elif self.query("login"):
-		result = "login"
-
-	elif self.query("signup"):
-		result = "signup"
-
-	elif self.query("vid"):
-		result = "vid"
-
-	elif self.query("czip"):
-		result = "zip"
-
-	elif url_path == "/favicon.ico":
-		result = "favicon"
-
-
-
-	elif os.path.isdir(os_path):
-		for index in "index.html", "index.htm":
-			index = os.path.join(os_path, index)
-			if os.path.exists(index):
-				result = "html"
-				break
-
-		else:
-			if self.query("json"):
-				result = "dir_json"
-			else:
-				result = "dir"
-
-	elif os.path.isfile(os_path):
-		result = "file"
-
-	return self.return_txt(result, cookie=cookie)
-
-
-
-
-@SH.on_req('HEAD', '/favicon.ico')
-def send_favicon(self: SH, *args, **kwargs):
-	self.redirect('https://cdn.jsdelivr.net/gh/RaSan147/pyrobox@main/assets/favicon.ico')
-
-@SH.on_req('HEAD', hasQ="reload")
-def reload(self: SH, *args, **kwargs):
-	# RELOADS THE SERVER BY RE-READING THE FILE, BEST FOR TESTING REMOTELY. VULNERABLE
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-
-	CoreConfig.reload = True
-	self.send_text("Reload initiated")
-
-	reload_server()
-
-@SH.on_req('HEAD', hasQ="shutdown")
-def shutdown(self: SH, *args, **kwargs):
-	# SHUTS DOWN THE SERVER. VULNERABLE
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	self.send_text("Shut down initiated", cookie=cookie)
-	self.server.shutdown()
-
-@SH.on_req('HEAD', hasQ="admin")
-def admin_page(self: SH, *args, **kwargs):
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	return self.html_main_page(user, cookie=cookie)
-
-
-
-
-@SH.on_req('HEAD', hasQ="get_users")
-def get_users(self: SH, *args, **kwargs):
-	"""Send list of users"""
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-
-
-	return self.send_json(Sconfig.get_users(), cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ="update_user_perm")
-def update_user_perm(self: SH, *args, **kwargs):
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	query = self.query
-	username = query.get("username", [None])[0]
-	permission = query.get("perms", [None])[0]
-
-	try:
-		permission = int(permission)
-	except Exception:
-		permission = None
-
-	if not (username is not None and permission is not None):
-		return self.send_json({"status": "Failed", "message": "Username or permission not provided"}, cookie=cookie)
-
-	USER = Sconfig.user_handler.get_user(username, temp=True)
-	if not USER:
-		return self.send_json({"status": "Failed", "message": "User not found"}, cookie=cookie)
-
-	USER.set_permission_pack(permission)
-
-	self.log_warning(f'Updating permission of "{username}" to "{permission}" by {[USER.uid]}')
-
-	return self.send_json({"status": "Success", "message": "Permission updated"}, cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ="get_user_perm")
-def get_user_perm(self: SH, *args, **kwargs):
-	"""Send permission of a user"""
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	username = self.query.get("username", [None])[0]
-
-	if not username:
-		return self.send_json({"status": False, "message": "Username not provided"}, cookie=cookie)
-
-	USER = Sconfig.user_handler.get_user(username, temp=True)
-	if not USER:
-		return self.send_json({"status": False, "message": "User not found"}, cookie=cookie)
-
-	return self.send_json({"status": True, "permissions_code": USER.permission_pack}, cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ="add_user") # added by Admin
-def add_user(self: SH, *args, **kwargs):
-	"""Add a user"""
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	username = self.query.get("username", [None])[0]
-	password = self.query.get("password", [None])[0]
-
-	if not (username and password):
-		return self.send_json({"status": False, "message": "Username or password not provided"}, cookie=cookie)
-
-	if Sconfig.user_handler.get_user(username):
-		return self.send_json({"status": False, "message": "Username already exists"}, cookie=cookie)
-
-	new_user = Sconfig.user_handler.create_user(username, password)
-	if not new_user:
-		return self.send_json({"status": False, "message": "Failed to create user"}, cookie=cookie)
-
-	return self.send_json({"status": True, "message": f"<h2>User created.</h2> UID: {new_user.uid}"}, cookie=cookie)
-
-
-
-@SH.on_req('HEAD', hasQ="delete_user")
-def delete_user(self: SH, *args, **kwargs):
-	"""Delete a user"""
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	username = self.query.get("username", [None])[0]
-
-	if not username:
-		return self.send_json({"status": False, "message": "Username not provided"}, cookie=cookie)
-
-	USER = Sconfig.user_handler.get_user(username, temp=True)
-	if not USER:
-		return self.send_json({"status": False, "message": "User not found"}, cookie=cookie)
-
-	if USER.is_admin():
-		return self.send_json({"status": False, "message": "Cannot delete admin! Remove from admin 1st."}, cookie=cookie)
-
-	if not Sconfig.user_handler.delete_user(username): # delete user
-		return self.send_json({"status": False, "message": "Failed to delete user"}, cookie=cookie)
-
-	return self.send_json({"status": True, "message": "User deleted"}, cookie=cookie)
-
-
-
-@SH.on_req('HEAD', hasQ="update")
-def update(self: SH, *args, **kwargs):
-	"""Check for update and return the latest version"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
-
-	if not user.is_admin():
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-
-
-	data = fetch_url("https://raw.githack.com/RaSan147/pyrobox/main/VERSION")
-	if data:
-		data  = data.decode("utf-8").strip()
-		ret = json.dumps({"update_available": data > __version__, "latest_version": data})
-		return self.return_txt(ret, HTTPStatus.OK, cookie=cookie)
-	else:
-		return self.return_txt("Failed to fetch latest version", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ="size")
-def get_size(self: SH, *args, **kwargs):
-	"""Return size of the file"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-
-	url_path = kwargs.get('url_path', '')
-	os_path = self.translate_path(url_path)
-
-	stat = get_stat(os_path)
-	if not stat:
-		return self.send_json({"status": 0}, cookie=cookie)
-	if os.path.isfile(os_path):
-		size = stat.st_size
-	else:
-		size = get_dir_size(os_path)
-
-	humanbyte = humanbytes(size)
-	fmbyte = fmbytes(size)
-	return self.send_json({"status": 1,
-														"byte": size,
-														"humanbyte": humanbyte,
-														"fmbyte": fmbyte}, cookie=cookie)
-
-@SH.on_req('HEAD', hasQ="size_n_count")
-def get_size_n_count(self: SH, *args, **kwargs):
-	"""Return size of the file"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-
-	url_path = kwargs.get('url_path', '')
-	os_path = self.translate_path(url_path)
-
-	stat = get_stat(os_path)
-	if not stat:
-		return self.send_json({"status": 0}, cookie=cookie)
-	if os.path.isfile(os_path):
-		count, size = 1, stat.st_size
-	else:
-		count, size = get_tree_count_n_size(os_path)
-
-	humanbyte = humanbytes(size)
-	fmbyte = fmbytes(size)
-	return self.send_json({"status": 1,
-														"byte": size,
-														"humanbyte": humanbyte,
-														"fmbyte": fmbyte,
-														"count": count}, cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ=("zip_id", "czip"))
-def get_zip_id(self: SH, *args, **kwargs):
-	"""Return ZIP ID status"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.ZIP:
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-	
-	if not (user.DOWNLOAD and user.VIEW):
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	if CoreConfig.disabled_func["zip"]:
-		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
-	
-	
-	os_path = kwargs.get('path')
-	spathsplit = kwargs.get('spathsplit')
-	filename = spathsplit[-2] + ".zip"
-
-	zid = None
-	status = False
-	message = ''
-	
-	try:
-		zid = zip_manager.get_id(os_path)
-		status = True
-
-	except LimitExceed:
-		message = 'Directory size limit exceed'
-		
-	except Exception:
-		self.log_error(traceback.format_exc())
-		message = 'Failed to create zip'
-
-	return self.send_json({
-		"status": status,
-		"message": message,
-		"zid": zid,
-		"filename": filename
-	}, cookie=cookie)
-
-
-@SH.on_req('HEAD', hasQ="czip")
-def create_zip(self: SH, *args, **kwargs):
-	"""Create ZIP task and return ID
-
-	# TODO: Move to Dynamic island
-	"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.ZIP:
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-	
-	if not (user.DOWNLOAD and user.VIEW):
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	if CoreConfig.disabled_func["zip"]:
-		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
-
-	url_path = kwargs.get('url_path', '')
-	os_path = self.translate_path(url_path)
-
-	# if not dir or not exists
-	if not os.path.isdir(os_path):
-		return self.send_error(HTTPStatus.NOT_FOUND, "Directory not found", cookie=cookie)
-
-
-	# dir_size = get_dir_size(path, limit=6*1024*1024*1024)
-
-	# if dir_size == -1:
-	# 	msg = "Directory size is too large, please contact the host"
-	# 	return self.return_txt(HTTPStatus.OK, msg)
-
-	displaypath = self.get_displaypath(url_path)
-
-	title = "Creating ZIP"
-
-	data = pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
-											PY_PUBLIC_URL=CoreConfig.address(),
-											PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
-	
-	return self.return_txt(data, cookie=cookie)
-
-
-
-@SH.on_req('HEAD', hasQ="zip")
-def get_zip(self: SH, *args, **kwargs):
-	"""Return ZIP file if available
-	Else return progress of the task"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	if not user.ZIP:
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-	
-	if not (user.DOWNLOAD and user.VIEW):
-		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
-
-	if CoreConfig.disabled_func["zip"]:
-		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
-
-
-
-	os_path = kwargs.get('path')
-	spathsplit = kwargs.get('spathsplit')
-
-	query = self.query
-	msg = False
-
-	def reply(status, msg=""):
-		return self.send_json({
-			"status": status,
-			"message": msg
-		}, cookie=cookie)
-
-	if not os.path.isdir(os_path):
-		msg = "Folder not found. Failed to create zip"
-		self.log_error(msg)
-		return reply("ERROR", msg)
-
-
-	filename = spathsplit[-2] + ".zip"
-
-	id = query["zid"][0]
-
-	# IF NOT STARTED
-	if zip_manager.calculating(id):
-		return reply("CALCULATING")
-
-	if not zip_manager.zip_id_status(id):
-		t = zip_manager.archive_thread(os_path, id)
-		t.start()
-
-		return reply("SUCCESS", "ARCHIVING")
-
-
-	if zip_manager.zip_id_status[id] == "DONE":
-		if query("download"):
-			zip_path = zip_manager.zip_ids[id]
-
-			return self.return_file(zip_path, filename, True, cookie=cookie)
-
-
-		if query("progress"):
-			return reply("DONE") #if query("progress") or no query
-
-	# IF IN PROGRESS
-	if zip_manager.zip_id_status[id] == "ARCHIVING":
-		progress = zip_manager.zip_in_progress[id]
-		# return self.return_txt("%.2f" % progress)
-		return reply("PROGRESS", "%.2f" % progress)
-
-	if zip_manager.zip_id_status[id].startswith("ERROR"):
-		# return self.return_txt(zip_manager.zip_id_status[id])
-		return reply("ERROR", zip_manager.zip_id_status[id])
-
-@SH.on_req('HEAD', hasQ="json")
-def send_ls_json(self: SH, *args, **kwargs):
-	"""Send directory listing in JSON format"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	return list_directory_json(self)
-
-
-
-
-@SH.on_req('HEAD', hasQ=("vid", "vid-data"))
-def send_video_data(self: SH, *args, **kwargs):
-	# SEND VIDEO DATA
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-
-
-	vid_source = url_path
-
-	content_type = self.guess_type(os_path)
-
-	if not content_type.startswith('video/'):
-		self.send_error(HTTPStatus.NOT_FOUND, "THIS IS NOT A VIDEO FILE", cookie=cookie)
-		return None
-
-
-	displaypath = self.get_displaypath(url_path)
-
-	title = get_titles(displaypath, file=True)
-
-
-	warning = ""
-
-	if content_type not in ['video/mp4', 'video/ogg', 'video/webm']:
-		warning = ('<h2>It seems HTML player may not be able to play this Video format, Try Downloading</h2>')
-
-	return self.send_json({
-		"status": "success",
-		"warning": warning,
-		"video": vid_source,
-		"title": displaypath.split("/")[-1],
-		"content_type": content_type,
-	}, cookie=cookie)
-
-
-
-@SH.on_req('HEAD', hasQ="vid")
-def send_video_page(self: SH, *args, **kwargs):
-	# SEND VIDEO PLAYER
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-	# vid_source = url_path
-	content_type = self.guess_type(os_path)
-
-	if not content_type.startswith('video/'):
-		self.send_error(HTTPStatus.NOT_FOUND, "THIS IS NOT A VIDEO FILE", cookie=cookie)
-		return None
-
-	r = []
-
-	displaypath = self.get_displaypath(url_path)
-
-
-
-	title = get_titles(displaypath, file=True)
-
-	r.append(pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
-													PY_PUBLIC_URL=CoreConfig.address(),
-													PY_DIR_TREE_NO_JS= dir_navigator(displaypath)))
-
-	encoded = '\n'.join(r).encode(enc, 'surrogateescape')
-	return self.return_txt(encoded, cookie=cookie)
-
-
-
-
-
-
-# @SH.on_req('HEAD', url_regex="/@assets/.*")
-# def send_assets(self: SH, *args, **kwargs):
-# 	"""Send assets"""
-# 	user = Authorize_user(self)
-
-# 	if not user: # guest or not will be handled in Authentication
-# 		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
-
-# 	if not CoreConfig.ASSETS:
-# 		self.send_error(HTTPStatus.NOT_FOUND, "Assets not available")
-# 		return None
-
-
-# 	path = kwargs.get('path')
-# 	spathsplit = kwargs.get('spathsplit')
-
-# 	path = CoreConfig.ASSETS_dir + "/".join(spathsplit[2:])
-# 	#	print("USING ASSETS", path)
-
-# 	if not os.path.isfile(path):
-# 		self.send_error(HTTPStatus.NOT_FOUND, "File not found")
-# 		return None
-
-# 	return self.return_file(path)
-
-@SH.on_req('HEAD', hasQ="style")
-def send_style(self: SH, *args, **kwargs):
-	"""Send style sheet"""
-	return self.send_css(pt.style_css())
-
-@SH.on_req('HEAD', hasQ="global_script")
-def send_global_script(self: SH, *args, **kwargs):
-	"""Send global script"""
-	return self.send_script(pt.global_script(), content_type="text/javascript")
-
-@SH.on_req('HEAD', hasQ="asset_script")
-def send_script(self: SH, *args, **kwargs):
-	"""Send script"""
-	return self.send_script(pt.assets_script())
-
-@SH.on_req('HEAD', hasQ="theme_script")
-def send_theme_script(self: SH, *args, **kwargs):
-	"""Send theme script"""
-	return self.send_script(pt.theme_script())
-
-@SH.on_req('HEAD', hasQ="page_handler_script")
-def send_page_handler_script(self: SH, *args, **kwargs):
-	"""Send page handler script"""
-	return self.send_script(pt.page_handler_script())
-
-@SH.on_req('HEAD', hasQ="video_page_script")
-def send_video_script(self: SH, *args, **kwargs):
-	"""Send video script"""
-	return self.send_script(pt.video_page_script())
-
-@SH.on_req('HEAD', hasQ="admin_page_script")
-def send_admin_script(self: SH, *args, **kwargs):
-	"""Send admin script"""
-	return self.send_script(pt.admin_page_script())
-
-@SH.on_req('HEAD', hasQ="file_list_script")
-def send_file_list_script(self: SH, *args, **kwargs):
-	"""Send file list script"""
-	return self.send_script(pt.file_list_script())
-
-@SH.on_req('HEAD', hasQ="error_page_script")
-def send_error_page_script(self: SH, *args, **kwargs):
-	"""Send error page script"""
-	return self.send_script(pt.error_page_script())
-
-@SH.on_req('HEAD', hasQ="zip_page_script")
-def send_zip_page_script(self: SH, *args, **kwargs):
-	"""Send zip page script"""
-	return self.send_script(pt.zip_page_script())
-
-
-
-@SH.on_req('HEAD', hasQ="login")
-def login_page(self: SH, *args, **kwargs):
-	"""Send login page"""
-	user, cookie = Authorize_user(self)
-
-	if user:
-		return self.redirect("/")
-
-	return self.send_text(pt.login_page())
-
-@SH.on_req('HEAD', hasQ="signup")
-def signup_page(self: SH, *args, **kwargs):
-	"""Send signup page"""
-	user, cookie = Authorize_user(self)
-
-	if user:
-		return self.redirect("/")
-
-	if Sconfig.cli_args.no_signup:
-		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Signup is disabled")
-
-	return self.send_text(pt.signup_page())
-
-
-
-
-
-
-
-
-
-@SH.on_req('HEAD', hasQ="folder_data")
-def get_folder_data(self: SH, *args, **kwargs):
-	"""Send folder data"""
-	user, cookie = Authorize_user(self)
-
-	if not user:
-		return self.send_json({
-			"status": 0,
-			"error_code": HTTPStatus.UNAUTHORIZED,
-			"error_message": "You must be logged in to access this data.",
-
-		}, cookie=cookie)
-
-	os_path = kwargs.get('path')
-
-	if not user.VIEW:
-		return self.send_json({
-			"status": 0,
-			"error_code": HTTPStatus.UNAUTHORIZED,
-			"error_message": "You don't have permission to view this folder",
-
-		}, cookie=cookie)
-
-
-	try:
-		if not os.path.isdir(os_path):
-			return self.send_json({"status": 0,
-						"warning": "Folder not found"}, cookie=cookie)
-
-	except Exception as e:
-		err = traceback.format_exc()
-		return self.send_json({
-			"status": 0,
-			"error_code": HTTPStatus.NOT_FOUND,
-			"error_message": str(e),
-
-		})
-
-	data = list_directory(self, os_path, user, cookie=cookie)
-
-	if data:
-		return self.send_json(data, cookie=cookie)
-
-
-@SH.on_req('HEAD')
-def default_get(self: SH, filename=None, *args, **kwargs):
-	"""Serve a GET request."""
-	user, cookie = Authorize_user(self)
-
-	#print("/"*50)
-	#print(user.permission)
-	#print("/"*50)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.redirect("?login")
-
-
-	os_path = kwargs.get('path')
-
-	if os.path.isdir(os_path):
-		parts = urllib.parse.urlsplit(self.path)
-		if not parts.path.endswith('/'):
-			# redirect browser - doing basically what apache does
-			self.send_response(HTTPStatus.MOVED_PERMANENTLY)
-			new_parts = (parts[0], parts[1], parts[2] + '/',
-							parts[3], parts[4])
-			new_url = urllib.parse.urlunsplit(new_parts)
-			self.send_header("Location", new_url)
-			self.send_header("Content-Length", "0")
-			self.end_headers()
-			return None
-		for index in "index.html", "index.htm":
-			index = os.path.join(os_path, index)
-			if os.path.exists(index):
-				os_path = index
-				break
-		else:
-			return list_directory_html(self, os_path, user, cookie=cookie)
-
-	# check for trailing "/" which should return 404. See Issue17324
-	# The test for this was added in test_httpserver.py
-	# However, some OS platforms accept a trailingSlash as a filename
-	# See discussion on python-dev and Issue34711 regarding
-	# parsing and rejection of filenames with a trailing slash
-
-	if os_path.endswith("/"):
-		self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie=cookie)
-		return None
-
-
-
-	# else:
-
-	if (not user.DOWNLOAD) or user.NOPERMISSION:
-		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Download is disabled", cookie=cookie)
-
-	if not os.path.exists(os_path):
-		return self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie=cookie)
-	return self.return_file(os_path, filename, cookie=cookie)
-
-
-
-
-
-
-
-
-
-
-
-
-# TODO check against user_mgmt
-def AUTHORIZE_POST(req: SH, post:DPD, post_type=''):
-	"""Check if the user is authorized to post"""
-
-	# START
-	post.start()
-	form = post.form
-
-	verify_1 = form.get_multi_field(verify_name='post-type', verify_msg=post_type, decode=T)
-
-	return verify_1[1]
-
-
-@SH.on_req('POST', hasQ="do_login")
-def handle_login_post(self: SH, *args, **kwargs):
-	"""Handle login post"""
-	user, cookie = Authorize_user(self)
-
-	if user:
-		return self.redirect("/")
-
-
-
-	post = DPD(self)
-
-	AUTHORIZE_POST(self, post, 'login')
-
-	form = post.form
-
-	username = form.get_multi_field(verify_name='username', decode=T)[1]
-
-	# GET PASSWORD
-	password = form.get_multi_field(verify_name='password', decode=T)[1]
-
-	user = Sconfig.user_handler.get_user(username)
-	if not user:
-		return self.send_json({"status": "failed", "message": "User not found"}, cookie=cookie)
-
-	if not user.check_password(password):
-		return self.send_json({"status": "failed", "message": "Incorrect password"}, cookie=cookie)
-
-	cookie = add_user_cookie(user)
-
-	return self.send_json({"status": "success", "message": "Login successful, if not Auto-redirecting, kindly Refresh"}, cookie=cookie)
-
-
-@SH.on_req('POST', hasQ="do_signup")
-def handle_signup_post(self: SH, *args, **kwargs):
-	"""Handle signup post"""
-	user, cookie = Authorize_user(self)
-
-	if user:
-		return self.redirect("/")
-
-	if Sconfig.cli_args.no_signup:
-		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Signup is disabled")
-
-
-	post = DPD(self)
-
-	AUTHORIZE_POST(self, post, 'signup')
-
-	form = post.form
-
-	username = form.get_multi_field(verify_name='username', decode=T)[1]
-
-	# GET PASSWORD
-	password = form.get_multi_field(verify_name='password', decode=T)[1]
-
-	user = Sconfig.user_handler.get_user(username)
-	if user:
-		return self.send_json({"status": "failed", "message": "Username is already in use!"}, cookie=cookie)
-
-	user = Sconfig.user_handler.create_user(username, password)
-	if not user:
-		return self.send_json({"status": "failed", "message": "Failed to create user"}, cookie=cookie)
-
-	cookie = add_user_cookie(user)
-
-	return self.send_json({"status": "success", "message": "Signup successful"}, cookie=cookie)
-
-
-
-
-# TODO check against user_mgmt
-@SH.on_req('POST', hasQ="upload")
-def upload(self: SH, *args, **kwargs):
-	"""GET Uploaded files"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	if user.NOPERMISSION or (not user.UPLOAD):
-		return self.send_txt("Upload not allowed", HTTPStatus.SERVICE_UNAVAILABLE, cookie=cookie)
-
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-
-	post = DPD(self)
-
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'upload')
-
-	form = post.form
-
-	if not uid:
-		return None
-
-
-	uploaded_files = [] # Uploaded folder list
-
-
-
-	# PASSWORD SYSTEM
-	password = form.get_multi_field(verify_name='password', decode=T)[1]
-
-	self.log_debug(f'post password: {[password]} by client')
-
-	if (user.MEMBER and not user.check_password(password)) or (not user.MEMBER and password != CoreConfig.PASSWORD): # readline returns password with \r\n at end
-		self.log_info(f"Incorrect password by {uid}")
-
-		return self.send_txt("Incorrect password", HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-	while post.remainbytes > 0:
-		fn = form.get_file_name() # reads the next line and returns the file name
-		if not fn:
-			return self.send_error(HTTPStatus.BAD_REQUEST, "Can't find out file name...", cookie=cookie)
-
-
-		rltv_path = posixpath.join(url_path, fn)
-		
-		if not self.path_safety_check(fn, rltv_path):
-			return self.send_txt("Invalid Path:  " + rltv_path, HTTPStatus.BAD_REQUEST, cookie=cookie)
-
-		temp_fn = os.path.join(os_path, ".LStemp-"+fn +'.tmp')
-		CoreConfig.temp_file.add(temp_fn)
-
-
-		os_f_path = os.path.join(os_path, fn)
-
-
-
-		line = post.get() # content type
-		line = post.get() # line gap
-
-
-
-		# ORIGINAL FILE STARTS FROM HERE
-		try:
-			with open(temp_fn, 'wb') as out:
-				preline = post.get()
-				while post.remainbytes > 0:
-					line = post.get()
-					if post.boundary in line:
-						preline = preline[0:-1]
-						if preline.endswith(b'\r'):
-							preline = preline[0:-1]
-						out.write(preline)
-						uploaded_files.append(rltv_path,)
-						break
-					else:
-						out.write(preline)
-						preline = line
-
-
-			while (not user.MODIFY) and os.path.isfile(os_f_path):
-				n = 1
-				name, ext = os.path.splitext(os_f_path)
-				fn = f"{name}({n}){ext}"
-				n += 1
-			os.replace(temp_fn, os_f_path)
-
-
-
-		except (IOError, OSError):
-			traceback.print_exc()
-
-			return self.send_txt("Can't create file to write, do you have permission to write?", HTTPStatus.SERVICE_UNAVAILABLE, cookie=cookie)
-
-		finally:
-			try:
-				os.remove(temp_fn)
-				CoreConfig.temp_file.remove(temp_fn)
-
-			except OSError:
-				pass
-
-
-
-	return self.return_txt("File(s) uploaded", cookie=cookie)
-
-
-
-
-
-@SH.on_req('POST', hasQ="del-f")
-def del_2_recycle(self: SH, *args, **kwargs):
-	"""Move 2 recycle bin"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	if user.NOPERMISSION or (not user.DELETE):
-		return self.send_json({"head": "Failed", "body": "You have no permission to delete."}, cookie=cookie)
-
-	url_path = kwargs.get('url_path')
-
-
-	post = DPD(self)
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'del-f')
-	form = post.form
-
-	if CoreConfig.disabled_func["send2trash"]:
-		return self.send_json({"head": "Failed", "body": "Recycling unavailable! Try deleting permanently..."}, cookie=cookie)
-
-
-
-	# File link to move to recycle bin
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-
-	rel_path = self.get_rel_path(filename)
-	
-	if not self.path_safety_check(filename, rel_path):
-		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
-	
-	os_f_path = self.translate_path(posixpath.join(url_path, filename))
-
-	self.log_warning(f'<-send2trash-> {os_f_path} by {[uid]}')
-
-	head = "Failed"
-	try:
-		if CoreConfig.OS == 'Android':
-			raise InterruptedError
-		send2trash(os_f_path)
-		msg = "Successfully Moved To Recycle bin"+ post.refresh
-		head = "Success"
-	except TrashPermissionError:
-		msg = "Recycling unavailable! Try deleting permanently..."
-	except InterruptedError:
-		msg = "Recycling unavailable! Try deleting permanently..."
-	except Exception as e:
-		traceback.print_exc()
-		msg = "<b>" + rel_path + "</b> " + e.__class__.__name__
-
-	return self.send_json({"head": head, "body": msg}, cookie=cookie)
-
-
-
-
-
-@SH.on_req('POST', hasQ="del-p")
-def del_permanently(self: SH, *args, **kwargs):
-	"""DELETE files permanently"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	if user.NOPERMISSION or (not user.DELETE):
-		return self.send_json({"head": "Failed", "body": "Recycling unavailable! Try deleting permanently..."}, cookie=cookie)
-
-	url_path = kwargs.get('url_path')
-
-
-	post = DPD(self)
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'del-p')
-	form = post.form
-
-
-
-	# File link to move to recycle bin
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-
-	rel_path = self.get_rel_path(filename)
-
-	if not self.path_safety_check(filename, rel_path):
-		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
-
-	os_f_path = self.translate_path(posixpath.join(url_path, filename))
-
-	self.log_warning(f'Perm. DELETED {os_f_path} by {[uid]}')
-
-
-	try:
-		if os.path.isfile(os_f_path): os.remove(os_f_path)
-		else: shutil.rmtree(os_f_path, ignore_errors=True)
-
-		return self.send_json({"head": "Success", "body": "PERMANENTLY DELETED  " + rel_path + post.refresh}, cookie=cookie)
-
-
-	except Exception as e:
-		traceback.print_exc()
-		return self.send_json({"head": "Failed", "body": "<b>" + rel_path + "<b>" + e.__class__.__name__}, cookie=cookie)
-
-
-
-
-
-@SH.on_req('POST', hasQ="rename")
-def rename_content(self: SH, *args, **kwargs):
-	"""Rename files"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	if user.NOPERMISSION or (not user.MODIFY):
-		return self.send_json({"head": "Failed", "body": "Renaming is disabled."}, cookie=cookie)
-
-
-	url_path = kwargs.get('url_path')
-
-
-	post = DPD(self)
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'rename')
-	form = post.form
-
-
-
-	# File link to move to recycle bin
-	
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-	new_name = form.get_multi_field(verify_name='data', decode=T)[1].strip()
-
-	rel_path = self.get_rel_path(filename)
-	new_rel_path = self.get_rel_path(new_name)
-
-	if not self.path_safety_check(filename, new_name, rel_path, new_rel_path):
-		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
-
-	os_f_path = self.translate_path(posixpath.join(url_path, filename))
-	os_new_f_path = self.translate_path(posixpath.join(url_path, new_name))
-
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-
-
-
-	self.log_warning(f'Renamed "{os_f_path}" to "{os_new_f_path}" by {[uid]}')
-
-
-	try:
-		os.rename(os_f_path, os_new_f_path)
-		return self.send_json({"head": "Renamed Successfully", "body":  post.refresh}, cookie=cookie)
-	except Exception as e:
-		return self.send_json({"head": "Failed", "body": "<b>" + rel_path + "</b><br><b>" + e.__class__.__name__ + "</b> : " + self.get_web_path(str(e), -1) }, cookie=cookie)
-
-
-
-
-
-@SH.on_req('POST', hasQ="info")
-def get_info(self: SH, *args, **kwargs):
-	"""Get files permanently"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
-
-
-	if user.NOPERMISSION:
-		return self.send_json({"head": "Failed", "body": "You have no permission to view."}, cookie=cookie)
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-	script = None
-
-
-	post = DPD(self)
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'info')
-	form = post.form
-
-
-	# File link to move to check info
-
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-
-	rel_path = self.get_rel_path(filename)
-
-	if not self.path_safety_check(filename, rel_path):
-		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
-
-	os_f_path = self.translate_path(posixpath.join(url_path, filename))
-
-
-	self.log_warning(f'Info Checked "{os_f_path}" by: {[uid]}')
-
-	if not os.path.exists(os_f_path):
-		return self.send_json({"head":"Failed", "body":"File/Folder Not Found"}, cookie=cookie)
-
-	file_stat = get_stat(os_f_path)
-	if not file_stat:
-		return self.send_json({"head":"Failed", "body":"Permission Denied"}, cookie=cookie)
-
-	data = []
-	data.append(["Name", urllib.parse.unquote(filename, errors= 'surrogatepass')])
-
-	if os.path.isfile(os_f_path):
-		data.append(["Type","File"])
-		if "." in filename:
-			data.append(["Extension", filename.rpartition(".")[2]])
-
-		size = file_stat.st_size
-		data.append(["Size", humanbytes(size) + " (%i bytes)"%size])
-
-	else: #if os.path.isdir(xpath):
-		data.append(["Type", "Folder"])
-		# size = get_dir_size(xpath)
-
-		data.append(["Total Files", '<span id="f_count">Please Wait</span>'])
-
-
-		data.append(["Total Size", '<span id="f_size">Please Wait</span>'])
-		script = '''
-		tools.fetch_json(tools.full_path("''' + rel_path + '''?size_n_count")).then(resp => {
-		// console.log(resp);
-		if (resp.status) {
-			size = resp.humanbyte;
-			count = resp.count;
-			document.getElementById("f_size").innerHTML = resp.humanbyte + " (" + resp.byte + " bytes)";
-			document.getElementById("f_count").innerHTML = count;
-		} else {
-			throw new Error(resp.msg);
-		}}).catch(err => {
-		console.log(err);
-		document.getElementById("f_size").innerHTML = "Error";
-		});
-		'''
-
-	data.append(["Path", rel_path])
-
-	def get_dt(time):
-		return datetime.datetime.fromtimestamp(time)
-
-	data.append(["Created on", get_dt(file_stat.st_ctime)])
-	data.append(["Last Modified", get_dt(file_stat.st_mtime)])
-	data.append(["Last Accessed", get_dt(file_stat.st_atime)])
-
-	body = """
-<style>
-table {
-	font-family: arial, sans-serif;
-	border-collapse: collapse;
-	width: 100%;
-}
-
-td, th {
-	border: 1px solid #00BFFF;
-	text-align: left;
-	padding: 8px;
-}
-
-tr:nth-child(even) {
-	background-color: #111;
-}
-</style>
-
-<table>
-<tr>
-<th>About</th>
-<th>Info</th>
-</tr>
-"""
-	for key, val in data:
-		body += "<tr><td>{key}</td><td>{val}</td></tr>".format(key=key, val=val)
-	body += "</table>"
-
-	return self.send_json({"head":"Properties", "body":body, "script":script}, cookie=cookie)
-
-
-@SH.on_req('POST', hasQ="new_folder")
-def new_folder(self: SH, *args, **kwargs):
-	"""Create new folder"""
-	user, cookie = Authorize_user(self)
-
-	if not user: # guest or not will be handled in Authentication
-		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
-
-	if user.NOPERMISSION or (not user.MODIFY):
-		return self.send_json({"head": "Failed", "body": "Permission denied."}, cookie=cookie)
-
-
-	os_path = kwargs.get('path')
-	url_path = kwargs.get('url_path')
-
-	post = DPD(self)
-
-	# AUTHORIZE
-	uid = AUTHORIZE_POST(self, post, 'new_folder')
-	form = post.form
-
-	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
-
-	rel_path = self.get_rel_path(filename)
-
-	if not self.path_safety_check(filename, rel_path):
-		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
-
-	os_f_path = self.translate_path(posixpath.join(url_path, filename))
-
-
-	self.log_warning(f'New Folder Created "{os_f_path}" by: {[uid]}')
-
-	try:
-		if os.path.exists(os_f_path):
-			return self.send_json({"head": "Failed", "body": "Folder Already Exists:  " + rel_path}, cookie=cookie)
-		if os.path.isfile(os_f_path):
-			return self.send_json({"head": "Failed", "body": "File Already Exists:  " + rel_path}, cookie=cookie)
-		os.makedirs(os_f_path)
-		return self.send_json({"head": "Success", "body": "New Folder Created:  " + rel_path +post.refresh}, cookie=cookie)
-
-	except Exception as e:
-		self.log_error(traceback.format_exc())
-		return self.send_json({"head": "Failed", "body": f"<b>{ rel_path }</b><br><b>{ e.__class__.__name__ }</b>"}, cookie=cookie)
-
-
-
-
-
-@SH.on_req('POST')
-def default_post(self: SH, *args, **kwargs):
-	raise PostError("Bad Request")
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# proxy for old versions
-def run(*args, **kwargs):
-	run_server(handler=SH, *args, **kwargs)
-
-if __name__ == '__main__':
-	run(port = 45454)
+
+
+
+# TODO
+# ----------------------------------------------------------------
+# * ADD MORE FILE TYPES
+# * ADD SEARCH
+
+import os
+#import sys
+import posixpath
+import shutil
+
+import datetime
+
+
+import threading
+import urllib.parse
+import urllib.request
+
+#import subprocess
+import json
+from http import HTTPStatus
+from http.cookies import SimpleCookie
+
+
+import traceback
+
+from .pyroboxCore import config as CoreConfig, logger, DealPostData as DPD, run as run_server, tools, reload_server, __version__
+
+from ._fs_utils import get_titles, dir_navigator, get_dir_size, get_stat, get_tree_count_n_size, fmbytes, humanbytes, UploadHandler
+from ._arg_parser import main as arg_parser
+from . import _page_templates as pt
+from ._exceptions import LimitExceed
+from ._zipfly_manager import ZIP_Manager
+from ._list_maker import list_directory, list_directory_json, list_directory_html
+
+
+from .pyrobox_ServerHost import ServerConfig, ServerHost as SH
+
+
+
+__version__ = __version__
+true = T = True
+false = F = False
+enc = "utf-8"
+
+###########################################
+# ADD COMMAND LINE ARGUMENTS
+###########################################
+arg_parser(CoreConfig)
+cli_args = CoreConfig.parser.parse_known_args()[0]
+CoreConfig.PASSWORD = cli_args.password
+
+logger.info(tools.text_box("Server Config", *({i: getattr(cli_args, i)} for i in vars(cli_args) if not (i.startswith("admin") or "password" in i))))
+
+
+Sconfig = ServerConfig(cli_args=cli_args)
+
+
+
+
+
+###########################################
+# CoreConfig.dev_mode = False
+pt.pt_config.dev_mode = CoreConfig.dev_mode
+
+CoreConfig.MAIN_FILE = os.path.abspath(__file__)
+
+CoreConfig.disabled_func.update({
+			"send2trash": False,
+			"natsort": False,
+			"zip": False,
+			"update": False,
+			"delete": False,
+			"download": False,
+			"upload": False,
+			"new_folder": False,
+			"rename": False,
+})
+
+########## ZIP MANAGER ################################
+# max_zip_size = 6*1024*1024*1024
+zip_manager = ZIP_Manager(CoreConfig, size_limit=Sconfig.max_zip_size)
+
+#######################################################
+
+
+
+# INSTALL REQUIRED PACKAGES
+REQUIREMENTS= ['send2trash', 'natsort']
+
+
+
+
+
+
+
+
+
+
+
+if not os.path.isdir(CoreConfig.log_location):
+	try:
+		os.mkdir(path=CoreConfig.log_location)
+	except Exception:
+		CoreConfig.log_location ="./"
+
+
+
+
+if not CoreConfig.disabled_func["send2trash"]:
+	try:
+		from send2trash import send2trash, TrashPermissionError
+	except Exception:
+		CoreConfig.disabled_func["send2trash"] = True
+		logger.warning("send2trash module not found, send2trash function disabled")
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# TODO check against user_mgmt
+# download file from url using urllib
+def fetch_url(url, file = None):
+	try:
+		with urllib.request.urlopen(url, timeout=5) as response:
+			data = response.read() # a `bytes` object
+			if not file:
+				return data
+
+		with open(file, 'wb') as f:
+			f.write(data)
+		return data
+	except Exception:
+		traceback.print_exc()
+		return None
+
+
+
+
+class PostError(Exception):
+	pass
+
+
+
+def handle_user_cookie(self: SH):
+	cookie = self.cookie
+	#print(cookie)
+	def get(k):
+		x = cookie.get(k)
+		if x is not None:
+			return x.value
+		return ""
+	username = get("user")
+	token = get("token")
+
+	self.log_info("COOKIE", username, token)
+
+	if not (username and token):
+		return None
+
+	user = Sconfig.user_handler.get_user(username)
+	#self.log_info("TEMP_USER", user)
+#	self.log_info("TEMP_TOKEN_CHECK", user.check_token(token))
+
+	if user:
+		if user.check_token(token):
+			return user
+		else:
+			return None
+	return None
+
+def add_user_cookie(user):
+	# add cookie with 1 year expire
+	cookie = SimpleCookie()
+	def x(k, v):
+		nonlocal cookie
+		cookie[k] = v
+		cookie[k]["expires"] = 365*86400
+		cookie[k]["path"] = "/"
+
+	x("user", user.username)
+	x("token", user.token_hex)
+	x("permissions", user.permission_pack)
+	return cookie
+
+def clear_user_cookie():
+	cookie = SimpleCookie()
+	keys = ("user", "token", "permissions")
+	for k in keys:
+		cookie[k] = ""
+		cookie[k]["expires"] = -1
+		cookie[k]["path"] = "/"
+
+	return cookie
+
+def Authorize_user(self:SH):
+	# do cookie stuffs and get user
+	user = handle_user_cookie(self)
+
+	# self.log_info("USER", user)
+
+
+	if not user and Sconfig.GUESTS:
+		user = Sconfig.guest_id # default guest user
+
+	if not user:
+		return None, clear_user_cookie()
+
+	cookie = add_user_cookie(user)
+
+
+	return user, cookie
+
+
+
+
+
+
+
+@SH.on_req('HEAD', hasQ="type")
+def get_page_type(self: SH, *args, **kwargs):
+	"""Return type of the page"""
+	user, cookie = Authorize_user(self)
+
+
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+
+	result= "unknown"
+
+	if self.query("admin"):
+		result = "admin"
+
+	elif self.query("login"):
+		result = "login"
+
+	elif self.query("signup"):
+		result = "signup"
+
+	elif self.query("vid"):
+		result = "vid"
+
+	elif self.query("czip"):
+		result = "zip"
+
+	elif url_path == "/favicon.ico":
+		result = "favicon"
+
+
+
+	elif os.path.isdir(os_path):
+		for index in "index.html", "index.htm":
+			index = os.path.join(os_path, index)
+			if os.path.exists(index):
+				result = "html"
+				break
+
+		else:
+			if self.query("json"):
+				result = "dir_json"
+			else:
+				result = "dir"
+
+	elif os.path.isfile(os_path):
+		result = "file"
+
+	return self.return_txt(result, cookie=cookie)
+
+
+
+
+@SH.on_req('HEAD', '/favicon.ico')
+def send_favicon(self: SH, *args, **kwargs):
+	self.redirect('https://cdn.jsdelivr.net/gh/RaSan147/pyrobox@main/assets/favicon.ico')
+
+@SH.on_req('HEAD', hasQ="reload")
+def reload(self: SH, *args, **kwargs):
+	# RELOADS THE SERVER BY RE-READING THE FILE, BEST FOR TESTING REMOTELY. VULNERABLE
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+
+	CoreConfig.reload = True
+	self.send_text("Reload initiated")
+
+	reload_server()
+
+@SH.on_req('HEAD', hasQ="shutdown")
+def shutdown(self: SH, *args, **kwargs):
+	# SHUTS DOWN THE SERVER. VULNERABLE
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	self.send_text("Shut down initiated", cookie=cookie)
+	self.server.shutdown()
+
+@SH.on_req('HEAD', hasQ="admin")
+def admin_page(self: SH, *args, **kwargs):
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	return self.html_main_page(user, cookie=cookie)
+
+
+
+
+@SH.on_req('HEAD', hasQ="get_users")
+def get_users(self: SH, *args, **kwargs):
+	"""Send list of users"""
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+
+
+	return self.send_json(Sconfig.get_users(), cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ="update_user_perm")
+def update_user_perm(self: SH, *args, **kwargs):
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	query = self.query
+	username = query.get("username", [None])[0]
+	permission = query.get("perms", [None])[0]
+
+	try:
+		permission = int(permission)
+	except Exception:
+		permission = None
+
+	if not (username is not None and permission is not None):
+		return self.send_json({"status": "Failed", "message": "Username or permission not provided"}, cookie=cookie)
+
+	USER = Sconfig.user_handler.get_user(username, temp=True)
+	if not USER:
+		return self.send_json({"status": "Failed", "message": "User not found"}, cookie=cookie)
+
+	USER.set_permission_pack(permission)
+
+	self.log_warning(f'Updating permission of "{username}" to "{permission}" by {[USER.uid]}')
+
+	return self.send_json({"status": "Success", "message": "Permission updated"}, cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ="get_user_perm")
+def get_user_perm(self: SH, *args, **kwargs):
+	"""Send permission of a user"""
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	username = self.query.get("username", [None])[0]
+
+	if not username:
+		return self.send_json({"status": False, "message": "Username not provided"}, cookie=cookie)
+
+	USER = Sconfig.user_handler.get_user(username, temp=True)
+	if not USER:
+		return self.send_json({"status": False, "message": "User not found"}, cookie=cookie)
+
+	return self.send_json({"status": True, "permissions_code": USER.permission_pack}, cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ="add_user") # added by Admin
+def add_user(self: SH, *args, **kwargs):
+	"""Add a user"""
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	username = self.query.get("username", [None])[0]
+	password = self.query.get("password", [None])[0]
+
+	if not (username and password):
+		return self.send_json({"status": False, "message": "Username or password not provided"}, cookie=cookie)
+
+	if Sconfig.user_handler.get_user(username):
+		return self.send_json({"status": False, "message": "Username already exists"}, cookie=cookie)
+
+	new_user = Sconfig.user_handler.create_user(username, password)
+	if not new_user:
+		return self.send_json({"status": False, "message": "Failed to create user"}, cookie=cookie)
+
+	return self.send_json({"status": True, "message": f"<h2>User created.</h2> UID: {new_user.uid}"}, cookie=cookie)
+
+
+
+@SH.on_req('HEAD', hasQ="delete_user")
+def delete_user(self: SH, *args, **kwargs):
+	"""Delete a user"""
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	username = self.query.get("username", [None])[0]
+
+	if not username:
+		return self.send_json({"status": False, "message": "Username not provided"}, cookie=cookie)
+
+	USER = Sconfig.user_handler.get_user(username, temp=True)
+	if not USER:
+		return self.send_json({"status": False, "message": "User not found"}, cookie=cookie)
+
+	if USER.is_admin():
+		return self.send_json({"status": False, "message": "Cannot delete admin! Remove from admin 1st."}, cookie=cookie)
+
+	if not Sconfig.user_handler.delete_user(username): # delete user
+		return self.send_json({"status": False, "message": "Failed to delete user"}, cookie=cookie)
+
+	return self.send_json({"status": True, "message": "User deleted"}, cookie=cookie)
+
+
+
+@SH.on_req('HEAD', hasQ="update")
+def update(self: SH, *args, **kwargs):
+	"""Check for update and return the latest version"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
+
+	if not user.is_admin():
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+
+
+	data = fetch_url("https://raw.githack.com/RaSan147/pyrobox/main/VERSION")
+	if data:
+		data  = data.decode("utf-8").strip()
+		ret = json.dumps({"update_available": data > __version__, "latest_version": data})
+		return self.return_txt(ret, HTTPStatus.OK, cookie=cookie)
+	else:
+		return self.return_txt("Failed to fetch latest version", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ="size")
+def get_size(self: SH, *args, **kwargs):
+	"""Return size of the file"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+
+	url_path = kwargs.get('url_path', '')
+	os_path = self.translate_path(url_path)
+
+	stat = get_stat(os_path)
+	if not stat:
+		return self.send_json({"status": 0}, cookie=cookie)
+	if os.path.isfile(os_path):
+		size = stat.st_size
+	else:
+		size = get_dir_size(os_path)
+
+	humanbyte = humanbytes(size)
+	fmbyte = fmbytes(size)
+	return self.send_json({"status": 1,
+														"byte": size,
+														"humanbyte": humanbyte,
+														"fmbyte": fmbyte}, cookie=cookie)
+
+@SH.on_req('HEAD', hasQ="size_n_count")
+def get_size_n_count(self: SH, *args, **kwargs):
+	"""Return size of the file"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+
+	url_path = kwargs.get('url_path', '')
+	os_path = self.translate_path(url_path)
+
+	stat = get_stat(os_path)
+	if not stat:
+		return self.send_json({"status": 0}, cookie=cookie)
+	if os.path.isfile(os_path):
+		count, size = 1, stat.st_size
+	else:
+		count, size = get_tree_count_n_size(os_path)
+
+	humanbyte = humanbytes(size)
+	fmbyte = fmbytes(size)
+	return self.send_json({"status": 1,
+														"byte": size,
+														"humanbyte": humanbyte,
+														"fmbyte": fmbyte,
+														"count": count}, cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ=("zip_id", "czip"))
+def get_zip_id(self: SH, *args, **kwargs):
+	"""Return ZIP ID status"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.ZIP:
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+	
+	if not (user.DOWNLOAD and user.VIEW):
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	if CoreConfig.disabled_func["zip"]:
+		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
+	
+	
+	os_path = kwargs.get('path')
+	spathsplit = kwargs.get('spathsplit')
+	filename = spathsplit[-2] + ".zip"
+
+	zid = None
+	status = False
+	message = ''
+	
+	try:
+		zid = zip_manager.get_id(os_path)
+		status = True
+
+	except LimitExceed:
+		message = 'Directory size limit exceed'
+		
+	except Exception:
+		self.log_error(traceback.format_exc())
+		message = 'Failed to create zip'
+
+	return self.send_json({
+		"status": status,
+		"message": message,
+		"zid": zid,
+		"filename": filename
+	}, cookie=cookie)
+
+
+@SH.on_req('HEAD', hasQ="czip")
+def create_zip(self: SH, *args, **kwargs):
+	"""Create ZIP task and return ID
+
+	# TODO: Move to Dynamic island
+	"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.ZIP:
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+	
+	if not (user.DOWNLOAD and user.VIEW):
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	if CoreConfig.disabled_func["zip"]:
+		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
+
+	url_path = kwargs.get('url_path', '')
+	os_path = self.translate_path(url_path)
+
+	# if not dir or not exists
+	if not os.path.isdir(os_path):
+		return self.send_error(HTTPStatus.NOT_FOUND, "Directory not found", cookie=cookie)
+
+
+	# dir_size = get_dir_size(path, limit=6*1024*1024*1024)
+
+	# if dir_size == -1:
+	# 	msg = "Directory size is too large, please contact the host"
+	# 	return self.return_txt(HTTPStatus.OK, msg)
+
+	displaypath = self.get_displaypath(url_path)
+
+	title = "Creating ZIP"
+
+	data = pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
+											PY_PUBLIC_URL=CoreConfig.address(),
+											PY_DIR_TREE_NO_JS=dir_navigator(displaypath))
+	
+	return self.return_txt(data, cookie=cookie)
+
+
+
+@SH.on_req('HEAD', hasQ="zip")
+def get_zip(self: SH, *args, **kwargs):
+	"""Return ZIP file if available
+	Else return progress of the task"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	if not user.ZIP:
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+	
+	if not (user.DOWNLOAD and user.VIEW):
+		return self.send_error(HTTPStatus.UNAUTHORIZED, "You are not authorized to perform this action", cookie=cookie)
+
+	if CoreConfig.disabled_func["zip"]:
+		return self.return_txt("ERROR: ZIP FEATURE IS UNAVAILABLE !", HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
+
+
+
+	os_path = kwargs.get('path')
+	spathsplit = kwargs.get('spathsplit')
+
+	query = self.query
+	msg = False
+
+	def reply(status, msg=""):
+		return self.send_json({
+			"status": status,
+			"message": msg
+		}, cookie=cookie)
+
+	if not os.path.isdir(os_path):
+		msg = "Folder not found. Failed to create zip"
+		self.log_error(msg)
+		return reply("ERROR", msg)
+
+
+	filename = spathsplit[-2] + ".zip"
+
+	id = query["zid"][0]
+
+	# IF NOT STARTED
+	if zip_manager.calculating(id):
+		return reply("CALCULATING")
+
+	if not zip_manager.zip_id_status(id):
+		t = zip_manager.archive_thread(os_path, id)
+		t.start()
+
+		return reply("SUCCESS", "ARCHIVING")
+
+
+	if zip_manager.zip_id_status[id] == "DONE":
+		if query("download"):
+			zip_path = zip_manager.zip_ids[id]
+
+			return self.return_file(zip_path, filename, True, cookie=cookie)
+
+
+		if query("progress"):
+			return reply("DONE") #if query("progress") or no query
+
+	# IF IN PROGRESS
+	if zip_manager.zip_id_status[id] == "ARCHIVING":
+		progress = zip_manager.zip_in_progress[id]
+		# return self.return_txt("%.2f" % progress)
+		return reply("PROGRESS", "%.2f" % progress)
+
+	if zip_manager.zip_id_status[id].startswith("ERROR"):
+		# return self.return_txt(zip_manager.zip_id_status[id])
+		return reply("ERROR", zip_manager.zip_id_status[id])
+
+@SH.on_req('HEAD', hasQ="json")
+def send_ls_json(self: SH, *args, **kwargs):
+	"""Send directory listing in JSON format"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	return list_directory_json(self)
+
+
+
+
+@SH.on_req('HEAD', hasQ=("vid", "vid-data"))
+def send_video_data(self: SH, *args, **kwargs):
+	# SEND VIDEO DATA
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+
+
+	vid_source = url_path
+
+	content_type = self.guess_type(os_path)
+
+	if not content_type.startswith('video/'):
+		self.send_error(HTTPStatus.NOT_FOUND, "THIS IS NOT A VIDEO FILE", cookie=cookie)
+		return None
+
+
+	displaypath = self.get_displaypath(url_path)
+
+	title = get_titles(displaypath, file=True)
+
+
+	warning = ""
+
+	if content_type not in ['video/mp4', 'video/ogg', 'video/webm']:
+		warning = ('<h2>It seems HTML player may not be able to play this Video format, Try Downloading</h2>')
+
+	return self.send_json({
+		"status": "success",
+		"warning": warning,
+		"video": vid_source,
+		"title": displaypath.split("/")[-1],
+		"content_type": content_type,
+	}, cookie=cookie)
+
+
+
+@SH.on_req('HEAD', hasQ="vid")
+def send_video_page(self: SH, *args, **kwargs):
+	# SEND VIDEO PLAYER
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+	# vid_source = url_path
+	content_type = self.guess_type(os_path)
+
+	if not content_type.startswith('video/'):
+		self.send_error(HTTPStatus.NOT_FOUND, "THIS IS NOT A VIDEO FILE", cookie=cookie)
+		return None
+
+	r = []
+
+	displaypath = self.get_displaypath(url_path)
+
+
+
+	title = get_titles(displaypath, file=True)
+
+	r.append(pt.directory_explorer_header().safe_substitute(PY_PAGE_TITLE=title,
+													PY_PUBLIC_URL=CoreConfig.address(),
+													PY_DIR_TREE_NO_JS= dir_navigator(displaypath)))
+
+	encoded = '\n'.join(r).encode(enc, 'surrogateescape')
+	return self.return_txt(encoded, cookie=cookie)
+
+
+
+
+
+
+# @SH.on_req('HEAD', url_regex="/@assets/.*")
+# def send_assets(self: SH, *args, **kwargs):
+# 	"""Send assets"""
+# 	user = Authorize_user(self)
+
+# 	if not user: # guest or not will be handled in Authentication
+# 		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
+
+# 	if not CoreConfig.ASSETS:
+# 		self.send_error(HTTPStatus.NOT_FOUND, "Assets not available")
+# 		return None
+
+
+# 	path = kwargs.get('path')
+# 	spathsplit = kwargs.get('spathsplit')
+
+# 	path = CoreConfig.ASSETS_dir + "/".join(spathsplit[2:])
+# 	#	print("USING ASSETS", path)
+
+# 	if not os.path.isfile(path):
+# 		self.send_error(HTTPStatus.NOT_FOUND, "File not found")
+# 		return None
+
+# 	return self.return_file(path)
+
+@SH.on_req('HEAD', hasQ="style")
+def send_style(self: SH, *args, **kwargs):
+	"""Send style sheet"""
+	return self.send_css(pt.style_css())
+
+@SH.on_req('HEAD', hasQ="global_script")
+def send_global_script(self: SH, *args, **kwargs):
+	"""Send global script"""
+	return self.send_script(pt.global_script(), content_type="text/javascript")
+
+@SH.on_req('HEAD', hasQ="asset_script")
+def send_script(self: SH, *args, **kwargs):
+	"""Send script"""
+	return self.send_script(pt.assets_script())
+
+@SH.on_req('HEAD', hasQ="theme_script")
+def send_theme_script(self: SH, *args, **kwargs):
+	"""Send theme script"""
+	return self.send_script(pt.theme_script())
+
+@SH.on_req('HEAD', hasQ="page_handler_script")
+def send_page_handler_script(self: SH, *args, **kwargs):
+	"""Send page handler script"""
+	return self.send_script(pt.page_handler_script())
+
+@SH.on_req('HEAD', hasQ="video_page_script")
+def send_video_script(self: SH, *args, **kwargs):
+	"""Send video script"""
+	return self.send_script(pt.video_page_script())
+
+@SH.on_req('HEAD', hasQ="admin_page_script")
+def send_admin_script(self: SH, *args, **kwargs):
+	"""Send admin script"""
+	return self.send_script(pt.admin_page_script())
+
+@SH.on_req('HEAD', hasQ="file_list_script")
+def send_file_list_script(self: SH, *args, **kwargs):
+	"""Send file list script"""
+	return self.send_script(pt.file_list_script())
+
+@SH.on_req('HEAD', hasQ="error_page_script")
+def send_error_page_script(self: SH, *args, **kwargs):
+	"""Send error page script"""
+	return self.send_script(pt.error_page_script())
+
+@SH.on_req('HEAD', hasQ="zip_page_script")
+def send_zip_page_script(self: SH, *args, **kwargs):
+	"""Send zip page script"""
+	return self.send_script(pt.zip_page_script())
+
+
+
+@SH.on_req('HEAD', hasQ="login")
+def login_page(self: SH, *args, **kwargs):
+	"""Send login page"""
+	user, cookie = Authorize_user(self)
+
+	if user:
+		return self.redirect("/")
+
+	return self.send_text(pt.login_page())
+
+@SH.on_req('HEAD', hasQ="signup")
+def signup_page(self: SH, *args, **kwargs):
+	"""Send signup page"""
+	user, cookie = Authorize_user(self)
+
+	if user:
+		return self.redirect("/")
+
+	if Sconfig.cli_args.no_signup:
+		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Signup is disabled")
+
+	return self.send_text(pt.signup_page())
+
+
+
+
+
+
+
+
+
+@SH.on_req('HEAD', hasQ="folder_data")
+def get_folder_data(self: SH, *args, **kwargs):
+	"""Send folder data"""
+	user, cookie = Authorize_user(self)
+
+	if not user:
+		return self.send_json({
+			"status": 0,
+			"error_code": HTTPStatus.UNAUTHORIZED,
+			"error_message": "You must be logged in to access this data.",
+
+		}, cookie=cookie)
+
+	os_path = kwargs.get('path')
+
+	if not user.VIEW:
+		return self.send_json({
+			"status": 0,
+			"error_code": HTTPStatus.UNAUTHORIZED,
+			"error_message": "You don't have permission to view this folder",
+
+		}, cookie=cookie)
+
+
+	try:
+		if not os.path.isdir(os_path):
+			return self.send_json({"status": 0,
+						"warning": "Folder not found"}, cookie=cookie)
+
+	except Exception as e:
+		err = traceback.format_exc()
+		return self.send_json({
+			"status": 0,
+			"error_code": HTTPStatus.NOT_FOUND,
+			"error_message": str(e),
+
+		})
+
+	data = list_directory(self, os_path, user, cookie=cookie)
+
+	if data:
+		return self.send_json(data, cookie=cookie)
+
+
+@SH.on_req('HEAD')
+def default_get(self: SH, filename=None, *args, **kwargs):
+	"""Serve a GET request."""
+	user, cookie = Authorize_user(self)
+
+	#print("/"*50)
+	#print(user.permission)
+	#print("/"*50)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.redirect("?login")
+
+
+	os_path = kwargs.get('path')
+
+	if os.path.isdir(os_path):
+		parts = urllib.parse.urlsplit(self.path)
+		if not parts.path.endswith('/'):
+			# redirect browser - doing basically what apache does
+			self.send_response(HTTPStatus.MOVED_PERMANENTLY)
+			new_parts = (parts[0], parts[1], parts[2] + '/',
+							parts[3], parts[4])
+			new_url = urllib.parse.urlunsplit(new_parts)
+			self.send_header("Location", new_url)
+			self.send_header("Content-Length", "0")
+			self.end_headers()
+			return None
+		for index in "index.html", "index.htm":
+			index = os.path.join(os_path, index)
+			if os.path.exists(index):
+				os_path = index
+				break
+		else:
+			return list_directory_html(self, os_path, user, cookie=cookie)
+
+	# check for trailing "/" which should return 404. See Issue17324
+	# The test for this was added in test_httpserver.py
+	# However, some OS platforms accept a trailingSlash as a filename
+	# See discussion on python-dev and Issue34711 regarding
+	# parsing and rejection of filenames with a trailing slash
+
+	if os_path.endswith("/"):
+		self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie=cookie)
+		return None
+
+
+
+	# else:
+
+	if (not user.DOWNLOAD) or user.NOPERMISSION:
+		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Download is disabled", cookie=cookie)
+
+	if not os.path.exists(os_path):
+		return self.send_error(HTTPStatus.NOT_FOUND, "File not found", cookie=cookie)
+	return self.return_file(os_path, filename, cookie=cookie)
+
+
+
+
+
+
+
+
+
+
+
+
+# TODO check against user_mgmt
+def AUTHORIZE_POST(req: SH, post:DPD, post_type=''):
+	"""Check if the user is authorized to post"""
+
+	# START
+	post.start()
+	form = post.form
+
+	verify_1 = form.get_multi_field(verify_name='post-type', verify_msg=post_type, decode=T)
+
+	return verify_1[1]
+
+
+@SH.on_req('POST', hasQ="do_login")
+def handle_login_post(self: SH, *args, **kwargs):
+	"""Handle login post"""
+	user, cookie = Authorize_user(self)
+
+	if user:
+		return self.redirect("/")
+
+
+
+	post = DPD(self)
+
+	AUTHORIZE_POST(self, post, 'login')
+
+	form = post.form
+
+	username = form.get_multi_field(verify_name='username', decode=T)[1]
+
+	# GET PASSWORD
+	password = form.get_multi_field(verify_name='password', decode=T)[1]
+
+	user = Sconfig.user_handler.get_user(username)
+	if not user:
+		return self.send_json({"status": "failed", "message": "User not found"}, cookie=cookie)
+
+	if not user.check_password(password):
+		return self.send_json({"status": "failed", "message": "Incorrect password"}, cookie=cookie)
+
+	cookie = add_user_cookie(user)
+
+	return self.send_json({"status": "success", "message": "Login successful, if not Auto-redirecting, kindly Refresh"}, cookie=cookie)
+
+
+@SH.on_req('POST', hasQ="do_signup")
+def handle_signup_post(self: SH, *args, **kwargs):
+	"""Handle signup post"""
+	user, cookie = Authorize_user(self)
+
+	if user:
+		return self.redirect("/")
+
+	if Sconfig.cli_args.no_signup:
+		return self.send_error(HTTPStatus.SERVICE_UNAVAILABLE, "Signup is disabled")
+
+
+	post = DPD(self)
+
+	AUTHORIZE_POST(self, post, 'signup')
+
+	form = post.form
+
+	username = form.get_multi_field(verify_name='username', decode=T)[1]
+
+	# GET PASSWORD
+	password = form.get_multi_field(verify_name='password', decode=T)[1]
+
+	user = Sconfig.user_handler.get_user(username)
+	if user:
+		return self.send_json({"status": "failed", "message": "Username is already in use!"}, cookie=cookie)
+
+	user = Sconfig.user_handler.create_user(username, password)
+	if not user:
+		return self.send_json({"status": "failed", "message": "Failed to create user"}, cookie=cookie)
+
+	cookie = add_user_cookie(user)
+
+	return self.send_json({"status": "success", "message": "Signup successful"}, cookie=cookie)
+
+
+
+
+# TODO check against user_mgmt
+@SH.on_req('POST', hasQ="upload")
+def upload(self: SH, *args, **kwargs):
+	"""GET Uploaded files"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	if user.NOPERMISSION or (not user.UPLOAD):
+		return self.send_txt("Upload not allowed", HTTPStatus.SERVICE_UNAVAILABLE, cookie=cookie)
+
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+
+	post = DPD(self)
+
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'upload')
+
+	form = post.form
+
+	if not uid:
+		return None
+
+
+	# uploaded_files = [] # Uploaded folder list
+
+	upload_handler = UploadHandler(uid)
+
+	upload_thread = threading.Thread(target=upload_handler.start, args=(self,))
+	upload_thread.start()
+
+	def remove_from_temp(temp_fn):
+		try:
+			upload_handler.kill()
+		except OSError:
+			pass
+
+		finally:
+			if temp_fn in CoreConfig.temp_file:
+				CoreConfig.temp_file.remove(temp_fn)
+
+
+
+	# PASSWORD SYSTEM
+	password = form.get_multi_field(verify_name='password', decode=T)[1]
+
+	self.log_debug(f'post password: {[password]} by client')
+
+	if (user.MEMBER and not user.check_password(password)) or (not user.MEMBER and password != CoreConfig.PASSWORD): # readline returns password with \r\n at end
+		self.log_info(f"Incorrect password by {uid}")
+
+		return self.send_txt("Incorrect password", HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+	while post.remainbytes > 0:
+		fn = form.get_file_name() # reads the next line and returns the file name
+		if not fn:
+			return self.send_error(HTTPStatus.BAD_REQUEST, "Can't find out file name...", cookie=cookie)
+
+
+		rltv_path = posixpath.join(url_path, fn)
+		
+		if not self.path_safety_check(fn, rltv_path):
+			return self.send_txt("Invalid Path:  " + rltv_path, HTTPStatus.BAD_REQUEST, cookie=cookie)
+
+		temp_fn = os.path.join(os_path, ".LStemp-"+fn +'.tmp')
+		CoreConfig.temp_file.add(temp_fn)
+
+
+		os_f_path = os.path.join(os_path, fn)
+
+
+
+		line = post.get() # content type
+		line = post.get() # line gap
+
+
+
+		# ORIGINAL FILE STARTS FROM HERE
+		try:
+			out = open(temp_fn, 'wb')
+			preline = post.get()
+			while post.remainbytes > 0 and not upload_handler.error:
+				line = post.get()
+				if post.boundary in line:
+					preline = preline[0:-1]
+					if preline.endswith(b'\r'):
+						preline = preline[0:-1]
+
+					upload_handler.upload(out, 'w', preline)
+					# out.write(preline)
+					# uploaded_files.append(rltv_path,)
+					break
+				else:
+					upload_handler.upload(out, 'w', preline)
+					# out.write(preline)
+					preline = line
+
+			upload_handler.upload(out, 's', (os_f_path, user.MODIFY))
+
+			if upload_handler.error and not upload_handler.active:
+				remove_from_temp(temp_fn)
+				return self.send_error(HTTPStatus.INTERNAL_SERVER_ERROR, upload_handler.error, cookie=cookie)
+
+
+
+		except (IOError, OSError):
+			traceback.print_exc()
+			return self.send_txt("Can't create file to write, do you have permission to write?", HTTPStatus.SERVICE_UNAVAILABLE, cookie=cookie)
+
+
+	upload_handler.active = False # will take no further inputs
+	upload_thread.join()
+
+	if upload_handler.error:
+		return self.send_error(upload_handler.error, HTTPStatus.INTERNAL_SERVER_ERROR, cookie=cookie)
+
+
+
+	return self.return_txt("File(s) uploaded", cookie=cookie)
+
+
+
+
+
+@SH.on_req('POST', hasQ="del-f")
+def del_2_recycle(self: SH, *args, **kwargs):
+	"""Move 2 recycle bin"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	if user.NOPERMISSION or (not user.DELETE):
+		return self.send_json({"head": "Failed", "body": "You have no permission to delete."}, cookie=cookie)
+
+	url_path = kwargs.get('url_path')
+
+
+	post = DPD(self)
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'del-f')
+	form = post.form
+
+	if CoreConfig.disabled_func["send2trash"]:
+		return self.send_json({"head": "Failed", "body": "Recycling unavailable! Try deleting permanently..."}, cookie=cookie)
+
+
+
+	# File link to move to recycle bin
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
+
+	rel_path = self.get_rel_path(filename)
+	
+	if not self.path_safety_check(filename, rel_path):
+		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
+	
+	os_f_path = self.translate_path(posixpath.join(url_path, filename))
+
+	self.log_warning(f'<-send2trash-> {os_f_path} by {[uid]}')
+
+	head = "Failed"
+	try:
+		if CoreConfig.OS == 'Android':
+			raise InterruptedError
+		send2trash(os_f_path)
+		msg = "Successfully Moved To Recycle bin"+ post.refresh
+		head = "Success"
+	except TrashPermissionError:
+		msg = "Recycling unavailable! Try deleting permanently..."
+	except InterruptedError:
+		msg = "Recycling unavailable! Try deleting permanently..."
+	except Exception as e:
+		traceback.print_exc()
+		msg = "<b>" + rel_path + "</b> " + e.__class__.__name__
+
+	return self.send_json({"head": head, "body": msg}, cookie=cookie)
+
+
+
+
+
+@SH.on_req('POST', hasQ="del-p")
+def del_permanently(self: SH, *args, **kwargs):
+	"""DELETE files permanently"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	if user.NOPERMISSION or (not user.DELETE):
+		return self.send_json({"head": "Failed", "body": "Recycling unavailable! Try deleting permanently..."}, cookie=cookie)
+
+	url_path = kwargs.get('url_path')
+
+
+	post = DPD(self)
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'del-p')
+	form = post.form
+
+
+
+	# File link to move to recycle bin
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
+
+	rel_path = self.get_rel_path(filename)
+
+	if not self.path_safety_check(filename, rel_path):
+		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
+
+	os_f_path = self.translate_path(posixpath.join(url_path, filename))
+
+	self.log_warning(f'Perm. DELETED {os_f_path} by {[uid]}')
+
+
+	try:
+		if os.path.isfile(os_f_path): os.remove(os_f_path)
+		else: shutil.rmtree(os_f_path, ignore_errors=True)
+
+		return self.send_json({"head": "Success", "body": "PERMANENTLY DELETED  " + rel_path + post.refresh}, cookie=cookie)
+
+
+	except Exception as e:
+		traceback.print_exc()
+		return self.send_json({"head": "Failed", "body": "<b>" + rel_path + "<b>" + e.__class__.__name__}, cookie=cookie)
+
+
+
+
+
+@SH.on_req('POST', hasQ="rename")
+def rename_content(self: SH, *args, **kwargs):
+	"""Rename files"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	if user.NOPERMISSION or (not user.MODIFY):
+		return self.send_json({"head": "Failed", "body": "Renaming is disabled."}, cookie=cookie)
+
+
+	url_path = kwargs.get('url_path')
+
+
+	post = DPD(self)
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'rename')
+	form = post.form
+
+
+
+	# File link to move to recycle bin
+	
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
+	new_name = form.get_multi_field(verify_name='data', decode=T)[1].strip()
+
+	rel_path = self.get_rel_path(filename)
+	new_rel_path = self.get_rel_path(new_name)
+
+	if not self.path_safety_check(filename, new_name, rel_path, new_rel_path):
+		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
+
+	os_f_path = self.translate_path(posixpath.join(url_path, filename))
+	os_new_f_path = self.translate_path(posixpath.join(url_path, new_name))
+
+	self.log_warning(f'Renamed "{os_f_path}" to "{os_new_f_path}" by {[uid]}')
+
+
+	try:
+		os.rename(os_f_path, os_new_f_path)
+		return self.send_json({"head": "Renamed Successfully", "body":  post.refresh}, cookie=cookie)
+	except Exception as e:
+		return self.send_json({"head": "Failed", "body": "<b>" + rel_path + "</b><br><b>" + e.__class__.__name__ + "</b> : " + self.get_web_path(str(e), -1) }, cookie=cookie)
+
+
+
+
+
+@SH.on_req('POST', hasQ="info")
+def get_info(self: SH, *args, **kwargs):
+	"""Get files permanently"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED, cookie=cookie)
+
+
+	if user.NOPERMISSION:
+		return self.send_json({"head": "Failed", "body": "You have no permission to view."}, cookie=cookie)
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+	script = None
+
+
+	post = DPD(self)
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'info')
+	form = post.form
+
+
+	# File link to move to check info
+
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
+
+	rel_path = self.get_rel_path(filename)
+
+	if not self.path_safety_check(filename, rel_path):
+		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
+
+	os_f_path = self.translate_path(posixpath.join(url_path, filename))
+
+
+	self.log_warning(f'Info Checked "{os_f_path}" by: {[uid]}')
+
+	if not os.path.exists(os_f_path):
+		return self.send_json({"head":"Failed", "body":"File/Folder Not Found"}, cookie=cookie)
+
+	file_stat = get_stat(os_f_path)
+	if not file_stat:
+		return self.send_json({"head":"Failed", "body":"Permission Denied"}, cookie=cookie)
+
+	data = []
+	data.append(["Name", urllib.parse.unquote(filename, errors= 'surrogatepass')])
+
+	if os.path.isfile(os_f_path):
+		data.append(["Type","File"])
+		if "." in filename:
+			data.append(["Extension", filename.rpartition(".")[2]])
+
+		size = file_stat.st_size
+		data.append(["Size", humanbytes(size) + " (%i bytes)"%size])
+
+	else: #if os.path.isdir(xpath):
+		data.append(["Type", "Folder"])
+		# size = get_dir_size(xpath)
+
+		data.append(["Total Files", '<span id="f_count">Please Wait</span>'])
+
+
+		data.append(["Total Size", '<span id="f_size">Please Wait</span>'])
+		script = '''
+		tools.fetch_json(tools.full_path("''' + rel_path + '''?size_n_count")).then(resp => {
+		// console.log(resp);
+		if (resp.status) {
+			size = resp.humanbyte;
+			count = resp.count;
+			document.getElementById("f_size").innerHTML = resp.humanbyte + " (" + resp.byte + " bytes)";
+			document.getElementById("f_count").innerHTML = count;
+		} else {
+			throw new Error(resp.msg);
+		}}).catch(err => {
+		console.log(err);
+		document.getElementById("f_size").innerHTML = "Error";
+		});
+		'''
+
+	data.append(["Path", rel_path])
+
+	def get_dt(time):
+		return datetime.datetime.fromtimestamp(time)
+
+	data.append(["Created on", get_dt(file_stat.st_ctime)])
+	data.append(["Last Modified", get_dt(file_stat.st_mtime)])
+	data.append(["Last Accessed", get_dt(file_stat.st_atime)])
+
+	body = """
+<style>
+table {
+	font-family: arial, sans-serif;
+	border-collapse: collapse;
+	width: 100%;
+}
+
+td, th {
+	border: 1px solid #00BFFF;
+	text-align: left;
+	padding: 8px;
+}
+
+tr:nth-child(even) {
+	background-color: #111;
+}
+</style>
+
+<table>
+<tr>
+<th>About</th>
+<th>Info</th>
+</tr>
+"""
+	for key, val in data:
+		body += "<tr><td>{key}</td><td>{val}</td></tr>".format(key=key, val=val)
+	body += "</table>"
+
+	return self.send_json({"head":"Properties", "body":body, "script":script}, cookie=cookie)
+
+
+@SH.on_req('POST', hasQ="new_folder")
+def new_folder(self: SH, *args, **kwargs):
+	"""Create new folder"""
+	user, cookie = Authorize_user(self)
+
+	if not user: # guest or not will be handled in Authentication
+		return self.send_text(pt.login_page(), HTTPStatus.UNAUTHORIZED)
+
+	if user.NOPERMISSION or (not user.MODIFY):
+		return self.send_json({"head": "Failed", "body": "Permission denied."}, cookie=cookie)
+
+
+	os_path = kwargs.get('path')
+	url_path = kwargs.get('url_path')
+
+	post = DPD(self)
+
+	# AUTHORIZE
+	uid = AUTHORIZE_POST(self, post, 'new_folder')
+	form = post.form
+
+	filename = form.get_multi_field(verify_name='name', decode=T)[1].strip()
+
+	rel_path = self.get_rel_path(filename)
+
+	if not self.path_safety_check(filename, rel_path):
+		return self.send_json({"head": "Failed", "body": "Invalid Path:  " + rel_path}, cookie=cookie)
+
+	os_f_path = self.translate_path(posixpath.join(url_path, filename))
+
+
+	self.log_warning(f'New Folder Created "{os_f_path}" by: {[uid]}')
+
+	try:
+		if os.path.exists(os_f_path):
+			return self.send_json({"head": "Failed", "body": "Folder Already Exists:  " + rel_path}, cookie=cookie)
+		if os.path.isfile(os_f_path):
+			return self.send_json({"head": "Failed", "body": "File Already Exists:  " + rel_path}, cookie=cookie)
+		os.makedirs(os_f_path)
+		return self.send_json({"head": "Success", "body": "New Folder Created:  " + rel_path +post.refresh}, cookie=cookie)
+
+	except Exception as e:
+		self.log_error(traceback.format_exc())
+		return self.send_json({"head": "Failed", "body": f"<b>{ rel_path }</b><br><b>{ e.__class__.__name__ }</b>"}, cookie=cookie)
+
+
+
+
+
+@SH.on_req('POST')
+def default_post(self: SH, *args, **kwargs):
+	raise PostError("Bad Request")
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+# proxy for old versions
+def run(*args, **kwargs):
+	run_server(handler=SH, *args, **kwargs)
+
+if __name__ == '__main__':
+	run(port = 45454)
```

### Comparing `pyrobox-0.9.4/src/tabulate.py` & `pyrobox-0.9.5/src/tabulate.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,2787 +1,2787 @@
-"""Pretty-print tabular data."""
-
-import warnings
-from collections import namedtuple
-from collections.abc import Iterable, Sized
-from html import escape as htmlescape
-from itertools import chain, zip_longest as izip_longest
-from functools import reduce, partial
-import io
-import re
-import math
-import textwrap
-import dataclasses
-
-try:
-    import wcwidth  # optional wide-character (CJK) support
-except ImportError:
-    wcwidth = None
-
-
-def _is_file(f):
-    return isinstance(f, io.IOBase)
-
-
-__all__ = ["tabulate", "tabulate_formats", "simple_separated_format"]
-try:
-    from .version import version as __version__  # noqa: F401
-except ImportError:
-    pass  # running __init__.py as a script, AppVeyor pytests
-
-
-# minimum extra space in headers
-MIN_PADDING = 2
-
-# Whether or not to preserve leading/trailing whitespace in data.
-PRESERVE_WHITESPACE = False
-
-_DEFAULT_FLOATFMT = "g"
-_DEFAULT_INTFMT = ""
-_DEFAULT_MISSINGVAL = ""
-# default align will be overwritten by "left", "center" or "decimal"
-# depending on the formatter
-_DEFAULT_ALIGN = "default"
-
-
-# if True, enable wide-character (CJK) support
-WIDE_CHARS_MODE = wcwidth is not None
-
-# Constant that can be used as part of passed rows to generate a separating line
-# It is purposely an unprintable character, very unlikely to be used in a table
-SEPARATING_LINE = "\001"
-
-Line = namedtuple("Line", ["begin", "hline", "sep", "end"])
-
-
-DataRow = namedtuple("DataRow", ["begin", "sep", "end"])
-
-
-# A table structure is supposed to be:
-#
-#     --- lineabove ---------
-#         headerrow
-#     --- linebelowheader ---
-#         datarow
-#     --- linebetweenrows ---
-#     ... (more datarows) ...
-#     --- linebetweenrows ---
-#         last datarow
-#     --- linebelow ---------
-#
-# TableFormat's line* elements can be
-#
-#   - either None, if the element is not used,
-#   - or a Line tuple,
-#   - or a function: [col_widths], [col_alignments] -> string.
-#
-# TableFormat's *row elements can be
-#
-#   - either None, if the element is not used,
-#   - or a DataRow tuple,
-#   - or a function: [cell_values], [col_widths], [col_alignments] -> string.
-#
-# padding (an integer) is the amount of white space around data values.
-#
-# with_header_hide:
-#
-#   - either None, to display all table elements unconditionally,
-#   - or a list of elements not to be displayed if the table has column headers.
-#
-TableFormat = namedtuple(
-    "TableFormat",
-    [
-        "lineabove",
-        "linebelowheader",
-        "linebetweenrows",
-        "linebelow",
-        "headerrow",
-        "datarow",
-        "padding",
-        "with_header_hide",
-    ],
-)
-
-
-def _is_separating_line(row):
-    row_type = type(row)
-    is_sl = (row_type == list or row_type == str) and (
-        (len(row) >= 1 and row[0] == SEPARATING_LINE)
-        or (len(row) >= 2 and row[1] == SEPARATING_LINE)
-    )
-    return is_sl
-
-
-def _pipe_segment_with_colons(align, colwidth):
-    """Return a segment of a horizontal line with optional colons which
-    indicate column's alignment (as in `pipe` output format)."""
-    w = colwidth
-    if align in ["right", "decimal"]:
-        return ("-" * (w - 1)) + ":"
-    elif align == "center":
-        return ":" + ("-" * (w - 2)) + ":"
-    elif align == "left":
-        return ":" + ("-" * (w - 1))
-    else:
-        return "-" * w
-
-
-def _pipe_line_with_colons(colwidths, colaligns):
-    """Return a horizontal line with optional colons to indicate column's
-    alignment (as in `pipe` output format)."""
-    if not colaligns:  # e.g. printing an empty data frame (github issue #15)
-        colaligns = [""] * len(colwidths)
-    segments = [_pipe_segment_with_colons(a, w) for a, w in zip(colaligns, colwidths)]
-    return "|" + "|".join(segments) + "|"
-
-
-def _mediawiki_row_with_attrs(separator, cell_values, colwidths, colaligns):
-    alignment = {
-        "left": "",
-        "right": 'style="text-align: right;"| ',
-        "center": 'style="text-align: center;"| ',
-        "decimal": 'style="text-align: right;"| ',
-    }
-    # hard-coded padding _around_ align attribute and value together
-    # rather than padding parameter which affects only the value
-    values_with_attrs = [
-        " " + alignment.get(a, "") + c + " " for c, a in zip(cell_values, colaligns)
-    ]
-    colsep = separator * 2
-    return (separator + colsep.join(values_with_attrs)).rstrip()
-
-
-def _textile_row_with_attrs(cell_values, colwidths, colaligns):
-    cell_values[0] += " "
-    alignment = {"left": "<.", "right": ">.", "center": "=.", "decimal": ">."}
-    values = (alignment.get(a, "") + v for a, v in zip(colaligns, cell_values))
-    return "|" + "|".join(values) + "|"
-
-
-def _html_begin_table_without_header(colwidths_ignore, colaligns_ignore):
-    # this table header will be suppressed if there is a header row
-    return "<table>\n<tbody>"
-
-
-def _html_row_with_attrs(celltag, unsafe, cell_values, colwidths, colaligns):
-    alignment = {
-        "left": "",
-        "right": ' style="text-align: right;"',
-        "center": ' style="text-align: center;"',
-        "decimal": ' style="text-align: right;"',
-    }
-    if unsafe:
-        values_with_attrs = [
-            "<{0}{1}>{2}</{0}>".format(celltag, alignment.get(a, ""), c)
-            for c, a in zip(cell_values, colaligns)
-        ]
-    else:
-        values_with_attrs = [
-            "<{0}{1}>{2}</{0}>".format(celltag, alignment.get(a, ""), htmlescape(c))
-            for c, a in zip(cell_values, colaligns)
-        ]
-    rowhtml = "<tr>{}</tr>".format("".join(values_with_attrs).rstrip())
-    if celltag == "th":  # it's a header row, create a new table header
-        rowhtml = f"<table>\n<thead>\n{rowhtml}\n</thead>\n<tbody>"
-    return rowhtml
-
-
-def _moin_row_with_attrs(celltag, cell_values, colwidths, colaligns, header=""):
-    alignment = {
-        "left": "",
-        "right": '<style="text-align: right;">',
-        "center": '<style="text-align: center;">',
-        "decimal": '<style="text-align: right;">',
-    }
-    values_with_attrs = [
-        "{}{} {} ".format(celltag, alignment.get(a, ""), header + c + header)
-        for c, a in zip(cell_values, colaligns)
-    ]
-    return "".join(values_with_attrs) + "||"
-
-
-def _latex_line_begin_tabular(colwidths, colaligns, booktabs=False, longtable=False):
-    alignment = {"left": "l", "right": "r", "center": "c", "decimal": "r"}
-    tabular_columns_fmt = "".join([alignment.get(a, "l") for a in colaligns])
-    return "\n".join(
-        [
-            ("\\begin{tabular}{" if not longtable else "\\begin{longtable}{")
-            + tabular_columns_fmt
-            + "}",
-            "\\toprule" if booktabs else "\\hline",
-        ]
-    )
-
-
-def _asciidoc_row(is_header, *args):
-    """handle header and data rows for asciidoc format"""
-
-    def make_header_line(is_header, colwidths, colaligns):
-        # generate the column specifiers
-
-        alignment = {"left": "<", "right": ">", "center": "^", "decimal": ">"}
-        # use the column widths generated by tabulate for the asciidoc column width specifiers
-        asciidoc_alignments = zip(
-            colwidths, [alignment[colalign] for colalign in colaligns]
-        )
-        asciidoc_column_specifiers = [
-            "{:d}{}".format(width, align) for width, align in asciidoc_alignments
-        ]
-        header_list = ['cols="' + (",".join(asciidoc_column_specifiers)) + '"']
-
-        # generate the list of options (currently only "header")
-        options_list = []
-
-        if is_header:
-            options_list.append("header")
-
-        if options_list:
-            header_list += ['options="' + ",".join(options_list) + '"']
-
-        # generate the list of entries in the table header field
-
-        return "[{}]\n|====".format(",".join(header_list))
-
-    if len(args) == 2:
-        # two arguments are passed if called in the context of aboveline
-        # print the table header with column widths and optional header tag
-        return make_header_line(False, *args)
-
-    elif len(args) == 3:
-        # three arguments are passed if called in the context of dataline or headerline
-        # print the table line and make the aboveline if it is a header
-
-        cell_values, colwidths, colaligns = args
-        data_line = "|" + "|".join(cell_values)
-
-        if is_header:
-            return make_header_line(True, colwidths, colaligns) + "\n" + data_line
-        else:
-            return data_line
-
-    else:
-        raise ValueError(
-            " _asciidoc_row() requires two (colwidths, colaligns) "
-            + "or three (cell_values, colwidths, colaligns) arguments) "
-        )
-
-
-LATEX_ESCAPE_RULES = {
-    r"&": r"\&",
-    r"%": r"\%",
-    r"$": r"\$",
-    r"#": r"\#",
-    r"_": r"\_",
-    r"^": r"\^{}",
-    r"{": r"\{",
-    r"}": r"\}",
-    r"~": r"\textasciitilde{}",
-    "\\": r"\textbackslash{}",
-    r"<": r"\ensuremath{<}",
-    r">": r"\ensuremath{>}",
-}
-
-
-def _latex_row(cell_values, colwidths, colaligns, escrules=LATEX_ESCAPE_RULES):
-    def escape_char(c):
-        return escrules.get(c, c)
-
-    escaped_values = ["".join(map(escape_char, cell)) for cell in cell_values]
-    rowfmt = DataRow("", "&", "\\\\")
-    return _build_simple_row(escaped_values, rowfmt)
-
-
-def _rst_escape_first_column(rows, headers):
-    def escape_empty(val):
-        if isinstance(val, (str, bytes)) and not val.strip():
-            return ".."
-        else:
-            return val
-
-    new_headers = list(headers)
-    new_rows = []
-    if headers:
-        new_headers[0] = escape_empty(headers[0])
-    for row in rows:
-        new_row = list(row)
-        if new_row:
-            new_row[0] = escape_empty(row[0])
-        new_rows.append(new_row)
-    return new_rows, new_headers
-
-
-_table_formats = {
-    "simple": TableFormat(
-        lineabove=Line("", "-", "  ", ""),
-        linebelowheader=Line("", "-", "  ", ""),
-        linebetweenrows=None,
-        linebelow=Line("", "-", "  ", ""),
-        headerrow=DataRow("", "  ", ""),
-        datarow=DataRow("", "  ", ""),
-        padding=0,
-        with_header_hide=["lineabove", "linebelow"],
-    ),
-    "plain": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("", "  ", ""),
-        datarow=DataRow("", "  ", ""),
-        padding=0,
-        with_header_hide=None,
-    ),
-    "grid": TableFormat(
-        lineabove=Line("+", "-", "+", "+"),
-        linebelowheader=Line("+", "=", "+", "+"),
-        linebetweenrows=Line("+", "-", "+", "+"),
-        linebelow=Line("+", "-", "+", "+"),
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "simple_grid": TableFormat(
-        lineabove=Line("┌", "─", "┬", "┐"),
-        linebelowheader=Line("├", "─", "┼", "┤"),
-        linebetweenrows=Line("├", "─", "┼", "┤"),
-        linebelow=Line("└", "─", "┴", "┘"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "rounded_grid": TableFormat(
-        lineabove=Line("╭", "─", "┬", "╮"),
-        linebelowheader=Line("├", "─", "┼", "┤"),
-        linebetweenrows=Line("├", "─", "┼", "┤"),
-        linebelow=Line("╰", "─", "┴", "╯"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "heavy_grid": TableFormat(
-        lineabove=Line("┏", "━", "┳", "┓"),
-        linebelowheader=Line("┣", "━", "╋", "┫"),
-        linebetweenrows=Line("┣", "━", "╋", "┫"),
-        linebelow=Line("┗", "━", "┻", "┛"),
-        headerrow=DataRow("┃", "┃", "┃"),
-        datarow=DataRow("┃", "┃", "┃"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "mixed_grid": TableFormat(
-        lineabove=Line("┍", "━", "┯", "┑"),
-        linebelowheader=Line("┝", "━", "┿", "┥"),
-        linebetweenrows=Line("├", "─", "┼", "┤"),
-        linebelow=Line("┕", "━", "┷", "┙"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "double_grid": TableFormat(
-        lineabove=Line("╔", "═", "╦", "╗"),
-        linebelowheader=Line("╠", "═", "╬", "╣"),
-        linebetweenrows=Line("╠", "═", "╬", "╣"),
-        linebelow=Line("╚", "═", "╩", "╝"),
-        headerrow=DataRow("║", "║", "║"),
-        datarow=DataRow("║", "║", "║"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "fancy_grid": TableFormat(
-        lineabove=Line("╒", "═", "╤", "╕"),
-        linebelowheader=Line("╞", "═", "╪", "╡"),
-        linebetweenrows=Line("├", "─", "┼", "┤"),
-        linebelow=Line("╘", "═", "╧", "╛"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "outline": TableFormat(
-        lineabove=Line("+", "-", "+", "+"),
-        linebelowheader=Line("+", "=", "+", "+"),
-        linebetweenrows=None,
-        linebelow=Line("+", "-", "+", "+"),
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "simple_outline": TableFormat(
-        lineabove=Line("┌", "─", "┬", "┐"),
-        linebelowheader=Line("├", "─", "┼", "┤"),
-        linebetweenrows=None,
-        linebelow=Line("└", "─", "┴", "┘"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "rounded_outline": TableFormat(
-        lineabove=Line("╭", "─", "┬", "╮"),
-        linebelowheader=Line("├", "─", "┼", "┤"),
-        linebetweenrows=None,
-        linebelow=Line("╰", "─", "┴", "╯"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "heavy_outline": TableFormat(
-        lineabove=Line("┏", "━", "┳", "┓"),
-        linebelowheader=Line("┣", "━", "╋", "┫"),
-        linebetweenrows=None,
-        linebelow=Line("┗", "━", "┻", "┛"),
-        headerrow=DataRow("┃", "┃", "┃"),
-        datarow=DataRow("┃", "┃", "┃"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "mixed_outline": TableFormat(
-        lineabove=Line("┍", "━", "┯", "┑"),
-        linebelowheader=Line("┝", "━", "┿", "┥"),
-        linebetweenrows=None,
-        linebelow=Line("┕", "━", "┷", "┙"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "double_outline": TableFormat(
-        lineabove=Line("╔", "═", "╦", "╗"),
-        linebelowheader=Line("╠", "═", "╬", "╣"),
-        linebetweenrows=None,
-        linebelow=Line("╚", "═", "╩", "╝"),
-        headerrow=DataRow("║", "║", "║"),
-        datarow=DataRow("║", "║", "║"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "fancy_outline": TableFormat(
-        lineabove=Line("╒", "═", "╤", "╕"),
-        linebelowheader=Line("╞", "═", "╪", "╡"),
-        linebetweenrows=None,
-        linebelow=Line("╘", "═", "╧", "╛"),
-        headerrow=DataRow("│", "│", "│"),
-        datarow=DataRow("│", "│", "│"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "github": TableFormat(
-        lineabove=Line("|", "-", "|", "|"),
-        linebelowheader=Line("|", "-", "|", "|"),
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=["lineabove"],
-    ),
-    "pipe": TableFormat(
-        lineabove=_pipe_line_with_colons,
-        linebelowheader=_pipe_line_with_colons,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=["lineabove"],
-    ),
-    "orgtbl": TableFormat(
-        lineabove=None,
-        linebelowheader=Line("|", "-", "+", "|"),
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "jira": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("||", "||", "||"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "presto": TableFormat(
-        lineabove=None,
-        linebelowheader=Line("", "-", "+", ""),
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("", "|", ""),
-        datarow=DataRow("", "|", ""),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "pretty": TableFormat(
-        lineabove=Line("+", "-", "+", "+"),
-        linebelowheader=Line("+", "-", "+", "+"),
-        linebetweenrows=None,
-        linebelow=Line("+", "-", "+", "+"),
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "psql": TableFormat(
-        lineabove=Line("+", "-", "+", "+"),
-        linebelowheader=Line("|", "-", "+", "|"),
-        linebetweenrows=None,
-        linebelow=Line("+", "-", "+", "+"),
-        headerrow=DataRow("|", "|", "|"),
-        datarow=DataRow("|", "|", "|"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "rst": TableFormat(
-        lineabove=Line("", "=", "  ", ""),
-        linebelowheader=Line("", "=", "  ", ""),
-        linebetweenrows=None,
-        linebelow=Line("", "=", "  ", ""),
-        headerrow=DataRow("", "  ", ""),
-        datarow=DataRow("", "  ", ""),
-        padding=0,
-        with_header_hide=None,
-    ),
-    "mediawiki": TableFormat(
-        lineabove=Line(
-            '{| class="wikitable" style="text-align: left;"',
-            "",
-            "",
-            "\n|+ <!-- caption -->\n|-",
-        ),
-        linebelowheader=Line("|-", "", "", ""),
-        linebetweenrows=Line("|-", "", "", ""),
-        linebelow=Line("|}", "", "", ""),
-        headerrow=partial(_mediawiki_row_with_attrs, "!"),
-        datarow=partial(_mediawiki_row_with_attrs, "|"),
-        padding=0,
-        with_header_hide=None,
-    ),
-    "moinmoin": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=partial(_moin_row_with_attrs, "||", header="'''"),
-        datarow=partial(_moin_row_with_attrs, "||"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "youtrack": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("|| ", " || ", " || "),
-        datarow=DataRow("| ", " | ", " |"),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "html": TableFormat(
-        lineabove=_html_begin_table_without_header,
-        linebelowheader="",
-        linebetweenrows=None,
-        linebelow=Line("</tbody>\n</table>", "", "", ""),
-        headerrow=partial(_html_row_with_attrs, "th", False),
-        datarow=partial(_html_row_with_attrs, "td", False),
-        padding=0,
-        with_header_hide=["lineabove"],
-    ),
-    "unsafehtml": TableFormat(
-        lineabove=_html_begin_table_without_header,
-        linebelowheader="",
-        linebetweenrows=None,
-        linebelow=Line("</tbody>\n</table>", "", "", ""),
-        headerrow=partial(_html_row_with_attrs, "th", True),
-        datarow=partial(_html_row_with_attrs, "td", True),
-        padding=0,
-        with_header_hide=["lineabove"],
-    ),
-    "latex": TableFormat(
-        lineabove=_latex_line_begin_tabular,
-        linebelowheader=Line("\\hline", "", "", ""),
-        linebetweenrows=None,
-        linebelow=Line("\\hline\n\\end{tabular}", "", "", ""),
-        headerrow=_latex_row,
-        datarow=_latex_row,
-        padding=1,
-        with_header_hide=None,
-    ),
-    "latex_raw": TableFormat(
-        lineabove=_latex_line_begin_tabular,
-        linebelowheader=Line("\\hline", "", "", ""),
-        linebetweenrows=None,
-        linebelow=Line("\\hline\n\\end{tabular}", "", "", ""),
-        headerrow=partial(_latex_row, escrules={}),
-        datarow=partial(_latex_row, escrules={}),
-        padding=1,
-        with_header_hide=None,
-    ),
-    "latex_booktabs": TableFormat(
-        lineabove=partial(_latex_line_begin_tabular, booktabs=True),
-        linebelowheader=Line("\\midrule", "", "", ""),
-        linebetweenrows=None,
-        linebelow=Line("\\bottomrule\n\\end{tabular}", "", "", ""),
-        headerrow=_latex_row,
-        datarow=_latex_row,
-        padding=1,
-        with_header_hide=None,
-    ),
-    "latex_longtable": TableFormat(
-        lineabove=partial(_latex_line_begin_tabular, longtable=True),
-        linebelowheader=Line("\\hline\n\\endhead", "", "", ""),
-        linebetweenrows=None,
-        linebelow=Line("\\hline\n\\end{longtable}", "", "", ""),
-        headerrow=_latex_row,
-        datarow=_latex_row,
-        padding=1,
-        with_header_hide=None,
-    ),
-    "tsv": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("", "\t", ""),
-        datarow=DataRow("", "\t", ""),
-        padding=0,
-        with_header_hide=None,
-    ),
-    "textile": TableFormat(
-        lineabove=None,
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=None,
-        headerrow=DataRow("|_. ", "|_.", "|"),
-        datarow=_textile_row_with_attrs,
-        padding=1,
-        with_header_hide=None,
-    ),
-    "asciidoc": TableFormat(
-        lineabove=partial(_asciidoc_row, False),
-        linebelowheader=None,
-        linebetweenrows=None,
-        linebelow=Line("|====", "", "", ""),
-        headerrow=partial(_asciidoc_row, True),
-        datarow=partial(_asciidoc_row, False),
-        padding=1,
-        with_header_hide=["lineabove"],
-    ),
-}
-
-
-tabulate_formats = list(sorted(_table_formats.keys()))
-
-# The table formats for which multiline cells will be folded into subsequent
-# table rows. The key is the original format specified at the API. The value is
-# the format that will be used to represent the original format.
-multiline_formats = {
-    "plain": "plain",
-    "simple": "simple",
-    "grid": "grid",
-    "simple_grid": "simple_grid",
-    "rounded_grid": "rounded_grid",
-    "heavy_grid": "heavy_grid",
-    "mixed_grid": "mixed_grid",
-    "double_grid": "double_grid",
-    "fancy_grid": "fancy_grid",
-    "pipe": "pipe",
-    "orgtbl": "orgtbl",
-    "jira": "jira",
-    "presto": "presto",
-    "pretty": "pretty",
-    "psql": "psql",
-    "rst": "rst",
-    "outline": "outline",
-    "simple_outline": "simple_outline",
-    "rounded_outline": "rounded_outline",
-    "heavy_outline": "heavy_outline",
-    "mixed_outline": "mixed_outline",
-    "double_outline": "double_outline",
-    "fancy_outline": "fancy_outline",
-}
-
-# TODO: Add multiline support for the remaining table formats:
-#       - mediawiki: Replace \n with <br>
-#       - moinmoin: TBD
-#       - youtrack: TBD
-#       - html: Replace \n with <br>
-#       - latex*: Use "makecell" package: In header, replace X\nY with
-#         \thead{X\\Y} and in data row, replace X\nY with \makecell{X\\Y}
-#       - tsv: TBD
-#       - textile: Replace \n with <br/> (must be well-formed XML)
-
-_multiline_codes = re.compile(r"\r|\n|\r\n")
-_multiline_codes_bytes = re.compile(b"\r|\n|\r\n")
-
-# Handle ANSI escape sequences for both control sequence introducer (CSI) and
-# operating system command (OSC). Both of these begin with 0x1b (or octal 033),
-# which will be shown below as ESC.
-#
-# CSI ANSI escape codes have the following format, defined in section 5.4 of ECMA-48:
-#
-# CSI: ESC followed by the '[' character (0x5b)
-# Parameter Bytes: 0..n bytes in the range 0x30-0x3f
-# Intermediate Bytes: 0..n bytes in the range 0x20-0x2f
-# Final Byte: a single byte in the range 0x40-0x7e
-#
-# Also include the terminal hyperlink sequences as described here:
-# https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
-#
-# OSC 8 ; params ; uri ST display_text OSC 8 ;; ST
-#
-# Example: \x1b]8;;https://example.com\x5ctext to show\x1b]8;;\x5c
-#
-# Where:
-# OSC: ESC followed by the ']' character (0x5d)
-# params: 0..n optional key value pairs separated by ':' (e.g. foo=bar:baz=qux:abc=123)
-# URI: the actual URI with protocol scheme (e.g. https://, file://, ftp://)
-# ST: ESC followed by the '\' character (0x5c)
-_esc = r"\x1b"
-_csi = rf"{_esc}\["
-_osc = rf"{_esc}\]"
-_st = rf"{_esc}\\"
-
-_ansi_escape_pat = rf"""
-    (
-        # terminal colors, etc
-        {_csi}        # CSI
-        [\x30-\x3f]*  # parameter bytes
-        [\x20-\x2f]*  # intermediate bytes
-        [\x40-\x7e]   # final byte
-    |
-        # terminal hyperlinks
-        {_osc}8;        # OSC opening
-        (\w+=\w+:?)*    # key=value params list (submatch 2)
-        ;               # delimiter
-        ([^{_esc}]+)    # URI - anything but ESC (submatch 3)
-        {_st}           # ST
-        ([^{_esc}]+)    # link text - anything but ESC (submatch 4)
-        {_osc}8;;{_st}  # "closing" OSC sequence
-    )
-"""
-_ansi_codes = re.compile(_ansi_escape_pat, re.VERBOSE)
-_ansi_codes_bytes = re.compile(_ansi_escape_pat.encode("utf8"), re.VERBOSE)
-_ansi_color_reset_code = "\033[0m"
-
-_float_with_thousands_separators = re.compile(
-    r"^(([+-]?[0-9]{1,3})(?:,([0-9]{3}))*)?(?(1)\.[0-9]*|\.[0-9]+)?$"
-)
-
-
-def simple_separated_format(separator):
-    """Construct a simple TableFormat with columns separated by a separator.
-
-    >>> tsv = simple_separated_format("\\t") ; \
-        tabulate([["foo", 1], ["spam", 23]], tablefmt=tsv) == 'foo \\t 1\\nspam\\t23'
-    True
-
-    """
-    return TableFormat(
-        None,
-        None,
-        None,
-        None,
-        headerrow=DataRow("", separator, ""),
-        datarow=DataRow("", separator, ""),
-        padding=0,
-        with_header_hide=None,
-    )
-
-
-def _isnumber_with_thousands_separator(string):
-    """
-    >>> _isnumber_with_thousands_separator(".")
-    False
-    >>> _isnumber_with_thousands_separator("1")
-    True
-    >>> _isnumber_with_thousands_separator("1.")
-    True
-    >>> _isnumber_with_thousands_separator(".1")
-    True
-    >>> _isnumber_with_thousands_separator("1000")
-    False
-    >>> _isnumber_with_thousands_separator("1,000")
-    True
-    >>> _isnumber_with_thousands_separator("1,0000")
-    False
-    >>> _isnumber_with_thousands_separator("1,000.1234")
-    True
-    >>> _isnumber_with_thousands_separator(b"1,000.1234")
-    True
-    >>> _isnumber_with_thousands_separator("+1,000.1234")
-    True
-    >>> _isnumber_with_thousands_separator("-1,000.1234")
-    True
-    """
-    try:
-        string = string.decode()
-    except (UnicodeDecodeError, AttributeError):
-        pass
-
-    return bool(re.match(_float_with_thousands_separators, string))
-
-
-def _isconvertible(conv, string):
-    try:
-        conv(string)
-        return True
-    except (ValueError, TypeError):
-        return False
-
-
-def _isnumber(string):
-    """
-    >>> _isnumber("123.45")
-    True
-    >>> _isnumber("123")
-    True
-    >>> _isnumber("spam")
-    False
-    >>> _isnumber("123e45678")
-    False
-    >>> _isnumber("inf")
-    True
-    """
-    if not _isconvertible(float, string):
-        return False
-    elif isinstance(string, (str, bytes)) and (
-        math.isinf(float(string)) or math.isnan(float(string))
-    ):
-        return string.lower() in ["inf", "-inf", "nan"]
-    return True
-
-
-def _isint(string, inttype=int):
-    """
-    >>> _isint("123")
-    True
-    >>> _isint("123.45")
-    False
-    """
-    return (
-        type(string) is inttype
-        or (
-            (hasattr(string, "is_integer") or hasattr(string, "__array__"))
-            and str(type(string)).startswith("<class 'numpy.int")
-        )  # numpy.int64 and similar
-        or (
-            isinstance(string, (bytes, str)) and _isconvertible(inttype, string)
-        )  # integer as string
-    )
-
-
-def _isbool(string):
-    """
-    >>> _isbool(True)
-    True
-    >>> _isbool("False")
-    True
-    >>> _isbool(1)
-    False
-    """
-    return type(string) is bool or (
-        isinstance(string, (bytes, str)) and string in ("True", "False")
-    )
-
-
-def _type(string, has_invisible=True, numparse=True):
-    """The least generic type (type(None), int, float, str, unicode).
-
-    >>> _type(None) is type(None)
-    True
-    >>> _type("foo") is type("")
-    True
-    >>> _type("1") is type(1)
-    True
-    >>> _type('\x1b[31m42\x1b[0m') is type(42)
-    True
-    >>> _type('\x1b[31m42\x1b[0m') is type(42)
-    True
-
-    """
-
-    if has_invisible and isinstance(string, (str, bytes)):
-        string = _strip_ansi(string)
-
-    if string is None:
-        return type(None)
-    elif hasattr(string, "isoformat"):  # datetime.datetime, date, and time
-        return str
-    elif _isbool(string):
-        return bool
-    elif _isint(string) and numparse:
-        return int
-    elif _isnumber(string) and numparse:
-        return float
-    elif isinstance(string, bytes):
-        return bytes
-    else:
-        return str
-
-
-def _afterpoint(string):
-    """Symbols after a decimal point, -1 if the string lacks the decimal point.
-
-    >>> _afterpoint("123.45")
-    2
-    >>> _afterpoint("1001")
-    -1
-    >>> _afterpoint("eggs")
-    -1
-    >>> _afterpoint("123e45")
-    2
-    >>> _afterpoint("123,456.78")
-    2
-
-    """
-    if _isnumber(string) or _isnumber_with_thousands_separator(string):
-        if _isint(string):
-            return -1
-        else:
-            pos = string.rfind(".")
-            pos = string.lower().rfind("e") if pos < 0 else pos
-            if pos >= 0:
-                return len(string) - pos - 1
-            else:
-                return -1  # no point
-    else:
-        return -1  # not a number
-
-
-def _padleft(width, s):
-    """Flush right.
-
-    >>> _padleft(6, '\u044f\u0439\u0446\u0430') == '  \u044f\u0439\u0446\u0430'
-    True
-
-    """
-    fmt = "{0:>%ds}" % width
-    return fmt.format(s)
-
-
-def _padright(width, s):
-    """Flush left.
-
-    >>> _padright(6, '\u044f\u0439\u0446\u0430') == '\u044f\u0439\u0446\u0430  '
-    True
-
-    """
-    fmt = "{0:<%ds}" % width
-    return fmt.format(s)
-
-
-def _padboth(width, s):
-    """Center string.
-
-    >>> _padboth(6, '\u044f\u0439\u0446\u0430') == ' \u044f\u0439\u0446\u0430 '
-    True
-
-    """
-    fmt = "{0:^%ds}" % width
-    return fmt.format(s)
-
-
-def _padnone(ignore_width, s):
-    return s
-
-
-def _strip_ansi(s):
-    r"""Remove ANSI escape sequences, both CSI (color codes, etc) and OSC hyperlinks.
-
-    CSI sequences are simply removed from the output, while OSC hyperlinks are replaced
-    with the link text. Note: it may be desirable to show the URI instead but this is not
-    supported.
-
-    >>> repr(_strip_ansi('\x1B]8;;https://example.com\x1B\\This is a link\x1B]8;;\x1B\\'))
-    "'This is a link'"
-
-    >>> repr(_strip_ansi('\x1b[31mred\x1b[0m text'))
-    "'red text'"
-
-    """
-    if isinstance(s, str):
-        return _ansi_codes.sub(r"\4", s)
-    else:  # a bytestring
-        return _ansi_codes_bytes.sub(r"\4", s)
-
-
-def _visible_width(s):
-    """Visible width of a printed string. ANSI color codes are removed.
-
-    >>> _visible_width('\x1b[31mhello\x1b[0m'), _visible_width("world")
-    (5, 5)
-
-    """
-    # optional wide-character support
-    if wcwidth is not None and WIDE_CHARS_MODE:
-        len_fn = wcwidth.wcswidth
-    else:
-        len_fn = len
-    if isinstance(s, (str, bytes)):
-        return len_fn(_strip_ansi(s))
-    else:
-        return len_fn(str(s))
-
-
-def _is_multiline(s):
-    if isinstance(s, str):
-        return bool(re.search(_multiline_codes, s))
-    else:  # a bytestring
-        return bool(re.search(_multiline_codes_bytes, s))
-
-
-def _multiline_width(multiline_s, line_width_fn=len):
-    """Visible width of a potentially multiline content."""
-    return max(map(line_width_fn, re.split("[\r\n]", multiline_s)))
-
-
-def _choose_width_fn(has_invisible, enable_widechars, is_multiline):
-    """Return a function to calculate visible cell width."""
-    if has_invisible:
-        line_width_fn = _visible_width
-    elif enable_widechars:  # optional wide-character support if available
-        line_width_fn = wcwidth.wcswidth
-    else:
-        line_width_fn = len
-    if is_multiline:
-        width_fn = lambda s: _multiline_width(s, line_width_fn)  # noqa
-    else:
-        width_fn = line_width_fn
-    return width_fn
-
-
-def _align_column_choose_padfn(strings, alignment, has_invisible):
-    if alignment == "right":
-        if not PRESERVE_WHITESPACE:
-            strings = [s.strip() for s in strings]
-        padfn = _padleft
-    elif alignment == "center":
-        if not PRESERVE_WHITESPACE:
-            strings = [s.strip() for s in strings]
-        padfn = _padboth
-    elif alignment == "decimal":
-        if has_invisible:
-            decimals = [_afterpoint(_strip_ansi(s)) for s in strings]
-        else:
-            decimals = [_afterpoint(s) for s in strings]
-        maxdecimals = max(decimals)
-        strings = [s + (maxdecimals - decs) * " " for s, decs in zip(strings, decimals)]
-        padfn = _padleft
-    elif not alignment:
-        padfn = _padnone
-    else:
-        if not PRESERVE_WHITESPACE:
-            strings = [s.strip() for s in strings]
-        padfn = _padright
-    return strings, padfn
-
-
-def _align_column_choose_width_fn(has_invisible, enable_widechars, is_multiline):
-    if has_invisible:
-        line_width_fn = _visible_width
-    elif enable_widechars:  # optional wide-character support if available
-        line_width_fn = wcwidth.wcswidth
-    else:
-        line_width_fn = len
-    if is_multiline:
-        width_fn = lambda s: _align_column_multiline_width(s, line_width_fn)  # noqa
-    else:
-        width_fn = line_width_fn
-    return width_fn
-
-
-def _align_column_multiline_width(multiline_s, line_width_fn=len):
-    """Visible width of a potentially multiline content."""
-    return list(map(line_width_fn, re.split("[\r\n]", multiline_s)))
-
-
-def _flat_list(nested_list):
-    ret = []
-    for item in nested_list:
-        if isinstance(item, list):
-            for subitem in item:
-                ret.append(subitem)
-        else:
-            ret.append(item)
-    return ret
-
-
-def _align_column(
-    strings,
-    alignment,
-    minwidth=0,
-    has_invisible=True,
-    enable_widechars=False,
-    is_multiline=False,
-):
-    """[string] -> [padded_string]"""
-    strings, padfn = _align_column_choose_padfn(strings, alignment, has_invisible)
-    width_fn = _align_column_choose_width_fn(
-        has_invisible, enable_widechars, is_multiline
-    )
-
-    s_widths = list(map(width_fn, strings))
-    maxwidth = max(max(_flat_list(s_widths)), minwidth)
-    # TODO: refactor column alignment in single-line and multiline modes
-    if is_multiline:
-        if not enable_widechars and not has_invisible:
-            padded_strings = [
-                "\n".join([padfn(maxwidth, s) for s in ms.splitlines()])
-                for ms in strings
-            ]
-        else:
-            # enable wide-character width corrections
-            s_lens = [[len(s) for s in re.split("[\r\n]", ms)] for ms in strings]
-            visible_widths = [
-                [maxwidth - (w - l) for w, l in zip(mw, ml)]
-                for mw, ml in zip(s_widths, s_lens)
-            ]
-            # wcswidth and _visible_width don't count invisible characters;
-            # padfn doesn't need to apply another correction
-            padded_strings = [
-                "\n".join([padfn(w, s) for s, w in zip((ms.splitlines() or ms), mw)])
-                for ms, mw in zip(strings, visible_widths)
-            ]
-    else:  # single-line cell values
-        if not enable_widechars and not has_invisible:
-            padded_strings = [padfn(maxwidth, s) for s in strings]
-        else:
-            # enable wide-character width corrections
-            s_lens = list(map(len, strings))
-            visible_widths = [maxwidth - (w - l) for w, l in zip(s_widths, s_lens)]
-            # wcswidth and _visible_width don't count invisible characters;
-            # padfn doesn't need to apply another correction
-            padded_strings = [padfn(w, s) for s, w in zip(strings, visible_widths)]
-    return padded_strings
-
-
-def _more_generic(type1, type2):
-    types = {
-        type(None): 0,
-        bool: 1,
-        int: 2,
-        float: 3,
-        bytes: 4,
-        str: 5,
-    }
-    invtypes = {
-        5: str,
-        4: bytes,
-        3: float,
-        2: int,
-        1: bool,
-        0: type(None),
-    }
-    moregeneric = max(types.get(type1, 5), types.get(type2, 5))
-    return invtypes[moregeneric]
-
-
-def _column_type(strings, has_invisible=True, numparse=True):
-    """The least generic type all column values are convertible to.
-
-    >>> _column_type([True, False]) is bool
-    True
-    >>> _column_type(["1", "2"]) is int
-    True
-    >>> _column_type(["1", "2.3"]) is float
-    True
-    >>> _column_type(["1", "2.3", "four"]) is str
-    True
-    >>> _column_type(["four", '\u043f\u044f\u0442\u044c']) is str
-    True
-    >>> _column_type([None, "brux"]) is str
-    True
-    >>> _column_type([1, 2, None]) is int
-    True
-    >>> import datetime as dt
-    >>> _column_type([dt.datetime(1991,2,19), dt.time(17,35)]) is str
-    True
-
-    """
-    types = [_type(s, has_invisible, numparse) for s in strings]
-    return reduce(_more_generic, types, bool)
-
-
-def _format(val, valtype, floatfmt, intfmt, missingval="", has_invisible=True):
-    """Format a value according to its type.
-
-    Unicode is supported:
-
-    >>> hrow = ['\u0431\u0443\u043a\u0432\u0430', '\u0446\u0438\u0444\u0440\u0430'] ; \
-        tbl = [['\u0430\u0437', 2], ['\u0431\u0443\u043a\u0438', 4]] ; \
-        good_result = '\\u0431\\u0443\\u043a\\u0432\\u0430      \\u0446\\u0438\\u0444\\u0440\\u0430\\n-------  -------\\n\\u0430\\u0437             2\\n\\u0431\\u0443\\u043a\\u0438           4' ; \
-        tabulate(tbl, headers=hrow) == good_result
-    True
-
-    """  # noqa
-    if val is None:
-        return missingval
-
-    if valtype is str:
-        return f"{val}"
-    elif valtype is int:
-        return format(val, intfmt)
-    elif valtype is bytes:
-        try:
-            return str(val, "ascii")
-        except (TypeError, UnicodeDecodeError):
-            return str(val)
-    elif valtype is float:
-        is_a_colored_number = has_invisible and isinstance(val, (str, bytes))
-        if is_a_colored_number:
-            raw_val = _strip_ansi(val)
-            formatted_val = format(float(raw_val), floatfmt)
-            return val.replace(raw_val, formatted_val)
-        else:
-            return format(float(val), floatfmt)
-    else:
-        return f"{val}"
-
-
-def _align_header(
-    header, alignment, width, visible_width, is_multiline=False, width_fn=None
-):
-    "Pad string header to width chars given known visible_width of the header."
-    if is_multiline:
-        header_lines = re.split(_multiline_codes, header)
-        padded_lines = [
-            _align_header(h, alignment, width, width_fn(h)) for h in header_lines
-        ]
-        return "\n".join(padded_lines)
-    # else: not multiline
-    ninvisible = len(header) - visible_width
-    width += ninvisible
-    if alignment == "left":
-        return _padright(width, header)
-    elif alignment == "center":
-        return _padboth(width, header)
-    elif not alignment:
-        return f"{header}"
-    else:
-        return _padleft(width, header)
-
-
-def _remove_separating_lines(rows):
-    if type(rows) == list:
-        separating_lines = []
-        sans_rows = []
-        for index, row in enumerate(rows):
-            if _is_separating_line(row):
-                separating_lines.append(index)
-            else:
-                sans_rows.append(row)
-        return sans_rows, separating_lines
-    else:
-        return rows, None
-
-
-def _reinsert_separating_lines(rows, separating_lines):
-    if separating_lines:
-        for index in separating_lines:
-            rows.insert(index, SEPARATING_LINE)
-
-
-def _prepend_row_index(rows, index):
-    """Add a left-most index column."""
-    if index is None or index is False:
-        return rows
-    if isinstance(index, Sized) and len(index) != len(rows):
-        raise ValueError(
-            "index must be as long as the number of data rows: "
-            + "len(index)={} len(rows)={}".format(len(index), len(rows))
-        )
-    sans_rows, separating_lines = _remove_separating_lines(rows)
-    new_rows = []
-    index_iter = iter(index)
-    for row in sans_rows:
-        index_v = next(index_iter)
-        new_rows.append([index_v] + list(row))
-    rows = new_rows
-    _reinsert_separating_lines(rows, separating_lines)
-    return rows
-
-
-def _bool(val):
-    "A wrapper around standard bool() which doesn't throw on NumPy arrays"
-    try:
-        return bool(val)
-    except ValueError:  # val is likely to be a numpy array with many elements
-        return False
-
-
-def _normalize_tabular_data(tabular_data, headers, showindex="default"):
-    """Transform a supported data type to a list of lists, and a list of headers, with headers padding.
-
-    Supported tabular data types:
-
-    * list-of-lists or another iterable of iterables
-
-    * list of named tuples (usually used with headers="keys")
-
-    * list of dicts (usually used with headers="keys")
-
-    * list of OrderedDicts (usually used with headers="keys")
-
-    * list of dataclasses (Python 3.7+ only, usually used with headers="keys")
-
-    * 2D NumPy arrays
-
-    * NumPy record arrays (usually used with headers="keys")
-
-    * dict of iterables (usually used with headers="keys")
-
-    * pandas.DataFrame (usually used with headers="keys")
-
-    The first row can be used as headers if headers="firstrow",
-    column indices can be used as headers if headers="keys".
-
-    If showindex="default", show row indices of the pandas.DataFrame.
-    If showindex="always", show row indices for all types of data.
-    If showindex="never", don't show row indices for all types of data.
-    If showindex is an iterable, show its values as row indices.
-
-    """
-
-    try:
-        bool(headers)
-        is_headers2bool_broken = False  # noqa
-    except ValueError:  # numpy.ndarray, pandas.core.index.Index, ...
-        is_headers2bool_broken = True  # noqa
-        headers = list(headers)
-
-    index = None
-    if hasattr(tabular_data, "keys") and hasattr(tabular_data, "values"):
-        # dict-like and pandas.DataFrame?
-        if hasattr(tabular_data.values, "__call__"):
-            # likely a conventional dict
-            keys = tabular_data.keys()
-            rows = list(
-                izip_longest(*tabular_data.values())
-            )  # columns have to be transposed
-        elif hasattr(tabular_data, "index"):
-            # values is a property, has .index => it's likely a pandas.DataFrame (pandas 0.11.0)
-            keys = list(tabular_data)
-            if (
-                showindex in ["default", "always", True]
-                and tabular_data.index.name is not None
-            ):
-                if isinstance(tabular_data.index.name, list):
-                    keys[:0] = tabular_data.index.name
-                else:
-                    keys[:0] = [tabular_data.index.name]
-            vals = tabular_data.values  # values matrix doesn't need to be transposed
-            # for DataFrames add an index per default
-            index = list(tabular_data.index)
-            rows = [list(row) for row in vals]
-        else:
-            raise ValueError("tabular data doesn't appear to be a dict or a DataFrame")
-
-        if headers == "keys":
-            headers = list(map(str, keys))  # headers should be strings
-
-    else:  # it's a usual iterable of iterables, or a NumPy array, or an iterable of dataclasses
-        rows = list(tabular_data)
-
-        if headers == "keys" and not rows:
-            # an empty table (issue #81)
-            headers = []
-        elif (
-            headers == "keys"
-            and hasattr(tabular_data, "dtype")
-            and getattr(tabular_data.dtype, "names")
-        ):
-            # numpy record array
-            headers = tabular_data.dtype.names
-        elif (
-            headers == "keys"
-            and len(rows) > 0
-            and isinstance(rows[0], tuple)
-            and hasattr(rows[0], "_fields")
-        ):
-            # namedtuple
-            headers = list(map(str, rows[0]._fields))
-        elif len(rows) > 0 and hasattr(rows[0], "keys") and hasattr(rows[0], "values"):
-            # dict-like object
-            uniq_keys = set()  # implements hashed lookup
-            keys = []  # storage for set
-            if headers == "firstrow":
-                firstdict = rows[0] if len(rows) > 0 else {}
-                keys.extend(firstdict.keys())
-                uniq_keys.update(keys)
-                rows = rows[1:]
-            for row in rows:
-                for k in row.keys():
-                    # Save unique items in input order
-                    if k not in uniq_keys:
-                        keys.append(k)
-                        uniq_keys.add(k)
-            if headers == "keys":
-                headers = keys
-            elif isinstance(headers, dict):
-                # a dict of headers for a list of dicts
-                headers = [headers.get(k, k) for k in keys]
-                headers = list(map(str, headers))
-            elif headers == "firstrow":
-                if len(rows) > 0:
-                    headers = [firstdict.get(k, k) for k in keys]
-                    headers = list(map(str, headers))
-                else:
-                    headers = []
-            elif headers:
-                raise ValueError(
-                    "headers for a list of dicts is not a dict or a keyword"
-                )
-            rows = [[row.get(k) for k in keys] for row in rows]
-
-        elif (
-            headers == "keys"
-            and hasattr(tabular_data, "description")
-            and hasattr(tabular_data, "fetchone")
-            and hasattr(tabular_data, "rowcount")
-        ):
-            # Python Database API cursor object (PEP 0249)
-            # print tabulate(cursor, headers='keys')
-            headers = [column[0] for column in tabular_data.description]
-
-        elif (
-            dataclasses is not None
-            and len(rows) > 0
-            and dataclasses.is_dataclass(rows[0])
-        ):
-            # Python 3.7+'s dataclass
-            field_names = [field.name for field in dataclasses.fields(rows[0])]
-            if headers == "keys":
-                headers = field_names
-            rows = [[getattr(row, f) for f in field_names] for row in rows]
-
-        elif headers == "keys" and len(rows) > 0:
-            # keys are column indices
-            headers = list(map(str, range(len(rows[0]))))
-
-    # take headers from the first row if necessary
-    if headers == "firstrow" and len(rows) > 0:
-        if index is not None:
-            headers = [index[0]] + list(rows[0])
-            index = index[1:]
-        else:
-            headers = rows[0]
-        headers = list(map(str, headers))  # headers should be strings
-        rows = rows[1:]
-    elif headers == "firstrow":
-        headers = []
-
-    headers = list(map(str, headers))
-    #    rows = list(map(list, rows))
-    rows = list(map(lambda r: r if _is_separating_line(r) else list(r), rows))
-
-    # add or remove an index column
-    showindex_is_a_str = type(showindex) in [str, bytes]
-    if showindex == "default" and index is not None:
-        rows = _prepend_row_index(rows, index)
-    elif isinstance(showindex, Sized) and not showindex_is_a_str:
-        rows = _prepend_row_index(rows, list(showindex))
-    elif isinstance(showindex, Iterable) and not showindex_is_a_str:
-        rows = _prepend_row_index(rows, showindex)
-    elif showindex == "always" or (_bool(showindex) and not showindex_is_a_str):
-        if index is None:
-            index = list(range(len(rows)))
-        rows = _prepend_row_index(rows, index)
-    elif showindex == "never" or (not _bool(showindex) and not showindex_is_a_str):
-        pass
-
-    # pad with empty headers for initial columns if necessary
-    headers_pad = 0
-    if headers and len(rows) > 0:
-        headers_pad = max(0, len(rows[0]) - len(headers))
-        headers = [""] * headers_pad + headers
-
-    return rows, headers, headers_pad
-
-
-def _wrap_text_to_colwidths(list_of_lists, colwidths, numparses=True):
-    if len(list_of_lists):
-        num_cols = len(list_of_lists[0])
-    else:
-        num_cols = 0
-    numparses = _expand_iterable(numparses, num_cols, True)
-
-    result = []
-
-    for row in list_of_lists:
-        new_row = []
-        for cell, width, numparse in zip(row, colwidths, numparses):
-            if _isnumber(cell) and numparse:
-                new_row.append(cell)
-                continue
-
-            if width is not None:
-                wrapper = _CustomTextWrap(width=width)
-                # Cast based on our internal type handling
-                # Any future custom formatting of types (such as datetimes)
-                # may need to be more explicit than just `str` of the object
-                casted_cell = (
-                    str(cell) if _isnumber(cell) else _type(cell, numparse)(cell)
-                )
-                wrapped = [
-                    "\n".join(wrapper.wrap(line))
-                    for line in casted_cell.splitlines()
-                    if line.strip() != ""
-                ]
-                new_row.append("\n".join(wrapped))
-            else:
-                new_row.append(cell)
-        result.append(new_row)
-
-    return result
-
-
-def _to_str(s, encoding="utf8", errors="ignore"):
-    """
-    A type safe wrapper for converting a bytestring to str. This is essentially just
-    a wrapper around .decode() intended for use with things like map(), but with some
-    specific behavior:
-
-    1. if the given parameter is not a bytestring, it is returned unmodified
-    2. decode() is called for the given parameter and assumes utf8 encoding, but the
-       default error behavior is changed from 'strict' to 'ignore'
-
-    >>> repr(_to_str(b'foo'))
-    "'foo'"
-
-    >>> repr(_to_str('foo'))
-    "'foo'"
-
-    >>> repr(_to_str(42))
-    "'42'"
-
-    """
-    if isinstance(s, bytes):
-        return s.decode(encoding=encoding, errors=errors)
-    return str(s)
-
-
-def tabulate(
-    tabular_data,
-    headers=(),
-    tablefmt="simple",
-    floatfmt=_DEFAULT_FLOATFMT,
-    intfmt=_DEFAULT_INTFMT,
-    numalign=_DEFAULT_ALIGN,
-    stralign=_DEFAULT_ALIGN,
-    missingval=_DEFAULT_MISSINGVAL,
-    showindex="default",
-    disable_numparse=False,
-    colglobalalign=None,
-    colalign=None,
-    maxcolwidths=None,
-    headersglobalalign=None,
-    headersalign=None,
-    rowalign=None,
-    maxheadercolwidths=None,
-):
-    """Format a fixed width table for pretty printing.
-
-    >>> print(tabulate([[1, 2.34], [-56, "8.999"], ["2", "10001"]]))
-    ---  ---------
-      1      2.34
-    -56      8.999
-      2  10001
-    ---  ---------
-
-    The first required argument (`tabular_data`) can be a
-    list-of-lists (or another iterable of iterables), a list of named
-    tuples, a dictionary of iterables, an iterable of dictionaries,
-    an iterable of dataclasses (Python 3.7+), a two-dimensional NumPy array,
-    NumPy record array, or a Pandas' dataframe.
-
-
-    Table headers
-    -------------
-
-    To print nice column headers, supply the second argument (`headers`):
-
-      - `headers` can be an explicit list of column headers
-      - if `headers="firstrow"`, then the first row of data is used
-      - if `headers="keys"`, then dictionary keys or column indices are used
-
-    Otherwise a headerless table is produced.
-
-    If the number of headers is less than the number of columns, they
-    are supposed to be names of the last columns. This is consistent
-    with the plain-text format of R and Pandas' dataframes.
-
-    >>> print(tabulate([["sex","age"],["Alice","F",24],["Bob","M",19]],
-    ...       headers="firstrow"))
-           sex      age
-    -----  -----  -----
-    Alice  F         24
-    Bob    M         19
-
-    By default, pandas.DataFrame data have an additional column called
-    row index. To add a similar column to all other types of data,
-    use `showindex="always"` or `showindex=True`. To suppress row indices
-    for all types of data, pass `showindex="never" or `showindex=False`.
-    To add a custom row index column, pass `showindex=some_iterable`.
-
-    >>> print(tabulate([["F",24],["M",19]], showindex="always"))
-    -  -  --
-    0  F  24
-    1  M  19
-    -  -  --
-
-
-    Column and Headers alignment
-    ----------------------------
-
-    `tabulate` tries to detect column types automatically, and aligns
-    the values properly. By default it aligns decimal points of the
-    numbers (or flushes integer numbers to the right), and flushes
-    everything else to the left. Possible column alignments
-    (`numalign`, `stralign`) are: "right", "center", "left", "decimal"
-    (only for `numalign`), and None (to disable alignment).
-
-    `colglobalalign` allows for global alignment of columns, before any
-        specific override from `colalign`. Possible values are: None
-        (defaults according to coltype), "right", "center", "decimal",
-        "left".
-    `colalign` allows for column-wise override starting from left-most
-        column. Possible values are: "global" (no override), "right",
-        "center", "decimal", "left".
-    `headersglobalalign` allows for global headers alignment, before any
-        specific override from `headersalign`. Possible values are: None
-        (follow columns alignment), "right", "center", "left".
-    `headersalign` allows for header-wise override starting from left-most
-        given header. Possible values are: "global" (no override), "same"
-        (follow column alignment), "right", "center", "left".
-
-    Note on intended behaviour: If there is no `tabular_data`, any column
-        alignment argument is ignored. Hence, in this case, header
-        alignment cannot be inferred from column alignment.
-
-    Table formats
-    -------------
-
-    `intfmt` is a format specification used for columns which
-    contain numeric data without a decimal point. This can also be
-    a list or tuple of format strings, one per column.
-
-    `floatfmt` is a format specification used for columns which
-    contain numeric data with a decimal point. This can also be
-    a list or tuple of format strings, one per column.
-
-    `None` values are replaced with a `missingval` string (like
-    `floatfmt`, this can also be a list of values for different
-    columns):
-
-    >>> print(tabulate([["spam", 1, None],
-    ...                 ["eggs", 42, 3.14],
-    ...                 ["other", None, 2.7]], missingval="?"))
-    -----  --  ----
-    spam    1  ?
-    eggs   42  3.14
-    other   ?  2.7
-    -----  --  ----
-
-    Various plain-text table formats (`tablefmt`) are supported:
-    'plain', 'simple', 'grid', 'pipe', 'orgtbl', 'rst', 'mediawiki',
-    'latex', 'latex_raw', 'latex_booktabs', 'latex_longtable' and tsv.
-    Variable `tabulate_formats`contains the list of currently supported formats.
-
-    "plain" format doesn't use any pseudographics to draw tables,
-    it separates columns with a double space:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                 ["strings", "numbers"], "plain"))
-    strings      numbers
-    spam         41.9999
-    eggs        451
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="plain"))
-    spam   41.9999
-    eggs  451
-
-    "simple" format is like Pandoc simple_tables:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                 ["strings", "numbers"], "simple"))
-    strings      numbers
-    ---------  ---------
-    spam         41.9999
-    eggs        451
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="simple"))
-    ----  --------
-    spam   41.9999
-    eggs  451
-    ----  --------
-
-    "grid" is similar to tables produced by Emacs table.el package or
-    Pandoc grid_tables:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "grid"))
-    +-----------+-----------+
-    | strings   |   numbers |
-    +===========+===========+
-    | spam      |   41.9999 |
-    +-----------+-----------+
-    | eggs      |  451      |
-    +-----------+-----------+
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="grid"))
-    +------+----------+
-    | spam |  41.9999 |
-    +------+----------+
-    | eggs | 451      |
-    +------+----------+
-
-    "simple_grid" draws a grid using single-line box-drawing
-    characters:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "simple_grid"))
-    ┌───────────┬───────────┐
-    │ strings   │   numbers │
-    ├───────────┼───────────┤
-    │ spam      │   41.9999 │
-    ├───────────┼───────────┤
-    │ eggs      │  451      │
-    └───────────┴───────────┘
-
-    "rounded_grid" draws a grid using single-line box-drawing
-    characters with rounded corners:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "rounded_grid"))
-    ╭───────────┬───────────╮
-    │ strings   │   numbers │
-    ├───────────┼───────────┤
-    │ spam      │   41.9999 │
-    ├───────────┼───────────┤
-    │ eggs      │  451      │
-    ╰───────────┴───────────╯
-
-    "heavy_grid" draws a grid using bold (thick) single-line box-drawing
-    characters:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "heavy_grid"))
-    ┏━━━━━━━━━━━┳━━━━━━━━━━━┓
-    ┃ strings   ┃   numbers ┃
-    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
-    ┃ spam      ┃   41.9999 ┃
-    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
-    ┃ eggs      ┃  451      ┃
-    ┗━━━━━━━━━━━┻━━━━━━━━━━━┛
-
-    "mixed_grid" draws a grid using a mix of light (thin) and heavy (thick) lines
-    box-drawing characters:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "mixed_grid"))
-    ┍━━━━━━━━━━━┯━━━━━━━━━━━┑
-    │ strings   │   numbers │
-    ┝━━━━━━━━━━━┿━━━━━━━━━━━┥
-    │ spam      │   41.9999 │
-    ├───────────┼───────────┤
-    │ eggs      │  451      │
-    ┕━━━━━━━━━━━┷━━━━━━━━━━━┙
-
-    "double_grid" draws a grid using double-line box-drawing
-    characters:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "double_grid"))
-    ╔═══════════╦═══════════╗
-    ║ strings   ║   numbers ║
-    ╠═══════════╬═══════════╣
-    ║ spam      ║   41.9999 ║
-    ╠═══════════╬═══════════╣
-    ║ eggs      ║  451      ║
-    ╚═══════════╩═══════════╝
-
-    "fancy_grid" draws a grid using a mix of single and
-    double-line box-drawing characters:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "fancy_grid"))
-    ╒═══════════╤═══════════╕
-    │ strings   │   numbers │
-    ╞═══════════╪═══════════╡
-    │ spam      │   41.9999 │
-    ├───────────┼───────────┤
-    │ eggs      │  451      │
-    ╘═══════════╧═══════════╛
-
-    "outline" is the same as the "grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "outline"))
-    +-----------+-----------+
-    | strings   |   numbers |
-    +===========+===========+
-    | spam      |   41.9999 |
-    | eggs      |  451      |
-    +-----------+-----------+
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="outline"))
-    +------+----------+
-    | spam |  41.9999 |
-    | eggs | 451      |
-    +------+----------+
-
-    "simple_outline" is the same as the "simple_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "simple_outline"))
-    ┌───────────┬───────────┐
-    │ strings   │   numbers │
-    ├───────────┼───────────┤
-    │ spam      │   41.9999 │
-    │ eggs      │  451      │
-    └───────────┴───────────┘
-
-    "rounded_outline" is the same as the "rounded_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "rounded_outline"))
-    ╭───────────┬───────────╮
-    │ strings   │   numbers │
-    ├───────────┼───────────┤
-    │ spam      │   41.9999 │
-    │ eggs      │  451      │
-    ╰───────────┴───────────╯
-
-    "heavy_outline" is the same as the "heavy_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "heavy_outline"))
-    ┏━━━━━━━━━━━┳━━━━━━━━━━━┓
-    ┃ strings   ┃   numbers ┃
-    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
-    ┃ spam      ┃   41.9999 ┃
-    ┃ eggs      ┃  451      ┃
-    ┗━━━━━━━━━━━┻━━━━━━━━━━━┛
-
-    "mixed_outline" is the same as the "mixed_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "mixed_outline"))
-    ┍━━━━━━━━━━━┯━━━━━━━━━━━┑
-    │ strings   │   numbers │
-    ┝━━━━━━━━━━━┿━━━━━━━━━━━┥
-    │ spam      │   41.9999 │
-    │ eggs      │  451      │
-    ┕━━━━━━━━━━━┷━━━━━━━━━━━┙
-
-    "double_outline" is the same as the "double_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "double_outline"))
-    ╔═══════════╦═══════════╗
-    ║ strings   ║   numbers ║
-    ╠═══════════╬═══════════╣
-    ║ spam      ║   41.9999 ║
-    ║ eggs      ║  451      ║
-    ╚═══════════╩═══════════╝
-
-    "fancy_outline" is the same as the "fancy_grid" format but doesn't draw lines between rows:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "fancy_outline"))
-    ╒═══════════╤═══════════╕
-    │ strings   │   numbers │
-    ╞═══════════╪═══════════╡
-    │ spam      │   41.9999 │
-    │ eggs      │  451      │
-    ╘═══════════╧═══════════╛
-
-    "pipe" is like tables in PHP Markdown Extra extension or Pandoc
-    pipe_tables:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "pipe"))
-    | strings   |   numbers |
-    |:----------|----------:|
-    | spam      |   41.9999 |
-    | eggs      |  451      |
-
-    "presto" is like tables produce by the Presto CLI:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "presto"))
-     strings   |   numbers
-    -----------+-----------
-     spam      |   41.9999
-     eggs      |  451
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="pipe"))
-    |:-----|---------:|
-    | spam |  41.9999 |
-    | eggs | 451      |
-
-    "orgtbl" is like tables in Emacs org-mode and orgtbl-mode. They
-    are slightly different from "pipe" format by not using colons to
-    define column alignment, and using a "+" sign to indicate line
-    intersections:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "orgtbl"))
-    | strings   |   numbers |
-    |-----------+-----------|
-    | spam      |   41.9999 |
-    | eggs      |  451      |
-
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="orgtbl"))
-    | spam |  41.9999 |
-    | eggs | 451      |
-
-    "rst" is like a simple table format from reStructuredText; please
-    note that reStructuredText accepts also "grid" tables:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
-    ...                ["strings", "numbers"], "rst"))
-    =========  =========
-    strings      numbers
-    =========  =========
-    spam         41.9999
-    eggs        451
-    =========  =========
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="rst"))
-    ====  ========
-    spam   41.9999
-    eggs  451
-    ====  ========
-
-    "mediawiki" produces a table markup used in Wikipedia and on other
-    MediaWiki-based sites:
-
-    >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
-    ...                headers="firstrow", tablefmt="mediawiki"))
-    {| class="wikitable" style="text-align: left;"
-    |+ <!-- caption -->
-    |-
-    ! strings   !! style="text-align: right;"|   numbers
-    |-
-    | spam      || style="text-align: right;"|   41.9999
-    |-
-    | eggs      || style="text-align: right;"|  451
-    |}
-
-    "html" produces HTML markup as an html.escape'd str
-    with a ._repr_html_ method so that Jupyter Lab and Notebook display the HTML
-    and a .str property so that the raw HTML remains accessible
-    the unsafehtml table format can be used if an unescaped HTML format is required:
-
-    >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
-    ...                headers="firstrow", tablefmt="html"))
-    <table>
-    <thead>
-    <tr><th>strings  </th><th style="text-align: right;">  numbers</th></tr>
-    </thead>
-    <tbody>
-    <tr><td>spam     </td><td style="text-align: right;">  41.9999</td></tr>
-    <tr><td>eggs     </td><td style="text-align: right;"> 451     </td></tr>
-    </tbody>
-    </table>
-
-    "latex" produces a tabular environment of LaTeX document markup:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex"))
-    \\begin{tabular}{lr}
-    \\hline
-     spam &  41.9999 \\\\
-     eggs & 451      \\\\
-    \\hline
-    \\end{tabular}
-
-    "latex_raw" is similar to "latex", but doesn't escape special characters,
-    such as backslash and underscore, so LaTeX commands may embedded into
-    cells' values:
-
-    >>> print(tabulate([["spam$_9$", 41.9999], ["\\\\emph{eggs}", "451.0"]], tablefmt="latex_raw"))
-    \\begin{tabular}{lr}
-    \\hline
-     spam$_9$    &  41.9999 \\\\
-     \\emph{eggs} & 451      \\\\
-    \\hline
-    \\end{tabular}
-
-    "latex_booktabs" produces a tabular environment of LaTeX document markup
-    using the booktabs.sty package:
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_booktabs"))
-    \\begin{tabular}{lr}
-    \\toprule
-     spam &  41.9999 \\\\
-     eggs & 451      \\\\
-    \\bottomrule
-    \\end{tabular}
-
-    "latex_longtable" produces a tabular environment that can stretch along
-    multiple pages, using the longtable package for LaTeX.
-
-    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_longtable"))
-    \\begin{longtable}{lr}
-    \\hline
-     spam &  41.9999 \\\\
-     eggs & 451      \\\\
-    \\hline
-    \\end{longtable}
-
-
-    Number parsing
-    --------------
-    By default, anything which can be parsed as a number is a number.
-    This ensures numbers represented as strings are aligned properly.
-    This can lead to weird results for particular strings such as
-    specific git SHAs e.g. "42992e1" will be parsed into the number
-    429920 and aligned as such.
-
-    To completely disable number parsing (and alignment), use
-    `disable_numparse=True`. For more fine grained control, a list column
-    indices is used to disable number parsing only on those columns
-    e.g. `disable_numparse=[0, 2]` would disable number parsing only on the
-    first and third columns.
-
-    Column Widths and Auto Line Wrapping
-    ------------------------------------
-    Tabulate will, by default, set the width of each column to the length of the
-    longest element in that column. However, in situations where fields are expected
-    to reasonably be too long to look good as a single line, tabulate can help automate
-    word wrapping long fields for you. Use the parameter `maxcolwidth` to provide a
-    list of maximal column widths
-
-    >>> print(tabulate( \
-          [('1', 'John Smith', \
-            'This is a rather long description that might look better if it is wrapped a bit')], \
-          headers=("Issue Id", "Author", "Description"), \
-          maxcolwidths=[None, None, 30], \
-          tablefmt="grid"  \
-        ))
-    +------------+------------+-------------------------------+
-    |   Issue Id | Author     | Description                   |
-    +============+============+===============================+
-    |          1 | John Smith | This is a rather long         |
-    |            |            | description that might look   |
-    |            |            | better if it is wrapped a bit |
-    +------------+------------+-------------------------------+
-
-    Header column width can be specified in a similar way using `maxheadercolwidth`
-
-    """
-
-    if tabular_data is None:
-        tabular_data = []
-
-    list_of_lists, headers, headers_pad = _normalize_tabular_data(
-        tabular_data, headers, showindex=showindex
-    )
-    list_of_lists, separating_lines = _remove_separating_lines(list_of_lists)
-
-    if maxcolwidths is not None:
-        if len(list_of_lists):
-            num_cols = len(list_of_lists[0])
-        else:
-            num_cols = 0
-        if isinstance(maxcolwidths, int):  # Expand scalar for all columns
-            maxcolwidths = _expand_iterable(maxcolwidths, num_cols, maxcolwidths)
-        else:  # Ignore col width for any 'trailing' columns
-            maxcolwidths = _expand_iterable(maxcolwidths, num_cols, None)
-
-        numparses = _expand_numparse(disable_numparse, num_cols)
-        list_of_lists = _wrap_text_to_colwidths(
-            list_of_lists, maxcolwidths, numparses=numparses
-        )
-
-    if maxheadercolwidths is not None:
-        num_cols = len(list_of_lists[0])
-        if isinstance(maxheadercolwidths, int):  # Expand scalar for all columns
-            maxheadercolwidths = _expand_iterable(
-                maxheadercolwidths, num_cols, maxheadercolwidths
-            )
-        else:  # Ignore col width for any 'trailing' columns
-            maxheadercolwidths = _expand_iterable(maxheadercolwidths, num_cols, None)
-
-        numparses = _expand_numparse(disable_numparse, num_cols)
-        headers = _wrap_text_to_colwidths(
-            [headers], maxheadercolwidths, numparses=numparses
-        )[0]
-
-    # empty values in the first column of RST tables should be escaped (issue #82)
-    # "" should be escaped as "\\ " or ".."
-    if tablefmt == "rst":
-        list_of_lists, headers = _rst_escape_first_column(list_of_lists, headers)
-
-    # PrettyTable formatting does not use any extra padding.
-    # Numbers are not parsed and are treated the same as strings for alignment.
-    # Check if pretty is the format being used and override the defaults so it
-    # does not impact other formats.
-    min_padding = MIN_PADDING
-    if tablefmt == "pretty":
-        min_padding = 0
-        disable_numparse = True
-        numalign = "center" if numalign == _DEFAULT_ALIGN else numalign
-        stralign = "center" if stralign == _DEFAULT_ALIGN else stralign
-    else:
-        numalign = "decimal" if numalign == _DEFAULT_ALIGN else numalign
-        stralign = "left" if stralign == _DEFAULT_ALIGN else stralign
-
-    # optimization: look for ANSI control codes once,
-    # enable smart width functions only if a control code is found
-    #
-    # convert the headers and rows into a single, tab-delimited string ensuring
-    # that any bytestrings are decoded safely (i.e. errors ignored)
-    plain_text = "\t".join(
-        chain(
-            # headers
-            map(_to_str, headers),
-            # rows: chain the rows together into a single iterable after mapping
-            # the bytestring conversino to each cell value
-            chain.from_iterable(map(_to_str, row) for row in list_of_lists),
-        )
-    )
-
-    has_invisible = _ansi_codes.search(plain_text) is not None
-
-    enable_widechars = wcwidth is not None and WIDE_CHARS_MODE
-    if (
-        not isinstance(tablefmt, TableFormat)
-        and tablefmt in multiline_formats
-        and _is_multiline(plain_text)
-    ):
-        tablefmt = multiline_formats.get(tablefmt, tablefmt)
-        is_multiline = True
-    else:
-        is_multiline = False
-    width_fn = _choose_width_fn(has_invisible, enable_widechars, is_multiline)
-
-    # format rows and columns, convert numeric values to strings
-    cols = list(izip_longest(*list_of_lists))
-    numparses = _expand_numparse(disable_numparse, len(cols))
-    coltypes = [_column_type(col, numparse=np) for col, np in zip(cols, numparses)]
-    if isinstance(floatfmt, str):  # old version
-        float_formats = len(cols) * [
-            floatfmt
-        ]  # just duplicate the string to use in each column
-    else:  # if floatfmt is list, tuple etc we have one per column
-        float_formats = list(floatfmt)
-        if len(float_formats) < len(cols):
-            float_formats.extend((len(cols) - len(float_formats)) * [_DEFAULT_FLOATFMT])
-    if isinstance(intfmt, str):  # old version
-        int_formats = len(cols) * [
-            intfmt
-        ]  # just duplicate the string to use in each column
-    else:  # if intfmt is list, tuple etc we have one per column
-        int_formats = list(intfmt)
-        if len(int_formats) < len(cols):
-            int_formats.extend((len(cols) - len(int_formats)) * [_DEFAULT_INTFMT])
-    if isinstance(missingval, str):
-        missing_vals = len(cols) * [missingval]
-    else:
-        missing_vals = list(missingval)
-        if len(missing_vals) < len(cols):
-            missing_vals.extend((len(cols) - len(missing_vals)) * [_DEFAULT_MISSINGVAL])
-    cols = [
-        [_format(v, ct, fl_fmt, int_fmt, miss_v, has_invisible) for v in c]
-        for c, ct, fl_fmt, int_fmt, miss_v in zip(
-            cols, coltypes, float_formats, int_formats, missing_vals
-        )
-    ]
-
-    # align columns
-    # first set global alignment
-    if colglobalalign is not None: # if global alignment provided
-        aligns = [colglobalalign] * len(cols)
-    else: # default
-        aligns = [numalign if ct in [int, float] else stralign for ct in coltypes]
-    # then specific alignements
-    if colalign is not None:
-        assert isinstance(colalign, Iterable)
-        if isinstance(colalign, str):
-            warnings.warn(f"As a string, `colalign` is interpreted as {[c for c in colalign]}. Did you mean `colglobalalign = \"{colalign}\"` or `colalign = (\"{colalign}\",)`?", stacklevel=2)
-        for idx, align in enumerate(colalign):
-            if not idx < len(aligns):
-                break
-            elif align != "global":
-                aligns[idx] = align
-    minwidths = (
-        [width_fn(h) + min_padding for h in headers] if headers else [0] * len(cols)
-    )
-    cols = [
-        _align_column(c, a, minw, has_invisible, enable_widechars, is_multiline)
-        for c, a, minw in zip(cols, aligns, minwidths)
-    ]
-
-    aligns_headers = None
-    if headers:
-        # align headers and add headers
-        t_cols = cols or [[""]] * len(headers)
-        # first set global alignment
-        if headersglobalalign is not None: # if global alignment provided
-            aligns_headers = [headersglobalalign] * len(t_cols)
-        else: # default
-            aligns_headers = aligns or [stralign] * len(headers)
-        # then specific header alignements
-        if headersalign is not None:
-            assert isinstance(headersalign, Iterable)
-            if isinstance(headersalign, str):
-                warnings.warn(f"As a string, `headersalign` is interpreted as {[c for c in headersalign]}. Did you mean `headersglobalalign = \"{headersalign}\"` or `headersalign = (\"{headersalign}\",)`?", stacklevel=2)
-            for idx, align in enumerate(headersalign):
-                hidx = headers_pad + idx
-                if not hidx < len(aligns_headers):
-                    break
-                elif align == "same" and hidx < len(aligns): # same as column align
-                    aligns_headers[hidx] = aligns[hidx]
-                elif align != "global":
-                    aligns_headers[hidx] = align
-        minwidths = [
-            max(minw, max(width_fn(cl) for cl in c))
-            for minw, c in zip(minwidths, t_cols)
-        ]
-        headers = [
-            _align_header(h, a, minw, width_fn(h), is_multiline, width_fn)
-            for h, a, minw in zip(headers, aligns_headers, minwidths)
-        ]
-        rows = list(zip(*cols))
-    else:
-        minwidths = [max(width_fn(cl) for cl in c) for c in cols]
-        rows = list(zip(*cols))
-
-    if not isinstance(tablefmt, TableFormat):
-        tablefmt = _table_formats.get(tablefmt, _table_formats["simple"])
-
-    ra_default = rowalign if isinstance(rowalign, str) else None
-    rowaligns = _expand_iterable(rowalign, len(rows), ra_default)
-    _reinsert_separating_lines(rows, separating_lines)
-
-    return _format_table(
-        tablefmt, headers, aligns_headers, rows, minwidths, aligns, is_multiline, rowaligns=rowaligns
-    )
-
-
-def _expand_numparse(disable_numparse, column_count):
-    """
-    Return a list of bools of length `column_count` which indicates whether
-    number parsing should be used on each column.
-    If `disable_numparse` is a list of indices, each of those indices are False,
-    and everything else is True.
-    If `disable_numparse` is a bool, then the returned list is all the same.
-    """
-    if isinstance(disable_numparse, Iterable):
-        numparses = [True] * column_count
-        for index in disable_numparse:
-            numparses[index] = False
-        return numparses
-    else:
-        return [not disable_numparse] * column_count
-
-
-def _expand_iterable(original, num_desired, default):
-    """
-    Expands the `original` argument to return a return a list of
-    length `num_desired`. If `original` is shorter than `num_desired`, it will
-    be padded with the value in `default`.
-    If `original` is not a list to begin with (i.e. scalar value) a list of
-    length `num_desired` completely populated with `default will be returned
-    """
-    if isinstance(original, Iterable) and not isinstance(original, str):
-        return original + [default] * (num_desired - len(original))
-    else:
-        return [default] * num_desired
-
-
-def _pad_row(cells, padding):
-    if cells:
-        pad = " " * padding
-        padded_cells = [pad + cell + pad for cell in cells]
-        return padded_cells
-    else:
-        return cells
-
-
-def _build_simple_row(padded_cells, rowfmt):
-    "Format row according to DataRow format without padding."
-    begin, sep, end = rowfmt
-    return (begin + sep.join(padded_cells) + end).rstrip()
-
-
-def _build_row(padded_cells, colwidths, colaligns, rowfmt):
-    "Return a string which represents a row of data cells."
-    if not rowfmt:
-        return None
-    if hasattr(rowfmt, "__call__"):
-        return rowfmt(padded_cells, colwidths, colaligns)
-    else:
-        return _build_simple_row(padded_cells, rowfmt)
-
-
-def _append_basic_row(lines, padded_cells, colwidths, colaligns, rowfmt, rowalign=None):
-    # NOTE: rowalign is ignored and exists for api compatibility with _append_multiline_row
-    lines.append(_build_row(padded_cells, colwidths, colaligns, rowfmt))
-    return lines
-
-
-def _align_cell_veritically(text_lines, num_lines, column_width, row_alignment):
-    delta_lines = num_lines - len(text_lines)
-    blank = [" " * column_width]
-    if row_alignment == "bottom":
-        return blank * delta_lines + text_lines
-    elif row_alignment == "center":
-        top_delta = delta_lines // 2
-        bottom_delta = delta_lines - top_delta
-        return top_delta * blank + text_lines + bottom_delta * blank
-    else:
-        return text_lines + blank * delta_lines
-
-
-def _append_multiline_row(
-    lines, padded_multiline_cells, padded_widths, colaligns, rowfmt, pad, rowalign=None
-):
-    colwidths = [w - 2 * pad for w in padded_widths]
-    cells_lines = [c.splitlines() for c in padded_multiline_cells]
-    nlines = max(map(len, cells_lines))  # number of lines in the row
-    # vertically pad cells where some lines are missing
-    # cells_lines = [
-    #     (cl + [" " * w] * (nlines - len(cl))) for cl, w in zip(cells_lines, colwidths)
-    # ]
-
-    cells_lines = [
-        _align_cell_veritically(cl, nlines, w, rowalign)
-        for cl, w in zip(cells_lines, colwidths)
-    ]
-    lines_cells = [[cl[i] for cl in cells_lines] for i in range(nlines)]
-    for ln in lines_cells:
-        padded_ln = _pad_row(ln, pad)
-        _append_basic_row(lines, padded_ln, colwidths, colaligns, rowfmt)
-    return lines
-
-
-def _build_line(colwidths, colaligns, linefmt):
-    "Return a string which represents a horizontal line."
-    if not linefmt:
-        return None
-    if hasattr(linefmt, "__call__"):
-        return linefmt(colwidths, colaligns)
-    else:
-        begin, fill, sep, end = linefmt
-        cells = [fill * w for w in colwidths]
-        return _build_simple_row(cells, (begin, sep, end))
-
-
-def _append_line(lines, colwidths, colaligns, linefmt):
-    lines.append(_build_line(colwidths, colaligns, linefmt))
-    return lines
-
-
-class JupyterHTMLStr(str):
-    """Wrap the string with a _repr_html_ method so that Jupyter
-    displays the HTML table"""
-
-    def _repr_html_(self):
-        return self
-
-    @property
-    def str(self):
-        """add a .str property so that the raw string is still accessible"""
-        return self
-
-
-def _format_table(fmt, headers, headersaligns, rows, colwidths, colaligns, is_multiline, rowaligns):
-    """Produce a plain-text representation of the table."""
-    lines = []
-    hidden = fmt.with_header_hide if (headers and fmt.with_header_hide) else []
-    pad = fmt.padding
-    headerrow = fmt.headerrow
-
-    padded_widths = [(w + 2 * pad) for w in colwidths]
-    if is_multiline:
-        pad_row = lambda row, _: row  # noqa do it later, in _append_multiline_row
-        append_row = partial(_append_multiline_row, pad=pad)
-    else:
-        pad_row = _pad_row
-        append_row = _append_basic_row
-
-    padded_headers = pad_row(headers, pad)
-    padded_rows = [pad_row(row, pad) for row in rows]
-
-    if fmt.lineabove and "lineabove" not in hidden:
-        _append_line(lines, padded_widths, colaligns, fmt.lineabove)
-
-    if padded_headers:
-        append_row(lines, padded_headers, padded_widths, headersaligns, headerrow)
-        if fmt.linebelowheader and "linebelowheader" not in hidden:
-            _append_line(lines, padded_widths, colaligns, fmt.linebelowheader)
-
-    if padded_rows and fmt.linebetweenrows and "linebetweenrows" not in hidden:
-        # initial rows with a line below
-        for row, ralign in zip(padded_rows[:-1], rowaligns):
-            append_row(
-                lines, row, padded_widths, colaligns, fmt.datarow, rowalign=ralign
-            )
-            _append_line(lines, padded_widths, colaligns, fmt.linebetweenrows)
-        # the last row without a line below
-        append_row(
-            lines,
-            padded_rows[-1],
-            padded_widths,
-            colaligns,
-            fmt.datarow,
-            rowalign=rowaligns[-1],
-        )
-    else:
-        separating_line = (
-            fmt.linebetweenrows
-            or fmt.linebelowheader
-            or fmt.linebelow
-            or fmt.lineabove
-            or Line("", "", "", "")
-        )
-        for row in padded_rows:
-            # test to see if either the 1st column or the 2nd column (account for showindex) has
-            # the SEPARATING_LINE flag
-            if _is_separating_line(row):
-                _append_line(lines, padded_widths, colaligns, separating_line)
-            else:
-                append_row(lines, row, padded_widths, colaligns, fmt.datarow)
-
-    if fmt.linebelow and "linebelow" not in hidden:
-        _append_line(lines, padded_widths, colaligns, fmt.linebelow)
-
-    if headers or rows:
-        output = "\n".join(lines)
-        if fmt.lineabove == _html_begin_table_without_header:
-            return JupyterHTMLStr(output)
-        else:
-            return output
-    else:  # a completely empty table
-        return ""
-
-
-class _CustomTextWrap(textwrap.TextWrapper):
-    """A custom implementation of CPython's textwrap.TextWrapper. This supports
-    both wide characters (Korea, Japanese, Chinese)  - including mixed string.
-    For the most part, the `_handle_long_word` and `_wrap_chunks` functions were
-    copy pasted out of the CPython baseline, and updated with our custom length
-    and line appending logic.
-    """
-
-    def __init__(self, *args, **kwargs):
-        self._active_codes = []
-        self.max_lines = None  # For python2 compatibility
-        textwrap.TextWrapper.__init__(self, *args, **kwargs)
-
-    @staticmethod
-    def _len(item):
-        """Custom len that gets console column width for wide
-        and non-wide characters as well as ignores color codes"""
-        stripped = _strip_ansi(item)
-        if wcwidth:
-            return wcwidth.wcswidth(stripped)
-        else:
-            return len(stripped)
-
-    def _update_lines(self, lines, new_line):
-        """Adds a new line to the list of lines the text is being wrapped into
-        This function will also track any ANSI color codes in this string as well
-        as add any colors from previous lines order to preserve the same formatting
-        as a single unwrapped string.
-        """
-        code_matches = [x for x in _ansi_codes.finditer(new_line)]
-        color_codes = [
-            code.string[code.span()[0] : code.span()[1]] for code in code_matches
-        ]
-
-        # Add color codes from earlier in the unwrapped line, and then track any new ones we add.
-        new_line = "".join(self._active_codes) + new_line
-
-        for code in color_codes:
-            if code != _ansi_color_reset_code:
-                self._active_codes.append(code)
-            else:  # A single reset code resets everything
-                self._active_codes = []
-
-        # Always ensure each line is color terminted if any colors are
-        # still active, otherwise colors will bleed into other cells on the console
-        if len(self._active_codes) > 0:
-            new_line = new_line + _ansi_color_reset_code
-
-        lines.append(new_line)
-
-    def _handle_long_word(self, reversed_chunks, cur_line, cur_len, width):
-        """_handle_long_word(chunks : [string],
-                             cur_line : [string],
-                             cur_len : int, width : int)
-        Handle a chunk of text (most likely a word, not whitespace) that
-        is too long to fit in any line.
-        """
-        # Figure out when indent is larger than the specified width, and make
-        # sure at least one character is stripped off on every pass
-        if width < 1:
-            space_left = 1
-        else:
-            space_left = width - cur_len
-
-        # If we're allowed to break long words, then do so: put as much
-        # of the next chunk onto the current line as will fit.
-        if self.break_long_words:
-            # Tabulate Custom: Build the string up piece-by-piece in order to
-            # take each charcter's width into account
-            chunk = reversed_chunks[-1]
-            i = 1
-            while self._len(chunk[:i]) <= space_left:
-                i = i + 1
-            cur_line.append(chunk[: i - 1])
-            reversed_chunks[-1] = chunk[i - 1 :]
-
-        # Otherwise, we have to preserve the long word intact.  Only add
-        # it to the current line if there's nothing already there --
-        # that minimizes how much we violate the width constraint.
-        elif not cur_line:
-            cur_line.append(reversed_chunks.pop())
-
-        # If we're not allowed to break long words, and there's already
-        # text on the current line, do nothing.  Next time through the
-        # main loop of _wrap_chunks(), we'll wind up here again, but
-        # cur_len will be zero, so the next line will be entirely
-        # devoted to the long word that we can't handle right now.
-
-    def _wrap_chunks(self, chunks):
-        """_wrap_chunks(chunks : [string]) -> [string]
-        Wrap a sequence of text chunks and return a list of lines of
-        length 'self.width' or less.  (If 'break_long_words' is false,
-        some lines may be longer than this.)  Chunks correspond roughly
-        to words and the whitespace between them: each chunk is
-        indivisible (modulo 'break_long_words'), but a line break can
-        come between any two chunks.  Chunks should not have internal
-        whitespace; ie. a chunk is either all whitespace or a "word".
-        Whitespace chunks will be removed from the beginning and end of
-        lines, but apart from that whitespace is preserved.
-        """
-        lines = []
-        if self.width <= 0:
-            raise ValueError("invalid width %r (must be > 0)" % self.width)
-        if self.max_lines is not None:
-            if self.max_lines > 1:
-                indent = self.subsequent_indent
-            else:
-                indent = self.initial_indent
-            if self._len(indent) + self._len(self.placeholder.lstrip()) > self.width:
-                raise ValueError("placeholder too large for max width")
-
-        # Arrange in reverse order so items can be efficiently popped
-        # from a stack of chucks.
-        chunks.reverse()
-
-        while chunks:
-
-            # Start the list of chunks that will make up the current line.
-            # cur_len is just the length of all the chunks in cur_line.
-            cur_line = []
-            cur_len = 0
-
-            # Figure out which static string will prefix this line.
-            if lines:
-                indent = self.subsequent_indent
-            else:
-                indent = self.initial_indent
-
-            # Maximum width for this line.
-            width = self.width - self._len(indent)
-
-            # First chunk on line is whitespace -- drop it, unless this
-            # is the very beginning of the text (ie. no lines started yet).
-            if self.drop_whitespace and chunks[-1].strip() == "" and lines:
-                del chunks[-1]
-
-            while chunks:
-                chunk_len = self._len(chunks[-1])
-
-                # Can at least squeeze this chunk onto the current line.
-                if cur_len + chunk_len <= width:
-                    cur_line.append(chunks.pop())
-                    cur_len += chunk_len
-
-                # Nope, this line is full.
-                else:
-                    break
-
-            # The current line is full, and the next chunk is too big to
-            # fit on *any* line (not just this one).
-            if chunks and self._len(chunks[-1]) > width:
-                self._handle_long_word(chunks, cur_line, cur_len, width)
-                cur_len = sum(map(self._len, cur_line))
-
-            # If the last chunk on this line is all whitespace, drop it.
-            if self.drop_whitespace and cur_line and cur_line[-1].strip() == "":
-                cur_len -= self._len(cur_line[-1])
-                del cur_line[-1]
-
-            if cur_line:
-                if (
-                    self.max_lines is None
-                    or len(lines) + 1 < self.max_lines
-                    or (
-                        not chunks
-                        or self.drop_whitespace
-                        and len(chunks) == 1
-                        and not chunks[0].strip()
-                    )
-                    and cur_len <= width
-                ):
-                    # Convert current line back to a string and store it in
-                    # list of all lines (return value).
-                    self._update_lines(lines, indent + "".join(cur_line))
-                else:
-                    while cur_line:
-                        if (
-                            cur_line[-1].strip()
-                            and cur_len + self._len(self.placeholder) <= width
-                        ):
-                            cur_line.append(self.placeholder)
-                            self._update_lines(lines, indent + "".join(cur_line))
-                            break
-                        cur_len -= self._len(cur_line[-1])
-                        del cur_line[-1]
-                    else:
-                        if lines:
-                            prev_line = lines[-1].rstrip()
-                            if (
-                                self._len(prev_line) + self._len(self.placeholder)
-                                <= self.width
-                            ):
-                                lines[-1] = prev_line + self.placeholder
-                                break
-                        self._update_lines(lines, indent + self.placeholder.lstrip())
-                    break
-
-        return lines
-
-
-def _main():
-    """\
-    Usage: tabulate [options] [FILE ...]
-
-    Pretty-print tabular data.
-    See also https://github.com/astanin/python-tabulate
-
-    FILE                      a filename of the file with tabular data;
-                              if "-" or missing, read data from stdin.
-
-    Options:
-
-    -h, --help                show this message
-    -1, --header              use the first row of data as a table header
-    -o FILE, --output FILE    print table to FILE (default: stdout)
-    -s REGEXP, --sep REGEXP   use a custom column separator (default: whitespace)
-    -F FPFMT, --float FPFMT   floating point number format (default: g)
-    -I INTFMT, --int INTFMT   integer point number format (default: "")
-    -f FMT, --format FMT      set output table format; supported formats:
-                              plain, simple, grid, fancy_grid, pipe, orgtbl,
-                              rst, mediawiki, html, latex, latex_raw,
-                              latex_booktabs, latex_longtable, tsv
-                              (default: simple)
-    """
-    import getopt
-    import sys
-    import textwrap
-
-    usage = textwrap.dedent(_main.__doc__)
-    try:
-        opts, args = getopt.getopt(
-            sys.argv[1:],
-            "h1o:s:F:A:f:",
-            ["help", "header", "output", "sep=", "float=", "int=", "align=", "format="],
-        )
-    except getopt.GetoptError as e:
-        print(e)
-        print(usage)
-        sys.exit(2)
-    headers = []
-    floatfmt = _DEFAULT_FLOATFMT
-    intfmt = _DEFAULT_INTFMT
-    colalign = None
-    tablefmt = "simple"
-    sep = r"\s+"
-    outfile = "-"
-    for opt, value in opts:
-        if opt in ["-1", "--header"]:
-            headers = "firstrow"
-        elif opt in ["-o", "--output"]:
-            outfile = value
-        elif opt in ["-F", "--float"]:
-            floatfmt = value
-        elif opt in ["-I", "--int"]:
-            intfmt = value
-        elif opt in ["-C", "--colalign"]:
-            colalign = value.split()
-        elif opt in ["-f", "--format"]:
-            if value not in tabulate_formats:
-                print("%s is not a supported table format" % value)
-                print(usage)
-                sys.exit(3)
-            tablefmt = value
-        elif opt in ["-s", "--sep"]:
-            sep = value
-        elif opt in ["-h", "--help"]:
-            print(usage)
-            sys.exit(0)
-    files = [sys.stdin] if not args else args
-    with (sys.stdout if outfile == "-" else open(outfile, "w")) as out:
-        for f in files:
-            if f == "-":
-                f = sys.stdin
-            if _is_file(f):
-                _pprint_file(
-                    f,
-                    headers=headers,
-                    tablefmt=tablefmt,
-                    sep=sep,
-                    floatfmt=floatfmt,
-                    intfmt=intfmt,
-                    file=out,
-                    colalign=colalign,
-                )
-            else:
-                with open(f) as fobj:
-                    _pprint_file(
-                        fobj,
-                        headers=headers,
-                        tablefmt=tablefmt,
-                        sep=sep,
-                        floatfmt=floatfmt,
-                        intfmt=intfmt,
-                        file=out,
-                        colalign=colalign,
-                    )
-
-
-def _pprint_file(fobject, headers, tablefmt, sep, floatfmt, intfmt, file, colalign):
-    rows = fobject.readlines()
-    table = [re.split(sep, r.rstrip()) for r in rows if r.strip()]
-    print(
-        tabulate(
-            table,
-            headers,
-            tablefmt,
-            floatfmt=floatfmt,
-            intfmt=intfmt,
-            colalign=colalign,
-        ),
-        file=file,
-    )
-
-
-if __name__ == "__main__":
-    _main()
+"""Pretty-print tabular data."""
+
+import warnings
+from collections import namedtuple
+from collections.abc import Iterable, Sized
+from html import escape as htmlescape
+from itertools import chain, zip_longest as izip_longest
+from functools import reduce, partial
+import io
+import re
+import math
+import textwrap
+import dataclasses
+
+try:
+    import wcwidth  # optional wide-character (CJK) support
+except ImportError:
+    wcwidth = None
+
+
+def _is_file(f):
+    return isinstance(f, io.IOBase)
+
+
+__all__ = ["tabulate", "tabulate_formats", "simple_separated_format"]
+try:
+    from .version import version as __version__  # noqa: F401
+except ImportError:
+    pass  # running __init__.py as a script, AppVeyor pytests
+
+
+# minimum extra space in headers
+MIN_PADDING = 2
+
+# Whether or not to preserve leading/trailing whitespace in data.
+PRESERVE_WHITESPACE = False
+
+_DEFAULT_FLOATFMT = "g"
+_DEFAULT_INTFMT = ""
+_DEFAULT_MISSINGVAL = ""
+# default align will be overwritten by "left", "center" or "decimal"
+# depending on the formatter
+_DEFAULT_ALIGN = "default"
+
+
+# if True, enable wide-character (CJK) support
+WIDE_CHARS_MODE = wcwidth is not None
+
+# Constant that can be used as part of passed rows to generate a separating line
+# It is purposely an unprintable character, very unlikely to be used in a table
+SEPARATING_LINE = "\001"
+
+Line = namedtuple("Line", ["begin", "hline", "sep", "end"])
+
+
+DataRow = namedtuple("DataRow", ["begin", "sep", "end"])
+
+
+# A table structure is supposed to be:
+#
+#     --- lineabove ---------
+#         headerrow
+#     --- linebelowheader ---
+#         datarow
+#     --- linebetweenrows ---
+#     ... (more datarows) ...
+#     --- linebetweenrows ---
+#         last datarow
+#     --- linebelow ---------
+#
+# TableFormat's line* elements can be
+#
+#   - either None, if the element is not used,
+#   - or a Line tuple,
+#   - or a function: [col_widths], [col_alignments] -> string.
+#
+# TableFormat's *row elements can be
+#
+#   - either None, if the element is not used,
+#   - or a DataRow tuple,
+#   - or a function: [cell_values], [col_widths], [col_alignments] -> string.
+#
+# padding (an integer) is the amount of white space around data values.
+#
+# with_header_hide:
+#
+#   - either None, to display all table elements unconditionally,
+#   - or a list of elements not to be displayed if the table has column headers.
+#
+TableFormat = namedtuple(
+    "TableFormat",
+    [
+        "lineabove",
+        "linebelowheader",
+        "linebetweenrows",
+        "linebelow",
+        "headerrow",
+        "datarow",
+        "padding",
+        "with_header_hide",
+    ],
+)
+
+
+def _is_separating_line(row):
+    row_type = type(row)
+    is_sl = (row_type == list or row_type == str) and (
+        (len(row) >= 1 and row[0] == SEPARATING_LINE)
+        or (len(row) >= 2 and row[1] == SEPARATING_LINE)
+    )
+    return is_sl
+
+
+def _pipe_segment_with_colons(align, colwidth):
+    """Return a segment of a horizontal line with optional colons which
+    indicate column's alignment (as in `pipe` output format)."""
+    w = colwidth
+    if align in ["right", "decimal"]:
+        return ("-" * (w - 1)) + ":"
+    elif align == "center":
+        return ":" + ("-" * (w - 2)) + ":"
+    elif align == "left":
+        return ":" + ("-" * (w - 1))
+    else:
+        return "-" * w
+
+
+def _pipe_line_with_colons(colwidths, colaligns):
+    """Return a horizontal line with optional colons to indicate column's
+    alignment (as in `pipe` output format)."""
+    if not colaligns:  # e.g. printing an empty data frame (github issue #15)
+        colaligns = [""] * len(colwidths)
+    segments = [_pipe_segment_with_colons(a, w) for a, w in zip(colaligns, colwidths)]
+    return "|" + "|".join(segments) + "|"
+
+
+def _mediawiki_row_with_attrs(separator, cell_values, colwidths, colaligns):
+    alignment = {
+        "left": "",
+        "right": 'style="text-align: right;"| ',
+        "center": 'style="text-align: center;"| ',
+        "decimal": 'style="text-align: right;"| ',
+    }
+    # hard-coded padding _around_ align attribute and value together
+    # rather than padding parameter which affects only the value
+    values_with_attrs = [
+        " " + alignment.get(a, "") + c + " " for c, a in zip(cell_values, colaligns)
+    ]
+    colsep = separator * 2
+    return (separator + colsep.join(values_with_attrs)).rstrip()
+
+
+def _textile_row_with_attrs(cell_values, colwidths, colaligns):
+    cell_values[0] += " "
+    alignment = {"left": "<.", "right": ">.", "center": "=.", "decimal": ">."}
+    values = (alignment.get(a, "") + v for a, v in zip(colaligns, cell_values))
+    return "|" + "|".join(values) + "|"
+
+
+def _html_begin_table_without_header(colwidths_ignore, colaligns_ignore):
+    # this table header will be suppressed if there is a header row
+    return "<table>\n<tbody>"
+
+
+def _html_row_with_attrs(celltag, unsafe, cell_values, colwidths, colaligns):
+    alignment = {
+        "left": "",
+        "right": ' style="text-align: right;"',
+        "center": ' style="text-align: center;"',
+        "decimal": ' style="text-align: right;"',
+    }
+    if unsafe:
+        values_with_attrs = [
+            "<{0}{1}>{2}</{0}>".format(celltag, alignment.get(a, ""), c)
+            for c, a in zip(cell_values, colaligns)
+        ]
+    else:
+        values_with_attrs = [
+            "<{0}{1}>{2}</{0}>".format(celltag, alignment.get(a, ""), htmlescape(c))
+            for c, a in zip(cell_values, colaligns)
+        ]
+    rowhtml = "<tr>{}</tr>".format("".join(values_with_attrs).rstrip())
+    if celltag == "th":  # it's a header row, create a new table header
+        rowhtml = f"<table>\n<thead>\n{rowhtml}\n</thead>\n<tbody>"
+    return rowhtml
+
+
+def _moin_row_with_attrs(celltag, cell_values, colwidths, colaligns, header=""):
+    alignment = {
+        "left": "",
+        "right": '<style="text-align: right;">',
+        "center": '<style="text-align: center;">',
+        "decimal": '<style="text-align: right;">',
+    }
+    values_with_attrs = [
+        "{}{} {} ".format(celltag, alignment.get(a, ""), header + c + header)
+        for c, a in zip(cell_values, colaligns)
+    ]
+    return "".join(values_with_attrs) + "||"
+
+
+def _latex_line_begin_tabular(colwidths, colaligns, booktabs=False, longtable=False):
+    alignment = {"left": "l", "right": "r", "center": "c", "decimal": "r"}
+    tabular_columns_fmt = "".join([alignment.get(a, "l") for a in colaligns])
+    return "\n".join(
+        [
+            ("\\begin{tabular}{" if not longtable else "\\begin{longtable}{")
+            + tabular_columns_fmt
+            + "}",
+            "\\toprule" if booktabs else "\\hline",
+        ]
+    )
+
+
+def _asciidoc_row(is_header, *args):
+    """handle header and data rows for asciidoc format"""
+
+    def make_header_line(is_header, colwidths, colaligns):
+        # generate the column specifiers
+
+        alignment = {"left": "<", "right": ">", "center": "^", "decimal": ">"}
+        # use the column widths generated by tabulate for the asciidoc column width specifiers
+        asciidoc_alignments = zip(
+            colwidths, [alignment[colalign] for colalign in colaligns]
+        )
+        asciidoc_column_specifiers = [
+            "{:d}{}".format(width, align) for width, align in asciidoc_alignments
+        ]
+        header_list = ['cols="' + (",".join(asciidoc_column_specifiers)) + '"']
+
+        # generate the list of options (currently only "header")
+        options_list = []
+
+        if is_header:
+            options_list.append("header")
+
+        if options_list:
+            header_list += ['options="' + ",".join(options_list) + '"']
+
+        # generate the list of entries in the table header field
+
+        return "[{}]\n|====".format(",".join(header_list))
+
+    if len(args) == 2:
+        # two arguments are passed if called in the context of aboveline
+        # print the table header with column widths and optional header tag
+        return make_header_line(False, *args)
+
+    elif len(args) == 3:
+        # three arguments are passed if called in the context of dataline or headerline
+        # print the table line and make the aboveline if it is a header
+
+        cell_values, colwidths, colaligns = args
+        data_line = "|" + "|".join(cell_values)
+
+        if is_header:
+            return make_header_line(True, colwidths, colaligns) + "\n" + data_line
+        else:
+            return data_line
+
+    else:
+        raise ValueError(
+            " _asciidoc_row() requires two (colwidths, colaligns) "
+            + "or three (cell_values, colwidths, colaligns) arguments) "
+        )
+
+
+LATEX_ESCAPE_RULES = {
+    r"&": r"\&",
+    r"%": r"\%",
+    r"$": r"\$",
+    r"#": r"\#",
+    r"_": r"\_",
+    r"^": r"\^{}",
+    r"{": r"\{",
+    r"}": r"\}",
+    r"~": r"\textasciitilde{}",
+    "\\": r"\textbackslash{}",
+    r"<": r"\ensuremath{<}",
+    r">": r"\ensuremath{>}",
+}
+
+
+def _latex_row(cell_values, colwidths, colaligns, escrules=LATEX_ESCAPE_RULES):
+    def escape_char(c):
+        return escrules.get(c, c)
+
+    escaped_values = ["".join(map(escape_char, cell)) for cell in cell_values]
+    rowfmt = DataRow("", "&", "\\\\")
+    return _build_simple_row(escaped_values, rowfmt)
+
+
+def _rst_escape_first_column(rows, headers):
+    def escape_empty(val):
+        if isinstance(val, (str, bytes)) and not val.strip():
+            return ".."
+        else:
+            return val
+
+    new_headers = list(headers)
+    new_rows = []
+    if headers:
+        new_headers[0] = escape_empty(headers[0])
+    for row in rows:
+        new_row = list(row)
+        if new_row:
+            new_row[0] = escape_empty(row[0])
+        new_rows.append(new_row)
+    return new_rows, new_headers
+
+
+_table_formats = {
+    "simple": TableFormat(
+        lineabove=Line("", "-", "  ", ""),
+        linebelowheader=Line("", "-", "  ", ""),
+        linebetweenrows=None,
+        linebelow=Line("", "-", "  ", ""),
+        headerrow=DataRow("", "  ", ""),
+        datarow=DataRow("", "  ", ""),
+        padding=0,
+        with_header_hide=["lineabove", "linebelow"],
+    ),
+    "plain": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("", "  ", ""),
+        datarow=DataRow("", "  ", ""),
+        padding=0,
+        with_header_hide=None,
+    ),
+    "grid": TableFormat(
+        lineabove=Line("+", "-", "+", "+"),
+        linebelowheader=Line("+", "=", "+", "+"),
+        linebetweenrows=Line("+", "-", "+", "+"),
+        linebelow=Line("+", "-", "+", "+"),
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "simple_grid": TableFormat(
+        lineabove=Line("┌", "─", "┬", "┐"),
+        linebelowheader=Line("├", "─", "┼", "┤"),
+        linebetweenrows=Line("├", "─", "┼", "┤"),
+        linebelow=Line("└", "─", "┴", "┘"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "rounded_grid": TableFormat(
+        lineabove=Line("╭", "─", "┬", "╮"),
+        linebelowheader=Line("├", "─", "┼", "┤"),
+        linebetweenrows=Line("├", "─", "┼", "┤"),
+        linebelow=Line("╰", "─", "┴", "╯"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "heavy_grid": TableFormat(
+        lineabove=Line("┏", "━", "┳", "┓"),
+        linebelowheader=Line("┣", "━", "╋", "┫"),
+        linebetweenrows=Line("┣", "━", "╋", "┫"),
+        linebelow=Line("┗", "━", "┻", "┛"),
+        headerrow=DataRow("┃", "┃", "┃"),
+        datarow=DataRow("┃", "┃", "┃"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "mixed_grid": TableFormat(
+        lineabove=Line("┍", "━", "┯", "┑"),
+        linebelowheader=Line("┝", "━", "┿", "┥"),
+        linebetweenrows=Line("├", "─", "┼", "┤"),
+        linebelow=Line("┕", "━", "┷", "┙"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "double_grid": TableFormat(
+        lineabove=Line("╔", "═", "╦", "╗"),
+        linebelowheader=Line("╠", "═", "╬", "╣"),
+        linebetweenrows=Line("╠", "═", "╬", "╣"),
+        linebelow=Line("╚", "═", "╩", "╝"),
+        headerrow=DataRow("║", "║", "║"),
+        datarow=DataRow("║", "║", "║"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "fancy_grid": TableFormat(
+        lineabove=Line("╒", "═", "╤", "╕"),
+        linebelowheader=Line("╞", "═", "╪", "╡"),
+        linebetweenrows=Line("├", "─", "┼", "┤"),
+        linebelow=Line("╘", "═", "╧", "╛"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "outline": TableFormat(
+        lineabove=Line("+", "-", "+", "+"),
+        linebelowheader=Line("+", "=", "+", "+"),
+        linebetweenrows=None,
+        linebelow=Line("+", "-", "+", "+"),
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "simple_outline": TableFormat(
+        lineabove=Line("┌", "─", "┬", "┐"),
+        linebelowheader=Line("├", "─", "┼", "┤"),
+        linebetweenrows=None,
+        linebelow=Line("└", "─", "┴", "┘"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "rounded_outline": TableFormat(
+        lineabove=Line("╭", "─", "┬", "╮"),
+        linebelowheader=Line("├", "─", "┼", "┤"),
+        linebetweenrows=None,
+        linebelow=Line("╰", "─", "┴", "╯"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "heavy_outline": TableFormat(
+        lineabove=Line("┏", "━", "┳", "┓"),
+        linebelowheader=Line("┣", "━", "╋", "┫"),
+        linebetweenrows=None,
+        linebelow=Line("┗", "━", "┻", "┛"),
+        headerrow=DataRow("┃", "┃", "┃"),
+        datarow=DataRow("┃", "┃", "┃"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "mixed_outline": TableFormat(
+        lineabove=Line("┍", "━", "┯", "┑"),
+        linebelowheader=Line("┝", "━", "┿", "┥"),
+        linebetweenrows=None,
+        linebelow=Line("┕", "━", "┷", "┙"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "double_outline": TableFormat(
+        lineabove=Line("╔", "═", "╦", "╗"),
+        linebelowheader=Line("╠", "═", "╬", "╣"),
+        linebetweenrows=None,
+        linebelow=Line("╚", "═", "╩", "╝"),
+        headerrow=DataRow("║", "║", "║"),
+        datarow=DataRow("║", "║", "║"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "fancy_outline": TableFormat(
+        lineabove=Line("╒", "═", "╤", "╕"),
+        linebelowheader=Line("╞", "═", "╪", "╡"),
+        linebetweenrows=None,
+        linebelow=Line("╘", "═", "╧", "╛"),
+        headerrow=DataRow("│", "│", "│"),
+        datarow=DataRow("│", "│", "│"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "github": TableFormat(
+        lineabove=Line("|", "-", "|", "|"),
+        linebelowheader=Line("|", "-", "|", "|"),
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=["lineabove"],
+    ),
+    "pipe": TableFormat(
+        lineabove=_pipe_line_with_colons,
+        linebelowheader=_pipe_line_with_colons,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=["lineabove"],
+    ),
+    "orgtbl": TableFormat(
+        lineabove=None,
+        linebelowheader=Line("|", "-", "+", "|"),
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "jira": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("||", "||", "||"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "presto": TableFormat(
+        lineabove=None,
+        linebelowheader=Line("", "-", "+", ""),
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("", "|", ""),
+        datarow=DataRow("", "|", ""),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "pretty": TableFormat(
+        lineabove=Line("+", "-", "+", "+"),
+        linebelowheader=Line("+", "-", "+", "+"),
+        linebetweenrows=None,
+        linebelow=Line("+", "-", "+", "+"),
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "psql": TableFormat(
+        lineabove=Line("+", "-", "+", "+"),
+        linebelowheader=Line("|", "-", "+", "|"),
+        linebetweenrows=None,
+        linebelow=Line("+", "-", "+", "+"),
+        headerrow=DataRow("|", "|", "|"),
+        datarow=DataRow("|", "|", "|"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "rst": TableFormat(
+        lineabove=Line("", "=", "  ", ""),
+        linebelowheader=Line("", "=", "  ", ""),
+        linebetweenrows=None,
+        linebelow=Line("", "=", "  ", ""),
+        headerrow=DataRow("", "  ", ""),
+        datarow=DataRow("", "  ", ""),
+        padding=0,
+        with_header_hide=None,
+    ),
+    "mediawiki": TableFormat(
+        lineabove=Line(
+            '{| class="wikitable" style="text-align: left;"',
+            "",
+            "",
+            "\n|+ <!-- caption -->\n|-",
+        ),
+        linebelowheader=Line("|-", "", "", ""),
+        linebetweenrows=Line("|-", "", "", ""),
+        linebelow=Line("|}", "", "", ""),
+        headerrow=partial(_mediawiki_row_with_attrs, "!"),
+        datarow=partial(_mediawiki_row_with_attrs, "|"),
+        padding=0,
+        with_header_hide=None,
+    ),
+    "moinmoin": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=partial(_moin_row_with_attrs, "||", header="'''"),
+        datarow=partial(_moin_row_with_attrs, "||"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "youtrack": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("|| ", " || ", " || "),
+        datarow=DataRow("| ", " | ", " |"),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "html": TableFormat(
+        lineabove=_html_begin_table_without_header,
+        linebelowheader="",
+        linebetweenrows=None,
+        linebelow=Line("</tbody>\n</table>", "", "", ""),
+        headerrow=partial(_html_row_with_attrs, "th", False),
+        datarow=partial(_html_row_with_attrs, "td", False),
+        padding=0,
+        with_header_hide=["lineabove"],
+    ),
+    "unsafehtml": TableFormat(
+        lineabove=_html_begin_table_without_header,
+        linebelowheader="",
+        linebetweenrows=None,
+        linebelow=Line("</tbody>\n</table>", "", "", ""),
+        headerrow=partial(_html_row_with_attrs, "th", True),
+        datarow=partial(_html_row_with_attrs, "td", True),
+        padding=0,
+        with_header_hide=["lineabove"],
+    ),
+    "latex": TableFormat(
+        lineabove=_latex_line_begin_tabular,
+        linebelowheader=Line("\\hline", "", "", ""),
+        linebetweenrows=None,
+        linebelow=Line("\\hline\n\\end{tabular}", "", "", ""),
+        headerrow=_latex_row,
+        datarow=_latex_row,
+        padding=1,
+        with_header_hide=None,
+    ),
+    "latex_raw": TableFormat(
+        lineabove=_latex_line_begin_tabular,
+        linebelowheader=Line("\\hline", "", "", ""),
+        linebetweenrows=None,
+        linebelow=Line("\\hline\n\\end{tabular}", "", "", ""),
+        headerrow=partial(_latex_row, escrules={}),
+        datarow=partial(_latex_row, escrules={}),
+        padding=1,
+        with_header_hide=None,
+    ),
+    "latex_booktabs": TableFormat(
+        lineabove=partial(_latex_line_begin_tabular, booktabs=True),
+        linebelowheader=Line("\\midrule", "", "", ""),
+        linebetweenrows=None,
+        linebelow=Line("\\bottomrule\n\\end{tabular}", "", "", ""),
+        headerrow=_latex_row,
+        datarow=_latex_row,
+        padding=1,
+        with_header_hide=None,
+    ),
+    "latex_longtable": TableFormat(
+        lineabove=partial(_latex_line_begin_tabular, longtable=True),
+        linebelowheader=Line("\\hline\n\\endhead", "", "", ""),
+        linebetweenrows=None,
+        linebelow=Line("\\hline\n\\end{longtable}", "", "", ""),
+        headerrow=_latex_row,
+        datarow=_latex_row,
+        padding=1,
+        with_header_hide=None,
+    ),
+    "tsv": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("", "\t", ""),
+        datarow=DataRow("", "\t", ""),
+        padding=0,
+        with_header_hide=None,
+    ),
+    "textile": TableFormat(
+        lineabove=None,
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=None,
+        headerrow=DataRow("|_. ", "|_.", "|"),
+        datarow=_textile_row_with_attrs,
+        padding=1,
+        with_header_hide=None,
+    ),
+    "asciidoc": TableFormat(
+        lineabove=partial(_asciidoc_row, False),
+        linebelowheader=None,
+        linebetweenrows=None,
+        linebelow=Line("|====", "", "", ""),
+        headerrow=partial(_asciidoc_row, True),
+        datarow=partial(_asciidoc_row, False),
+        padding=1,
+        with_header_hide=["lineabove"],
+    ),
+}
+
+
+tabulate_formats = list(sorted(_table_formats.keys()))
+
+# The table formats for which multiline cells will be folded into subsequent
+# table rows. The key is the original format specified at the API. The value is
+# the format that will be used to represent the original format.
+multiline_formats = {
+    "plain": "plain",
+    "simple": "simple",
+    "grid": "grid",
+    "simple_grid": "simple_grid",
+    "rounded_grid": "rounded_grid",
+    "heavy_grid": "heavy_grid",
+    "mixed_grid": "mixed_grid",
+    "double_grid": "double_grid",
+    "fancy_grid": "fancy_grid",
+    "pipe": "pipe",
+    "orgtbl": "orgtbl",
+    "jira": "jira",
+    "presto": "presto",
+    "pretty": "pretty",
+    "psql": "psql",
+    "rst": "rst",
+    "outline": "outline",
+    "simple_outline": "simple_outline",
+    "rounded_outline": "rounded_outline",
+    "heavy_outline": "heavy_outline",
+    "mixed_outline": "mixed_outline",
+    "double_outline": "double_outline",
+    "fancy_outline": "fancy_outline",
+}
+
+# TODO: Add multiline support for the remaining table formats:
+#       - mediawiki: Replace \n with <br>
+#       - moinmoin: TBD
+#       - youtrack: TBD
+#       - html: Replace \n with <br>
+#       - latex*: Use "makecell" package: In header, replace X\nY with
+#         \thead{X\\Y} and in data row, replace X\nY with \makecell{X\\Y}
+#       - tsv: TBD
+#       - textile: Replace \n with <br/> (must be well-formed XML)
+
+_multiline_codes = re.compile(r"\r|\n|\r\n")
+_multiline_codes_bytes = re.compile(b"\r|\n|\r\n")
+
+# Handle ANSI escape sequences for both control sequence introducer (CSI) and
+# operating system command (OSC). Both of these begin with 0x1b (or octal 033),
+# which will be shown below as ESC.
+#
+# CSI ANSI escape codes have the following format, defined in section 5.4 of ECMA-48:
+#
+# CSI: ESC followed by the '[' character (0x5b)
+# Parameter Bytes: 0..n bytes in the range 0x30-0x3f
+# Intermediate Bytes: 0..n bytes in the range 0x20-0x2f
+# Final Byte: a single byte in the range 0x40-0x7e
+#
+# Also include the terminal hyperlink sequences as described here:
+# https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
+#
+# OSC 8 ; params ; uri ST display_text OSC 8 ;; ST
+#
+# Example: \x1b]8;;https://example.com\x5ctext to show\x1b]8;;\x5c
+#
+# Where:
+# OSC: ESC followed by the ']' character (0x5d)
+# params: 0..n optional key value pairs separated by ':' (e.g. foo=bar:baz=qux:abc=123)
+# URI: the actual URI with protocol scheme (e.g. https://, file://, ftp://)
+# ST: ESC followed by the '\' character (0x5c)
+_esc = r"\x1b"
+_csi = rf"{_esc}\["
+_osc = rf"{_esc}\]"
+_st = rf"{_esc}\\"
+
+_ansi_escape_pat = rf"""
+    (
+        # terminal colors, etc
+        {_csi}        # CSI
+        [\x30-\x3f]*  # parameter bytes
+        [\x20-\x2f]*  # intermediate bytes
+        [\x40-\x7e]   # final byte
+    |
+        # terminal hyperlinks
+        {_osc}8;        # OSC opening
+        (\w+=\w+:?)*    # key=value params list (submatch 2)
+        ;               # delimiter
+        ([^{_esc}]+)    # URI - anything but ESC (submatch 3)
+        {_st}           # ST
+        ([^{_esc}]+)    # link text - anything but ESC (submatch 4)
+        {_osc}8;;{_st}  # "closing" OSC sequence
+    )
+"""
+_ansi_codes = re.compile(_ansi_escape_pat, re.VERBOSE)
+_ansi_codes_bytes = re.compile(_ansi_escape_pat.encode("utf8"), re.VERBOSE)
+_ansi_color_reset_code = "\033[0m"
+
+_float_with_thousands_separators = re.compile(
+    r"^(([+-]?[0-9]{1,3})(?:,([0-9]{3}))*)?(?(1)\.[0-9]*|\.[0-9]+)?$"
+)
+
+
+def simple_separated_format(separator):
+    """Construct a simple TableFormat with columns separated by a separator.
+
+    >>> tsv = simple_separated_format("\\t") ; \
+        tabulate([["foo", 1], ["spam", 23]], tablefmt=tsv) == 'foo \\t 1\\nspam\\t23'
+    True
+
+    """
+    return TableFormat(
+        None,
+        None,
+        None,
+        None,
+        headerrow=DataRow("", separator, ""),
+        datarow=DataRow("", separator, ""),
+        padding=0,
+        with_header_hide=None,
+    )
+
+
+def _isnumber_with_thousands_separator(string):
+    """
+    >>> _isnumber_with_thousands_separator(".")
+    False
+    >>> _isnumber_with_thousands_separator("1")
+    True
+    >>> _isnumber_with_thousands_separator("1.")
+    True
+    >>> _isnumber_with_thousands_separator(".1")
+    True
+    >>> _isnumber_with_thousands_separator("1000")
+    False
+    >>> _isnumber_with_thousands_separator("1,000")
+    True
+    >>> _isnumber_with_thousands_separator("1,0000")
+    False
+    >>> _isnumber_with_thousands_separator("1,000.1234")
+    True
+    >>> _isnumber_with_thousands_separator(b"1,000.1234")
+    True
+    >>> _isnumber_with_thousands_separator("+1,000.1234")
+    True
+    >>> _isnumber_with_thousands_separator("-1,000.1234")
+    True
+    """
+    try:
+        string = string.decode()
+    except (UnicodeDecodeError, AttributeError):
+        pass
+
+    return bool(re.match(_float_with_thousands_separators, string))
+
+
+def _isconvertible(conv, string):
+    try:
+        conv(string)
+        return True
+    except (ValueError, TypeError):
+        return False
+
+
+def _isnumber(string):
+    """
+    >>> _isnumber("123.45")
+    True
+    >>> _isnumber("123")
+    True
+    >>> _isnumber("spam")
+    False
+    >>> _isnumber("123e45678")
+    False
+    >>> _isnumber("inf")
+    True
+    """
+    if not _isconvertible(float, string):
+        return False
+    elif isinstance(string, (str, bytes)) and (
+        math.isinf(float(string)) or math.isnan(float(string))
+    ):
+        return string.lower() in ["inf", "-inf", "nan"]
+    return True
+
+
+def _isint(string, inttype=int):
+    """
+    >>> _isint("123")
+    True
+    >>> _isint("123.45")
+    False
+    """
+    return (
+        type(string) is inttype
+        or (
+            (hasattr(string, "is_integer") or hasattr(string, "__array__"))
+            and str(type(string)).startswith("<class 'numpy.int")
+        )  # numpy.int64 and similar
+        or (
+            isinstance(string, (bytes, str)) and _isconvertible(inttype, string)
+        )  # integer as string
+    )
+
+
+def _isbool(string):
+    """
+    >>> _isbool(True)
+    True
+    >>> _isbool("False")
+    True
+    >>> _isbool(1)
+    False
+    """
+    return type(string) is bool or (
+        isinstance(string, (bytes, str)) and string in ("True", "False")
+    )
+
+
+def _type(string, has_invisible=True, numparse=True):
+    """The least generic type (type(None), int, float, str, unicode).
+
+    >>> _type(None) is type(None)
+    True
+    >>> _type("foo") is type("")
+    True
+    >>> _type("1") is type(1)
+    True
+    >>> _type('\x1b[31m42\x1b[0m') is type(42)
+    True
+    >>> _type('\x1b[31m42\x1b[0m') is type(42)
+    True
+
+    """
+
+    if has_invisible and isinstance(string, (str, bytes)):
+        string = _strip_ansi(string)
+
+    if string is None:
+        return type(None)
+    elif hasattr(string, "isoformat"):  # datetime.datetime, date, and time
+        return str
+    elif _isbool(string):
+        return bool
+    elif _isint(string) and numparse:
+        return int
+    elif _isnumber(string) and numparse:
+        return float
+    elif isinstance(string, bytes):
+        return bytes
+    else:
+        return str
+
+
+def _afterpoint(string):
+    """Symbols after a decimal point, -1 if the string lacks the decimal point.
+
+    >>> _afterpoint("123.45")
+    2
+    >>> _afterpoint("1001")
+    -1
+    >>> _afterpoint("eggs")
+    -1
+    >>> _afterpoint("123e45")
+    2
+    >>> _afterpoint("123,456.78")
+    2
+
+    """
+    if _isnumber(string) or _isnumber_with_thousands_separator(string):
+        if _isint(string):
+            return -1
+        else:
+            pos = string.rfind(".")
+            pos = string.lower().rfind("e") if pos < 0 else pos
+            if pos >= 0:
+                return len(string) - pos - 1
+            else:
+                return -1  # no point
+    else:
+        return -1  # not a number
+
+
+def _padleft(width, s):
+    """Flush right.
+
+    >>> _padleft(6, '\u044f\u0439\u0446\u0430') == '  \u044f\u0439\u0446\u0430'
+    True
+
+    """
+    fmt = "{0:>%ds}" % width
+    return fmt.format(s)
+
+
+def _padright(width, s):
+    """Flush left.
+
+    >>> _padright(6, '\u044f\u0439\u0446\u0430') == '\u044f\u0439\u0446\u0430  '
+    True
+
+    """
+    fmt = "{0:<%ds}" % width
+    return fmt.format(s)
+
+
+def _padboth(width, s):
+    """Center string.
+
+    >>> _padboth(6, '\u044f\u0439\u0446\u0430') == ' \u044f\u0439\u0446\u0430 '
+    True
+
+    """
+    fmt = "{0:^%ds}" % width
+    return fmt.format(s)
+
+
+def _padnone(ignore_width, s):
+    return s
+
+
+def _strip_ansi(s):
+    r"""Remove ANSI escape sequences, both CSI (color codes, etc) and OSC hyperlinks.
+
+    CSI sequences are simply removed from the output, while OSC hyperlinks are replaced
+    with the link text. Note: it may be desirable to show the URI instead but this is not
+    supported.
+
+    >>> repr(_strip_ansi('\x1B]8;;https://example.com\x1B\\This is a link\x1B]8;;\x1B\\'))
+    "'This is a link'"
+
+    >>> repr(_strip_ansi('\x1b[31mred\x1b[0m text'))
+    "'red text'"
+
+    """
+    if isinstance(s, str):
+        return _ansi_codes.sub(r"\4", s)
+    else:  # a bytestring
+        return _ansi_codes_bytes.sub(r"\4", s)
+
+
+def _visible_width(s):
+    """Visible width of a printed string. ANSI color codes are removed.
+
+    >>> _visible_width('\x1b[31mhello\x1b[0m'), _visible_width("world")
+    (5, 5)
+
+    """
+    # optional wide-character support
+    if wcwidth is not None and WIDE_CHARS_MODE:
+        len_fn = wcwidth.wcswidth
+    else:
+        len_fn = len
+    if isinstance(s, (str, bytes)):
+        return len_fn(_strip_ansi(s))
+    else:
+        return len_fn(str(s))
+
+
+def _is_multiline(s):
+    if isinstance(s, str):
+        return bool(re.search(_multiline_codes, s))
+    else:  # a bytestring
+        return bool(re.search(_multiline_codes_bytes, s))
+
+
+def _multiline_width(multiline_s, line_width_fn=len):
+    """Visible width of a potentially multiline content."""
+    return max(map(line_width_fn, re.split("[\r\n]", multiline_s)))
+
+
+def _choose_width_fn(has_invisible, enable_widechars, is_multiline):
+    """Return a function to calculate visible cell width."""
+    if has_invisible:
+        line_width_fn = _visible_width
+    elif enable_widechars:  # optional wide-character support if available
+        line_width_fn = wcwidth.wcswidth
+    else:
+        line_width_fn = len
+    if is_multiline:
+        width_fn = lambda s: _multiline_width(s, line_width_fn)  # noqa
+    else:
+        width_fn = line_width_fn
+    return width_fn
+
+
+def _align_column_choose_padfn(strings, alignment, has_invisible):
+    if alignment == "right":
+        if not PRESERVE_WHITESPACE:
+            strings = [s.strip() for s in strings]
+        padfn = _padleft
+    elif alignment == "center":
+        if not PRESERVE_WHITESPACE:
+            strings = [s.strip() for s in strings]
+        padfn = _padboth
+    elif alignment == "decimal":
+        if has_invisible:
+            decimals = [_afterpoint(_strip_ansi(s)) for s in strings]
+        else:
+            decimals = [_afterpoint(s) for s in strings]
+        maxdecimals = max(decimals)
+        strings = [s + (maxdecimals - decs) * " " for s, decs in zip(strings, decimals)]
+        padfn = _padleft
+    elif not alignment:
+        padfn = _padnone
+    else:
+        if not PRESERVE_WHITESPACE:
+            strings = [s.strip() for s in strings]
+        padfn = _padright
+    return strings, padfn
+
+
+def _align_column_choose_width_fn(has_invisible, enable_widechars, is_multiline):
+    if has_invisible:
+        line_width_fn = _visible_width
+    elif enable_widechars:  # optional wide-character support if available
+        line_width_fn = wcwidth.wcswidth
+    else:
+        line_width_fn = len
+    if is_multiline:
+        width_fn = lambda s: _align_column_multiline_width(s, line_width_fn)  # noqa
+    else:
+        width_fn = line_width_fn
+    return width_fn
+
+
+def _align_column_multiline_width(multiline_s, line_width_fn=len):
+    """Visible width of a potentially multiline content."""
+    return list(map(line_width_fn, re.split("[\r\n]", multiline_s)))
+
+
+def _flat_list(nested_list):
+    ret = []
+    for item in nested_list:
+        if isinstance(item, list):
+            for subitem in item:
+                ret.append(subitem)
+        else:
+            ret.append(item)
+    return ret
+
+
+def _align_column(
+    strings,
+    alignment,
+    minwidth=0,
+    has_invisible=True,
+    enable_widechars=False,
+    is_multiline=False,
+):
+    """[string] -> [padded_string]"""
+    strings, padfn = _align_column_choose_padfn(strings, alignment, has_invisible)
+    width_fn = _align_column_choose_width_fn(
+        has_invisible, enable_widechars, is_multiline
+    )
+
+    s_widths = list(map(width_fn, strings))
+    maxwidth = max(max(_flat_list(s_widths)), minwidth)
+    # TODO: refactor column alignment in single-line and multiline modes
+    if is_multiline:
+        if not enable_widechars and not has_invisible:
+            padded_strings = [
+                "\n".join([padfn(maxwidth, s) for s in ms.splitlines()])
+                for ms in strings
+            ]
+        else:
+            # enable wide-character width corrections
+            s_lens = [[len(s) for s in re.split("[\r\n]", ms)] for ms in strings]
+            visible_widths = [
+                [maxwidth - (w - l) for w, l in zip(mw, ml)]
+                for mw, ml in zip(s_widths, s_lens)
+            ]
+            # wcswidth and _visible_width don't count invisible characters;
+            # padfn doesn't need to apply another correction
+            padded_strings = [
+                "\n".join([padfn(w, s) for s, w in zip((ms.splitlines() or ms), mw)])
+                for ms, mw in zip(strings, visible_widths)
+            ]
+    else:  # single-line cell values
+        if not enable_widechars and not has_invisible:
+            padded_strings = [padfn(maxwidth, s) for s in strings]
+        else:
+            # enable wide-character width corrections
+            s_lens = list(map(len, strings))
+            visible_widths = [maxwidth - (w - l) for w, l in zip(s_widths, s_lens)]
+            # wcswidth and _visible_width don't count invisible characters;
+            # padfn doesn't need to apply another correction
+            padded_strings = [padfn(w, s) for s, w in zip(strings, visible_widths)]
+    return padded_strings
+
+
+def _more_generic(type1, type2):
+    types = {
+        type(None): 0,
+        bool: 1,
+        int: 2,
+        float: 3,
+        bytes: 4,
+        str: 5,
+    }
+    invtypes = {
+        5: str,
+        4: bytes,
+        3: float,
+        2: int,
+        1: bool,
+        0: type(None),
+    }
+    moregeneric = max(types.get(type1, 5), types.get(type2, 5))
+    return invtypes[moregeneric]
+
+
+def _column_type(strings, has_invisible=True, numparse=True):
+    """The least generic type all column values are convertible to.
+
+    >>> _column_type([True, False]) is bool
+    True
+    >>> _column_type(["1", "2"]) is int
+    True
+    >>> _column_type(["1", "2.3"]) is float
+    True
+    >>> _column_type(["1", "2.3", "four"]) is str
+    True
+    >>> _column_type(["four", '\u043f\u044f\u0442\u044c']) is str
+    True
+    >>> _column_type([None, "brux"]) is str
+    True
+    >>> _column_type([1, 2, None]) is int
+    True
+    >>> import datetime as dt
+    >>> _column_type([dt.datetime(1991,2,19), dt.time(17,35)]) is str
+    True
+
+    """
+    types = [_type(s, has_invisible, numparse) for s in strings]
+    return reduce(_more_generic, types, bool)
+
+
+def _format(val, valtype, floatfmt, intfmt, missingval="", has_invisible=True):
+    """Format a value according to its type.
+
+    Unicode is supported:
+
+    >>> hrow = ['\u0431\u0443\u043a\u0432\u0430', '\u0446\u0438\u0444\u0440\u0430'] ; \
+        tbl = [['\u0430\u0437', 2], ['\u0431\u0443\u043a\u0438', 4]] ; \
+        good_result = '\\u0431\\u0443\\u043a\\u0432\\u0430      \\u0446\\u0438\\u0444\\u0440\\u0430\\n-------  -------\\n\\u0430\\u0437             2\\n\\u0431\\u0443\\u043a\\u0438           4' ; \
+        tabulate(tbl, headers=hrow) == good_result
+    True
+
+    """  # noqa
+    if val is None:
+        return missingval
+
+    if valtype is str:
+        return f"{val}"
+    elif valtype is int:
+        return format(val, intfmt)
+    elif valtype is bytes:
+        try:
+            return str(val, "ascii")
+        except (TypeError, UnicodeDecodeError):
+            return str(val)
+    elif valtype is float:
+        is_a_colored_number = has_invisible and isinstance(val, (str, bytes))
+        if is_a_colored_number:
+            raw_val = _strip_ansi(val)
+            formatted_val = format(float(raw_val), floatfmt)
+            return val.replace(raw_val, formatted_val)
+        else:
+            return format(float(val), floatfmt)
+    else:
+        return f"{val}"
+
+
+def _align_header(
+    header, alignment, width, visible_width, is_multiline=False, width_fn=None
+):
+    "Pad string header to width chars given known visible_width of the header."
+    if is_multiline:
+        header_lines = re.split(_multiline_codes, header)
+        padded_lines = [
+            _align_header(h, alignment, width, width_fn(h)) for h in header_lines
+        ]
+        return "\n".join(padded_lines)
+    # else: not multiline
+    ninvisible = len(header) - visible_width
+    width += ninvisible
+    if alignment == "left":
+        return _padright(width, header)
+    elif alignment == "center":
+        return _padboth(width, header)
+    elif not alignment:
+        return f"{header}"
+    else:
+        return _padleft(width, header)
+
+
+def _remove_separating_lines(rows):
+    if type(rows) == list:
+        separating_lines = []
+        sans_rows = []
+        for index, row in enumerate(rows):
+            if _is_separating_line(row):
+                separating_lines.append(index)
+            else:
+                sans_rows.append(row)
+        return sans_rows, separating_lines
+    else:
+        return rows, None
+
+
+def _reinsert_separating_lines(rows, separating_lines):
+    if separating_lines:
+        for index in separating_lines:
+            rows.insert(index, SEPARATING_LINE)
+
+
+def _prepend_row_index(rows, index):
+    """Add a left-most index column."""
+    if index is None or index is False:
+        return rows
+    if isinstance(index, Sized) and len(index) != len(rows):
+        raise ValueError(
+            "index must be as long as the number of data rows: "
+            + "len(index)={} len(rows)={}".format(len(index), len(rows))
+        )
+    sans_rows, separating_lines = _remove_separating_lines(rows)
+    new_rows = []
+    index_iter = iter(index)
+    for row in sans_rows:
+        index_v = next(index_iter)
+        new_rows.append([index_v] + list(row))
+    rows = new_rows
+    _reinsert_separating_lines(rows, separating_lines)
+    return rows
+
+
+def _bool(val):
+    "A wrapper around standard bool() which doesn't throw on NumPy arrays"
+    try:
+        return bool(val)
+    except ValueError:  # val is likely to be a numpy array with many elements
+        return False
+
+
+def _normalize_tabular_data(tabular_data, headers, showindex="default"):
+    """Transform a supported data type to a list of lists, and a list of headers, with headers padding.
+
+    Supported tabular data types:
+
+    * list-of-lists or another iterable of iterables
+
+    * list of named tuples (usually used with headers="keys")
+
+    * list of dicts (usually used with headers="keys")
+
+    * list of OrderedDicts (usually used with headers="keys")
+
+    * list of dataclasses (Python 3.7+ only, usually used with headers="keys")
+
+    * 2D NumPy arrays
+
+    * NumPy record arrays (usually used with headers="keys")
+
+    * dict of iterables (usually used with headers="keys")
+
+    * pandas.DataFrame (usually used with headers="keys")
+
+    The first row can be used as headers if headers="firstrow",
+    column indices can be used as headers if headers="keys".
+
+    If showindex="default", show row indices of the pandas.DataFrame.
+    If showindex="always", show row indices for all types of data.
+    If showindex="never", don't show row indices for all types of data.
+    If showindex is an iterable, show its values as row indices.
+
+    """
+
+    try:
+        bool(headers)
+        is_headers2bool_broken = False  # noqa
+    except ValueError:  # numpy.ndarray, pandas.core.index.Index, ...
+        is_headers2bool_broken = True  # noqa
+        headers = list(headers)
+
+    index = None
+    if hasattr(tabular_data, "keys") and hasattr(tabular_data, "values"):
+        # dict-like and pandas.DataFrame?
+        if hasattr(tabular_data.values, "__call__"):
+            # likely a conventional dict
+            keys = tabular_data.keys()
+            rows = list(
+                izip_longest(*tabular_data.values())
+            )  # columns have to be transposed
+        elif hasattr(tabular_data, "index"):
+            # values is a property, has .index => it's likely a pandas.DataFrame (pandas 0.11.0)
+            keys = list(tabular_data)
+            if (
+                showindex in ["default", "always", True]
+                and tabular_data.index.name is not None
+            ):
+                if isinstance(tabular_data.index.name, list):
+                    keys[:0] = tabular_data.index.name
+                else:
+                    keys[:0] = [tabular_data.index.name]
+            vals = tabular_data.values  # values matrix doesn't need to be transposed
+            # for DataFrames add an index per default
+            index = list(tabular_data.index)
+            rows = [list(row) for row in vals]
+        else:
+            raise ValueError("tabular data doesn't appear to be a dict or a DataFrame")
+
+        if headers == "keys":
+            headers = list(map(str, keys))  # headers should be strings
+
+    else:  # it's a usual iterable of iterables, or a NumPy array, or an iterable of dataclasses
+        rows = list(tabular_data)
+
+        if headers == "keys" and not rows:
+            # an empty table (issue #81)
+            headers = []
+        elif (
+            headers == "keys"
+            and hasattr(tabular_data, "dtype")
+            and getattr(tabular_data.dtype, "names")
+        ):
+            # numpy record array
+            headers = tabular_data.dtype.names
+        elif (
+            headers == "keys"
+            and len(rows) > 0
+            and isinstance(rows[0], tuple)
+            and hasattr(rows[0], "_fields")
+        ):
+            # namedtuple
+            headers = list(map(str, rows[0]._fields))
+        elif len(rows) > 0 and hasattr(rows[0], "keys") and hasattr(rows[0], "values"):
+            # dict-like object
+            uniq_keys = set()  # implements hashed lookup
+            keys = []  # storage for set
+            if headers == "firstrow":
+                firstdict = rows[0] if len(rows) > 0 else {}
+                keys.extend(firstdict.keys())
+                uniq_keys.update(keys)
+                rows = rows[1:]
+            for row in rows:
+                for k in row.keys():
+                    # Save unique items in input order
+                    if k not in uniq_keys:
+                        keys.append(k)
+                        uniq_keys.add(k)
+            if headers == "keys":
+                headers = keys
+            elif isinstance(headers, dict):
+                # a dict of headers for a list of dicts
+                headers = [headers.get(k, k) for k in keys]
+                headers = list(map(str, headers))
+            elif headers == "firstrow":
+                if len(rows) > 0:
+                    headers = [firstdict.get(k, k) for k in keys]
+                    headers = list(map(str, headers))
+                else:
+                    headers = []
+            elif headers:
+                raise ValueError(
+                    "headers for a list of dicts is not a dict or a keyword"
+                )
+            rows = [[row.get(k) for k in keys] for row in rows]
+
+        elif (
+            headers == "keys"
+            and hasattr(tabular_data, "description")
+            and hasattr(tabular_data, "fetchone")
+            and hasattr(tabular_data, "rowcount")
+        ):
+            # Python Database API cursor object (PEP 0249)
+            # print tabulate(cursor, headers='keys')
+            headers = [column[0] for column in tabular_data.description]
+
+        elif (
+            dataclasses is not None
+            and len(rows) > 0
+            and dataclasses.is_dataclass(rows[0])
+        ):
+            # Python 3.7+'s dataclass
+            field_names = [field.name for field in dataclasses.fields(rows[0])]
+            if headers == "keys":
+                headers = field_names
+            rows = [[getattr(row, f) for f in field_names] for row in rows]
+
+        elif headers == "keys" and len(rows) > 0:
+            # keys are column indices
+            headers = list(map(str, range(len(rows[0]))))
+
+    # take headers from the first row if necessary
+    if headers == "firstrow" and len(rows) > 0:
+        if index is not None:
+            headers = [index[0]] + list(rows[0])
+            index = index[1:]
+        else:
+            headers = rows[0]
+        headers = list(map(str, headers))  # headers should be strings
+        rows = rows[1:]
+    elif headers == "firstrow":
+        headers = []
+
+    headers = list(map(str, headers))
+    #    rows = list(map(list, rows))
+    rows = list(map(lambda r: r if _is_separating_line(r) else list(r), rows))
+
+    # add or remove an index column
+    showindex_is_a_str = type(showindex) in [str, bytes]
+    if showindex == "default" and index is not None:
+        rows = _prepend_row_index(rows, index)
+    elif isinstance(showindex, Sized) and not showindex_is_a_str:
+        rows = _prepend_row_index(rows, list(showindex))
+    elif isinstance(showindex, Iterable) and not showindex_is_a_str:
+        rows = _prepend_row_index(rows, showindex)
+    elif showindex == "always" or (_bool(showindex) and not showindex_is_a_str):
+        if index is None:
+            index = list(range(len(rows)))
+        rows = _prepend_row_index(rows, index)
+    elif showindex == "never" or (not _bool(showindex) and not showindex_is_a_str):
+        pass
+
+    # pad with empty headers for initial columns if necessary
+    headers_pad = 0
+    if headers and len(rows) > 0:
+        headers_pad = max(0, len(rows[0]) - len(headers))
+        headers = [""] * headers_pad + headers
+
+    return rows, headers, headers_pad
+
+
+def _wrap_text_to_colwidths(list_of_lists, colwidths, numparses=True):
+    if len(list_of_lists):
+        num_cols = len(list_of_lists[0])
+    else:
+        num_cols = 0
+    numparses = _expand_iterable(numparses, num_cols, True)
+
+    result = []
+
+    for row in list_of_lists:
+        new_row = []
+        for cell, width, numparse in zip(row, colwidths, numparses):
+            if _isnumber(cell) and numparse:
+                new_row.append(cell)
+                continue
+
+            if width is not None:
+                wrapper = _CustomTextWrap(width=width)
+                # Cast based on our internal type handling
+                # Any future custom formatting of types (such as datetimes)
+                # may need to be more explicit than just `str` of the object
+                casted_cell = (
+                    str(cell) if _isnumber(cell) else _type(cell, numparse)(cell)
+                )
+                wrapped = [
+                    "\n".join(wrapper.wrap(line))
+                    for line in casted_cell.splitlines()
+                    if line.strip() != ""
+                ]
+                new_row.append("\n".join(wrapped))
+            else:
+                new_row.append(cell)
+        result.append(new_row)
+
+    return result
+
+
+def _to_str(s, encoding="utf8", errors="ignore"):
+    """
+    A type safe wrapper for converting a bytestring to str. This is essentially just
+    a wrapper around .decode() intended for use with things like map(), but with some
+    specific behavior:
+
+    1. if the given parameter is not a bytestring, it is returned unmodified
+    2. decode() is called for the given parameter and assumes utf8 encoding, but the
+       default error behavior is changed from 'strict' to 'ignore'
+
+    >>> repr(_to_str(b'foo'))
+    "'foo'"
+
+    >>> repr(_to_str('foo'))
+    "'foo'"
+
+    >>> repr(_to_str(42))
+    "'42'"
+
+    """
+    if isinstance(s, bytes):
+        return s.decode(encoding=encoding, errors=errors)
+    return str(s)
+
+
+def tabulate(
+    tabular_data,
+    headers=(),
+    tablefmt="simple",
+    floatfmt=_DEFAULT_FLOATFMT,
+    intfmt=_DEFAULT_INTFMT,
+    numalign=_DEFAULT_ALIGN,
+    stralign=_DEFAULT_ALIGN,
+    missingval=_DEFAULT_MISSINGVAL,
+    showindex="default",
+    disable_numparse=False,
+    colglobalalign=None,
+    colalign=None,
+    maxcolwidths=None,
+    headersglobalalign=None,
+    headersalign=None,
+    rowalign=None,
+    maxheadercolwidths=None,
+):
+    """Format a fixed width table for pretty printing.
+
+    >>> print(tabulate([[1, 2.34], [-56, "8.999"], ["2", "10001"]]))
+    ---  ---------
+      1      2.34
+    -56      8.999
+      2  10001
+    ---  ---------
+
+    The first required argument (`tabular_data`) can be a
+    list-of-lists (or another iterable of iterables), a list of named
+    tuples, a dictionary of iterables, an iterable of dictionaries,
+    an iterable of dataclasses (Python 3.7+), a two-dimensional NumPy array,
+    NumPy record array, or a Pandas' dataframe.
+
+
+    Table headers
+    -------------
+
+    To print nice column headers, supply the second argument (`headers`):
+
+      - `headers` can be an explicit list of column headers
+      - if `headers="firstrow"`, then the first row of data is used
+      - if `headers="keys"`, then dictionary keys or column indices are used
+
+    Otherwise a headerless table is produced.
+
+    If the number of headers is less than the number of columns, they
+    are supposed to be names of the last columns. This is consistent
+    with the plain-text format of R and Pandas' dataframes.
+
+    >>> print(tabulate([["sex","age"],["Alice","F",24],["Bob","M",19]],
+    ...       headers="firstrow"))
+           sex      age
+    -----  -----  -----
+    Alice  F         24
+    Bob    M         19
+
+    By default, pandas.DataFrame data have an additional column called
+    row index. To add a similar column to all other types of data,
+    use `showindex="always"` or `showindex=True`. To suppress row indices
+    for all types of data, pass `showindex="never" or `showindex=False`.
+    To add a custom row index column, pass `showindex=some_iterable`.
+
+    >>> print(tabulate([["F",24],["M",19]], showindex="always"))
+    -  -  --
+    0  F  24
+    1  M  19
+    -  -  --
+
+
+    Column and Headers alignment
+    ----------------------------
+
+    `tabulate` tries to detect column types automatically, and aligns
+    the values properly. By default it aligns decimal points of the
+    numbers (or flushes integer numbers to the right), and flushes
+    everything else to the left. Possible column alignments
+    (`numalign`, `stralign`) are: "right", "center", "left", "decimal"
+    (only for `numalign`), and None (to disable alignment).
+
+    `colglobalalign` allows for global alignment of columns, before any
+        specific override from `colalign`. Possible values are: None
+        (defaults according to coltype), "right", "center", "decimal",
+        "left".
+    `colalign` allows for column-wise override starting from left-most
+        column. Possible values are: "global" (no override), "right",
+        "center", "decimal", "left".
+    `headersglobalalign` allows for global headers alignment, before any
+        specific override from `headersalign`. Possible values are: None
+        (follow columns alignment), "right", "center", "left".
+    `headersalign` allows for header-wise override starting from left-most
+        given header. Possible values are: "global" (no override), "same"
+        (follow column alignment), "right", "center", "left".
+
+    Note on intended behaviour: If there is no `tabular_data`, any column
+        alignment argument is ignored. Hence, in this case, header
+        alignment cannot be inferred from column alignment.
+
+    Table formats
+    -------------
+
+    `intfmt` is a format specification used for columns which
+    contain numeric data without a decimal point. This can also be
+    a list or tuple of format strings, one per column.
+
+    `floatfmt` is a format specification used for columns which
+    contain numeric data with a decimal point. This can also be
+    a list or tuple of format strings, one per column.
+
+    `None` values are replaced with a `missingval` string (like
+    `floatfmt`, this can also be a list of values for different
+    columns):
+
+    >>> print(tabulate([["spam", 1, None],
+    ...                 ["eggs", 42, 3.14],
+    ...                 ["other", None, 2.7]], missingval="?"))
+    -----  --  ----
+    spam    1  ?
+    eggs   42  3.14
+    other   ?  2.7
+    -----  --  ----
+
+    Various plain-text table formats (`tablefmt`) are supported:
+    'plain', 'simple', 'grid', 'pipe', 'orgtbl', 'rst', 'mediawiki',
+    'latex', 'latex_raw', 'latex_booktabs', 'latex_longtable' and tsv.
+    Variable `tabulate_formats`contains the list of currently supported formats.
+
+    "plain" format doesn't use any pseudographics to draw tables,
+    it separates columns with a double space:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                 ["strings", "numbers"], "plain"))
+    strings      numbers
+    spam         41.9999
+    eggs        451
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="plain"))
+    spam   41.9999
+    eggs  451
+
+    "simple" format is like Pandoc simple_tables:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                 ["strings", "numbers"], "simple"))
+    strings      numbers
+    ---------  ---------
+    spam         41.9999
+    eggs        451
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="simple"))
+    ----  --------
+    spam   41.9999
+    eggs  451
+    ----  --------
+
+    "grid" is similar to tables produced by Emacs table.el package or
+    Pandoc grid_tables:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "grid"))
+    +-----------+-----------+
+    | strings   |   numbers |
+    +===========+===========+
+    | spam      |   41.9999 |
+    +-----------+-----------+
+    | eggs      |  451      |
+    +-----------+-----------+
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="grid"))
+    +------+----------+
+    | spam |  41.9999 |
+    +------+----------+
+    | eggs | 451      |
+    +------+----------+
+
+    "simple_grid" draws a grid using single-line box-drawing
+    characters:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "simple_grid"))
+    ┌───────────┬───────────┐
+    │ strings   │   numbers │
+    ├───────────┼───────────┤
+    │ spam      │   41.9999 │
+    ├───────────┼───────────┤
+    │ eggs      │  451      │
+    └───────────┴───────────┘
+
+    "rounded_grid" draws a grid using single-line box-drawing
+    characters with rounded corners:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "rounded_grid"))
+    ╭───────────┬───────────╮
+    │ strings   │   numbers │
+    ├───────────┼───────────┤
+    │ spam      │   41.9999 │
+    ├───────────┼───────────┤
+    │ eggs      │  451      │
+    ╰───────────┴───────────╯
+
+    "heavy_grid" draws a grid using bold (thick) single-line box-drawing
+    characters:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "heavy_grid"))
+    ┏━━━━━━━━━━━┳━━━━━━━━━━━┓
+    ┃ strings   ┃   numbers ┃
+    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
+    ┃ spam      ┃   41.9999 ┃
+    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
+    ┃ eggs      ┃  451      ┃
+    ┗━━━━━━━━━━━┻━━━━━━━━━━━┛
+
+    "mixed_grid" draws a grid using a mix of light (thin) and heavy (thick) lines
+    box-drawing characters:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "mixed_grid"))
+    ┍━━━━━━━━━━━┯━━━━━━━━━━━┑
+    │ strings   │   numbers │
+    ┝━━━━━━━━━━━┿━━━━━━━━━━━┥
+    │ spam      │   41.9999 │
+    ├───────────┼───────────┤
+    │ eggs      │  451      │
+    ┕━━━━━━━━━━━┷━━━━━━━━━━━┙
+
+    "double_grid" draws a grid using double-line box-drawing
+    characters:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "double_grid"))
+    ╔═══════════╦═══════════╗
+    ║ strings   ║   numbers ║
+    ╠═══════════╬═══════════╣
+    ║ spam      ║   41.9999 ║
+    ╠═══════════╬═══════════╣
+    ║ eggs      ║  451      ║
+    ╚═══════════╩═══════════╝
+
+    "fancy_grid" draws a grid using a mix of single and
+    double-line box-drawing characters:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "fancy_grid"))
+    ╒═══════════╤═══════════╕
+    │ strings   │   numbers │
+    ╞═══════════╪═══════════╡
+    │ spam      │   41.9999 │
+    ├───────────┼───────────┤
+    │ eggs      │  451      │
+    ╘═══════════╧═══════════╛
+
+    "outline" is the same as the "grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "outline"))
+    +-----------+-----------+
+    | strings   |   numbers |
+    +===========+===========+
+    | spam      |   41.9999 |
+    | eggs      |  451      |
+    +-----------+-----------+
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="outline"))
+    +------+----------+
+    | spam |  41.9999 |
+    | eggs | 451      |
+    +------+----------+
+
+    "simple_outline" is the same as the "simple_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "simple_outline"))
+    ┌───────────┬───────────┐
+    │ strings   │   numbers │
+    ├───────────┼───────────┤
+    │ spam      │   41.9999 │
+    │ eggs      │  451      │
+    └───────────┴───────────┘
+
+    "rounded_outline" is the same as the "rounded_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "rounded_outline"))
+    ╭───────────┬───────────╮
+    │ strings   │   numbers │
+    ├───────────┼───────────┤
+    │ spam      │   41.9999 │
+    │ eggs      │  451      │
+    ╰───────────┴───────────╯
+
+    "heavy_outline" is the same as the "heavy_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "heavy_outline"))
+    ┏━━━━━━━━━━━┳━━━━━━━━━━━┓
+    ┃ strings   ┃   numbers ┃
+    ┣━━━━━━━━━━━╋━━━━━━━━━━━┫
+    ┃ spam      ┃   41.9999 ┃
+    ┃ eggs      ┃  451      ┃
+    ┗━━━━━━━━━━━┻━━━━━━━━━━━┛
+
+    "mixed_outline" is the same as the "mixed_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "mixed_outline"))
+    ┍━━━━━━━━━━━┯━━━━━━━━━━━┑
+    │ strings   │   numbers │
+    ┝━━━━━━━━━━━┿━━━━━━━━━━━┥
+    │ spam      │   41.9999 │
+    │ eggs      │  451      │
+    ┕━━━━━━━━━━━┷━━━━━━━━━━━┙
+
+    "double_outline" is the same as the "double_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "double_outline"))
+    ╔═══════════╦═══════════╗
+    ║ strings   ║   numbers ║
+    ╠═══════════╬═══════════╣
+    ║ spam      ║   41.9999 ║
+    ║ eggs      ║  451      ║
+    ╚═══════════╩═══════════╝
+
+    "fancy_outline" is the same as the "fancy_grid" format but doesn't draw lines between rows:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "fancy_outline"))
+    ╒═══════════╤═══════════╕
+    │ strings   │   numbers │
+    ╞═══════════╪═══════════╡
+    │ spam      │   41.9999 │
+    │ eggs      │  451      │
+    ╘═══════════╧═══════════╛
+
+    "pipe" is like tables in PHP Markdown Extra extension or Pandoc
+    pipe_tables:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "pipe"))
+    | strings   |   numbers |
+    |:----------|----------:|
+    | spam      |   41.9999 |
+    | eggs      |  451      |
+
+    "presto" is like tables produce by the Presto CLI:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "presto"))
+     strings   |   numbers
+    -----------+-----------
+     spam      |   41.9999
+     eggs      |  451
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="pipe"))
+    |:-----|---------:|
+    | spam |  41.9999 |
+    | eggs | 451      |
+
+    "orgtbl" is like tables in Emacs org-mode and orgtbl-mode. They
+    are slightly different from "pipe" format by not using colons to
+    define column alignment, and using a "+" sign to indicate line
+    intersections:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "orgtbl"))
+    | strings   |   numbers |
+    |-----------+-----------|
+    | spam      |   41.9999 |
+    | eggs      |  451      |
+
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="orgtbl"))
+    | spam |  41.9999 |
+    | eggs | 451      |
+
+    "rst" is like a simple table format from reStructuredText; please
+    note that reStructuredText accepts also "grid" tables:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]],
+    ...                ["strings", "numbers"], "rst"))
+    =========  =========
+    strings      numbers
+    =========  =========
+    spam         41.9999
+    eggs        451
+    =========  =========
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="rst"))
+    ====  ========
+    spam   41.9999
+    eggs  451
+    ====  ========
+
+    "mediawiki" produces a table markup used in Wikipedia and on other
+    MediaWiki-based sites:
+
+    >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
+    ...                headers="firstrow", tablefmt="mediawiki"))
+    {| class="wikitable" style="text-align: left;"
+    |+ <!-- caption -->
+    |-
+    ! strings   !! style="text-align: right;"|   numbers
+    |-
+    | spam      || style="text-align: right;"|   41.9999
+    |-
+    | eggs      || style="text-align: right;"|  451
+    |}
+
+    "html" produces HTML markup as an html.escape'd str
+    with a ._repr_html_ method so that Jupyter Lab and Notebook display the HTML
+    and a .str property so that the raw HTML remains accessible
+    the unsafehtml table format can be used if an unescaped HTML format is required:
+
+    >>> print(tabulate([["strings", "numbers"], ["spam", 41.9999], ["eggs", "451.0"]],
+    ...                headers="firstrow", tablefmt="html"))
+    <table>
+    <thead>
+    <tr><th>strings  </th><th style="text-align: right;">  numbers</th></tr>
+    </thead>
+    <tbody>
+    <tr><td>spam     </td><td style="text-align: right;">  41.9999</td></tr>
+    <tr><td>eggs     </td><td style="text-align: right;"> 451     </td></tr>
+    </tbody>
+    </table>
+
+    "latex" produces a tabular environment of LaTeX document markup:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex"))
+    \\begin{tabular}{lr}
+    \\hline
+     spam &  41.9999 \\\\
+     eggs & 451      \\\\
+    \\hline
+    \\end{tabular}
+
+    "latex_raw" is similar to "latex", but doesn't escape special characters,
+    such as backslash and underscore, so LaTeX commands may embedded into
+    cells' values:
+
+    >>> print(tabulate([["spam$_9$", 41.9999], ["\\\\emph{eggs}", "451.0"]], tablefmt="latex_raw"))
+    \\begin{tabular}{lr}
+    \\hline
+     spam$_9$    &  41.9999 \\\\
+     \\emph{eggs} & 451      \\\\
+    \\hline
+    \\end{tabular}
+
+    "latex_booktabs" produces a tabular environment of LaTeX document markup
+    using the booktabs.sty package:
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_booktabs"))
+    \\begin{tabular}{lr}
+    \\toprule
+     spam &  41.9999 \\\\
+     eggs & 451      \\\\
+    \\bottomrule
+    \\end{tabular}
+
+    "latex_longtable" produces a tabular environment that can stretch along
+    multiple pages, using the longtable package for LaTeX.
+
+    >>> print(tabulate([["spam", 41.9999], ["eggs", "451.0"]], tablefmt="latex_longtable"))
+    \\begin{longtable}{lr}
+    \\hline
+     spam &  41.9999 \\\\
+     eggs & 451      \\\\
+    \\hline
+    \\end{longtable}
+
+
+    Number parsing
+    --------------
+    By default, anything which can be parsed as a number is a number.
+    This ensures numbers represented as strings are aligned properly.
+    This can lead to weird results for particular strings such as
+    specific git SHAs e.g. "42992e1" will be parsed into the number
+    429920 and aligned as such.
+
+    To completely disable number parsing (and alignment), use
+    `disable_numparse=True`. For more fine grained control, a list column
+    indices is used to disable number parsing only on those columns
+    e.g. `disable_numparse=[0, 2]` would disable number parsing only on the
+    first and third columns.
+
+    Column Widths and Auto Line Wrapping
+    ------------------------------------
+    Tabulate will, by default, set the width of each column to the length of the
+    longest element in that column. However, in situations where fields are expected
+    to reasonably be too long to look good as a single line, tabulate can help automate
+    word wrapping long fields for you. Use the parameter `maxcolwidth` to provide a
+    list of maximal column widths
+
+    >>> print(tabulate( \
+          [('1', 'John Smith', \
+            'This is a rather long description that might look better if it is wrapped a bit')], \
+          headers=("Issue Id", "Author", "Description"), \
+          maxcolwidths=[None, None, 30], \
+          tablefmt="grid"  \
+        ))
+    +------------+------------+-------------------------------+
+    |   Issue Id | Author     | Description                   |
+    +============+============+===============================+
+    |          1 | John Smith | This is a rather long         |
+    |            |            | description that might look   |
+    |            |            | better if it is wrapped a bit |
+    +------------+------------+-------------------------------+
+
+    Header column width can be specified in a similar way using `maxheadercolwidth`
+
+    """
+
+    if tabular_data is None:
+        tabular_data = []
+
+    list_of_lists, headers, headers_pad = _normalize_tabular_data(
+        tabular_data, headers, showindex=showindex
+    )
+    list_of_lists, separating_lines = _remove_separating_lines(list_of_lists)
+
+    if maxcolwidths is not None:
+        if len(list_of_lists):
+            num_cols = len(list_of_lists[0])
+        else:
+            num_cols = 0
+        if isinstance(maxcolwidths, int):  # Expand scalar for all columns
+            maxcolwidths = _expand_iterable(maxcolwidths, num_cols, maxcolwidths)
+        else:  # Ignore col width for any 'trailing' columns
+            maxcolwidths = _expand_iterable(maxcolwidths, num_cols, None)
+
+        numparses = _expand_numparse(disable_numparse, num_cols)
+        list_of_lists = _wrap_text_to_colwidths(
+            list_of_lists, maxcolwidths, numparses=numparses
+        )
+
+    if maxheadercolwidths is not None:
+        num_cols = len(list_of_lists[0])
+        if isinstance(maxheadercolwidths, int):  # Expand scalar for all columns
+            maxheadercolwidths = _expand_iterable(
+                maxheadercolwidths, num_cols, maxheadercolwidths
+            )
+        else:  # Ignore col width for any 'trailing' columns
+            maxheadercolwidths = _expand_iterable(maxheadercolwidths, num_cols, None)
+
+        numparses = _expand_numparse(disable_numparse, num_cols)
+        headers = _wrap_text_to_colwidths(
+            [headers], maxheadercolwidths, numparses=numparses
+        )[0]
+
+    # empty values in the first column of RST tables should be escaped (issue #82)
+    # "" should be escaped as "\\ " or ".."
+    if tablefmt == "rst":
+        list_of_lists, headers = _rst_escape_first_column(list_of_lists, headers)
+
+    # PrettyTable formatting does not use any extra padding.
+    # Numbers are not parsed and are treated the same as strings for alignment.
+    # Check if pretty is the format being used and override the defaults so it
+    # does not impact other formats.
+    min_padding = MIN_PADDING
+    if tablefmt == "pretty":
+        min_padding = 0
+        disable_numparse = True
+        numalign = "center" if numalign == _DEFAULT_ALIGN else numalign
+        stralign = "center" if stralign == _DEFAULT_ALIGN else stralign
+    else:
+        numalign = "decimal" if numalign == _DEFAULT_ALIGN else numalign
+        stralign = "left" if stralign == _DEFAULT_ALIGN else stralign
+
+    # optimization: look for ANSI control codes once,
+    # enable smart width functions only if a control code is found
+    #
+    # convert the headers and rows into a single, tab-delimited string ensuring
+    # that any bytestrings are decoded safely (i.e. errors ignored)
+    plain_text = "\t".join(
+        chain(
+            # headers
+            map(_to_str, headers),
+            # rows: chain the rows together into a single iterable after mapping
+            # the bytestring conversino to each cell value
+            chain.from_iterable(map(_to_str, row) for row in list_of_lists),
+        )
+    )
+
+    has_invisible = _ansi_codes.search(plain_text) is not None
+
+    enable_widechars = wcwidth is not None and WIDE_CHARS_MODE
+    if (
+        not isinstance(tablefmt, TableFormat)
+        and tablefmt in multiline_formats
+        and _is_multiline(plain_text)
+    ):
+        tablefmt = multiline_formats.get(tablefmt, tablefmt)
+        is_multiline = True
+    else:
+        is_multiline = False
+    width_fn = _choose_width_fn(has_invisible, enable_widechars, is_multiline)
+
+    # format rows and columns, convert numeric values to strings
+    cols = list(izip_longest(*list_of_lists))
+    numparses = _expand_numparse(disable_numparse, len(cols))
+    coltypes = [_column_type(col, numparse=np) for col, np in zip(cols, numparses)]
+    if isinstance(floatfmt, str):  # old version
+        float_formats = len(cols) * [
+            floatfmt
+        ]  # just duplicate the string to use in each column
+    else:  # if floatfmt is list, tuple etc we have one per column
+        float_formats = list(floatfmt)
+        if len(float_formats) < len(cols):
+            float_formats.extend((len(cols) - len(float_formats)) * [_DEFAULT_FLOATFMT])
+    if isinstance(intfmt, str):  # old version
+        int_formats = len(cols) * [
+            intfmt
+        ]  # just duplicate the string to use in each column
+    else:  # if intfmt is list, tuple etc we have one per column
+        int_formats = list(intfmt)
+        if len(int_formats) < len(cols):
+            int_formats.extend((len(cols) - len(int_formats)) * [_DEFAULT_INTFMT])
+    if isinstance(missingval, str):
+        missing_vals = len(cols) * [missingval]
+    else:
+        missing_vals = list(missingval)
+        if len(missing_vals) < len(cols):
+            missing_vals.extend((len(cols) - len(missing_vals)) * [_DEFAULT_MISSINGVAL])
+    cols = [
+        [_format(v, ct, fl_fmt, int_fmt, miss_v, has_invisible) for v in c]
+        for c, ct, fl_fmt, int_fmt, miss_v in zip(
+            cols, coltypes, float_formats, int_formats, missing_vals
+        )
+    ]
+
+    # align columns
+    # first set global alignment
+    if colglobalalign is not None: # if global alignment provided
+        aligns = [colglobalalign] * len(cols)
+    else: # default
+        aligns = [numalign if ct in [int, float] else stralign for ct in coltypes]
+    # then specific alignements
+    if colalign is not None:
+        assert isinstance(colalign, Iterable)
+        if isinstance(colalign, str):
+            warnings.warn(f"As a string, `colalign` is interpreted as {[c for c in colalign]}. Did you mean `colglobalalign = \"{colalign}\"` or `colalign = (\"{colalign}\",)`?", stacklevel=2)
+        for idx, align in enumerate(colalign):
+            if not idx < len(aligns):
+                break
+            elif align != "global":
+                aligns[idx] = align
+    minwidths = (
+        [width_fn(h) + min_padding for h in headers] if headers else [0] * len(cols)
+    )
+    cols = [
+        _align_column(c, a, minw, has_invisible, enable_widechars, is_multiline)
+        for c, a, minw in zip(cols, aligns, minwidths)
+    ]
+
+    aligns_headers = None
+    if headers:
+        # align headers and add headers
+        t_cols = cols or [[""]] * len(headers)
+        # first set global alignment
+        if headersglobalalign is not None: # if global alignment provided
+            aligns_headers = [headersglobalalign] * len(t_cols)
+        else: # default
+            aligns_headers = aligns or [stralign] * len(headers)
+        # then specific header alignements
+        if headersalign is not None:
+            assert isinstance(headersalign, Iterable)
+            if isinstance(headersalign, str):
+                warnings.warn(f"As a string, `headersalign` is interpreted as {[c for c in headersalign]}. Did you mean `headersglobalalign = \"{headersalign}\"` or `headersalign = (\"{headersalign}\",)`?", stacklevel=2)
+            for idx, align in enumerate(headersalign):
+                hidx = headers_pad + idx
+                if not hidx < len(aligns_headers):
+                    break
+                elif align == "same" and hidx < len(aligns): # same as column align
+                    aligns_headers[hidx] = aligns[hidx]
+                elif align != "global":
+                    aligns_headers[hidx] = align
+        minwidths = [
+            max(minw, max(width_fn(cl) for cl in c))
+            for minw, c in zip(minwidths, t_cols)
+        ]
+        headers = [
+            _align_header(h, a, minw, width_fn(h), is_multiline, width_fn)
+            for h, a, minw in zip(headers, aligns_headers, minwidths)
+        ]
+        rows = list(zip(*cols))
+    else:
+        minwidths = [max(width_fn(cl) for cl in c) for c in cols]
+        rows = list(zip(*cols))
+
+    if not isinstance(tablefmt, TableFormat):
+        tablefmt = _table_formats.get(tablefmt, _table_formats["simple"])
+
+    ra_default = rowalign if isinstance(rowalign, str) else None
+    rowaligns = _expand_iterable(rowalign, len(rows), ra_default)
+    _reinsert_separating_lines(rows, separating_lines)
+
+    return _format_table(
+        tablefmt, headers, aligns_headers, rows, minwidths, aligns, is_multiline, rowaligns=rowaligns
+    )
+
+
+def _expand_numparse(disable_numparse, column_count):
+    """
+    Return a list of bools of length `column_count` which indicates whether
+    number parsing should be used on each column.
+    If `disable_numparse` is a list of indices, each of those indices are False,
+    and everything else is True.
+    If `disable_numparse` is a bool, then the returned list is all the same.
+    """
+    if isinstance(disable_numparse, Iterable):
+        numparses = [True] * column_count
+        for index in disable_numparse:
+            numparses[index] = False
+        return numparses
+    else:
+        return [not disable_numparse] * column_count
+
+
+def _expand_iterable(original, num_desired, default):
+    """
+    Expands the `original` argument to return a return a list of
+    length `num_desired`. If `original` is shorter than `num_desired`, it will
+    be padded with the value in `default`.
+    If `original` is not a list to begin with (i.e. scalar value) a list of
+    length `num_desired` completely populated with `default will be returned
+    """
+    if isinstance(original, Iterable) and not isinstance(original, str):
+        return original + [default] * (num_desired - len(original))
+    else:
+        return [default] * num_desired
+
+
+def _pad_row(cells, padding):
+    if cells:
+        pad = " " * padding
+        padded_cells = [pad + cell + pad for cell in cells]
+        return padded_cells
+    else:
+        return cells
+
+
+def _build_simple_row(padded_cells, rowfmt):
+    "Format row according to DataRow format without padding."
+    begin, sep, end = rowfmt
+    return (begin + sep.join(padded_cells) + end).rstrip()
+
+
+def _build_row(padded_cells, colwidths, colaligns, rowfmt):
+    "Return a string which represents a row of data cells."
+    if not rowfmt:
+        return None
+    if hasattr(rowfmt, "__call__"):
+        return rowfmt(padded_cells, colwidths, colaligns)
+    else:
+        return _build_simple_row(padded_cells, rowfmt)
+
+
+def _append_basic_row(lines, padded_cells, colwidths, colaligns, rowfmt, rowalign=None):
+    # NOTE: rowalign is ignored and exists for api compatibility with _append_multiline_row
+    lines.append(_build_row(padded_cells, colwidths, colaligns, rowfmt))
+    return lines
+
+
+def _align_cell_veritically(text_lines, num_lines, column_width, row_alignment):
+    delta_lines = num_lines - len(text_lines)
+    blank = [" " * column_width]
+    if row_alignment == "bottom":
+        return blank * delta_lines + text_lines
+    elif row_alignment == "center":
+        top_delta = delta_lines // 2
+        bottom_delta = delta_lines - top_delta
+        return top_delta * blank + text_lines + bottom_delta * blank
+    else:
+        return text_lines + blank * delta_lines
+
+
+def _append_multiline_row(
+    lines, padded_multiline_cells, padded_widths, colaligns, rowfmt, pad, rowalign=None
+):
+    colwidths = [w - 2 * pad for w in padded_widths]
+    cells_lines = [c.splitlines() for c in padded_multiline_cells]
+    nlines = max(map(len, cells_lines))  # number of lines in the row
+    # vertically pad cells where some lines are missing
+    # cells_lines = [
+    #     (cl + [" " * w] * (nlines - len(cl))) for cl, w in zip(cells_lines, colwidths)
+    # ]
+
+    cells_lines = [
+        _align_cell_veritically(cl, nlines, w, rowalign)
+        for cl, w in zip(cells_lines, colwidths)
+    ]
+    lines_cells = [[cl[i] for cl in cells_lines] for i in range(nlines)]
+    for ln in lines_cells:
+        padded_ln = _pad_row(ln, pad)
+        _append_basic_row(lines, padded_ln, colwidths, colaligns, rowfmt)
+    return lines
+
+
+def _build_line(colwidths, colaligns, linefmt):
+    "Return a string which represents a horizontal line."
+    if not linefmt:
+        return None
+    if hasattr(linefmt, "__call__"):
+        return linefmt(colwidths, colaligns)
+    else:
+        begin, fill, sep, end = linefmt
+        cells = [fill * w for w in colwidths]
+        return _build_simple_row(cells, (begin, sep, end))
+
+
+def _append_line(lines, colwidths, colaligns, linefmt):
+    lines.append(_build_line(colwidths, colaligns, linefmt))
+    return lines
+
+
+class JupyterHTMLStr(str):
+    """Wrap the string with a _repr_html_ method so that Jupyter
+    displays the HTML table"""
+
+    def _repr_html_(self):
+        return self
+
+    @property
+    def str(self):
+        """add a .str property so that the raw string is still accessible"""
+        return self
+
+
+def _format_table(fmt, headers, headersaligns, rows, colwidths, colaligns, is_multiline, rowaligns):
+    """Produce a plain-text representation of the table."""
+    lines = []
+    hidden = fmt.with_header_hide if (headers and fmt.with_header_hide) else []
+    pad = fmt.padding
+    headerrow = fmt.headerrow
+
+    padded_widths = [(w + 2 * pad) for w in colwidths]
+    if is_multiline:
+        pad_row = lambda row, _: row  # noqa do it later, in _append_multiline_row
+        append_row = partial(_append_multiline_row, pad=pad)
+    else:
+        pad_row = _pad_row
+        append_row = _append_basic_row
+
+    padded_headers = pad_row(headers, pad)
+    padded_rows = [pad_row(row, pad) for row in rows]
+
+    if fmt.lineabove and "lineabove" not in hidden:
+        _append_line(lines, padded_widths, colaligns, fmt.lineabove)
+
+    if padded_headers:
+        append_row(lines, padded_headers, padded_widths, headersaligns, headerrow)
+        if fmt.linebelowheader and "linebelowheader" not in hidden:
+            _append_line(lines, padded_widths, colaligns, fmt.linebelowheader)
+
+    if padded_rows and fmt.linebetweenrows and "linebetweenrows" not in hidden:
+        # initial rows with a line below
+        for row, ralign in zip(padded_rows[:-1], rowaligns):
+            append_row(
+                lines, row, padded_widths, colaligns, fmt.datarow, rowalign=ralign
+            )
+            _append_line(lines, padded_widths, colaligns, fmt.linebetweenrows)
+        # the last row without a line below
+        append_row(
+            lines,
+            padded_rows[-1],
+            padded_widths,
+            colaligns,
+            fmt.datarow,
+            rowalign=rowaligns[-1],
+        )
+    else:
+        separating_line = (
+            fmt.linebetweenrows
+            or fmt.linebelowheader
+            or fmt.linebelow
+            or fmt.lineabove
+            or Line("", "", "", "")
+        )
+        for row in padded_rows:
+            # test to see if either the 1st column or the 2nd column (account for showindex) has
+            # the SEPARATING_LINE flag
+            if _is_separating_line(row):
+                _append_line(lines, padded_widths, colaligns, separating_line)
+            else:
+                append_row(lines, row, padded_widths, colaligns, fmt.datarow)
+
+    if fmt.linebelow and "linebelow" not in hidden:
+        _append_line(lines, padded_widths, colaligns, fmt.linebelow)
+
+    if headers or rows:
+        output = "\n".join(lines)
+        if fmt.lineabove == _html_begin_table_without_header:
+            return JupyterHTMLStr(output)
+        else:
+            return output
+    else:  # a completely empty table
+        return ""
+
+
+class _CustomTextWrap(textwrap.TextWrapper):
+    """A custom implementation of CPython's textwrap.TextWrapper. This supports
+    both wide characters (Korea, Japanese, Chinese)  - including mixed string.
+    For the most part, the `_handle_long_word` and `_wrap_chunks` functions were
+    copy pasted out of the CPython baseline, and updated with our custom length
+    and line appending logic.
+    """
+
+    def __init__(self, *args, **kwargs):
+        self._active_codes = []
+        self.max_lines = None  # For python2 compatibility
+        textwrap.TextWrapper.__init__(self, *args, **kwargs)
+
+    @staticmethod
+    def _len(item):
+        """Custom len that gets console column width for wide
+        and non-wide characters as well as ignores color codes"""
+        stripped = _strip_ansi(item)
+        if wcwidth:
+            return wcwidth.wcswidth(stripped)
+        else:
+            return len(stripped)
+
+    def _update_lines(self, lines, new_line):
+        """Adds a new line to the list of lines the text is being wrapped into
+        This function will also track any ANSI color codes in this string as well
+        as add any colors from previous lines order to preserve the same formatting
+        as a single unwrapped string.
+        """
+        code_matches = [x for x in _ansi_codes.finditer(new_line)]
+        color_codes = [
+            code.string[code.span()[0] : code.span()[1]] for code in code_matches
+        ]
+
+        # Add color codes from earlier in the unwrapped line, and then track any new ones we add.
+        new_line = "".join(self._active_codes) + new_line
+
+        for code in color_codes:
+            if code != _ansi_color_reset_code:
+                self._active_codes.append(code)
+            else:  # A single reset code resets everything
+                self._active_codes = []
+
+        # Always ensure each line is color terminted if any colors are
+        # still active, otherwise colors will bleed into other cells on the console
+        if len(self._active_codes) > 0:
+            new_line = new_line + _ansi_color_reset_code
+
+        lines.append(new_line)
+
+    def _handle_long_word(self, reversed_chunks, cur_line, cur_len, width):
+        """_handle_long_word(chunks : [string],
+                             cur_line : [string],
+                             cur_len : int, width : int)
+        Handle a chunk of text (most likely a word, not whitespace) that
+        is too long to fit in any line.
+        """
+        # Figure out when indent is larger than the specified width, and make
+        # sure at least one character is stripped off on every pass
+        if width < 1:
+            space_left = 1
+        else:
+            space_left = width - cur_len
+
+        # If we're allowed to break long words, then do so: put as much
+        # of the next chunk onto the current line as will fit.
+        if self.break_long_words:
+            # Tabulate Custom: Build the string up piece-by-piece in order to
+            # take each charcter's width into account
+            chunk = reversed_chunks[-1]
+            i = 1
+            while self._len(chunk[:i]) <= space_left:
+                i = i + 1
+            cur_line.append(chunk[: i - 1])
+            reversed_chunks[-1] = chunk[i - 1 :]
+
+        # Otherwise, we have to preserve the long word intact.  Only add
+        # it to the current line if there's nothing already there --
+        # that minimizes how much we violate the width constraint.
+        elif not cur_line:
+            cur_line.append(reversed_chunks.pop())
+
+        # If we're not allowed to break long words, and there's already
+        # text on the current line, do nothing.  Next time through the
+        # main loop of _wrap_chunks(), we'll wind up here again, but
+        # cur_len will be zero, so the next line will be entirely
+        # devoted to the long word that we can't handle right now.
+
+    def _wrap_chunks(self, chunks):
+        """_wrap_chunks(chunks : [string]) -> [string]
+        Wrap a sequence of text chunks and return a list of lines of
+        length 'self.width' or less.  (If 'break_long_words' is false,
+        some lines may be longer than this.)  Chunks correspond roughly
+        to words and the whitespace between them: each chunk is
+        indivisible (modulo 'break_long_words'), but a line break can
+        come between any two chunks.  Chunks should not have internal
+        whitespace; ie. a chunk is either all whitespace or a "word".
+        Whitespace chunks will be removed from the beginning and end of
+        lines, but apart from that whitespace is preserved.
+        """
+        lines = []
+        if self.width <= 0:
+            raise ValueError("invalid width %r (must be > 0)" % self.width)
+        if self.max_lines is not None:
+            if self.max_lines > 1:
+                indent = self.subsequent_indent
+            else:
+                indent = self.initial_indent
+            if self._len(indent) + self._len(self.placeholder.lstrip()) > self.width:
+                raise ValueError("placeholder too large for max width")
+
+        # Arrange in reverse order so items can be efficiently popped
+        # from a stack of chucks.
+        chunks.reverse()
+
+        while chunks:
+
+            # Start the list of chunks that will make up the current line.
+            # cur_len is just the length of all the chunks in cur_line.
+            cur_line = []
+            cur_len = 0
+
+            # Figure out which static string will prefix this line.
+            if lines:
+                indent = self.subsequent_indent
+            else:
+                indent = self.initial_indent
+
+            # Maximum width for this line.
+            width = self.width - self._len(indent)
+
+            # First chunk on line is whitespace -- drop it, unless this
+            # is the very beginning of the text (ie. no lines started yet).
+            if self.drop_whitespace and chunks[-1].strip() == "" and lines:
+                del chunks[-1]
+
+            while chunks:
+                chunk_len = self._len(chunks[-1])
+
+                # Can at least squeeze this chunk onto the current line.
+                if cur_len + chunk_len <= width:
+                    cur_line.append(chunks.pop())
+                    cur_len += chunk_len
+
+                # Nope, this line is full.
+                else:
+                    break
+
+            # The current line is full, and the next chunk is too big to
+            # fit on *any* line (not just this one).
+            if chunks and self._len(chunks[-1]) > width:
+                self._handle_long_word(chunks, cur_line, cur_len, width)
+                cur_len = sum(map(self._len, cur_line))
+
+            # If the last chunk on this line is all whitespace, drop it.
+            if self.drop_whitespace and cur_line and cur_line[-1].strip() == "":
+                cur_len -= self._len(cur_line[-1])
+                del cur_line[-1]
+
+            if cur_line:
+                if (
+                    self.max_lines is None
+                    or len(lines) + 1 < self.max_lines
+                    or (
+                        not chunks
+                        or self.drop_whitespace
+                        and len(chunks) == 1
+                        and not chunks[0].strip()
+                    )
+                    and cur_len <= width
+                ):
+                    # Convert current line back to a string and store it in
+                    # list of all lines (return value).
+                    self._update_lines(lines, indent + "".join(cur_line))
+                else:
+                    while cur_line:
+                        if (
+                            cur_line[-1].strip()
+                            and cur_len + self._len(self.placeholder) <= width
+                        ):
+                            cur_line.append(self.placeholder)
+                            self._update_lines(lines, indent + "".join(cur_line))
+                            break
+                        cur_len -= self._len(cur_line[-1])
+                        del cur_line[-1]
+                    else:
+                        if lines:
+                            prev_line = lines[-1].rstrip()
+                            if (
+                                self._len(prev_line) + self._len(self.placeholder)
+                                <= self.width
+                            ):
+                                lines[-1] = prev_line + self.placeholder
+                                break
+                        self._update_lines(lines, indent + self.placeholder.lstrip())
+                    break
+
+        return lines
+
+
+def _main():
+    """\
+    Usage: tabulate [options] [FILE ...]
+
+    Pretty-print tabular data.
+    See also https://github.com/astanin/python-tabulate
+
+    FILE                      a filename of the file with tabular data;
+                              if "-" or missing, read data from stdin.
+
+    Options:
+
+    -h, --help                show this message
+    -1, --header              use the first row of data as a table header
+    -o FILE, --output FILE    print table to FILE (default: stdout)
+    -s REGEXP, --sep REGEXP   use a custom column separator (default: whitespace)
+    -F FPFMT, --float FPFMT   floating point number format (default: g)
+    -I INTFMT, --int INTFMT   integer point number format (default: "")
+    -f FMT, --format FMT      set output table format; supported formats:
+                              plain, simple, grid, fancy_grid, pipe, orgtbl,
+                              rst, mediawiki, html, latex, latex_raw,
+                              latex_booktabs, latex_longtable, tsv
+                              (default: simple)
+    """
+    import getopt
+    import sys
+    import textwrap
+
+    usage = textwrap.dedent(_main.__doc__)
+    try:
+        opts, args = getopt.getopt(
+            sys.argv[1:],
+            "h1o:s:F:A:f:",
+            ["help", "header", "output", "sep=", "float=", "int=", "align=", "format="],
+        )
+    except getopt.GetoptError as e:
+        print(e)
+        print(usage)
+        sys.exit(2)
+    headers = []
+    floatfmt = _DEFAULT_FLOATFMT
+    intfmt = _DEFAULT_INTFMT
+    colalign = None
+    tablefmt = "simple"
+    sep = r"\s+"
+    outfile = "-"
+    for opt, value in opts:
+        if opt in ["-1", "--header"]:
+            headers = "firstrow"
+        elif opt in ["-o", "--output"]:
+            outfile = value
+        elif opt in ["-F", "--float"]:
+            floatfmt = value
+        elif opt in ["-I", "--int"]:
+            intfmt = value
+        elif opt in ["-C", "--colalign"]:
+            colalign = value.split()
+        elif opt in ["-f", "--format"]:
+            if value not in tabulate_formats:
+                print("%s is not a supported table format" % value)
+                print(usage)
+                sys.exit(3)
+            tablefmt = value
+        elif opt in ["-s", "--sep"]:
+            sep = value
+        elif opt in ["-h", "--help"]:
+            print(usage)
+            sys.exit(0)
+    files = [sys.stdin] if not args else args
+    with (sys.stdout if outfile == "-" else open(outfile, "w")) as out:
+        for f in files:
+            if f == "-":
+                f = sys.stdin
+            if _is_file(f):
+                _pprint_file(
+                    f,
+                    headers=headers,
+                    tablefmt=tablefmt,
+                    sep=sep,
+                    floatfmt=floatfmt,
+                    intfmt=intfmt,
+                    file=out,
+                    colalign=colalign,
+                )
+            else:
+                with open(f) as fobj:
+                    _pprint_file(
+                        fobj,
+                        headers=headers,
+                        tablefmt=tablefmt,
+                        sep=sep,
+                        floatfmt=floatfmt,
+                        intfmt=intfmt,
+                        file=out,
+                        colalign=colalign,
+                    )
+
+
+def _pprint_file(fobject, headers, tablefmt, sep, floatfmt, intfmt, file, colalign):
+    rows = fobject.readlines()
+    table = [re.split(sep, r.rstrip()) for r in rows if r.strip()]
+    print(
+        tabulate(
+            table,
+            headers,
+            tablefmt,
+            floatfmt=floatfmt,
+            intfmt=intfmt,
+            colalign=colalign,
+        ),
+        file=file,
+    )
+
+
+if __name__ == "__main__":
+    _main()
```

### Comparing `pyrobox-0.9.4/src/user_mgmt.py` & `pyrobox-0.9.5/src/user_mgmt.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,562 +1,562 @@
-# import pickledb
-import hashlib
-import time, datetime
-from secrets import compare_digest
-from enum import Enum
-from typing import Tuple, List, TypeVar, Union
-
-
-
-import binascii
-
-from .pyroboxCore import logger
-from .pyroDB import PickleTable, _PickleTRow
-from .data_types import LimitedDict
-
-# Loads user database. Database is plaintext but stores passwords as a hash salted by config.PASSWORD
-
-
-__all__ = [
-	"User",
-	"UserPermission",
-	"permits"
-]
-
-
-
-def compare_digest_hex(digest, hex_data):
-	return compare_digest(hex_data.encode("ascii"), binascii.hexlify(digest))
-
-
-
-
-
-
-class UserPermission(Enum):
-	"""Enum for WebUI user permissions, inspired by Unix permission style
-
-	Args:
-		Enum (int): Permission code for user
-	"""
-
-	NOPERMISSION = -1
-	VIEW = 0        # view file list
-	DOWNLOAD = 1    # download files
-	MODIFY = 2      # rename, overwrite, new folder
-	DELETE = 3      # delete files
-	UPLOAD = 4      # upload files
-	ZIP = 5         # download zip folder
-	ADMIN = 6       # admin
-	MEMBER = 7      # member or guest
-
-TOTAL_PERMISSIONS = max([each.value for each in UserPermission]) + 1
-
-permits = UserPermission # lazy to type long words
-
-
-class PermissionList(list):
-	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
-
-	def __getattr__(self, name:str):
-		name = name.upper()
-		options = dict(
-			VIEW = 0,       # view file list
-			DOWNLOAD = 1,   # download files
-			MODIFY = 2,     # rename, overwrite, new folder
-			DELETE = 3,     # delete files
-			UPLOAD = 4,     # upload files
-			ZIP = 5,        # download zip folder
-			ADMIN = 6,      # admin
-			MEMBER = 7,     # member or guest
-		)
-		if name in options:
-			return bool(self[options[name]])
-
-		if name == "NOPERMISSION":
-			return not any(self)
-
-
-class User:
-	"""Object for WebUI users"""
-	def __init__(self, row:_PickleTRow={}):
-		"""Generate Object for WebUI users
-
-		Args:
-			row (_PickleTRow|dict): user data row
-			[username] (str): plaintext username
-			[permission] (int): compiled UserPermission set
-			[password ](str, hash): hashed password.
-
-		Raises:
-			ValueError: User failed to create
-
-		Returns:
-			User: Object for WebUI users
-		"""
-
-
-		self.db = row
-		self.user_handler = User_handler() # type: User_handler
-
-
-
-
-	Self = TypeVar("Self")
-	# self reference for use in classmethods that can't strong type User because it's inside the method
-
-	def __getattr__(self, name):
-		if hasattr(UserPermission, name):
-			return self.check_permission(getattr(UserPermission, name))
-
-	@property
-	def username(self) -> str:
-		return self.db["username"]
-
-	@property
-	def permission_pack(self) -> int:
-		return self.db["permission"]
-
-	@property
-	def password(self) -> bytes:
-		return self.db["password"]
-
-	@property
-	def token(self) -> bytes:
-		return self.db["token"]
-
-	@property
-	def uid(self) -> str:
-		return self.db["id"]
-
-	@property
-	def token_hex(self) -> str:
-		return binascii.hexlify(self.token).decode("ascii")
-
-	@property
-	def permission(self) -> PermissionList:
-		return self.unpack_permission(self.permission_pack)
-
-
-	def is_admin(self) -> bool:
-		return self.ADMIN
-
-	# get the sha1 hash of the CLI password to use as a salt, makes a longer string and avoids holding secrets in memory
-
-	def salt_password(self, password) -> bytes:
-		return hashlib.sha256((self.user_handler.common_salt+password).encode('utf-8')).digest()
-
-	def set_password(self, password:str) -> None:
-		# salt, hash and store password
-		p_hash = self.salt_password(password)
-		token = hashlib.sha256(p_hash + str(time.time()).encode()).digest()
-
-		# only store binary data
-
-		self.update("password", p_hash)
-		self.update("token", token)
-
-
-
-	def reset_pw(self, old_password: str, new_password: str) -> bool:
-		"""Reset password
-
-		Args:
-			old_password (str): Old plaintext password for confirmation before change
-			new_password (str): New plaintext password to be saved
-
-		Returns:
-			int: True if old_password accepted, else False
-		"""
-
-
-		if self.check_password(old_password):
-			logger.info(f"Updating password of user {self.username}")
-			salted_new_password = self.salt_password(new_password)
-
-			self.update("password", salted_new_password)
-			return True
-		else:
-			logger.info(f"User {self.username} password mismatch")
-			return False
-
-	def __setitem__(self, attr, value):
-		self.update(attr, value)
-
-	def __getitem__(self, attr):
-		return self.db[attr]
-
-	def __bool__(self):
-		return bool(self.username)
-
-	def __str__(self):
-		return str(self.db)
-
-	def update(self, attr, value):
-		self.db[attr] = value
-
-	@staticmethod
-	def unpack_permission(packed: int) -> List[int]:
-		"""Unpacks permission as int -> list of binary/bool switches like [0,1,0,0,1,0,1]
-
-		Args:
-			packed (int): permission stored as an integer in the object and db
-
-		Returns:
-			List[int]: list of binary switches to be changed [reversed to make correct order]
-		"""
-		return PermissionList([packed >> index & 1 for index in range(0, TOTAL_PERMISSIONS)])
-
-	@staticmethod
-	def pack_permission(unpacked: List[int]) -> int:
-		"""Packs permissions from an ordered list of binary switches to an integer for storage in memory/object
-
-		Args:
-			unpacked (List[int]): list of binary switched that were modified
-
-		Returns:
-			int: permission stored as an integer in the object and db
-		"""
-		packed = 0
-		for index, each in enumerate(unpacked):
-			packed |= each << index
-		return packed
-
-	@staticmethod
-	def pack_permission_from_list(unpacked: List[UserPermission]) -> int:
-		"""Packs permissions from an ordered list of UserPermission to an integer for storage in memory/object
-
-		Args:
-			unpacked (List[UserPermission]): list of UserPermission that were modified
-
-		Returns:
-			int: permission stored as an integer in the object and db
-		"""
-
-		packed = 0
-		for each in unpacked:
-			packed |= 1 << each.value
-		return packed
-
-	@staticmethod
-	def unpack_permission_to_list(packed: int) -> List[UserPermission]:
-		"""Unpacks permission as int -> list of UserPermission like [UserPermission.VIEW, UserPermission.DOWNLOAD, UserPermission.ZIP]
-
-		Args:
-			packed (int): permission stored as an integer in the object and db
-
-		Returns:
-			List[UserPermission]: list of UserPermission that were modified
-		"""
-		return [UserPermission(each) for each in range(TOTAL_PERMISSIONS) if packed >> each & 1]
-
-	def set_permission_pack(self, code) -> None:
-		self.update("permission", code)
-
-	def get_permissions(self) -> Tuple[UserPermission]:
-		"""Get searchable permissions tuple
-
-		Returns:
-			Tuple[UserPermission]: Tuple that can be checked with `UserPermission(5) in user.get_permission()` to discern if user has given permission
-		"""
-		output = []
-		for index, each in enumerate(self.permission):
-			if each:
-				output.append(UserPermission(index))
-		if output.__len__() == 0:
-			output.append(UserPermission(-1)) # no permission
-		return tuple(output)
-
-	def check_permission(self, perm) -> bool:
-		if isinstance(perm, list):
-			return all([self.check_permission(each) for each in perm])
-		return perm in self.get_permissions()
-
-
-	def permit(self, *permission:  Union[UserPermission,List[UserPermission],Tuple[UserPermission]]):
-		"""Turn on permissions
-
-		Args:
-			permission (UserPermission,... | Tuple[UserPermission]): Single UserPermission to enable, or tuple of several
-		"""
-		# if isinstance(permission, (list, tuple)) and len(permission) == 1:
-		# 	permission = permission[0]
-
-		if len(permission) == 1 and isinstance(permission[0], (list, tuple)):
-			permission = permission[0]
-
-		if UserPermission.NOPERMISSION in permission:
-			self.revoke_all()
-			return
-
-		new_permission = self.permission
-
-		for each in permission:
-			if not hasattr(each, 'value') and not each: continue # default permission may have none or empty at Initialization
-			new_permission[each.value] = 1
-			# -1 because 0 is no permission
-		self._save_permission(new_permission)
-
-
-	def revoke(self, *permission: Union[UserPermission,List[UserPermission],Tuple[UserPermission]]) -> None:
-		"""Turn off permissions
-
-		Args:
-			permission (UserPermission | Tuple[UserPermission]): Single UserPermission to disable, or tuple of several
-		"""
-		if len(permission) == 1 and isinstance(permission[0], (list, tuple)):
-			permission = permission[0]
-
-		new_permission = self.permission
-		for each in permission:
-			new_permission[each.value] = 0
-
-		self._save_permission(new_permission)
-
-	def revoke_all(self) -> None:
-		"""Turn off all permissions
-		"""
-		permission = [0 for _ in range(len(self.permission))]
-		self._save_permission(permission)
-
-
-	def _save_permission(self, permission: list) -> None:
-		"""Save permission to database
-		"""
-		self.update("permission", self.pack_permission(permission))
-
-
-
-
-	def check_password(self, password: str) -> bool:
-		"""Check credentials
-
-		Args:
-			password (str): Password as plaintext
-
-		Returns:
-			bool: Was password valid?
-		"""
-		salted_new_password = self.salt_password(password)
-		return compare_digest(self.password, salted_new_password)
-
-	def check_token(self, token) -> bool:
-		"""match cookie token (hex str) with db["token"] (digest binary)
-		"""
-		return compare_digest_hex(digest=self.token, hex_data=token)
-
-
-class User_handler:
-	def __init__(self, init_permissions={}):
-		"""
-		init_permissions: `dict` of `UserPermission` to be used as default for new users (member, admin, guest) `{"member": [perms,..], ...}`
-		"""
-		self.user_db = PickleTable()
-
-		self.cached = LimitedDict({}, max=500)
-
-		self.common_salt = "0123456789"
-
-		self.admins:List[User] = []
-		self.member_permission = init_permissions
-
-	def set_common_salt(self, sys_Pass):
-		self.common_salt = hashlib.md5(sys_Pass).hexdigest()
-
-	def load_db(self, db_path=""):
-		self.user_db = PickleTable(db_path)
-		self.user_db.add_column("username",
-			"password",
-			"created_at",
-			"last_active",
-			"id",
-			"token",
-			"permission",
-
-			exist_ok=True)
-
-
-	def create_user(self, username, password, is_admin=False) -> User:
-		p_hash = token = None
-		uid = hashlib.sha1((str(time.time()) + username).encode("utf-8")).hexdigest()
-
-		u_data = {
-			"username": username,
-			"password": p_hash,
-			"created_at": round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2),
-			"last_active": round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2), # datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
-
-			"id": uid, #
-			"token": token,
-
-			"permission": 0,
-		}
-
-		row = self.user_db.add_row(u_data)
-
-		user = User(row=row)
-		self.assign_handler(user)
-		user.set_password(password)
-
-		user.permit(self.member_permission.get("member", []) )
-		if is_admin:
-			self.set_admin(user)
-
-		return user
-
-	def assign_handler(self, user:User):
-		# assign user handler to user
-		# so that if multiple user handlers are created, the user can always find the correct parent
-		user.user_handler = self
-
-	def set_admin(self, user:User):
-		# add user to admin list
-		if user not in self.admins:
-			self.admins.append(user)
-		user.revoke_all()
-		user.permit(self.member_permission.get("admin", []))
-		user.permit(permits.ADMIN)
-
-	def create_guest(self) -> User:
-		user = self.create_user("Guest", "Guest")
-		if "guest" in self.member_permission:
-			user.revoke_all()
-			user.permit(self.member_permission["guest"])
-
-		return user
-
-	def create_admin(self, username, password) -> User:
-		user = self.create_user(username, password, is_admin=True)
-		return user
-
-
-
-	def _user(self, username=None, user=None) -> User:
-		if not user:
-			user = self.get_user(username)
-
-		if not user:
-			raise LookupError("User not found")
-		return user
-
-	def server_signup(self, username, password) -> dict:
-		# check if username is already taken
-		if self.get_user(username, temp=True) is not None:
-			return {
-				"status": "error",
-				"message": "Username already taken"
-			}
-
-		# create user
-		user = self.create_user(username, password)
-		return {
-			"status": "success",
-			"message": "User created",
-			"user_name": user.username,
-			"token": user.token_hex,
-		}
-
-	def server_login(self, username, password) -> dict:
-		user = self.get_user(username)
-		if user is None:
-			return {
-				"status": "error",
-				"message": "User not found"
-			}
-
-		if not user.check_password(password):
-			return {
-				"status": "error",
-				"message": "Wrong password"
-			}
-
-		user.update("last_active", round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2))
-		# print("logged in", user)
-		# user.flags.clear() # clear flags
-
-		return {
-			"status": "success",
-			"message": "User logged in",
-			"user_name": username,
-			"user_id": user["id"]
-		}
-
-	def get_user(self, username, temp=False) -> User:
-		user = self.cached.get(username)
-		if user:
-			return user
-
-
-		user_cell = self.user_db.find_1st(kw=username, column="username", return_obj=True)
-
-		if not user_cell:
-			return None
-
-		user_row = user_cell.row_obj()
-
-		user = User(row=user_row)
-		self.assign_handler(user)
-
-		if not temp:
-			self.cached[username] = user
-
-		return user
-
-	def delete_user(self, username) -> bool:
-		user = self.get_user(username)
-		if user is None:
-			return False
-
-		user.db.del_row() # delete from db
-		self.cached.pop(username, None) # delete from cache
-		return True
-
-
-	def server_verify(self, username:str, token:str, return_user=False) -> Union[bool, User]:
-		user = self.get_user(username)
-		if not user:
-			return False
-		if user.check_token(token):
-			return False
-
-		user["last_active"] = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
-
-		if return_user:
-			return user
-		return True
-
-
-
-
-
-
-
-def test():
-	user_handler = User_handler()
-	user_handler.load_db()
-	z = user_handler.server_signup(username="Admin", password="pass")
-	print(z)
-
-
-
-	u = user_handler.get_user("Admin")
-	if u is None:
-		print("User not found")
-		return
-
-	print(u)
-	print(u.username)
-	print(u.db)
-	print(u.permission)
-	# u.permit(permits.DOWNLOAD, permits.DELETE, permits.ZIP)
-	print(u.permission)
-	print(u.permission.NOPERMISSION)
-	print(u.permission.DOWNLOAD)
-	print(u.get_permissions())
-	print(u.NOPERMISSION)
-	user_handler.set_admin(u)
-	print(u.is_admin())
-
-if __name__ == "__main__":
-	test()
-
+# import pickledb
+import hashlib
+import time, datetime
+from secrets import compare_digest
+from enum import Enum
+from typing import Tuple, List, TypeVar, Union
+
+
+
+import binascii
+
+from .pyroboxCore import logger
+from .pyroDB import PickleTable, _PickleTRow
+from .data_types import LimitedDict
+
+# Loads user database. Database is plaintext but stores passwords as a hash salted by config.PASSWORD
+
+
+__all__ = [
+	"User",
+	"UserPermission",
+	"permits"
+]
+
+
+
+def compare_digest_hex(digest, hex_data):
+	return compare_digest(hex_data.encode("ascii"), binascii.hexlify(digest))
+
+
+
+
+
+
+class UserPermission(Enum):
+	"""Enum for WebUI user permissions, inspired by Unix permission style
+
+	Args:
+		Enum (int): Permission code for user
+	"""
+
+	NOPERMISSION = -1
+	VIEW = 0        # view file list
+	DOWNLOAD = 1    # download files
+	MODIFY = 2      # rename, overwrite, new folder
+	DELETE = 3      # delete files
+	UPLOAD = 4      # upload files
+	ZIP = 5         # download zip folder
+	ADMIN = 6       # admin
+	MEMBER = 7      # member or guest
+
+TOTAL_PERMISSIONS = max([each.value for each in UserPermission]) + 1
+
+permits = UserPermission # lazy to type long words
+
+
+class PermissionList(list):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+
+	def __getattr__(self, name:str):
+		name = name.upper()
+		options = dict(
+			VIEW = 0,       # view file list
+			DOWNLOAD = 1,   # download files
+			MODIFY = 2,     # rename, overwrite, new folder
+			DELETE = 3,     # delete files
+			UPLOAD = 4,     # upload files
+			ZIP = 5,        # download zip folder
+			ADMIN = 6,      # admin
+			MEMBER = 7,     # member or guest
+		)
+		if name in options:
+			return bool(self[options[name]])
+
+		if name == "NOPERMISSION":
+			return not any(self)
+
+
+class User:
+	"""Object for WebUI users"""
+	def __init__(self, row:_PickleTRow={}):
+		"""Generate Object for WebUI users
+
+		Args:
+			row (_PickleTRow|dict): user data row
+			[username] (str): plaintext username
+			[permission] (int): compiled UserPermission set
+			[password ](str, hash): hashed password.
+
+		Raises:
+			ValueError: User failed to create
+
+		Returns:
+			User: Object for WebUI users
+		"""
+
+
+		self.db = row
+		self.user_handler = User_handler() # type: User_handler
+
+
+
+
+	Self = TypeVar("Self")
+	# self reference for use in classmethods that can't strong type User because it's inside the method
+
+	def __getattr__(self, name):
+		if hasattr(UserPermission, name):
+			return self.check_permission(getattr(UserPermission, name))
+
+	@property
+	def username(self) -> str:
+		return self.db["username"]
+
+	@property
+	def permission_pack(self) -> int:
+		return self.db["permission"]
+
+	@property
+	def password(self) -> bytes:
+		return self.db["password"]
+
+	@property
+	def token(self) -> bytes:
+		return self.db["token"]
+
+	@property
+	def uid(self) -> str:
+		return self.db["id"]
+
+	@property
+	def token_hex(self) -> str:
+		return binascii.hexlify(self.token).decode("ascii")
+
+	@property
+	def permission(self) -> PermissionList:
+		return self.unpack_permission(self.permission_pack)
+
+
+	def is_admin(self) -> bool:
+		return self.ADMIN
+
+	# get the sha1 hash of the CLI password to use as a salt, makes a longer string and avoids holding secrets in memory
+
+	def salt_password(self, password) -> bytes:
+		return hashlib.sha256((self.user_handler.common_salt+password).encode('utf-8')).digest()
+
+	def set_password(self, password:str) -> None:
+		# salt, hash and store password
+		p_hash = self.salt_password(password)
+		token = hashlib.sha256(p_hash + str(time.time()).encode()).digest()
+
+		# only store binary data
+
+		self.update("password", p_hash)
+		self.update("token", token)
+
+
+
+	def reset_pw(self, old_password: str, new_password: str) -> bool:
+		"""Reset password
+
+		Args:
+			old_password (str): Old plaintext password for confirmation before change
+			new_password (str): New plaintext password to be saved
+
+		Returns:
+			int: True if old_password accepted, else False
+		"""
+
+
+		if self.check_password(old_password):
+			logger.info(f"Updating password of user {self.username}")
+			salted_new_password = self.salt_password(new_password)
+
+			self.update("password", salted_new_password)
+			return True
+		else:
+			logger.info(f"User {self.username} password mismatch")
+			return False
+
+	def __setitem__(self, attr, value):
+		self.update(attr, value)
+
+	def __getitem__(self, attr):
+		return self.db[attr]
+
+	def __bool__(self):
+		return bool(self.username)
+
+	def __str__(self):
+		return str(self.db)
+
+	def update(self, attr, value):
+		self.db[attr] = value
+
+	@staticmethod
+	def unpack_permission(packed: int) -> List[int]:
+		"""Unpacks permission as int -> list of binary/bool switches like [0,1,0,0,1,0,1]
+
+		Args:
+			packed (int): permission stored as an integer in the object and db
+
+		Returns:
+			List[int]: list of binary switches to be changed [reversed to make correct order]
+		"""
+		return PermissionList([packed >> index & 1 for index in range(0, TOTAL_PERMISSIONS)])
+
+	@staticmethod
+	def pack_permission(unpacked: List[int]) -> int:
+		"""Packs permissions from an ordered list of binary switches to an integer for storage in memory/object
+
+		Args:
+			unpacked (List[int]): list of binary switched that were modified
+
+		Returns:
+			int: permission stored as an integer in the object and db
+		"""
+		packed = 0
+		for index, each in enumerate(unpacked):
+			packed |= each << index
+		return packed
+
+	@staticmethod
+	def pack_permission_from_list(unpacked: List[UserPermission]) -> int:
+		"""Packs permissions from an ordered list of UserPermission to an integer for storage in memory/object
+
+		Args:
+			unpacked (List[UserPermission]): list of UserPermission that were modified
+
+		Returns:
+			int: permission stored as an integer in the object and db
+		"""
+
+		packed = 0
+		for each in unpacked:
+			packed |= 1 << each.value
+		return packed
+
+	@staticmethod
+	def unpack_permission_to_list(packed: int) -> List[UserPermission]:
+		"""Unpacks permission as int -> list of UserPermission like [UserPermission.VIEW, UserPermission.DOWNLOAD, UserPermission.ZIP]
+
+		Args:
+			packed (int): permission stored as an integer in the object and db
+
+		Returns:
+			List[UserPermission]: list of UserPermission that were modified
+		"""
+		return [UserPermission(each) for each in range(TOTAL_PERMISSIONS) if packed >> each & 1]
+
+	def set_permission_pack(self, code) -> None:
+		self.update("permission", code)
+
+	def get_permissions(self) -> Tuple[UserPermission]:
+		"""Get searchable permissions tuple
+
+		Returns:
+			Tuple[UserPermission]: Tuple that can be checked with `UserPermission(5) in user.get_permission()` to discern if user has given permission
+		"""
+		output = []
+		for index, each in enumerate(self.permission):
+			if each:
+				output.append(UserPermission(index))
+		if output.__len__() == 0:
+			output.append(UserPermission(-1)) # no permission
+		return tuple(output)
+
+	def check_permission(self, perm) -> bool:
+		if isinstance(perm, list):
+			return all([self.check_permission(each) for each in perm])
+		return perm in self.get_permissions()
+
+
+	def permit(self, *permission:  Union[UserPermission,List[UserPermission],Tuple[UserPermission]]):
+		"""Turn on permissions
+
+		Args:
+			permission (UserPermission,... | Tuple[UserPermission]): Single UserPermission to enable, or tuple of several
+		"""
+		# if isinstance(permission, (list, tuple)) and len(permission) == 1:
+		# 	permission = permission[0]
+
+		if len(permission) == 1 and isinstance(permission[0], (list, tuple)):
+			permission = permission[0]
+
+		if UserPermission.NOPERMISSION in permission:
+			self.revoke_all()
+			return
+
+		new_permission = self.permission
+
+		for each in permission:
+			if not hasattr(each, 'value') and not each: continue # default permission may have none or empty at Initialization
+			new_permission[each.value] = 1
+			# -1 because 0 is no permission
+		self._save_permission(new_permission)
+
+
+	def revoke(self, *permission: Union[UserPermission,List[UserPermission],Tuple[UserPermission]]) -> None:
+		"""Turn off permissions
+
+		Args:
+			permission (UserPermission | Tuple[UserPermission]): Single UserPermission to disable, or tuple of several
+		"""
+		if len(permission) == 1 and isinstance(permission[0], (list, tuple)):
+			permission = permission[0]
+
+		new_permission = self.permission
+		for each in permission:
+			new_permission[each.value] = 0
+
+		self._save_permission(new_permission)
+
+	def revoke_all(self) -> None:
+		"""Turn off all permissions
+		"""
+		permission = [0 for _ in range(len(self.permission))]
+		self._save_permission(permission)
+
+
+	def _save_permission(self, permission: list) -> None:
+		"""Save permission to database
+		"""
+		self.update("permission", self.pack_permission(permission))
+
+
+
+
+	def check_password(self, password: str) -> bool:
+		"""Check credentials
+
+		Args:
+			password (str): Password as plaintext
+
+		Returns:
+			bool: Was password valid?
+		"""
+		salted_new_password = self.salt_password(password)
+		return compare_digest(self.password, salted_new_password)
+
+	def check_token(self, token) -> bool:
+		"""match cookie token (hex str) with db["token"] (digest binary)
+		"""
+		return compare_digest_hex(digest=self.token, hex_data=token)
+
+
+class User_handler:
+	def __init__(self, init_permissions={}):
+		"""
+		init_permissions: `dict` of `UserPermission` to be used as default for new users (member, admin, guest) `{"member": [perms,..], ...}`
+		"""
+		self.user_db = PickleTable()
+
+		self.cached = LimitedDict({}, max=500)
+
+		self.common_salt = "0123456789"
+
+		self.admins:List[User] = []
+		self.member_permission = init_permissions
+
+	def set_common_salt(self, sys_Pass):
+		self.common_salt = hashlib.md5(sys_Pass).hexdigest()
+
+	def load_db(self, db_path=""):
+		self.user_db = PickleTable(db_path)
+		self.user_db.add_column("username",
+			"password",
+			"created_at",
+			"last_active",
+			"id",
+			"token",
+			"permission",
+
+			exist_ok=True)
+
+
+	def create_user(self, username, password, is_admin=False) -> User:
+		p_hash = token = None
+		uid = hashlib.sha1((str(time.time()) + username).encode("utf-8")).hexdigest()
+
+		u_data = {
+			"username": username,
+			"password": p_hash,
+			"created_at": round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2),
+			"last_active": round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2), # datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
+
+			"id": uid, #
+			"token": token,
+
+			"permission": 0,
+		}
+
+		row = self.user_db.add_row(u_data)
+
+		user = User(row=row)
+		self.assign_handler(user)
+		user.set_password(password)
+
+		user.permit(self.member_permission.get("member", []) )
+		if is_admin:
+			self.set_admin(user)
+
+		return user
+
+	def assign_handler(self, user:User):
+		# assign user handler to user
+		# so that if multiple user handlers are created, the user can always find the correct parent
+		user.user_handler = self
+
+	def set_admin(self, user:User):
+		# add user to admin list
+		if user not in self.admins:
+			self.admins.append(user)
+		user.revoke_all()
+		user.permit(self.member_permission.get("admin", []))
+		user.permit(permits.ADMIN)
+
+	def create_guest(self) -> User:
+		user = self.create_user("Guest", "Guest")
+		if "guest" in self.member_permission:
+			user.revoke_all()
+			user.permit(self.member_permission["guest"])
+
+		return user
+
+	def create_admin(self, username, password) -> User:
+		user = self.create_user(username, password, is_admin=True)
+		return user
+
+
+
+	def _user(self, username=None, user=None) -> User:
+		if not user:
+			user = self.get_user(username)
+
+		if not user:
+			raise LookupError("User not found")
+		return user
+
+	def server_signup(self, username, password) -> dict:
+		# check if username is already taken
+		if self.get_user(username, temp=True) is not None:
+			return {
+				"status": "error",
+				"message": "Username already taken"
+			}
+
+		# create user
+		user = self.create_user(username, password)
+		return {
+			"status": "success",
+			"message": "User created",
+			"user_name": user.username,
+			"token": user.token_hex,
+		}
+
+	def server_login(self, username, password) -> dict:
+		user = self.get_user(username)
+		if user is None:
+			return {
+				"status": "error",
+				"message": "User not found"
+			}
+
+		if not user.check_password(password):
+			return {
+				"status": "error",
+				"message": "Wrong password"
+			}
+
+		user.update("last_active", round(datetime.datetime.now(datetime.timezone.utc).timestamp(),2))
+		# print("logged in", user)
+		# user.flags.clear() # clear flags
+
+		return {
+			"status": "success",
+			"message": "User logged in",
+			"user_name": username,
+			"user_id": user["id"]
+		}
+
+	def get_user(self, username, temp=False) -> User:
+		user = self.cached.get(username)
+		if user:
+			return user
+
+
+		user_cell = self.user_db.find_1st(kw=username, column="username", return_obj=True)
+
+		if not user_cell:
+			return None
+
+		user_row = user_cell.row_obj()
+
+		user = User(row=user_row)
+		self.assign_handler(user)
+
+		if not temp:
+			self.cached[username] = user
+
+		return user
+
+	def delete_user(self, username) -> bool:
+		user = self.get_user(username)
+		if user is None:
+			return False
+
+		user.db.del_row() # delete from db
+		self.cached.pop(username, None) # delete from cache
+		return True
+
+
+	def server_verify(self, username:str, token:str, return_user=False) -> Union[bool, User]:
+		user = self.get_user(username)
+		if not user:
+			return False
+		if user.check_token(token):
+			return False
+
+		user["last_active"] = datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")
+
+		if return_user:
+			return user
+		return True
+
+
+
+
+
+
+
+def test():
+	user_handler = User_handler()
+	user_handler.load_db()
+	z = user_handler.server_signup(username="Admin", password="pass")
+	print(z)
+
+
+
+	u = user_handler.get_user("Admin")
+	if u is None:
+		print("User not found")
+		return
+
+	print(u)
+	print(u.username)
+	print(u.db)
+	print(u.permission)
+	# u.permit(permits.DOWNLOAD, permits.DELETE, permits.ZIP)
+	print(u.permission)
+	print(u.permission.NOPERMISSION)
+	print(u.permission.DOWNLOAD)
+	print(u.get_permissions())
+	print(u.NOPERMISSION)
+	user_handler.set_admin(u)
+	print(u.is_admin())
+
+if __name__ == "__main__":
+	test()
+
```

