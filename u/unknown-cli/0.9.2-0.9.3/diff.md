# Comparing `tmp/unknown-cli-0.9.2.tar.gz` & `tmp/unknown-cli-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknown-cli-0.9.2.tar", last modified: Thu Mar 14 21:55:44 2024, max compression
+gzip compressed data, was "unknown-cli-0.9.3.tar", last modified: Fri Apr  5 17:28:53 2024, max compression
```

## Comparing `unknown-cli-0.9.2.tar` & `unknown-cli-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-03-14 21:55:44.333763 unknown-cli-0.9.2/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-03-14 21:55:44.331762 unknown-cli-0.9.2/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       30 2023-09-08 21:53:36.000000 unknown-cli-0.9.2/README.md
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       38 2024-03-14 21:55:44.333763 unknown-cli-0.9.2/setup.cfg
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2695 2024-03-13 22:40:13.000000 unknown-cli-0.9.2/setup.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-03-14 21:55:44.198387 unknown-cli-0.9.2/unknown_cli.egg-info/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      561 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        1 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       83 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      130 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/requires.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       11 2024-03-14 21:55:44.000000 unknown-cli-0.9.2/unknown_cli.egg-info/top_level.txt
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-03-14 21:55:44.251928 unknown-cli-0.9.2/unknowncli/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        5 2024-03-14 21:55:43.000000 unknown-cli-0.9.2/unknowncli/VERSION
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      407 2024-03-11 22:54:16.000000 unknown-cli-0.9.2/unknowncli/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1815 2024-03-13 17:08:34.000000 unknown-cli-0.9.2/unknowncli/__main__.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-03-14 21:55:44.309763 unknown-cli-0.9.2/unknowncli/commands/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2023-09-08 21:53:36.000000 unknown-cli-0.9.2/unknowncli/commands/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    34140 2024-03-14 21:52:34.000000 unknown-cli-0.9.2/unknowncli/commands/preflight.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19538 2024-03-13 17:08:34.000000 unknown-cli-0.9.2/unknowncli/commands/project.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    17827 2023-12-07 23:07:53.000000 unknown-cli-0.9.2/unknowncli/commands/task.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2436 2023-09-08 21:53:36.000000 unknown-cli-0.9.2/unknowncli/commands/unreal.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-03-14 21:55:44.321762 unknown-cli-0.9.2/unknowncli/data/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     3560 2023-09-08 21:53:36.000000 unknown-cli-0.9.2/unknowncli/data/.p4ignore.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      840 2023-12-07 23:07:53.000000 unknown-cli-0.9.2/unknowncli/set_registry_keys.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1005 2023-12-07 23:07:53.000000 unknown-cli-0.9.2/unknowncli/set_url_handler.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    11456 2024-03-13 17:08:34.000000 unknown-cli-0.9.2/unknowncli/utils.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.491376 unknown-cli-0.9.3/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-05 17:28:53.489375 unknown-cli-0.9.3/PKG-INFO
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       30 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/README.md
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       38 2024-04-05 17:28:53.491376 unknown-cli-0.9.3/setup.cfg
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2695 2024-03-13 22:40:13.000000 unknown-cli-0.9.3/setup.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.353945 unknown-cli-0.9.3/unknown_cli.egg-info/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      561 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        1 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       83 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      130 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/requires.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       11 2024-04-05 17:28:53.000000 unknown-cli-0.9.3/unknown_cli.egg-info/top_level.txt
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.408944 unknown-cli-0.9.3/unknowncli/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        5 2024-04-04 23:22:42.000000 unknown-cli-0.9.3/unknowncli/VERSION
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      407 2024-03-11 22:54:16.000000 unknown-cli-0.9.3/unknowncli/__init__.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1815 2024-04-04 23:21:31.000000 unknown-cli-0.9.3/unknowncli/__main__.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.466654 unknown-cli-0.9.3/unknowncli/commands/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/commands/__init__.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    34140 2024-03-22 11:18:20.000000 unknown-cli-0.9.3/unknowncli/commands/preflight.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19657 2024-04-04 23:22:04.000000 unknown-cli-0.9.3/unknowncli/commands/project.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    18247 2024-04-04 23:22:04.000000 unknown-cli-0.9.3/unknowncli/commands/task.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2436 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/commands/unreal.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-05 17:28:53.478611 unknown-cli-0.9.3/unknowncli/data/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     3560 2023-09-08 21:53:36.000000 unknown-cli-0.9.3/unknowncli/data/.p4ignore.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      840 2023-12-07 23:07:53.000000 unknown-cli-0.9.3/unknowncli/set_registry_keys.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1005 2023-12-07 23:07:53.000000 unknown-cli-0.9.3/unknowncli/set_url_handler.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    11456 2024-04-04 23:21:31.000000 unknown-cli-0.9.3/unknowncli/utils.py
```

### Comparing `unknown-cli-0.9.2/setup.py` & `unknown-cli-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknown_cli.egg-info/SOURCES.txt` & `unknown-cli-0.9.3/unknown_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/__main__.py` & `unknown-cli-0.9.3/unknowncli/__main__.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/commands/preflight.py` & `unknown-cli-0.9.3/unknowncli/commands/preflight.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/commands/project.py` & `unknown-cli-0.9.3/unknowncli/commands/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
 STREAMS = {
     "sn2-main": "//project/sn2-main-ue"
 }
 SUB_STREAMS = {
     "//project/sn2-main": {
-        "Project    ": "//project/sn2-main-ue",
-        "Project+Raw": "//project/sn2-main-ue-raw",
-        "Everything ": "//project/sn2-main",
-        "Staging ": "//project/sn2-staging",
+        "Project"               : "//project/sn2-main-ue",
+        "Project+RawRecommended": "//project/sn2-main-ue-raw-content",
+        "Project+RawAll"        : "//project/sn2-main-ue-raw",
+        "Everything"            : "//project/sn2-main",
+        "Staging"               : "//project/sn2-staging",
     }
 }
 
 is_windows = os.name == "nt"
 DEFAULT_FOLDER = "C:\\Work" if is_windows else "~/Work"
 MIN_FREE_GB = 200
```

### Comparing `unknown-cli-0.9.2/unknowncli/commands/task.py` & `unknown-cli-0.9.3/unknowncli/commands/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import logging
 import socket
 import sys
 from ..utils import abort
+from .project import SUB_STREAMS
 from P4 import P4, P4Exception
 from typing import Optional
 from subprocess import check_call
 
 log = logging.getLogger(__name__)
 
 from typer import echo, secho, Option, Typer, confirm, prompt
@@ -14,15 +15,16 @@
 
 app = Typer()
 
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
 path = f"{SUBST_DRIVE}\\sn2-main\\"
 BASE_STREAM = "//Project/SN2-Main"
-UE_STREAM = "//project/sn2-main-ue"
+STREAM_LIST_LOWER = [s.lower() for s in list(list(SUB_STREAMS.values())[0].values())]
+STREAM_LIST_STRING = "\n\t" + "\n\t".join(STREAM_LIST_LOWER)
 
 p4 = None
 
 
 def connect_p4():
     p4_conn = P4()
     try:
@@ -49,17 +51,19 @@
         )
 
     if "Stream" not in ret:
         abort("Invalid workspace. You must be working in Streams to use this tool")
     stream_name = ret["Stream"]
     parent = ret["Parent"]
     secho(f"You are currently working in stream: {stream_name}", fg="blue")
-    if parent.lower() != UE_STREAM and stream_name.lower() != UE_STREAM:
+    if parent.lower() not in STREAM_LIST_LOWER and stream_name.lower() not in STREAM_LIST_LOWER:
         abort(
-            f"To use this tool you must be working in the {UE_STREAM} stream but your workspace is set on {stream_name}. Please change your workspace with 'p4 set'"
+            f"To use this tool you must be working in a valid stream but your workspace is set to {stream_name}." +
+            "\nPlease change to a relevant workspace with 'p4 set p4client=<your_valid_workspace>'" +
+            "\nOr set up a workspace with 'unk project setup'."
         )
 
 
 def get_task_streams(owner):
     lst = p4.run_streams("-F", f"Owner={owner} Type=task baseParent={BASE_STREAM}")
     return lst
 
@@ -104,69 +108,55 @@
     s = confirm("Sync latest?")
 
     if not s:
         return
 
     secho(f"Syncing latest...")
     try:
-        ret = p4.run_sync("-q", f"{path}UE/Subnautica2/...")
+        ret = p4.run_client("-o")[0]
+        root_path = ret["Root"]
+        p4.run_sync("-q", f"{root_path}/...")
     except P4Exception as e:
         print(e)
 
 
 @app.command()
 def create(label: str = Option(None, prompt="Task branch label")):
     """
     Create a new task branch
     """
-    
+
     if not label:
         abort("Aborted.")
-    clients = get_clients()
-    current_stream = get_current_stream()["Stream"].lower()
-    if current_stream != UE_STREAM:
-        abort(f"You are in the {current_stream} stream. Please switch to the {UE_STREAM} main stream before creating a new task stream")
-
-    ue_stream_client = None
-    for k, c in clients.items():
-        if k == UE_STREAM:
-            ue_stream_client = c
-    if not ue_stream_client:
-        abort(f"You have no workspace mapped to the {UE_STREAM} stream. Please set one up.")
+    current_stream = get_current_stream()["Stream"]
+    if current_stream.lower() not in STREAM_LIST_LOWER:
+        abort(f"You are working in stream {current_stream}. Please first run 'unk task switch' to a parent stream.\nValid parent streams:{STREAM_LIST_STRING}")
 
     ret = p4.run_opened()
     if len(ret):
         abort("You have opened files. Please revert or submit before creating new task stream.")
 
-    # print(ue_stream_client)
-    # task_client_name = ue_stream_client["client"] + "_task"
-    # task_client = None
-    # for k, c in clients.items():
-    #    if c["client"] == task_client_name:
-    #        echo(f"Reusing existin workspace {k}")
-    #        task_client = c
-    #        break
-    # sync latest from parent
-    echo(f"Syncing parent branch {path}...")
+    client_root = get_current_client()["Root"]
+    echo(f"Syncing parent branch {client_root}\...")
     try:
-        ret = p4.run_sync("-q", f"{path}...")
+        ret = p4.run_sync("-q", f"{client_root}\...")
     except P4Exception as e:
         secho(str(e), fg="yellow")
         abort("Please fix the issues above before continuing")
 
     d = datetime.datetime.utcnow().isoformat().split("T")[0]
     label = label.replace(" ", "_").lower()
     stream_name = f"{p4.user}-{d}-{label}"
     full_stream_name = f"//Project/{stream_name}"
-    secho(f"Creating task stream {stream_name} from {UE_STREAM}...")
+    secho(f"Creating task stream {stream_name} from {current_stream} ...")
     args = f"""
 Stream: {full_stream_name}
 Owner:  {p4.user}
 Name:   {stream_name}
-Parent: {UE_STREAM}
+Parent: {current_stream}
 Type:   task
 Description:
     Created by {p4.user}.
 Options:        allsubmit unlocked toparent fromparent mergedown
 ParentView:     inherit
 Paths:
     share ...
@@ -177,35 +167,35 @@
 
     try:
         with Progress(
             SpinnerColumn(),
             TextColumn("Populating {task.description}"),
             transient=True,
             ) as progress:
-            progress.add_task(description=f"{full_stream_name}...", total=None)
+            progress.add_task(description=f"{full_stream_name} ...", total=None)
             ret = p4.run_populate("-o", "-S", full_stream_name, "-r", "-d", "Initial branch")
-        
+
     except P4Exception as e:
         if e.errors:
             secho(e.errors[0], fg="yellow")
 
-    secho(f"Switching current workspace {p4.client} to {full_stream_name}...")
+    secho(f"Switching current workspace {p4.client} to {full_stream_name} ...")
     p4.run_client("-s", "-S", full_stream_name)
     ret = p4.run_client("-o")[0]
     root_path = ret["Root"]
 
     ret = p4.run_stream("-o")[0]
     stream_name = ret["Stream"]
     parent = ret["Parent"]
 
     if ret["Type"] != "task":
         abort(f"Something went wrong. Current stream {stream_name} is not a task stream")
 
     # update the server without syncing
-    ret = p4.run_sync("-q", "-k", f"{path}...")
+    ret = p4.run_sync("-q", "-k", f"{root_path}\...")
 
     secho(f"You are now working in task stream {stream_name} from parent {parent}", bold=True, fg="green")
 
 
 @app.command()
 def switch():
     """
@@ -266,15 +256,15 @@
 @app.command()
 def mergedown(nosubmit: Optional[bool] = Option(False, help="Do not submit the changelist after resolving")):
     """
     Merge from parent into your current task branch
     """
     ret = p4.run_stream("-o")[0]
     stream_name = ret["Stream"]
-    parent = ret["Parent"]
+    parent_stream = ret["Parent"]
     if ret["Type"] != "task":
         abort(f"Current stream {stream_name} is not a task stream")
 
     ret = p4.run_client("-o")[0]
     root_path = ret["Root"]
     client = ret["Client"]
 
@@ -287,26 +277,26 @@
 
     try:
         with Progress(
             SpinnerColumn(),
             TextColumn("{task.description}"),
             transient=True,
             ) as progress:
-            progress.add_task(description=f"Merging files from {UE_STREAM} to {stream_name}...", total=None)
+            progress.add_task(description=f"Merging files from {parent_stream} to {stream_name}/...", total=None)
             try:
                 cmd = ["-Af", "-S", stream_name, "-r", f"{stream_name}/..."]
                 merge_response = p4.run_merge(*cmd)
             except P4Exception as e:
                 echo("\n")
                 if e.errors:
                     secho(e.errors[0], fg="red")
                 if e.warnings:
                     secho(e.warnings[0], fg="yellow")
                 if "already integrated" in str(e):
-                    secho(f"Your task stream is already up to date with {UE_STREAM}", fg="green")
+                    secho(f"Your task stream is already up to date with {parent_stream}", fg="green")
                 return
 
     except P4Exception as e:
         if e.errors:
             secho(e.errors[0], fg="yellow")
 
     num_files = len(merge_response)
@@ -338,49 +328,49 @@
     if not ret:
         abort("Your task stream is up to date.")
 
     unresolved = []
     for r in ret:
         if "unresolved" in r:
             unresolved.append(r)
-            secho(f"  {r['clientFile']}... conflict", fg="yellow")
+            secho(f"  {r['clientFile']} ... conflict", fg="yellow")
         else:
-            secho(f"  {r['clientFile']}... ok", fg="green")
+            secho(f"  {r['clientFile']} ... ok", fg="green")
 
     if unresolved:
         secho(
-            f"\nThere are conflicting files where you have changed files which have also been changed in {UE_STREAM}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v."
+            f"\nThere are conflicting files where you have changed files which have also been changed in {parent_stream}.\nYou can force overwrite these files in your task stream or resolve yourself via p4v."
         )
         overwrite_all = False
         overwrite_none = False
         num_skipped = 0
         for i, r in enumerate(unresolved):
             y = None
             if not overwrite_all and not overwrite_none:
                 y = prompt(f"[{i+1}/{len(unresolved)}] Overwrite {r['clientFile']} [Yes/No/None/All] ").upper()
             if y not in ("YES", "Y", "NO", "N", "NONE", "ALL"):
                 abort(
-                    f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}"
+                    f"Please resolve remaining files in p4v. You can use this description: Automatically merge {parent_stream} to {stream_name}"
                 )
             if y in ("ALL"):
                 overwrite_none = False
                 overwrite_all = True
             elif y in ("NONE"):
                 overwrite_none = True
                 overwrite_all = False
 
             if y in ("Y", "YES") or overwrite_all:
                 ret = p4.run_resolve("-f", "-at", f"{r['clientFile']}")
             if y in ("N", "NO") or overwrite_none:
-                secho(f"Skipping {r['clientFile']}...")
+                secho(f"Skipping {r['clientFile']} ...")
                 num_skipped += 1
 
         if num_skipped:
             abort(
-                f"Please resolve remaining files in p4v. You can use this description: Automatically merge {UE_STREAM} to {stream_name}"
+                f"Please resolve remaining files in p4v. You can use this description: Automatically merge {parent_stream} to {stream_name}"
             )
 
         secho("All Unresolved files have been overwritten by parent stream")
 
     try:
         ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
     except P4Exception as e:
@@ -397,40 +387,40 @@
     if not nosubmit:
         txt = f"""
 Change:	new
 Client:	{client}
 User:	{p4.user}
 
 Description:
-    Automatically merge {UE_STREAM} to {stream_name}. {mr}
+    Automatically merge {parent_stream} to {stream_name}. {mr}
 Files:
 {filelist}"""
         p4.input = txt
         p4.run_submit("-i")
 
         try:
             ret = p4.run_resolve("-f", "-am", "-as", f"{root_path}/...")
         except P4Exception as e:
             if "no file(s) to resolve" not in str(e):
                 raise
         try:
             ret = p4.run_fstat("-Olhp", "-Rco", "-e", "default", f"{root_path}/...")
         except P4Exception as e:
             if "not opened on this client." in str(e) or "no such file(s)." in str(e):
-                secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
+                secho(f"Your task stream is now up to date with {parent_stream}", fg="green")
                 return
             else:
                 echo(str(e))
         if not ret:
-            secho(f"Your task stream is now up to date with {UE_STREAM}", fg="green")
+            secho(f"Your task stream is now up to date with {parent_stream}", fg="green")
         else:
             abort("Something is amiss. Your task stream is not up to date after the merge. Take a look at p4v")
     else:
         echo(
-            f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {UE_STREAM} to {stream_name}. {mr}"
+            f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {parent_stream} to {stream_name}. {mr}"
         )
 
 
 @app.command()
 def copyup():
     """
     Finish the task and copy into the parent stream
@@ -442,25 +432,28 @@
     ## p4 copy -Af -S //Project/jonb-2023-03-03-plugin_functional_tests //Project/SN2-Main/...
     ret = get_current_stream()
     stream_name = ret["Stream"]
     parent = ret["Parent"]
     if ret["Type"] != "task":
         abort(f"Current stream {stream_name} is not a task stream")
 
-    echo(f"Switching to parent stream {parent}...")
+    secho(f"Switching to parent stream {parent} ...", fg="blue")
     p4.run_client("-s", "-S", parent)
 
     p4.run_sync("-q")
-    echo(f"Performing copy from {stream_name} to {ret['baseParent']}...")
+    echo(f"Performing copy from {stream_name} to {ret['baseParent']}/...")
     try:
         copy_ret = p4.run_copy("-Af", "-S", stream_name, ret["baseParent"] + "/...")
     except P4Exception as e:
         if "up-to-date" in str(e):
             secho(f"Nothing to do. Parent {parent} is identical to task stream {stream_name}", fg="green")
             return
+        elif "No such file(s)" in str(e):
+            secho(f"Nothing to do. No changes were made yet in task stream {stream_name}", fg="green")
+            return
         else:
             raise
     else:
         echo("Adding files...")
         for r in copy_ret:
             echo(f"  {r['fromFile']} -> {r['depotFile']}")
 
@@ -471,21 +464,20 @@
 def delete(current: Optional[bool] = Option(False, help="Delete the current task stream")):
     """
     Permanently delete a named task stream or your current one"""
 
     ret = p4.run_stream("-o")[0]
     current_stream_name = ret["Stream"]
     parent = ret["Parent"]
+    root_path = get_current_client()["Root"]
 
     if current:
         if ret["Type"] != "task":
             abort(f"Current stream {current_stream_name} is not a task stream")
-
-        if confirm("Are you sure you want to delete the current task stream?"):
-            streams_to_delete = [current_stream_name]
+        streams_to_delete = [current_stream_name]
     else:
         client = p4.run_client("-o")[0]
         client_owner = client["Owner"]
         task_streams = get_task_streams(client_owner)
 
         if not task_streams:
             abort("You have no task streams.")
@@ -501,28 +493,36 @@
             try:
                 n = int(n)
             except:
                 abort("Aborted.")
             if n <= 0 or n > len(task_streams):
                 abort("Aborted.")
             stream_name = task_streams[n - 1]["Stream"]
-            if confirm(f"Are you sure you want to delete the task stream {stream_name}?"):
-                streams_to_delete = [stream_name]
+            streams_to_delete = [stream_name]
 
     if streams_to_delete:
+        streams_to_delete_string = "\n\t" + "\n\t".join(
+            [f"(**YOUR CURRENT TASK STREAM**) {x}" if current_stream_name == x else x for x in streams_to_delete]
+        )
+        if not confirm(
+            f"==============\nTask stream(s) to delete:{streams_to_delete_string}" +
+            "\nAre you sure you want to delete these task stream(s)?"
+        ):
+            abort("Aborted.")
+
         if current_stream_name in streams_to_delete:
             if not parent:
-                abort("Please switch to sn2-main stream before continuing")
-            secho(f"Switching to {parent}...")
+                abort(f"Please run 'unk task switch' to a parent stream before continuing:{STREAM_LIST_STRING}")
+            secho(f"Switching to {parent} before deleting the task stream ...")
             p4.run_client("-s", "-S", parent)
-            ret = p4.run_sync("-q", f"{path}...")
+            ret = p4.run_sync("-q", f"{root_path}\...")
 
         for stream_name in streams_to_delete:
             cmd = [sys.executable, "s:/sn2-main/BuildScripts/trigger_task_stream_deletion.py", stream_name]
-            secho(f"Deleting task stream {stream_name}...")
+            secho(f"Deleting task stream {stream_name} ...")
 
             check_call(cmd)
         secho("Request to delete selected streams has been sent. It might take a few minutes to finish", fg="green")
     else:
         abort("Aborted")
-    ret = p4.run_sync("-q", "-k", f"{path}...")
+    ret = p4.run_sync("-q", "-k", f"{root_path}\...")
     # sync()
```

### Comparing `unknown-cli-0.9.2/unknowncli/commands/unreal.py` & `unknown-cli-0.9.3/unknowncli/commands/unreal.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/data/.p4ignore.txt` & `unknown-cli-0.9.3/unknowncli/data/.p4ignore.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/set_registry_keys.py` & `unknown-cli-0.9.3/unknowncli/set_registry_keys.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/set_url_handler.py` & `unknown-cli-0.9.3/unknowncli/set_url_handler.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.2/unknowncli/utils.py` & `unknown-cli-0.9.3/unknowncli/utils.py`

 * *Files identical despite different names*

