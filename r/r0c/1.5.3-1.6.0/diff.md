# Comparing `tmp/r0c-1.5.3.tar.gz` & `tmp/r0c-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r0c-1.5.3.tar", last modified: Tue Oct 10 03:32:38 2023, max compression
+gzip compressed data, was "r0c-1.6.0.tar", last modified: Thu Apr  4 23:56:32 2024, max compression
```

## Comparing `r0c-1.5.3.tar` & `r0c-1.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-10 03:32:38.921347 r0c-1.5.3/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-19 15:14:09.000000 r0c-1.5.3/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2023-10-10 03:32:38.000000 r0c-1.5.3/MANIFEST.in
--rw-r--r--   0 ed        (1000) ed        (1000)     8692 2023-10-10 03:32:38.921347 r0c-1.5.3/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     6772 2023-10-10 03:16:50.000000 r0c-1.5.3/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-10 03:32:38.919347 r0c-1.5.3/clients/
--rwxr-xr-x   0 ed        (1000) ed        (1000)     1002 2021-09-19 15:14:09.000000 r0c-1.5.3/clients/bash.sh
--rw-r--r--   0 ed        (1000) ed        (1000)     5605 2023-09-19 18:59:16.000000 r0c-1.5.3/clients/powershell.ps1
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-10 03:32:38.919347 r0c-1.5.3/docs/
--rw-r--r--   0 ed        (1000) ed        (1000)      333 2021-09-19 15:14:09.000000 r0c-1.5.3/docs/help-about.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2555 2023-09-17 18:02:43.000000 r0c-1.5.3/docs/help-commands.md
--rw-r--r--   0 ed        (1000) ed        (1000)      836 2023-09-17 18:02:49.000000 r0c-1.5.3/docs/help-hotkeys.md
--rw-r--r--   0 ed        (1000) ed        (1000)      197 2023-09-19 19:21:36.000000 r0c-1.5.3/docs/help-topics.md
--rw-r--r--   0 ed        (1000) ed        (1000)      670 2023-09-20 00:08:59.000000 r0c-1.5.3/docs/help-ui.md
--rw-r--r--   0 ed        (1000) ed        (1000)     2507 2023-09-18 22:23:06.000000 r0c-1.5.3/docs/todo.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-10 03:32:38.920347 r0c-1.5.3/r0c/
--rw-------   0 ed        (1000) ed        (1000)     2543 2022-08-31 21:02:50.000000 r0c-1.5.3/r0c/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21291 2023-10-10 00:29:12.000000 r0c-1.5.3/r0c/__main__.py
--rw-------   0 ed        (1000) ed        (1000)      213 2023-10-10 03:27:11.000000 r0c-1.5.3/r0c/__version__.py
--rw-------   0 ed        (1000) ed        (1000)     8258 2023-09-19 21:32:47.000000 r0c-1.5.3/r0c/chat.py
--rw-------   0 ed        (1000) ed        (1000)     2227 2022-09-01 21:50:46.000000 r0c-1.5.3/r0c/diag.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3538 2023-10-09 23:43:46.000000 r0c-1.5.3/r0c/inetcat.py
--rw-r--r--   0 ed        (1000) ed        (1000)    13828 2023-10-09 23:43:58.000000 r0c-1.5.3/r0c/itelnet.py
--rw-r--r--   0 ed        (1000) ed        (1000)   107552 2023-10-10 03:29:28.000000 r0c-1.5.3/r0c/ivt100.py
--rw-------   0 ed        (1000) ed        (1000)    36286 2023-10-10 00:31:59.000000 r0c-1.5.3/r0c/user.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17105 2023-10-10 00:18:17.000000 r0c-1.5.3/r0c/util.py
--rw-------   0 ed        (1000) ed        (1000)    19230 2023-09-19 23:26:40.000000 r0c-1.5.3/r0c/world.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-10-10 03:32:38.921347 r0c-1.5.3/r0c.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)     8692 2023-10-10 03:32:38.000000 r0c-1.5.3/r0c.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)      482 2023-10-10 03:32:38.000000 r0c-1.5.3/r0c.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-10-10 03:32:38.000000 r0c-1.5.3/r0c.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       42 2023-10-10 03:32:38.000000 r0c-1.5.3/r0c.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        4 2023-10-10 03:32:38.000000 r0c-1.5.3/r0c.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-10-10 03:32:38.921347 r0c-1.5.3/setup.cfg
--rwxr-xr-x   0 ed        (1000) ed        (1000)     4658 2023-05-14 22:32:58.000000 r0c-1.5.3/setup.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.988482 r0c-1.6.0/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-19 15:14:09.000000 r0c-1.6.0/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2024-04-04 23:56:32.000000 r0c-1.6.0/MANIFEST.in
+-rw-r--r--   0 ed        (1000) ed        (1000)     9139 2024-04-04 23:56:32.988482 r0c-1.6.0/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     7219 2024-04-02 16:47:55.000000 r0c-1.6.0/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.985482 r0c-1.6.0/clients/
+-rwxr-xr-x   0 ed        (1000) ed        (1000)     1002 2021-09-19 15:14:09.000000 r0c-1.6.0/clients/bash.sh
+-rw-r--r--   0 ed        (1000) ed        (1000)     5605 2023-09-19 18:59:16.000000 r0c-1.6.0/clients/powershell.ps1
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.985482 r0c-1.6.0/docs/
+-rw-r--r--   0 ed        (1000) ed        (1000)      333 2021-09-19 15:14:09.000000 r0c-1.6.0/docs/help-about.md
+-rw-r--r--   0 ed        (1000) ed        (1000)     2730 2024-04-04 22:12:04.000000 r0c-1.6.0/docs/help-commands.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      836 2023-09-17 18:02:49.000000 r0c-1.6.0/docs/help-hotkeys.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      197 2023-09-19 19:21:36.000000 r0c-1.6.0/docs/help-topics.md
+-rw-r--r--   0 ed        (1000) ed        (1000)      670 2023-09-20 00:08:59.000000 r0c-1.6.0/docs/help-ui.md
+-rw-r--r--   0 ed        (1000) ed        (1000)     2367 2024-04-04 23:26:14.000000 r0c-1.6.0/docs/todo.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.987482 r0c-1.6.0/r0c/
+-rw-------   0 ed        (1000) ed        (1000)     2543 2022-08-31 21:02:50.000000 r0c-1.6.0/r0c/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    24287 2024-04-04 23:35:45.000000 r0c-1.6.0/r0c/__main__.py
+-rw-------   0 ed        (1000) ed        (1000)      211 2024-04-04 23:27:04.000000 r0c-1.6.0/r0c/__version__.py
+-rw-------   0 ed        (1000) ed        (1000)     8453 2024-04-04 22:25:29.000000 r0c-1.6.0/r0c/chat.py
+-rw-------   0 ed        (1000) ed        (1000)     2227 2022-09-01 21:50:46.000000 r0c-1.6.0/r0c/diag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3538 2023-10-09 23:43:46.000000 r0c-1.6.0/r0c/inetcat.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8648 2024-04-04 23:36:51.000000 r0c-1.6.0/r0c/irc.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    13828 2023-10-09 23:43:58.000000 r0c-1.6.0/r0c/itelnet.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   108688 2024-04-04 22:28:29.000000 r0c-1.6.0/r0c/ivt100.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    37076 2024-04-04 23:44:07.000000 r0c-1.6.0/r0c/user.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20569 2024-04-04 22:23:55.000000 r0c-1.6.0/r0c/util.py
+-rw-------   0 ed        (1000) ed        (1000)    21402 2024-04-04 23:43:38.000000 r0c-1.6.0/r0c/world.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2024-04-04 23:56:32.988482 r0c-1.6.0/r0c.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)     9139 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)      493 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       42 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        4 2024-04-04 23:56:32.000000 r0c-1.6.0/r0c.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2024-04-04 23:56:32.988482 r0c-1.6.0/setup.cfg
+-rwxr-xr-x   0 ed        (1000) ed        (1000)     4658 2023-05-14 22:32:58.000000 r0c-1.6.0/setup.py
```

### Comparing `r0c-1.5.3/LICENSE` & `r0c-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/PKG-INFO` & `r0c-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.5.3
+Version: 1.6.0
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,23 +49,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
+* is not an irc server, but can bridge to/from irc servers
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
+## compatibility
+
+* 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
+* 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
 * notifications (bell/visual) on hilights and PMs
@@ -74,14 +80,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
+* bridge several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -178,13 +185,14 @@
 ## protips
 
 try the following commands and hotkeys after connecting:
 
 * `/cy` enables colored nicknames
 * `/b3` (max cowbell) beeps on every message
 * `/v` or `ctrl-n` hides names and makes wordwrap more obvious; good for viewing a wall of text that somebody pasted
+* `CTRL-L` or `/r` if rendering breaks
 
 ## other surprises
 
 * when running **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** it will extract a few bundled clients for your convenience (powershell and bash); look for the `[SFX] sfxdir: /tmp/pe-r0c.1000` message during startup, they'll be in a `clients` subfolder over there
 
   * if you installed r0c through `pip` instead then the clients will be somewhere crazy like `C:\Users\ed\AppData\Roaming\Python\share\doc\r0c\clients\powershell.ps1` or `/home/ed/.local/share/doc/r0c/clients/powershell.ps1`, good luck!
```

### Comparing `r0c-1.5.3/README.md` & `r0c-1.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
+* is not an irc server, but can bridge to/from irc servers
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
+## compatibility
+
+* 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
+* 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
 * notifications (bell/visual) on hilights and PMs
@@ -38,14 +44,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
+* bridge several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -142,13 +149,14 @@
 ## protips
 
 try the following commands and hotkeys after connecting:
 
 * `/cy` enables colored nicknames
 * `/b3` (max cowbell) beeps on every message
 * `/v` or `ctrl-n` hides names and makes wordwrap more obvious; good for viewing a wall of text that somebody pasted
+* `CTRL-L` or `/r` if rendering breaks
 
 ## other surprises
 
 * when running **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** it will extract a few bundled clients for your convenience (powershell and bash); look for the `[SFX] sfxdir: /tmp/pe-r0c.1000` message during startup, they'll be in a `clients` subfolder over there
 
   * if you installed r0c through `pip` instead then the clients will be somewhere crazy like `C:\Users\ed\AppData\Roaming\Python\share\doc\r0c\clients\powershell.ps1` or `/home/ed/.local/share/doc/r0c/clients/powershell.ps1`, good luck!
```

### Comparing `r0c-1.5.3/clients/bash.sh` & `r0c-1.6.0/clients/bash.sh`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/clients/powershell.ps1` & `r0c-1.6.0/clients/powershell.ps1`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/docs/help-commands.md` & `r0c-1.6.0/docs/help-commands.md`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 **`/r`** or **`/redraw`** or `CTRL-L` redraws the screen to fix corruption, use this if things are glitchy after resizing the window
 
 **`/sy`** and **`/sn`** turns on/off slowmo (avoids bug in telnet.exe on windows)
 
 **`/b1`** and **`/b0`** turns on/off audible alerts when someone mentions your name;  
 **`/b2`** makes it also trigger in active channels, and **`/b3`** beeps on any activity at all
 
+**`/hsy`** and **`/hsn`** turns on/off logging of hilights/mentions to the status channel
+
+**`/ey`** and **`/en`** turns on/off notifications on @all / @everyone in messages
+
 **`/cy`** and **`/cn`** turns on/off colored nicknames
 
 **`/my`** and **`/mn`** turns on/off wordwrap margins
 
 **`/v`** or **`/view`** or `CTRL-N` toggles visibility of names in messages
 
 **`/sw`** and **`/sh`** sets the terminal width/height in case the detection fails
```

### Comparing `r0c-1.5.3/docs/help-hotkeys.md` & `r0c-1.6.0/docs/help-hotkeys.md`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/docs/help-ui.md` & `r0c-1.6.0/docs/help-ui.md`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/docs/todo.md` & `r0c-1.6.0/docs/todo.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,17 @@
 # bugs: important
 
 * `nothing to see here`
 
 # bugs: whatever
 
 * wordwrap slices colour codes in half
-* powershell's vt100 impl is a glitchy mess
 * py2 deadlocks on quit with threadcapture running
 * channel cleanup doesn't happen unless user joins another channel after parting
-* check for queue buildups in general
 * colours don't carry over in wordwraps
-* wasteful redraws (text input before channel redraw etc)
 
 # done
 
 * config wizard
   * cp437
   * colors
   * stty
```

### Comparing `r0c-1.5.3/r0c/__init__.py` & `r0c-1.6.0/r0c/__init__.py`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/r0c/__main__.py` & `r0c-1.6.0/r0c/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from __future__ import print_function
 from .__version__ import S_VERSION
 from .__init__ import EP, WINDOWS, COLORS, unicode
 from . import util as Util
 from . import inetcat as Inetcat
 from . import itelnet as Itelnet
 from . import world as World
+from .irc import IRC_Net
 
 import os
 import sys
 import time
 import signal
 import select
 import threading
 from datetime import datetime
 
 print = Util.print
+UTC = Util.UTC
 
 
 """r0c.py: retr0chat Telnet/Netcat Server"""
 __author__ = "ed <a@ocv.me>"
 __credits__ = ["stackoverflow.com"]
 __license__ = "MIT"
 __copyright__ = 2018
@@ -44,35 +46,44 @@
     ac.add_argument("-pt", metavar="PORT", type=int, default=pt, help="telnet port (disable with 0)")
     ac.add_argument("-pn", metavar="PORT", type=int, default=pn, help="netcat port (disable with 0)")
     ac.add_argument("-tpt", metavar="PORT", type=int, default=0, help="TLS telnet port, e.g. 2424 (disable with 0)")
     ac.add_argument("-tpn", metavar="PORT", type=int, default=0, help="TLS netcat port, e.g. 1515 (disable with 0)")
     ac.add_argument("-pw", metavar="PWD", type=u, default=pwd, help="admin password")
     ac.add_argument("--ara", action="store_true", help="admin-access requires auth (even for localhost)")
     ac.add_argument("--nsalt", metavar="TXT", type=u, default="lammo/", help="salt for generated nicknames based on IP")
+    ac.add_argument("--proxy", metavar="A,A", type=u, default="", help="comma-sep. list of IPs which are relays to disable config persistence on")
 
     ac = ap.add_argument_group("logging")
     ac.add_argument("--log-rx", action="store_true", help="log incoming traffic from clients")
     ac.add_argument("--log-tx", action="store_true", help="log outgoing traffic to clients")
     ac.add_argument("--rot-msg", metavar="N", type=int, default=131072, help="max num msgs per logfile")
 
     ac = ap.add_argument_group("tls")
     ac.add_argument("--ciphers", metavar="S", type=u, default="", help="specify allowed TLS ciphers; python default if unset")
     ac.add_argument("--tls-min", metavar="S", type=u, default="", help="oldest ver to allow; SSLv3 TLSv1 TLSv1_1 TLSv1_2 TLSv1_3")
     ac.add_argument("--old-tls", action="store_true", help="support old clients (centos6/powershell), bad ciphers")
 
+    ac = ap.add_argument_group("irc-bridge")
+    ac.add_argument("--ircn", metavar="TXT", type=u, action="append", help='connect to an irc server; TXT is: "netname,hostname,[+]port,nick[,username[,password]]" (if password contains "," then use ", " as separator)')
+    ac.add_argument("--ircb", metavar="N,C,L", type=u, action="append", help="bridge irc-netname N, irc-channel #C with r0c-channel #L")
+    ac.add_argument("--i-rate", metavar="B,R", type=u, default="4,2", help="rate limit; burst of B messages, then R seconds between each")
+    ac.add_argument("--ctcp-ver", metavar="S", type=u, default="r0c v%s" % (S_VERSION), help="reply to CTCP VERSION")
+
     ac = ap.add_argument_group("ux")
     ac.add_argument("--no-all", action="store_true", help="default-disable @all / @everyone")
+    ac.add_argument("--motd", metavar="PATH", type=u, default="", help="file to include at the end of the welcome-text (can be edited at runtime)")
 
     ac = ap.add_argument_group("perf")
     ac.add_argument("--hist-rd", metavar="N", type=int, default=65535, help="max num msgs to load from disk when joining a channel")
     ac.add_argument("--hist-mem", metavar="N", type=int, default=98303, help="max num msgs to keep in channel scrollback")
     ac.add_argument("--hist-tsz", metavar="N", type=int, default=16384, help="num msgs to discard when chat exceeds hist-mem")
 
     ac = ap.add_argument_group("debug")
     ac.add_argument("--dbg", action="store_true", help="show negotiations etc")
+    ac.add_argument("--dbg-irc", action="store_true", help="show irc traffic")
     ac.add_argument("--hex-rx", action="store_true", help="print incoming traffic from clients")
     ac.add_argument("--hex-tx", action="store_true", help="print outgoing traffic to clients")
     ac.add_argument("--hex-lim", metavar="N", type=int, default=128, help="filter packets larger than N bytes from being hexdumped")
     ac.add_argument("--hex-w", metavar="N", type=int, default=16, help="width of the hexdump, in bytes per line, mod-8")
     ac.add_argument("--dev", action="store_true", help="enable dangerous shortcuts (devmode)")
     ac.add_argument("--thr-mon", action="store_true", help="start monitoring threads on ctrl-c")
     if WINDOWS:
@@ -105,15 +116,15 @@
         print()
         sys.exit(0)
 
     try:
         setattr(ap, "pt", int(argv[1]))
         setattr(ap, "pn", int(argv[2]))
         setattr(ap, "pw", unicode(argv[3]))
-    except:
+    except IndexError:
         pass
 
     return ap
 
 
 try:
     import argparse
@@ -192,14 +203,22 @@
         try:
             _ = int(argv[1])
             rap = run_fap
         except:
             rap = run_ap
 
         ar = self.ar = rap(argv, pwd)  # type: argparse.Namespace
+        ar.ircn = ar.ircn or []
+        ar.ircb = ar.ircb or []
+        ar.i_rate_b, ar.i_rate_s = [float(x) for x in ar.i_rate.split(",")]
+        ar.proxy = ar.proxy.split(",")
+        if "127.0.0.1" in ar.proxy or "::1" in ar.proxy:
+            t = "\033[33mWARNING: you have localhost in --proxy, you probably want --ara too\033[0m"
+            print(t)
+
         Util.HEX_WIDTH = ar.hex_w
         Itelnet.init(ar)
 
         cert = EP.app + "cert.pem"
         if ar.tpt or ar.tpn:
             print("  *  Loading certificate {0}".format(cert))
             import ssl
@@ -276,19 +295,68 @@
             target=self.push_worker,
             args=(self.world, self.servers),
             name="push",
         )
         # self.push_thr.daemon = True
         self.push_thr.start()
 
+        for irc_cfg in ar.ircn:
+            self.add_irc_net(irc_cfg)
+
+        for irc_cfg in ar.ircb:
+            self.add_irc_ch(irc_cfg)
+
+        for ircn in self.world.ircn.values():
+            ircn.connect()
+
         print("  *  Running")
         self.select_thr = Util.Daemon(self.select_worker, "selector")
 
         return True
 
+    def add_irc_net(self, scfg):
+        acfg = scfg.split(", " if ", " in scfg else ",")
+        try:
+            netname, hostname, sport, nick = acfg[:4]
+            netname = netname.lower()
+        except:
+            raise Exception("invalid argument to --ircn: [%s]" % (scfg,))
+
+        username = ""
+        password = ""
+        try:
+            username = acfg[4]
+            password = acfg[5]
+        except:
+            pass
+
+        port = int(sport.lstrip("+"))
+        tls = sport.startswith("+")
+
+        print("  *  Adding irc-net %s (%s:%s)" % (netname, hostname, sport))
+        self.world.ircn[netname] = IRC_Net(
+            self.world, netname, hostname, port, tls, nick, username, password
+        )
+
+    def add_irc_ch(self, scfg):
+        try:
+            netname, irc_cname, r0c_cname = scfg.lower().split(",")
+        except:
+            raise Exception("invalid argument to --ircb: [%s]" % (scfg,))
+
+        if netname not in self.world.ircn:
+            t = "ircnet '%s' (mentioned in --ircb %s) not defined by --ircn"
+            raise Exception(t % (netname, scfg))
+
+        t = "  *  Adding irc-bridge <%s:#%s> #%s"
+        print(t % (netname, irc_cname, r0c_cname))
+
+        ircn = self.world.ircn[netname]
+        ircn.addchan(irc_cname, r0c_cname)
+
     def run(self):
         print("  *  r0c is up  ^^,")
 
         if not self.ar.bench:
             try:
                 timeout = 69
                 if WINDOWS:
@@ -347,14 +415,16 @@
         return True
 
     def select_worker(self):
         srvs = {}
         for iface in self.servers:
             srvs[iface.srv_sck] = iface
 
+        t_fast = 0.5 if self.ar.ircn else 1
+
         sn = -1
         sc = {}
         slow = {}  # sck:cli
         fast = {}
         nfast = 0
         dirty_ref = 0
         next_slow = 0
@@ -371,15 +441,15 @@
                         if c.slowmo_tx or (c.wizard_stage is not None and not c.is_bot):
                             slow[c.sck] = c
                         else:
                             fast[c.sck] = c
 
                         sc[c.sck] = c
 
-                timeout = 0.2 if slow else 1 if fast else 69
+                timeout = 0.2 if slow else t_fast if fast else 69
 
             want_tx = [s for s, c in fast.items() if c.writable()]
             want_rx = [s for s, c in sc.items() if c.readable()]
             want_rx += list(srvs.keys())
 
             now = time.time()
             if slow and now >= next_slow:
@@ -456,15 +526,15 @@
             else:
                 c_refresh = 1
 
             with world.mutex:
                 if self.stopping:
                     break
 
-                zd = datetime.utcfromtimestamp(ts)
+                zd = datetime.fromtimestamp(ts, UTC)
                 date = u"%04d-%02d-%02d" % (zd.year, zd.month, zd.day)
 
                 if date != last_date:
                     if last_date:
                         world.broadcast_message(
                             u"\033[36mday changed to \033[1m{0}".format(date), False
                         )
```

### Comparing `r0c-1.5.3/r0c/chat.py` & `r0c-1.6.0/r0c/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # coding: utf-8
 from __future__ import print_function
 from .__init__ import TYPE_CHECKING
 from . import util as Util
+from .util import t2ymd_hms
 
 from datetime import datetime
 import calendar
 import operator
 
 if TYPE_CHECKING:
     from . import ivt100 as Ivt100
     from . import user as User
+    from .irc import IRC_Chan
 
 print = Util.print
+UTC = Util.UTC
 
 
 class NChannel(object):
     def __init__(self, name, topic):
         # type: (str, str) -> NChannel
         self.uchans = []  # type: list[UChannel]
         self.msgs = []  # type: list[Message]
         self.name = name
         self.topic = topic
         self.topic_bak = None
         self.user_act_ts = {}  # type: dict[str, int]  # str(nick) -> ts(last activity)
         self.usernames = u""  # sorted by activity
+        self.immortal = False  # has bridges
+        self.ircb = []  # type: list[IRC_Chan]
 
         self.log_fh = None  # active log file
         self.log_ctr = 0  # number of messages in file
 
     def get_name(self):
         if self.name:
             return u"#" + self.name
@@ -225,31 +230,31 @@
             self.txt[0] = ln
 
 
 class Message(object):
     def __init__(self, to, ts, user, txt):
         # type: (NChannel, int, str, str) -> Message
         self.ts = ts  # int timestamp; 1M msgs = 38MiB
-        self.dt = datetime.utcfromtimestamp(ts)  # 1M msgs = 53MiB
+        self.dt = datetime.fromtimestamp(ts, UTC)  # 1M msgs = 53MiB
         self.user = user  # str username
         self.txt = txt  # str text
 
         # set serial number based on last message in target
         if to and to.msgs:
             self.sno = to.msgs[-1].sno + 1
         else:
             self.sno = 0
 
     def __unicode__(self):
-        hhmmss = self.dt.strftime("%Y-%m%d-%H%M%S")
+        hhmmss = t2ymd_hms(self.dt, "%04d-%02d%02d-%02d%02d%02d")
         return u"Message {0:x} time({1},{2}) from({3}) body({4})".format(
             id(self), self.ts, hhmmss, self.user, self.txt
         )
 
     def __str__(self):
-        hhmmss = self.dt.strftime("%Y-%m%d-%H%M%S")
+        hhmmss = t2ymd_hms(self.dt, "%04d-%02d%02d-%02d%02d%02d")
         return "Message {0:x} time({1},{2}) from({3}) body({4})".format(
             id(self), self.ts, hhmmss, self.user, self.txt
         )
 
     def __repr__(self):
         return "Message({0}, '{1}', {2})".format(self.ts, self.user, repr(self.txt))
```

### Comparing `r0c-1.5.3/r0c/diag.py` & `r0c-1.6.0/r0c/diag.py`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/r0c/inetcat.py` & `r0c-1.6.0/r0c/inetcat.py`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/r0c/itelnet.py` & `r0c-1.6.0/r0c/itelnet.py`

 * *Files identical despite different names*

### Comparing `r0c-1.5.3/r0c/ivt100.py` & `r0c-1.6.0/r0c/ivt100.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # coding: utf-8
 from __future__ import print_function
 from .__init__ import EP, PY2, COLORS, IRONPY, TYPE_CHECKING, WINDOWS, unicode
 from . import util as Util
 from . import chat as Chat
 from . import user as User
+from .util import t2hms
 
 import os
 import re
 import time
 import zlib
 import socket
 import threading
 import binascii
 from datetime import datetime
 import operator
 
 print = Util.print
+UTC = Util.UTC
 
 # dont try-import ssl; avoids crash on systems with broken openssl libs
 ssl = None
 
 
 if PY2:
     from Queue import Queue
 else:
     from queue import Queue
 
 
 if TYPE_CHECKING:
     from . import world as World
+    from . import user as User
+    from .chat import Message, NChannel, UChannel
 
 
 class VT100_Server(object):
     def __init__(self, host, port, world, other_if, tls):
         global ssl
         if tls:
             import importlib
@@ -90,22 +94,14 @@
 
     def ipy__eq__(self, other):
         return id(self) == id(other)
 
     def ipy__ne__(self, other):
         return id(self) != id(other)
 
-    def con(self, msg, adr, add=0):
-        ht = time.strftime("%d/%m/%Y, %H:%M:%S")
-        print(
-            " {0} {1}  {2}  {3} :{4}".format(
-                msg, ht, len(self.clients) + add, adr[0], adr[1]
-            )
-        )
-
     def gen_remote(self, sck, addr, usr):
         if sck:
             raise RuntimeError("inherit me")
 
     def handle_error(self):
         Util.whoops()
 
@@ -298,14 +294,15 @@
         self.echo_on = False
         self.vt100 = True
         self.cnicks = False
         self.align = True
         self.view = False
         self.bell = 1
         self.atall = True
+        self.hilog = True
         self.crlf = u"\n"
         self.bps = 0
         self.codec = "utf-8"
         self.multibyte_codec = True
         self.inband_will_fail_decode = True
 
         self.wire_log = None
@@ -468,37 +465,42 @@
         self.linemode = False  # set true by buggy clients
         self.echo_on = False  # set true by buffy clients
         self.vt100 = True  # set nope by butty clients
         self.cnicks = False  # colored nicknames
         self.align = True  # fixed left margin
         self.bell = 1  # doot on hilights in other channels
         self.atall = not self.ar.no_all  # hilight on @all / @everyone
+        self.hilog = True  # hilights/mentions log in status chan
         self.crlf = u"\n"  # return key
         self.bps = 0  # will autodetect
         self.set_codec("utf-8")
 
     def load_config(self):
         load_ok = False
         with self.world.mutex:
             self.default_config()
             self.user.client = self
             self.user.admin = self.adr[0] == "127.0.0.1" and not self.ar.ara
 
             try:
+                if self.adr[0] in self.ar.proxy:
+                    raise Exception()
+
                 (
                     ts,
                     nick,
                     slowmo,
                     linemode,
                     vt100,
                     echo_on,
                     crlf,
                     codec,
                     bell,
                     atall,
+                    hilog,
                     cnicks,
                     align,
                 ) = self.host.user_config[self.adr[0]].split(u" ")
 
                 # print('],['.join([nick,linemode,vt100,echo_on,codec,bell]))
 
                 # terminal behavior
@@ -507,15 +509,16 @@
                 self.vt100 = 1 == int(vt100)
                 self.echo_on = 1 == int(echo_on)
                 self.crlf = binascii.unhexlify(crlf).decode("utf-8")
                 self.set_codec(codec)
 
                 # user config
                 self.bell = int(bell)
-                self.atall = int(atall)
+                self.atall = 1 == int(atall)
+                self.hilog = 1 == int(hilog)
                 self.cnicks = 1 == int(cnicks)
                 self.align = 1 == int(align)
 
                 if not self.world.find_user(nick):
                     self.user.set_nick(nick)
 
                 load_ok = True
@@ -546,14 +549,15 @@
                     u"1" if self.vt100 else u"0",
                     u"1" if self.echo_on else u"0",
                     binascii.hexlify(self.crlf.encode("utf-8")).decode("utf-8"),
                     self.codec,
                     # user config
                     unicode(self.bell),
                     u"1" if self.atall else u"0",
+                    u"1" if self.hilog else u"0",
                     u"1" if self.cnicks else u"0",
                     u"1" if self.align else u"0",
                 ]
             )
 
             try:
                 if self.host.user_config[self.adr[0]] == conf_str:
@@ -971,15 +975,16 @@
                 else:
                     cause = u"\nsomeone mentioned your nick in {0}.\n".format(ch_name)
 
             self.world.send_chan_msg(
                 u"-nfo-",
                 inf_n,
                 u"""[about notifications]{0}
-  to jump through unread channels,
+  to jump through unread channels
+  (or return to previous channel),
   press CTRL-E or use the command /a
 
   to disable audible alerts,
   use the command /b0
 """.format(
                     cause
                 ),
@@ -1007,15 +1012,15 @@
         if self.screen[0] != top_bar:
             self.screen[0] = top_bar
             return Util.trunc(top_bar, self.w)[0]
         return u""
 
     def update_status_bar(self, full_redraw):
         preface = u"\033[%dH\033[0;37;44;48;5;235m" % (self.h - self.y_status,)
-        hhmmss = datetime.utcnow().strftime("%H%M%S")
+        hhmmss = t2hms(datetime.now(UTC), "%02d%02d%02d")
         uchan = self.user.active_chan
         nchan = uchan.nchan
 
         # print('@@@ active chan = {0}, other chans {1}'.format(
         # 	self.user.active_chan.alias or self.user.active_chan.nchan.name,
         # 	u', '.join(x.alias or x.nchan.name for x in self.user.chans)))
 
@@ -1062,15 +1067,16 @@
 
         if nchan.name and self.vt100:
             online = u"\033[22;36m   %s" % (nchan.usernames,)
         else:
             online = u""
 
         line = Util.trunc(
-            u"%s%s   %s: \033[1;37m%s%s%s%s%s%s\033[K" % (
+            u"%s%s   %s: \033[1;37m%s%s%s%s%s%s\033[K"
+            % (
                 preface,
                 hhmmss,
                 nbuf,
                 chan_hash,
                 chan_name,
                 offscreen or u"",
                 hilights or u"",
@@ -2087,15 +2093,15 @@
                 to_say += enc_unicode.encode(self.codec, "backslashreplace")
                 to_say += b'"\r\n'
 
             to_say += (
                 u"""\
 \033[32m    this sentence is{0} green \033[0m
 """.format(
-                    u"" if self.vt100 else " NOT"
+                    u"" if self.vt100 else u" NOT"
                 )
                 .replace(u"\n", u"\r\n")
                 .encode("utf-8")
             )
 
             ok = "your client is OK"
             ng = "get better software"
@@ -2842,19 +2848,26 @@
                                 # this is a command
                                 self.user.exec_cmd(self.linebuf[1:])
                             else:
                                 if double:
                                     # remove escape character
                                     self.linebuf = self.linebuf[1:]
 
+                                nch = self.user.active_chan.nchan
                                 self.world.send_chan_msg(
                                     self.user.nick,
-                                    self.user.active_chan.nchan,
+                                    nch,
                                     Util.convert_color_codes(self.linebuf),
                                 )
+                                for ircb in nch.ircb:
+                                    t = Util.color_to_irc(self.linebuf)
+                                    ircb.net.say(
+                                        "PRIVMSG #%s :<%s> %s"
+                                        % (ircb.irc_cname, self.user.nick, t)
+                                    )
 
                             self.msg_hist_n = None
                             self.linebuf = u""
                             self.linepos = 0
 
                     elif act == "pgup" or act == "pgdn":
 
@@ -2879,14 +2892,24 @@
                         chan_shift = -1
                     elif act == "next-chan":
                         chan_shift = +1
                     elif act == "alt-tab":
                         self.user.exec_cmd("a")
                     elif act == "tab":
                         self.tabcomplete()
+                    elif act == "del":
+                        self.linepos += 1
+                        if self.linepos > len(self.linebuf):
+                            self.linepos = len(self.linebuf)
+                        if self.linepos > 0:
+                            self.linebuf = (
+                                self.linebuf[: self.linepos - 1]
+                                + self.linebuf[self.linepos :]
+                            )
+                            self.linepos -= 1
                     else:
                         print("unimplemented action: {0}".format(act))
 
                     if chan_shift != 0:
                         i = self.user.chans.index(self.user.active_chan) + chan_shift
                         if i < 0:
                             i = len(self.user.chans) - 1
```

### Comparing `r0c-1.5.3/r0c/user.py` & `r0c-1.6.0/r0c/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 # debug imports
 import code
 import gc
 
 if TYPE_CHECKING:
     from . import world as World
+    from .ivt100 import VT100_Client
 
 print = Util.print
 
 
 HELP_INTRO = u"""\
 Useful commands:
    \033[36m/nick\033[0m  change your nickname
@@ -65,15 +66,15 @@
 
 class User(object):
     def __init__(self, world, address):
         # type: (World.World, tuple[str, int]) -> User
         self.ar = world.ar
         self.world = world
         self.admin = False  # set true after challenge success
-        self.client = None  # the client which this object belongs to
+        self.client = None  # type: VT100_Client  # the connected client
         self.chans = []  # type: list[Chat.UChannel]
         self.active_chan = None  # type: Chat.UChannel
         self.new_active_chan = None  # set for channel change
         self.old_active_chan = None  # last focused channel
         self.nick = None  # type: str
         self.lnick = None  # type: str
         self.nick_re = None  # regex object for ping assert
@@ -168,14 +169,22 @@
             .replace(u"r0c_build", S_BUILD_DT)
             .replace(u"r0c_ver", S_VERSION)
             .replace(u"pad1", pad1)
             .replace(u"pad2", pad2)
         )
         text += HELP_INTRO
 
+        if self.ar.motd:
+            try:
+                with open(self.ar.motd, "rb") as f:
+                    text += f.read().replace(b"\r", b"").decode("utf-8", "replace")[:-1]
+            except Exception as ex:
+                t = "WARNING: could not read motd-file [%s]: %s"
+                print(t % (self.ar.motd, ex))
+
         # x = u"`1;30m░▒▓█▀▀▀▀`37m█▀`46m▓`0;1;30m▀▀▀▀█▓▒░`0;36m┌ "
         # text += x.replace(u"`", u"\033[") * 66
 
         uchan = self.world.join_priv_chan(self, u"r0c-status")
         nchan = uchan.nchan
         nchan.topic = u"r0c readme (and status info)"
 
@@ -318,18 +327,15 @@
                         False,
                     )
 
                 # update last-spoke tables
                 now = time.time()
                 for nchan in [x.nchan for x in self.chans]:
                     nchan.user_act_ts[new_nick] = now
-                    try:
-                        del nchan.user_act_ts[self.nick]
-                    except:
-                        pass
+                    nchan.user_act_ts.pop(self.nick, None)
                     nchan.update_usernames()
 
                 # update title in DM windows
                 for nchan in self.world.priv_ch:
                     for usr in nchan.uchans:
                         if usr.alias == self.nick:
                             usr.alias = new_nick
@@ -805,17 +811,17 @@
 
             else:
                 self.world.send_chan_msg(
                     u"-err-",
                     inf,
                     u"""[invalid arguments]
   usage:     /ss  lines_scrolled_per_pgup_pgdn
-  example:   /sh  0     (entire screen)
-  example:   /sh  10    (10 lines)
-  example:   /sh  50%   (half the screen)
+  example:   /ss  0     (entire screen)
+  example:   /ss  10    (10 lines)
+  example:   /ss  50%   (half the screen)
 """,
                 )
             return
 
         elif cmd in (u"b?", u"b0", u"b1", u"b2", u"b3"):
             zi = self.client.bell if cmd == u"b?" else int(cmd[1:])
             if zi == 0:
@@ -836,20 +842,32 @@
             t = u"Hilight on @all / @everyone enabled. Disable with /en"
             self.client.atall = True
             self.world.send_chan_msg(u"--", inf, t, False)
             self.build_nick_re()
             self.client.save_config()
 
         elif cmd == u"en":
-            t = u"Hilight on @all / @everyone disabled. Enable with /en"
+            t = u"Hilight on @all / @everyone disabled. Enable with /ey"
             self.client.atall = False
             self.world.send_chan_msg(u"--", inf, t, False)
             self.build_nick_re()
             self.client.save_config()
 
+        elif cmd == u"hsy":
+            t = u"Hilights/mentions-log in status channel enabled. Disable with /hsn"
+            self.client.hilog = True
+            self.world.send_chan_msg(u"--", inf, t, False)
+            self.client.save_config()
+
+        elif cmd == u"hsn":
+            t = u"Hilights/mentions-log in status channel disabled. Enable with /hsy"
+            self.client.hilog = False
+            self.world.send_chan_msg(u"--", inf, t, False)
+            self.client.save_config()
+
         elif cmd == u"cy":
             self.client.cnicks = True
             self.client.need_full_redraw = True
             self.world.send_chan_msg(
                 u"--", inf, u"Colored nicknames enabled. Disable with /cn", False
             )
             self.client.save_config()
```

### Comparing `r0c-1.5.3/r0c/util.py` & `r0c-1.6.0/r0c/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import traceback
 import threading
 import socket
 import struct
 import time
 import sys
 import os
+import re
 import platform
 import itertools
 from datetime import datetime
 
 
 print_mutex = threading.Lock()
 if PY2:
@@ -32,14 +33,36 @@
         range(70, 88),
         range(103, 124),
         range(132, 232),
     )
 )
 
 
+try:
+    from datetime import datetime, timezone
+
+    UTC = timezone.utc
+except:
+    from datetime import datetime, timedelta, tzinfo
+
+    TD_ZERO = timedelta(0)
+
+    class _UTC(tzinfo):
+        def utcoffset(self, dt):
+            return TD_ZERO
+
+        def tzname(self, dt):
+            return "UTC"
+
+        def dst(self, dt):
+            return TD_ZERO
+
+    UTC = _UTC()
+
+
 class Daemon(threading.Thread):
     def __init__(self, target, name=None, a=None):
         threading.Thread.__init__(self, target=target, args=a or (), name=name)
         self.daemon = True
         self.start()
 
 
@@ -48,15 +71,15 @@
     try:
         if not COLORS and u"\033" in args[0]:
             args[0] = strip_ansi(args[0])
     except:
         pass
 
     with print_mutex:
-        zd = datetime.utcnow()
+        zd = datetime.now(UTC)
         t = "%06d " % (
             (zd.hour * 100 + zd.minute) * 100 + zd.second,
             # zd.microsecond // 1000
         )
         builtins.print(
             t + str(args[0] if args else u"").replace(u"\n", u"\n" + t),
             *args[1:],
@@ -67,14 +90,34 @@
 def num(c):
     try:
         return int(c)
     except:
         return None
 
 
+def t2ymd(dt, fmt):
+    return fmt % (dt.year, dt.month, dt.day)
+
+
+def t2ymd_hm(dt, fmt):
+    return fmt % (dt.year, dt.month, dt.day, dt.hour, dt.minute)
+
+
+def t2ymd_hms(dt, fmt):
+    return fmt % (dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second)
+
+
+def t2hms(dt, fmt):
+    return fmt % (dt.hour, dt.minute, dt.second)
+
+
+def t2hm(dt, fmt):
+    return fmt % (dt.hour, dt.minute)
+
+
 def b2hex(data):
     if PY2:
         return " ".join(map(lambda b: format(ord(b), "02x"), data))
     else:
         if type(data) is str:
             return " ".join(map(lambda b: format(ord(b), "02x"), data))
         else:
@@ -428,22 +471,25 @@
             txt = u"%s%s%sm%s%s" % (txt[:ofs], fg, bg, preview_k, txt[resume_txt:])
         elif fg:
             txt = u"%s%sm%s%s" % (txt[:ofs], fg, preview_k, txt[resume_txt:])
         else:
             txt = u"%sK%s" % (txt[:ofs], txt[resume_txt:])
 
     scan_from = 0
+    is_bold = False
     while txt:
         ofs = txt.find(u"\x02", scan_from)
         if ofs < 0:
             break
 
         scan_from = ofs + 1
-        txt = u"%s\033[1m%s%s" % (
+        is_bold = not is_bold
+        txt = u"%s\033[%dm%s%s" % (
             txt[:ofs],
+            1 if is_bold else 22,
             u"B" if preview else u"",
             txt[scan_from:],
         )
 
     scan_from = 0
     while txt:
         ofs = txt.find(u"\x0f", scan_from)
@@ -456,14 +502,116 @@
             u"O" if preview else u"",
             txt[scan_from:],
         )
 
     return txt
 
 
+FG_TO_IRC = {}
+FG_FROM_IRC = {}
+for n, ch in enumerate(u"f0429153ba6ecd87"):
+    FG_FROM_IRC[n] = u"\x0b%s" % (ch,)
+    FG_TO_IRC[ch] = u"\x03%02d" % (n,)
+
+BG_TO_IRC = {}
+BG_FROM_IRC = {}
+for n, ch in enumerate(u"7042115332664507"):
+    BG_FROM_IRC[n] = u",%s" % (ch,)
+    BG_TO_IRC[ch] = u",%02d" % (n,)
+
+IRC_COLOR_RE = re.compile("^([0-9]{1,2})(,[0-9]{1,2})?")
+
+
+def color_to_irc(txt):
+    # mostly copy-pasted from `convert_color_codes`
+    foregrounds = FG_TO_IRC
+    backgrounds = BG_TO_IRC
+    scan_from = 0
+    while txt:
+        ofs = txt.find(u"\x0b", scan_from)
+        if ofs < 0:
+            break
+
+        scan_from = ofs + 1
+
+        fg = None
+        if len(txt) > ofs + 1:
+            fg = txt[ofs + 1]
+
+        bg = None
+        if len(txt) > ofs + 3 and txt[ofs + 2] == u",":
+            bg = txt[ofs + 3]
+
+        if fg in foregrounds:
+            fg = foregrounds[fg]
+        else:
+            fg = None
+            bg = None  # can't set bg without valid fg
+
+        if bg in backgrounds:
+            bg = backgrounds[bg]
+        else:
+            bg = None
+
+        resume_txt = ofs + 1
+        if fg:
+            resume_txt += 1
+            scan_from = len(fg) + 1
+        if bg:
+            resume_txt += 2
+            scan_from += len(bg)
+
+        if fg and bg:
+            txt = u"%s%s%s%s" % (txt[:ofs], fg, bg, txt[resume_txt:])
+        elif fg:
+            txt = u"%s%s%s" % (txt[:ofs], fg, txt[resume_txt:])
+        else:
+            txt = u"%s\x03%s" % (txt[:ofs], txt[resume_txt:])
+
+    # irc bold  == r0c, \x02
+    # irc reset == r0c, \x0f
+    return txt
+
+
+def color_from_irc(txt):
+    fgs = FG_FROM_IRC
+    bgs = BG_FROM_IRC
+    ptn = IRC_COLOR_RE
+    scan_from = 0
+    while txt:
+        ofs = txt.find(u"\x03", scan_from)
+        if ofs < 0:
+            break
+
+        fg = bg = ""
+        scan_from = ofs + 1
+        m = ptn.search(txt[scan_from : scan_from + 5])
+        if m:
+            i = int(m.group(1))
+            if i < 16:
+                fg = fgs[i]
+                if m.group(2):
+                    i = int(m.group(2)[1:])
+                    if i < 16:
+                        bg = bgs[i]
+
+                scan_from += len(m.group(0 if bg else 1))
+
+        if bg:
+            txt = u"%s%s%s%s" % (txt[:ofs], fg, bg, txt[scan_from:])
+        elif fg:
+            txt = u"%s%s%s" % (txt[:ofs], fg, txt[scan_from:])
+        else:
+            txt = u"%s\x0f%s" % (txt[:ofs], txt[scan_from:])
+            # no easy/cheap way to encode "keep boldness and reset color";
+            # `convert_color_codes` would then eat any following a..f
+
+    return txt
+
+
 """
 
 def visualize_all_unicode_codepoints_as_utf8():
     stats = [0] * 256
     nmax = sys.maxunicode + 1
     print("collecting all codepoints until {0}d, 0x{1:x}".format(nmax, nmax))
```

### Comparing `r0c-1.5.3/r0c/world.py` & `r0c-1.6.0/r0c/world.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 from __future__ import print_function
 from .__init__ import EP, PY2, INTERP, TYPE_CHECKING
 from . import util as Util
 from . import chat as Chat
+from .util import t2ymd_hm, t2ymd_hms
 
 import os
 import re
 import time
 import threading
 from datetime import datetime
 
@@ -14,16 +15,19 @@
     from Queue import Queue
 else:
     from queue import Queue
 
 if TYPE_CHECKING:
     from . import __main__ as Main
     from . import user as User
+    from .chat import NChannel, UChannel
+    from .irc import IRC_Chan, IRC_Net
 
 print = Util.print
+UTC = Util.UTC
 
 
 class World(object):
     def __init__(self, core):
         # type: (Main.Core) -> World
         self.core = core
         self.ar = core.ar
@@ -36,14 +40,18 @@
         self.cserial = 0  # selector configuration serial number
         self.task_queue = Queue()  # Delayed processing of expensive tasks
         self.mutex = threading.RLock()
         self.dirty_flag = threading.Event()  # raise after setting dirty_ch
         self.last_dirty = 0  # scheduler hint
         Util.py26_threading_event_wait(self.dirty_flag)
 
+        # irc bridges
+        self.ircn = {}  # type: dict[str, IRC_Net]  # netname:ircnet
+        self.ircb = {}  # type: dict[NChannel, IRC_Chan]
+
         # config
         self.messages_per_log_file = self.ar.rot_msg
 
         # stats for benchmarking
         self.num_joins = 0
         self.num_parts = 0
         self.num_messages = 0
@@ -114,14 +122,15 @@
                 # print('refreshing {0} for {1}'.format(nchan.get_name(), uchan.user.nick))
                 upd_users.add(uchan.user)
 
         for user in upd_users:
             user.client.refresh(False)
 
     def send_chan_msg(self, from_nick, nchan, text, ping_self=True):
+        # type: (str, NChannel, str, bool) -> None
         max_hist_mem = self.ar.hist_mem
         msg_trunc_size = self.ar.hist_tsz
         with self.mutex:
             self.num_messages += 1
             if nchan.name is None and not from_nick.startswith(u"-"):
                 # private chan, check if we have anyone to send to
                 if len(nchan.uchans) == 1:
@@ -157,14 +166,16 @@
 
             now = time.time()
             msg = Chat.Message(nchan, now, from_nick, text)
             nchan.msgs.append(msg)
             nchan.latest = msg.ts
 
             if not from_nick.startswith(u"-") and not from_nick == u"***":
+                if len(nchan.user_act_ts) > 9000:
+                    nchan.user_act_ts = {}
                 nchan.user_act_ts[from_nick] = now
                 nchan.update_usernames()
 
             if len(nchan.msgs) > max_hist_mem:
                 new_len = len(nchan.msgs) - msg_trunc_size
                 print(
                     " hist trunc:  [{0}] from {1} to {2}".format(
@@ -174,29 +185,32 @@
                 while new_len > max_hist_mem:
                     print("\033[1;31!!!\033[0m")
                     new_len -= msg_trunc_size
                 nchan.msgs = nchan.msgs[msg_trunc_size:]
 
             # self.refresh_chan(nchan)
             for uchan in nchan.uchans:
-                if nchan.name is None or uchan.user.nick_re.search(text):
-                    # if len(nchan.uchans) == 1:
-                    # 	break
-                    if PY2 and INTERP != "IronPython":
-                        if isinstance(uchan.user.nick, str):
-                            Util.whoops("uchan.user.nick is bytestring")
-                        if isinstance(from_nick, str):
-                            Util.whoops("from_nick is bytestring")
-
-                    if uchan.alias == u"r0c-status":
-                        if ping_self:
-                            uchan.last_ping = msg.sno
-                    else:
-                        if ping_self or uchan.user.nick != from_nick:
-                            uchan.last_ping = msg.sno
+                if nchan.name and not uchan.user.nick_re.search(text):
+                    continue
+
+                if PY2 and INTERP != "IronPython":
+                    if isinstance(uchan.user.nick, str):
+                        Util.whoops("uchan.user.nick is bytestring")
+                    if isinstance(from_nick, str):
+                        Util.whoops("from_nick is bytestring")
+
+                if uchan.alias != u"r0c-status" and uchan.user.nick != from_nick:
+                    uchan.last_ping = msg.sno
+                    if uchan.user.client.hilog and nchan.name:
+                        inf = self.get_priv_chan(uchan.user, u"r0c-status").nchan
+                        t = "you were mentioned in \033[1m#%s:\033[0m <%s> %s"
+                        t = t % (nchan.name, msg.user, msg.txt)
+                        self.send_chan_msg(u"-nfo-", inf, t, False)
+                elif ping_self:
+                    uchan.last_ping = msg.sno
 
             if nchan not in self.dirty_ch:
                 self.dirty_ch[nchan] = 1
                 self.dirty_flag.set()
 
             if nchan.log_fh:
                 # print('logrotate counter at {0}'.format(nchan.log_ctr))
@@ -221,55 +235,59 @@
                 if uchan.nchan == nchan:
                     return uchan
 
             self.num_joins += 1
             uchan = Chat.UChannel(user, nchan, alias)
             user.chans.append(uchan)
             nchan.uchans.append(uchan)
+            if len(nchan.user_act_ts) > 9000:
+                nchan.user_act_ts = {}
             nchan.user_act_ts[user.nick] = time.time()
             nchan.update_usernames()
             self.send_chan_msg(
                 u"--",
                 nchan,
                 u"\033[1;32m{0}\033[22m has joined".format(user.nick),
                 False,
             )
             if not alias:
                 uchan.last_read = -1
 
             return uchan
 
     def get_pub_chan(self, name):
+        # type: (str) -> NChannel
         for ch in self.pub_ch:
             if ch.name == name:
                 return ch
         return None
 
     def get_priv_chan(self, user, alias):
+        # type: (User.User, str) -> UChannel
         for ch in user.chans:
             if ch.alias == alias:
                 return ch
         return None
 
     def join_pub_chan(self, user, name):
+        # type: (User.User, str) -> Optional[UChannel]
         with self.mutex:
             name = name.strip().lower()
             nchan = self.get_pub_chan(name)
             if nchan is None:
+                st = t2ymd_hms(datetime.now(UTC), "%04d-%02d-%02d, %02d:%02d:%02dZ")
                 nchan = Chat.NChannel(
                     name, u"#{0} - no topic has been set".format(name)
                 )
                 nchan.msgs.append(
                     Chat.Message(
                         nchan,
                         time.time(),
                         u"--",
-                        u"\033[36mchannel created at \033[1m{0}".format(
-                            datetime.utcnow().strftime("%Y-%m-%d, %H:%M:%SZ")
-                        ),
+                        u"\033[36mchannel created at \033[1m%s" % (st,),
                     )
                 )
                 if nchan.name != u"scrolltest":
                     self.load_chat_log(nchan)
                     # self.task_queue.put([self.load_chat_log, [nchan], {}])
                 else:
                     for n1 in range(10):
@@ -282,16 +300,52 @@
 
                     txt = u"aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa " * 6
                     msg = Chat.Message(nchan, time.time(), u"--", txt)
                     nchan.msgs.append(msg)
 
                 self.pub_ch.append(nchan)
 
+            if not user:
+                nchan.immortal = True
+                return None
+
             ret = self.join_chan_obj(user, nchan)
             user.new_active_chan = ret
+            if user.client.hilog:
+                hls = []
+                nmsg = 0
+                ptn = user.nick_re
+                for msg in reversed(nchan.msgs):
+                    if len(hls) >= 50 or nmsg > 9000:
+                        break
+
+                    nmsg += 1
+                    if ptn.search(msg.txt):
+                        hls.append(msg)
+
+                inf = self.get_priv_chan(user, u"r0c-status").nchan
+                tf = "%d %ss ago (%s) you were mentioned in \033[1m#%s:\033[0m <%s> %s"
+                for msg in reversed(hls):
+                    dt = t2ymd_hm(msg.dt, "%04d-%02d-%02d %02d:%02d")
+                    td = int(time.time() - msg.ts)
+                    if td >= 172800:
+                        tu = "day"
+                        td //= 86400
+                    elif td >= 7200:
+                        tu = "hour"
+                        td //= 3600
+                    elif td >= 300:
+                        tu = "minute"
+                        td //= 60
+                    else:
+                        tu = "second"
+
+                    t = tf % (td, tu, dt, nchan.name, msg.user, msg.txt)
+                    self.send_chan_msg(u"-nfo-", inf, t, False)
+
             return ret
 
     def join_priv_chan(self, user, alias):
         with self.mutex:
             uchan = self.get_priv_chan(user, alias)
             if uchan is None:
                 nchan = Chat.NChannel(None, u"DM with [[uch_a]]")
@@ -362,15 +416,15 @@
             i = None
             if user.active_chan == uchan:
                 i = user.chans.index(uchan)
             user.chans.remove(uchan)
             nchan.uchans.remove(uchan)
 
             try:
-                del nchan.user_act_ts[user.nick]
+                nchan.user_act_ts.pop(user.nick, None)
                 nchan.update_usernames()
             except:
                 pass
 
             if i:
                 if len(user.chans) <= i:
                     i -= 1
@@ -383,15 +437,15 @@
 
                 self.send_chan_msg(
                     u"--",
                     nchan,
                     u"\033[1;33m{0}\033[22m has left{1}".format(user.nick, suf),
                 )
 
-            if not nchan.uchans:
+            if not nchan.uchans and not nchan.immortal:
                 print(" close chan:  [{0}]".format(nchan.get_name()))
 
                 if nchan.log_fh:
                     nchan.log_fh.close()
 
                 ch_list = self.pub_ch
                 if not nchan.name:
@@ -511,15 +565,15 @@
         # always mkdir because direction can turn on reconnect
         try:
             os.makedirs(log_dir)
         except:
             if not os.path.isdir(log_dir):
                 raise
 
-        ts = datetime.utcnow().strftime("%Y-%m%d-%H%M%S")
+        ts = t2ymd_hms(datetime.now(UTC), "%04d-%02d%02d-%02d%02d%02d")
         log_fn = u"{0}/{1}".format(log_dir, ts)
 
         while os.path.isfile(log_fn):
             log_fn += u"-"
 
         nchan.log_ctr = 0
         nchan.log_fh = open(log_fn, "wb")
```

### Comparing `r0c-1.5.3/r0c.egg-info/PKG-INFO` & `r0c-1.6.0/r0c.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r0c
-Version: 1.5.3
+Version: 1.6.0
 Summary: retr0chat telnet/vt100 chat server
 Home-page: https://github.com/9001/r0c
 Author: ed
 Author-email: r0c@ocv.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,23 +49,29 @@
 imagine being stuck on ancient gear, in the middle of nowhere, on a slow connection between machines that are even more archaic than the toaster you're trying to keep from falling apart
 
 retr0chat is the lightweight, no-dependencies, runs-anywhere solution for when life gives you lemons
 
 * tries to be irssi
 * zero dependencies on python 2.6, 2.7, 3.x
 * supports telnet, netcat, /dev/tcp, TLS clients
+* is not an irc server, but can bridge to/from irc servers
 * [modem-aware](https://ocv.me/r0c-2400.webm); comfortable at 1200 bps
 * fallbacks for inhumane conditions
   * linemode
   * no vt100 / ansi escape codes
 
 ## endorsements
 
 * the german federal office for information security [does not approve](https://ocv.me/stuff/r0c-bsi.png)
 
+## compatibility
+
+* 1980: [TVI 920C](https://a.ocv.me/pub/g/nerd-stuff/r0c-tvi-920c.jpg)
+* 1987: [IBM 3151](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.jpg) (also [video](https://a.ocv.me/pub/g/nerd-stuff/r0c-ibm-3151.webm)), using gnu-screen to translate VT100 sequences
+
 ## features
 
 irc-like:
 * public channels with persistent history (pgup/pgdn)
 * private messages (`/msg acidburn hey`)
 * nick completion with `Tab ↹`
 * notifications (bell/visual) on hilights and PMs
@@ -74,14 +80,15 @@
 
 technical:
 * client behavior detection (echo, colors, charset, newline)
 * message input with readline-like editing (arrow-left/right, home/end, backspace)
   * history of sent messages (arrow-up/down)
 * bandwidth-conservative (push/pop lines instead of full redraws; scroll-regions)
 * fast enough; 600 clients @ 750 msgs/sec, or 1'000 cli @ 350 msg/s
+* bridge several irc channels from several networks into one r0c channel
 
 ## windows clients
 
 * use [putty](https://the.earth.li/~sgtatham/putty/latest/w32/putty.exe) in telnet mode
 * or [the powershell client](https://github.com/9001/r0c/blob/master/clients/powershell.ps1)
 * or enable `Telnet Client` in control panel `->` programs `->` programs and features `->` turn windows features on or off, then press WIN+R and run `telnet r0c.int`
 
@@ -178,13 +185,14 @@
 ## protips
 
 try the following commands and hotkeys after connecting:
 
 * `/cy` enables colored nicknames
 * `/b3` (max cowbell) beeps on every message
 * `/v` or `ctrl-n` hides names and makes wordwrap more obvious; good for viewing a wall of text that somebody pasted
+* `CTRL-L` or `/r` if rendering breaks
 
 ## other surprises
 
 * when running **[r0c.py](https://github.com/9001/r0c/releases/latest/download/r0c.py)** it will extract a few bundled clients for your convenience (powershell and bash); look for the `[SFX] sfxdir: /tmp/pe-r0c.1000` message during startup, they'll be in a `clients` subfolder over there
 
   * if you installed r0c through `pip` instead then the clients will be somewhere crazy like `C:\Users\ed\AppData\Roaming\Python\share\doc\r0c\clients\powershell.ps1` or `/home/ed/.local/share/doc/r0c/clients/powershell.ps1`, good luck!
```

### Comparing `r0c-1.5.3/setup.py` & `r0c-1.6.0/setup.py`

 * *Files identical despite different names*

