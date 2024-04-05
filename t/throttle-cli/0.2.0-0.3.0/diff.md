# Comparing `tmp/throttle_cli-0.2.0.tar.gz` & `tmp/throttle_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "throttle_cli-0.2.0.tar", max compression
+gzip compressed data, was "throttle_cli-0.3.0.tar", max compression
```

## Comparing `throttle_cli-0.2.0.tar` & `throttle_cli-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    13827 2024-03-04 13:14:43.080562 throttle_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     9213 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/README.md
--rw-r--r--   0        0        0      756 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-17 19:54:08.955808 throttle_cli-0.2.0/throttle_cli/__init__.py
--rw-r--r--   0        0        0     1197 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/arglib.py
--rw-r--r--   0        0        0     1777 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/cli.py
--rw-r--r--   0        0        0     1287 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/client.py
--rw-r--r--   0        0        0     9009 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/commandworker.py
--rw-r--r--   0        0        0     1439 2024-02-29 20:24:41.296737 throttle_cli-0.2.0/throttle_cli/loglib.py
--rw-r--r--   0        0        0     1490 2024-03-12 22:07:09.496788 throttle_cli-0.2.0/throttle_cli/server.py
--rw-r--r--   0        0        0     1155 2024-04-04 18:43:15.772207 throttle_cli-0.2.0/throttle_cli/structures.py
--rw-r--r--   0        0        0     9940 1970-01-01 00:00:00.000000 throttle_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-03-04 13:14:43.080562 throttle_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11559 2024-04-05 20:13:36.051593 throttle_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      836 2024-04-05 20:13:36.063593 throttle_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      789 2024-04-05 07:42:05.494387 throttle_cli-0.3.0/throttle_cli/__init__.py
+-rw-r--r--   0        0        0     1197 2024-04-04 18:43:15.772207 throttle_cli-0.3.0/throttle_cli/arglib.py
+-rw-r--r--   0        0        0     2204 2024-04-05 20:13:36.055594 throttle_cli-0.3.0/throttle_cli/cli_client.py
+-rw-r--r--   0        0        0      820 2024-04-05 20:13:36.055594 throttle_cli-0.3.0/throttle_cli/cli_server.py
+-rw-r--r--   0        0        0     2200 2024-04-05 19:41:21.377872 throttle_cli-0.3.0/throttle_cli/client.py
+-rw-r--r--   0        0        0    10257 2024-04-05 19:35:47.392917 throttle_cli-0.3.0/throttle_cli/commandworker.py
+-rw-r--r--   0        0        0     1633 2024-04-05 19:53:28.358412 throttle_cli-0.3.0/throttle_cli/infoparser.py
+-rw-r--r--   0        0        0     1439 2024-02-29 20:24:41.296737 throttle_cli-0.3.0/throttle_cli/loglib.py
+-rw-r--r--   0        0        0     1730 2024-04-05 09:46:17.896815 throttle_cli-0.3.0/throttle_cli/server.py
+-rw-r--r--   0        0        0     1322 2024-04-05 19:30:04.275903 throttle_cli-0.3.0/throttle_cli/structures.py
+-rw-r--r--   0        0        0    12331 1970-01-01 00:00:00.000000 throttle_cli-0.3.0/PKG-INFO
```

### Comparing `throttle_cli-0.2.0/LICENSE` & `throttle_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.2.0/README.md` & `throttle_cli-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Throttle
 
 A small client-server utility, that throttles commands sent to it from multiple
-async sources.
+async sources. Also doubles as an error-notification handler for these jobs.
 
 Features:
 
 - if receiving multiple instances of an already running command, only one other instance will be executed, after the current one finishes, by running each command in it's own process
 - allows chaining commands, each command in the chain is still correctly throttled
 - repeats failed commands in configurable intervals
 - configurable notification callback for failed commands
 - configuration allows handling spammed notifications from flaky commands (e.g because of flaky networks)
 - regex based on the fly rewrite of commands
+- statistics on the amount of throttling
 
 ## Social
 
 Development and support happens on
 [sourcehut](https://sr.ht/~ferdinandyb/throttle/), but there's a mirror on
 [github](https://github.com/ferdinandyb/throttle) for convenience and
 discoverability. You can also star there to show your interest/appreciation.
@@ -58,15 +59,15 @@
 ```
 pipx install git+https://git.sr.ht/~ferdinandyb/throttle
 ```
 
 Start server with
 
 ```
-throttle --server
+throttle-server
 ```
 
 And send a command to the server (via unix socket):
 
 ```
 throttle mbsync inbox
 ```
@@ -74,32 +75,52 @@
 `throttle` should now run `mbsync inbox` for you. If you spam the above command
 a couple of hundred times before the first one finishes, `throttle` will queue
 up a single other instance of `mbsync inbox` after the first one finished.
 
 
 ## Usage
 
+### Server
+
 ```
-usage: throttle [-h] [-s | -j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+usage: throttle-server [-h] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+
+start the throttle server
 
 options:
   -h, --help            show this help message and exit
-  -s, --server          Start server.
+  --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
+                        Set loglevel.
+```
+
+### Client
+
+```
+usage: throttle [-h] [--version] [-j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--statistics] [--status] [--format {text,csv,latex,html,json,markdown,plain}]
+
+send jobs to the throttle server
+
+options:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
   -j JOB, --job JOB     Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.
   -J SILENT_JOB, --silent-job SILENT_JOB
                         Same as --job, but no notifications will be sent on failure.
   -k, --kill            Kill a previously started job.
   -o ORIGIN, --origin ORIGIN
                         Set the origin of the message, which might be useful in tracking logs.
-  --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
-                        Set loglevel.
-
+  --statistics          Print statistics for handled commands.
+  --status              Print status information for currently running workers.
+  --format {text,csv,latex,html,json,markdown,plain}
+                        Format for printing results.
 ```
 
-First start a server with `throttle --server`. It will log to
+### Step-by-step and examples
+
+First start a server with `throttle-server`. It will log to
 `$XDG_STATE/throttle/throttle.log`, which should default to
 `~/.local/state/throttle/throttle.log`.
 
 To start a job run `throttle my command` which will run `my command`. You can
 make it explicit by running `throttle --job "my command"`. Multiple `--job`
 flags will execute the command successively. Any dangling parameters will be
 scooped up for a last command so
@@ -151,14 +172,15 @@
 Configuration happens in `$XDG_CONFIG/throttle/config.toml`.
 
 Example config:
 
 ```
 task_timeout = 30
 retry_sequence = [5,15,30,60,120,300,900]
+retry_sequence_silent = [5,15,30,60]
 notification_cmd = 'notify-send --urgency={urgency} --app-name="throttle" "{job} ({origin})" "({errcode}): {msg}"'
 
 notify_on_counter = 2
 job_timeout = 600
 
 [[filters]]
 pattern = '^sleep \d$'
@@ -170,27 +192,57 @@
 
 [[filters]]
 pattern = '^mbsync (\w+)-(?!(inbox|archive|sent|drafts)$).+'
 substitute = 'mbsync \1-folders'
 ```
 
 - `task_timeout`: how long to wait before cleaning up a process with no more incoming commands (probably no need to change this)
-- `retry_sequence`: list of seconds to successively wait if a command fails (e.g. no internet connection), the last element is retried in perpetuity
+- `retry_sequence`: list of seconds to successively wait if a (non-silent) job fails (e.g. bad credentials), the last element is retried in perpetuity
+- `retry_sequence_silent`: list of seconds to successively wait if a silent job fails (e.g. no internet connection), the last element is retried in perpetuity
 - `notification_cmd`: in case of a command failure, this command is called. See below for template keys
 - `notify_on_counter`: how many failures before a notification should be sent
 - `job_timeout`: how many seconds to let a job run, before timeouting it
 - filters: each `filters` section defines a specific transformation, the first matching one is applied. `pattern` is checked against the command and if it matches, replaced by `substitute` using regex substitution (python `re.sub({pattern},{substitute},{input})` is used). In case of multiple commands in one call, it is done per command separately.
 
 Key that can be used in `notification_cmd`:
 
 - job: a job (single `--job`)
 - urgency: this is always "urgent" for now
 - errcode: errorcode if it exists (set to -1000 if error code was not returned)
 - msg: usually stderr of subprocess
 
+## Statistics
+
+Running `throttle --statistics --format=markdown` will output something like
+this. If connected to a tty, the job names will be truncated to make each row
+fit on a line. When redirected, there's not truncating.
+
+The column are the following (statistics are gathered from starting the server
+and are not persisted across sessions):
+
+- `run`: number of times the job has been actually run
+- `total`: number of times the job has been submitted for running
+- `throttle`: ratio of requests that were requested, but did not run
+- `avg/min`: average number of `run` per minute
+
+```
+| job                               | run | total | throttle | avg/min |
+| :---------------------------------| :-: | :---: | :------: | :-----: |
+| mbsync priestoferis-folders       |  18 |  216  |   0.92   |   0.03  |
+| mbsync priestoferis-inbox         |  10 |   37  |   0.73   |   0.02  |
+| mbsync priestoferis-sent          |  10 |   36  |   0.72   |   0.02  |
+| mbsync priestoferis-drafts        |  10 |   36  |   0.72   |   0.02  |
+| mbsync priestoferis-archive       |  10 |   36  |   0.72   |   0.02  |
+| mbsync elte-folders               |  72 |  144  |   0.50   |   0.13  |
+| notmuch new                       | 832 |  1118 |   0.26   |   1.46  |
+| mbsync elte-sent                  |  31 |   37  |   0.16   |   0.05  |
+| mbsync elte-inbox                 |  44 |   49  |   0.10   |   0.08  |
+| testinternetconnection            | 992 |  1080 |   0.08   |   1.74  |
+
+```
 ## Troubleshooting
 
 ### pinentry on frequent gpg access
 
 If the command you are running requires gpg, and after multiple commands you are being asked for a pinentry, although normally your gpg key is unlocked, you need to add something like this to `gpg-agent.conf`:
 
 ```
```

### Comparing `throttle_cli-0.2.0/pyproject.toml` & `throttle_cli-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "throttle-cli"
-version = "0.2.0"
+version = "0.3.0"
 description = "Throttle commands triggered from multiple async sources."
 authors = ["Bence Ferdinandy <bence@ferdinandy.com>"]
 readme = "README.md"
 license = "EUPL-1.2"
 homepage = "https://sr.ht/~ferdinandyb/throttle/"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 jsonrpclib-pelix = "^0.4.3.2"
 toml = "^0.10.2"
 pyxdg = "^0.28"
+prettytable = "^3.10.0"
 
 [tool.poetry.scripts]
-throttle = "throttle_cli.cli:main"
+throttle = "throttle_cli.cli_client:main"
+throttle-server = "throttle_cli.cli_server:main"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 ruff = "^0.2.2"
 mypy = "^1.8.0"
 
 [build-system]
```

### Comparing `throttle_cli-0.2.0/throttle_cli/arglib.py` & `throttle_cli-0.3.0/throttle_cli/arglib.py`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.2.0/throttle_cli/cli.py` & `throttle_cli-0.3.0/throttle_cli/cli_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-import logging
 from pathlib import Path
 
 from xdg import BaseDirectory
 
-from .client import send_message
-from .server import start_server
+from . import __version__
 from .arglib import storeJob, storeSilentJob
+from .client import get_info, send_message
+from .structures import ActionType
 
 
 def main():
     import argparse
 
-    parser = argparse.ArgumentParser()
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument("-s", "--server", action="store_true", help="Start server.")
-    group.add_argument(
+    parser = argparse.ArgumentParser(
+        prog="throttle", description="send jobs to the throttle server"
+    )
+    parser.add_argument(
+        "--version", action="version", version=f"throttle {__version__}"
+    )
+    parser.add_argument(
         "-j",
         "--job",
         action=storeJob,
         help="Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.",
     )
     parser.add_argument(
         "-J",
@@ -32,25 +35,36 @@
     parser.add_argument(
         "-o",
         "--origin",
         type=str,
         help="Set the origin of the message, which might be useful in tracking logs.",
     )
     parser.add_argument(
-        "--LOGLEVEL",
-        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
-        help="Set loglevel.",
+        "--statistics",
+        action="store_true",
+        help="Print statistics for handled commands.",
+    )
+    parser.add_argument(
+        "--status",
+        action="store_true",
+        help="Print status information for currently running workers.",
+    )
+    parser.add_argument(
+        "--format",
+        choices=["text", "csv", "latex", "html", "json", "markdown", "plain"],
+        default="text",
+        help="Format for printing results.",
     )
     args, unknownargs = parser.parse_known_args()
     socketpath = Path(BaseDirectory.get_runtime_dir()) / "throttle.sock"
-    loglevel = logging.INFO
-    if args.LOGLEVEL:
-        loglevel = getattr(logging, args.LOGLEVEL)
-    if args.server:
-        start_server(socketpath, loglevel)
+    if args.statistics:
+        get_info(socketpath, ActionType.STATS, args.format)
+        return
+    if args.status:
+        get_info(socketpath, ActionType.STATUS, args.format)
         return
     if hasattr(args, "notifications"):
         notifications = args.notifications
     else:
         notifications = []
     send_message(
         socketpath, args.kill, args.job, notifications, args.origin, unknownargs
```

### Comparing `throttle_cli-0.2.0/throttle_cli/client.py` & `throttle_cli-0.3.0/throttle_cli/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from pathlib import Path
 from typing import List
 
 from jsonrpclib import ServerProxy
 
+from .infoparser import parse_stat, parse_status
 from .structures import ActionType
 
 
 def send_message(
     socketpath: Path,
     kill: bool,
     jobs: List[str],
     notifications: List[int],
     origin: str,
     unknownargs: List[str],
 ) -> None:
     if not socketpath.exists():
-        print("socket doesn't exist, is throttle running?")
+        print("Socket doesn't exist, is the throttle server running?")
+        print("You can start the server by running throttle-server")
         import sys
 
         sys.exit(1)
     action = ActionType.KILL if kill else ActionType.RUN
     mergedjobs: List[str] = []
     if notifications is None:
         notifications = []
@@ -41,11 +43,36 @@
             }
         )
         client("close")()
     except ConnectionRefusedError:
         import sys
 
         print(
-            "Connection refused: did you start the server with `throttle --server`?",
+            "Connection refused: did you start the server with `throttle-server`?",
+            file=sys.stderr,
+        )
+        sys.exit(1)
+
+
+def get_info(socketpath, action, format):
+    if not socketpath.exists():
+        print("Socket doesn't exist, is the throttle server running?")
+        print("You can start the server by running throttle-server")
+        import sys
+
+        sys.exit(1)
+    try:
+        client = ServerProxy(f"unix+http://{socketpath}")
+        retval = client.info({"action": action})
+        if action == ActionType.STATS:
+            print(parse_stat(retval, format))
+        elif action == ActionType.STATUS:
+            print(parse_status(retval, format))
+        client("close")()
+    except ConnectionRefusedError:
+        import sys
+
+        print(
+            "Connection refused: did you start the server with `throttle-server`?",
             file=sys.stderr,
         )
         sys.exit(1)
```

### Comparing `throttle_cli-0.2.0/throttle_cli/commandworker.py` & `throttle_cli-0.3.0/throttle_cli/commandworker.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,25 +22,28 @@
     p: Process
     q: Queue
     e: SyncEvent
     t: float
 
 
 class CommandWorker:
-    def __init__(self, queue: Queue, logqueue: Queue):
+    def __init__(self, queue: Queue, logqueue: Queue, comqueue: Queue):
         self.q = queue
         self.logqueue = logqueue
+        self.comqueue = comqueue
         self.logger = logging.getLogger("msg_worker")
         self.data: Dict[str, workeritem] = {}
         self.timeout = 30
         self.filters: List[Dict[str, str]] = []
         self.notification_cmd = None
         self.notify_on_counter = 0
         self.job_timeout = 60 * 60
         self.retry_sequence = [5, 15, 30, 60, 120, 300, 900]
+        self.retry_sequence_silent = [5, 15, 30, 60]
+        self.statistics = {"start": time.time(), "jobs": {}}
 
         self.loadConfig()
 
     def loadConfig(self):
         configdir = BaseDirectory.load_first_config("throttle")
         if configdir is None:
             return
@@ -57,14 +60,16 @@
         if "filters" in config:
             for f in config["filters"]:
                 if "pattern" not in f or "substitute" not in f:
                     self.logger.error(f"{f} is not a valid filter config")
             self.filters = config["filters"]
         if "retry_sequence" in config:
             self.retry_sequence = config["retry_sequence"]
+        if "retry_sequence_silent" in config:
+            self.retry_sequence_silent = config["retry_sequence_silent"]
         if "notification_cmd" in config:
             self.notification_cmd = config["notification_cmd"]
         if "notify_on_counter" in config:
             self.notify_on_counter = config["notify_on_counter"]
         if "job_timeout" in config:
             self.job_timeout = config["job_timeout"]
 
@@ -81,17 +86,30 @@
                     self.handleRun(msg)
                 case ActionType.CONT:
                     self.handleRun(msg)
                 case ActionType.KILL:
                     self.handleKill(msg)
                 case ActionType.CLEAN:
                     self.handleCleanup()
+                case ActionType.STATS:
+                    self.comqueue.put(self.statistics)
+                case ActionType.STATUS:
+                    self.comqueue.put(self.get_status())
+
+    def get_status(self):
+        retval = {}
+        for key, value in self.data.items():
+            retval[key] = {"queuesize": value.q.qsize(), "uptime": value.t}
+        return retval
 
     def handleRun(self, msg) -> None:
         msg.job = self.checkregex(msg.job)
+        if msg.job not in self.statistics["jobs"]:
+            self.statistics["jobs"][msg.job] = {"total": 0, "run": 0}
+        self.statistics["jobs"][msg.job]["total"] += 1
         if msg.job not in self.data or not self.data[msg.job].p.is_alive():
             self.logger.debug(f"{msg.job}: doesn't exist or finished, creating")
             q: Queue[Msg] = Queue()
             e = Event()
             p = Process(
                 target=self.runworkerFactory(),
                 args=(q, e, self.timeout, msg.job),
@@ -100,30 +118,31 @@
             self.data[msg.job] = workeritem(p, q, e, time.time())
         qsize = self.data[msg.job].q.qsize()
         self.logger.debug(f"{msg.job}: approx queue size {qsize}")
         self.data[msg.job].t = time.time()
         if self.data[msg.job].q.empty():
             self.logger.debug(f"{msg.job}: empty, adding new")
             self.data[msg.job].q.put(msg)
+            self.statistics["jobs"][msg.job]["run"] += 1
             return
         self.logger.debug(f"{msg.job} already queued")
         if msg.cont():
             self.logger.debug(f"{msg.job}: adding CONT")
             self.data[msg.job].q.put(msg)
 
-    def handleCleanup(self):
+    def handleCleanup(self) -> None:
         self.logger.debug(f"cleanup underway, {self.data.keys()}")
         toclean = []
         for key, val in self.data.items():
             if not val.p.is_alive():
                 toclean.append(key)
 
         for key in toclean:
             del self.data[key]
-        self.logger.debug(f"cleanup finished, {self.data.keys()}")
+        self.logger.info(f"cleanup finished, {self.data.keys()}")
 
     def handleKill(self, msg) -> None:
         for job in msg.jobs:
             if job in self.data:
                 self.data[job].e.set()
         self.logger.debug(f"remaining jobs: {self.data.keys()}")
 
@@ -170,18 +189,22 @@
         """
         Factory for handling each type of job.
         """
 
         def handlejobs(msg: Msg, e, logger) -> None:
             retry_timeout_index = -1
             error_counter = 0
+            if msg.notification:
+                retry_sequence = self.retry_sequence
+            else:
+                retry_sequence = self.retry_sequence_silent
             while True:
                 if e.is_set():
                     break
-                if retry_timeout_index + 1 < len(self.retry_sequence):
+                if retry_timeout_index + 1 < len(retry_sequence):
                     retry_timeout_index += 1
                 success = True
                 logger.debug(msg)
                 logger.debug(f"running job: {msg.job} with timeout {self.job_timeout}")
                 try:
                     proc = subprocess.run(
                         shlex.split(msg.job),
@@ -214,36 +237,38 @@
                         )
                         error_counter = 0
 
                 if success:
                     break
                 if e.is_set():
                     break
-                time.sleep(self.retry_sequence[retry_timeout_index])
+                time.sleep(retry_sequence[retry_timeout_index])
 
         def worker(q, e, timeout, name) -> None:
             self.retry_sequence
-
-            logger = logging.getLogger(f"{name.replace(' ','_')}_worker")
+            logger_name = f"{name.replace(' ','_')}_worker"
+            logger = logging.getLogger(logger_name)
             counter = 0
-            logger.info("starting process")
+            cont_counter = 0
+            logger.debug(f"starting process for {logger_name}")
 
             while True:
                 if e.is_set():
                     break
                 try:
                     msg = q.get(timeout=timeout)
                     if msg.action == ActionType.RUN:
                         counter += 1
-                        logger.info(f"start run no: {counter}")
+                        logger.debug(f"start run no: {counter} (CONT: {cont_counter})")
                         handlejobs(msg, e, logger)
-                        logger.info(f"finish run no: {counter}")
+                        logger.debug(f"finish run no: {counter} (CONT: {cont_counter})")
                     else:
-                        logger.info("handling CONT")
+                        cont_counter += 1
+                        logger.debug(f"handling CONT no. {cont_counter}")
                     if msg.next():
                         self.q.put(msg)
                 except queue.Empty:
-                    logger.info("closing process")
+                    logger.debug(f"closing process for {logger_name}")
                     break
-            self.q.put(Msg(jobs=[], notifications=[], action=ActionType.CLEAN))
+            self.q.put(Msg(action=ActionType.CLEAN))
 
         return worker
```

### Comparing `throttle_cli-0.2.0/throttle_cli/loglib.py` & `throttle_cli-0.3.0/throttle_cli/loglib.py`

 * *Files identical despite different names*

### Comparing `throttle_cli-0.2.0/throttle_cli/server.py` & `throttle_cli-0.3.0/throttle_cli/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,42 +9,49 @@
 from jsonrpclib.SimpleJSONRPCServer import SimpleJSONRPCServer
 
 from . import loglib
 from .commandworker import CommandWorker
 from .structures import Msg
 
 
-def ipcworker(socketpath: Path, handleMsg: Callable) -> None:
+def ipcworker(socketpath: Path, handleMsg: Callable, handleInfo: Callable) -> None:
     socketpath.parent.mkdir(parents=True, exist_ok=True)
     if Path(socketpath).exists():
         Path(socketpath).unlink()
     logger = logging.getLogger("ipc_worker")
     srv = SimpleJSONRPCServer(str(socketpath), address_family=socket.AF_UNIX)
     srv.register_function(handleMsg, "handle")
+    srv.register_function(handleInfo, "info")
     logger.info(f"starting up server on socket: {socketpath}")
     srv.serve_forever()
 
 
 def start_server(socketpath: Path, loglevel) -> None:
     ipcqueue: Queue[Msg] = Queue()
     logqueue: Queue[Any] = Queue()
+    comqueue: Queue[Any] = Queue()
     loggerp = Process(target=loglib.consumer, args=(logqueue,))
     loggerp.start()
 
-    msgworker = CommandWorker(ipcqueue, logqueue)
+    msgworker = CommandWorker(ipcqueue, logqueue, comqueue)
     loglib.publisher_config(logqueue, loglevel)
     logger = logging.getLogger("server")
     logger.debug(os.environ)
 
     def handleMsg(msg) -> None:
         ipcqueue.put(Msg(**msg))
 
+    def handleInfo(msg):
+        print("handling")
+        ipcqueue.put(Msg(**msg))
+        return comqueue.get()
+
     p_ipc = Process(
         target=ipcworker,
-        args=(socketpath, handleMsg),
+        args=(socketpath, handleMsg, handleInfo),
     )
     p_msg = Process(target=msgworker.msgworker, args=())
     p_ipc.start()
     p_msg.start()
     while True:
         time.sleep(1)
         if not active_children():
```

### Comparing `throttle_cli-0.2.0/throttle_cli/structures.py` & `throttle_cli-0.3.0/throttle_cli/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import List
 
 
 class ActionType(Enum):
     RUN = auto()  # run job
     CONT = auto()  # don't run this job, but call next
     KILL = auto()  # kill job
     CLEAN = auto()  # clear up dangling jobs
+    STATS = auto()  # return stats to client
+    STATUS = auto()  # return current status to client
 
 
 @dataclass
 class Msg:
-    jobs: List[str]
-    notifications: List[int]
     action: ActionType
+    jobs: List[str] = field(default_factory=list)
+    notifications: List[int] = field(default_factory=list)
     index: int = 0
     origin: str = ""
 
     @property
     def job(self) -> str:
         return self.jobs[self.index]
```

### Comparing `throttle_cli-0.2.0/PKG-INFO` & `throttle_cli-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: throttle-cli
-Version: 0.2.0
+Version: 0.3.0
 Summary: Throttle commands triggered from multiple async sources.
 Home-page: https://sr.ht/~ferdinandyb/throttle/
 License: EUPL-1.2
 Author: Bence Ferdinandy
 Author-email: bence@ferdinandy.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jsonrpclib-pelix (>=0.4.3.2,<0.5.0.0)
+Requires-Dist: prettytable (>=3.10.0,<4.0.0)
 Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Throttle
 
 A small client-server utility, that throttles commands sent to it from multiple
-async sources.
+async sources. Also doubles as an error-notification handler for these jobs.
 
 Features:
 
 - if receiving multiple instances of an already running command, only one other instance will be executed, after the current one finishes, by running each command in it's own process
 - allows chaining commands, each command in the chain is still correctly throttled
 - repeats failed commands in configurable intervals
 - configurable notification callback for failed commands
 - configuration allows handling spammed notifications from flaky commands (e.g because of flaky networks)
 - regex based on the fly rewrite of commands
+- statistics on the amount of throttling
 
 ## Social
 
 Development and support happens on
 [sourcehut](https://sr.ht/~ferdinandyb/throttle/), but there's a mirror on
 [github](https://github.com/ferdinandyb/throttle) for convenience and
 discoverability. You can also star there to show your interest/appreciation.
@@ -77,15 +79,15 @@
 ```
 pipx install git+https://git.sr.ht/~ferdinandyb/throttle
 ```
 
 Start server with
 
 ```
-throttle --server
+throttle-server
 ```
 
 And send a command to the server (via unix socket):
 
 ```
 throttle mbsync inbox
 ```
@@ -93,32 +95,52 @@
 `throttle` should now run `mbsync inbox` for you. If you spam the above command
 a couple of hundred times before the first one finishes, `throttle` will queue
 up a single other instance of `mbsync inbox` after the first one finished.
 
 
 ## Usage
 
+### Server
+
 ```
-usage: throttle [-h] [-s | -j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+usage: throttle-server [-h] [--LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
+
+start the throttle server
 
 options:
   -h, --help            show this help message and exit
-  -s, --server          Start server.
+  --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
+                        Set loglevel.
+```
+
+### Client
+
+```
+usage: throttle [-h] [--version] [-j JOB] [-J SILENT_JOB] [-k] [-o ORIGIN] [--statistics] [--status] [--format {text,csv,latex,html,json,markdown,plain}]
+
+send jobs to the throttle server
+
+options:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
   -j JOB, --job JOB     Explicitly give job to execute, can be given multiple times, in that case, they will be run consecutively.
   -J SILENT_JOB, --silent-job SILENT_JOB
                         Same as --job, but no notifications will be sent on failure.
   -k, --kill            Kill a previously started job.
   -o ORIGIN, --origin ORIGIN
                         Set the origin of the message, which might be useful in tracking logs.
-  --LOGLEVEL {DEBUG,INFO,WARNING,ERROR,CRITICAL}
-                        Set loglevel.
-
+  --statistics          Print statistics for handled commands.
+  --status              Print status information for currently running workers.
+  --format {text,csv,latex,html,json,markdown,plain}
+                        Format for printing results.
 ```
 
-First start a server with `throttle --server`. It will log to
+### Step-by-step and examples
+
+First start a server with `throttle-server`. It will log to
 `$XDG_STATE/throttle/throttle.log`, which should default to
 `~/.local/state/throttle/throttle.log`.
 
 To start a job run `throttle my command` which will run `my command`. You can
 make it explicit by running `throttle --job "my command"`. Multiple `--job`
 flags will execute the command successively. Any dangling parameters will be
 scooped up for a last command so
@@ -170,14 +192,15 @@
 Configuration happens in `$XDG_CONFIG/throttle/config.toml`.
 
 Example config:
 
 ```
 task_timeout = 30
 retry_sequence = [5,15,30,60,120,300,900]
+retry_sequence_silent = [5,15,30,60]
 notification_cmd = 'notify-send --urgency={urgency} --app-name="throttle" "{job} ({origin})" "({errcode}): {msg}"'
 
 notify_on_counter = 2
 job_timeout = 600
 
 [[filters]]
 pattern = '^sleep \d$'
@@ -189,27 +212,57 @@
 
 [[filters]]
 pattern = '^mbsync (\w+)-(?!(inbox|archive|sent|drafts)$).+'
 substitute = 'mbsync \1-folders'
 ```
 
 - `task_timeout`: how long to wait before cleaning up a process with no more incoming commands (probably no need to change this)
-- `retry_sequence`: list of seconds to successively wait if a command fails (e.g. no internet connection), the last element is retried in perpetuity
+- `retry_sequence`: list of seconds to successively wait if a (non-silent) job fails (e.g. bad credentials), the last element is retried in perpetuity
+- `retry_sequence_silent`: list of seconds to successively wait if a silent job fails (e.g. no internet connection), the last element is retried in perpetuity
 - `notification_cmd`: in case of a command failure, this command is called. See below for template keys
 - `notify_on_counter`: how many failures before a notification should be sent
 - `job_timeout`: how many seconds to let a job run, before timeouting it
 - filters: each `filters` section defines a specific transformation, the first matching one is applied. `pattern` is checked against the command and if it matches, replaced by `substitute` using regex substitution (python `re.sub({pattern},{substitute},{input})` is used). In case of multiple commands in one call, it is done per command separately.
 
 Key that can be used in `notification_cmd`:
 
 - job: a job (single `--job`)
 - urgency: this is always "urgent" for now
 - errcode: errorcode if it exists (set to -1000 if error code was not returned)
 - msg: usually stderr of subprocess
 
+## Statistics
+
+Running `throttle --statistics --format=markdown` will output something like
+this. If connected to a tty, the job names will be truncated to make each row
+fit on a line. When redirected, there's not truncating.
+
+The column are the following (statistics are gathered from starting the server
+and are not persisted across sessions):
+
+- `run`: number of times the job has been actually run
+- `total`: number of times the job has been submitted for running
+- `throttle`: ratio of requests that were requested, but did not run
+- `avg/min`: average number of `run` per minute
+
+```
+| job                               | run | total | throttle | avg/min |
+| :---------------------------------| :-: | :---: | :------: | :-----: |
+| mbsync priestoferis-folders       |  18 |  216  |   0.92   |   0.03  |
+| mbsync priestoferis-inbox         |  10 |   37  |   0.73   |   0.02  |
+| mbsync priestoferis-sent          |  10 |   36  |   0.72   |   0.02  |
+| mbsync priestoferis-drafts        |  10 |   36  |   0.72   |   0.02  |
+| mbsync priestoferis-archive       |  10 |   36  |   0.72   |   0.02  |
+| mbsync elte-folders               |  72 |  144  |   0.50   |   0.13  |
+| notmuch new                       | 832 |  1118 |   0.26   |   1.46  |
+| mbsync elte-sent                  |  31 |   37  |   0.16   |   0.05  |
+| mbsync elte-inbox                 |  44 |   49  |   0.10   |   0.08  |
+| testinternetconnection            | 992 |  1080 |   0.08   |   1.74  |
+
+```
 ## Troubleshooting
 
 ### pinentry on frequent gpg access
 
 If the command you are running requires gpg, and after multiple commands you are being asked for a pinentry, although normally your gpg key is unlocked, you need to add something like this to `gpg-agent.conf`:
 
 ```
```

