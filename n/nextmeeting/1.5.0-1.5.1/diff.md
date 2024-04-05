# Comparing `tmp/nextmeeting-1.5.0.tar.gz` & `tmp/nextmeeting-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextmeeting-1.5.0.tar", max compression
+gzip compressed data, was "nextmeeting-1.5.1.tar", max compression
```

## Comparing `nextmeeting-1.5.0.tar` & `nextmeeting-1.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-09-29 18:26:44.726056 nextmeeting-1.5.0/LICENSE
--rw-r--r--   0        0        0     3561 2024-03-18 08:14:39.312984 nextmeeting-1.5.0/README.md
--rw-r--r--   0        0        0        0 2023-09-29 18:32:44.557415 nextmeeting-1.5.0/nextmeeting/__init__.py
--rwxr-xr-x   0        0        0    13769 2024-03-27 11:10:00.075284 nextmeeting-1.5.0/nextmeeting/cli.py
--rw-r--r--   0        0        0      829 2024-03-27 11:10:39.257505 nextmeeting-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 nextmeeting-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-29 18:26:44.726056 nextmeeting-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3561 2024-03-18 08:14:39.312984 nextmeeting-1.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-09-29 18:32:44.557415 nextmeeting-1.5.1/nextmeeting/__init__.py
+-rwxr-xr-x   0        0        0    13884 2024-04-05 07:42:01.288982 nextmeeting-1.5.1/nextmeeting/cli.py
+-rw-r--r--   0        0        0      829 2024-04-05 07:42:56.608385 nextmeeting-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 nextmeeting-1.5.1/PKG-INFO
```

### Comparing `nextmeeting-1.5.0/LICENSE` & `nextmeeting-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmeeting-1.5.0/README.md` & `nextmeeting-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nextmeeting-1.5.0/nextmeeting/cli.py` & `nextmeeting-1.5.1/nextmeeting/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 REG_TSV = re.compile(
     r"(?P<startdate>(\d{4})-(\d{2})-(\d{2}))\s*?(?P<starthour>(\d{2}:\d{2}))\s*(?P<enddate>(\d{4})-(\d{2})-(\d{2}))\s*?(?P<endhour>(\d{2}:\d{2}))\s*(?P<calendar_url>(https://\S+))\s*(?P<meet_url>(https://\S*)?)\s*(?P<title>.*)$"
 )
 DEFAULT_CALENDAR = os.environ.get("GCALCLI_DEFAULT_CALENDAR", "Work")
 GCALCLI_CMDLINE = f"gcalcli --nocolor --calendar={DEFAULT_CALENDAR} agenda today --nodeclined  --details=end --details=url --tsv "
 TITLE_ELIPSIS_LENGTH = 50
+MAX_CACHED_ENTRIES = 30
 NOTIFY_MIN_BEFORE_EVENTS = 5
 NOTIFY_MIN_COLOR = "#FF5733"  # red
 NOTIFY_MIN_COLOR_FOREGROUND = "#F4F1DE"  # white
 CACHE_DIR = pathlib.Path(os.path.expanduser("~/.cache/nextmeeting"))
 NOTIFY_PROGRAM: str = shutil.which("notify-send") or ""
 NOTIFY_ICON = "/usr/share/icons/hicolor/scalable/apps/org.gnome.Calendar.svg"
 GOOGLE_CALENDAR_PUBLIC_URL = "www.google.com/calendar"
@@ -230,14 +231,16 @@
             cached = json.load(f)
             if uuid in cached:
                 notified = True
     if notified:
         return
     cached.append(uuid)
     with cache_path.open("w") as f:
+        if cached >= MAX_CACHED_ENTRIES:
+            cached = cached[-MAX_CACHED_ENTRIES:]
         json.dump(cached, f)
     if NOTIFY_PROGRAM == "":
         return
     other_args = []
     if args.notify_expiry > 0:
         milliseconds = args.notify_expiry * 60 * 1000
         other_args += ["-t", str(milliseconds)]
```

### Comparing `nextmeeting-1.5.0/pyproject.toml` & `nextmeeting-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextmeeting"
-version = "1.5.0"
+version = "1.5.1"
 description = "Show your nextmeeting in your poly/waybar with gcalcli"
 authors = ["Chmouel Boudjnah <chmouel@chmouel.com>"]
 keywords = ["calendar", "cli"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/chmouel/nextmeeting"
 repository = "https://github.com/chmouel/nextmeeting"
```

### Comparing `nextmeeting-1.5.0/PKG-INFO` & `nextmeeting-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextmeeting
-Version: 1.5.0
+Version: 1.5.1
 Summary: Show your nextmeeting in your poly/waybar with gcalcli
 Home-page: https://github.com/chmouel/nextmeeting
 License: Apache-2.0
 Keywords: calendar,cli
 Author: Chmouel Boudjnah
 Author-email: chmouel@chmouel.com
 Requires-Python: >=3.9,<4.0
```

