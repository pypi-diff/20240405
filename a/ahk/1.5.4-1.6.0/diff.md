# Comparing `tmp/ahk-1.5.4.tar.gz` & `tmp/ahk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.5.4.tar", last modified: Wed Apr  3 17:27:58 2024, max compression
+gzip compressed data, was "ahk-1.6.0.tar", last modified: Wed Apr  3 22:17:23 2024, max compression
```

## Comparing `ahk-1.5.4.tar` & `ahk-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 17:27:51.000000 ahk-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 17:27:51.000000 ahk-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-04-03 17:27:58.246258 ahk-1.5.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.242258 ahk-1.5.4/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.242258 ahk-1.5.4/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   207850 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    49795 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   170783 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   201130 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    44845 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    79868 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 17:27:51.000000 ahk-1.5.4/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-03 17:27:51.000000 ahk-1.5.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 17:27:51.000000 ahk-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 17:27:58.246258 ahk-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:27:51.000000 ahk-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.850993 ahk-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 22:17:17.000000 ahk-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 22:17:17.000000 ahk-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-03 22:17:23.850993 ahk-1.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.842993 ahk-1.6.0/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.846993 ahk-1.6.0/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207815 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49795 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30505 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.846993 ahk-1.6.0/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201095 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44845 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27712 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.850993 ahk-1.6.0/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-03 22:17:17.000000 ahk-1.6.0/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.850993 ahk-1.6.0/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-03 22:17:23.000000 ahk-1.6.0/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 22:17:23.000000 ahk-1.6.0/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:17:23.000000 ahk-1.6.0/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 22:17:23.000000 ahk-1.6.0/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 22:17:23.000000 ahk-1.6.0/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 22:17:17.000000 ahk-1.6.0/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:17:23.850993 ahk-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-04-03 22:17:17.000000 ahk-1.6.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 22:17:17.000000 ahk-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 22:17:23.850993 ahk-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:17:17.000000 ahk-1.6.0/setup.py
```

### Comparing `ahk-1.5.4/LICENSE` & `ahk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/PKG-INFO` & `ahk-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.5.4
+Version: 1.6.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
@@ -691,15 +691,15 @@
 Some of the notable differences that you may experience when using AutoHotkey v2 with this library include:
 
 1. Functions that find and return windows will often raise an exception rather than returning `None` (as in AutoHotkey v2, a TargetError is thrown in most cases where the window or control cannot be found)
 2. The behavior of `ControlSend` (`ahk.control_send` or `Window.send` or `Control.send`) differs in AutoHotkey v2 when the `control` parameter is not specified. In v1, keys are sent to the topmost controls, which is usually the correct behavior. In v2, keys are sent directly to the window. This means in many cases, you need to specify the control explicitly when using V2.
 3. Some functionality is not supported in v2 -- specifically: the `secondstowait` paramater for `TrayTip` (`ahk.show_traytip`) was removed in v2. Specifying this parameter in the Python wrapper will cause a warning to be emitted and the parameter is ignored.
 4. Some functionality that is present in v1 is not yet implemented in v2 -- this is expected to change in future versions. Specifically: some [sound functions](https://www.autohotkey.com/docs/v2/lib/Sound.htm) are not implemented.
 5. The default SendMode changes in v2 to `Input` rather than `Event` in v1 (as a consequence, for example, mouse speed parameters to `mouse_move` and `mouse_drag` will be ignored in V2 unless the send mode is changed)
-
+6. The default [TitleMatchMode](https://www.autohotkey.com/docs/v2/lib/SetTitleMatchMode.htm) is `2` in AutoHotkey v2. It is `1` in AutoHotkey v1. Use the `title_match_mode` keyword arguments to `win_get` and other methods that accept this keyword to control this behavior or use `set_title_match_mode` to change the default behavior (non-blocking calls are run in separate processes and are not affected by `set_title_match_mode`)
 
 ## Extending: add your own AutoHotkey code (beta)
 
 You can develop extensions for extending functionality of `ahk` -- that is: writing your own AutoHotkey code and adding
 additional methods to the AHK class. See the [extending docs](https://ahk.readthedocs.io/en/latest/extending.html) for
 more information.
```

### Comparing `ahk-1.5.4/ahk/__init__.py` & `ahk-1.6.0/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/_async/engine.py` & `ahk-1.6.0/ahk/_async/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,17 +413,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `ControlClick <https://www.autohotkey.com/docs/commands/ControlClick.htm>`_
         """
         args = [control, title, text, str(button), str(click_count), options, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -472,17 +472,17 @@
     ) -> Union[str, AsyncFutureResult[str]]:
         """
         Analog for `ControlGetText <https://www.autohotkey.com/docs/commands/ControlGetText.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -530,17 +530,17 @@
     ) -> Union[Position, AsyncFutureResult[Position]]:
         """
         Analog to `ControlGetPos <https://www.autohotkey.com/docs/commands/ControlGetPos.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -590,17 +590,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `ControlSend <https://www.autohotkey.com/docs/commands/ControlSend.htm>`_
         """
         args = [control, keys, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -647,17 +647,17 @@
         :param value: The setting value. ``True`` to turn on hidden window detection, ``False`` to turn it off.
         """
 
         if value not in (True, False):
             raise TypeError(f'detect hidden windows must be a boolean, got object of type {type(value)}')
         args = []
         if value is True:
-            args.append('On')
+            args.append('1')
         else:
-            args.append('Off')
+            args.append('0')
         await self._transport.function_call('AHKSetDetectHiddenWindows', args=args)
         return None
 
     @staticmethod
     def _format_win_args(
         title: str,
         text: str,
@@ -665,17 +665,17 @@
         exclude_text: str,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
     ) -> List[str]:
         args = [title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -874,15 +874,15 @@
         exclude_title: str = '',
         exclude_text: str = '',
         exact: Optional[bool] = None,
     ) -> List[AsyncWindow]:
         if exact is not None and title_match_mode is not None:
             raise TypeError('exact and match_mode parameters are mutually exclusive')
         if exact is not None:
-            warnings.warn('exact parameter is deprecated. Use match_mode=3 instead', stacklevel=2)
+            warnings.warn('exact parameter is deprecated. Use title_match_mode instead', stacklevel=2)
             if exact:
                 title_match_mode = (3, 'Fast')
             else:
                 title_match_mode = (1, 'Fast')
         elif title_match_mode is None:
             title_match_mode = (1, 'Fast')
 
@@ -2224,17 +2224,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `WinSetTitle <https://www.autohotkey.com/docs/commands/WinSetTitle.htm>`_
         """
         args = [new_title, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2282,17 +2282,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `AlwaysOnTop subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#AlwaysOnTop>`_
         """
         args = [str(toggle), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2517,17 +2517,17 @@
         """
         Analog for `Style subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Style>`_
         """
 
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2575,17 +2575,17 @@
     ) -> Union[bool, AsyncFutureResult[bool]]:
         """
         Analog for `ExStyle subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#ExStyle>`_
         """
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2633,17 +2633,17 @@
     ) -> Union[bool, AsyncFutureResult[bool]]:
         """
         Analog for `Region subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Region>`_
         """
         args = [options, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2691,17 +2691,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `Transparent subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Transparent>`_
         """
         args = [str(transparency), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2749,17 +2749,17 @@
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `TransColor subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#TransColor>`_
         """
         args = [str(color), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
```

### Comparing `ahk-1.5.4/ahk/_async/transport.py` & `ahk-1.6.0/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/_async/window.py` & `ahk-1.6.0/ahk/_async/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 from typing import Coroutine
 from typing import Literal
 from typing import Optional
 from typing import overload
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
+from typing import TypedDict
 from typing import TypeVar
 from typing import Union
 
 from ahk.message import Position
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
+if sys.version_info < (3, 11):
+    from typing_extensions import NotRequired
+else:
+    from typing import NotRequired
+
 if TYPE_CHECKING:
     from .engine import AsyncAHK
     from .transport import AsyncFutureResult
 
 
 class WindowNotFoundException(Exception): ...
 
@@ -648,93 +654,108 @@
         return await engine.win_get(title=f'ahk_pid {pid}')
 
     @classmethod
     async def from_mouse_position(cls, engine: AsyncAHK[Any]) -> Optional[AsyncWindow]:
         return await engine.win_get_from_mouse_position()
 
 
+_ControlTargetKwargs = TypedDict('_ControlTargetKwargs', {'title': str, 'control': NotRequired[str]})
+
+
 class AsyncControl:
     def __init__(self, window: AsyncWindow, hwnd: str, control_class: str):
         self.window: AsyncWindow = window
         self.hwnd: str = hwnd
         self.control_class: str = control_class
         self._engine = window._engine
+        self.use_hwnd: bool = False
+
+    def _get_target_params(self, use_hwnd: Optional[bool] = None) -> _ControlTargetKwargs:
+        if use_hwnd is None:
+            use_hwnd = self.use_hwnd
+        if use_hwnd:
+            return {'title': f'ahk_id {self.hwnd}'}
+        else:
+            return {'title': f'ahk_id {self.window._ahk_id}', 'control': self.control_class}
 
     # fmt: off
     @overload
-    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '') -> None: ...
+    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None) -> None: ...
     @overload
-    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: Literal[False]) -> AsyncFutureResult[None]: ...
+    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
-    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: Literal[True]) -> None: ...
+    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> None: ...
     @overload
-    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    async def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def click(
         self,
         *,
         button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L',
         click_count: int = 1,
         options: str = '',
+        use_hwnd: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
         return await self._engine.control_click(
             button=button,
-            control=self.control_class,
             click_count=click_count,
             options=options,
-            title=f'ahk_id {self.window._ahk_id}',
             title_match_mode=(1, 'Fast'),
             detect_hidden_windows=True,
             blocking=blocking,
+            **self._get_target_params(use_hwnd),
         )
 
     # fmt: off
     @overload
-    async def send(self, keys: str) -> None: ...
+    async def send(self, keys: str, *, use_hwnd: Optional[bool] = None) -> None: ...
     @overload
-    async def send(self, keys: str, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
+    async def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
-    async def send(self, keys: str, *, blocking: Literal[True]) -> None: ...
+    async def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> None: ...
     @overload
-    async def send(self, keys: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    async def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
-    async def send(self, keys: str, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]:
+    async def send(
+        self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[None, AsyncFutureResult[None]]:
         return await self._engine.control_send(
             keys=keys,
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
-    async def get_text(self, blocking: bool = True) -> Union[str, AsyncFutureResult[str]]:
+    async def get_text(
+        self, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[str, AsyncFutureResult[str]]:
         return await self._engine.control_get_text(
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
     # fmt: off
     @overload
-    async def get_position(self) -> Position: ...
+    async def get_position(self, *, use_hwnd: Optional[bool] = None) -> Position: ...
     @overload
-    async def get_position(self, blocking: Literal[False]) -> AsyncFutureResult[Position]: ...
+    async def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> AsyncFutureResult[Position]: ...
     @overload
-    async def get_position(self, blocking: Literal[True]) -> Position: ...
+    async def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> Position: ...
     @overload
-    async def get_position(self, blocking: bool = True) -> Union[Position, AsyncFutureResult[Position]]: ...
+    async def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[Position, AsyncFutureResult[Position]]: ...
     # fmt: on
-    async def get_position(self, blocking: bool = True) -> Union[Position, AsyncFutureResult[Position]]:
+    async def get_position(
+        self, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[Position, AsyncFutureResult[Position]]:
         return await self._engine.control_get_position(
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} window={self.window!r}, control_hwnd={self.hwnd!r}, control_class={self.control_class!r}>'
```

### Comparing `ahk-1.5.4/ahk/_constants.py` & `ahk-1.6.0/ahk/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -5490,14 +5490,23 @@
         SetTitleMatchMode(match_speed)
     }
     current_detect_hw := Format("{}", A_DetectHiddenWindows)
 
     if (detect_hw != "") {
         DetectHiddenWindows(detect_hw)
     }
+    if (width = "" or height = "") {
+        WinGetPos(&_, &__, &w, &h, title, text, extitle, extext)
+        if (width = "") {
+            width := w
+        }
+        if (height = "") {
+            height := h
+        }
+    }
 
     try {
         WinMove(x, y, width, height, title, text, extitle, extext)
     }
     finally {
         DetectHiddenWindows(current_detect_hw)
         SetTitleMatchMode(current_match_mode)
```

### Comparing `ahk-1.5.4/ahk/_hotkey.py` & `ahk-1.6.0/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/_sync/engine.py` & `ahk-1.6.0/ahk/_sync/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,17 +408,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `ControlClick <https://www.autohotkey.com/docs/commands/ControlClick.htm>`_
         """
         args = [control, title, text, str(button), str(click_count), options, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -467,17 +467,17 @@
     ) -> Union[str, FutureResult[str]]:
         """
         Analog for `ControlGetText <https://www.autohotkey.com/docs/commands/ControlGetText.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -525,17 +525,17 @@
     ) -> Union[Position, FutureResult[Position]]:
         """
         Analog to `ControlGetPos <https://www.autohotkey.com/docs/commands/ControlGetPos.htm>`_
         """
         args = [control, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -585,17 +585,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `ControlSend <https://www.autohotkey.com/docs/commands/ControlSend.htm>`_
         """
         args = [control, keys, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -642,17 +642,17 @@
         :param value: The setting value. ``True`` to turn on hidden window detection, ``False`` to turn it off.
         """
 
         if value not in (True, False):
             raise TypeError(f'detect hidden windows must be a boolean, got object of type {type(value)}')
         args = []
         if value is True:
-            args.append('On')
+            args.append('1')
         else:
-            args.append('Off')
+            args.append('0')
         self._transport.function_call('AHKSetDetectHiddenWindows', args=args)
         return None
 
     @staticmethod
     def _format_win_args(
         title: str,
         text: str,
@@ -660,17 +660,17 @@
         exclude_text: str,
         title_match_mode: Optional[TitleMatchMode] = None,
         detect_hidden_windows: Optional[bool] = None,
     ) -> List[str]:
         args = [title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -862,15 +862,15 @@
         exclude_title: str = '',
         exclude_text: str = '',
         exact: Optional[bool] = None,
     ) -> List[Window]:
         if exact is not None and title_match_mode is not None:
             raise TypeError('exact and match_mode parameters are mutually exclusive')
         if exact is not None:
-            warnings.warn('exact parameter is deprecated. Use match_mode=3 instead', stacklevel=2)
+            warnings.warn('exact parameter is deprecated. Use title_match_mode instead', stacklevel=2)
             if exact:
                 title_match_mode = (3, 'Fast')
             else:
                 title_match_mode = (1, 'Fast')
         elif title_match_mode is None:
             title_match_mode = (1, 'Fast')
 
@@ -2212,17 +2212,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `WinSetTitle <https://www.autohotkey.com/docs/commands/WinSetTitle.htm>`_
         """
         args = [new_title, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2270,17 +2270,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `AlwaysOnTop subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#AlwaysOnTop>`_
         """
         args = [str(toggle), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2505,17 +2505,17 @@
         """
         Analog for `Style subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Style>`_
         """
 
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2563,17 +2563,17 @@
     ) -> Union[bool, FutureResult[bool]]:
         """
         Analog for `ExStyle subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#ExStyle>`_
         """
         args = [style, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2621,17 +2621,17 @@
     ) -> Union[bool, FutureResult[bool]]:
         """
         Analog for `Region subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Region>`_
         """
         args = [options, title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2679,17 +2679,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `Transparent subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#Transparent>`_
         """
         args = [str(transparency), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
@@ -2737,17 +2737,17 @@
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `TransColor subcommand of WinSet <https://www.autohotkey.com/docs/v1/lib/WinSet.htm#TransColor>`_
         """
         args = [str(color), title, text, exclude_title, exclude_text]
         if detect_hidden_windows is not None:
             if detect_hidden_windows is True:
-                args.append('On')
+                args.append('1')
             elif detect_hidden_windows is False:
-                args.append('Off')
+                args.append('0')
             else:
                 raise TypeError(
                     f'Invalid value for parameter detect_hidden_windows. Expected boolean or None, got {detect_hidden_windows!r}'
                 )
         else:
             args.append('')
         if title_match_mode is not None:
```

### Comparing `ahk-1.5.4/ahk/_sync/transport.py` & `ahk-1.6.0/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/_sync/window.py` & `ahk-1.6.0/ahk/_sync/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 from typing import Coroutine
 from typing import Literal
 from typing import Optional
 from typing import overload
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
+from typing import TypedDict
 from typing import TypeVar
 from typing import Union
 
 from ahk.message import Position
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
+if sys.version_info < (3, 11):
+    from typing_extensions import NotRequired
+else:
+    from typing import NotRequired
+
 if TYPE_CHECKING:
     from .engine import AHK
     from .transport import FutureResult
 
 
 class WindowNotFoundException(Exception): ...
 
@@ -627,93 +633,108 @@
         return engine.win_get(title=f'ahk_pid {pid}')
 
     @classmethod
     def from_mouse_position(cls, engine: AHK[Any]) -> Optional[Window]:
         return engine.win_get_from_mouse_position()
 
 
+_ControlTargetKwargs = TypedDict('_ControlTargetKwargs', {'title': str, 'control': NotRequired[str]})
+
+
 class Control:
     def __init__(self, window: Window, hwnd: str, control_class: str):
         self.window: Window = window
         self.hwnd: str = hwnd
         self.control_class: str = control_class
         self._engine = window._engine
+        self.use_hwnd: bool = False
+
+    def _get_target_params(self, use_hwnd: Optional[bool] = None) -> _ControlTargetKwargs:
+        if use_hwnd is None:
+            use_hwnd = self.use_hwnd
+        if use_hwnd:
+            return {'title': f'ahk_id {self.hwnd}'}
+        else:
+            return {'title': f'ahk_id {self.window._ahk_id}', 'control': self.control_class}
 
     # fmt: off
     @overload
-    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '') -> None: ...
+    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None) -> None: ...
     @overload
-    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: Literal[False]) -> FutureResult[None]: ...
+    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
-    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: Literal[True]) -> None: ...
+    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> None: ...
     @overload
-    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    def click(self, *, button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L', click_count: int = 1, options: str = '', use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def click(
         self,
         *,
         button: Literal['L', 'R', 'M', 'LEFT', 'RIGHT', 'MIDDLE'] = 'L',
         click_count: int = 1,
         options: str = '',
+        use_hwnd: Optional[bool] = None,
         blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
         return self._engine.control_click(
             button=button,
-            control=self.control_class,
             click_count=click_count,
             options=options,
-            title=f'ahk_id {self.window._ahk_id}',
             title_match_mode=(1, 'Fast'),
             detect_hidden_windows=True,
             blocking=blocking,
+            **self._get_target_params(use_hwnd),
         )
 
     # fmt: off
     @overload
-    def send(self, keys: str) -> None: ...
+    def send(self, keys: str, *, use_hwnd: Optional[bool] = None) -> None: ...
     @overload
-    def send(self, keys: str, *, blocking: Literal[False]) -> FutureResult[None]: ...
+    def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
-    def send(self, keys: str, *, blocking: Literal[True]) -> None: ...
+    def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> None: ...
     @overload
-    def send(self, keys: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    def send(self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
-    def send(self, keys: str, *, blocking: bool = True) -> Union[None, FutureResult[None]]:
+    def send(
+        self, keys: str, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[None, FutureResult[None]]:
         return self._engine.control_send(
             keys=keys,
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
-    def get_text(self, blocking: bool = True) -> Union[str, FutureResult[str]]:
+    def get_text(
+        self, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[str, FutureResult[str]]:
         return self._engine.control_get_text(
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
     # fmt: off
     @overload
-    def get_position(self) -> Position: ...
+    def get_position(self, *, use_hwnd: Optional[bool] = None) -> Position: ...
     @overload
-    def get_position(self, blocking: Literal[False]) -> FutureResult[Position]: ...
+    def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: Literal[False]) -> FutureResult[Position]: ...
     @overload
-    def get_position(self, blocking: Literal[True]) -> Position: ...
+    def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: Literal[True]) -> Position: ...
     @overload
-    def get_position(self, blocking: bool = True) -> Union[Position, FutureResult[Position]]: ...
+    def get_position(self, *, use_hwnd: Optional[bool] = None, blocking: bool = True) -> Union[Position, FutureResult[Position]]: ...
     # fmt: on
-    def get_position(self, blocking: bool = True) -> Union[Position, FutureResult[Position]]:
+    def get_position(
+        self, *, use_hwnd: Optional[bool] = None, blocking: bool = True
+    ) -> Union[Position, FutureResult[Position]]:
         return self._engine.control_get_position(
-            control=self.control_class,
-            title=f'ahk_id {self.window._ahk_id}',
             blocking=blocking,
             detect_hidden_windows=True,
             title_match_mode=(1, 'Fast'),
+            **self._get_target_params(use_hwnd),
         )
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} window={self.window!r}, control_hwnd={self.hwnd!r}, control_class={self.control_class!r}>'
```

### Comparing `ahk-1.5.4/ahk/_utils.py` & `ahk-1.6.0/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/directives.py` & `ahk-1.6.0/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/extensions.py` & `ahk-1.6.0/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/keys.py` & `ahk-1.6.0/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/message.py` & `ahk-1.6.0/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/templates/daemon-v2.ahk` & `ahk-1.6.0/ahk/templates/daemon-v2.ahk`

 * *Files 1% similar despite different names*

```diff
@@ -2500,14 +2500,23 @@
         SetTitleMatchMode(match_speed)
     }
     current_detect_hw := Format("{}", A_DetectHiddenWindows)
 
     if (detect_hw != "") {
         DetectHiddenWindows(detect_hw)
     }
+    if (width = "" or height = "") {
+        WinGetPos(&_, &__, &w, &h, title, text, extitle, extext)
+        if (width = "") {
+            width := w
+        }
+        if (height = "") {
+            height := h
+        }
+    }
 
     try {
         WinMove(x, y, width, height, title, text, extitle, extext)
     }
     finally {
         DetectHiddenWindows(current_detect_hw)
         SetTitleMatchMode(current_match_mode)
```

### Comparing `ahk-1.5.4/ahk/templates/daemon.ahk` & `ahk-1.6.0/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/templates/hotkeys-v2.ahk` & `ahk-1.6.0/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk/templates/hotkeys.ahk` & `ahk-1.6.0/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/ahk.egg-info/PKG-INFO` & `ahk-1.6.0/ahk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.5.4
+Version: 1.6.0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
@@ -691,15 +691,15 @@
 Some of the notable differences that you may experience when using AutoHotkey v2 with this library include:
 
 1. Functions that find and return windows will often raise an exception rather than returning `None` (as in AutoHotkey v2, a TargetError is thrown in most cases where the window or control cannot be found)
 2. The behavior of `ControlSend` (`ahk.control_send` or `Window.send` or `Control.send`) differs in AutoHotkey v2 when the `control` parameter is not specified. In v1, keys are sent to the topmost controls, which is usually the correct behavior. In v2, keys are sent directly to the window. This means in many cases, you need to specify the control explicitly when using V2.
 3. Some functionality is not supported in v2 -- specifically: the `secondstowait` paramater for `TrayTip` (`ahk.show_traytip`) was removed in v2. Specifying this parameter in the Python wrapper will cause a warning to be emitted and the parameter is ignored.
 4. Some functionality that is present in v1 is not yet implemented in v2 -- this is expected to change in future versions. Specifically: some [sound functions](https://www.autohotkey.com/docs/v2/lib/Sound.htm) are not implemented.
 5. The default SendMode changes in v2 to `Input` rather than `Event` in v1 (as a consequence, for example, mouse speed parameters to `mouse_move` and `mouse_drag` will be ignored in V2 unless the send mode is changed)
-
+6. The default [TitleMatchMode](https://www.autohotkey.com/docs/v2/lib/SetTitleMatchMode.htm) is `2` in AutoHotkey v2. It is `1` in AutoHotkey v1. Use the `title_match_mode` keyword arguments to `win_get` and other methods that accept this keyword to control this behavior or use `set_title_match_mode` to change the default behavior (non-blocking calls are run in separate processes and are not affected by `set_title_match_mode`)
 
 ## Extending: add your own AutoHotkey code (beta)
 
 You can develop extensions for extending functionality of `ahk` -- that is: writing your own AutoHotkey code and adding
 additional methods to the AHK class. See the [extending docs](https://ahk.readthedocs.io/en/latest/extending.html) for
 more information.
```

### Comparing `ahk-1.5.4/ahk.egg-info/SOURCES.txt` & `ahk-1.6.0/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/buildunasync.py` & `ahk-1.6.0/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.4/docs/README.md` & `ahk-1.6.0/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -660,15 +660,15 @@
 Some of the notable differences that you may experience when using AutoHotkey v2 with this library include:
 
 1. Functions that find and return windows will often raise an exception rather than returning `None` (as in AutoHotkey v2, a TargetError is thrown in most cases where the window or control cannot be found)
 2. The behavior of `ControlSend` (`ahk.control_send` or `Window.send` or `Control.send`) differs in AutoHotkey v2 when the `control` parameter is not specified. In v1, keys are sent to the topmost controls, which is usually the correct behavior. In v2, keys are sent directly to the window. This means in many cases, you need to specify the control explicitly when using V2.
 3. Some functionality is not supported in v2 -- specifically: the `secondstowait` paramater for `TrayTip` (`ahk.show_traytip`) was removed in v2. Specifying this parameter in the Python wrapper will cause a warning to be emitted and the parameter is ignored.
 4. Some functionality that is present in v1 is not yet implemented in v2 -- this is expected to change in future versions. Specifically: some [sound functions](https://www.autohotkey.com/docs/v2/lib/Sound.htm) are not implemented.
 5. The default SendMode changes in v2 to `Input` rather than `Event` in v1 (as a consequence, for example, mouse speed parameters to `mouse_move` and `mouse_drag` will be ignored in V2 unless the send mode is changed)
-
+6. The default [TitleMatchMode](https://www.autohotkey.com/docs/v2/lib/SetTitleMatchMode.htm) is `2` in AutoHotkey v2. It is `1` in AutoHotkey v1. Use the `title_match_mode` keyword arguments to `win_get` and other methods that accept this keyword to control this behavior or use `set_title_match_mode` to change the default behavior (non-blocking calls are run in separate processes and are not affected by `set_title_match_mode`)
 
 ## Extending: add your own AutoHotkey code (beta)
 
 You can develop extensions for extending functionality of `ahk` -- that is: writing your own AutoHotkey code and adding
 additional methods to the AHK class. See the [extending docs](https://ahk.readthedocs.io/en/latest/extending.html) for
 more information.
```

### Comparing `ahk-1.5.4/setup.cfg` & `ahk-1.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.5.4
+version = 1.6.0
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

