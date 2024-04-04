# Comparing `tmp/xontrib-prompt-starship-0.3.5.tar.gz` & `tmp/xontrib-prompt-starship-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-prompt-starship-0.3.5.tar", last modified: Tue Mar 19 12:51:15 2024, max compression
+gzip compressed data, was "xontrib-prompt-starship-0.3.6.tar", last modified: Thu Apr  4 23:45:27 2024, max compression
```

## Comparing `xontrib-prompt-starship-0.3.5.tar` & `xontrib-prompt-starship-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:51:15.962860 xontrib-prompt-starship-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-19 12:51:06.000000 xontrib-prompt-starship-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-19 12:51:06.000000 xontrib-prompt-starship-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-19 12:51:15.962860 xontrib-prompt-starship-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-19 12:51:06.000000 xontrib-prompt-starship-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 12:51:15.962860 xontrib-prompt-starship-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-19 12:51:06.000000 xontrib-prompt-starship-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:51:15.962860 xontrib-prompt-starship-0.3.5/xontrib/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-19 12:51:06.000000 xontrib-prompt-starship-0.3.5/xontrib/prompt_starship.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:51:15.962860 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-19 12:51:15.000000 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-19 12:51:15.000000 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 12:51:15.000000 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-19 12:51:15.000000 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 12:51:15.000000 xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:45:27.645087 xontrib-prompt-starship-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 23:45:20.000000 xontrib-prompt-starship-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 23:45:20.000000 xontrib-prompt-starship-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-04 23:45:27.645087 xontrib-prompt-starship-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-04 23:45:20.000000 xontrib-prompt-starship-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:45:27.649087 xontrib-prompt-starship-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-04 23:45:20.000000 xontrib-prompt-starship-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:45:27.645087 xontrib-prompt-starship-0.3.6/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-04 23:45:20.000000 xontrib-prompt-starship-0.3.6/xontrib/prompt_starship.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:45:27.645087 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-04 23:45:27.000000 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 23:45:27.000000 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:45:27.000000 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 23:45:27.000000 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 23:45:27.000000 xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/top_level.txt
```

### Comparing `xontrib-prompt-starship-0.3.5/LICENSE` & `xontrib-prompt-starship-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-prompt-starship-0.3.5/PKG-INFO` & `xontrib-prompt-starship-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-starship
-Version: 0.3.5
+Version: 0.3.6
 Summary: Starship prompt in xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-starship
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-starship/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-starship
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-starship Version: 0.3.5 Summary:
+Metadata-Version: 2.1 Name: xontrib-prompt-starship Version: 0.3.6 Summary:
 Starship prompt in xonsh shell. Home-page: https://github.com/anki-code/
 xontrib-prompt-starship Author: anki-code Author-email: no@no.no License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-
 starship/blob/master/README.md Project-URL: Code, https://github.com/anki-code/
 xontrib-prompt-starship Project-URL: Issue tracker, https://github.com/anki-
 code/xontrib-prompt-starship/issues Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `xontrib-prompt-starship-0.3.5/README.md` & `xontrib-prompt-starship-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-prompt-starship-0.3.5/setup.py` & `xontrib-prompt-starship-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setuptools.setup(
     name='xontrib-prompt-starship',
-    version='0.3.5',
+    version='0.3.6',
     license='MIT',
     author='anki-code',
     author_email='no@no.no',
     description="Starship prompt in xonsh shell.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-prompt-starship-0.3.5/xontrib/prompt_starship.py` & `xontrib-prompt-starship-0.3.6/xontrib/prompt_starship.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Starship cross-shell prompt in xonsh shell. """
 
-import sys
-import os
-from pathlib import Path
+import sys as _sys
+from pathlib import Path as _Path
 
 
 __xonsh__.env['STARSHIP_SHELL'] = 'xonsh'
 __xonsh__.env['STARSHIP_SESSION_KEY'] = __xonsh__.subproc_captured_stdout(['starship','session']).strip()
 
 
 def _starship_prompt(cfg: str) -> None:
+    import os
     with __xonsh__.env.swap({'STARSHIP_CONFIG': cfg} if cfg else {}):
         return __xonsh__.subproc_captured_stdout([
             'starship', 'prompt',
             ('--status=' + (str(int( __xonsh__.history[-1].rtn)) if len(__xonsh__.history) > 0 else '0')),
             '--cmd-duration' , str(int((__xonsh__.history[-1].ts[1] - __xonsh__.history[-1].ts[0])*1000)) if len(__xonsh__.history) > 0 else '0',
             '--jobs', str(len(__xonsh__.all_jobs)),
             '--terminal-width', str(os.get_terminal_size().columns),
@@ -21,36 +21,36 @@
 
 
 _replace = __xonsh__.env.get('XONTRIB_PROMPT_STARSHIP_REPLACE_PROMPT' , True)
 
 
 _left_cfg  = __xonsh__.env.get('XONTRIB_PROMPT_STARSHIP_LEFT_CONFIG' , __xonsh__.env.get('STARSHIP_CONFIG' , ''))
 if _left_cfg:
-    _left_cfg = Path(_left_cfg).expanduser()
+    _left_cfg = _Path(_left_cfg).expanduser()
     if not _left_cfg.exists():
-        print(f"xontrib-prompt-starship: The path doesn't exist: {_left_cfg}", file=sys.stderr)
+        print(f"xontrib-prompt-starship: The path doesn't exist: {_left_cfg}", file=_sys.stderr)
 
 __xonsh__.env['PROMPT_FIELDS']['starship_left']	= lambda: _starship_prompt(_left_cfg)
 if _replace:
     __xonsh__.env['PROMPT'] = '{starship_left}'
 
 
 _right_cfg = __xonsh__.env.get('XONTRIB_PROMPT_STARSHIP_RIGHT_CONFIG', '')
 if _right_cfg:
-    _right_cfg = Path(_right_cfg).expanduser()
+    _right_cfg = _Path(_right_cfg).expanduser()
     if _right_cfg.exists():
         __xonsh__.env['PROMPT_FIELDS']['starship_right'] = lambda: _starship_prompt(_right_cfg)
         if _replace:
             __xonsh__.env['RIGHT_PROMPT'] = '{starship_right}'
     else:
-        print(f"xontrib-prompt-starship: The path doesn't exist: {_right_cfg}", file=sys.stderr)
+        print(f"xontrib-prompt-starship: The path doesn't exist: {_right_cfg}", file=_sys.stderr)
 
 
 _bottom_cfg = __xonsh__.env.get('XONTRIB_PROMPT_STARSHIP_BOTTOM_CONFIG', '')
 if _bottom_cfg:
-    _bottom_cfg = Path(_bottom_cfg).expanduser()
+    _bottom_cfg = _Path(_bottom_cfg).expanduser()
     if _bottom_cfg.exists():
         __xonsh__.env['PROMPT_FIELDS']['starship_bottom_toolbar'] = lambda: _starship_prompt(_bottom_cfg)
         if _replace:
             __xonsh__.env['BOTTOM_TOOLBAR'] = '{starship_bottom_toolbar}'
     else:
-        print(f"xontrib-prompt-starship: The path doesn't exist: {_bottom_cfg}", file=sys.stderr)
+        print(f"xontrib-prompt-starship: The path doesn't exist: {_bottom_cfg}", file=_sys.stderr)
```

### Comparing `xontrib-prompt-starship-0.3.5/xontrib_prompt_starship.egg-info/PKG-INFO` & `xontrib-prompt-starship-0.3.6/xontrib_prompt_starship.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-prompt-starship
-Version: 0.3.5
+Version: 0.3.6
 Summary: Starship prompt in xonsh shell.
 Home-page: https://github.com/anki-code/xontrib-prompt-starship
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-starship/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-prompt-starship
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xontrib-prompt-starship Version: 0.3.5 Summary:
+Metadata-Version: 2.1 Name: xontrib-prompt-starship Version: 0.3.6 Summary:
 Starship prompt in xonsh shell. Home-page: https://github.com/anki-code/
 xontrib-prompt-starship Author: anki-code Author-email: no@no.no License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xontrib-prompt-
 starship/blob/master/README.md Project-URL: Code, https://github.com/anki-code/
 xontrib-prompt-starship Project-URL: Issue tracker, https://github.com/anki-
 code/xontrib-prompt-starship/issues Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
```

